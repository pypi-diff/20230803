# Comparing `tmp/patroni-3.0.4.tar.gz` & `tmp/patroni-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patroni-3.0.4.tar", last modified: Thu Jul 13 10:23:00 2023, max compression
+gzip compressed data, was "patroni-3.1.0.tar", last modified: Thu Aug  3 11:37:51 2023, max compression
```

## Comparing `patroni-3.0.4.tar` & `patroni-3.1.0.tar`

### file list

```diff
@@ -1,97 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.144235 patroni-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 10:22:09.000000 patroni-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 10:22:09.000000 patroni-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-13 10:23:00.144235 patroni-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-13 10:22:09.000000 patroni-3.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.136235 patroni-3.0.4/patroni/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82325 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/async_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   101568 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/ctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/dcs/
--rw-r--r--   0 runner    (1001) docker     (123)    46802 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28670 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/consul.py
--rw-r--r--   0 runner    (1001) docker     (123)    38262 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/etcd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/exhibitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    63858 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/raft.py
--rw-r--r--   0 runner    (1001) docker     (123)    23478 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/zookeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   102190 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/ha.py
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)    60661 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/postgresql/available_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/available_parameters/0_postgres.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/callback_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/cancellable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/citus.py
--rw-r--r--   0 runner    (1001) docker     (123)    58301 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/postmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    27305 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/rewind.py
--rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/slots.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/psycopg.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/raft_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3234 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/scripts/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14799 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/scripts/wale_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    38723 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42892 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/watchdog/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/watchdog/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.136235 patroni-3.0.4/patroni.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 10:22:09.000000 patroni-3.0.4/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 10:22:09.000000 patroni-3.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:23:00.144235 patroni-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-13 10:22:09.000000 patroni-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.144235 patroni-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31056 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_async_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_callback_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_cancellable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_citus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_consul.py
--rw-r--r--   0 runner    (1001) docker     (123)    36966 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_ctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_etcd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_exhibitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    78993 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_ha.py
--rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_patroni.py
--rw-r--r--   0 runner    (1001) docker     (123)    46321 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_postmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_raft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_raft_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_rewind.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_wale_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_watchdog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_zookeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.746397 patroni-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 11:36:48.000000 patroni-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 11:36:48.000000 patroni-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-08-03 11:37:51.746397 patroni-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-08-03 11:36:48.000000 patroni-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.738397 patroni-3.1.0/patroni/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82693 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28244 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101516 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/ctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.738397 patroni-3.1.0/patroni/dcs/
+-rw-r--r--   0 runner    (1001) docker     (123)    54519 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28671 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39414 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/etcd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/exhibitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64700 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/raft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23478 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/dcs/zookeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/file_perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104536 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/ha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.742397 patroni-3.1.0/patroni/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)    60530 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.742397 patroni-3.1.0/patroni/postgresql/available_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/available_parameters/0_postgres.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/callback_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/cancellable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/citus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59748 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/postmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27309 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26945 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/postgresql/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/psycopg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/raft_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.742397 patroni-3.1.0/patroni/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3234 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/scripts/aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14799 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/scripts/wale_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38723 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.742397 patroni-3.1.0/patroni/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/watchdog/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-08-03 11:36:48.000000 patroni-3.1.0/patroni/watchdog/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.738397 patroni-3.1.0/patroni.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-08-03 11:37:51.000000 patroni-3.1.0/patroni.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-03 11:37:51.000000 patroni-3.1.0/patroni.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:37:51.000000 patroni-3.1.0/patroni.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-03 11:37:51.000000 patroni-3.1.0/patroni.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-03 11:37:51.000000 patroni-3.1.0/patroni.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 11:37:51.000000 patroni-3.1.0/patroni.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-03 11:36:48.000000 patroni-3.1.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 11:36:48.000000 patroni-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:37:51.746397 patroni-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-08-03 11:36:48.000000 patroni-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:37:51.746397 patroni-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31058 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_callback_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_cancellable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_citus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37222 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_ctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_etcd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_exhibitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_file_perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_ha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25930 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_patroni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46307 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_postmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_raft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_raft_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_rewind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_wale_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-08-03 11:36:48.000000 patroni-3.1.0/tests/test_zookeeper.py
```

### Comparing `patroni-3.0.4/LICENSE` & `patroni-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/PKG-INFO` & `patroni-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patroni
-Version: 3.0.4
+Version: 3.1.0
 Summary: PostgreSQL High-Available orchestrator and CLI
 Home-page: https://github.com/zalando/patroni
 Author: Alexander Kukushkin, Polina Bungina
 Author-email: akukushkin@microsoft.com, polina.bungina@zalando.de
 License: The MIT License
 Keywords: etcd governor patroni postgresql postgres ha haproxy confd zookeeper exhibitor consul streaming replication kubernetes k8s
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `patroni-3.0.4/README.rst` & `patroni-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/__init__.py` & `patroni-3.1.0/patroni/__init__.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/__main__.py` & `patroni-3.1.0/patroni/__main__.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/api.py` & `patroni-3.1.0/patroni/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,20 @@
         * ``patroni_postgres_server_version``: Postgres version without periods, e.g. ``150002`` for Postgres ``15.2``;
         * ``patroni_cluster_unlocked``: ``1`` if no one holds the leader lock, else ``0``;
         * ``patroni_failsafe_mode_is_active``: ``1`` if ``failsafe_mode`` is currently active, else ``0``;
         * ``patroni_postgres_timeline``: PostgreSQL timeline based on current WAL file name;
         * ``patroni_dcs_last_seen``: epoch timestamp when DCS was last contacted successfully;
         * ``patroni_pending_restart``: ``1`` if this PostgreSQL node is pending a restart, else ``0``;
         * ``patroni_is_paused``: ``1`` if Patroni is in maintenance node, else ``0``.
+
+        For PostgreSQL v9.6+ the response will also have the following:
+
+        * ``patroni_postgres_streaming``: 1 if Postgres is streaming from another node, else ``0``;
+        * ``patroni_postgres_in_archive_recovery``: ``1`` if Postgres isn't streaming and
+                                                    there is ``restore_command`` available, else ``0``.
         """
         postgres = self.get_postgresql_status(True)
         patroni = self.server.patroni
         epoch = datetime.datetime(1970, 1, 1, tzinfo=tzutc)
 
         metrics: List[str] = []
```

### Comparing `patroni-3.0.4/patroni/async_executor.py` & `patroni-3.1.0/patroni/async_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/collections.py` & `patroni-3.1.0/patroni/collections.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/config.py` & `patroni-3.1.0/patroni/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from copy import deepcopy
 from typing import Any, Callable, Collection, Dict, List, Optional, Union, TYPE_CHECKING
 
 from . import PATRONI_ENV_PREFIX
 from .collections import CaseInsensitiveDict
 from .dcs import ClusterConfig, Cluster
 from .exceptions import ConfigParseError
+from .file_perm import pg_perm
 from .postgresql.config import ConfigHandler
 from .utils import deep_compare, parse_bool, parse_int, patch_config
 
 logger = logging.getLogger(__name__)
 
 _AUTH_ALLOWED_PARAMETERS = (
     'username',
@@ -271,19 +272,21 @@
             except Exception:
                 logger.exception('Exception when loading file: %s', self._cache_file)
 
     def save_cache(self) -> None:
         if self._cache_needs_saving:
             tmpfile = fd = None
             try:
+                pg_perm.set_permissions_from_data_directory(self._data_dir)
                 (fd, tmpfile) = tempfile.mkstemp(prefix=self.__CACHE_FILENAME, dir=self._data_dir)
                 with os.fdopen(fd, 'w') as f:
                     fd = None
                     json.dump(self.dynamic_configuration, f)
                 tmpfile = shutil.move(tmpfile, self._cache_file)
+                os.chmod(self._cache_file, pg_perm.file_create_mode)
                 self._cache_needs_saving = False
             except Exception:
                 logger.exception('Exception when saving file: %s', self._cache_file)
                 if fd:
                     try:
                         os.close(fd)
                     except Exception:
@@ -325,17 +328,27 @@
                 else:
                     logger.info('No local configuration items changed.')
             except Exception:
                 logger.exception('Exception when reloading local configuration from %s', self.config_file)
 
     @staticmethod
     def _process_postgresql_parameters(parameters: Dict[str, Any], is_local: bool = False) -> Dict[str, Any]:
-        return {name: value for name, value in (parameters or {}).items()
-                if name not in ConfigHandler.CMDLINE_OPTIONS
-                or not is_local and ConfigHandler.CMDLINE_OPTIONS[name][1](value)}
+        pg_params: Dict[str, Any] = {}
+
+        for name, value in (parameters or {}).items():
+            if name not in ConfigHandler.CMDLINE_OPTIONS:
+                pg_params[name] = value
+            elif not is_local:
+                if ConfigHandler.CMDLINE_OPTIONS[name][1](value):
+                    pg_params[name] = value
+                else:
+                    logging.warning("postgresql parameter %s=%s failed validation, defaulting to %s",
+                                    name, value, ConfigHandler.CMDLINE_OPTIONS[name][0])
+
+        return pg_params
 
     def _safe_copy_dynamic_configuration(self, dynamic_configuration: Dict[str, Any]) -> Dict[str, Any]:
         config = deepcopy(self.__DEFAULT_CONFIG)
 
         for name, value in dynamic_configuration.items():
             if name == 'postgresql':
                 for name, value in (value or {}).items():
@@ -448,17 +461,18 @@
             ret: Dict[str, str] = {}
             for param in params or _AUTH_ALLOWED_PARAMETERS[:2]:
                 value = _popenv(name + '_' + param)
                 if value:
                     ret[param] = value
             return ret
 
-        restapi_auth = _get_auth('restapi')
-        if restapi_auth:
-            ret['restapi']['authentication'] = restapi_auth
+        for section in ('ctl', 'restapi'):
+            auth = _get_auth(section)
+            if auth:
+                ret[section]['authentication'] = auth
 
         authentication = {}
         for user_type in ('replication', 'superuser', 'rewind'):
             entry = _get_auth(user_type, _AUTH_ALLOWED_PARAMETERS)
             if entry:
                 authentication[user_type] = entry
 
@@ -470,15 +484,16 @@
                 # PATRONI_(ETCD|CONSUL|ZOOKEEPER|EXHIBITOR|...)_(HOSTS?|PORT|..)
                 name, suffix = (param[8:].split('_', 1) + [''])[:2]
                 if suffix in ('HOST', 'HOSTS', 'PORT', 'USE_PROXIES', 'PROTOCOL', 'SRV', 'SRV_SUFFIX', 'URL', 'PROXY',
                               'CACERT', 'CERT', 'KEY', 'VERIFY', 'TOKEN', 'CHECKS', 'DC', 'CONSISTENCY',
                               'REGISTER_SERVICE', 'SERVICE_CHECK_INTERVAL', 'SERVICE_CHECK_TLS_SERVER_NAME',
                               'SERVICE_TAGS', 'NAMESPACE', 'CONTEXT', 'USE_ENDPOINTS', 'SCOPE_LABEL', 'ROLE_LABEL',
                               'POD_IP', 'PORTS', 'LABELS', 'BYPASS_API_SERVICE', 'RETRIABLE_HTTP_CODES', 'KEY_PASSWORD',
-                              'USE_SSL', 'SET_ACLS', 'GROUP', 'DATABASE') and name:
+                              'USE_SSL', 'SET_ACLS', 'GROUP', 'DATABASE', 'LEADER_LABEL_VALUE', 'FOLLOWER_LABEL_VALUE',
+                              'STANDBY_LEADER_LABEL_VALUE', 'TMP_ROLE_LABEL') and name:
                     value = os.environ.pop(param)
                     if name == 'CITUS':
                         if suffix == 'GROUP':
                             value = parse_int(value)
                         elif suffix != 'DATABASE':
                             continue
                     elif suffix == 'PORT':
@@ -527,17 +542,18 @@
                     if name == 'parameters':
                         config['postgresql'][name].update(self._process_postgresql_parameters(value, True))
                     elif name != 'use_slots':  # replication slots must be enabled/disabled globally
                         config['postgresql'][name] = deepcopy(value)
             elif name not in config or name in ['watchdog']:
                 config[name] = deepcopy(value) if value else {}
 
-        # restapi server expects to get restapi.auth = 'username:password'
-        if 'restapi' in config and 'authentication' in config['restapi']:
-            config['restapi']['auth'] = '{username}:{password}'.format(**config['restapi']['authentication'])
+        # restapi server expects to get restapi.auth = 'username:password' and similarly for `ctl`
+        for section in ('ctl', 'restapi'):
+            if section in config and 'authentication' in config[section]:
+                config[section]['auth'] = '{username}:{password}'.format(**config[section]['authentication'])
 
         # special treatment for old config
 
         # 'exhibitor' inside 'zookeeper':
         if 'zookeeper' in config and 'exhibitor' in config['zookeeper']:
             config['exhibitor'] = config['zookeeper'].pop('exhibitor')
             config.pop('zookeeper')
```

### Comparing `patroni-3.0.4/patroni/ctl.py` & `patroni-3.1.0/patroni/ctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import time
 import yaml
 
 from collections import defaultdict
 from contextlib import contextmanager
 from prettytable import ALL, FRAME, PrettyTable
 from urllib.parse import urlparse
-from typing import Any, Dict, Generator, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING
+from typing import Any, Dict, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Cursor
     from psycopg2 import cursor
 
 try:
     from ydiff import markup_to_pager, PatchStream  # pyright: ignore [reportMissingModuleSource]
 except ImportError:  # pragma: no cover
@@ -250,23 +250,22 @@
 option_watch = click.option('-W', is_flag=True, help='Auto update the screen every 2 seconds')
 option_force = click.option('--force', is_flag=True, help='Do not ask for confirmation at any point')
 arg_cluster_name = click.argument('cluster_name', required=False,
                                   default=lambda: click.get_current_context().obj.get('scope'))
 option_default_citus_group = click.option('--group', required=False, type=int, help='Citus group',
                                           default=lambda: click.get_current_context().obj.get('citus', {}).get('group'))
 option_citus_group = click.option('--group', required=False, type=int, help='Citus group')
-option_insecure = click.option('-k', '--insecure', is_flag=True, help='Allow connections to SSL sites without certs')
 role_choice = click.Choice(['leader', 'primary', 'standby-leader', 'replica', 'standby', 'any', 'master'])
 
 
 @click.group(cls=click.Group)
 @click.option('--config-file', '-c', help='Configuration file',
               envvar='PATRONICTL_CONFIG_FILE', default=CONFIG_FILE_PATH)
 @click.option('--dcs-url', '--dcs', '-d', 'dcs_url', help='The DCS connect url', envvar='DCS_URL')
-@option_insecure
+@click.option('-k', '--insecure', is_flag=True, help='Allow connections to SSL sites without certs')
 @click.pass_context
 def ctl(ctx: click.Context, config_file: str, dcs_url: Optional[str], insecure: bool) -> None:
     """Entry point of ``patronictl`` utility.
 
     Load the configuration file.
 
     .. note::
@@ -1540,15 +1539,15 @@
 
     sort = topology_sort if fmt == 'topology' else iter
     for g, c in sorted(clusters.items()):
         for member in sort(c['members']):
             logging.debug(member)
 
             lag = member.get('lag', '')
-            member.update(c=name, member=member['name'], group=g,
+            member.update(cluster=name, member=member['name'], group=g,
                           host=member.get('host', ''), tl=member.get('timeline', ''),
                           role=member['role'].replace('_', ' ').title(),
                           lag_in_mb=round(lag / 1024 / 1024) if isinstance(lag, int) else lag,
                           pending_restart='*' if member.get('pending_restart') else '')
 
             if append_port and member['host'] and member.get('port'):
                 member['host'] = ':'.join([member['host'], str(member['port'])])
@@ -1813,15 +1812,15 @@
     :param group: filter which Citus group we should unpause. Refer to the module note for more details.
     :param wait: ``True`` if it should block until the operation is finished or ``false`` for returning immediately.
     """
     return toggle_pause(obj, cluster_name, group, False, wait)
 
 
 @contextmanager
-def temporary_file(contents: bytes, suffix: str = '', prefix: str = 'tmp') -> Generator[str, None, None]:
+def temporary_file(contents: bytes, suffix: str = '', prefix: str = 'tmp') -> Iterator[str]:
     """Create a temporary file with specified contents that persists for the context.
 
     :param contents: binary string that will be written to the file.
     :param prefix: will be prefixed to the filename.
     :param suffix: will be appended to the filename.
 
     :yields: path of the created file.
```

### Comparing `patroni-3.0.4/patroni/daemon.py` & `patroni-3.1.0/patroni/daemon.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/dcs/__init__.py` & `patroni-3.1.0/patroni/dcs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 import sys
 import time
 
 from collections import defaultdict
 from copy import deepcopy
 from random import randint
 from threading import Event, Lock
-from typing import Any, Callable, Collection, Dict, List, NamedTuple, Optional, Set, Tuple, Union, TYPE_CHECKING
+from types import ModuleType
+from typing import Any, Callable, Collection, Dict, List, NamedTuple, Optional, Set, Tuple, Union, TYPE_CHECKING, \
+    Type, Iterator
 from urllib.parse import urlparse, urlunparse, parse_qsl
 
 from ..exceptions import PatroniFatalException
 from ..utils import deep_compare, uri
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
@@ -81,68 +83,123 @@
             if hasattr(importer, 'toc'):
                 toc |= getattr(importer, 'toc')
         return [module for module in toc if module.startswith(module_prefix) and module.count('.') == 2]
     else:
         return [module_prefix + name for _, name, is_pkg in pkgutil.iter_modules([dcs_dirname]) if not is_pkg]
 
 
-def get_dcs(config: Union['Config', Dict[str, Any]]) -> 'AbstractDCS':
-    modules = dcs_modules()
+def iter_dcs_classes(
+        config: Optional[Union['Config', Dict[str, Any]]] = None
+) -> Iterator[Tuple[str, Type['AbstractDCS']]]:
+    """Attempt to import DCS modules that are present in the given configuration.
+
+    .. note::
+            If a module successfully imports we can assume that all its requirements are installed.
+
+    :param config: configuration information with possible DCS names as keys. If given, only attempt to import DCS
+                   modules defined in the configuration. Else, if ``None``, attempt to import any supported DCS module.
+
+    :yields: a tuple containing the module ``name`` and the imported DCS class object.
+    """
+    for mod_name in dcs_modules():
+        name = mod_name.rpartition('.')[2]
+        if config is None or name in config:
 
-    for module_name in modules:
-        name = module_name.split('.')[-1]
-        if name in config:  # we will try to import only modules which have configuration section in the config file
             try:
-                module = importlib.import_module(module_name)
-                for key, item in module.__dict__.items():  # iterate through the module content
-                    # try to find implementation of AbstractDCS interface, class name must match with module_name
-                    if key.lower() == name and inspect.isclass(item) and issubclass(item, AbstractDCS):
-                        # propagate some parameters
-                        config[name].update({p: config[p] for p in ('namespace', 'name', 'scope', 'loop_wait',
-                                             'patronictl', 'ttl', 'retry_timeout') if p in config})
-                        # From citus section we only need "group" parameter, but will propagate everything just in case.
-                        if isinstance(config.get('citus'), dict):
-                            config[name].update(config['citus'])
-                        return item(config[name])
+                module = importlib.import_module(mod_name)
+                dcs_module = find_dcs_class_in_module(module)
+                if dcs_module:
+                    yield name, dcs_module
+
             except ImportError:
-                logger.debug('Failed to import %s', module_name)
+                logger.log(logging.DEBUG if config is not None else logging.INFO,
+                           'Failed to import %s', mod_name)
 
-    available_implementations: List[str] = []
-    for module_name in modules:
-        name = module_name.split('.')[-1]
-        try:
-            module = importlib.import_module(module_name)
-            available_implementations.extend(name for key, item in module.__dict__.items() if key.lower() == name
-                                             and inspect.isclass(item) and issubclass(item, AbstractDCS))
-        except ImportError:
-            logger.info('Failed to import %s', module_name)
-    raise PatroniFatalException("""Can not find suitable configuration of distributed configuration store
-Available implementations: """ + ', '.join(sorted(set(available_implementations))))
+
+def find_dcs_class_in_module(module: ModuleType) -> Optional[Type['AbstractDCS']]:
+    """Try to find the implementation of :class:`AbstractDCS` interface in *module* matching the *module* name.
+
+    :param module: Imported DCS module.
+
+    :returns: class with a name matching the name of *module* that implements :class:`AbstractDCS` or ``None`` if not
+              found.
+    """
+    module_name = module.__name__.rpartition('.')[2]
+    return next(
+        (obj for obj_name, obj in module.__dict__.items()
+         if (obj_name.lower() == module_name
+             and inspect.isclass(obj) and issubclass(obj, AbstractDCS))),
+        None)
+
+
+def get_dcs(config: Union['Config', Dict[str, Any]]) -> 'AbstractDCS':
+    """Attempt to load a Distributed Configuration Store from known available implementations.
+
+    .. note::
+        Using the list of available DCS modules returned by :func:`iter_dcs_modules` attempt to dynamically import and
+        instantiate the class that implements a DCS using the abstract class :class:`AbstractDCS`.
+
+        Basic top-level configuration parameters retrieved from *config* are propagated to the DCS specific config
+        before being passed to the module DCS class.
+
+        If no module is found to satisfy configuration then report and log an error. This will cause Patroni to exit.
+
+    :raises :exc:`PatroniFatalException`: if a load of all available DCS modules have been tried and none succeeded.
+
+    :param config: object or dictionary with Patroni configuration. This is normally a representation of the main
+                   Patroni
+
+    :returns: The first successfully loaded DCS module which is an implementation of :class:`AbstractDCS`.
+    """
+    for name, dcs_class in iter_dcs_classes(config):
+        # Propagate some parameters from top level of config if defined to the DCS specific config section.
+        config[name].update({
+            p: config[p] for p in ('namespace', 'name', 'scope', 'loop_wait',
+                                   'patronictl', 'ttl', 'retry_timeout')
+            if p in config})
+        # From citus section we only need "group" parameter, but will propagate everything just in case.
+        if isinstance(config.get('citus'), dict):
+            config[name].update(config['citus'])
+        return dcs_class(config[name])
+
+    raise PatroniFatalException(
+        f"Can not find suitable configuration of distributed configuration store\n"
+        f"Available implementations: {', '.join(sorted([n for n, _ in iter_dcs_classes()]))}")
 
 
 _Version = Union[int, str]
 _Session = Union[int, float, str, None]
 
 
-class Member(NamedTuple):
+class Member(NamedTuple('Member',
+                        [('version', _Version),
+                         ('name', str),
+                         ('session', _Session),
+                         ('data', Dict[str, Any])])):
     """Immutable object (namedtuple) which represents single member of PostgreSQL cluster.
+
+    .. note::
+        We are using an old-style attribute declaration here because otherwise it is not possible to override
+        ``__new__`` method in the :class:`RemoteMember` class.
+
+    .. note::
+        These two keys in data are always written to the DCS, but care is taken to maintain consistency and resilience
+        from data that is read:
+
+        ``conn_url``: connection string containing host, user and password which could be used to access this member.
+        ``api_url``: REST API url of patroni instance
+
     Consists of the following fields:
-    :param version: modification version of a given member key in a Configuration Store
-    :param name: name of PostgreSQL cluster member
-    :param session: either session id or just ttl in seconds
-    :param data: arbitrary data i.e. conn_url, api_url, xlog location, state, role, tags, etc...
 
-    There are two mandatory keys in a data:
-    conn_url: connection string containing host, user and password which could be used to access this member.
-    api_url: REST API url of patroni instance
+    :ivar version: modification version of a given member key in a Configuration Store.
+    :ivar name: name of PostgreSQL cluster member.
+    :ivar session: either session id or just ttl in seconds.
+    :ivar data: dictionary containing arbitrary data i.e. ``conn_url``, ``api_url``, ``xlog_location``, ``state``,
+                ``role``, ``tags``, etc...
     """
-    version: _Version
-    name: str
-    session: _Session
-    data: Dict[str, Any]
 
     @staticmethod
     def from_node(version: _Version, name: str, session: _Session, value: str) -> 'Member':
         """
         >>> Member.from_node(-1, '', '', '{"conn_url": "postgres://foo@bar/postgres"}') is not None
         True
         >>> Member.from_node(-1, '', '', '{')
@@ -249,16 +306,22 @@
         'create_replica_methods',
         'restore_command',
         'archive_cleanup_command',
         'recovery_min_apply_delay',
         'no_replication_slot'
     )
 
-    @classmethod
-    def from_name_and_data(cls, name: str, data: Dict[str, Any]) -> 'RemoteMember':
+    def __new__(cls, name: str, data: Dict[str, Any]) -> 'RemoteMember':
+        """Factory method to construct instance from given *name* and *data*.
+
+        :param name: name of the remote member.
+        :param data: dictionary of member information.
+
+        :returns: constructed instance using supplied parameters.
+        """
         return super(RemoteMember, cls).__new__(cls, -1, name, None, data)
 
     def __getattr__(self, name: str) -> Any:
         if name in RemoteMember.ALLOWED_KEYS:
             return self.data.get(name)
 
 
@@ -504,44 +567,58 @@
             lines = json.loads(value)
             assert isinstance(lines, list)
         except (AssertionError, TypeError, ValueError):
             lines: List[_HistoryTuple] = []
         return TimelineHistory(version, value, lines)
 
 
-class Cluster(NamedTuple):
-    """Immutable object (namedtuple) which represents PostgreSQL cluster.
+class Cluster(NamedTuple('Cluster',
+                         [('initialize', Optional[str]),
+                          ('config', Optional[ClusterConfig]),
+                          ('leader', Optional[Leader]),
+                          ('last_lsn', int),
+                          ('members', List[Member]),
+                          ('failover', Optional[Failover]),
+                          ('sync', SyncState),
+                          ('history', Optional[TimelineHistory]),
+                          ('slots', Optional[Dict[str, int]]),
+                          ('failsafe', Optional[Dict[str, str]]),
+                          ('workers', Dict[int, 'Cluster'])])):
+    """Immutable object (namedtuple) which represents PostgreSQL or Citus cluster.
+
+    .. note::
+        We are using an old-style attribute declaration here because otherwise it is not possible to override `__new__`
+        method. Without it the *workers* by default gets always the same :class:`dict` object that could be mutated.
+
     Consists of the following fields:
-    :param initialize: shows whether this cluster has initialization key stored in DC or not.
-    :param config: global dynamic configuration, reference to `ClusterConfig` object
-    :param leader: `Leader` object which represents current leader of the cluster
-    :param last_lsn: int or long object containing position of last known leader LSN.
-        This value is stored in the `/status` key or `/optime/leader` (legacy) key
-    :param members: list of Member object, all PostgreSQL cluster members including leader
-    :param failover: reference to `Failover` object
-    :param sync: reference to `SyncState` object, last observed synchronous replication state.
-    :param history: reference to `TimelineHistory` object
-    :param slots: state of permanent logical replication slots on the primary in the format: {"slot_name": int}
-    :param failsafe: failsafe topology. Node is allowed to become the leader only if its name is found in this list.
-    :param workers: workers of the Citus cluster, optional. Format: {int(group): Cluster()}
+
+    :ivar initialize: shows whether this cluster has initialization key stored in DC or not.
+    :ivar config: global dynamic configuration, reference to `ClusterConfig` object.
+    :ivar leader: :class:`Leader` object which represents current leader of the cluster.
+    :ivar last_lsn: :class:int object containing position of last known leader LSN.
+                     This value is stored in the `/status` key or `/optime/leader` (legacy) key.
+    :ivar members: list of:class:` Member` objects, all PostgreSQL cluster members including leader
+    :ivar failover: reference to :class:`Failover` object.
+    :ivar sync: reference to :class:`SyncState` object, last observed synchronous replication state.
+    :ivar history: reference to `TimelineHistory` object.
+    :ivar slots: state of permanent logical replication slots on the primary in the format: {"slot_name": int}.
+    :ivar failsafe: failsafe topology. Node is allowed to become the leader only if its name is found in this list.
+    :ivar workers: dictionary of workers of the Citus cluster, optional. Each key is an :class:`int` representing
+                   the group, and the corresponding value is a :class:`Cluster` instance.
     """
-    initialize: Optional[str]
-    config: Optional[ClusterConfig]
-    leader: Optional[Leader]
-    last_lsn: int
-    members: List[Member]
-    failover: Optional[Failover]
-    sync: SyncState
-    history: Optional[TimelineHistory]
-    slots: Optional[Dict[str, int]]
-    failsafe: Optional[Dict[str, str]]
-    workers: Dict[int, 'Cluster'] = {}
+
+    def __new__(cls, *args: Any, **kwargs: Any):
+        """Make workers argument optional and set it to an empty dict object."""
+        if len(args) < len(cls._fields) and 'workers' not in kwargs:
+            kwargs['workers'] = {}
+        return super(Cluster, cls).__new__(cls, *args, **kwargs)
 
     @staticmethod
     def empty() -> 'Cluster':
+        """Produce an empty :class:`Cluster` instance."""
         return Cluster(None, None, None, 0, [], None, SyncState.empty(), None, None, None)
 
     def is_empty(self):
         return self.initialize is None and self.config is None and self.leader is None and self.last_lsn == 0\
             and self.members == [] and self.failover is None and self.sync.version is None\
             and self.history is None and self.slots is None and self.failsafe is None and self.workers == {}
 
@@ -582,44 +659,72 @@
 
     @property
     def use_slots(self) -> bool:
         return bool(self.config and (self.config.data.get('postgresql') or {}).get('use_slots', True))
 
     def get_replication_slots(self, my_name: str, role: str, nofailover: bool,
                               major_version: int, show_error: bool = False) -> Dict[str, Dict[str, Any]]:
-        # if the replicatefrom tag is set on the member - we should not create the replication slot for it on
-        # the current primary, because that member would replicate from elsewhere. We still create the slot if
-        # the replicatefrom destination member is currently not a member of the cluster (fallback to the
-        # primary), or if replicatefrom destination member happens to be the current primary
-        use_slots = self.use_slots
-        if role in ('master', 'primary', 'standby_leader'):
-            slot_members = [m.name for m in self.members if use_slots and m.name != my_name
-                            and (m.replicatefrom is None or m.replicatefrom == my_name
-                                 or not self.has_member(m.replicatefrom))]
-            permanent_slots = self.__permanent_slots if use_slots and \
-                role in ('master', 'primary') else self.__permanent_physical_slots
-        else:
-            # only manage slots for replicas that replicate from this one, except for the leader among them
-            slot_members = [m.name for m in self.members if use_slots
-                            and m.replicatefrom == my_name and m.name != self.leader_name]
-            permanent_slots = self.__permanent_logical_slots if use_slots and not nofailover else {}
+        """Lookup configured slot names in the DCS, report issues found and merge with permanent slots.
+
+        Will log an error if:
+
+            * Conflicting slot names between members are found
+            * Any logical slots are disabled, due to version compatibility, and *show_error* is ``True``.
+
+        :param my_name: name of this node.
+        :param role: role of this node.
+        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
+        :param major_version: postgresql major version.
+        :param show_error: if ``True`` report error if any disabled logical slots or conflicting slot names are found.
+
+        :returns: final dictionary of slot names, after merging with permanent slots and performing sanity checks.
+        """
+        slot_members: List[str] = self._get_slot_members(my_name, role) if self.use_slots else []
 
-        slots = {slot_name_from_member_name(name): {'type': 'physical'} for name in slot_members}
+        slots: Dict[str, Dict[str, str]] = {slot_name_from_member_name(name): {'type': 'physical'}
+                                            for name in slot_members}
 
         if len(slots) < len(slot_members):
             # Find which names are conflicting for a nicer error message
             slot_conflicts: Dict[str, List[str]] = defaultdict(list)
             for name in slot_members:
                 slot_conflicts[slot_name_from_member_name(name)].append(name)
             logger.error("Following cluster members share a replication slot name: %s",
-                         "; ".join("{} map to {}".format(", ".join(v), k)
+                         "; ".join(f"{', '.join(v)} map to {k}"
                                    for k, v in slot_conflicts.items() if len(v) > 1))
 
-        # "merge" replication slots for members with permanent_replication_slots
+        permanent_slots: dict[str, Any] = self._get_permanent_slots(role, nofailover) if self.use_slots else {}
+        disabled_permanent_logical_slots: List[str] = self._merge_permanent_slots(
+            slots, permanent_slots, my_name, major_version)
+
+        if disabled_permanent_logical_slots and show_error:
+            logger.error("Permanent logical replication slots supported by Patroni only starting from PostgreSQL 11. "
+                         "Following slots will not be created: %s.", disabled_permanent_logical_slots)
+
+        return slots
+
+    @staticmethod
+    def _merge_permanent_slots(slots: Dict[str, Dict[str, str]], permanent_slots: Dict[str, Any], my_name: str,
+                               major_version: int) -> List[str]:
+        """Merge replication *slots* for members with *permanent_slots*.
+
+        Perform validation of configured permanent slot name, skipping invalid names.
+
+        Will update *slots* in-line based on ``type`` of slot, ``physical`` or ``logical``, and name of node.
+        Type is assumed to be ``physical`` if there are no attributes stored as the slot value.
+
+        :param slots: Slot names with existing attributes if known.
+        :param my_name: name of this node.
+        :param permanent_slots: dictionary containing slot name key and slot information values.
+        :param major_version: postgresql major version.
+
+        :returns: List of disabled permanent, logical slot names, if postgresql version < 11.
+        """
         disabled_permanent_logical_slots: List[str] = []
+
         for name, value in permanent_slots.items():
             if not slot_name_re.match(name):
                 logger.error("Invalid permanent replication slot name '%s'", name)
                 logger.error("Slot name may only contain lower case letters, numbers, and the underscore chars")
                 continue
 
             value = deepcopy(value) if value else {'type': 'physical'}
@@ -628,31 +733,82 @@
                     value['type'] = 'logical' if value.get('database') and value.get('plugin') else 'physical'
 
                 if value['type'] == 'physical':
                     # Don't try to create permanent physical replication slot for yourself
                     if name != slot_name_from_member_name(my_name):
                         slots[name] = value
                     continue
-                elif value['type'] == 'logical' and value.get('database') and value.get('plugin'):
+
+                if value['type'] == 'logical' and value.get('database') and value.get('plugin'):
                     if major_version < 110000:
                         disabled_permanent_logical_slots.append(name)
                     elif name in slots:
                         logger.error("Permanent logical replication slot {'%s': %s} is conflicting with"
                                      " physical replication slot for cluster member", name, value)
                     else:
                         slots[name] = value
                     continue
 
             logger.error("Bad value for slot '%s' in permanent_slots: %s", name, permanent_slots[name])
+        return disabled_permanent_logical_slots
 
-        if disabled_permanent_logical_slots and show_error:
-            logger.error("Permanent logical replication slots supported by Patroni only starting from PostgreSQL 11. "
-                         "Following slots will not be created: %s.", disabled_permanent_logical_slots)
+    def _get_permanent_slots(self, role: str, nofailover: bool) -> Dict[str, Any]:
+        """Get configured permanent slot names.
 
-        return slots
+        .. note::
+            Permanent logical replication slots are only considered if ``use_slots`` configuration is enabled. Also,
+            only considered if *role* is ``primary`` or if it is a promotable ``replica`` -- what excludes a
+            ``standby_leader`` or ``replica`` with ``nofailover`` tag enabled. That combination is used for failing
+            over logical replication slots, and the latter nodes are not eligible for such task.
+
+            Permanent physical slots are only considered if *role* is ``primary`` or ``standby_leader``, independently
+            if ``use_slots`` is enabled or not. That is done that way because even if Patroni itself is not using slots
+            to replicate among its members when ``use_slots`` is disabled, the user may still have configured Patroni to
+            keep permanent physical slots used out of Patroni.
+
+        :param role: role of this node -- ``primary``, ``standby_leader`` or ``replica``.
+                     or logical slots being consumed.
+        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
+
+        :returns: dictionary of permanent slot names mapped to attributes.
+        """
+        if role in ('master', 'primary', 'standby_leader'):
+            permanent_slots = (self.__permanent_slots
+                               if role in ('master', 'primary')
+                               else self.__permanent_physical_slots)
+        else:
+            permanent_slots = self.__permanent_logical_slots if not nofailover else {}
+        return permanent_slots
+
+    def _get_slot_members(self, my_name: str, role: str) -> List[str]:
+        """Get a list of member names that have replication slots sourcing from this node.
+
+        If the ``replicatefrom`` tag is set on the member - we should not create the replication slot for it on
+        the current primary, because that member would replicate from elsewhere. We still create the slot if
+        the ``replicatefrom`` destination member is currently not a member of the cluster (fallback to the
+        primary), or if ``replicatefrom`` destination member happens to be the current primary.
+
+        :param my_name: name of this node.
+        :param role: role of this node, if this is a ``primary`` or ``standby_leader`` return list of members
+                     replicating from this node. If not then return a list of members replicating as cascaded
+                     replicas from this node.
+
+        :returns: list of member names.
+        """
+        if role in ('master', 'primary', 'standby_leader'):
+            slot_members = [m.name for m in self.members
+                            if m.name != my_name
+                            and (m.replicatefrom is None
+                                 or m.replicatefrom == my_name
+                                 or not self.has_member(m.replicatefrom))]
+        else:
+            # only manage slots for replicas that replicate from this one, except for the leader among them
+            slot_members = [m.name for m in self.members
+                            if m.replicatefrom == my_name and m.name != self.leader_name]
+        return slot_members
 
     def has_permanent_logical_slots(self, my_name: str, nofailover: bool, major_version: int = 110000) -> bool:
         if major_version < 110000:
             return False
         slots = self.get_replication_slots(my_name, 'replica', nofailover, major_version).values()
         return any(v for v in slots if v.get("type") == "logical")
 
@@ -903,15 +1059,17 @@
         try:
             cluster = self._get_citus_cluster() if self.is_citus_coordinator() else self.__get_patroni_cluster()
         except Exception:
             self.reset_cluster()
             raise
 
         self._last_seen = int(time.time())
-        self._last_status = {self._OPTIME: cluster.last_lsn, 'slots': cluster.slots}
+        self._last_status = {self._OPTIME: cluster.last_lsn}
+        if cluster.slots:
+            self._last_status['slots'] = cluster.slots
         self._last_failsafe = cluster.failsafe
 
         with self._cluster_thread_lock:
             self._cluster = cluster
             self._cluster_valid_till = time.time() + self.ttl
             return cluster
```

### Comparing `patroni-3.0.4/patroni/dcs/consul.py` & `patroni-3.1.0/patroni/dcs/consul.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from collections import defaultdict
 from consul import ConsulException, NotFound, base
 from http.client import HTTPException
 from urllib3.exceptions import HTTPError
 from urllib.parse import urlencode, urlparse, quote
 from typing import Any, Callable, Dict, List, Mapping, NamedTuple, Optional, Union, Tuple, TYPE_CHECKING
 
-from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, SyncState,\
+from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, SyncState, \
     TimelineHistory, ReturnFalseException, catch_return_false_exception, citus_group_re
 from ..exceptions import DCSError
 from ..utils import deep_compare, parse_bool, Retry, RetryFailedError, split_host_port, uri, USER_AGENT
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
```

### Comparing `patroni-3.0.4/patroni/dcs/etcd.py` & `patroni-3.1.0/patroni/dcs/etcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from queue import Queue
 from threading import Thread
 from typing import Any, Callable, Collection, Dict, List, Optional, Union, Tuple, Type, TYPE_CHECKING
 from urllib.parse import urlparse
 from urllib3 import Timeout
 from urllib3.exceptions import HTTPError, ReadTimeoutError, ProtocolError
 
-from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, SyncState,\
+from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, SyncState, \
     TimelineHistory, ReturnFalseException, catch_return_false_exception, citus_group_re
 from ..exceptions import DCSError
 from ..request import get as requests_get
 from ..utils import Retry, RetryFailedError, split_host_port, uri, USER_AGENT
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
```

### Comparing `patroni-3.0.4/patroni/dcs/etcd3.py` & `patroni-3.1.0/patroni/dcs/etcd3.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from collections import defaultdict
 from enum import IntEnum
 from urllib3.exceptions import ReadTimeoutError, ProtocolError
 from threading import Condition, Lock, Thread
 from typing import Any, Callable, Collection, Dict, Iterator, List, Optional, Tuple, Type, TYPE_CHECKING, Union
 
-from . import ClusterConfig, Cluster, Failover, Leader, Member, SyncState,\
+from . import ClusterConfig, Cluster, Failover, Leader, Member, SyncState, \
     TimelineHistory, catch_return_false_exception, citus_group_re
 from .etcd import AbstractEtcdClientWithFailover, AbstractEtcd, catch_etcd_errors, DnsCachingResolver, Retry
 from ..exceptions import DCSError, PatroniException
 from ..utils import deep_compare, enable_keepalive, iter_response_objects, RetryFailedError, USER_AGENT
 
 logger = logging.getLogger(__name__)
 
@@ -224,15 +224,15 @@
                          method: Optional[str] = None) -> Callable[..., urllib3.response.HTTPResponse]:
         if params is not None:
             kwargs['body'] = json.dumps(params)
             kwargs['headers']['Content-Type'] = 'application/json'
         return self.http.urlopen
 
     def _handle_server_response(self, response: urllib3.response.HTTPResponse) -> Dict[str, Any]:
-        data: Union[bytes, str] = response.data
+        data = response.data
         try:
             data = data.decode('utf-8')
             ret: Dict[str, Any] = json.loads(data)
             if response.status < 400:
                 return ret
         except (TypeError, ValueError, UnicodeError) as e:
             if response.status < 400:
@@ -626,14 +626,24 @@
                 value['mod_revision'] = ret['header']['revision']
                 self._kv_cache.set(value)
             elif delete and 'range_end' not in delete:
                 self._kv_cache.delete(delete['key'], ret['header']['revision'])
 
         return ret
 
+    def txn(self, compare: Dict[str, Any], success: Dict[str, Any],
+            failure: Optional[Dict[str, Any]] = None, retry: Optional[Retry] = None) -> Dict[str, Any]:
+        ret = super(PatroniEtcd3Client, self).txn(compare, success, failure, retry)
+        # Here we abuse the fact that the `failure` is only set in the call from update_leader().
+        # In all other cases the txn() call failure may be an indicator of a stale cache,
+        # and therefore we want to restart watcher.
+        if not failure and not ret:
+            self._restart_watcher()
+        return ret
+
 
 class Etcd3(AbstractEtcd):
 
     def __init__(self, config: Dict[str, Any]) -> None:
         super(Etcd3, self).__init__(config, PatroniEtcd3Client, (DeadlineExceeded, Unavailable, FailedPrecondition))
         self.__do_not_watch = False
         self._lease = None
```

### Comparing `patroni-3.0.4/patroni/dcs/exhibitor.py` & `patroni-3.1.0/patroni/dcs/exhibitor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/dcs/kubernetes.py` & `patroni-3.1.0/patroni/dcs/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from collections import defaultdict
 from copy import deepcopy
 from http.client import HTTPException
 from urllib3.exceptions import HTTPError
 from threading import Condition, Lock, Thread
 from typing import Any, Callable, Collection, Dict, List, Optional, Tuple, Type, Union, TYPE_CHECKING
 
-from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, SyncState,\
+from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, SyncState, \
     TimelineHistory, CITUS_COORDINATOR_GROUP_ID, citus_group_re
 from ..exceptions import DCSError
-from ..utils import deep_compare, iter_response_objects, keepalive_socket_options,\
+from ..utils import deep_compare, iter_response_objects, keepalive_socket_options, \
     Retry, RetryFailedError, tzutc, uri, USER_AGENT
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
 
 KUBE_CONFIG_DEFAULT_LOCATION = os.environ.get('KUBECONFIG', '~/.kube/config')
@@ -130,14 +130,16 @@
             self.pool_config[pool_key_name] = config[file_key_name]
 
     def load_kube_config(self, context: Optional[str] = None) -> None:
         with open(os.path.expanduser(KUBE_CONFIG_DEFAULT_LOCATION)) as f:
             config: Dict[str, Any] = yaml.safe_load(f)
 
         context = context or config['current-context']
+        if TYPE_CHECKING:  # pragma: no cover
+            assert isinstance(context, str)
         context_value = self._get_by_name(config, 'context', context)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(context_value, dict)
         cluster = self._get_by_name(config, 'cluster', context_value['cluster'])
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(cluster, dict)
         user = self._get_by_name(config, 'user', context_value['user'])
@@ -748,14 +750,18 @@
 
     def __init__(self, config: Dict[str, Any]) -> None:
         self._labels = deepcopy(config['labels'])
         self._labels[config.get('scope_label', 'cluster-name')] = config['scope']
         self._label_selector = ','.join('{0}={1}'.format(k, v) for k, v in self._labels.items())
         self._namespace = config.get('namespace') or 'default'
         self._role_label = config.get('role_label', 'role')
+        self._leader_label_value = config.get('leader_label_value', 'master')
+        self._follower_label_value = config.get('follower_label_value', 'replica')
+        self._standby_leader_label_value = config.get('standby_leader_label_value', 'standby-leader')
+        self._tmp_role_label = config.get('tmp_role_label')
         self._ca_certs = os.environ.get('PATRONI_KUBERNETES_CACERT', config.get('cacert')) or SERVICE_CERT_FILENAME
         super(Kubernetes, self).__init__({**config, 'namespace': ''})
         if self._citus_group:
             self._labels[self._CITUS_LABEL] = self._citus_group
 
         self._retry = Retry(deadline=config['retry_timeout'], max_delay=1, max_tries=-1,
                             retry_exceptions=KubernetesRetriableException)
@@ -1259,27 +1265,38 @@
     def set_config_value(self, value: str, version: Optional[str] = None) -> bool:
         return self.patch_or_create_config({self._CONFIG: value}, version, bool(self._config_resource_version), False)
 
     @catch_kubernetes_errors
     def touch_member(self, data: Dict[str, Any]) -> bool:
         cluster = self.cluster
         if cluster and cluster.leader and cluster.leader.name == self._name:
-            role = 'master'
+            role = self._leader_label_value
+            tmp_role = 'master'
         elif data['state'] == 'running' and data['role'] not in ('master', 'primary'):
-            role = data['role']
+            role = {
+                'replica': self._follower_label_value,
+                'standby-leader': self._standby_leader_label_value,
+            }.get(data['role'], data['role'])
+            tmp_role = data['role']
         else:
             role = None
+            tmp_role = None
+
+        role_labels = {self._role_label: role}
+        if self._tmp_role_label:
+            role_labels[self._tmp_role_label] = tmp_role
 
         member = cluster and cluster.get_member(self._name, fallback_to_leader=False)
         pod_labels = member and member.data.pop('pod_labels', None)
         ret = member and pod_labels is not None\
-            and pod_labels.get(self._role_label) == role and deep_compare(data, member.data)
+            and all(pod_labels.get(k) == v for k, v in role_labels.items())\
+            and deep_compare(data, member.data)
 
         if not ret:
-            metadata = {'namespace': self._namespace, 'name': self._name, 'labels': {self._role_label: role},
+            metadata = {'namespace': self._namespace, 'name': self._name, 'labels': role_labels,
                         'annotations': {'status': json.dumps(data, separators=(',', ':'))}}
             body = k8s_client.V1Pod(metadata=k8s_client.V1ObjectMeta(**metadata))
             ret = self._api.patch_namespaced_pod(self._name, self._namespace, body)
             if ret:
                 self._pods.set(self._name, ret)
         if self._should_create_config_service:
             self._create_config_service()
```

### Comparing `patroni-3.0.4/patroni/dcs/raft.py` & `patroni-3.1.0/patroni/dcs/raft.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/dcs/zookeeper.py` & `patroni-3.1.0/patroni/dcs/zookeeper.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/exceptions.py` & `patroni-3.1.0/patroni/exceptions.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/ha.py` & `patroni-3.1.0/patroni/ha.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         :param member: dcs.Member object
         :param json: RestApiHandler.get_postgresql_status() result
         :returns: _MemberStatus object
         """
         # If one of those is not in a response we want to count the node as not healthy/reachable
         wal: Dict[str, Any] = json.get('wal') or json['xlog']
         # abuse difference in primary/replica response format
-        in_recovery = not bool(wal.get('location')) or json.get('role') in ('master', 'primary')
+        in_recovery = not (bool(wal.get('location')) or json.get('role') in ('master', 'primary'))
         timeline = json.get('timeline', 0)
         dcs_last_seen = json.get('dcs_last_seen', 0)
         lsn = int(in_recovery and max(wal.get('received_location', 0), wal.get('replayed_location', 0)))
         return cls(member, True, in_recovery, dcs_last_seen, timeline, lsn,
                    json.get('tags', {}), json.get('watchdog_failed', False))
 
     @classmethod
@@ -97,17 +97,17 @@
             self._api_url = data['api_url']
             self._slots = data.get('slots')
 
     @property
     def leader(self) -> Optional[Leader]:
         with self._lock:
             if self._last_update + self._dcs.ttl > time.time() and self._name:
-                return Leader('', '', RemoteMember.from_name_and_data(self._name, {'api_url': self._api_url,
-                                                                                   'conn_url': self._conn_url,
-                                                                                   'slots': self._slots}))
+                return Leader('', '', RemoteMember(self._name, {'api_url': self._api_url,
+                                                                'conn_url': self._conn_url,
+                                                                'slots': self._slots}))
 
     def update_cluster(self, cluster: Cluster) -> Cluster:
         # Enreach cluster with the real leader if there was a ping from it
         leader = self.leader
         if leader:
             # We rely on the strict order of fields in the namedtuple
             cluster = Cluster(*cluster[0:2], leader, *cluster[3:8], leader.member.data['slots'], *cluster[9:])
@@ -469,15 +469,16 @@
             timeout = None
 
         data = self.state_handler.controldata()
         logger.info('pg_controldata:\n%s\n', '\n'.join('  {0}: {1}'.format(k, v) for k, v in data.items()))
 
         # timeout > 0 indicates that we still have the leader lock, and it was just updated
         if timeout\
-                and data.get('Database cluster state') in ('in production', 'shutting down', 'shut down')\
+                and data.get('Database cluster state') in ('in production', 'in crash recovery',
+                                                           'shutting down', 'shut down')\
                 and self.state_handler.state == 'crashed'\
                 and self.state_handler.role in ('primary', 'master')\
                 and not self.state_handler.config.recovery_conf_exists():
             # We know 100% that we were running as a primary a few moments ago, therefore could just start postgres
             msg = 'starting primary after failure'
             if self._async_executor.try_run_async(msg, self.state_handler.start,
                                                   args=(timeout, self._async_executor.critical_task)) is None:
@@ -492,14 +493,15 @@
             if msg:
                 return msg
 
         self.load_cluster_from_dcs()
 
         role = 'replica'
         if self.has_lock() and not self.is_standby_cluster():
+            self._rewind.reset_state()  # we want to later trigger CHECKPOINT after promote
             msg = "starting as readonly because i had the session lock"
             node_to_follow = None
         else:
             if not self._rewind.executed:
                 self._rewind.trigger_check_diverged_lsn()
             msg = self._handle_rewind_or_reinitialize()
             if msg:
@@ -521,18 +523,25 @@
 
         if self._async_executor.try_run_async('restarting after failure', self.state_handler.follow,
                                               args=(node_to_follow, role, timeout)) is None:
             self.recovering = True
         return msg
 
     def _get_node_to_follow(self, cluster: Cluster) -> Union[Leader, Member, None]:
-        # determine the node to follow. If replicatefrom tag is set,
-        # try to follow the node mentioned there, otherwise, follow the leader.
-        if self.is_standby_cluster() and (self.cluster.is_unlocked() or self.has_lock(False)):
+        """Determine the node to follow.
+
+        :param cluster: the currently known cluster state from DCS.
+
+        :returns: the node which we should be replicating from.
+        """
+        # The standby leader or when there is no standby leader we want to follow
+        # the remote member, except when there is no standby leader in pause.
+        if self.is_standby_cluster() and (self.has_lock(False) or self.cluster.is_unlocked() and not self.is_paused()):
             node_to_follow = self.get_remote_member()
+        # If replicatefrom tag is set, try to follow the node mentioned there, otherwise, follow the leader.
         elif self.patroni.replicatefrom and self.patroni.replicatefrom != self.state_handler.name:
             node_to_follow = cluster.get_member(self.patroni.replicatefrom)
         else:
             node_to_follow = cluster.leader if cluster.leader and cluster.leader.name else None
 
         node_to_follow = node_to_follow if node_to_follow and node_to_follow.name != self.state_handler.name else None
 
@@ -764,26 +773,22 @@
                 if not self.dcs.write_sync_state(self.state_handler.name, None, version=self.cluster.sync.version):
                     # Somebody else updated sync state, it may be due to us losing the lock. To be safe, postpone
                     # promotion until next cycle. TODO: trigger immediate retry of run_cycle
                     return 'Postponing promotion because synchronous replication state was updated by somebody else'
                 self.state_handler.sync_handler.set_synchronous_standby_names(
                     CaseInsensitiveSet('*') if self.global_config.is_synchronous_mode_strict else CaseInsensitiveSet())
             if self.state_handler.role not in ('master', 'promoted', 'primary'):
-                def on_success():
-                    self._rewind.reset_state()
-                    logger.info("cleared rewind state after becoming the leader")
-
                 def before_promote():
                     self.notify_citus_coordinator('before_promote')
 
                 with self._async_response:
                     self._async_response.reset()
+
                 self._async_executor.try_run_async('promote', self.state_handler.promote,
-                                                   args=(self.dcs.loop_wait, self._async_response,
-                                                         before_promote, on_success))
+                                                   args=(self.dcs.loop_wait, self._async_response, before_promote))
             return promote_message
 
     def fetch_node_status(self, member: Member) -> _MemberStatus:
         """This function perform http get request on member.api_url and fetches its status
         :returns: `_MemberStatus` object
         """
 
@@ -830,15 +835,15 @@
             'conn_url': self.state_handler.connection_string,
             'api_url': self.patroni.api.connection_string,
         }
         try:
             data['slots'] = self.state_handler.slots()
         except Exception:
             logger.exception('Exception when called state_handler.slots()')
-        members = [RemoteMember.from_name_and_data(name, {'api_url': url})
+        members = [RemoteMember(name, {'api_url': url})
                    for name, url in failsafe.items() if name != self.state_handler.name]
         if not members:  # A sinlge node cluster
             return True
         pool = ThreadPool(len(members))
         call_failsafe_member = functools.partial(self.call_failsafe_member, data)
         results = pool.map(call_failsafe_member, members)
         pool.close()
@@ -994,17 +999,30 @@
         if self.is_paused() and not self.patroni.nofailover and \
                 self.cluster.failover and not self.cluster.failover.scheduled_at:
             ret = self.manual_failover_process_no_leader()
             if ret is not None:  # continue if we just deleted the stale failover key as a leader
                 return ret
 
         if self.state_handler.is_leader():
-            # in pause leader is the healthiest only when no initialize or sysid matches with initialize!
-            return not self.is_paused() or not self.cluster.initialize\
-                or self.state_handler.sysid == self.cluster.initialize
+            if self.is_paused():
+                # in pause leader is the healthiest only when no initialize or sysid matches with initialize!
+                return not self.cluster.initialize or self.state_handler.sysid == self.cluster.initialize
+
+            # We want to protect from the following scenario:
+            # 1. node1 is stressed so much that heart-beat isn't running regularly and the leader lock expires.
+            # 2. node2 promotes, gets heavy load and the situation described in 1 repeats.
+            # 3. Patroni on node1 comes back, notices that Postgres is running as primary but there is
+            #    no leader key and "happily" acquires the leader lock.
+            # That is, node1 discarded promotion of node2. To avoid it we want to detect timeline change.
+            my_timeline = self.state_handler.get_primary_timeline()
+            if my_timeline < self.cluster.timeline:
+                logger.warning('My timeline %s is behind last known cluster timeline %s',
+                               my_timeline, self.cluster.timeline)
+                return False
+            return True
 
         if self.is_paused():
             return False
 
         if self.patroni.nofailover:  # nofailover tag makes node always unhealthy
             return False
 
@@ -1024,16 +1042,15 @@
             failsafe_members = self.dcs.failsafe
             # We want to discard failsafe_mode if the /failsafe key contains garbage or empty.
             if isinstance(failsafe_members, dict):
                 # If current node is missing in the /failsafe key we immediately disqualify it from the race.
                 if failsafe_members and self.state_handler.name not in failsafe_members:
                     return False
                 # Race among not only existing cluster members, but also all known members from the failsafe config
-                all_known_members += [RemoteMember.from_name_and_data(name, {'api_url': url})
-                                      for name, url in failsafe_members.items()]
+                all_known_members += [RemoteMember(name, {'api_url': url}) for name, url in failsafe_members.items()]
         all_known_members += self.cluster.members
 
         # When in sync mode, only last known primary and sync standby are allowed to promote automatically.
         if self.is_synchronous_mode() and not self.cluster.sync.is_empty:
             if not self.cluster.sync.matches(self.state_handler.name, True):
                 return False
             # pick between synchronous candidates so we minimize unnecessary failovers/demotions
@@ -1080,15 +1097,17 @@
         status = {'released': False}
 
         def on_shutdown(checkpoint_location: int) -> None:
             # Postmaster is still running, but pg_control already reports clean "shut down".
             # It could happen if Postgres is still archiving the backlog of WAL files.
             # If we know that there are replicas that received the shutdown checkpoint
             # location, we can remove the leader key and allow them to start leader race.
-            if self.is_failover_possible(self.cluster.members, cluster_lsn=checkpoint_location):
+
+            # for a manual failover/switchover with a candidate, we should check the requested candidate only
+            if self.is_failover_possible(self.get_failover_candidates(), cluster_lsn=checkpoint_location):
                 self.state_handler.set_role('demoted')
                 with self._async_executor:
                     self.release_leader_key_voluntarily(checkpoint_location)
                     status['released'] = True
 
         def before_shutdown() -> None:
             if self.state_handler.citus_handler.is_coordinator():
@@ -1184,23 +1203,20 @@
 
         if not failover.leader or failover.leader == self.state_handler.name:
             if not failover.candidate or failover.candidate != self.state_handler.name:
                 if not failover.candidate and self.is_paused():
                     logger.warning('Failover is possible only to a specific candidate in a paused state')
                 else:
                     if self.is_synchronous_mode():
-                        if failover.candidate and not self.cluster.sync.matches(failover.candidate):
+                        members = self.get_failover_candidates(check_sync=True)
+                        if failover.candidate and not members:
                             logger.warning('Failover candidate=%s does not match with sync_standbys=%s',
                                            failover.candidate, self.cluster.sync.sync_standby)
-                            members = []
-                        else:
-                            members = [m for m in self.cluster.members if self.cluster.sync.matches(m.name)]
                     else:
-                        members = [m for m in self.cluster.members
-                                   if not failover.candidate or m.name == failover.candidate]
+                        members = self.get_failover_candidates()
                     if self.is_failover_possible(members, False):  # check that there are healthy members
                         ret = self._async_executor.try_run_async('manual failover: demote', self.demote, ('graceful',))
                         return ret or 'manual failover: demoting myself'
                     else:
                         logger.warning('manual failover: no healthy members found, failover is not possible')
             else:
                 logger.warning('manual failover: I am already the leader, no need to failover')
@@ -1610,14 +1626,17 @@
 
             if self.is_paused():
                 self.watchdog.disable()
                 self._was_paused = True
             else:
                 if self._was_paused:
                     self.state_handler.schedule_sanity_checks_after_pause()
+                    # during pause people could manually do something with Postgres, therefore we want
+                    # to double check rewind conditions on replicas and maybe run CHECKPOINT on the primary
+                    self._rewind.reset_state()
                 self._was_paused = False
 
             if not self.cluster.has_member(self.state_handler.name):
                 self.touch_member()
 
             # cluster has leader key but not initialize key
             if not (self.cluster.is_unlocked() or self.sysid_valid(self.cluster.initialize)) and self.has_lock():
@@ -1844,15 +1863,17 @@
 
             def _on_shutdown(checkpoint_location: int) -> None:
                 if self.is_leader():
                     # Postmaster is still running, but pg_control already reports clean "shut down".
                     # It could happen if Postgres is still archiving the backlog of WAL files.
                     # If we know that there are replicas that received the shutdown checkpoint
                     # location, we can remove the leader key and allow them to start leader race.
-                    if self.is_failover_possible(self.cluster.members, cluster_lsn=checkpoint_location):
+
+                    # for a manual failover/switchover with a candidate, we should check the requested candidate only
+                    if self.is_failover_possible(self.get_failover_candidates(), cluster_lsn=checkpoint_location):
                         self.dcs.delete_leader(checkpoint_location)
                         status['deleted'] = True
                     else:
                         self.dcs.write_leader_optime(checkpoint_location)
 
             def _before_shutdown() -> None:
                 self.notify_citus_coordinator('before_demote')
@@ -1903,8 +1924,29 @@
             data['no_replication_slot'] = 'primary_slot_name' not in cluster_params
             conn_kwargs = member.conn_kwargs() if member else \
                 {k: cluster_params[k] for k in ('host', 'port') if k in cluster_params}
             if conn_kwargs:
                 data['conn_kwargs'] = conn_kwargs
 
         name = member.name if member else 'remote_member:{}'.format(uuid.uuid1())
-        return RemoteMember.from_name_and_data(name, data)
+        return RemoteMember(name, data)
+
+    def get_failover_candidates(self, check_sync: bool = False) -> List[Member]:
+        """Return list of candidates for either manual or automatic failover.
+
+        Mainly used to later be passed to ``Ha.is_failover_possible()``.
+
+        :param check_sync: if ``True``, also check against the sync key members
+
+        :returns: a list of ``Member`` ojects or an empty list if there is no candidate available
+        """
+        failover = self.cluster.failover
+        if check_sync:
+            # TODO: allow manual failover (=no leader specified) to async node
+            # every sync_standby or the candidate specified if is in sync_standbys
+            return [m for m in self.cluster.members
+                    if self.cluster.sync.matches(m.name)
+                    and (not failover or not failover.candidate or m.name == failover.candidate)]
+        else:
+            # every member or the candidate specified
+            return [m for m in self.cluster.members
+                    if not failover or not failover.candidate or m.name == failover.candidate]
```

### Comparing `patroni-3.0.4/patroni/log.py` & `patroni-3.1.0/patroni/log.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/__init__.py` & `patroni-3.1.0/patroni/postgresql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from contextlib import contextmanager
 from copy import deepcopy
 from datetime import datetime
 from dateutil import tz
 from psutil import TimeoutExpired
 from threading import current_thread, Lock
-from typing import Any, Callable, Dict, Generator, List, Optional, Union, Tuple, TYPE_CHECKING
+from typing import Any, Callable, Dict, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING
 
 from .bootstrap import Bootstrap
 from .callback_executor import CallbackAction, CallbackExecutor
 from .cancellable import CancellableSubprocess
 from .config import ConfigHandler, mtime
 from .connection import Connection, get_connection_cursor
 from .citus import CitusHandler
@@ -995,15 +995,15 @@
             return out, err
         except Exception as e:
             logger.error('Failed to execute `%s -t %s -s %s -n %s`: %r', cmd, timeline, lsn, limit, e)
             return None, None
 
     @contextmanager
     def get_replication_connection_cursor(self, host: Optional[str] = None, port: int = 5432,
-                                          **kwargs: Any) -> Generator[Union['cursor', 'Cursor[Any]'], None, None]:
+                                          **kwargs: Any) -> Iterator[Union['cursor', 'Cursor[Any]']]:
         conn_kwargs = self.config.replication.copy()
         conn_kwargs.update(host=host, port=int(port) if port else None, user=conn_kwargs.pop('username'),
                            connect_timeout=3, replication=1, options='-c statement_timeout=2000')
         with get_connection_cursor(**conn_kwargs) as cur:
             yield cur
 
     def get_replica_timeline(self) -> Optional[int]:
@@ -1121,16 +1121,16 @@
         try:
             ret = self.cancellable.call(shlex.split(cmd))
             if ret is not None:
                 logger.info('before_stop script `%s` exited with %s', cmd, ret)
         except Exception as e:
             logger.error('Exception when calling `%s`: %r', cmd, e)
 
-    def promote(self, wait_seconds: int, task: CriticalTask, before_promote: Optional[Callable[..., Any]] = None,
-                on_success: Optional[Callable[..., Any]] = None) -> Optional[bool]:
+    def promote(self, wait_seconds: int, task: CriticalTask,
+                before_promote: Optional[Callable[..., Any]] = None) -> Optional[bool]:
         if self.role in ('promoted', 'master', 'primary'):
             return True
 
         ret = self._pre_promote()
         with task:
             if task.is_cancelled:
                 return False
@@ -1148,16 +1148,14 @@
 
         self.slots_handler.on_promote()
         self.citus_handler.schedule_cache_rebuild()
 
         ret = self.pg_ctl('promote', '-W')
         if ret:
             self.set_role('promoted')
-            if on_success is not None:
-                on_success()
             self.call_nowait(CallbackAction.ON_ROLE_CHANGE)
             ret = self._wait_promote(wait_seconds)
         return ret
 
     @staticmethod
     def _wal_position(is_leader: bool, wal_position: int,
                       received_location: Optional[int], replayed_location: Optional[int]) -> int:
```

### Comparing `patroni-3.0.4/patroni/postgresql/available_parameters/0_postgres.yml` & `patroni-3.1.0/patroni/postgresql/available_parameters/0_postgres.yml`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/bootstrap.py` & `patroni-3.1.0/patroni/postgresql/bootstrap.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/callback_executor.py` & `patroni-3.1.0/patroni/postgresql/callback_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/cancellable.py` & `patroni-3.1.0/patroni/postgresql/cancellable.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/citus.py` & `patroni-3.1.0/patroni/postgresql/citus.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/config.py` & `patroni-3.1.0/patroni/postgresql/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import os
 import re
 import shutil
 import socket
 import stat
 import time
 
+from contextlib import contextmanager
 from urllib.parse import urlparse, parse_qsl, unquote
 from types import TracebackType
-from typing import Any, Collection, Dict, List, Optional, Union, Tuple, Type, TYPE_CHECKING
+from typing import Any, Collection, Dict, Iterator, List, Optional, Union, Tuple, Type, TYPE_CHECKING
 
 from .validator import recovery_parameters, transform_postgresql_parameter_value, transform_recovery_parameter_value
 from ..collections import CaseInsensitiveDict, CaseInsensitiveSet
 from ..dcs import Leader, Member, RemoteMember, slot_name_from_member_name
 from ..exceptions import PatroniFatalException
+from ..file_perm import pg_perm
 from ..utils import compare_values, parse_bool, parse_int, split_host_port, uri, validate_directory, is_subpath
-from ..validator import IntValidator
+from ..validator import IntValidator, EnumValidator
 
 if TYPE_CHECKING:  # pragma: no cover
     from . import Postgresql
 
 logger = logging.getLogger(__name__)
 
 PARAMETER_RE = re.compile(r'([a-z_]+)\s*=\s*')
@@ -254,22 +256,22 @@
         self.writeline("{0} = '{1}'".format(param, self.escape(value)))
 
 
 def _false_validator(value: Any) -> bool:
     return False
 
 
-def _wal_level_validator(value: Any) -> bool:
-    return str(value).lower() in ('hot_standby', 'replica', 'logical')
-
-
 def _bool_validator(value: Any) -> bool:
     return parse_bool(value) is not None
 
 
+def _bool_is_true_validator(value: Any) -> bool:
+    return parse_bool(value) is True
+
+
 class ConfigHandler(object):
 
     # List of parameters which must be always passed to postmaster as command line options
     # to make it not possible to change them with 'ALTER SYSTEM'.
     # Some of these parameters have sane default value assigned and Patroni doesn't allow
     # to decrease this value. E.g. 'wal_level' can't be lower then 'hot_standby' and so on.
     # These parameters could be changed only globally, i.e. via DCS.
@@ -282,26 +284,26 @@
     #    default_value -- some sane default value
     #    check_function -- if the new value is not correct must return `!False`
     #    min_version -- major version of PostgreSQL when parameter was introduced
     CMDLINE_OPTIONS = CaseInsensitiveDict({
         'listen_addresses': (None, _false_validator, 90100),
         'port': (None, _false_validator, 90100),
         'cluster_name': (None, _false_validator, 90500),
-        'wal_level': ('hot_standby', _wal_level_validator, 90100),
-        'hot_standby': ('on', _false_validator, 90100),
+        'wal_level': ('hot_standby', EnumValidator(('hot_standby', 'replica', 'logical')), 90100),
+        'hot_standby': ('on', _bool_is_true_validator, 90100),
         'max_connections': (100, IntValidator(min=25), 90100),
         'max_wal_senders': (10, IntValidator(min=3), 90100),
         'wal_keep_segments': (8, IntValidator(min=1), 90100),
         'wal_keep_size': ('128MB', IntValidator(min=16, base_unit='MB'), 130000),
         'max_prepared_transactions': (0, IntValidator(min=0), 90100),
         'max_locks_per_transaction': (64, IntValidator(min=32), 90100),
         'track_commit_timestamp': ('off', _bool_validator, 90500),
         'max_replication_slots': (10, IntValidator(min=4), 90400),
         'max_worker_processes': (8, IntValidator(min=2), 90400),
-        'wal_log_hints': ('on', _false_validator, 90400)
+        'wal_log_hints': ('on', _bool_is_true_validator, 90400)
     })
 
     _RECOVERY_PARAMETERS = CaseInsensitiveSet(recovery_parameters.keys())
 
     def __init__(self, postgresql: 'Postgresql', config: Dict[str, Any]) -> None:
         self._postgresql = postgresql
         self._config_dir = os.path.abspath(config.get('config_dir', '') or postgresql.data_dir)
@@ -363,57 +365,84 @@
             configuration.append(os.path.basename(self._postgresql_base_conf_name))
         if not self.hba_file:
             configuration.append('pg_hba.conf')
         if not self.ident_file:
             configuration.append('pg_ident.conf')
         return configuration
 
+    def set_file_permissions(self, filename: str) -> None:
+        """Set permissions of file *filename* according to the expected permissions if it resides under PGDATA.
+
+        .. note::
+            Do nothing if the file is not under PGDATA.
+
+        :param filename: path to a file which permissions might need to be adjusted.
+        """
+        if is_subpath(self._postgresql.data_dir, filename):
+            pg_perm.set_permissions_from_data_directory(self._postgresql.data_dir)
+            os.chmod(filename, pg_perm.file_create_mode)
+
+    @contextmanager
+    def config_writer(self, filename: str) -> Iterator[ConfigWriter]:
+        """Create :class:`ConfigWriter` object and set permissions on a *filename*.
+
+        :param filename: path to a config file.
+
+        :yields: :class:`ConfigWriter` object.
+        """
+        with ConfigWriter(filename) as writer:
+            yield writer
+        self.set_file_permissions(filename)
+
     def save_configuration_files(self, check_custom_bootstrap: bool = False) -> bool:
         """
             copy postgresql.conf to postgresql.conf.backup to be able to retrieve configuration files
             - originally stored as symlinks, those are normally skipped by pg_basebackup
             - in case of WAL-E basebackup (see http://comments.gmane.org/gmane.comp.db.postgresql.wal-e/239)
         """
         if not (check_custom_bootstrap and self._postgresql.bootstrap.running_custom_bootstrap):
             try:
                 for f in self._configuration_to_save:
                     config_file = os.path.join(self._config_dir, f)
                     backup_file = os.path.join(self._postgresql.data_dir, f + '.backup')
                     if os.path.isfile(config_file):
                         shutil.copy(config_file, backup_file)
+                        self.set_file_permissions(backup_file)
             except IOError:
                 logger.exception('unable to create backup copies of configuration files')
         return True
 
     def restore_configuration_files(self) -> None:
         """ restore a previously saved postgresql.conf """
         try:
             for f in self._configuration_to_save:
                 config_file = os.path.join(self._config_dir, f)
                 backup_file = os.path.join(self._postgresql.data_dir, f + '.backup')
                 if not os.path.isfile(config_file):
                     if os.path.isfile(backup_file):
                         shutil.copy(backup_file, config_file)
+                        self.set_file_permissions(config_file)
                     # Previously we didn't backup pg_ident.conf, if file is missing just create empty
                     elif f == 'pg_ident.conf':
                         open(config_file, 'w').close()
+                        self.set_file_permissions(config_file)
         except IOError:
             logger.exception('unable to restore configuration files from backup')
 
     def write_postgresql_conf(self, configuration: Optional[CaseInsensitiveDict] = None) -> None:
         # rename the original configuration if it is necessary
         if 'custom_conf' not in self._config and not os.path.exists(self._postgresql_base_conf):
             os.rename(self._postgresql_conf, self._postgresql_base_conf)
 
         configuration = configuration or self._server_parameters.copy()
         # Due to the permanent logical replication slots configured we have to enable hot_standby_feedback
         if self._postgresql.enforce_hot_standby_feedback:
             configuration['hot_standby_feedback'] = 'on'
 
-        with ConfigWriter(self._postgresql_conf) as f:
+        with self.config_writer(self._postgresql_conf) as f:
             include = self._config.get('custom_conf') or self._postgresql_base_conf_name
             f.writeline("include '{0}'\n".format(ConfigWriter.escape(include)))
             for name, value in sorted((configuration).items()):
                 value = transform_postgresql_parameter_value(self._postgresql.major_version, name, value,
                                                              self._postgresql.available_gucs)
                 if value is not None and\
                         (name != 'hba_file' or not self._postgresql.bootstrap.running_custom_bootstrap):
@@ -435,14 +464,15 @@
                 if not self._postgresql.bootstrap.keep_existing_recovery_conf:
                     self._sanitize_auto_conf()
 
     def append_pg_hba(self, config: List[str]) -> bool:
         if not self.hba_file and not self._config.get('pg_hba'):
             with open(self._pg_hba_conf, 'a') as f:
                 f.write('\n{}\n'.format('\n'.join(config)))
+            self.set_file_permissions(self._pg_hba_conf)
         return True
 
     def replace_pg_hba(self) -> Optional[bool]:
         """
         Replace pg_hba.conf content in the PGDATA if hba_file is not defined in the
         `postgresql.parameters` and pg_hba is defined in `postgresql` configuration section.
 
@@ -454,35 +484,35 @@
         if self._postgresql.bootstrap.running_custom_bootstrap:
             addresses = {} if os.name == 'nt' else {'': 'local'}  # windows doesn't yet support unix-domain sockets
             if 'host' in self.local_replication_address and not self.local_replication_address['host'].startswith('/'):
                 addresses.update({sa[0] + '/32': 'host' for _, _, _, _, sa in socket.getaddrinfo(
                                   self.local_replication_address['host'], self.local_replication_address['port'],
                                   0, socket.SOCK_STREAM, socket.IPPROTO_TCP)})
 
-            with ConfigWriter(self._pg_hba_conf) as f:
+            with self.config_writer(self._pg_hba_conf) as f:
                 for address, t in addresses.items():
                     f.writeline((
                         '{0}\treplication\t{1}\t{3}\ttrust\n'
                         '{0}\tall\t{2}\t{3}\ttrust'
                     ).format(t, self.replication['username'], self._superuser.get('username') or 'all', address))
         elif not self.hba_file and self._config.get('pg_hba'):
-            with ConfigWriter(self._pg_hba_conf) as f:
+            with self.config_writer(self._pg_hba_conf) as f:
                 f.writelines(self._config['pg_hba'])
             return True
 
     def replace_pg_ident(self) -> Optional[bool]:
         """
         Replace pg_ident.conf content in the PGDATA if ident_file is not defined in the
         `postgresql.parameters` and pg_ident is defined in the `postgresql` section.
 
         :returns: True if pg_ident.conf was rewritten.
         """
 
         if not self.ident_file and self._config.get('pg_ident'):
-            with ConfigWriter(self._pg_ident_conf) as f:
+            with self.config_writer(self._pg_ident_conf) as f:
                 f.writelines(self._config['pg_ident'])
             return True
 
     def primary_conninfo_params(self, member: Union[Leader, Member, None]) -> Optional[Dict[str, Any]]:
         if not member or not member.conn_url or member.name == self._postgresql.name:
             return None
         ret = member.conn_kwargs(self.replication)
@@ -796,29 +826,30 @@
         return {**os.environ, 'PGPASSFILE': self._pgpass}
 
     def write_recovery_conf(self, recovery_params: CaseInsensitiveDict) -> None:
         self._recovery_params = recovery_params
         if self._postgresql.major_version >= 120000:
             if parse_bool(recovery_params.pop('standby_mode', None)):
                 open(self._standby_signal, 'w').close()
+                self.set_file_permissions(self._standby_signal)
             else:
                 self._remove_file_if_exists(self._standby_signal)
                 open(self._recovery_signal, 'w').close()
+                self.set_file_permissions(self._recovery_signal)
 
             def restart_required(name: str) -> bool:
                 if self._postgresql.major_version >= 140000:
                     return False
                 return name == 'restore_command' or (self._postgresql.major_version < 130000
                                                      and name in ('primary_conninfo', 'primary_slot_name'))
 
             self._current_recovery_params = CaseInsensitiveDict({n: [v, restart_required(n), self._postgresql_conf]
                                                                  for n, v in recovery_params.items()})
         else:
-            with ConfigWriter(self._recovery_conf) as f:
-                os.chmod(self._recovery_conf, stat.S_IWRITE | stat.S_IREAD)
+            with self.config_writer(self._recovery_conf) as f:
                 self._write_recovery_params(f, recovery_params)
 
     def remove_recovery_conf(self) -> None:
         for name in (self._recovery_conf, self._standby_signal, self._recovery_signal):
             self._remove_file_if_exists(name)
         self._recovery_params = CaseInsensitiveDict()
         self._current_recovery_params = None
@@ -839,14 +870,15 @@
                             lines.append(raw_line)
             except Exception:
                 logger.info('Failed to read %s', self._auto_conf)
 
         if overwrite:
             try:
                 with open(self._auto_conf, 'w') as f:
+                    self.set_file_permissions(self._auto_conf)
                     for raw_line in lines:
                         f.write(raw_line)
             except Exception:
                 logger.exception('Failed to remove some unwanted parameters from %s', self._auto_conf)
 
     def _adjust_recovery_parameters(self) -> None:
         # It is not strictly necessary, but we can make patroni configs crossi-compatible with all postgres versions.
```

### Comparing `patroni-3.0.4/patroni/postgresql/connection.py` & `patroni-3.1.0/patroni/postgresql/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from contextlib import contextmanager
 from threading import Lock
-from typing import Any, Dict, Generator, Union, TYPE_CHECKING
+from typing import Any, Dict, Iterator, Union, TYPE_CHECKING
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Connection as Connection3, Cursor
     from psycopg2 import connection, cursor
 
 from .. import psycopg
 
 logger = logging.getLogger(__name__)
@@ -40,12 +40,12 @@
         if self._connection and self._connection.closed == 0:
             self._connection.close()
             logger.info("closed patroni connection to the postgresql cluster")
         self._cursor_holder = self._connection = None
 
 
 @contextmanager
-def get_connection_cursor(**kwargs: Any) -> Generator[Union['cursor', 'Cursor[Any]'], None, None]:
+def get_connection_cursor(**kwargs: Any) -> Iterator[Union['cursor', 'Cursor[Any]']]:
     conn = psycopg.connect(**kwargs)
     with conn.cursor() as cur:
         yield cur
     conn.close()
```

### Comparing `patroni-3.0.4/patroni/postgresql/misc.py` & `patroni-3.1.0/patroni/postgresql/misc.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/postmaster.py` & `patroni-3.1.0/patroni/postgresql/postmaster.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/postgresql/rewind.py` & `patroni-3.1.0/patroni/postgresql/rewind.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             if task.result:
                 wakeup()
 
     def ensure_checkpoint_after_promote(self, wakeup: Callable[..., Any]) -> None:
         """After promote issue a CHECKPOINT from a new thread and asynchronously check the result.
         In case if CHECKPOINT failed, just check that timeline in pg_control was updated."""
 
-        if self._state == REWIND_STATUS.INITIAL and self._postgresql.is_leader():
+        if self._state != REWIND_STATUS.CHECKPOINT and self._postgresql.is_leader():
             with self._checkpoint_task_lock:
                 if self._checkpoint_task:
                     with self._checkpoint_task:
                         if self._checkpoint_task.result is not None:
                             self._state = REWIND_STATUS.CHECKPOINT
                             self._checkpoint_task = None
                 elif self._postgresql.get_primary_timeline() == self._postgresql.pg_control_timeline():
@@ -366,15 +366,15 @@
             old_name = os.path.join(status_dir, wal + '.ready')
             # wal file might have alredy been archived
             if os.path.isfile(old_name) and os.path.isfile(os.path.join(self._postgresql.wal_dir, wal)):
                 cmd = self._buid_archiver_command(archive_cmd, wal)
                 # it is the author of archive_command, who is responsible
                 # for not overriding the WALs already present in archive
                 logger.info('Trying to archive %s: %s', wal, cmd)
-                if self._postgresql.cancellable.call(shlex.split(cmd)) == 0:
+                if self._postgresql.cancellable.call([cmd], shell=True) == 0:
                     new_name = os.path.join(status_dir, wal + '.done')
                     try:
                         shutil.move(old_name, new_name)
                     except Exception as e:
                         logger.error('Unable to rename %s to %s: %r', old_name, new_name, e)
                 else:
                     logger.info('Failed to archive WAL segment %s', wal)
```

### Comparing `patroni-3.0.4/patroni/postgresql/slots.py` & `patroni-3.1.0/patroni/postgresql/slots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
 import shutil
 
 from collections import defaultdict
 from contextlib import contextmanager
 from threading import Condition, Thread
-from typing import Any, Dict, Generator, List, Optional, Union, Tuple, TYPE_CHECKING
+from typing import Any, Dict, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING
 
 from .connection import get_connection_cursor
 from .misc import format_lsn, fsync_dir
 from ..dcs import Cluster, Leader
+from ..file_perm import pg_perm
 from ..psycopg import OperationalError
 
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Cursor
     from psycopg2 import cursor
     from . import Postgresql
 
@@ -126,15 +127,15 @@
 
 class SlotsHandler(object):
 
     def __init__(self, postgresql: 'Postgresql') -> None:
         self._postgresql = postgresql
         self._advance = None
         self._replication_slots: Dict[str, Dict[str, Any]] = {}  # already existing replication slots
-        self._unready_logical_slots: Dict[str, Optional[int]] = {}
+        self._logical_slots_processing_queue: Dict[str, Optional[int]] = {}
         self.pg_replslot_dir = os.path.join(self._postgresql.data_dir, 'pg_replslot')
         self.schedule()
 
     def _query(self, sql: str, *params: Any) -> Union['cursor', 'Cursor[Any]']:
         return self._postgresql.query(sql, *params, retry=False)
 
     @staticmethod
@@ -186,15 +187,16 @@
                     value.update(plugin=r[2], database=r[3], datoid=r[4])
                     if self._postgresql.major_version >= 100000:
                         value.update(catalog_xmin=r[5], confirmed_flush_lsn=r[6])
                 replication_slots[r[0]] = value
             self._replication_slots = replication_slots
             self._schedule_load_slots = False
             if self._force_readiness_check:
-                self._unready_logical_slots = {n: None for n, v in replication_slots.items() if v['type'] == 'logical'}
+                self._logical_slots_processing_queue = {n: None for n, v in replication_slots.items()
+                                                        if v['type'] == 'logical'}
                 self._force_readiness_check = False
 
     def ignore_replication_slot(self, cluster: Cluster, name: str) -> bool:
         slot = self._replication_slots[name]
         if cluster.config:
             for matcher in cluster.config.ignore_slots_matchers:
                 if ((matcher.get("name") is None or matcher["name"] == name)
@@ -248,15 +250,15 @@
                                  " WHERE slot_type = 'physical' AND slot_name = %s)").format(
                                      immediately_reserve), name, name)
                 except Exception:
                     logger.exception("Failed to create physical replication slot '%s'", name)
                 self._schedule_load_slots = True
 
     @contextmanager
-    def get_local_connection_cursor(self, **kwargs: Any) -> Generator[Union['cursor', 'Cursor[Any]'], None, None]:
+    def get_local_connection_cursor(self, **kwargs: Any) -> Iterator[Union['cursor', 'Cursor[Any]']]:
         conn_kwargs = self._postgresql.config.local_connect_kwargs
         conn_kwargs.update(kwargs)
         with get_connection_cursor(**conn_kwargs) as cur:
             yield cur
 
     def _ensure_logical_slots_primary(self, slots: Dict[str, Any]) -> None:
         # Group logical slots to be created by database name
@@ -323,76 +325,128 @@
                                                       nofailover, self._postgresql.major_version, True)
 
                 self._drop_incorrect_slots(cluster, slots, paused)
 
                 self._ensure_physical_slots(slots)
 
                 if self._postgresql.is_leader():
-                    self._unready_logical_slots.clear()
+                    self._logical_slots_processing_queue.clear()
                     self._ensure_logical_slots_primary(slots)
                 elif cluster.slots and slots:
-                    self.check_logical_slots_readiness(cluster, nofailover, replicatefrom)
+                    self.check_logical_slots_readiness(cluster, replicatefrom)
 
                     ret = self._ensure_logical_slots_replica(cluster, slots)
 
                 self._replication_slots = slots
             except Exception:
                 logger.exception('Exception when changing replication slots')
                 self._schedule_load_slots = True
         return ret
 
     @contextmanager
-    def _get_leader_connection_cursor(self, leader: Leader) -> Generator[Union['cursor', 'Cursor[Any]'], None, None]:
+    def _get_leader_connection_cursor(self, leader: Leader) -> Iterator[Union['cursor', 'Cursor[Any]']]:
         conn_kwargs = leader.conn_kwargs(self._postgresql.config.rewind_credentials)
         conn_kwargs['dbname'] = self._postgresql.database
         with get_connection_cursor(connect_timeout=3, options="-c statement_timeout=2000", **conn_kwargs) as cur:
             yield cur
 
-    def check_logical_slots_readiness(self, cluster: Cluster, nofailover: bool, replicatefrom: Optional[str]) -> None:
+    def check_logical_slots_readiness(self, cluster: Cluster, replicatefrom: Optional[str]) -> bool:
+        """Determine whether all known logical slots are synchronised from the leader.
+
+         1) Retrieve the current ``catalog_xmin`` value for the physical slot from the cluster leader, and
+         2) using previously stored list of "unready" logical slots, those which have yet to be checked hence have no
+            stored slot attributes,
+         3) store logical slot ``catalog_xmin`` when the physical slot ``catalog_xmin`` becomes valid.
+
+         :param cluster: object containing stateful information for the cluster.
+         :param replicatefrom: name of the member that should be used to replicate from.
+
+         :returns: ``False`` if any issue while checking logical slots readiness, ``True`` otherwise.
+         """
         catalog_xmin = None
-        if self._unready_logical_slots and cluster.leader:
+        if self._logical_slots_processing_queue and cluster.leader:
             slot_name = cluster.get_my_slot_name_on_primary(self._postgresql.name, replicatefrom)
             try:
                 with self._get_leader_connection_cursor(cluster.leader) as cur:
                     cur.execute("SELECT slot_name, catalog_xmin FROM pg_catalog.pg_get_replication_slots()"
                                 " WHERE NOT pg_catalog.pg_is_in_recovery() AND slot_name = ANY(%s)",
-                                ([n for n, v in self._unready_logical_slots.items() if v is None] + [slot_name],))
+                                ([n for n, v in self._logical_slots_processing_queue.items()
+                                  if v is None] + [slot_name],))
                     slots = {row[0]: row[1] for row in cur}
                     if slot_name not in slots:
-                        return logger.warning('Physical slot %s does not exist on the primary', slot_name)
+                        logger.warning('Physical slot %s does not exist on the primary', slot_name)
+                        return False
                     catalog_xmin = slots.pop(slot_name)
             except Exception as e:
-                return logger.error("Failed to check %s physical slot on the primary: %r", slot_name, e)
-            # Remember catalog_xmin of logical slots on the primary when catalog_xmin of
-            # the physical slot became valid. Logical slots on replica will be safe to use after
-            # promote when catalog_xmin of the physical slot overtakes these values.
-            if catalog_xmin is not None:
-                for name, value in slots.items():
-                    self._unready_logical_slots[name] = value
-            else:  # Replica isn't streaming or the hot_standby_feedback isn't enabled
-                try:
-                    cur = self._query("SELECT pg_catalog.current_setting('hot_standby_feedback')::boolean")
-                    row = cur.fetchone()
-                    if row and not row[0]:
-                        logger.error('Logical slot failover requires "hot_standby_feedback".'
-                                     ' Please check postgresql.auto.conf')
-                except Exception as e:
-                    logger.error('Failed to check the hot_standby_feedback setting: %r', e)
-                return  # since `catalog_xmin` isn't valid further checks don't make any sense
+                logger.error("Failed to check %s physical slot on the primary: %r", slot_name, e)
+                return False
+
+            if not self._update_pending_logical_slot_primary(slots, catalog_xmin):
+                return False  # since `catalog_xmin` isn't valid further checks don't make any sense
+
+        self._ready_logical_slots(catalog_xmin)
+        return True
+
+    def _update_pending_logical_slot_primary(self, slots: Dict[str, Any], catalog_xmin: Optional[int] = None) -> bool:
+        """Store pending logical slot information for ``catalog_xmin`` on the primary.
+
+        Remember ``catalog_xmin`` of logical slots on the primary when ``catalog_xmin`` of the physical slot became
+        valid. Logical slots on replica will be safe to use after promote when ``catalog_xmin`` of the physical slot
+        overtakes these values.
+
+        :param slots: dictionary of slot information from the primary
+        :param catalog_xmin: ``catalog_xmin`` of the physical slot used by this replica to stream changes from primary.
+
+        :returns: ``False`` if any issue was faced while processing, ``True`` otherwise.
+        """
+        if catalog_xmin is not None:
+            for name, value in slots.items():
+                self._logical_slots_processing_queue[name] = value
+            return True
+
+        # Replica isn't streaming or the hot_standby_feedback isn't enabled
+        try:
+            cur = self._query("SELECT pg_catalog.current_setting('hot_standby_feedback')::boolean")
+            row = cur.fetchone()
+            if row and not row[0]:
+                logger.error('Logical slot failover requires "hot_standby_feedback".'
+                             ' Please check postgresql.auto.conf')
+        except Exception as e:
+            logger.error('Failed to check the hot_standby_feedback setting: %r', e)
+        return False
+
+    def _ready_logical_slots(self, primary_physical_catalog_xmin: Optional[int] = None) -> None:
+        """Ready logical slots by comparing primary physical slot ``catalog_xmin`` to logical ``catalog_xmin``.
+
+        The logical slot on a replica is safe to use when the physical replica slot on the primary:
+
+            1. has a nonzero/non-null ``catalog_xmin`` represented by ``primary_physical_xmin``.
+            2. has a ``catalog_xmin`` that is not newer (greater) than the ``catalog_xmin`` of any slot on the standby
+            3. overtook the ``catalog_xmin`` of remembered values of logical slots on the primary.
+
+        :param primary_physical_catalog_xmin: is the value retrieved from ``pg_catalog.pg_get_replication_slots()`` for
+                                              the physical replication slot on the primary.
+        """
+        # Make a copy of processing queue keys as a list as the queue dictionary is modified inside the loop.
+        for name in list(self._logical_slots_processing_queue):
+            primary_logical_catalog_xmin = self._logical_slots_processing_queue[name]
+            standby_logical_slot = self._replication_slots.get(name, {})
+            standby_logical_catalog_xmin = standby_logical_slot.get('catalog_xmin', 0)
+            if TYPE_CHECKING:  # pragma: no cover
+                assert primary_logical_catalog_xmin is not None
+
+            if (
+                    not standby_logical_slot
+                    or primary_physical_catalog_xmin is not None
+                    and primary_logical_catalog_xmin <= primary_physical_catalog_xmin <= standby_logical_catalog_xmin
+            ):
+
+                del self._logical_slots_processing_queue[name]
 
-        for name in list(self._unready_logical_slots):
-            value = self._replication_slots.get(name)
-            # The logical slot on a replica is safe to use when the physical replica slot on the primary:
-            # 1. has a nonzero/non-null catalog_xmin
-            # 2. has a catalog_xmin that is not newer (greater) than the catalog_xmin of any slot on the standby
-            # 3. overtook the catalog_xmin of remembered values of logical slots on the primary.
-            if not value or catalog_xmin is not None and\
-                    self._unready_logical_slots[name] <= catalog_xmin <= value['catalog_xmin']:
-                del self._unready_logical_slots[name]
-                if value:
+                if standby_logical_slot:
                     logger.info('Logical slot %s is safe to be used after a failover', name)
 
     def copy_logical_slots(self, cluster: Cluster, create_slots: List[str]) -> None:
         leader = cluster.leader
         if not leader:
             return
         slots = cluster.get_replication_slots(self._postgresql.name, 'replica', False, self._postgresql.major_version)
@@ -414,38 +468,43 @@
                         else:
                             logger.warning('Will not copy the logical slot "%s" due to the configuration mismatch: '
                                            'configuration=%s, slot on the primary=%s', r[0], slots[r[0]], slot)
             except Exception as e:
                 logger.error("Failed to copy logical slots from the %s via postgresql connection: %r", leader.name, e)
 
         if copy_slots and self._postgresql.stop():
+            pg_perm.set_permissions_from_data_directory(self._postgresql.data_dir)
             for name, value in copy_slots.items():
-                slot_dir = os.path.join(self._postgresql.slots_handler.pg_replslot_dir, name)
+                slot_dir = os.path.join(self.pg_replslot_dir, name)
                 slot_tmp_dir = slot_dir + '.tmp'
                 if os.path.exists(slot_tmp_dir):
                     shutil.rmtree(slot_tmp_dir)
                 os.makedirs(slot_tmp_dir)
+                os.chmod(slot_tmp_dir, pg_perm.dir_create_mode)
                 fsync_dir(slot_tmp_dir)
-                with open(os.path.join(slot_tmp_dir, 'state'), 'wb') as f:
+                slot_filename = os.path.join(slot_tmp_dir, 'state')
+                with open(slot_filename, 'wb') as f:
+                    os.chmod(slot_filename, pg_perm.file_create_mode)
                     f.write(value['data'])
                     f.flush()
                     os.fsync(f.fileno())
                 if os.path.exists(slot_dir):
                     shutil.rmtree(slot_dir)
                 os.rename(slot_tmp_dir, slot_dir)
+                os.chmod(slot_dir, pg_perm.dir_create_mode)
                 fsync_dir(slot_dir)
-                self._unready_logical_slots[name] = None
-            fsync_dir(self._postgresql.slots_handler.pg_replslot_dir)
+                self._logical_slots_processing_queue[name] = None
+            fsync_dir(self.pg_replslot_dir)
             self._postgresql.start()
 
     def schedule(self, value: Optional[bool] = None) -> None:
         if value is None:
             value = self._postgresql.major_version >= 90400
         self._schedule_load_slots = self._force_readiness_check = value
 
     def on_promote(self) -> None:
         if self._advance:
             self._advance.on_promote()
 
-        if self._unready_logical_slots:
+        if self._logical_slots_processing_queue:
             logger.warning('Logical replication slots that might be unsafe to use after promote: %s',
-                           set(self._unready_logical_slots))
+                           set(self._logical_slots_processing_queue))
```

### Comparing `patroni-3.0.4/patroni/postgresql/sync.py` & `patroni-3.1.0/patroni/postgresql/sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -149,14 +149,80 @@
             members.add(a_value[1:-1].replace('""', '"'))
         else:
             raise ValueError("Unparseable synchronous_standby_names value %r: Unexpected token %s %r at %d" %
                              (value, a_type, a_value, a_pos))
     return _SSN(sync_type, has_star, num, members)
 
 
+class _Replica(NamedTuple):
+    """Class representing a single replica that is eligible to be synchronous.
+
+    Attributes are taken from ``pg_stat_replication`` view and respective ``Cluster.members``.
+
+    :ivar pid: PID of walsender process.
+    :ivar application_name: matches with the ``Member.name``.
+    :ivar sync_state: possible values are: ``async``, ``potential``, ``quorum``, and ``sync``.
+    :ivar lsn: ``write_lsn``, ``flush_lsn``, or ``replay_lsn``, depending on the value of ``synchronous_commit`` GUC.
+    :ivar nofailover: whether the corresponding member has ``nofailover`` tag set to ``True``.
+    """
+    pid: int
+    application_name: str
+    sync_state: str
+    lsn: int
+    nofailover: bool
+
+
+class _ReplicaList(List[_Replica]):
+    """A collection of :class:``_Replica`` objects.
+
+    Values are reverse ordered by ``_Replica.sync_state`` and ``_Replica.lsn``.
+    That is, first there will be replicas that have ``sync_state`` == ``sync``, even if they are not
+    the most up-to-date in term of write/flush/replay LSN. It helps to keep the result of chosing new
+    synchronous nodes consistent in case if a synchronous standby member is slowed down OR async node
+    is receiving changes faster than the sync member. Such cases would trigger sync standby member
+    swapping, but only if lag on this member is exceeding a threshold (``maximum_lag_on_syncnode``).
+
+    :ivar max_lsn: maximum value of ``_Replica.lsn`` among all values. In case if there is just one
+                   element in the list we take value of ``pg_current_wal_lsn()``.
+    """
+
+    def __init__(self, postgresql: 'Postgresql', cluster: Cluster) -> None:
+        """Create :class:``_ReplicaList`` object.
+
+        :param postgresql: reference to :class:``Postgresql`` object.
+        :param cluster: currently known cluster state from DCS.
+        """
+        super().__init__()
+
+        # We want to prioritize candidates based on `write_lsn``, ``flush_lsn``, or ``replay_lsn``.
+        # Which column exactly to pick depends on the values of ``synchronous_commit`` GUC.
+        sort_col = {
+            'remote_apply': 'replay',
+            'remote_write': 'write'
+        }.get(postgresql.synchronous_commit(), 'flush') + '_lsn'
+
+        members = CaseInsensitiveDict({m.name: m for m in cluster.members})
+        for row in postgresql.pg_stat_replication():
+            member = members.get(row['application_name'])
+
+            # We want to consider only rows from ``pg_stat_replication` that:
+            # 1. are known to be streaming (write/flush/replay LSN are not NULL).
+            # 2. can be mapped to a ``Member`` of the ``Cluster``:
+            #   a. ``Member`` doesn't have ``nosync`` tag set;
+            #   b. PostgreSQL on the member is known to be running and accepting client connections.
+            if member and row[sort_col] is not None and member.is_running and not member.tags.get('nosync', False):
+                self.append(_Replica(row['pid'], row['application_name'],
+                                     row['sync_state'], row[sort_col], bool(member.nofailover)))
+
+        # Prefer replicas that are in state ``sync`` and with higher values of ``write``/``flush``/``replay`` LSN.
+        self.sort(key=lambda r: (r.sync_state, r.lsn), reverse=True)
+
+        self.max_lsn = max(self, key=lambda x: x.lsn).lsn if len(self) > 1 else postgresql.last_operation()
+
+
 class SyncHandler(object):
     """Class responsible for working with the `synchronous_standby_names`.
 
     Sync standbys are chosen based on their state in `pg_stat_replication`.
     When `synchronous_standby_names` is changed we memorize the `_primary_flush_lsn`
     and the `current_state()` method will count newly added names as "sync" only when
     they reached memorized LSN and also reported as "sync" by `pg_stat_replication`"""
@@ -197,14 +263,29 @@
         self._postgresql.query("""DO $$
 BEGIN
     SET local synchronous_commit = 'off';
     PERFORM * FROM pg_catalog.txid_current();
 END;$$""")
         self._postgresql.reset_cluster_info_state(None)  # Reset internal cache to query fresh values
 
+    def _process_replica_readiness(self, cluster: Cluster, replica_list: _ReplicaList) -> None:
+        """Flags replicas as truly "synchronous" when they have caught up with ``_primary_flush_lsn``.
+
+        :param cluster: current cluster topology from DCS
+        :param replica_list: collection of replicas that we want to evaluate.
+        """
+        for replica in replica_list:
+            # if standby name is listed in the /sync key we can count it as synchronous, otherwise
+            # it becomes really synchronous when sync_state = 'sync' and it is known that it managed to catch up
+            if replica.application_name not in self._ready_replicas\
+                    and replica.application_name in self._ssn_data.members\
+                    and (cluster.sync.matches(replica.application_name)
+                         or replica.sync_state == 'sync' and replica.lsn >= self._primary_flush_lsn):
+                self._ready_replicas[replica.application_name] = replica.pid
+
     def current_state(self, cluster: Cluster) -> Tuple[CaseInsensitiveSet, CaseInsensitiveSet]:
         """Finds best candidates to be the synchronous standbys.
 
         Current synchronous standby is always preferred, unless it has disconnected or does not want to be a
         synchronous standby any longer.
 
         Standbys are selected based on values from the global configuration:
@@ -214,60 +295,31 @@
           Please note that it will not also swap sync standbys in case where all replicas are hung.
         - `synchronous_node_count`: controlls how many nodes should be set as synchronous.
 
         :returns: tuple of candidates :class:`CaseInsensitiveSet` and synchronous standbys :class:`CaseInsensitiveSet`.
         """
         self._handle_synchronous_standby_names_change()
 
-        # Pick candidates based on who has higher replay/remote_write/flush lsn.
-        sort_col = {
-            'remote_apply': 'replay',
-            'remote_write': 'write'
-        }.get(self._postgresql.synchronous_commit(), 'flush') + '_lsn'
-
-        pg_stat_replication = [(r['pid'], r['application_name'], r['sync_state'], r[sort_col])
-                               for r in self._postgresql.pg_stat_replication()
-                               if r[sort_col] is not None]
-
-        members = CaseInsensitiveDict({m.name: m for m in cluster.members})
-        replica_list: List[Tuple[int, str, str, int, bool]] = []
-        # pg_stat_replication.sync_state has 4 possible states - async, potential, quorum, sync.
-        # That is, alphabetically they are in the reversed order of priority.
-        # Since we are doing reversed sort on (sync_state, lsn) tuples, it helps to keep the result
-        # consistent in case if a synchronous standby member is slowed down OR async node receiving
-        # changes faster than the sync member (very rare but possible).
-        # Such cases would trigger sync standby member swapping, but only if lag on a sync node exceeding a threshold.
-        for pid, app_name, sync_state, replica_lsn in sorted(pg_stat_replication, key=lambda r: r[2:4], reverse=True):
-            member = members.get(app_name)
-            if member and member.is_running and not member.tags.get('nosync', False):
-                replica_list.append((pid, member.name, sync_state, replica_lsn, bool(member.nofailover)))
-
-        max_lsn = max(replica_list, key=lambda x: x[3])[3]\
-            if len(replica_list) > 1 else self._postgresql.last_operation()
+        replica_list = _ReplicaList(self._postgresql, cluster)
+        self._process_replica_readiness(cluster, replica_list)
 
         if TYPE_CHECKING:  # pragma: no cover
             assert self._postgresql.global_config is not None
         sync_node_count = self._postgresql.global_config.synchronous_node_count\
             if self._postgresql.supports_multiple_sync else 1
         sync_node_maxlag = self._postgresql.global_config.maximum_lag_on_syncnode
 
         candidates = CaseInsensitiveSet()
         sync_nodes = CaseInsensitiveSet()
         # Prefer members without nofailover tag. We are relying on the fact that sorts are guaranteed to be stable.
-        for pid, app_name, sync_state, replica_lsn, _ in sorted(replica_list, key=lambda x: x[4]):
-            # if standby name is listed in the /sync key we can count it as synchronous, otherwice
-            # it becomes really synchronous when sync_state = 'sync' and it is known that it managed to catch up
-            if app_name not in self._ready_replicas and app_name in self._ssn_data.members and\
-                    (cluster.sync.matches(app_name) or sync_state == 'sync' and replica_lsn >= self._primary_flush_lsn):
-                self._ready_replicas[app_name] = pid
-
-            if sync_node_maxlag <= 0 or max_lsn - replica_lsn <= sync_node_maxlag:
-                candidates.add(app_name)
-                if sync_state == 'sync' and app_name in self._ready_replicas:
-                    sync_nodes.add(app_name)
+        for replica in sorted(replica_list, key=lambda x: x.nofailover):
+            if sync_node_maxlag <= 0 or replica_list.max_lsn - replica.lsn <= sync_node_maxlag:
+                candidates.add(replica.application_name)
+                if replica.sync_state == 'sync' and replica.application_name in self._ready_replicas:
+                    sync_nodes.add(replica.application_name)
             if len(candidates) >= sync_node_count:
                 break
 
         return candidates, sync_nodes
 
     def set_synchronous_standby_names(self, sync: Collection[str]) -> None:
         """Constructs and sets "synchronous_standby_names" GUC value.
```

### Comparing `patroni-3.0.4/patroni/postgresql/validator.py` & `patroni-3.1.0/patroni/postgresql/validator.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/psycopg.py` & `patroni-3.1.0/patroni/psycopg.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/raft_controller.py` & `patroni-3.1.0/patroni/raft_controller.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/request.py` & `patroni-3.1.0/patroni/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 from urllib.parse import urlparse, urlunparse
 
 from .config import Config
 from .dcs import Member
 from .utils import USER_AGENT
 
 
+class HTTPSConnectionPool(urllib3.HTTPSConnectionPool):
+
+    def _validate_conn(self, *args: Any, **kwargs: Any) -> None:
+        """Override parent method to silence warnings about requests without certificate verification enabled."""
+
+
+class PatroniPoolManager(urllib3.PoolManager):
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super(PatroniPoolManager, self).__init__(*args, **kwargs)
+        self.pool_classes_by_scheme = {'http': urllib3.HTTPConnectionPool, 'https': HTTPSConnectionPool}
+
+
 class PatroniRequest(object):
     """Wrapper for performing requests to Patroni's REST API.
 
     Prepares the request manager with the configured settings before performing the request.
     """
 
     def __init__(self, config: Union[Config, Dict[str, Any]], insecure: Optional[bool] = None) -> None:
@@ -24,30 +37,38 @@
         :param insecure: how to deal with SSL certs verification
             * If ``True`` it will perform REST API requests without verifying SSL certs; or
             * If ``False`` it will perform REST API requests and verify SSL certs; or
             * If ``None`` it will behave according to the value of ``ctl -> insecure`` configuration; or
             * If none of the above applies, then it falls back to ``False``.
         """
         self._insecure = insecure
-        self._pool = urllib3.PoolManager(num_pools=10, maxsize=10)
+        self._pool = PatroniPoolManager(num_pools=10, maxsize=10)
         self.reload_config(config)
 
     @staticmethod
-    def _get_cfg_value(config: Union[Config, Dict[str, Any]], name: str) -> Union[Any, None]:
-        """Get value of *name* setting in *config*.
+    def _get_ctl_value(config: Union[Config, Dict[str, Any]], name: str, default: Any = None) -> Optional[Any]:
+        """Get value of *name* setting from the ``ctl`` section of the *config*.
+
+        :param config: Patroni YAML configuration.
+        :param name: name of the setting value to be retrieved.
 
-        .. note::
-            *name* key will be searched only under ``ctl`` and ``restapi`` sections, in that order.
+        :returns: value of ``ctl -> *name*`` if present, ``None`` otherwise.
+        """
+        return config.get('ctl', {}).get(name, default)
+
+    @staticmethod
+    def _get_restapi_value(config: Union[Config, Dict[str, Any]], name: str) -> Optional[Any]:
+        """Get value of *name* setting from the ``restapi`` section of the *config*.
 
         :param config: Patroni YAML configuration.
         :param name: name of the setting value to be retrieved.
 
-        :returns: value of ``ctl -> *name*`` or ``restapi -> *name*``, if either is present, ``None`` otherwise.
+        :returns: value of ``restapi -> *name*`` if present, ``None`` otherwise.
         """
-        return config.get('ctl', {}).get(name) or config.get('restapi', {}).get(name)
+        return config.get('restapi', {}).get(name)
 
     def _apply_pool_param(self, param: str, value: Any) -> None:
         """Configure *param* as *value* in the request manager.
 
         :param param: name of the setting to be changed.
         :param value: new value for *param*. If ``None``, ``0``, ``False``, and similar values, then explicit *param*
             declaration is removed, in which case it takes its default value, if any.
@@ -61,59 +82,60 @@
         """Apply a given SSL related param to the request manager.
 
         :param config: Patroni YAML configuration.
         :param name: prefix of the Patroni SSL related setting name. Currently, supports these:
             * ``cert``: gets translated to ``certfile``
             * ``key``: gets translated to ``keyfile``
 
-            Will attempt to fetch the requested key first from ``ctl`` section, and fall back to ``restapi`` section
-            if the former is missing.
+            Will attempt to fetch the requested key first from ``ctl`` section.
 
-        :returns: value of ``ctl -> *name*file`` or ``restapi -> *name*file`` if either is present, ``None`` otherwise.
+        :returns: value of ``ctl -> *name*file`` if present, ``None`` otherwise.
         """
-        value = self._get_cfg_value(config, name + 'file')
+        value = self._get_ctl_value(config, name + 'file')
         self._apply_pool_param(name + '_file', value)
         return value
 
     def reload_config(self, config: Union[Config, Dict[str, Any]]) -> None:
         """Apply *config* to request manager.
 
         Configure these HTTP headers for requests:
 
-        * ``authorization``: based on Patroni' REST API authentication config;
+        * ``authorization``: based on Patroni' CTL or REST API authentication config;
         * ``user-agent``: based on `patroni.utils.USER_AGENT`.
 
         Also configure SSL related settings for requests:
 
         * ``ca_certs`` is configured if ``ctl -> cacert`` or ``restapi -> cafile`` is available;
-        * ``cert``, ``key`` and ``key_password`` are configured if ``ctl -> certile`` or ``restapi -> certfile`` is
-            available.
+        * ``cert``, ``key`` and ``key_password`` are configured if ``ctl -> certfile`` is available.
 
         :param config: Patroni YAML configuration.
         """
-        # ``restapi -> auth`` is equivalent to ``restapi -> authentication -> username`` + ``:`` +
-        # ``restapi -> authentication -> password``
-        self._pool.headers = urllib3.make_headers(basic_auth=self._get_cfg_value(config, 'auth'), user_agent=USER_AGENT)
+        # ``ctl -> auth`` is equivalent to ``ctl -> authentication -> username`` + ``:`` +
+        # ``ctl -> authentication -> password``. And the same for ``restapi -> auth``
+        basic_auth = self._get_ctl_value(config, 'auth') or self._get_restapi_value(config, 'auth')
+        self._pool.headers = urllib3.make_headers(basic_auth=basic_auth, user_agent=USER_AGENT)
+        self._pool.connection_pool_kw['cert_reqs'] = 'CERT_REQUIRED'
+
+        insecure = self._insecure if isinstance(self._insecure, bool)\
+            else self._get_ctl_value(config, 'insecure', False)
 
-        insecure = self._insecure if isinstance(self._insecure, bool) else config.get('ctl', {}).get('insecure', False)
         if self._apply_ssl_file_param(config, 'cert'):
-            #  With client certificate the cert_reqs must be set to CERT_REQUIRED even if insecure option is used
-            self._pool.connection_pool_kw['cert_reqs'] = 'CERT_REQUIRED'
-            #  The assert_hostname = False helps to silence warnings
-            self._pool.connection_pool_kw['assert_hostname'] = False if insecure else None
+            if insecure:  # The assert_hostname = False helps to silence warnings
+                self._pool.connection_pool_kw['assert_hostname'] = False
 
             self._apply_ssl_file_param(config, 'key')
-
-            password = self._get_cfg_value(config, 'keyfile_password')
+            password = self._get_ctl_value(config, 'keyfile_password')
             self._apply_pool_param('key_password', password)
         else:
-            self._pool.connection_pool_kw['cert_reqs'] = 'CERT_NONE' if insecure else 'CERT_REQUIRED'
+            if insecure:  # Disable server certificate validation if requested
+                self._pool.connection_pool_kw['cert_reqs'] = 'CERT_NONE'
+            self._pool.connection_pool_kw.pop('assert_hostname', None)
             self._pool.connection_pool_kw.pop('key_file', None)
 
-        cacert = config.get('ctl', {}).get('cacert') or config.get('restapi', {}).get('cafile')
+        cacert = self._get_ctl_value(config, 'cacert') or self._get_restapi_value(config, 'cafile')
         self._apply_pool_param('ca_certs', cacert)
 
     def request(self, method: str, url: str, body: Optional[Any] = None,
                 **kwargs: Any) -> urllib3.response.HTTPResponse:
         """Perform an HTTP request.
 
         :param method: the HTTP method to be used, e.g. ``GET``.
```

### Comparing `patroni-3.0.4/patroni/scripts/aws.py` & `patroni-3.1.0/patroni/scripts/aws.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/scripts/wale_restore.py` & `patroni-3.1.0/patroni/scripts/wale_restore.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/utils.py` & `patroni-3.1.0/patroni/utils.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/validator.py` & `patroni-3.1.0/patroni/validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 """
 import os
 import re
 import shutil
 import socket
 import subprocess
 
-from typing import Any, Dict, Union, Iterator, List, Optional as OptionalType, TYPE_CHECKING
+from typing import Any, Dict, Union, Iterator, List, Optional as OptionalType, Tuple, TYPE_CHECKING
 
-from .utils import parse_int, split_host_port, data_directory_is_empty
+from .collections import CaseInsensitiveSet
 from .dcs import dcs_modules
 from .exceptions import ConfigParseError
+from .utils import parse_int, split_host_port, data_directory_is_empty
 
 
 def data_directory_empty(data_dir: str) -> bool:
     """Check if PostgreSQL data directory is empty.
 
     :param data_dir: path to the PostgreSQL data directory to be checked.
     :returns: ``True`` if the data directory is empty.
@@ -780,15 +781,15 @@
         :param raise_assert: if an ``assert`` call should be performed regarding expected type and valid range.
         """
         self.min = min
         self.max = max
         self.base_unit = base_unit
         self.raise_assert = raise_assert
 
-    def __call__(self, value: Union[int, str]) -> bool:
+    def __call__(self, value: Any) -> bool:
         """Check if *value* is a valid integer and within the expected range.
 
         .. note::
             If ``raise_assert`` is ``True`` and *value* is not valid, then an ``AssertionError`` will be triggered.
         :param value: value to be checked against the rules defined for this :class:`IntValidator` instance.
         :returns: ``True`` if *value* is valid and within the expected range.
         """
@@ -798,14 +799,47 @@
             and (self.max is None or value <= self.max)
 
         if self.raise_assert:
             assert_(ret)
         return ret
 
 
+class EnumValidator(object):
+    """Validate enum setting
+
+    :ivar allowed_values: a ``set`` or ``CaseInsensitiveSet`` object with allowed enum values.
+    :ivar raise_assert: if an ``assert`` call should be performed regarding expected type and valid range.
+    """
+
+    def __init__(self, allowed_values: Tuple[str, ...],
+                 case_sensitive: bool = False, raise_assert: bool = False) -> None:
+        """Create an :class:`EnumValidator` object with given allowed values.
+
+        :param allowed_values: a tuple with allowed enum values
+        :param case_sensitive: set to ``True`` to do case sensitive comparisons
+        :param raise_assert: if an ``assert`` call should be performed regarding expected values.
+        """
+        self.allowed_values = set(allowed_values) if case_sensitive else CaseInsensitiveSet(allowed_values)
+        self.raise_assert = raise_assert
+
+    def __call__(self, value: Any) -> bool:
+        """Check if provided *value* could be found within *allowed_values*.
+
+        .. note::
+            If ``raise_assert`` is ``True`` and *value* is not valid, then an ``AssertionError`` will be triggered.
+        :param value: value to be checked.
+        :returns: ``True`` if *value* could be found within *allowed_values*.
+        """
+        ret = isinstance(value, str) and value in self.allowed_values
+
+        if self.raise_assert:
+            assert_(ret)
+        return ret
+
+
 def validate_watchdog_mode(value: Any) -> None:
     """Validate ``watchdog.mode`` configuration option.
 
     :param value: value of ``watchdog.mode`` to be validated.
     """
     assert_(isinstance(value, (str, bool)), "expected type is not a string")
     assert_(value in (False, "off", "automatic", "required"))
@@ -823,39 +857,117 @@
 validate_etcd = {
     Or("host", "hosts", "srv", "srv_suffix", "url", "proxy"): Case({
         "host": validate_host_port,
         "hosts": Or(comma_separated_host_port, [validate_host_port]),
         "srv": str,
         "srv_suffix": str,
         "url": str,
-        "proxy": str})
+        "proxy": str
+    }),
+    Optional("protocol"): str,
+    Optional("username"): str,
+    Optional("password"): str,
+    Optional("cacert"): str,
+    Optional("cert"): str,
+    Optional("key"): str
 }
 
 schema = Schema({
     "name": str,
     "scope": str,
+    Optional("ctl"): {
+        Optional("insecure"): bool,
+        Optional("cacert"): str,
+        Optional("certfile"): str,
+        Optional("keyfile"): str,
+        Optional("keyfile_password"): str
+    },
     "restapi": {
         "listen": validate_host_port_listen,
         "connect_address": validate_connect_address,
+        Optional("authentication"): {
+            "username": str,
+            "password": str
+        },
+        Optional("certfile"): str,
+        Optional("keyfile"): str,
+        Optional("keyfile_password"): str,
+        Optional("cafile"): str,
+        Optional("ciphers"): str,
+        Optional("verify_client"): EnumValidator(("none", "optional", "required"),
+                                                 case_sensitive=True, raise_assert=True),
+        Optional("allowlist"): [str],
+        Optional("allowlist_include_members"): bool,
+        Optional("http_extra_headers"): dict,
+        Optional("https_extra_headers"): dict,
         Optional("request_queue_size"): IntValidator(min=0, max=4096, raise_assert=True)
     },
     Optional("bootstrap"): {
         "dcs": {
             Optional("ttl"): int,
             Optional("loop_wait"): int,
             Optional("retry_timeout"): int,
-            Optional("maximum_lag_on_failover"): int
+            Optional("maximum_lag_on_failover"): int,
+            Optional("maximum_lag_on_syncnode"): int,
+            Optional("postgresql"): {
+                Optional("parameters"): {
+                    Optional("max_connections"): int,
+                    Optional("max_locks_per_transaction"): int,
+                    Optional("max_prepared_transactions"): int,
+                    Optional("max_replication_slots"): int,
+                    Optional("max_wal_senders"): int,
+                    Optional("max_worker_processes"): int
+                },
+                Optional("use_pg_rewind"): bool,
+                Optional("pg_hba"): [str],
+                Optional("pg_ident"): [str],
+                Optional("pg_ctl_timeout"): int,
+                Optional("use_slots"): bool,
+            },
+            Optional("primary_start_timeout"): int,
+            Optional("primary_stop_timeout"): int,
+            Optional("standby_cluster"): {
+                Or("host", "port", "restore_command"): Case({
+                    "host": str,
+                    "port": int,
+                    "restore_command": str
+                }),
+                Optional("primary_slot_name"): str,
+                Optional("create_replica_methods"): [str],
+                Optional("archive_cleanup_command"): str,
+                Optional("recovery_min_apply_delay"): str
+            },
+            Optional("synchronous_mode"): bool,
+            Optional("synchronous_mode_strict"): bool,
+            Optional("synchronous_node_count"): int
         },
-        Optional("initdb"): [Or(str, dict)]
+        Optional("initdb"): [Or(str, dict)],
+        Optional("method"): str
     },
     Or(*available_dcs): Case({
         "consul": {
             Or("host", "url"): Case({
                 "host": validate_host_port,
-                "url": str})
+                "url": str
+            }),
+            Optional("port"): int,
+            Optional("scheme"): str,
+            Optional("token"): str,
+            Optional("verify"): bool,
+            Optional("cacert"): str,
+            Optional("cert"): str,
+            Optional("key"): str,
+            Optional("dc"): str,
+            Optional("checks"): [str],
+            Optional("register_service"): bool,
+            Optional("service_tags"): [str],
+            Optional("service_check_interval"): str,
+            Optional("service_check_tls_server_name"): str,
+            Optional("consistency"): EnumValidator(('default', 'consistent', 'stale'),
+                                                   case_sensitive=True, raise_assert=True)
         },
         "etcd": validate_etcd,
         "etcd3": validate_etcd,
         "exhibitor": {
             "hosts": [str],
             "port": IntValidator(max=65535, raise_assert=True),
             Optional("pool_interval"): int
@@ -865,23 +977,36 @@
             Optional("bind_addr"): validate_host_port_listen,
             "partner_addrs": validate_host_port_list,
             Optional("data_dir"): str,
             Optional("password"): str
         },
         "zookeeper": {
             "hosts": Or(comma_separated_host_port, [validate_host_port]),
+            Optional("use_ssl"): bool,
+            Optional("cacert"): str,
+            Optional("cert"): str,
+            Optional("key"): str,
+            Optional("key_password"): str,
+            Optional("verify"): bool,
+            Optional("set_acls"): dict
         },
         "kubernetes": {
             "labels": {},
+            Optional("bypass_api_service"): bool,
             Optional("namespace"): str,
             Optional("scope_label"): str,
             Optional("role_label"): str,
+            Optional("leader_label_value"): str,
+            Optional("follower_label_value"): str,
+            Optional("standby_leader_label_value"): str,
+            Optional("tmp_role_label"): str,
             Optional("use_endpoints"): bool,
             Optional("pod_ip"): Or(is_ipv4_address, is_ipv6_address),
             Optional("ports"): [{"name": str, "port": int}],
+            Optional("cacert"): str,
             Optional("retriable_http_codes"): Or(int, [int]),
         },
     }),
     Optional("citus"): {
         "database": str,
         "group": int
     },
@@ -911,15 +1036,16 @@
         Optional("pg_hba"): [str],
         Optional("pg_ident"): [str],
         Optional("pg_ctl_timeout"): int,
         Optional("use_pg_rewind"): bool
     },
     Optional("watchdog"): {
         Optional("mode"): validate_watchdog_mode,
-        Optional("device"): str
+        Optional("device"): str,
+        Optional("safety_margin"): int
     },
     Optional("tags"): {
         Optional("nofailover"): bool,
         Optional("clonefrom"): bool,
         Optional("noloadbalance"): bool,
         Optional("replicatefrom"): str,
         Optional("nosync"): bool
```

### Comparing `patroni-3.0.4/patroni/watchdog/base.py` & `patroni-3.1.0/patroni/watchdog/base.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni/watchdog/linux.py` & `patroni-3.1.0/patroni/watchdog/linux.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/patroni.egg-info/PKG-INFO` & `patroni-3.1.0/patroni.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patroni
-Version: 3.0.4
+Version: 3.1.0
 Summary: PostgreSQL High-Available orchestrator and CLI
 Home-page: https://github.com/zalando/patroni
 Author: Alexander Kukushkin, Polina Bungina
 Author-email: akukushkin@microsoft.com, polina.bungina@zalando.de
 License: The MIT License
 Keywords: etcd governor patroni postgresql postgres ha haproxy confd zookeeper exhibitor consul streaming replication kubernetes k8s
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `patroni-3.0.4/patroni.egg-info/SOURCES.txt` & `patroni-3.1.0/patroni.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 patroni/api.py
 patroni/async_executor.py
 patroni/collections.py
 patroni/config.py
 patroni/ctl.py
 patroni/daemon.py
 patroni/exceptions.py
+patroni/file_perm.py
 patroni/ha.py
 patroni/log.py
 patroni/psycopg.py
 patroni/raft_controller.py
 patroni/request.py
 patroni/utils.py
 patroni/validator.py
@@ -64,14 +65,15 @@
 tests/test_citus.py
 tests/test_config.py
 tests/test_consul.py
 tests/test_ctl.py
 tests/test_etcd.py
 tests/test_etcd3.py
 tests/test_exhibitor.py
+tests/test_file_perm.py
 tests/test_ha.py
 tests/test_kubernetes.py
 tests/test_log.py
 tests/test_patroni.py
 tests/test_postgresql.py
 tests/test_postmaster.py
 tests/test_raft.py
```

### Comparing `patroni-3.0.4/setup.py` & `patroni-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_api.py` & `patroni-3.1.0/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         with patch.object(RestApiHandler, 'get_postgresql_status', Mock(return_value={'role': 'primary'})):
             MockRestApiServer(RestApiHandler, 'GET /primary')
         with patch.object(MockHa, 'restart_scheduled', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /primary')
         self.assertIsNotNone(MockRestApiServer(RestApiHandler, 'GET /primary'))
         with patch.object(RestApiServer, 'query', Mock(return_value=[('', 1, '', '', '', '', False, None, None, '')])):
             self.assertIsNotNone(MockRestApiServer(RestApiHandler, 'GET /patroni'))
-        with patch.object(GlobalConfig, 'is_standby_cluster', Mock(return_value=True)),\
+        with patch.object(GlobalConfig, 'is_standby_cluster', Mock(return_value=True)), \
                 patch.object(GlobalConfig, 'is_paused', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /standby_leader')
 
         # test tags
         #
         MockRestApiServer(RestApiHandler, 'GET /primary?lag=1M&'
                                           'tag_key1=true&tag_key2=false&'
@@ -555,15 +555,15 @@
         with patch.object(MockHa, 'fetch_nodes_statuses', Mock(return_value=[])):
             MockRestApiServer(RestApiHandler, request)
 
         # Valid future date
         request = post + '103\n\n{"leader": "postgresql1", "member": "postgresql2",' +\
                          ' "scheduled_at": "6016-02-15T18:13:30.568224+01:00"}'
         MockRestApiServer(RestApiHandler, request)
-        with patch.object(GlobalConfig, 'is_paused', PropertyMock(return_value=True)),\
+        with patch.object(GlobalConfig, 'is_paused', PropertyMock(return_value=True)), \
                 patch.object(MockPatroni, 'dcs') as d:
             d.manual_failover.return_value = False
             MockRestApiServer(RestApiHandler, request)
 
         # Exception: No timezone specified
         request = post + '97\n\n{"leader": "postgresql1", "member": "postgresql2",' +\
                          ' "scheduled_at": "6016-02-15T18:13:30.568224"}'
```

### Comparing `patroni-3.0.4/tests/test_async_executor.py` & `patroni-3.1.0/tests/test_async_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_aws.py` & `patroni-3.1.0/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_bootstrap.py` & `patroni-3.1.0/tests/test_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,17 +151,17 @@
                                                                 'max_locks_per_xact setting': 64}))
     def test_bootstrap(self):
         with patch('subprocess.call', Mock(return_value=1)):
             self.assertFalse(self.b.bootstrap({}))
 
         config = {'users': {'replicator': {'password': 'rep-pass', 'options': ['replication']}}}
 
-        with patch.object(Postgresql, 'is_running', Mock(return_value=False)),\
-                patch.object(Postgresql, 'get_major_version', Mock(return_value=140000)),\
-                patch('multiprocessing.Process', Mock(side_effect=Exception)),\
+        with patch.object(Postgresql, 'is_running', Mock(return_value=False)), \
+                patch.object(Postgresql, 'get_major_version', Mock(return_value=140000)), \
+                patch('multiprocessing.Process', Mock(side_effect=Exception)), \
                 patch('multiprocessing.get_context', Mock(side_effect=Exception), create=True):
             self.assertRaises(Exception, self.b.bootstrap, config)
         with open(os.path.join(self.p.data_dir, 'pg_hba.conf')) as f:
             lines = f.readlines()
             self.assertTrue('host all all 0.0.0.0/0 md5\n' in lines)
 
         self.p.config._config.pop('pg_hba')
@@ -181,20 +181,20 @@
         self.p.config._config.pop('pg_hba')
         config = {'method': 'foo', 'foo': {'command': 'bar'}}
 
         mock_cancellable_subprocess_call.return_value = 1
         self.assertFalse(self.b.bootstrap(config))
 
         mock_cancellable_subprocess_call.return_value = 0
-        with patch('multiprocessing.Process', Mock(side_effect=Exception("42"))),\
-                patch('multiprocessing.get_context', Mock(side_effect=Exception("42")), create=True),\
-                patch('os.path.isfile', Mock(return_value=True)),\
-                patch('os.unlink', Mock()),\
-                patch.object(ConfigHandler, 'save_configuration_files', Mock()),\
-                patch.object(ConfigHandler, 'restore_configuration_files', Mock()),\
+        with patch('multiprocessing.Process', Mock(side_effect=Exception("42"))), \
+                patch('multiprocessing.get_context', Mock(side_effect=Exception("42")), create=True), \
+                patch('os.path.isfile', Mock(return_value=True)), \
+                patch('os.unlink', Mock()), \
+                patch.object(ConfigHandler, 'save_configuration_files', Mock()), \
+                patch.object(ConfigHandler, 'restore_configuration_files', Mock()), \
                 patch.object(ConfigHandler, 'write_recovery_conf', Mock()):
             with self.assertRaises(Exception) as e:
                 self.b.bootstrap(config)
             self.assertEqual(str(e.exception), '42')
 
             config['foo']['recovery_conf'] = {'foo': 'bar'}
```

### Comparing `patroni-3.0.4/tests/test_callback_executor.py` & `patroni-3.1.0/tests/test_callback_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_cancellable.py` & `patroni-3.1.0/tests/test_cancellable.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_citus.py` & `patroni-3.1.0/tests/test_citus.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def test_handle_event(self):
         self.c.handle_event(self.cluster, {})
         with patch.object(CitusHandler, 'is_alive', Mock(return_value=True)):
             self.c.handle_event(self.cluster, {'type': 'after_promote', 'group': 2,
                                                'leader': 'leader', 'timeout': 30, 'cooldown': 10})
 
     def test_add_task(self):
-        with patch('patroni.postgresql.citus.logger.error') as mock_logger,\
+        with patch('patroni.postgresql.citus.logger.error') as mock_logger, \
                 patch('patroni.postgresql.citus.urlparse', Mock(side_effect=Exception)):
             self.c.add_task('', 1, None)
             mock_logger.assert_called_once()
 
         with patch('patroni.postgresql.citus.logger.debug') as mock_logger:
             self.c.add_task('before_demote', 1, 'postgres://host:5432/postgres', 30)
             mock_logger.assert_called_once()
@@ -103,15 +103,15 @@
             self.assertEqual(mock_query.call_args[0][0], 'COMMIT')
 
     def test_process_tasks(self):
         self.c.add_task('after_promote', 0, 'postgres://host2:5432/postgres')
         self.c.process_tasks()
 
         self.c.add_task('after_promote', 0, 'postgres://host3:5432/postgres')
-        with patch('patroni.postgresql.citus.logger.error') as mock_logger,\
+        with patch('patroni.postgresql.citus.logger.error') as mock_logger, \
                 patch.object(CitusHandler, 'query', Mock(side_effect=Exception)):
             self.c.process_tasks()
             mock_logger.assert_called_once()
             self.assertTrue(mock_logger.call_args[0][0].startswith('Exception when working with pg_dist_node: '))
 
     def test_on_demote(self):
         self.c.on_demote()
```

### Comparing `patroni-3.0.4/tests/test_config.py` & `patroni-3.1.0/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         os.environ[Config.PATRONI_CONFIG_VARIABLE] = 'restapi: {}\npostgresql: {data_dir: foo}'
         self.config = Config(None)
 
     def test_set_dynamic_configuration(self):
         with patch.object(Config, '_build_effective_configuration', Mock(side_effect=Exception)):
             self.assertFalse(self.config.set_dynamic_configuration({'foo': 'bar'}))
         self.assertTrue(self.config.set_dynamic_configuration({'standby_cluster': {}, 'postgresql': {
-            'parameters': {'cluster_name': 1, 'wal_keep_size': 1, 'track_commit_timestamp': 1, 'wal_level': 1}}}))
+            'parameters': {'cluster_name': 1, 'hot_standby': 1, 'wal_keep_size': 1,
+                           'track_commit_timestamp': 1, 'wal_level': 1}}}))
 
     def test_reload_local_configuration(self):
         os.environ.update({
             'PATRONI_NAME': 'postgres0',
             'PATRONI_NAMESPACE': '/patroni/',
             'PATRONI_SCOPE': 'batman2',
             'PATRONI_LOGLEVEL': 'ERROR',
@@ -80,14 +81,15 @@
             self.assertTrue(config.reload_local_configuration())
             self.assertIsNone(config.reload_local_configuration())
 
     @patch('tempfile.mkstemp', Mock(return_value=[3000, 'blabla']))
     @patch('os.path.exists', Mock(return_value=True))
     @patch('os.remove', Mock(side_effect=IOError))
     @patch('os.close', Mock(side_effect=IOError))
+    @patch('os.chmod', Mock())
     @patch('shutil.move', Mock(return_value=None))
     @patch('json.dump', Mock())
     def test_save_cache(self):
         self.config.set_dynamic_configuration({'ttl': 30, 'postgresql': {'foo': 'bar'}})
         with patch('os.fdopen', Mock(side_effect=IOError)):
             self.config.save_cache()
         with patch('os.fdopen', MagicMock()):
```

### Comparing `patroni-3.0.4/tests/test_consul.py` & `patroni-3.1.0/tests/test_consul.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_ctl.py` & `patroni-3.1.0/tests/test_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from . import MockConnect, MockCursor, MockResponse, psycopg_connect
 from .test_etcd import etcd_read, socket_getaddrinfo
 from .test_ha import get_cluster_initialized_without_leader, get_cluster_initialized_with_leader, \
     get_cluster_initialized_with_only_leader, get_cluster_not_initialized_without_leader, get_cluster, Member
 
 
 @patch('patroni.ctl.load_config', Mock(return_value={
-    'scope': 'alpha', 'restapi': {'listen': '::', 'certfile': 'a'},
+    'scope': 'alpha', 'restapi': {'listen': '::', 'certfile': 'a'}, 'ctl': {'certfile': 'a'},
     'etcd': {'host': 'localhost:2379'}, 'citus': {'database': 'citus', 'group': 0},
     'postgresql': {'data_dir': '.', 'pgpass': './pgpass', 'parameters': {}, 'retry_timeout': 5}}))
 class TestCtl(unittest.TestCase):
     TEST_ROLES = ('master', 'primary', 'leader')
 
     @patch('socket.getaddrinfo', socket_getaddrinfo)
     @patch.object(AbstractEtcdClientWithFailover, '_get_machines_list', Mock(return_value=['http://remotehost:2379']))
@@ -79,17 +79,21 @@
         assert parse_dcs('etcd3://random.com:2399') == {'etcd3': {'host': 'random.com:2399'}}
         self.assertRaises(PatroniCtlException, parse_dcs, 'invalid://test')
 
     def test_output_members(self):
         scheduled_at = datetime.now(tzutc) + timedelta(seconds=600)
         cluster = get_cluster_initialized_with_leader(Failover(1, 'foo', 'bar', scheduled_at))
         del cluster.members[1].data['conn_url']
-        for fmt in ('pretty', 'json', 'yaml', 'tsv', 'topology'):
+        for fmt in ('pretty', 'json', 'yaml', 'topology'):
             self.assertIsNone(output_members({}, cluster, name='abc', fmt=fmt))
 
+        with patch('click.echo') as mock_echo:
+            self.assertIsNone(output_members({}, cluster, name='abc', fmt='tsv'))
+            self.assertEqual(mock_echo.call_args[0][0], 'abc\tother\t\tReplica\trunning\t\tunknown')
+
     @patch('patroni.ctl.get_dcs')
     @patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
     def test_switchover(self, mock_get_dcs):
         mock_get_dcs.return_value = self.e
         mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
         mock_get_dcs.return_value.set_failover_value = Mock()
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
@@ -447,15 +451,15 @@
     @patch('patroni.ctl.get_dcs')
     @patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
     def test_flush_restart(self, mock_get_dcs):
         mock_get_dcs.return_value = self.e
         mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
 
         for role in self.TEST_ROLES:
-            result = self.runner.invoke(ctl, ['flush', 'dummy', 'restart', '-r', role], input='y')
+            result = self.runner.invoke(ctl, ['-k', 'flush', 'dummy', 'restart', '-r', role], input='y')
             assert 'No scheduled restart' in result.output
 
         result = self.runner.invoke(ctl, ['flush', 'dummy', 'restart', '--force'])
         assert 'Success: flush scheduled restart' in result.output
         with patch.object(PoolManager, 'request', return_value=MockResponse(404)):
             result = self.runner.invoke(ctl, ['flush', 'dummy', 'restart', '--force'])
             assert 'Failed: flush scheduled restart' in result.output
```

### Comparing `patroni-3.0.4/tests/test_etcd.py` & `patroni-3.1.0/tests/test_etcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,20 +168,20 @@
         rtry(self.client.api_execute, '/', 'POST', timeout=0, params={'retry': rtry})
         self.client._machines_cache_updated = 0
         self.client.api_execute('/', 'POST', timeout=0)
         self.client._machines_cache = [self.client._base_uri]
         self.assertRaises(etcd.EtcdWatchTimedOut, self.client.api_execute, '/timeout', 'POST', params={'wait': 'true'})
         self.assertRaises(etcd.EtcdWatchTimedOut, self.client.api_execute, '/timeout', 'POST', params={'wait': 'true'})
 
-        with patch.object(EtcdClient, '_calculate_timeouts', Mock(side_effect=[(1, 1, 0), (1, 1, 0), (0, 1, 0)])),\
+        with patch.object(EtcdClient, '_calculate_timeouts', Mock(side_effect=[(1, 1, 0), (1, 1, 0), (0, 1, 0)])), \
                 patch.object(EtcdClient, '_load_machines_cache', Mock(side_effect=Exception)):
             self.client.http.request = Mock(side_effect=socket.error)
             self.assertRaises(etcd.EtcdException, rtry, self.client.api_execute, '/', 'GET', params={'retry': rtry})
 
-        with patch.object(EtcdClient, '_calculate_timeouts', Mock(side_effect=[(1, 1, 0), (1, 1, 0), (0, 1, 0)])),\
+        with patch.object(EtcdClient, '_calculate_timeouts', Mock(side_effect=[(1, 1, 0), (1, 1, 0), (0, 1, 0)])), \
                 patch.object(EtcdClient, '_load_machines_cache', Mock(return_value=True)):
             self.assertRaises(etcd.EtcdException, rtry, self.client.api_execute, '/', 'GET', params={'retry': rtry})
 
         with patch.object(EtcdClient, '_do_http_request', Mock(side_effect=etcd.EtcdException)):
             self.client._read_timeout = 0.01
             self.assertRaises(etcd.EtcdException, self.client.api_execute, '/', 'GET')
```

### Comparing `patroni-3.0.4/tests/test_etcd3.py` & `patroni-3.1.0/tests/test_etcd3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import etcd
 import json
 import unittest
 import urllib3
 
 from mock import Mock, PropertyMock, patch
 from patroni.dcs.etcd import DnsCachingResolver
-from patroni.dcs.etcd3 import PatroniEtcd3Client, Cluster, Etcd3Client, Etcd3Error, Etcd3ClientError, RetryFailedError,\
-    InvalidAuthToken, Unavailable, Unknown, UnsupportedEtcdVersion, UserEmpty, AuthFailed, base64_encode, Etcd3
+from patroni.dcs.etcd3 import PatroniEtcd3Client, Cluster, Etcd3, Etcd3Client, \
+    Etcd3Error, Etcd3ClientError, RetryFailedError, InvalidAuthToken, Unavailable, \
+    Unknown, UnsupportedEtcdVersion, UserEmpty, AuthFailed, base64_encode
 from threading import Thread
 
 from . import SleepException, MockResponse
 
 
 def mock_urlopen(self, method, url, **kwargs):
     ret = MockResponse()
@@ -122,18 +123,24 @@
         self.assertRaises(SystemExit, self.setUp)
 
     @patch.object(urllib3.PoolManager, 'urlopen')
     def test_call_rpc(self, mock_urlopen):
         request = {'key': base64_encode('/patroni/test/leader')}
         mock_urlopen.return_value = MockResponse()
         mock_urlopen.return_value.content = '{"succeeded":true,"header":{"revision":"1"}}'
-        self.client.call_rpc('/kv/txn', {'success': [{'request_delete_range': request}]})
         self.client.call_rpc('/kv/put', request)
         self.client.call_rpc('/kv/deleterange', request)
 
+    @patch.object(urllib3.PoolManager, 'urlopen')
+    def test_txn(self, mock_urlopen):
+        mock_urlopen.return_value = MockResponse()
+        mock_urlopen.return_value.content = '{"header":{"revision":"1"}}'
+        self.client.txn({'target': 'MOD', 'mod_revision': '1'},
+                        {'request_delete_range': {'key': base64_encode('/patroni/test/leader')}})
+
     @patch('time.time', Mock(side_effect=[1, 10.9, 100]))
     def test__wait_cache(self):
         with self.kv_cache.condition:
             self.assertRaises(RetryFailedError, self.client._wait_cache, 10)
 
     @patch.object(urllib3.PoolManager, 'urlopen')
     def test__restart_watcher(self, mock_urlopen):
@@ -237,15 +244,15 @@
     def test__update_leader(self):
         leader = self.etcd3.get_cluster().leader
         self.etcd3._lease = None
         with patch.object(Etcd3Client, 'txn', Mock(return_value={'succeeded': True})):
             self.etcd3.update_leader(leader, '123', failsafe={'foo': 'bar'})
         self.etcd3._last_lease_refresh = 0
         self.etcd3.update_leader(leader, '124')
-        with patch.object(PatroniEtcd3Client, 'lease_keepalive', Mock(return_value=True)),\
+        with patch.object(PatroniEtcd3Client, 'lease_keepalive', Mock(return_value=True)), \
                 patch('time.time', Mock(side_effect=[0, 100, 200, 300])):
             self.assertRaises(Etcd3Error, self.etcd3.update_leader, leader, '126')
         self.etcd3._lease = leader.session
         self.etcd3.update_leader(leader, '124')
         self.etcd3._last_lease_refresh = 0
         with patch.object(PatroniEtcd3Client, 'lease_keepalive', Mock(side_effect=Unknown)):
             self.assertFalse(self.etcd3.update_leader(leader, '125'))
```

### Comparing `patroni-3.0.4/tests/test_exhibitor.py` & `patroni-3.1.0/tests/test_exhibitor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_ha.py` & `patroni-3.1.0/tests/test_ha.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,16 +274,18 @@
 
     def test_recover_raft(self):
         self.p.controldata = lambda: {'Database cluster state': 'in recovery', 'Database system identifier': SYSID}
         self.p.is_running = false
         self.p.follow = true
         self.assertEqual(self.ha.run_cycle(), 'starting as a secondary')
         self.p.is_running = true
+        ha_dcs_orig_name = self.ha.dcs.__class__.__name__
         self.ha.dcs.__class__.__name__ = 'Raft'
         self.assertEqual(self.ha.run_cycle(), 'started as a secondary')
+        self.ha.dcs.__class__.__name__ = ha_dcs_orig_name
 
     def test_recover_former_primary(self):
         self.p.follow = false
         self.p.is_running = false
         self.p.name = 'leader'
         self.p.set_role('demoted')
         self.p.controldata = lambda: {'Database cluster state': 'shut down', 'Database system identifier': SYSID}
@@ -301,15 +303,15 @@
 
     @patch.object(Rewind, 'ensure_clean_shutdown', Mock())
     def test_crash_recovery(self):
         self.ha.has_lock = true
         self.p.is_running = false
         self.p.controldata = lambda: {'Database cluster state': 'in production', 'Database system identifier': SYSID}
         self.assertEqual(self.ha.run_cycle(), 'doing crash recovery in a single user mode')
-        with patch('patroni.async_executor.AsyncExecutor.busy', PropertyMock(return_value=True)),\
+        with patch('patroni.async_executor.AsyncExecutor.busy', PropertyMock(return_value=True)), \
                 patch.object(Ha, 'check_timeline', Mock(return_value=False)):
             self.ha._async_executor.schedule('doing crash recovery in a single user mode')
             self.ha.state_handler.cancellable._process = Mock()
             self.ha._crash_recovery_started -= 600
             self.ha.cluster.config.data.update({'maximum_lag_on_failover': 10})
             self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
             self.assertEqual(self.ha.run_cycle(), 'terminated crash recovery because of startup timeout')
@@ -334,15 +336,15 @@
         self.p.is_running = false
         self.ha.cluster = get_cluster_initialized_with_leader()
         self.ha.cluster.leader.member.data.update(version='2.0.2', role='primary')
         self.ha._rewind.pg_rewind = true
         self.ha._rewind.check_leader_is_not_in_recovery = true
         with patch.object(Rewind, 'rewind_or_reinitialize_needed_and_possible', Mock(return_value=True)):
             self.assertEqual(self.ha.run_cycle(), 'running pg_rewind from leader')
-        with patch.object(Rewind, 'rewind_or_reinitialize_needed_and_possible', Mock(return_value=False)),\
+        with patch.object(Rewind, 'rewind_or_reinitialize_needed_and_possible', Mock(return_value=False)), \
                 patch.object(Ha, 'is_synchronous_mode', Mock(return_value=True)):
             self.p.follow = true
             self.assertEqual(self.ha.run_cycle(), 'starting as a secondary')
             self.p.is_running = true
             self.ha.follow = Mock(return_value='fake')
             self.assertEqual(self.ha.run_cycle(), 'fake')
 
@@ -369,14 +371,20 @@
         self.p.controldata = lambda: {'Database cluster state': 'in production', 'Database system identifier': SYSID}
         self.assertEqual(self.ha.run_cycle(), 'promoted self to leader because I had the session lock')
 
     @patch('patroni.psycopg.connect', psycopg_connect)
     def test_acquire_lock_as_primary(self):
         self.assertEqual(self.ha.run_cycle(), 'acquired session lock as a leader')
 
+    def test_leader_race_stale_primary(self):
+        with patch.object(Postgresql, 'get_primary_timeline', Mock(return_value=1)), \
+                patch('patroni.ha.logger.warning') as mock_logger:
+            self.assertEqual(self.ha.run_cycle(), 'demoting self because i am not the healthiest node')
+            self.assertEqual(mock_logger.call_args[0][0], 'My timeline %s is behind last known cluster timeline %s')
+
     def test_promoted_by_acquiring_lock(self):
         self.ha.is_healthiest_node = true
         self.p.is_leader = false
         self.assertEqual(self.ha.run_cycle(), 'promoted self to leader by acquiring session lock')
 
     def test_promotion_cancelled_after_pre_promote_failed(self):
         self.p.is_leader = false
@@ -602,15 +610,15 @@
     @patch('patroni.postgresql.citus.quote_ident', Mock())
     @patch.object(Postgresql, 'connection', Mock(return_value=None))
     def test_bootstrap_release_initialize_key_on_watchdog_failure(self):
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.e.initialize = true
         self.ha.bootstrap()
         self.p.is_leader = true
-        with patch.object(Watchdog, 'activate', Mock(return_value=False)),\
+        with patch.object(Watchdog, 'activate', Mock(return_value=False)), \
                 patch('patroni.ha.logger.error') as mock_logger:
             self.assertEqual(self.ha.post_bootstrap(), 'running post_bootstrap')
             self.assertRaises(PatroniFatalException, self.ha.post_bootstrap)
             self.assertTrue(mock_logger.call_args[0][0].startswith('Cancelling bootstrap because'
                                                                    ' watchdog activation failed'))
 
     @patch('patroni.psycopg.connect', psycopg_connect)
@@ -663,17 +671,17 @@
             self.assertEqual(self.ha.run_cycle(), 'restart in progress')
 
             self.ha.has_lock = true
             self.assertEqual(self.ha.run_cycle(), 'updated leader lock during restart')
 
             self.ha.update_lock = false
             self.p.set_role('primary')
-            with patch('patroni.async_executor.CriticalTask.cancel', Mock(return_value=False)),\
+            with patch('patroni.async_executor.CriticalTask.cancel', Mock(return_value=False)), \
                     patch('patroni.async_executor.CriticalTask.result',
-                          PropertyMock(return_value=PostmasterProcess(os.getpid())), create=True),\
+                          PropertyMock(return_value=PostmasterProcess(os.getpid())), create=True), \
                     patch('patroni.postgresql.Postgresql.terminate_starting_postmaster') as mock_terminate:
                 self.assertEqual(self.ha.run_cycle(), 'lost leader lock during restart')
                 mock_terminate.assert_called()
 
             self.ha.is_paused = true
             self.assertEqual(self.ha.run_cycle(), 'PAUSE: restart in progress')
 
@@ -879,15 +887,18 @@
         self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.patroni.nofailover = False
 
     def test_fetch_node_status(self):
         member = Member(0, 'test', 1, {'api_url': 'http://127.0.0.1:8011/patroni'})
         self.ha.fetch_node_status(member)
         member = Member(0, 'test', 1, {'api_url': 'http://localhost:8011/patroni'})
-        self.ha.fetch_node_status(member)
+        self.ha.patroni.request = Mock()
+        self.ha.patroni.request.return_value.data = b'{"wal":{"location":1},"role":"primary"}'
+        ret = self.ha.fetch_node_status(member)
+        self.assertFalse(ret.in_recovery)
 
     @patch.object(Rewind, 'pg_rewind', true)
     @patch.object(Rewind, 'check_leader_is_not_in_recovery', true)
     @patch('os.listdir', Mock(return_value=[]))
     @patch('patroni.postgresql.rewind.fsync_dir', Mock())
     def test_post_recover(self):
         self.p.is_running = false
@@ -1406,14 +1417,15 @@
     @patch('patroni.psycopg.connect', psycopg_connect)
     @patch('os.path.exists', Mock(return_value=True))
     @patch('shutil.rmtree', Mock())
     @patch('os.makedirs', Mock())
     @patch('os.open', Mock())
     @patch('os.fsync', Mock())
     @patch('os.close', Mock())
+    @patch('os.chmod', Mock())
     @patch('os.rename', Mock())
     @patch('patroni.postgresql.Postgresql.is_starting', Mock(return_value=False))
     @patch('builtins.open', mock_open())
     @patch.object(ConfigHandler, 'check_recovery_conf', Mock(return_value=(False, False)))
     @patch.object(Postgresql, 'major_version', PropertyMock(return_value=130000))
     @patch.object(SlotsHandler, 'sync_replication_slots', Mock(return_value=['ls']))
     def test_follow_copy(self):
```

### Comparing `patroni-3.0.4/tests/test_kubernetes.py` & `patroni-3.1.0/tests/test_kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import mock
 import socket
 import time
 import unittest
 import urllib3
 
 from mock import Mock, PropertyMock, mock_open, patch
-from patroni.dcs.kubernetes import Cluster, k8s_client, k8s_config, K8sConfig, K8sConnectionFailed,\
-    K8sException, K8sObject, Kubernetes, KubernetesError, KubernetesRetriableException,\
+from patroni.dcs.kubernetes import Cluster, k8s_client, k8s_config, K8sConfig, K8sConnectionFailed, \
+    K8sException, K8sObject, Kubernetes, KubernetesError, KubernetesRetriableException, \
     Retry, RetryFailedError, SERVICE_HOST_ENV_NAME, SERVICE_PORT_ENV_NAME
 from threading import Thread
 from . import MockResponse, SleepException
 
 
 def mock_list_namespaced_config_map(*args, **kwargs):
     metadata = {'resource_version': '1', 'labels': {'f': 'b'}, 'name': 'test-config',
@@ -82,28 +82,28 @@
 class TestK8sConfig(unittest.TestCase):
 
     def test_load_incluster_config(self):
         for env in ({}, {SERVICE_HOST_ENV_NAME: '', SERVICE_PORT_ENV_NAME: ''}):
             with patch('os.environ', env):
                 self.assertRaises(k8s_config.ConfigException, k8s_config.load_incluster_config)
 
-        with patch('os.environ', {SERVICE_HOST_ENV_NAME: 'a', SERVICE_PORT_ENV_NAME: '1'}),\
-                patch('os.path.isfile', Mock(side_effect=[False, True, True, False, True, True, True, True])),\
+        with patch('os.environ', {SERVICE_HOST_ENV_NAME: 'a', SERVICE_PORT_ENV_NAME: '1'}), \
+                patch('os.path.isfile', Mock(side_effect=[False, True, True, False, True, True, True, True])), \
                 patch('builtins.open', Mock(side_effect=[
                     mock_open()(), mock_open(read_data='a')(), mock_open(read_data='a')(),
                     mock_open()(), mock_open(read_data='a')(), mock_open(read_data='a')()])):
             for _ in range(0, 4):
                 self.assertRaises(k8s_config.ConfigException, k8s_config.load_incluster_config)
             k8s_config.load_incluster_config()
             self.assertEqual(k8s_config.server, 'https://a:1')
             self.assertEqual(k8s_config.headers.get('authorization'), 'Bearer a')
 
     def test_refresh_token(self):
-        with patch('os.environ', {SERVICE_HOST_ENV_NAME: 'a', SERVICE_PORT_ENV_NAME: '1'}),\
-                patch('os.path.isfile', Mock(side_effect=[True, True, False, True, True, True])),\
+        with patch('os.environ', {SERVICE_HOST_ENV_NAME: 'a', SERVICE_PORT_ENV_NAME: '1'}), \
+                patch('os.path.isfile', Mock(side_effect=[True, True, False, True, True, True])), \
                 patch('builtins.open', Mock(side_effect=[
                     mock_open(read_data='cert')(), mock_open(read_data='a')(),
                     mock_open()(), mock_open(read_data='b')(), mock_open(read_data='c')()])):
             k8s_config.load_incluster_config(token_refresh_interval=datetime.timedelta(milliseconds=100))
             self.assertEqual(k8s_config.headers.get('authorization'), 'Bearer a')
             time.sleep(0.1)
             # token file doesn't exist
@@ -134,18 +134,18 @@
         config["users"][0]["user"]["token"] = "token"
         with patch('builtins.open', mock_open(read_data=json.dumps(config))):
             k8s_config.load_kube_config()
             self.assertEqual(k8s_config.headers.get('authorization'), 'Bearer token')
 
         config["users"][0]["user"]["client-key-data"] = base64.b64encode(b'foobar').decode('utf-8')
         config["clusters"][0]["cluster"]["certificate-authority-data"] = base64.b64encode(b'foobar').decode('utf-8')
-        with patch('builtins.open', mock_open(read_data=json.dumps(config))),\
-                patch('os.write', Mock()), patch('os.close', Mock()),\
-                patch('os.remove') as mock_remove,\
-                patch('atexit.register') as mock_atexit,\
+        with patch('builtins.open', mock_open(read_data=json.dumps(config))), \
+                patch('os.write', Mock()), patch('os.close', Mock()), \
+                patch('os.remove') as mock_remove, \
+                patch('atexit.register') as mock_atexit, \
                 patch('tempfile.mkstemp') as mock_mkstemp:
             mock_mkstemp.side_effect = [(3, '1.tmp'), (4, '2.tmp')]
             k8s_config.load_kube_config()
             mock_atexit.assert_called_once()
             mock_remove.side_effect = OSError
             mock_atexit.call_args[0][0]()  # call _cleanup_temp_files
             mock_remove.assert_has_calls([mock.call('1.tmp'), mock.call('2.tmp')])
@@ -294,14 +294,36 @@
     def test_touch_member(self, mock_patch_namespaced_pod):
         mock_patch_namespaced_pod.return_value.metadata.resource_version = '10'
         self.k.touch_member({'role': 'replica'})
         self.k._name = 'p-1'
         self.k.touch_member({'state': 'running', 'role': 'replica'})
         self.k.touch_member({'state': 'stopped', 'role': 'primary'})
 
+        self.k._role_label = 'isMaster'
+        self.k._leader_label_value = 'true'
+        self.k._follower_label_value = 'false'
+        self.k._standby_leader_label_value = 'false'
+        self.k._tmp_role_label = 'tmp_role'
+
+        self.k.touch_member({'state': 'running', 'role': 'replica'})
+        mock_patch_namespaced_pod.assert_called()
+        self.assertEqual(mock_patch_namespaced_pod.call_args[0][2].metadata.labels['isMaster'], 'false')
+        self.assertEqual(mock_patch_namespaced_pod.call_args[0][2].metadata.labels['tmp_role'], 'replica')
+
+        self.k.touch_member({'state': 'running', 'role': 'standby-leader'})
+        mock_patch_namespaced_pod.assert_called()
+        self.assertEqual(mock_patch_namespaced_pod.call_args[0][2].metadata.labels['isMaster'], 'false')
+        self.assertEqual(mock_patch_namespaced_pod.call_args[0][2].metadata.labels['tmp_role'], 'standby-leader')
+
+        self.k._name = 'p-0'
+        self.k.touch_member({'role': 'primary'})
+        mock_patch_namespaced_pod.assert_called()
+        self.assertEqual(mock_patch_namespaced_pod.call_args[0][2].metadata.labels['isMaster'], 'true')
+        self.assertEqual(mock_patch_namespaced_pod.call_args[0][2].metadata.labels['tmp_role'], 'master')
+
     def test_initialize(self):
         self.k.initialize()
 
     def test_delete_leader(self):
         self.k.delete_leader(1)
 
     def test_cancel_initialization(self):
```

### Comparing `patroni-3.0.4/tests/test_log.py` & `patroni-3.1.0/tests/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         os.environ[Config.PATRONI_CONFIG_VARIABLE] = yaml.dump(config, default_flow_style=False)
         logger = PatroniLogger()
         patroni_config = Config(None)
         logger.reload_config(patroni_config['log'])
         _LOG.exception('test')
         logger.start()
 
-        with patch.object(logging.Handler, 'format', Mock(side_effect=Exception)),\
+        with patch.object(logging.Handler, 'format', Mock(side_effect=Exception)), \
                 patch('_pytest.logging.LogCaptureHandler.emit', Mock()):
             logging.error('test')
 
         self.assertEqual(logger.log_handler.maxBytes, config['log']['file_size'])
         self.assertEqual(logger.log_handler.backupCount, config['log']['file_num'])
 
         config['log']['level'] = 'DEBUG'
```

### Comparing `patroni-3.0.4/tests/test_patroni.py` & `patroni-3.1.0/tests/test_patroni.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_postgresql.py` & `patroni-3.1.0/tests/test_postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,29 +329,28 @@
     def test_write_postgresql_and_sanitize_auto_conf(self):
         read_data = 'primary_conninfo = foo\nfoo = bar\n'
         with open(os.path.join(self.p.data_dir, 'postgresql.auto.conf'), 'w') as f:
             f.write(read_data)
 
         mock_read_auto = mock_open(read_data=read_data)
         mock_read_auto.return_value.__iter__ = lambda o: iter(o.readline, '')
-        with patch('builtins.open', Mock(side_effect=[mock_open()(), mock_read_auto(), IOError])),\
+        with patch('builtins.open', Mock(side_effect=[mock_open()(), mock_read_auto(), IOError])), \
                 patch('os.chmod', Mock()):
             self.p.config.write_postgresql_conf()
 
         with patch('builtins.open', Mock(side_effect=[mock_open()(), IOError])), patch('os.chmod', Mock()):
             self.p.config.write_postgresql_conf()
         self.p.config.write_recovery_conf({'foo': 'bar'})
         self.p.config.write_postgresql_conf()
 
     @patch.object(Postgresql, 'is_running', Mock(return_value=False))
     @patch.object(Postgresql, 'start', Mock())
     def test_follow(self):
         self.p.call_nowait(CallbackAction.ON_START)
-        m = RemoteMember.from_name_and_data('1', {'restore_command': '2', 'primary_slot_name': 'foo',
-                                                  'conn_kwargs': {'host': 'bar'}})
+        m = RemoteMember('1', {'restore_command': '2', 'primary_slot_name': 'foo', 'conn_kwargs': {'host': 'bar'}})
         self.p.follow(m)
         with patch.object(Postgresql, 'ensure_major_version_is_known', Mock(return_value=False)):
             self.assertIsNone(self.p.follow(m))
 
     @patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError))
     def test__query(self):
         self.assertRaises(PostgresConnectionException, self.p._query, 'blabla')
@@ -492,16 +491,16 @@
     @patch('os.path.isdir', Mock(return_value=True))
     @patch('os.path.exists', Mock(return_value=True))
     def test_remove_data_directory(self):
         with patch('os.path.islink', Mock(return_value=True)):
             self.p.remove_data_directory()
         with patch('os.path.isfile', Mock(return_value=True)):
             self.p.remove_data_directory()
-        with patch('os.path.islink', Mock(side_effect=[False, False, True, True])),\
-                patch('os.listdir', Mock(return_value=['12345'])),\
+        with patch('os.path.islink', Mock(side_effect=[False, False, True, True])), \
+                patch('os.listdir', Mock(return_value=['12345'])), \
                 patch('os.path.realpath', Mock(side_effect=['../foo', '../foo_tsp'])):
             self.p.remove_data_directory()
 
     @patch('patroni.postgresql.Postgresql._version_file_exists', Mock(return_value=True))
     def test_controldata(self):
         with patch('subprocess.check_output', Mock(return_value=0, side_effect=pg_controldata_string)):
             data = self.p.controldata()
@@ -519,16 +518,17 @@
         self.assertEqual(self.p.sysid, "6200971513092291716")
 
     @patch('os.path.isfile', Mock(return_value=True))
     @patch('shutil.copy', Mock(side_effect=IOError))
     def test_save_configuration_files(self):
         self.p.config.save_configuration_files()
 
-    @patch('os.path.isfile', Mock(side_effect=[False, True]))
-    @patch('shutil.copy', Mock(side_effect=IOError))
+    @patch('os.path.isfile', Mock(side_effect=[False, True, False, True]))
+    @patch('shutil.copy', Mock(side_effect=[None, IOError]))
+    @patch('os.chmod', Mock())
     def test_restore_configuration_files(self):
         self.p.config.restore_configuration_files()
 
     def test_can_create_replica_without_replication_connection(self):
         self.p.config._config['create_replica_method'] = []
         self.assertFalse(self.p.can_create_replica_without_replication_connection(None))
         self.p.config._config['create_replica_method'] = ['wale', 'basebackup']
```

### Comparing `patroni-3.0.4/tests/test_postmaster.py` & `patroni-3.1.0/tests/test_postmaster.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_raft.py` & `patroni-3.1.0/tests/test_raft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 import tempfile
 import time
 
 from mock import Mock, PropertyMock, patch
-from patroni.dcs.raft import Cluster, DynMemberSyncObj, KVStoreTTL,\
+from patroni.dcs.raft import Cluster, DynMemberSyncObj, KVStoreTTL, \
     Raft, RaftError, SyncObjUtility, TCPTransport, _TCPTransport
 from pysyncobj import SyncObjConf, FAIL_REASON
 
 
 def remove_files(prefix):
     for f in ('journal', 'journal.meta', 'dump'):
         f = prefix + f
```

### Comparing `patroni-3.0.4/tests/test_raft_controller.py` & `patroni-3.1.0/tests/test_raft_controller.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_rewind.py` & `patroni-3.1.0/tests/test_rewind.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
         with patch('subprocess.call', side_effect=OSError):
             self.assertFalse(self.r.can_rewind)
         self.p.config._config['use_pg_rewind'] = False
         self.assertFalse(self.r.can_rewind)
 
     def test_pg_rewind(self):
         r = {'user': '', 'host': '', 'port': '', 'database': '', 'password': ''}
-        with patch.object(Postgresql, 'major_version', PropertyMock(return_value=150000)),\
+        with patch.object(Postgresql, 'major_version', PropertyMock(return_value=150000)), \
                 patch.object(CancellableSubprocess, 'call', Mock(return_value=None)):
             with patch('subprocess.check_output', Mock(return_value=b'boo')):
                 self.assertFalse(self.r.pg_rewind(r))
             with patch('subprocess.check_output', Mock(side_effect=Exception)):
                 self.assertFalse(self.r.pg_rewind(r))
 
-        with patch.object(Postgresql, 'major_version', PropertyMock(return_value=120000)),\
+        with patch.object(Postgresql, 'major_version', PropertyMock(return_value=120000)), \
                 patch('subprocess.check_output', Mock(return_value=b'foo %f %p %r %% % %')):
             with patch.object(CancellableSubprocess, 'call', mock_cancellable_call):
                 self.assertFalse(self.r.pg_rewind(r))
             with patch.object(CancellableSubprocess, 'call', mock_cancellable_call0):
                 self.assertTrue(self.r.pg_rewind(r))
             with patch.object(CancellableSubprocess, 'call', mock_cancellable_call1):
                 self.assertFalse(self.r.pg_rewind(r))
@@ -87,15 +87,15 @@
         with patch.object(Postgresql, 'controldata',
                           Mock(return_value={'Database cluster state': 'shut down in recovery',
                                              'Minimum recovery ending location': '0/0',
                                              "Min recovery ending loc's timeline": '0',
                                              'Latest checkpoint location': '0/'})):
             self.r.rewind_or_reinitialize_needed_and_possible(self.leader)
 
-        with patch.object(Postgresql, 'is_running', Mock(return_value=True)),\
+        with patch.object(Postgresql, 'is_running', Mock(return_value=True)), \
                 patch.object(MockCursor, 'fetchone',
                              Mock(side_effect=[(0, 0, 1, 1, 0, 0, 0, 0, 0, None, None, None), Exception])):
             self.r.rewind_or_reinitialize_needed_and_possible(self.leader)
 
     @patch.object(CancellableSubprocess, 'call', mock_cancellable_call)
     @patch.object(Postgresql, 'checkpoint', side_effect=['', '1'],)
     @patch.object(Postgresql, 'stop', Mock(return_value=False))
@@ -235,27 +235,31 @@
         with patch.object(Postgresql, 'get_guc_value', Mock(side_effect=get_guc_value_res)):
             for _ in range(len(get_guc_value_res) // 2):
                 self.r._archive_ready_wals()
                 mock_logger_info.assert_not_called()
 
         with patch('os.listdir', Mock(return_value=['000000000000000000000000.ready'])):
             # successful archive_command call
-            with patch.object(CancellableSubprocess, 'call', Mock(return_value=0)):
+            with patch.object(CancellableSubprocess, 'call', Mock(return_value=0)) as mock_subprocess_call:
                 get_guc_value_res = [
                     'on', 'command %f',
                     'always', 'command %f',
                 ]
                 with patch.object(Postgresql, 'get_guc_value', Mock(side_effect=get_guc_value_res)):
                     for _ in range(len(get_guc_value_res) // 2):
                         self.r._archive_ready_wals()
                         mock_logger_info.assert_called_once()
                         self.assertEqual(('Trying to archive %s: %s',
                                           '000000000000000000000000', 'command 000000000000000000000000'),
                                          mock_logger_info.call_args[0])
                         mock_logger_info.reset_mock()
+                        mock_subprocess_call.assert_called_once()
+                        self.assertEqual(mock_subprocess_call.call_args[0][0], ['command 000000000000000000000000'])
+                        self.assertEqual(mock_subprocess_call.call_args[1]['shell'], True)
+                        mock_subprocess_call.reset_mock()
 
             # failed archive_command call
             with patch.object(CancellableSubprocess, 'call', Mock(return_value=1)):
                 with patch.object(Postgresql, 'get_guc_value', Mock(side_effect=['on', 'command %f'])):
                     self.r._archive_ready_wals()
                     self.assertEqual(('Trying to archive %s: %s',
                                       '000000000000000000000000', 'command 000000000000000000000000'),
```

### Comparing `patroni-3.0.4/tests/test_slots.py` & `patroni-3.1.0/tests/test_slots.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,20 +39,20 @@
                                              'A': 0, 'ls': 0, 'b': {'type': 'logical', 'plugin': '1'}},
                                    'ignore_slots': [{'name': 'blabla'}]}, 1)
         cluster = Cluster(True, config, self.leader, 0, [self.me, self.other, self.leadermem],
                           None, SyncState.empty(), None, {'test_3': 10}, None)
         with mock.patch('patroni.postgresql.Postgresql._query', Mock(side_effect=psycopg.OperationalError)):
             self.s.sync_replication_slots(cluster, False)
         self.p.set_role('standby_leader')
-        with patch.object(SlotsHandler, 'drop_replication_slot', Mock(return_value=(True, False))),\
+        with patch.object(SlotsHandler, 'drop_replication_slot', Mock(return_value=(True, False))), \
                 patch('patroni.postgresql.slots.logger.debug') as mock_debug:
             self.s.sync_replication_slots(cluster, False)
             mock_debug.assert_called_once()
         self.p.set_role('replica')
-        with patch.object(Postgresql, 'is_leader', Mock(return_value=False)),\
+        with patch.object(Postgresql, 'is_leader', Mock(return_value=False)), \
                 patch.object(SlotsHandler, 'drop_replication_slot') as mock_drop:
             self.s.sync_replication_slots(cluster, False, paused=True)
             mock_drop.assert_not_called()
         self.p.set_role('primary')
         with mock.patch('patroni.postgresql.Postgresql.role', new_callable=PropertyMock(return_value='replica')):
             self.s.sync_replication_slots(cluster, False)
         with patch('patroni.dcs.logger.error', new_callable=Mock()) as errorlog_mock:
@@ -89,19 +89,19 @@
                   "confirmed_flush_lsn": 12345, "catalog_xmin": 105}])
             self.assertEqual(self.p.slots(), {})
 
     @patch.object(Postgresql, 'is_leader', Mock(return_value=False))
     def test__ensure_logical_slots_replica(self):
         self.p.set_role('replica')
         self.cluster.slots['ls'] = 12346
-        with patch.object(SlotsHandler, 'check_logical_slots_readiness', Mock()):
+        with patch.object(SlotsHandler, 'check_logical_slots_readiness', Mock(return_value=False)):
             self.assertEqual(self.s.sync_replication_slots(self.cluster, False), [])
         self.s._schedule_load_slots = False
-        with patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError)),\
-                patch.object(SlotsAdvanceThread, 'schedule', Mock(return_value=(True, ['ls']))),\
+        with patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError)), \
+                patch.object(SlotsAdvanceThread, 'schedule', Mock(return_value=(True, ['ls']))), \
                 patch.object(psycopg.OperationalError, 'diag') as mock_diag:
             type(mock_diag).sqlstate = PropertyMock(return_value='58P01')
             self.assertEqual(self.s.sync_replication_slots(self.cluster, False), ['ls'])
         self.cluster.slots['ls'] = 'a'
         self.assertEqual(self.s.sync_replication_slots(self.cluster, False), [])
         with patch.object(MockCursor, 'rowcount', PropertyMock(return_value=1), create=True):
             self.assertEqual(self.s.sync_replication_slots(self.cluster, False), ['ls'])
@@ -115,22 +115,22 @@
             self.s.copy_logical_slots(self.cluster, ['foo'])
 
     @patch.object(Postgresql, 'stop', Mock(return_value=True))
     @patch.object(Postgresql, 'start', Mock(return_value=True))
     @patch.object(Postgresql, 'is_leader', Mock(return_value=False))
     def test_check_logical_slots_readiness(self):
         self.s.copy_logical_slots(self.cluster, ['ls'])
-        with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('postgresql0', None)]))),\
+        with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('postgresql0', None)]))), \
                 patch.object(MockCursor, 'fetchone', Mock(side_effect=Exception)):
-            self.assertIsNone(self.s.check_logical_slots_readiness(self.cluster, False, None))
-        with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('postgresql0', None)]))),\
+            self.assertFalse(self.s.check_logical_slots_readiness(self.cluster, None))
+        with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('postgresql0', None)]))), \
                 patch.object(MockCursor, 'fetchone', Mock(return_value=(False,))):
-            self.assertIsNone(self.s.check_logical_slots_readiness(self.cluster, False, None))
+            self.assertFalse(self.s.check_logical_slots_readiness(self.cluster, None))
         with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('ls', 100)]))):
-            self.s.check_logical_slots_readiness(self.cluster, False, None)
+            self.s.check_logical_slots_readiness(self.cluster, None)
 
     @patch.object(Postgresql, 'stop', Mock(return_value=True))
     @patch.object(Postgresql, 'start', Mock(return_value=True))
     @patch.object(Postgresql, 'is_leader', Mock(return_value=False))
     def test_on_promote(self):
         self.s.schedule_advance_slots({'foo': {'bar': 100}})
         self.s.copy_logical_slots(self.cluster, ['ls'])
@@ -140,15 +140,15 @@
     @patch('os.open', Mock())
     @patch('os.close', Mock())
     @patch('os.fsync', Mock(side_effect=OSError))
     def test_fsync_dir(self):
         self.assertRaises(OSError, fsync_dir, 'foo')
 
     def test_slots_advance_thread(self):
-        with patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError)),\
+        with patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError)), \
                 patch.object(psycopg.OperationalError, 'diag') as mock_diag:
             type(mock_diag).sqlstate = PropertyMock(return_value='58P01')
             self.s.schedule_advance_slots({'foo': {'bar': 100}})
             self.s._advance.sync_slots()
 
         with patch.object(SlotsAdvanceThread, 'sync_slots', Mock(side_effect=Exception)):
             self.s._advance._condition.wait = Mock()
```

### Comparing `patroni-3.0.4/tests/test_sync.py` & `patroni-3.1.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_utils.py` & `patroni-3.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_validator.py` & `patroni-3.1.0/tests/test_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 available_dcs = [m.split(".")[-1] for m in dcs_modules()]
 config = {
     "name": "string",
     "scope": "string",
     "restapi": {
         "listen": "127.0.0.2:800",
-        "connect_address": "127.0.0.2:800"
+        "connect_address": "127.0.0.2:800",
+        "verify_client": 'none'
     },
     "bootstrap": {
         "dcs": {
             "ttl": 1000,
             "loop_wait": 1000,
             "retry_timeout": 1000,
             "maximum_lag_on_failover": 1000
```

### Comparing `patroni-3.0.4/tests/test_wale_restore.py` & `patroni-3.1.0/tests/test_wale_restore.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_watchdog.py` & `patroni-3.1.0/tests/test_watchdog.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.4/tests/test_zookeeper.py` & `patroni-3.1.0/tests/test_zookeeper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from kazoo.client import KazooClient, KazooState
 from kazoo.exceptions import NoNodeError, NodeExistsError
 from kazoo.handlers.threading import SequentialThreadingHandler
 from kazoo.protocol.states import KeeperState, ZnodeStat
 from kazoo.retry import RetryFailedError
 from mock import Mock, PropertyMock, patch
-from patroni.dcs.zookeeper import Cluster, Leader, PatroniKazooClient,\
+from patroni.dcs.zookeeper import Cluster, Leader, PatroniKazooClient, \
     PatroniSequentialThreadingHandler, ZooKeeper, ZooKeeperError
 
 
 class MockKazooClient(Mock):
 
     handler = PatroniSequentialThreadingHandler(10)
     leader = False
```

