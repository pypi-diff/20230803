# Comparing `tmp/rapyuta-io-cli-3.1.0.tar.gz` & `tmp/rapyuta-io-cli-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-3.1.0.tar", last modified: Wed Jun 14 14:34:11 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-4.0.0.tar", last modified: Thu Aug  3 12:50:03 2023, max compression
```

## Comparing `rapyuta-io-cli-3.1.0.tar` & `rapyuta-io-cli-4.0.0.tar`

### file list

```diff
@@ -1,213 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.461439 rapyuta-io-cli-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4645 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/riocli/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)    15434 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8273 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4480 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     4735 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/build/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/import_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/trigger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     3182 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)     1638 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    16564 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/jsonschema/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/organization/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/organization/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/organization/select.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/project/features/
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/features/vpn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/docker_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/import_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/source_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/usergroup/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/v2client/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/v2client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/v2client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/vpn/
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/ping.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/util.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 14:34:11.461439 rapyuta-io-cli-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/riocli/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     5051 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16402 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4039 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/import_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3223 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/constants/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/constants/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2801 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17137 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5745 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1857 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2745 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1739 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4481 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6455 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/organization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3479 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2628 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/project/features/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/features/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4157 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/docker_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/import_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/source_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/v2client/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/v2client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/v2client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/vpn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/setup.py
```

### Comparing `rapyuta-io-cli-3.1.0/PKG-INFO` & `rapyuta-io-cli-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 3.1.0
+Version: 4.0.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-3.1.0/README.md` & `rapyuta-io-cli-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 3.1.0
+Version: 4.0.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,25 +40,28 @@
 riocli/chart/info.py
 riocli/chart/list.py
 riocli/chart/search.py
 riocli/chart/util.py
 riocli/completion/__init__.py
 riocli/config/__init__.py
 riocli/config/config.py
+riocli/constants/__init__.py
+riocli/constants/colors.py
+riocli/constants/symbols.py
 riocli/deployment/__init__.py
 riocli/deployment/delete.py
 riocli/deployment/errors.py
 riocli/deployment/execute.py
 riocli/deployment/inspect.py
 riocli/deployment/list.py
 riocli/deployment/logs.py
 riocli/deployment/model.py
-riocli/deployment/run.py
 riocli/deployment/ssh.py
 riocli/deployment/status.py
+riocli/deployment/update.py
 riocli/deployment/util.py
 riocli/deployment/wait.py
 riocli/device/__init__.py
 riocli/device/config.py
 riocli/device/create.py
 riocli/device/delete.py
 riocli/device/deployment.py
@@ -107,14 +110,16 @@
 riocli/network/model.py
 riocli/network/native_network.py
 riocli/network/routed_network.py
 riocli/network/util.py
 riocli/organization/__init__.py
 riocli/organization/list.py
 riocli/organization/select.py
+riocli/organization/users.py
+riocli/organization/utils.py
 riocli/package/__init__.py
 riocli/package/create.py
 riocli/package/delete.py
 riocli/package/deployment.py
 riocli/package/inspect.py
 riocli/package/list.py
 riocli/package/model.py
@@ -158,15 +163,19 @@
 riocli/static_route/delete.py
 riocli/static_route/inspect.py
 riocli/static_route/list.py
 riocli/static_route/model.py
 riocli/static_route/open.py
 riocli/static_route/util.py
 riocli/usergroup/__init__.py
+riocli/usergroup/delete.py
+riocli/usergroup/inspect.py
 riocli/usergroup/list.py
+riocli/usergroup/model.py
+riocli/usergroup/util.py
 riocli/utils/__init__.py
 riocli/utils/context.py
 riocli/utils/execute.py
 riocli/utils/mermaid.py
 riocli/utils/selector.py
 riocli/utils/spinner.py
 riocli/utils/ssh_tunnel.py
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/__main__.py` & `rapyuta-io-cli-4.0.0/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/apply/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/apply/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 import click
 from click_help_colors import HelpColorsCommand
 
 from riocli.apply.explain import explain
 from riocli.apply.parse import Applier
 from riocli.apply.template import template
 from riocli.apply.util import process_files_values_secrets
+from riocli.constants import Colors
 
 
 @click.command(
     'apply',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 @click.option('--dryrun', '-d', is_flag=True, default=False,
               help='dry run the yaml files without applying any change')
 @click.option('--show-graph', '-g', is_flag=True, default=False,
               help='Opens a mermaid.live dependency graph')
 @click.option('--values', '-v',
               help="path to values yaml file. key/values "
@@ -43,37 +44,43 @@
                    "decoding files on this computer")
 @click.option('--workers', '-w',
               help="number of parallel workers while running apply "
                    "command. defaults to 6.", type=int)
 @click.option('-f', '--force', '--silent', 'silent', is_flag=True,
               type=click.BOOL, default=False,
               help="Skip confirmation")
+@click.option('--retry-count', '-rc', type=int, default=50,
+              help="Number of retries before a resource creation times out status, defaults to 50")
+@click.option('--retry-interval', '-ri', type=int, default=6,
+              help="Interval between retries defaults to 6")
 @click.argument('files', nargs=-1)
 def apply(
         values: str,
         secrets: str,
         files: Iterable[str],
+        retry_count: int,
+        retry_interval: int,
         dryrun: bool = False,
         workers: int = 6,
         silent: bool = False,
         show_graph: bool = False,
 ) -> None:
     """
     Apply resource manifests
     """
     glob_files, abs_values, abs_secrets = process_files_values_secrets(
         files, values, secrets)
 
     if len(glob_files) == 0:
-        click.secho('no files specified', fg='red')
+        click.secho('No files specified', fg=Colors.RED)
         raise SystemExit(1)
 
-    click.secho("----- Files Processed ----", fg="yellow")
+    click.secho("----- Files Processed ----", fg=Colors.YELLOW)
     for file in glob_files:
-        click.secho(file, fg="yellow")
+        click.secho(file, fg=Colors.YELLOW)
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies()
 
     if show_graph and dryrun:
         click.secho('You cannot dry run and launch the graph together.',
                     fg='yellow')
@@ -82,40 +89,50 @@
     if show_graph:
         rc.show_dependency_graph()
         return
 
     if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
 
-    rc.apply(dryrun=dryrun, workers=workers)
+    rc.apply(dryrun=dryrun, workers=workers, retry_count=retry_count, retry_interval=retry_interval)
 
 
 @click.command(
     'delete',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
-@click.option('--dryrun', '-d', is_flag=True, default=False, help='dry run the yaml files without applying any change')
+@click.option('--dryrun', '-d', is_flag=True, default=False,
+              help='dry run the yaml files without applying any change')
 @click.option('--values', '-v',
-              help="path to values yaml file. key/values specified in the values file can be used as variables in template yamls")
+              help="Path to values yaml file. key/values specified in the"
+                   " values file can be used as variables in template YAMLs")
 @click.option('--secrets', '-s',
-              help="secret files are sops encoded value files. rio-cli expects sops to be authorized for decoding files on this computer")
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
+              help="Secret files are sops encoded value files. riocli expects "
+                   "sops to be authorized for decoding files on this computer")
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True,
+              type=click.BOOL, default=False,
               help="Skip confirmation")
 @click.argument('files', nargs=-1)
-def delete(values: str, secrets: str, files: Iterable[str], dryrun: bool = False, silent: bool = False) -> None:
+def delete(
+        values: str,
+        secrets: str,
+        files: Iterable[str],
+        dryrun: bool = False,
+        silent: bool = False
+) -> None:
     """
     Removes resources defined in the manifest
     """
     glob_files, abs_values, abs_secrets = process_files_values_secrets(
         files, values, secrets)
 
     if len(glob_files) == 0:
-        click.secho('no files specified', fg='red')
+        click.secho('no files specified', fg=Colors.RED)
         raise SystemExit(1)
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies(check_missing=False, delete=True)
 
     if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/apply/explain.py` & `rapyuta-io-cli-4.0.0/riocli/apply/explain.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 
 import click
 from click_help_colors import HelpColorsCommand
 
+from riocli.constants import Colors, Symbols
+
 
 @click.command(
     'explain',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
     help='Generates a sample resource manifest for the given type'
 )
 @click.option('--templates', help='Alternate root for templates',
               default=None)
 @click.argument('resource')
 def explain(resource: str, templates: str = None) -> None:
     if templates:
@@ -35,9 +37,10 @@
 
     for each in path.glob('**/*'):
         if resource + '.yaml' == each.name:
             with open(each) as f:
                 click.echo_via_pager(f.readlines())
                 raise SystemExit(0)
 
-    click.secho("[Err] Resource \"{}\" not found".format(resource), fg='red')
+    click.secho('{} Resource "{}" not found'.format(Symbols.ERROR, resource),
+                fg=Colors.RED)
     raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/apply/parse.py` & `rapyuta-io-cli-4.0.0/riocli/apply/parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 import click
 import jinja2
 import yaml
 from tabulate import tabulate
 
 from riocli.apply.resolver import ResolverCache
 from riocli.config import Configuration
-from riocli.utils import dump_all_yaml
-from riocli.utils import print_separator
-from riocli.utils import run_bash
+from riocli.constants import Colors, Symbols
+from riocli.utils import dump_all_yaml, print_separator, run_bash
 from riocli.utils.mermaid import mermaid_link, mermaid_safe
+from riocli.utils.spinner import with_spinner
 
 
 class Applier(object):
     DEFAULT_MAX_WORKERS = 6
 
     EXPECTED_TIME = {
         "organization": 3,
@@ -75,36 +75,47 @@
 
         self._process_file_list(files)
 
     # Public Functions
     def order(self):
         return self.graph.static_order()
 
+    @with_spinner(text='Applying...', timer=True)
     def apply(self, *args, **kwargs):
+        spinner = kwargs.get('spinner')
         kwargs['workers'] = int(kwargs.get('workers')
                                 or self.DEFAULT_MAX_WORKERS)
+        apply_func = self.apply_async
         if kwargs['workers'] == 1:
-            return self.apply_sync(*args, **kwargs)
+            apply_func = self.apply_sync
 
-        return self.apply_async(*args, **kwargs)
+        try:
+            apply_func(*args, **kwargs)
+            spinner.text = 'Apply successful.'
+            spinner.green.ok(Symbols.SUCCESS)
+        except Exception as e:
+            spinner.text = 'Apply failed. Error: {}'.format(e)
+            spinner.red.fail(Symbols.ERROR)
 
     def apply_async(self, *args, **kwargs):
         workers = int(kwargs.get('workers') or self.DEFAULT_MAX_WORKERS)
         task_queue = queue.Queue()
         done_queue = queue.Queue()
 
         def worker():
             while True:
                 o = task_queue.get()
-                if o in self.resolved_objects and 'manifest' in self.resolved_objects[o]:
+                if o in self.resolved_objects and 'manifest' in \
+                        self.resolved_objects[o]:
                     try:
                         self._apply_manifest(o, *args, **kwargs)
                     except Exception as ex:
                         click.secho(
-                            '[Err] Object "{}" apply failed. Apply will not progress further.'.format(o, str(ex)))
+                            '[Err] Object "{}" apply failed. Apply will not progress further.'.format(
+                                o, str(ex)))
                         done_queue.put(ex)
                         continue
 
                 task_queue.task_done()
                 done_queue.put(o)
 
         worker_list = []
@@ -125,75 +136,88 @@
 
         task_queue.join()
 
     def apply_sync(self, *args, **kwargs):
         self.graph.prepare()
         while self.graph.is_active():
             for obj in self.graph.get_ready():
-                if obj in self.resolved_objects and 'manifest' in self.resolved_objects[obj]:
+                if (obj in self.resolved_objects and
+                        'manifest' in self.resolved_objects[obj]):
                     self._apply_manifest(obj, *args, **kwargs)
                 self.graph.done(obj)
 
+    @with_spinner(text='Deleting...', timer=True)
     def delete(self, *args, **kwargs):
+        spinner = kwargs.get('spinner')
         delete_order = list(self.graph.static_order())
         delete_order.reverse()
-        for obj in delete_order:
-            if obj in self.resolved_objects and 'manifest' in \
-                    self.resolved_objects[obj]:
-                self._delete_manifest(obj, *args, **kwargs)
+        try:
+            for obj in delete_order:
+                if (obj in self.resolved_objects and
+                        'manifest' in self.resolved_objects[obj]):
+                    self._delete_manifest(obj, *args, **kwargs)
+            spinner.text = 'Delete successful.'
+            spinner.green.ok(Symbols.SUCCESS)
+        except Exception as e:
+            spinner.text = 'Delete failed. Error: {}'.format(e)
+            spinner.red.fail(Symbols.ERROR)
 
     def print_resolved_manifests(self):
         manifests = [o for _, o in self.objects.items()]
         dump_all_yaml(manifests)
 
     def parse_dependencies(
             self,
             check_missing=True,
             delete=False,
-            template=False,
+            template=False
     ):
         number_of_objects = 0
         for f, data in self.files.items():
             for model in data:
                 key = self._get_object_key(model)
                 self._parse_dependency(key, model)
                 self._add_graph_node(key)
                 number_of_objects = number_of_objects + 1
 
         resource_list = []
         total_time = 0
 
         for node in copy.deepcopy(self.graph).static_order():
-
-            action = 'CREATE' if not self.resolved_objects[node]['src'] == 'remote' else 'UPDATE'
-            if delete:
+            action = 'UPDATE'
+            if not self.resolved_objects[node]['src'] == 'remote':
+                action = 'CREATE'
+            elif delete:
                 action = 'DELETE'
             kind = node.split(":")[0]
             expected_time = round(
                 self.EXPECTED_TIME.get(kind.lower(), 5) / 60, 2)
-            total_time = total_time + expected_time
+            total_time += expected_time
             resource_list.append([node, action, expected_time])
 
         if not template:
             self._display_context(
                 total_time=total_time,
                 total_objects=number_of_objects,
-                resource_list=resource_list,
+                resource_list=resource_list
             )
 
         if check_missing:
             missing_resources = []
             for key, item in self.resolved_objects.items():
                 if 'src' in item and item['src'] == 'missing':
                     missing_resources.append(key)
 
             if missing_resources:
-                click.secho("missing resources found in yaml. " +
-                            "Please ensure the following are either available in your yaml" +
-                            "or created on the server. {}".format(set(missing_resources)), fg="red")
+                click.secho(
+                    "Missing resources found in yaml. Please ensure the "
+                    "following are either available in your YAML or created"
+                    " on the server. {}".format(
+                        set(missing_resources)), fg=Colors.RED)
+
                 raise SystemExit(1)
 
     # Manifest Operations via base.py
     def _apply_manifest(self, obj_key, *args, **kwargs):
         obj = self.objects[obj_key]
         cls = ResolverCache.get_model(obj)
         ist = cls.from_dict(self.client, obj)
@@ -220,15 +244,15 @@
 
     def _register_object(self, data):
         try:
             key = self._get_object_key(data)
             self.objects[key] = data
             self.resolved_objects[key] = {'src': 'local', 'manifest': data}
         except KeyError:
-            click.secho("Key error {}".format(data), fg='red')
+            click.secho("Key error {}".format(data), fg=Colors.RED)
             return
 
     def _load_file_content(self, file_name, is_value=False, is_secret=False):
         if not is_secret:
             with open(file_name) as opened:
                 data = opened.read()
         else:
@@ -281,15 +305,16 @@
     def _add_graph_node(self, key):
         self.graph.add(key)
         self.diagram.append('\t{}[{}]'.format(mermaid_safe(key), key))
 
     def _add_graph_edge(self, dependent_key, key):
         self.graph.add(dependent_key, key)
         self.diagram.append('\t{}[{}] --> {}[{}] '.format(mermaid_safe(key),
-                                                          key, mermaid_safe(dependent_key), dependent_key))
+                                                          key, mermaid_safe(
+                dependent_key), dependent_key))
 
     # Dependency Resolution
     def _parse_dependency(self, dependent_key, model):
         for key, value in model.items():
             if key == "depends":
                 if 'kind' in value and value.get('kind'):
                     self._resolve_dependency(dependent_key, value)
@@ -324,15 +349,16 @@
 
             if kind == 'package':
                 if guid and obj_guid == guid:
                     self._add_remote_object_to_resolve_tree(
                         dependent_key, obj_guid, dependency, obj)
 
                 if (name_or_guid == obj_name) and (
-                        'version' in dependency and obj['packageVersion'] == dependency.get('version')):
+                        'version' in dependency and obj[
+                    'packageVersion'] == dependency.get('version')):
                     self._add_remote_object_to_resolve_tree(
                         dependent_key, obj_guid, dependency, obj)
 
             # Special handling for Static route since it doesn't have a name field.
             # StaticRoute sends a URLPrefix field with name being the prefix along with short org guid.
             elif kind == 'staticroute' and name_or_guid in obj_name:
                 self._add_remote_object_to_resolve_tree(
@@ -344,15 +370,16 @@
 
         self.dependencies[kind][name_or_guid] = {'local': True}
         self._add_graph_edge(dependent_key, key)
 
         if key not in self.resolved_objects:
             self.resolved_objects[key] = {'src': 'missing'}
 
-    def _add_remote_object_to_resolve_tree(self, dependent_key, guid, dependency, obj):
+    def _add_remote_object_to_resolve_tree(self, dependent_key, guid,
+                                           dependency, obj):
         kind = dependency.get('kind')
         name_or_guid = dependency.get('nameOrGUID')
         key = '{}:{}'.format(kind, name_or_guid)
         self.dependencies[kind][name_or_guid] = {
             'guid': guid, 'raw': obj, 'local': False}
         if key not in self.resolved_objects:
             self.resolved_objects[key] = {}
@@ -381,28 +408,28 @@
     # Utils
     def _display_context(
             self,
             total_time: int,
             total_objects: int,
             resource_list: typing.List
     ) -> None:
-        # Display context
-        headers = [click.style('Resource Context', bold=True, fg='yellow')]
+        headers = [
+            click.style('Resource Context', bold=True, fg=Colors.YELLOW)]
         context = [
             ['Expected Time (mins)', round(total_time, 2)],
             ['Files', len(self.files)],
             ['Resources', total_objects],
         ]
         click.echo(tabulate(context, headers=headers,
                             tablefmt='simple', numalign='center'))
 
         # Display Resource Inventory
         headers = []
         for header in ['Resource', 'Action', 'Expected Time (mins)']:
-            headers.append(click.style(header, fg='yellow', bold=True))
+            headers.append(click.style(header, fg=Colors.YELLOW, bold=True))
 
         print_separator()
         click.echo(tabulate(resource_list, headers=headers,
                             tablefmt='simple', numalign='center'))
         print_separator()
 
     @staticmethod
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/apply/resolver.py` & `rapyuta-io-cli-4.0.0/riocli/apply/resolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from riocli.disk.model import Disk
 from riocli.managedservice.model import ManagedService
 from riocli.network.model import Network
 from riocli.package.model import Package
 from riocli.project.model import Project
 from riocli.secret.model import Secret
 from riocli.static_route.model import StaticRoute
+from riocli.usergroup.model import UserGroup
 
 
 class _Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
@@ -51,15 +52,16 @@
         'Build': Build,
         'Device': Device,
         'Network': Network,
         'StaticRoute': StaticRoute,
         'Package': Package,
         'Disk': Disk,
         'Deployment': Deployment,
-        "ManagedService": ManagedService
+        "ManagedService": ManagedService,
+        'UserGroup': UserGroup,
     }
 
     KIND_REGEX = {
         "organization": "^org-[a-z]{24}$",
         "project": "^project-[a-z]{24}$",
         "secret": "^secret-[a-z]{24}$",
         "package": "^pkg-[a-z]{24}$",
@@ -95,15 +97,20 @@
 
     def find_depends(self, depends, *args):
         if 'depGuid' in depends and depends['kind'] == 'disk':
             return depends['depGuid'], None
         elif 'guid' in depends and depends['kind'] not in ('network', 'managedservice'):
             return depends['guid'], None
         elif 'nameOrGUID' in depends:
-            obj_list = self._list_functors(depends['kind'])()
+            if depends['kind'] == 'usergroup':
+                org_guid = depends['organization']
+                obj_list = self._list_functors(depends['kind'])(org_guid)
+            else:
+                obj_list = self._list_functors(depends['kind'])()
+
             obj_match = list(self._find_functors(depends['kind'])(
                 depends['nameOrGUID'], obj_list, *args))
             if not obj_list or (isinstance(obj_list, list) and len(obj_list) == 0):
                 return None, None
             if obj_match and isinstance(obj_match, list) and len(obj_match) > 0:
                 return self._guid_functor(depends['kind'])(obj_match[0]), obj_match[0]
             else:
@@ -114,19 +121,20 @@
         mapping = {
             'secret': lambda x: munchify(x).guid,
             "project": lambda x: munchify(x).metadata.guid,
             "package": lambda x: munchify(x)['id'],
             "staticroute": lambda x: munchify(x)['guid'],
             "build": lambda x: munchify(x)['guid'],
             "deployment": lambda x: munchify(x)['deploymentId'],
-            "network": lambda x: munchify(x)['guid'],
+            "network": lambda x: munchify(x).guid,
             # This is only temporarily like this
             "disk": lambda x: munchify(x)['internalDeploymentGUID'],
             "device": lambda x: munchify(x)['uuid'],
             "managedservice": lambda x: munchify(x)['metadata']['name'],
+            "usergroup": lambda x: munchify(x).guid
         }
         return mapping[kind]
 
     def _list_functors(self, kind):
         mapping = {
             'secret': self.client.list_secrets,
             "project": self.v2client.list_projects,
@@ -136,14 +144,15 @@
             "deployment": functools.partial(self.client.get_all_deployments,
                                             phases=[DeploymentPhaseConstants.SUCCEEDED,
                                                     DeploymentPhaseConstants.PROVISIONING]),
             "network": self._list_networks,
             "disk": self._list_disks,
             "device": self.client.get_all_devices,
             "managedservice": self._list_managedservices,
+            "usergroup": self.client.list_usergroups
         }
 
         return mapping[kind]
 
     def _find_functors(self, kind):
         mapping = {
             'secret': self._generate_find_guid_functor(),
@@ -154,14 +163,15 @@
                                                          obj_list),
             "build": self._generate_find_guid_functor(name_field='buildName'),
             "deployment": self._generate_find_guid_functor(),
             "network": self._generate_find_guid_functor(),
             "disk": self._generate_find_guid_functor(),
             "device": self._generate_find_guid_functor(),
             "managedservice": lambda name, instances: filter(lambda i: i.metadata.name == name, instances),
+            "usergroup": lambda name, groups: filter(lambda i: i.name == name, groups),
         }
 
         return mapping[kind]
 
     def _generate_find_guid_functor(self, name_field='name'):
         return lambda name, obj_list: filter(lambda x: name == getattr(x, name_field), obj_list)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/apply/template.py` & `rapyuta-io-cli-4.0.0/riocli/apply/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 from typing import Iterable
 
 import click
 from click_help_colors import HelpColorsCommand
 
 from riocli.apply.parse import Applier
 from riocli.apply.util import process_files_values_secrets
+from riocli.constants import Colors
 
 
 @click.command(
     'template',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 @click.option('--values', '-v',
-              help="path to values yaml file. key/values specified in the values file can be used as variables in template yamls")
+              help='Path to values yaml file. key/values specified in the '
+                   'values file can be used as variables in template YAMLs')
 @click.option('--secrets', '-s',
-              help="secret files are sops encoded value files. rio-cli expects sops to be authorized for decoding files on this computer")
+              help='Secret files are sops encoded value files. riocli '
+                   'expects sops to be authorized for decoding files on this computer')
 @click.argument('files', nargs=-1)
 def template(values: str, secrets: str, files: Iterable[str]) -> None:
     """
     Print manifests with filled values
     """
     glob_files, abs_values, abs_secrets = process_files_values_secrets(
         files, values, secrets)
 
     if len(glob_files) == 0:
-        click.secho('no files specified', fg='red')
+        click.secho('No files specified', fg=Colors.RED)
         raise SystemExit(1)
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.print_resolved_manifests()
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/apply/util.py` & `rapyuta-io-cli-4.0.0/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/auth/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,32 +18,33 @@
 from riocli.auth.login import login
 from riocli.auth.logout import logout
 from riocli.auth.refresh_token import refresh_token
 from riocli.auth.staging import environment
 from riocli.auth.status import status
 from riocli.auth.token import token
 from riocli.config import new_client
+from riocli.constants import Colors
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color="yellow",
-    help_options_color="green",
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def auth():
     """
     Account and Login on Rapyuta.io
     """
     pass
 
 
 def get_rio_client() -> Client:
     return new_client()
 
 
 auth.add_command(login)
 auth.add_command(logout)
-auth.add_command(status)
-auth.add_command(refresh_token)
 auth.add_command(token)
+auth.add_command(status)
 auth.add_command(environment)
+auth.add_command(refresh_token)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/login.py` & `rapyuta-io-cli-4.0.0/riocli/auth/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,23 +16,25 @@
 
 from riocli.auth.util import (
     get_token,
     select_organization,
     select_project,
     validate_token,
 )
+from riocli.constants import Colors, Symbols
 from riocli.utils.context import get_root_context
 
-LOGIN_SUCCESS = click.style('Logged in successfully!', fg='green')
+LOGIN_SUCCESS = click.style('{} Logged in successfully!'.format(Symbols.SUCCESS), fg=Colors.GREEN)
 
 
 @click.command(
+    'login',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 @click.option('--email', type=str,
               help='Email of the rapyuta.io account')
 @click.option('--password', type=str,
               help='Password for the rapyuta.io account')
 @click.option('--organization', type=str, default=None,
               help=('Context will be set to the organization after '
@@ -84,41 +86,42 @@
         ctx.obj.data['password'] = password
         ctx.obj.data['auth_token'] = get_token(email, password)
 
     # Save if the file does not already exist
     if not ctx.obj.exists or not interactive:
         ctx.obj.save()
     else:
-        click.secho("[Warning] rio already has a config file present",
-                    fg='yellow')
-        click.confirm('Do you want to override the config?', abort=True)
+        click.confirm(
+            '{} Config already exists. Do you want to override'
+            ' the existing config?'.format(Symbols.WARNING),
+            abort=True)
 
     if not interactive:
         # When just the email and password are provided
         if not project and not organization:
             click.echo(LOGIN_SUCCESS)
             return
 
         # When project is provided without an organization.
         # It is quite possible to have a project with the
         # same name in two organizations. Hence, organization
         # needs to be explicitly provided in this case.
         if project and not organization:
             click.secho(
                 'Please specify an organization. See `rio auth login --help`',
-                fg='yellow')
+                fg=Colors.YELLOW)
             raise SystemExit(1)
 
         # When just the organization is provided, we save the
         # organization name and id and the login is marked as
         # successful.
         if organization and not project:
             select_organization(ctx.obj, organization=organization)
             click.secho("Your organization is set to '{}'".format(
-                ctx.obj.data['organization_name']), fg='green')
+                ctx.obj.data['organization_name']), fg=Colors.CYAN)
             ctx.obj.save()
             click.echo(LOGIN_SUCCESS)
             return
 
     organization = select_organization(ctx.obj, organization=organization)
     select_project(ctx.obj, project=project, organization=organization)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/logout.py` & `rapyuta-io-cli-4.0.0/riocli/utils/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
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
-import click
+from click import Context
 
 
-@click.command()
-@click.pass_context
-def logout(ctx: click.Context):
+def get_root_context(ctx: Context) -> Context:
     """
-    Log out from the Rapyuta.io account using the CLI.
-    """
-
-    if not ctx.obj.exists:
-        return
+    get_root_context figures out the top-level Context from the given context by walking down the linked-list.
 
-    ctx.obj.data.pop('auth_token', None)
-    ctx.obj.data.pop('password', None)
-    ctx.obj.data.pop('email_id', None)
-    ctx.obj.data.pop('project_id', None)
-    ctx.obj.save()
+    https://click.palletsprojects.com/en/8.0.x/complex/#contexts
+    """
+    while True:
+        if ctx.parent is None:
+            return ctx
 
-    click.secho('Logged out successfully!', fg='green')
+        ctx = ctx.parent
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/refresh_token.py` & `rapyuta-io-cli-4.0.0/riocli/managedservice/delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
+
 import click
 
-from riocli.auth.util import get_token
-from riocli.exceptions import LoggedOut
+from riocli.config import new_v2_client
 
 
-@click.command()
-@click.pass_context
-def refresh_token(ctx: click.Context):
+@click.command('delete')
+@click.argument('instance-name', required=True)
+def delete_instance(instance_name: str):
     """
-    Refreshes the authentication Token after it expires
+    Delete a managedservice instance
     """
-
-    email = ctx.obj.data.get('email_id', None)
-    password = ctx.obj.data.get('password', None)
-    if not ctx.obj.exists or not email or not password:
-        raise LoggedOut
-
-    ctx.obj.data['auth_token'] = get_token(email, password)
-
-    ctx.obj.save()
-    click.echo('Token refreshed successfully!')
+    try:
+        client = new_v2_client()
+        r = client.delete_instance(instance_name)
+        if r.get('success', None):
+            click.secho("✅ Deleted instance '{}'".format(instance_name), fg='green')
+    except Exception as e:
+        click.secho(str(e), fg='red')
+        raise SystemExit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/staging.py` & `rapyuta-io-cli-4.0.0/riocli/auth/staging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,28 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 
 from riocli.auth.login import select_project, select_organization
 from riocli.auth.util import get_token
 from riocli.config import Configuration
+from riocli.constants import Colors, Symbols
 from riocli.utils.context import get_root_context
 
 _STAGING_ENVIRONMENT_SUBDOMAIN = "apps.okd4v2.okd4beta.rapyuta.io"
 _NAMED_ENVIRONMENTS = ["v11", "v12", "v13", "v14", "v15", "qa", "dev"]
 
 
 @click.command('environment', hidden=True)
 @click.argument('name', type=str)
 @click.pass_context
 def environment(ctx: click.Context, name: str):
     """
     Sets the Rapyuta.io environment to use (Internal use)
     """
-
     ctx = get_root_context(ctx)
 
     if name == 'ga':
         ctx.obj.data.pop('environment', None)
         ctx.obj.data.pop('catalog_host', None)
         ctx.obj.data.pop('core_api_host', None)
         ctx.obj.data.pop('rip_host', None)
@@ -46,26 +46,24 @@
     password = ctx.obj.data.get('password', None)
     ctx.obj.save()
 
     ctx.obj.data['auth_token'] = get_token(email, password)
 
     organization = select_organization(ctx.obj)
     select_project(ctx.obj, organization=organization)
-    ctx.obj.save()
 
-
-def _validate_environment(name: str) -> bool:
-    valid = name in _NAMED_ENVIRONMENTS or name.startswith('pr')
-    if not valid:
-        click.secho('Invalid staging environment!', fg='red')
-        raise SystemExit(1)
+    ctx.obj.save()
 
 
 def _configure_environment(config: Configuration, name: str) -> None:
-    _validate_environment(name)
+    is_valid_env = name in _NAMED_ENVIRONMENTS or name.startswith('pr')
+
+    if not is_valid_env:
+        click.secho('{} Invalid environment: {}'.format(Symbols.ERROR, name), fg=Colors.RED)
+        raise SystemExit(1)
 
     catalog = 'https://{}catalog.{}'.format(name, _STAGING_ENVIRONMENT_SUBDOMAIN)
     core = 'https://{}apiserver.{}'.format(name, _STAGING_ENVIRONMENT_SUBDOMAIN)
     rip = 'https://{}rip.{}'.format(name, _STAGING_ENVIRONMENT_SUBDOMAIN)
     v2api = 'https://{}api.{}'.format(name, _STAGING_ENVIRONMENT_SUBDOMAIN)
 
     config.data['environment'] = name
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/status.py` & `rapyuta-io-cli-4.0.0/riocli/shell/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,20 +10,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 
 
-@click.command()
 @click.pass_context
-def status(ctx: click.Context):
-    """
-    Shows the Login status of the CLI
-    """
-
-    if not ctx.obj.exists:
-        click.secho('Logged out 🔒', fg='red')
-        raise SystemExit(1)
-
-    if 'auth_token' in ctx.obj.data:
-        click.secho('Logged in 🎉', fg='green')
+def prompt_callback(ctx: click.Context) -> str:
+    organization_name = ctx.obj.data['organization_name']
+    project_name = ctx.obj.data['project_name']
+    return '{}:{} > '.format(organization_name, project_name)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/token.py` & `rapyuta-io-cli-4.0.0/riocli/auth/token.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
+from click_help_colors import HelpColorsCommand
 
 from riocli.auth.util import get_token, TOKEN_LEVELS
 from riocli.config import Configuration
+from riocli.constants import Colors
 from riocli.exceptions import LoggedOut
 
 
-@click.command()
+@click.command(
+    'token',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option("--email", default=None, help="Email of the Rapyuta.io account")
 @click.option("--password", default=None, hide_input=True,
               help="Password for the Rapyuta.io account")
 @click.option("--level", default=0,
               help="Level of the token. 0 = low, 1 = med, 2 = high")
 def token(email: str, password: str, level: int = 0):
     """
     Generates a fresh rapyuta.io auth token
     """
     config = Configuration()
 
     if level not in TOKEN_LEVELS:
-        click.secho('Invalid token level. Valid levels are {0}'.format(
-            list(TOKEN_LEVELS.keys())), fg='red')
+        click.secho(
+            'Invalid token level. Valid levels are {0}'.format(
+                list(TOKEN_LEVELS.keys())), fg=Colors.RED)
         raise SystemExit(1)
 
     if not email:
         email = config.data.get("email_id", None)
 
     if not password:
         password = config.data.get("password", None)
 
     if not config.exists or not email or not password:
         raise LoggedOut
 
-    click.echo(get_token(email, password, level))
+    new_token = get_token(email, password)
+    click.echo(new_token)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/auth/util.py` & `rapyuta-io-cli-4.0.0/riocli/auth/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,26 +10,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 import click
-from click_spinner import spinner
 from rapyuta_io import Client
 from rapyuta_io.clients.rip_client import AuthTokenLevel
 from rapyuta_io.utils import UnauthorizedError
 
 from riocli.config import Configuration
+from riocli.constants import Colors, Symbols
 from riocli.project.util import find_project_guid, find_organization_guid
 from riocli.utils.selector import show_selection
+from riocli.utils.spinner import with_spinner
+
+TOKEN_LEVELS = {
+    0: AuthTokenLevel.LOW,
+    1: AuthTokenLevel.MED,
+    2: AuthTokenLevel.HIGH
+}
 
 
-def select_organization(config: Configuration,
-                        organization: str = None) -> str:
+def select_organization(
+        config: Configuration,
+        organization: str = None,
+) -> str:
+    """
+    Launches the org selection prompt by listing all the orgs that the user is a part of.
+
+    Sets the choice in the given configuration.
+    """
     client = config.new_client(with_project=False)
 
     org_guid = None
 
     if organization:
         org_guid = organization if organization.startswith(
             'org-') else find_organization_guid(client, name=organization)
@@ -40,43 +54,47 @@
 
     org_map = {o.guid: o.name for o in organizations}
 
     if not org_guid:
         org_guid = show_selection(org_map, "Select an organization:")
 
     if org_guid and org_guid not in org_map:
-        click.secho('invalid organization guid', fg='red')
+        click.secho('invalid organization guid', fg=Colors.RED)
         raise SystemExit(1)
 
     config.data['organization_id'] = org_guid
     config.data['organization_name'] = org_map[org_guid]
 
     return org_guid
 
 
-def select_project(config: Configuration, project: str = None,
-                   organization: str = None) -> None:
+def select_project(
+        config: Configuration,
+        project: str = None,
+        organization: str = None,
+) -> None:
     """
     Launches the project selection prompt by listing all the projects.
+
     Sets the choice in the given configuration.
     """
     client = config.new_v2_client(with_project=False)
 
     project_guid = None
     if project:
         project_guid = (project if project.startswith('project-') else
                         find_project_guid(client, project,
                                           organization=organization))
 
     projects = client.list_projects(organization_guid=organization)
     if len(projects) == 0:
         config.data['project_id'] = ""
         config.data['project_name'] = ""
-        click.secho("There are no projects in this organization", fg='black',
-                    bg='white')
+        click.secho("There are no projects in this organization",
+                    fg=Colors.BLACK, bg=Colors.WHITE)
         return
 
     # Sort projects based on their names for an easier selection
     projects = sorted(projects, key=lambda p: p.metadata.name.lower())
     project_map = dict()
 
     for project in projects:
@@ -89,57 +107,62 @@
     config.data['project_id'] = project_guid
     config.data['project_name'] = project_map[project_guid]
 
     confirmation = "Your project has been set to '{}' in the organization '{}'".format(
         config.data['project_name'], config.data['organization_name'],
     )
 
-    click.secho(confirmation, fg='green')
+    click.secho(confirmation, fg=Colors.GREEN)
 
 
-TOKEN_LEVELS = {
-    0: AuthTokenLevel.LOW,
-    1: AuthTokenLevel.MED,
-    2: AuthTokenLevel.HIGH
-}
-
-
-def get_token(email: str, password: str, level: int = 1) -> str:
+@with_spinner(text='Fetching token...')
+def get_token(
+        email: str,
+        password: str,
+        level: int = 1,
+        spinner=None,
+) -> str:
     """
     Generates a new token using email and password.
     """
     config = Configuration()
     if 'environment' in config.data:
         os.environ['RIO_CONFIG'] = config.filepath
 
     try:
-        with spinner():
-            token = Client.get_auth_token(
-                email, password, TOKEN_LEVELS[level])
+        token = Client.get_auth_token(
+            email, password, TOKEN_LEVELS[level])
         return token
-    except UnauthorizedError:
-        click.secho("✘ incorrect email/password", fg='red')
-        raise SystemExit(1)
+    except UnauthorizedError as e:
+        spinner.text = click.style("incorrect email/password", fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
     except Exception as e:
-        click.secho(e, fg='red')
-        raise SystemExit(1)
+        click.style(str(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
 
 
-def validate_token(token: str) -> bool:
+@with_spinner(text='Validating token...')
+def validate_token(token: str, spinner=None) -> bool:
     """Validates an auth token."""
     config = Configuration()
     if 'environment' in config.data:
         os.environ['RIO_CONFIG'] = config.filepath
 
     client = Client(auth_token=token)
 
     try:
         user = client.get_authenticated_user()
-        click.secho('Token belongs to user {}'.format(user.email_id),
-                    fg='cyan')
+        spinner.text = click.style(
+            'Token belongs to user {}'.format(user.email_id),
+            fg=Colors.CYAN)
+        spinner.ok(Symbols.INFO)
         return True
     except UnauthorizedError:
-        click.secho("✘ incorrect auth token", fg='red')
+        spinner.text = click.style("incorrect auth token", fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         return False
     except Exception as e:
-        click.secho(e, fg='red')
+        spinner.text = click.style(str(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/bootstrap.py` & `rapyuta-io-cli-4.0.0/riocli/device/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,59 @@
-# -*- coding: utf-8 -*-
 # Copyright 2021 Rapyuta Robotics
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
-
-__version__ = "3.1.0"
-
 import click
-import rapyuta_io.version
-from click import Context
 from click_help_colors import HelpColorsGroup
-from click_plugins import with_plugins
-from pkg_resources import iter_entry_points
 
-from riocli.apply import apply, explain, delete, template
-from riocli.auth import auth
-from riocli.build import build
-from riocli.chart import chart
-from riocli.completion import completion
-from riocli.config import Configuration
-from riocli.deployment import deployment
-from riocli.device import device
-from riocli.disk import disk
-from riocli.managedservice import managedservice
-from riocli.network import network
-from riocli.organization import organization
-from riocli.package import package
-from riocli.parameter import parameter
-from riocli.project import project
-from riocli.rosbag import rosbag
-from riocli.secret import secret
-from riocli.shell import shell, deprecated_repl
-from riocli.static_route import static_route
-from riocli.vpn import vpn
+from riocli.device.config import device_config
+from riocli.device.create import create_device
+from riocli.device.delete import delete_device
+from riocli.device.deployment import list_deployments
+from riocli.device.execute import execute_command
+from riocli.device.files import device_uploads
+from riocli.device.inspect import inspect_device
+from riocli.device.label import device_labels
+from riocli.device.list import list_devices
+from riocli.device.metric import device_metrics
+from riocli.device.onboard import device_onboard
+from riocli.device.tools import tools
+from riocli.device.topic import device_topics
+from riocli.device.vpn import toggle_vpn
 
 
-@with_plugins(iter_entry_points('riocli.plugins'))
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color="yellow",
-    help_options_color="green",
+    help_headers_color='yellow',
+    help_options_color='green',
 )
-@click.pass_context
-def cli(ctx: Context, config: str = None):
-    ctx.obj = Configuration(filepath=config)
-
-
-@cli.command("help")
-@click.pass_context
-def cli_help(ctx):
-    """
-    Prints the help message
-    """
-    click.echo(cli.get_help(ctx))
-
-
-@cli.command()
-def version():
+def device():
     """
-    Version of the CLI/SDK
+    Devices on Rapyuta.io
     """
-    click.echo("rio {} / SDK {}".format(__version__, rapyuta_io.__version__))
-    return
+    pass
 
 
-cli.add_command(apply)
-cli.add_command(chart)
-cli.add_command(explain)
-cli.add_command(delete)
-cli.add_command(auth)
-cli.add_command(project)
-cli.add_command(device)
-cli.add_command(build)
-cli.add_command(secret)
-cli.add_command(package)
-cli.add_command(deployment)
-cli.add_command(static_route)
-cli.add_command(rosbag)
-cli.add_command(network)
-cli.add_command(completion)
-cli.add_command(parameter)
-cli.add_command(disk)
-cli.add_command(shell)
-cli.add_command(deprecated_repl)
-cli.add_command(managedservice)
-cli.add_command(template)
-cli.add_command(organization)
-cli.add_command(vpn)
+device.add_command(create_device)
+device.add_command(execute_command)
+device.add_command(delete_device)
+device.add_command(device_config)
+device.add_command(device_onboard)
+device.add_command(device_labels)
+device.add_command(device_metrics)
+device.add_command(device_topics)
+device.add_command(device_uploads)
+device.add_command(inspect_device)
+device.add_command(list_deployments)
+device.add_command(list_devices)
+device.add_command(tools)
+device.add_command(toggle_vpn)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/create.py` & `rapyuta-io-cli-4.0.0/riocli/build/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/delete.py` & `rapyuta-io-cli-4.0.0/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/import_build.py` & `rapyuta-io-cli-4.0.0/riocli/build/import_build.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/list.py` & `rapyuta-io-cli-4.0.0/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/logs.py` & `rapyuta-io-cli-4.0.0/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/model.py` & `rapyuta-io-cli-4.0.0/riocli/build/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         guid, obj = self.rc.find_depends(
             {"kind": "build", "nameOrGUID": self.metadata.name})
         if not guid:
             return False
 
         return obj
 
-    def create_object(self, client: Client) -> v1Build:
+    def create_object(self, client: Client, **kwargs) -> v1Build:
         build = client.create_build(build=self.to_v1())
         return build
 
     def update_object(self, client: Client, obj: typing.Any) -> None:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/trigger.py` & `rapyuta-io-cli-4.0.0/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/build/util.py` & `rapyuta-io-cli-4.0.0/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/chart/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,21 +15,22 @@
 from click_help_colors import HelpColorsGroup
 
 from riocli.chart.apply import apply_chart
 from riocli.chart.delete import delete_chart
 from riocli.chart.info import info_chart
 from riocli.chart.list import list_charts
 from riocli.chart.search import search_chart
+from riocli.constants import Colors
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def chart() -> None:
     """
     Rapyuta Charts is a way to package the complete Application for
     Rapyuta.io Platform.
     """
     pass
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/apply.py` & `rapyuta-io-cli-4.0.0/riocli/chart/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,21 +13,22 @@
 # limitations under the License.
 
 import click
 from click_help_colors import HelpColorsCommand
 
 from riocli.chart.chart import Chart
 from riocli.chart.util import find_chart
+from riocli.constants import Colors
 
 
 @click.command(
     'apply',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
     help='Apply a new Rapyuta Chart in the Project',
 )
 @click.option('--dryrun', '-d', is_flag=True, default=False,
               help='dry run the yaml files without applying any change')
 @click.option('-f', '--force', '--silent', 'silent', is_flag=True,
               type=click.BOOL, default=False,
               help="Skip confirmation")
@@ -50,13 +51,13 @@
         workers: int = 6,
         silent: bool = False) -> None:
     """Install a chart from the rapyuta-charts repository."""
     versions = find_chart(chart)
     if len(versions) > 1:
         click.secho(
             'More than one charts are available, please specify the version!',
-            fg='red')
+            fg=Colors.RED)
 
     chart = Chart(**versions[0])
     chart.apply_chart(values, secrets, dryrun=dryrun, workers=workers,
                       silent=silent)
     chart.cleanup()
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/chart.py` & `rapyuta-io-cli-4.0.0/riocli/chart/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,14 +16,15 @@
 from tempfile import TemporaryDirectory
 
 import click
 import requests
 from munch import Munch
 
 from riocli.apply import apply, delete
+from riocli.constants import Colors
 
 
 class Chart(Munch):
     def __init__(self, *args, **kwargs):
         super(Chart, self).__init__(*args, **kwargs)
         self.tmp_dir = None
         self.downloaded = False
@@ -62,15 +63,15 @@
 
         delete.callback(values=values, files=[templates_dir], secrets=secrets,
                         dryrun=dryrun, silent=silent)
 
     def download_chart(self):
         self._create_temp_directory()
         click.secho('Downloading {}:{} chart in {}'.format(
-            self.name, self.version, self.tmp_dir.name), fg='cyan')
+            self.name, self.version, self.tmp_dir.name), fg=Colors.CYAN)
         chart_filepath = Path(self.tmp_dir.name, self._chart_filename())
 
         with open(chart_filepath, 'wb') as f:
             resp = requests.get(self.urls[0])
             f.write(resp.content)
 
         self.extract_chart()
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/delete.py` & `rapyuta-io-cli-4.0.0/riocli/chart/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,21 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsCommand
 
 from riocli.chart.chart import Chart
 from riocli.chart.util import find_chart
+from riocli.constants import Colors
 
 
 @click.command(
     'delete',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
     help='Delete the Rapyuta Chart from the Project',
 )
 @click.option('--dryrun', '-d', is_flag=True, default=False,
               help='Dry run the yaml files without applying any change')
 @click.option('-f', '--force', '--silent', 'silent', is_flag=True,
               type=click.BOOL, default=False, help="Skip confirmation")
 @click.option('--values', '-v',
@@ -43,13 +44,13 @@
         secrets: str,
         dryrun: bool = False,
         silent: bool = False) -> None:
     """Uninstall a chart."""
     versions = find_chart(chart)
     if len(versions) > 1:
         click.secho('More than one charts are available, '
-                    'please specify the version!', fg='yellow')
+                    'please specify the version!', fg=Colors.YELLOW)
 
     chart = Chart(**versions[0])
     chart.delete_chart(values=values, secrets=secrets,
                        dryrun=dryrun, silent=silent)
     chart.cleanup()
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/info.py` & `rapyuta-io-cli-4.0.0/riocli/chart/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,22 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 from click_help_colors import HelpColorsCommand
 
 from riocli.chart.util import find_chart
+from riocli.constants import Colors
 from riocli.utils import dump_all_yaml
 
 
 @click.command(
     'info',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
     help='Describe the available chart with versions',
 )
 @click.argument('chart', type=str)
 def info_chart(chart: str) -> None:
     """Print a chart's details."""
     versions = find_chart(chart)
     dump_all_yaml(versions)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/list.py` & `rapyuta-io-cli-4.0.0/riocli/chart/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,21 +13,22 @@
 # limitations under the License.
 
 import click
 from click_help_colors import HelpColorsCommand
 from munch import munchify
 
 from riocli.chart.util import fetch_index, print_chart_entries
+from riocli.constants import Colors
 
 
 @click.command(
     'list',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 @click.option('-w', '--wide', is_flag=True, default=False,
               help='Print more details')
 def list_charts(wide: bool = False) -> None:
     """List all available charts."""
     index = fetch_index()
     if 'entries' not in index:
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/search.py` & `rapyuta-io-cli-4.0.0/riocli/chart/search.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,25 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 from click_help_colors import HelpColorsCommand
+from yaspin.api import Yaspin
 
 from riocli.chart.util import find_chart, print_chart_entries
+from riocli.constants import Colors, Symbols
+from riocli.utils.spinner import with_spinner
 
 
 @click.command(
     'search',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
     help='Search for available charts in the repository',
 )
 @click.option('-w', '--wide', is_flag=True, default=False,
               help='Print more details')
 @click.argument('chart', type=str)
-def search_chart(chart: str, wide: bool = False) -> None:
+@with_spinner(text="Searching for chart...")
+def search_chart(chart: str, wide: bool = False,
+                 spinner: Yaspin = None) -> None:
     """Search for a chart in the chart repo."""
-    versions = find_chart(chart)
-    print_chart_entries(versions, wide=wide)
+    try:
+        versions = find_chart(chart)
+        with spinner.hidden():
+            print_chart_entries(versions, wide=wide)
+    except Exception as e:
+        spinner.text = click.style(str(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/chart/util.py` & `rapyuta-io-cli-4.0.0/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/completion/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/config/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/config/config.py` & `rapyuta-io-cli-4.0.0/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,29 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.constants import Colors
 from riocli.deployment.delete import delete_deployment
+from riocli.deployment.execute import execute_command
+from riocli.deployment.execute import execute_command
 from riocli.deployment.inspect import inspect_deployment
 from riocli.deployment.list import list_deployments
 from riocli.deployment.logs import deployment_logs
 from riocli.deployment.ssh import ssh_init, ssh_deployment
 from riocli.deployment.status import status
+from riocli.deployment.update import update_deployment
 from riocli.deployment.wait import wait_for_deployment
-from riocli.deployment.execute import execute_command
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def deployment():
     """
     Deployment of the packages
     """
     pass
 
@@ -42,7 +45,8 @@
 deployment.add_command(list_deployments)
 deployment.add_command(deployment_logs)
 deployment.add_command(wait_for_deployment)
 deployment.add_command(status)
 deployment.add_command(ssh_deployment)
 deployment.add_command(ssh_init)
 deployment.add_command(execute_command)
+deployment.add_command(update_deployment)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/delete.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/status.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.deployment.util import name_to_guid
 
 
-@click.command('delete')
-@click.option('--force', '-f', '--silent', is_flag=True, default=False,
-              help='Skip confirmation')
+@click.command(
+    'status',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('deployment-name', type=str)
 @name_to_guid
-def delete_deployment(force: bool, deployment_name: str, deployment_guid: str) -> None:
+def status(deployment_name: str, deployment_guid: str) -> None:
     """
-    Delete the deployment from the Platform
+    Current status of the deployment
     """
-    if not force:
-        click.confirm('Deleting {} ({}) deployment'.format(deployment_name, deployment_guid), abort=True)
-
     try:
-        with spinner():
-            client = new_client()
-            deployment = client.get_deployment(deployment_guid)
-            deployment.deprovision()
-        click.secho('Deployment deleted successfully!', fg='green')
+        client = new_client()
+        deployment = client.get_deployment(deployment_guid)
+        click.secho(deployment.status)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/errors.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/execute.py` & `rapyuta-io-cli-4.0.0/riocli/device/execute.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,36 +7,51 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
+import typing
 
 import click
-import typing
+from click_help_colors import HelpColorsCommand
 
-from riocli.deployment.util import name_to_guid, select_details
-from riocli.utils.execute import run_on_cloud
+from riocli.constants import Colors
+from riocli.device.util import name_to_guid
+from riocli.utils.execute import run_on_device
 
 
-@click.command('execute')
-@click.option('--component', 'component_name', default=None)
-@click.option('--exec', 'exec_name', default=None)
-@click.argument('deployment-name', type=str)
+@click.command(
+    'execute',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--user', default='root')
+@click.option('--shell', default='/bin/bash')
+@click.argument('device-name', type=str)
 @click.argument('command', nargs=-1)
 @name_to_guid
-def execute_command(component_name: str, exec_name: str, deployment_name: str, deployment_guid: str, command: typing.List[str]) -> None:
+def execute_command(
+        device_name: str,
+        device_guid: str,
+        user: str,
+        shell: str,
+        command: typing.List[str]
+) -> None:
     """
-    Execute commands on cloud deployment
+    Execute commands on the Device
     """
     try:
-        comp_id, exec_id, pod_name = select_details(deployment_guid, component_name, exec_name)
-        stdout, stderr = run_on_cloud(deployment_guid, comp_id, exec_id, pod_name, command)
-        if stderr:
-            click.secho(stderr, fg='red')
-        if stdout:
-            click.secho(stdout, fg='yellow')
+        response = run_on_device(
+            device_guid=device_guid,
+            user=user,
+            shell=shell,
+            command=command,
+            background=False,
+        )
+
+        click.secho(response)
     except Exception as e:
-        click.secho(e, fg='red')
-        raise SystemExit(1)
+        click.secho(str(e), fg=Colors.RED)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/inspect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
+from click_help_colors import HelpColorsCommand
 from rapyuta_io.clients.deployment import Deployment
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.deployment.util import name_to_guid
 from riocli.utils import inspect_with_format
 
 
-@click.command('inspect')
+@click.command(
+    'inspect',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--format', '-f', 'format_type', default='yaml',
               type=click.Choice(['json', 'yaml'], case_sensitive=False))
 @click.argument('deployment-name')
 @name_to_guid
-def inspect_deployment(format_type: str, deployment_name: str, deployment_guid: str) -> None:
+def inspect_deployment(
+        format_type: str,
+        deployment_name: str,
+        deployment_guid: str,
+) -> None:
     """
     Inspect the deployment resource
     """
     try:
         client = new_client()
         deployment = client.get_deployment(deployment_guid)
         data = make_deployment_inspectable(deployment)
         inspect_with_format(data, format_type)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
 
 
 def make_deployment_inspectable(deployment: Deployment) -> dict:
     return {
         'created_at': deployment.CreatedAt,
         'updated_at': deployment.UpdatedAt,
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/list.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/delete.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,60 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-import typing
-
 import click
-from rapyuta_io.clients.deployment import Deployment
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
-from riocli.utils import tabulate_data
-
-
-@click.command('list')
-@click.option('--device', prompt_required=False, default='', type=str,
-              help='Filter the Deployment list by Device ID')
-@click.option('--phase', prompt_required=False, multiple=True,
-              type=click.Choice(['In progress', 'Provisioning', 'Succeeded', 'Failed to start',
-                                 'Partially deprovisioned', 'Deployment stopped']),
-              default=['In progress', 'Provisioning', 'Succeeded', 'Failed to start'],
-              help='Filter the Deployment list by Phases')
-def list_deployments(device: str, phase: typing.List[str]) -> None:
+from riocli.constants import Colors, Symbols
+from riocli.deployment.util import name_to_guid
+from riocli.utils.spinner import with_spinner
+
+
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--force', '-f', '--silent', is_flag=True, default=False,
+              help='Skip confirmation')
+@click.argument('deployment-name', type=str)
+@name_to_guid
+@with_spinner(text="Deleting deployment...")
+def delete_deployment(
+        force: bool,
+        deployment_name: str,
+        deployment_guid: str,
+        spinner=None,
+) -> None:
     """
-    List the deployments in the selected project
+    Deletes a deployment
     """
+    with spinner.hidden():
+        if not force:
+            click.confirm(
+                'Deleting {} ({}) deployment'.format(
+                    deployment_name, deployment_guid), abort=True)
+
     try:
         client = new_client()
-        deployments = client.get_all_deployments(device_id=device, phases=phase)
-        deployments = sorted(deployments, key=lambda d: d.name.lower())
-        display_deployment_list(deployments, show_header=True)
+        deployment = client.get_deployment(deployment_guid)
+        deployment.deprovision()
+        spinner.text = click.style(
+            'Deployment deleted successfully.', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.text = click.style(
+            'Failed to delete deployment: {}'.format(e), Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
-
-
-def display_deployment_list(deployments: typing.List[Deployment], show_header: bool = True):
-    headers = []
-    if show_header:
-        headers = ('Deployment ID', 'Name', 'Phase', 'Package')
-
-    data = []
-    for deployment in deployments:
-        package_name_version = "{} ({})".format(deployment.packageName, deployment.packageVersion)
-        data.append([deployment.deploymentId, deployment.name,
-                     deployment.phase, package_name_version])
-
-    tabulate_data(data, headers=headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/logs.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/logs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,45 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 import click
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import Configuration
+from riocli.constants import Colors
 from riocli.deployment.util import name_to_guid, select_details
 
 _LOG_URL_FORMAT = '{}/deployment/logstream?tailLines={}&deploymentId={}&componentId={}&executableId={}&podName={}'
 
 
-@click.command('logs')
-@click.option('--component', 'component_name', default=None)
-@click.option('--exec', 'exec_name', default=None)
+@click.command(
+    'logs',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--component', 'component_name', default=None,
+              help='Name of the component in the deployment')
+@click.option('--exec', 'exec_name', default=None,
+              help='Name of a executable in the component')
 @click.argument('deployment-name', type=str)
 @name_to_guid
-def deployment_logs(component_name: str, exec_name: str, deployment_name: str, deployment_guid: str) -> None:
+def deployment_logs(
+        component_name: str,
+        exec_name: str,
+        deployment_name: str,
+        deployment_guid: str,
+) -> None:
     """
-    Stream the live logs for the Deployment (only Cloud)
+    Stream live logs from cloud deployments (not supported for device deployments)
     """
     try:
         comp_id, exec_id, pod_name = select_details(deployment_guid, component_name, exec_name)
         stream_deployment_logs(deployment_guid, comp_id, exec_id, pod_name)
     except Exception as e:
-        click.secho(e, fg='red')
+        click.secho(e, fg=Colors.RED)
         raise SystemExit(1)
 
 
 def stream_deployment_logs(deployment_id, component_id, exec_id, pod_name=None):
     # FIXME(ankit): The Upstream API ends up timing out when there is no log being written.
     #               IMO the correct behaviour should be to not timeout and keep the stream open.
     config = Configuration()
+
     url = get_log_stream_url(config, deployment_id, component_id, exec_id, pod_name)
     auth = config.get_auth_header()
-    curl = 'curl -H "project: {}" -H "Authorization: {}" "{}"'.format(auth['project'], auth['Authorization'], url)
-    click.secho(curl, fg='blue')
+    curl = 'curl -H "project: {}" -H "Authorization: {}" "{}"'.format(
+        auth['project'], auth['Authorization'], url)
+    click.echo(click.style(curl, fg=Colors.BLUE, italic=True))
+
     os.system(curl)
 
 
 def get_log_stream_url(config, deployment_id, component_id, exec_id, pod_name=None, tail=50000):
     catalog_host = config.data.get('catalog_host', 'https://gacatalog.apps.rapyuta.io')
     return _LOG_URL_FORMAT.format(catalog_host, tail, deployment_id, component_id, exec_id, pod_name)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/model.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,24 +13,25 @@
 # limitations under the License.
 import os
 import typing
 
 import click
 from rapyuta_io import Client
 from rapyuta_io.clients.catalog_client import Package
-from rapyuta_io.clients.deployment import DeploymentNotRunningException
+from rapyuta_io.clients.deployment import DeploymentNotRunningException, DeploymentPhaseConstants
 from rapyuta_io.clients.native_network import NativeNetwork
 from rapyuta_io.clients.package import ProvisionConfiguration, RestartPolicy, \
     ExecutableMount
 from rapyuta_io.clients.rosbag import (
     ROSBagJob, ROSBagOptions, ROSBagCompression,
     UploadOptions, ROSBagOnDemandUploadOptions, ROSBagTimeRange,
     ROSBagUploadTypes, OverrideOptions, TopicOverrideInfo)
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
+from riocli.constants import Colors
 from riocli.deployment.errors import ERRORS
 from riocli.deployment.util import add_mount_volume_provision_config
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 from riocli.package.util import find_package_guid
 from riocli.static_route.util import find_static_route_guid
 
@@ -39,19 +40,22 @@
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
     }
 
     def find_object(self, client: Client) -> typing.Any:
-        guid, obj = self.rc.find_depends(
-            {"kind": "deployment", "nameOrGUID": self.metadata.name})
+        guid, obj = self.rc.find_depends({
+            "kind": "deployment",
+            "nameOrGUID": self.metadata.name,
+        })
+
         return obj if guid else False
 
-    def create_object(self, client: Client) -> typing.Any:
+    def create_object(self, client: Client, **kwargs) -> typing.Any:
         pkg_guid, pkg = self.rc.find_depends(self.metadata.depends,
                                              self.metadata.depends.version)
 
         if pkg_guid:
             pkg = client.get_package(pkg_guid)
         pkg.update()
 
@@ -59,21 +63,21 @@
         plan_id = default_plan['planId']
         internal_component = default_plan['internalComponents'][0]
         component_name = internal_component.componentName
         component = default_plan['components']['components'][0]
         executables = component['executables']
         runtime = internal_component['runtime']
 
+        retry_count = int(kwargs.get('retry_count'))
+        retry_interval = int(kwargs.get('retry_interval'))
+
         if 'runtime' in self.spec and runtime != self.spec.runtime:
-            click.secho(
-                '>> runtime mismatch => ' +
-                'deployment:{}.runtime !== package:{}.runtime '.format(
+            raise Exception('>> runtime mismatch => deployment:{}.runtime !== package:{}.runtime '.format(
                     self.metadata.name, pkg['packageName']
-                ), fg='red')
-            return
+                ))
 
         provision_config = pkg.get_provision_configuration(plan_id)
 
         # add label
         if 'labels' in self.metadata:
             for key, value in self.metadata.labels.items():
                 provision_config.add_label(key, value)
@@ -86,15 +90,17 @@
 
         # Add Dependent Deployment
         if 'depends' in self.spec:
             for item in self.spec.depends:
                 dep_guid, dep = self.rc.find_depends(item)
                 if dep is None and dep_guid:
                     dep = client.get_deployment(dep_guid)
-                provision_config.add_dependent_deployment(dep)
+                provision_config.add_dependent_deployment(dep, ready_phases=[
+                    DeploymentPhaseConstants.PROVISIONING.value,
+                    DeploymentPhaseConstants.SUCCEEDED.value])
 
         # Add Network
         if 'rosNetworks' in self.spec:
             for network_depends in self.spec.rosNetworks:
                 network_guid, network_obj = self.rc.find_depends(network_depends.depends)
 
                 if type(network_obj) == RoutedNetwork:
@@ -213,15 +219,17 @@
 
         if os.environ.get('DEBUG'):
             print(provision_config)
 
         deployment = pkg.provision(self.metadata.name, provision_config)
 
         try:
-            deployment.poll_deployment_till_ready()
+            deployment.poll_deployment_till_ready(retry_count=retry_count, sleep_interval=retry_interval,
+                                                  ready_phases=[DeploymentPhaseConstants.PROVISIONING.value,
+                                                                DeploymentPhaseConstants.SUCCEEDED.value])
         except DeploymentNotRunningException as e:
             raise Exception(process_deployment_errors(e)) from e
         except Exception as e:
             raise e
 
         deployment.get_status()
 
@@ -388,14 +396,14 @@
         elif code.startswith('DEP_E3'):
             description = 'Internal rapyuta.io error in the components deployed on a device'
             action = support_action
         elif code.startswith('DEP_E4'):
             description = 'Internal rapyuta.io error'
             action = support_action
 
-        code = click.style(code, fg='yellow')
-        description = click.style(description, fg='red')
-        action = click.style(action, fg='green')
+        code = click.style(code, fg=Colors.YELLOW)
+        description = click.style(description, fg=Colors.RED)
+        action = click.style(action, fg=Colors.GREEN)
 
         msgs.append(err_fmt.format(code, description, action))
 
     return '\n'.join(msgs)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/run.py` & `rapyuta-io-cli-4.0.0/riocli/constants/symbols.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-import click
 
-
-@click.command('run', hidden=True)
-@click.argument('docker-image', type=str)
-def run_deployment(docker_image: str) -> None:
-    # TODO(ankit): Implement `kubectl run` like command to instantly create a Deployment.
-    # Possibly implement --interactive --tty to SSH into the session
-    pass
+class Symbols:
+    INFO = 'ℹ️'
+    ERROR = '❌'
+    SUCCESS = '✅'
+    WARNING = '⚠️'
+    WAITING = '⏳'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/ssh.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/status.py` & `rapyuta-io-cli-4.0.0/riocli/device/onboard.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 
 from riocli.config import new_client
-from riocli.deployment.util import name_to_guid
+from riocli.device.util import name_to_guid
 
 
-@click.command('status')
-@click.argument('deployment-name', type=str)
+@click.command('onboard')
+@click.argument('device-name', type=str)
 @name_to_guid
-def status(deployment_name: str, deployment_guid: str) -> None:
+def device_onboard(device_name: str, device_guid: str) -> None:
     """
-    Current status of the deployment
+    Generates the on-boarding script for the Device
+
+    To onboard the current device, run the following
+
+        exec $(rio device onboard {device-name})
     """
     try:
         client = new_client()
-        deployment = client.get_deployment(deployment_guid)
-        click.secho(deployment.status)
+        device = client.get_device(device_id=device_guid)
+        script = device.onboard_script()
+        click.secho(script.full_command())
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/util.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,38 +19,43 @@
 from rapyuta_io import Client, DeploymentPhaseConstants
 from rapyuta_io.clients import Device
 from rapyuta_io.clients.package import ExecutableMount
 from rapyuta_io.utils import InvalidParameterException, OperationNotAllowedError
 from rapyuta_io.utils.constants import DEVICE_ID
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.utils.selector import show_selection
 
 
 def name_to_guid(f: typing.Callable) -> typing.Callable:
     @functools.wraps(f)
     def decorated(**kwargs: typing.Any) -> None:
         try:
             client = new_client()
         except Exception as e:
-            click.secho(str(e), fg='red')
-            raise SystemExit(1)
+            click.secho(str(e), fg=Colors.RED)
+            raise SystemExit(1) from e
 
         name = kwargs.pop('deployment_name')
         guid = None
 
         if name.startswith('dep-'):
             guid = name
             name = None
 
-        if name is None:
-            name = get_deployment_name(client, guid)
+        try:
+            if name is None:
+                name = get_deployment_name(client, guid)
 
-        if guid is None:
-            guid = find_deployment_guid(client, name)
+            if guid is None:
+                guid = find_deployment_guid(client, name)
+        except Exception as e:
+            click.secho(str(e), fg=Colors.RED)
+            raise SystemExit(1) from e
 
         kwargs['deployment_name'] = name
         kwargs['deployment_guid'] = guid
         f(**kwargs)
 
     return decorated
 
@@ -118,16 +123,14 @@
         raise InvalidParameterException('device must be of type Device')
 
     component_id = provision_config.plan.get_component_id(component_name)
     if not isinstance(executable_mounts, list) or not all(
             isinstance(mount, ExecutableMount) for mount in executable_mounts):
         raise InvalidParameterException(
             'executable_mounts must be a list of rapyuta_io.clients.package.ExecutableMount')
-    if not device.is_online():
-        raise OperationNotAllowedError('Device should be online')
     if device.get_runtime() != Device.DOCKER_COMPOSE and not device.is_docker_enabled():
         raise OperationNotAllowedError('Device must be a {} device'.format(Device.DOCKER_COMPOSE))
     component_params = provision_config.parameters.get(component_id)
     if component_params.get(DEVICE_ID) != device.deviceId:
         raise OperationNotAllowedError('Device must be added to the component')
     # self._add_disk_mount_info(device.deviceId, component_id, executable_mounts)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/deployment/wait.py` & `rapyuta-io-cli-4.0.0/riocli/device/deployment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
-from rapyuta_io.utils import RetriesExhausted, DeploymentNotRunningException
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
-from riocli.deployment.util import name_to_guid
+from riocli.constants import Colors
+from riocli.deployment.list import display_deployment_list
+from riocli.device.util import name_to_guid
 
 
-@click.command('wait')
-@click.argument('deployment-name', type=str)
+@click.command(
+    'deployments',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.argument('device-name', type=str)
 @name_to_guid
-def wait_for_deployment(deployment_name: str, deployment_guid: str) -> None:
+def list_deployments(device_name: str, device_guid: str) -> None:
     """
-    Wait until the Deployment succeeds/fails
+    Lists all the deployments running on the Device
     """
     try:
         client = new_client()
-        with spinner():
-            deployment = client.get_deployment(deployment_guid)
-            # TODO(ankit): Fix the poll_deployment_till_ready for Runtime Error
-            status = deployment.poll_deployment_till_ready()
-        click.secho('Deployment status: {}'.format(status.status))
-    except RetriesExhausted as e:
-        click.secho(str(e), fg='red')
-        click.secho('Retry Again?', fg='red')
-    except DeploymentNotRunningException as e:
-        if 'DEP_E151' in e.deployment_status.errors:
-            click.secho('Device is either offline or not reachable', fg='red')
-        else:
-            click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        device = client.get_device(device_guid)
+        partials = device.get_deployments()  # Partials
+        deployments = []
+        for partial in partials:
+            # FIXME: get_deployments call doesn't return Deployment partial and instead just returns generic
+            # ObjDict object. PartialMixin methods are not available on it.
+            # partial.refresh()
+            deployment = client.get_deployment(partial.io_deployment_id)
+            deployments.append(deployment)
+        display_deployment_list(deployments, show_header=True)
     except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        click.secho(str(e), fg=Colors.RED)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/create.py` & `rapyuta-io-cli-4.0.0/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/delete.py` & `rapyuta-io-cli-4.0.0/riocli/device/delete.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-import click_spinner
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
+from riocli.constants import Colors, Symbols
 from riocli.device.util import name_to_guid
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('delete')
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--force', '-f', 'force', is_flag=True, help='Skip confirmation')
 @click.argument('device-name', type=str)
 @name_to_guid
-def delete_device(device_name: str, device_guid: str, force: bool):
+@with_spinner(text='Deleting device...')
+def delete_device(device_name: str, device_guid: str, force: bool, spinner=None):
     """
-    Deletes the device from the Platform
+    Deletes a device
     """
-    if not force:
-        click.confirm('Deleting device {} ({})'.format(device_name, device_guid), abort=True)
+    with spinner.hidden():
+        if not force:
+            click.confirm(
+                'Deleting device {} ({})'.format(
+                    device_name, device_guid), abort=True)
 
     try:
         client = new_client(with_project=True)
-        with click_spinner.spinner():
-            client.delete_device(device_id=device_guid)
-        click.secho('Device deleted successfully!', fg='green')
+        client.delete_device(device_id=device_guid)
+        spinner.text = click.style('Device deleted successfully', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        spinner.text = click.style('Failed to delete device: {}'.format(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/deployment.py` & `rapyuta-io-cli-4.0.0/riocli/device/list.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import typing
+
 import click
+from rapyuta_io.clients import Device
 
 from riocli.config import new_client
-from riocli.deployment.list import display_deployment_list
-from riocli.device.util import name_to_guid
+from riocli.utils import tabulate_data
 
 
-@click.command('deployments')
-@click.argument('device-name', type=str)
-@name_to_guid
-def list_deployments(device_name: str, device_guid: str) -> None:
+@click.command('list')
+def list_devices() -> None:
     """
-    Lists all the deployments running on the Device
+    List all the devices in the selected Project
     """
     try:
         client = new_client()
-        device = client.get_device(device_guid)
-        partials = device.get_deployments()  # Partials
-        deployments = []
-        for partial in partials:
-            # FIXME: get_deployments call doesn't return Deployment partial and instead just returns generic
-            # ObjDict object. PartialMixin methods are not available on it.
-            # partial.refresh()
-            deployment = client.get_deployment(partial.io_deployment_id)
-            deployments.append(deployment)
-        display_deployment_list(deployments, show_header=True)
+        devices = client.get_all_devices()
+        devices = sorted(devices, key=lambda d: d.name.lower())
+        _display_device_list(devices, show_header=True)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
+
+
+def _display_device_list(devices: typing.List[Device], show_header: bool = True) -> None:
+    headers = []
+    if show_header:
+        headers = ('Device ID', 'Name', 'Status')
+
+    data = [[d.uuid, d.name, d.status] for d in devices]
+
+    tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/execute.py` & `rapyuta-io-cli-4.0.0/riocli/package/create.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,31 +7,39 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import typing
+import json
 
 import click
+import yaml
+from click_spinner import spinner
 
-from riocli.device.util import name_to_guid
-from riocli.utils.execute import run_on_device
+from riocli.config import new_client
 
 
-@click.command('execute')
-@click.option('--user', default='root')
-@click.option('--shell', default='/bin/bash')
-@click.argument('device-name', type=str)
-@click.argument('command', nargs=-1)
-@name_to_guid
-def execute_command(device_name: str, device_guid: str, user: str, shell: str, command: typing.List[str]):
+@click.command('create', hidden=True)
+@click.option('--manifest', type=click.File(mode='r', lazy=True),
+              help='Path for the manifest file')
+@click.option('--format', 'format_type', default='json',
+              type=click.Choice(['json', 'yaml'], case_sensitive=False))
+def create_package(manifest: click.File, format_type: str) -> None:
     """
-    Execute commands on the Device
+    Create a new package
     """
+    data = manifest.read()
+    if format_type == 'json':
+        package = json.loads(data)
+    else:
+        package = yaml.load(data)
+
     try:
-        response = run_on_device(device_guid=device_guid, user=user, shell=shell, command=command, background=False)
-        click.secho(response)
+        client = new_client()
+        with spinner():
+            client.create_package(package)
+        click.secho('Package created successfully!', fg='green')
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/files.py` & `rapyuta-io-cli-4.0.0/riocli/deployment/update.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,179 +1,199 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-from datetime import datetime, timedelta
+
+import functools
+import re
+from concurrent.futures import ThreadPoolExecutor
+from queue import Queue
+from typing import List
 
 import click
-from click_help_colors import HelpColorsGroup
-from click_spinner import spinner
-from rapyuta_io.clients import LogsUploadRequest, LogUploads, SharedURL
+from click_help_colors import HelpColorsCommand
+from rapyuta_io import Client, DeploymentPhaseConstants
+from rapyuta_io.clients.deployment import Deployment
+from yaspin.api import Yaspin
 
 from riocli.config import new_client
-from riocli.device.util import name_to_guid, name_to_request_id
+from riocli.constants import Symbols, Colors
 from riocli.utils import tabulate_data
+from riocli.utils.spinner import with_spinner
 
 
-@click.group(
-    'uploads',
-    invoke_without_command=False,
-    cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+@click.command(
+    'update',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
-def device_uploads() -> None:
+@click.option('--force', '-f', '--silent', is_flag=True, default=False,
+              help='Skip confirmation')
+@click.option('--update-all', '-a', is_flag=True, default=False,
+              help='Updates all deployments')
+@click.option('--workers', '-w',
+              help="number of parallel workers while running update deployment "
+                   "command. defaults to 10.", type=int, default=10)
+@click.argument('deployment-name-or-regex', type=str, default="")
+@with_spinner(text="Updating...")
+def update_deployment(
+        force: bool,
+        update_all: bool,
+        workers: int,
+        deployment_name_or_regex: str,
+        spinner: Yaspin = None,
+) -> None:
     """
-    Uploaded files from the Device
+    Updates one more deployments
     """
-    pass
-
-
-@device_uploads.command('list')
-@click.argument('device-name', type=str)
-@name_to_guid
-def list_uploads(device_name: str, device_guid: str) -> None:
-    try:
-        client = new_client()
-        device = client.get_device(device_id=device_guid)
-        uploads = device.list_uploaded_files_for_device()
-        _display_upload_list(uploads=uploads, show_header=True)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-@device_uploads.command('create')
-@click.option('--max-upload-rate', type=int, default=1 * 1024 * 1024,
-              help='Network bandwidth limit to be used for upload (Bytes per second)')
-@click.option('--override', is_flag=True, default=False, help='Flag to override destination file')
-@click.option('--purge', is_flag=True, default=False, help='Flag to enable purging the file, after it is uploaded')
-@click.argument('device-name', type=str)
-@click.argument('upload-name', type=str)
-@click.argument('file-path', type=str)
-@name_to_guid
-def create_upload(
-        device_name: str,
-        device_guid: str,
-        upload_name: str,
-        file_path: str,
-        max_upload_rate: int,
-        override: bool,
-        purge: bool,
+    client = new_client()
+    if not (deployment_name_or_regex or update_all):
+        spinner.text = "Nothing to update"
+        spinner.green.ok(Symbols.SUCCESS)
+        return
+
+    try:
+        deployments = fetch_deployments(
+            client, deployment_name_or_regex, update_all)
+    except Exception as e:
+        spinner.text = click.style(
+            'Failed to update deployment(s): {}'.format(e), Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
+
+    if not deployments:
+        spinner.text = "Nothing to update"
+        spinner.ok(Symbols.SUCCESS)
+        return
+
+    headers = ['Name', 'GUID', 'Phase', 'Status']
+    data = [[d.name, d.deploymentId, d.phase, d.status] for d in deployments]
+
+    with spinner.hidden():
+        tabulate_data(data, headers)
+
+    spinner.write('')
+
+    if not force:
+        with spinner.hidden():
+            click.confirm('Do you want to update above deployment(s)?',
+                          default=True, abort=True)
+        spinner.write('')
+
+    try:
+        result = Queue()
+        func = functools.partial(_apply_update, client, result)
+        with ThreadPoolExecutor(max_workers=workers) as executor:
+            executor.map(func, deployments)
+
+        result = sorted(list(result.queue), key=lambda x: x[0])
+
+        data, fg, statuses = [], Colors.GREEN, []
+        for name, status in result:
+            fg = Colors.GREEN if status else Colors.RED
+            icon = Symbols.SUCCESS if status else Symbols.ERROR
+            statuses.append(status)
+            data.append([
+                click.style(name, fg),
+                click.style(icon, fg)
+            ])
+
+        with spinner.hidden():
+            tabulate_data(data, headers=['Name', 'Status'])
+
+        icon = Symbols.SUCCESS if all(statuses) else Symbols.WARNING
+        fg = Colors.GREEN if all(statuses) else Colors.YELLOW
+        text = "successfully" if all(statuses) else "partially"
+
+        spinner.write('')
+        spinner.text = click.style(
+            'Deployment(s) updated {}.'.format(text), fg)
+        spinner.ok(click.style(icon, fg))
+    except Exception as e:
+        spinner.text = click.style(
+            'Failed to update deployment(s): {}'.format(e), Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
+
+
+def fetch_deployments(
+        client: Client,
+        deployment_name_or_regex: str,
+        update_all: bool,
+) -> List[Deployment]:
+    deployments = client.get_all_deployments(
+        phases=[DeploymentPhaseConstants.SUCCEEDED,
+                DeploymentPhaseConstants.PROVISIONING])
+    result = []
+    for deployment in deployments:
+        if (update_all or deployment.name == deployment_name_or_regex or
+                (deployment_name_or_regex not in deployment.name and
+                 re.search(deployment_name_or_regex, deployment.name))):
+            result.append(deployment)
+
+    return result
+
+
+def get_component_context(component_info) -> dict:
+    result = {}
+
+    for component in component_info:
+        comp = {}
+        executables = []
+        exec_metadata = component.get("executableMetaData", []) or []
+
+        for e in exec_metadata:
+            # Component will be considered only if any of its executables is
+            # docker or build
+            if not (e.get("docker") or e.get("buildGUID")):
+                continue
+
+            executable = {}
+
+            if e.get("buildGUID"):
+                executable["buildGUID"] = e["buildGUID"]
+
+            if e.get("docker"):
+                executable["docker"] = e["docker"]
+
+            executable["id"] = e.get("id", "")
+            executable["name"] = e.get("name", "")
+            executables.append(executable)
+
+        if len(executables) > 0:
+            result[component["componentID"]] = comp
+            comp["component"] = {"executables": executables}
+            comp["update_deployment"] = True
+
+    return result
+
+
+def _apply_update(
+        client: Client,
+        result: Queue,
+        deployment: Deployment,
 ) -> None:
     try:
-        client = new_client()
-        with spinner():
-            device = client.get_device(device_id=device_guid)
-            upload_request = LogsUploadRequest(device_path=file_path, file_name=upload_name,
-                                               max_upload_rate=max_upload_rate, override=override,
-                                               purge_after=purge)
-            device.upload_log_file(upload_request)
-        click.secho('File upload requested successfully!', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-@device_uploads.command('status')
-@click.argument('device-name', type=str)
-@click.argument('file-name', type=str)
-@name_to_guid
-@name_to_request_id
-def upload_status(device_name: str, device_guid: str, file_name: str, request_id: str):
-    try:
-        client = new_client()
-        device = client.get_device(device_id=device_guid)
-        status = device.get_log_upload_status(request_uuid=request_id)
-        click.secho(status.status)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-@device_uploads.command('delete')
-@click.argument('device-name', type=str)
-@click.argument('file-name', type=str)
-@name_to_guid
-@name_to_request_id
-def delete_upload(device_name: str, device_guid: str, file_name: str, request_id: str):
-    try:
-        client = new_client()
-        with spinner():
-            device = client.get_device(device_id=device_guid)
-            device.delete_uploaded_log_file(request_uuid=request_id)
-        click.secho('Deleted upload successfully!', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-@device_uploads.command('download')
-@click.argument('device-name', type=str)
-@click.argument('file-name', type=str)
-@name_to_guid
-@name_to_request_id
-def download_log(device_name: str, device_guid: str, file_name: str, request_id: str):
-    try:
-        client = new_client()
-        with spinner():
-            device = client.get_device(device_id=device_guid)
-            url = device.download_log_file(request_uuid=request_id)
-        click.secho(url)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-@device_uploads.command('cancel')
-@click.argument('device-name', type=str)
-@click.argument('file-name', type=str)
-@name_to_guid
-@name_to_request_id
-def cancel_upload(device_name: str, device_guid: str, file_name: str, request_id: str):
-    try:
-        client = new_client()
-        with spinner():
-            device = client.get_device(device_id=device_guid)
-            device.cancel_log_file_upload(request_uuid=request_id)
-        click.secho('Cancelled upload successfully!', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-@device_uploads.command('share')
-@click.option('--expiry', help='Flag to set the expiry date for the Shared URL [default: 7 days]', default=7)
-@click.argument('device-name', type=str)
-@click.argument('file-name', type=str)
-@name_to_guid
-@name_to_request_id
-def shared_url(device_name: str, device_guid: str, file_name: str, request_id: str, expiry: int) -> None:
-    try:
-        client = new_client()
-        with spinner():
-            device = client.get_device(device_id=device_guid)
-            expiry_time = datetime.now() + timedelta(days=7)
-            public_url = device.create_shared_url(SharedURL(request_id, expiry_time=expiry_time))
-        click.secho(public_url.url, fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-def _display_upload_list(uploads: LogUploads, show_header: bool = True) -> None:
-    headers = []
-    if show_header:
-        headers = ('Upload ID', 'Name', 'Status', 'Total Size')
-
-    data = [[u.request_uuid, u.filename, u.status, u.total_size] for u in uploads]
-
-    tabulate_data(data, headers)
+        dep = client.get_deployment(deployment['deploymentId'])
+        component_context = get_component_context(dep.get("componentInfo", {}))
+        payload = {
+            "service_id": dep["packageId"],
+            "plan_id": dep["planId"],
+            "deployment_id": dep["deploymentId"],
+            "context": {
+                "component_context": component_context
+            }
+        }
+        client.update_deployment(payload)
+        result.put((deployment["name"], True))
+    except Exception:
+        result.put((deployment["name"], False))
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/label.py` & `rapyuta-io-cli-4.0.0/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/list.py` & `rapyuta-io-cli-4.0.0/riocli/disk/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,36 +10,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
-from rapyuta_io.clients import Device
+from rapyuta_io.utils.rest_client import HttpMethod
 
-from riocli.config import new_client
+from riocli.constants import Colors
+from riocli.disk.util import _api_call
 from riocli.utils import tabulate_data
 
 
 @click.command('list')
-def list_devices() -> None:
+def list_disks() -> None:
     """
-    List all the devices in the selected Project
+    List the disks in the selected project
     """
     try:
-        client = new_client()
-        devices = client.get_all_devices()
-        devices = sorted(devices, key=lambda d: d.name.lower())
-        _display_device_list(devices, show_header=True)
+        disks = _api_call(HttpMethod.GET)
+        disks = sorted(disks, key=lambda d: d['name'].lower())
+        _display_disk_list(disks, show_header=True)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
 
 
-def _display_device_list(devices: typing.List[Device], show_header: bool = True) -> None:
+def _display_disk_list(disks: typing.Any, show_header: bool = True):
     headers = []
     if show_header:
-        headers = ('Device ID', 'Name', 'Status')
-
-    data = [[d.uuid, d.name, d.status] for d in devices]
+        headers = (
+            'Disk ID', 'Name', 'Status', 'Capacity',
+            'Used', 'Available', 'Used By',
+        )
+
+    data = [[d['guid'],
+             d['name'],
+             d['status'],
+             d['capacity'],
+             d.get('used', 'NA'),
+             d.get('available', 'NA'),
+             d['usedBy']]
+            for d in disks]
 
     tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/metric.py` & `rapyuta-io-cli-4.0.0/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/model.py` & `rapyuta-io-cli-4.0.0/riocli/device/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,27 +17,29 @@
 from rapyuta_io.clients.device import Device as v1Device, DevicePythonVersion
 
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 
 
 class Device(Model):
-
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        guid, obj = self.rc.find_depends(
-            {"kind": "device", "nameOrGUID": self.metadata.name})
+        guid, obj = self.rc.find_depends({
+            "kind": "device",
+            "nameOrGUID": self.metadata.name,
+        })
+
         if not guid:
             return False
 
         return obj
 
-    def create_object(self, client: Client) -> v1Device:
+    def create_object(self, client: Client, **kwargs) -> v1Device:
         device = client.create_device(self.to_v1())
         return device
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
@@ -52,18 +54,20 @@
         if docker_enabled:
             rosbag_mount_path = self.spec.docker.rosbagMountPath
 
         preinstalled_enabled = self.spec.get('preinstalled', False) and self.spec.preinstalled.enabled
         if preinstalled_enabled and self.spec.preinstalled.get('catkinWorkspace'):
             ros_workspace = self.spec.preinstalled.catkinWorkspace
 
-        return v1Device(name=self.metadata.name, description=self.spec.get('description'),
-                        runtime_docker=docker_enabled, runtime_preinstalled=preinstalled_enabled,
-                        ros_distro=self.spec.rosDistro, python_version=python_version,
-                        rosbag_mount_path=rosbag_mount_path, ros_workspace=ros_workspace)
+        return v1Device(
+            name=self.metadata.name, description=self.spec.get('description'),
+            runtime_docker=docker_enabled, runtime_preinstalled=preinstalled_enabled,
+            ros_distro=self.spec.rosDistro, python_version=python_version,
+            rosbag_mount_path=rosbag_mount_path, ros_workspace=ros_workspace
+        )
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
     def validate(data):
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/onboard.py` & `rapyuta-io-cli-4.0.0/riocli/secret/delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,29 +10,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 
 from riocli.config import new_client
-from riocli.device.util import name_to_guid
+from riocli.constants import Colors, Symbols
+from riocli.secret.util import name_to_guid
+from riocli.utils.spinner import with_spinner
+from click_help_colors import HelpColorsCommand
 
-
-@click.command('onboard')
-@click.argument('device-name', type=str)
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--force', '-f', '--silent', 'force', is_flag=True,
+              default=False, help='Skip confirmation')
+@click.argument('secret-name', type=str)
 @name_to_guid
-def device_onboard(device_name: str, device_guid: str) -> None:
+@with_spinner(text='Deleting secret...')
+def delete_secret(force: str, secret_name: str, secret_guid: str, spinner=None) -> None:
     """
-    Generates the on-boarding script for the Device
-
-    To onboard the current device, run the following
-
-        exec $(rio device onboard {device-name})
+    Deletes a secret
     """
+    with spinner.hidden():
+        if not force:
+            click.confirm(
+                'Deleting secret {} ({})'.format(secret_name, secret_guid),
+                abort=True)
+
     try:
         client = new_client()
-        device = client.get_device(device_id=device_guid)
-        script = device.onboard_script()
-        click.secho(script.full_command())
+        client.delete_secret(secret_guid)
+        spinner.text = click.style('Secret deleted successfully.', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        spinner.text = click.style('Failed to delete secret: {}'.format(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/forward.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/scp.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/service.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/ssh.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/ssh.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,63 +11,96 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 import click
 
-from riocli.device.tools.util import run_tunnel_on_device, run_tunnel_on_local, copy_to_device
+from riocli.constants import Colors, Symbols
+from riocli.device.tools.util import (
+    run_tunnel_on_device,
+    run_tunnel_on_local,
+    copy_to_device,
+)
 from riocli.device.util import name_to_guid
 from riocli.utils import random_string
 from riocli.utils.execute import run_on_device
+from riocli.utils.spinner import with_spinner
 from riocli.utils.ssh_tunnel import get_free_tcp_port
 
 
 @click.command('ssh')
 @click.option('--user', '-u', default='root', help='Username for the SSH')
-@click.option('--local-port', '-L', default=None, help='Port number on the local machine for forwarding SSH')
-@click.option('--remote-port', '-R', default=22, help='Port number on the Device on which SSH Server is listening')
+@click.option('--local-port', '-L', default=None,
+              help='Port number on the local machine for forwarding SSH')
+@click.option('--remote-port', '-R', default=22,
+              help='Port number on the Device on which SSH Server is listening')
 @click.option('--x-forward/--no-x-forward', '-X', default=False, is_flag=True,
               help='Flag to enable X Forwarding over SSH')
 @click.argument('device-name', type=str)
 @name_to_guid
-def device_ssh(device_name: str, device_guid: str, user: str, local_port: int, remote_port: int,
-               x_forward: bool) -> None:
+def device_ssh(
+        device_name: str,
+        device_guid: str,
+        user: str,
+        local_port: int,
+        remote_port: int,
+        x_forward: bool,
+) -> None:
     """
     SSH to the Device
     """
     extra_args = ""
     if not x_forward:
         extra_args = extra_args + " -X "
     try:
         path = random_string(8, 5)
         if not local_port:
             local_port = get_free_tcp_port()
-        run_tunnel_on_device(device_guid=device_guid, remote_port=remote_port, path=path)
+        run_tunnel_on_device(device_guid=device_guid, remote_port=remote_port,
+                             path=path)
         run_tunnel_on_local(local_port=local_port, path=path, background=True)
-        os.system('ssh -p {} {} -o StrictHostKeyChecking=no {}@localhost'.format(local_port, extra_args, user))
+        os.system(
+            'ssh -p {} {} -o StrictHostKeyChecking=no {}@localhost'.format(
+                local_port, extra_args, user))
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
 
 
 @click.command('ssh-authorize')
-@click.option('--user', '-u', default='root', help='User for which SSH keys are added')
+@click.option('--user', '-u', default='root',
+              help='User for which SSH keys are added')
 @click.argument('device-name', type=str)
-@click.argument('public-key-file', default="~/.ssh/id_rsa.pub", type=click.Path(exists=True))
+@click.argument('public-key-file', default="~/.ssh/id_rsa.pub",
+                type=click.Path(exists=True))
+@with_spinner(text="Authorizing public SSH key...", timer=True)
 @name_to_guid
-def ssh_authorize_key(device_name: str, device_guid: str, user: str, public_key_file: click.Path) -> None:
+def ssh_authorize_key(device_name: str, device_guid: str, user: str,
+                      public_key_file: click.Path, spinner=None) -> None:
     """
     Authorize Public SSH Key
     """
     try:
         temp_path = "/tmp/{}".format(random_string(8, 5))
-        copy_to_device(device_guid, public_key_file, temp_path)
-        if user != "root":
-            command = ['cat', temp_path, '>>', '/home/' + user + '/.ssh/authorized_keys']
+
+        spinner.write("> Uploading public SSH key to device")
+        copy_to_device(device_guid, str(public_key_file), temp_path,
+                       spinner=spinner)
+
+        if user != 'root':
+            command = ['cat', temp_path, '>>',
+                       '/home/' + user + '/.ssh/authorized_keys']
         else:
             command = ['cat', temp_path, '>>', '/root/.ssh/authorized_keys']
+
         run_on_device(device_guid=device_guid, command=command, user=user)
-        click.secho('Keys added successfully!', fg='green')
+
+        spinner.text = click.style(
+            'Public key {} added successfully'.format(public_key_file),
+            fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.text = click.style("Failed to add keys".format(e),
+                                   fg=Colors.RED)
+        spinner.red.ok(Symbols.ERROR)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/tools/util.py` & `rapyuta-io-cli-4.0.0/riocli/device/tools/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,12 +56,15 @@
     if status.status != "COMPLETED":
         raise Exception('Upload status: {}'.format(status.status, status.error_message))
 
     url = device.download_log_file(request_uuid)
     run_bash('curl -o "{}" "{}"'.format(dest, url))
 
 
-def copy_to_device(device_guid: str, src: str, dest: str) -> None:
+def copy_to_device(device_guid: str, src: str, dest: str, spinner=None) -> None:
     config = Configuration()
     path = random_string(8, 5)
     run_bash('curl -sT {} {}/{}'.format(src, config.piping_server, path), bg=True)
-    run_on_device(device_guid=device_guid, command=['curl', '-o', dest, '{}/{}'.format(config.piping_server, path)])
+    with spinner.hidden():
+        run_on_device(
+            device_guid=device_guid,
+            command=['curl', '-s', '-o', dest, '{}/{}'.format(config.piping_server, path)])
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/topic.py` & `rapyuta-io-cli-4.0.0/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/util.py` & `rapyuta-io-cli-4.0.0/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/device/vpn.py` & `rapyuta-io-cli-4.0.0/riocli/device/vpn.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
 from click_help_colors import HelpColorsCommand
+from yaspin import kbi_safe_yaspin
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.utils import tabulate_data
 
 
 @click.command(
     'vpn',
     cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green'
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN
 )
 @click.option('--devices', type=click.STRING, multiple=True, default=(),
               help='Device names to toggle VPN client')
 @click.argument('enable', type=click.BOOL)
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True,
+              type=click.BOOL, default=False,
               help="Skip confirmation")
-def toggle_vpn(devices: typing.List, enable: bool, silent: bool = False) -> None:
+def toggle_vpn(devices: typing.List, enable: bool,
+               silent: bool = False) -> None:
     """
     Enable or disable VPN client on the device
 
     Examples:
 
         1. Enable VPN on specific devices
 
@@ -67,18 +71,23 @@
         print_final_devices(final)
 
         if not silent:
             click.confirm(
                 "\nDo you want to proceed?",
                 default=True, abort=True)
 
+        click.echo("")  # Echo an empty line
+
         result = []
-        for device in final:
-            r = client.toggle_features(device.uuid, [('vpn', enable)])
-            result.append([device.name, r.get('status')])
+        with kbi_safe_yaspin() as spinner:
+            for device in final:
+                spinner.text = 'Updating VPN state on device {}'.format(
+                    click.style(device.name, bold=True, fg=Colors.CYAN))
+                r = client.toggle_features(device.uuid, [('vpn', enable)])
+                result.append([device.name, r.get('status')])
 
         click.echo("")  # Echo an empty line
 
         tabulate_data(result, headers=["Device", "Status"])
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/disk/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/disk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,29 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.constants import Colors
 from riocli.disk.create import create_disk
 from riocli.disk.delete import delete_disk
 from riocli.disk.list import list_disks
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def disk() -> None:
     """
     Persistent disks
     """
     pass
 
 
 disk.add_command(list_disks)
 disk.add_command(create_disk)
 disk.add_command(delete_disk)
-# disk.add_command(inspect_project)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/disk/delete.py` & `rapyuta-io-cli-4.0.0/riocli/network/inspect.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,49 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
-from rapyuta_io.utils.rest_client import HttpMethod
+from click_help_colors import HelpColorsCommand
 
-from riocli.disk.util import name_to_guid, _api_call
+from riocli.constants import Colors
+from riocli.network.native_network import inspect_native_network
+from riocli.network.routed_network import inspect_routed_network
+from riocli.network.util import name_to_guid
+from riocli.utils import inspect_with_format
 
 
-@click.command('delete')
-@click.option('--force', '-f', 'force', is_flag=True, default=False, help='Skip confirmation')
-@click.argument('disk-name', required=True)
+@click.command(
+    'inspect',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--format', '-f', 'format_type',
+              type=click.Choice(['json', 'yaml'], case_sensitive=False),
+              default='yaml')
+@click.argument('network-name', type=str)
 @name_to_guid
-def delete_disk(disk_name: str, disk_guid: str, force: bool):
+def inspect_network(format_type: str, network_name: str, network_guid: str,
+                    network_type: str) -> None:
     """
-    Delete the disk from the Platform
+    Inspect the network resource
     """
-    if not force:
-        click.confirm('Deleting disk {} ({})'.format(disk_name, disk_guid), abort=True)
-
     try:
-        with spinner():
-            _api_call(HttpMethod.DELETE, guid=disk_guid, load_response=False)
-        click.echo(click.style('Disk deleted successfully!', fg='green'))
+        if network_type == 'routed':
+            data = inspect_routed_network(network_guid)
+        else:
+            data = inspect_native_network(network_guid)
+
+        inspect_with_format(data, format_type)
     except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        click.secho(str(e), fg=Colors.RED)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/disk/list.py` & `rapyuta-io-cli-4.0.0/riocli/utils/mermaid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-import typing
 
-import click
-from rapyuta_io.utils.rest_client import HttpMethod
+import base64
+import json
 
-from riocli.disk.util import _api_call
-from riocli.utils import tabulate_data
 
+def mermaid_safe(s: str):
+    return s.replace(" ", "_")
 
-@click.command('list')
-def list_disks() -> None:
-    """
-    List the disks in the selected project
-    """
-    try:
-        disks = _api_call(HttpMethod.GET)
-        disks = sorted(disks, key=lambda d: d['name'].lower())
-        _display_disk_list(disks, show_header=True)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
 
+def js_string_to_byte(data: str):
+    return bytes(data, 'iso-8859-1')
 
-def _display_disk_list(disks: typing.Any, show_header: bool = True):
-    headers = []
-    if show_header:
-        headers = ('Disk ID', 'Name', 'Status', 'Capacity', 'Used By')
 
-    data = [[d['guid'], d['name'], d['status'], d['capacity'], d['usedBy']] for d in disks]
+def js_bytes_to_string(data: bytes):
+    return data.decode('iso-8859-1')
 
-    tabulate_data(data, headers)
+
+def js_btoa(data: bytes):
+    return base64.b64encode(data)
+
+
+def mermaid_link(diagram):
+    obj = {
+        "code": diagram,
+        "mermaid": {
+            "theme": "default"
+        },
+        "updateEditor": False,
+        "autoSync": True,
+        "updateDiagram": False
+    }
+    json_str = json.dumps(obj)
+    json_bytes = js_string_to_byte(json_str)
+    encoded_uri = js_btoa(json_bytes)
+    return 'https://mermaid.live/view#base64:{}'.format(
+        js_bytes_to_string(encoded_uri))
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/disk/model.py` & `rapyuta-io-cli-4.0.0/riocli/disk/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,53 +11,69 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 from time import sleep
 
 import click
-import click_spinner
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.utils.rest_client import HttpMethod
 
+from riocli.constants import Colors, Symbols
 from riocli.disk.util import _api_call
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 
 
 class Disk(Model):
     def find_object(self, client: Client) -> typing.Any:
-        _, disk = self.rc.find_depends({'kind': 'disk', 'nameOrGUID': self.metadata.name})
+        _, disk = self.rc.find_depends({
+            'kind': 'disk',
+            'nameOrGUID': self.metadata.name
+        })
+
         if not disk:
             return False
 
         return disk
 
-    def create_object(self, client: Client) -> typing.Any:
+    def create_object(self, client: Client, **kwargs) -> typing.Any:
         labels = self.metadata.get('labels', None)
         payload = {
             "labels": labels,
             "name": self.metadata.name,
             "diskType": "ssd",
             "runtime": self.spec.runtime,
             "capacity": self.spec.capacity,
         }
-        with click_spinner.spinner():
-            result = _api_call(HttpMethod.POST, payload=payload)
-            result = munchify(result)
-            disk_dep_guid, disk = self.rc.find_depends({'kind': self.kind.lower(), 'nameOrGUID': self.metadata.name})
-            volume_instance = client.get_volume_instance(disk_dep_guid)
-            try:
-                volume_instance.poll_deployment_till_ready(sleep_interval=5)
-                return result
-            except Exception as e:
-                click.secho(">> Warning: Error Polling for disk ({}:{})".format(self.kind.lower(), self.metadata.name),
-                            fg="yellow")
-            return result
+
+        result = _api_call(HttpMethod.POST, payload=payload)
+        result = munchify(result)
+        disk_dep_guid, disk = self.rc.find_depends({
+            'kind': self.kind.lower(),
+            'nameOrGUID': self.metadata.name
+        })
+
+        volume_instance = client.get_volume_instance(disk_dep_guid)
+
+        retry_count = int(kwargs.get('retry_count'))
+        retry_interval = int(kwargs.get('retry_interval'))
+        try:
+            volume_instance.poll_deployment_till_ready(
+                retry_count=retry_count,
+                sleep_interval=retry_interval
+            )
+        except Exception as e:
+            click.secho(">> {}: Error polling for disk ({}:{})".format(
+                Symbols.WARNING,
+                self.kind.lower(),
+                self.metadata.name), fg=Colors.YELLOW)
+
+        return result
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         self._poll_till_available(client, obj)
         volume_instance = client.get_volume_instance(obj.internalDeploymentGUID)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/disk/util.py` & `rapyuta-io-cli-4.0.0/riocli/disk/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,65 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import functools
 import json
+import time
 import typing
 
 import click
 from rapyuta_io import Client
+from rapyuta_io.clients.persistent_volumes import DiskCapacity, DiskType
 from rapyuta_io.utils.rest_client import RestClient, HttpMethod
 
 from riocli.config import Configuration, new_client
+from riocli.constants import Colors, Symbols
+
+
+class DiskNotFound(Exception):
+    def __init__(self):
+        super().__init__('Disk not found')
+
+
+def _api_call(
+        method: str,
+        guid: typing.Union[str, None] = None,
+        payload: typing.Union[typing.Dict, None] = None,
+        load_response: bool = True,
+) -> typing.Any:
+    config = Configuration()
+    catalog_host = config.data.get(
+        'catalog_host', 'https://gacatalog.apps.rapyuta.io')
+
+    url = '{}/disk'.format(catalog_host)
+    if guid:
+        url = '{}/{}'.format(url, guid)
+
+    headers = config.get_auth_header()
+    response = RestClient(url).method(method).headers(
+        headers).execute(payload=payload)
+
+    data = None
+    if load_response:
+        data = json.loads(response.text)
+
+    if not response.ok:
+        err_msg = data.get('error')
+        raise Exception(err_msg)
+    return data
 
 
 def name_to_guid(f: typing.Callable) -> typing.Callable:
     @functools.wraps(f)
     def decorated(**kwargs: typing.Any):
         client = new_client()
         name = kwargs.pop('disk_name')
@@ -36,16 +72,16 @@
         if name is None:
             name = get_disk_name(client, guid)
 
         if guid is None:
             try:
                 guid = find_disk_guid(client, name)
             except Exception as e:
-                click.secho(str(e), fg='red')
-                raise SystemExit(1)
+                click.secho('{} {}'.format(Symbols.ERROR, e), fg=Colors.RED)
+                raise SystemExit(1) from e
 
         kwargs['disk_name'] = name
         kwargs['disk_guid'] = guid
         f(**kwargs)
 
     return decorated
 
@@ -62,34 +98,29 @@
             if disk['name'] == name:
                 return disk['guid']
         raise DiskNotFound()
     except Exception:
         raise DiskNotFound()
 
 
-def _api_call(method: str, guid: typing.Union[str, None] = None,
-              payload: typing.Union[typing.Dict, None] = None, load_response: bool = True,
-              ) -> typing.Any:
-    config = Configuration()
-    catalog_host = config.data.get(
-        'catalog_host', 'https://gacatalog.apps.rapyuta.io')
-    url = '{}/disk'.format(catalog_host)
-    if guid:
-        url = '{}/{}'.format(url, guid)
-    headers = config.get_auth_header()
-    response = RestClient(url).method(method).headers(
-        headers).execute(payload=payload)
-    data = None
-    err_msg = 'error in the api call'
-    if load_response:
-        data = json.loads(response.text)
-
-    if not response.ok:
-        err_msg = data.get('error')
-        raise Exception(err_msg)
-    return data
-
-
-class DiskNotFound(Exception):
-    def __init__(self, message='disk not found!'):
-        self.message = message
-        super().__init__(self.message)
+def create_cloud_disk(disk_name: str, capacity: int) -> typing.Dict:
+    """
+    Creates a new cloud disk and waits until it is provisioned
+    """
+    payload = {
+        "name": disk_name,
+        "diskType": DiskType.SSD,
+        "runtime": "cloud",
+        "capacity": DiskCapacity(capacity).value,
+    }
+
+    disk = _api_call(HttpMethod.POST, payload=payload)
+
+    while not is_disk_ready(disk.get('guid')):
+        time.sleep(5)
+
+    return disk
+
+
+def is_disk_ready(disk_guid: str) -> bool:
+    disk = _api_call(HttpMethod.GET, disk_guid, load_response=True)
+    return disk.get('status') != 'Pending'
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/exceptions/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/jsonschema/validate.py` & `rapyuta-io-cli-4.0.0/riocli/jsonschema/validate.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/managedservice/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/managedservice/delete.py` & `rapyuta-io-cli-4.0.0/riocli/managedservice/list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,45 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
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
+import typing
 
 import click
+from munch import unmunchify
 
 from riocli.config import new_v2_client
+from riocli.utils import tabulate_data
 
 
-@click.command('delete')
-@click.argument('instance-name', required=True)
-def delete_instance(instance_name: str):
+@click.command('list')
+def list_instances():
     """
-    Delete a managedservice instance
+    List all the managedservice instances
     """
     try:
         client = new_v2_client()
-        r = client.delete_instance(instance_name)
-        if r.get('success', None):
-            click.secho("✅ Deleted instance '{}'".format(instance_name), fg='green')
+        instances = client.list_instances()
+        _display_instances(instances)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
+
+
+def _display_instances(instances: typing.Any):
+    headers = ["Provider", "Name", "Created At", "Labels"]
+
+    data = []
+    for i in instances:
+        m = i.metadata
+        data.append([i.spec.provider, m.name, m.createdAt, unmunchify(m.labels)])
+
+    tabulate_data(data, headers)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/managedservice/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/managedservice/list.py` & `rapyuta-io-cli-4.0.0/riocli/managedservice/list_providers.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
-from munch import unmunchify
 
 from riocli.config import new_v2_client
 from riocli.utils import tabulate_data
 
 
-@click.command('list')
-def list_instances():
+@click.command('providers')
+def list_providers():
     """
-    List all the managedservice instances
+    List available managedservice providers
     """
     try:
         client = new_v2_client()
-        instances = client.list_instances()
-        _display_instances(instances)
+        providers = client.list_providers()
+        _display_providers(providers)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
 
 
-def _display_instances(instances: typing.Any):
-    headers = ["Provider", "Name", "Created At", "Labels"]
+def _display_providers(providers: typing.Any):
+    headers = ['Provider Name']
 
     data = []
-    for i in instances:
-        m = i.metadata
-        data.append([i.spec.provider, m.name, m.createdAt, unmunchify(m.labels)])
+    for provider in providers:
+        if provider.name == 'dummy':
+            continue
+        data.append([provider.name])
 
     tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-4.0.0/riocli/secret/docker_secret.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2021 Rapyuta Robotics
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
-import typing
-
 import click
+from click_spinner import spinner
+from rapyuta_io.clients.secret import DOCKER_HUB_REGISTRY, SecretConfigDocker, Secret
+
+from riocli.config import new_client
+
+
+def create_docker_secret(
+        secret_name: str,
+        username: str = None,
+        password: str = None,
+        email: str = None,
+        registry=DOCKER_HUB_REGISTRY,
+) -> None:
+    if not username:
+        username = click.prompt('docker username')
+
+    if not password:
+        password = click.prompt('docker password', hide_input=True)
 
-from riocli.config import new_v2_client
-from riocli.utils import tabulate_data
+    if not email:
+        email = click.prompt('docker email')
 
+    secret_config = SecretConfigDocker(username=username, password=password, email=email,
+                                       registry=registry)
+    client = new_client()
 
-@click.command('providers')
-def list_providers():
-    """
-    List available managedservice providers
-    """
-    try:
-        client = new_v2_client()
-        providers = client.list_providers()
-        _display_providers(providers)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-def _display_providers(providers: typing.Any):
-    headers = ['Provider Name']
-
-    data = []
-    for provider in providers:
-        if provider.name == 'dummy':
-            continue
-        data.append([provider.name])
+    with spinner():
+        client.create_secret(Secret(secret_name, secret_config=secret_config))
 
-    tabulate_data(data, headers)
+    click.secho('Secret created successfully!', fg='green')
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/managedservice/model.py` & `rapyuta-io-cli-4.0.0/riocli/managedservice/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         try:
             instance = client.get_instance(name)
             return munchify(instance)
         except Exception:
             return False
 
-    def create_object(self, client: Client) -> typing.Any:
+    def create_object(self, client: Client, **kwargs) -> typing.Any:
         client = new_v2_client()
 
         ms = unmunchify(self)
         ms.pop('rc', None)
         result = client.create_instance(ms)
         return munchify(result)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/network/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,26 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.constants import Colors
 from riocli.network.create import create_network
 from riocli.network.delete import delete_network
 from riocli.network.inspect import inspect_network
 from riocli.network.list import list_networks
 from riocli.network.logs import network_logs
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def network() -> None:
     """
     ROS Communication between the Deployments
     """
     pass
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/create.py` & `rapyuta-io-cli-4.0.0/riocli/network/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,22 +21,27 @@
 
 
 @click.command('create', hidden=True)
 @click.argument('name', type=str)
 @click.option('--network', help='Type of Network',
               type=click.Choice(['routed', 'native']), default='routed')
 @click.option('--ros', help='Version of ROS',
-              type=click.Choice(['kinetic', 'melodic', 'noetic']), default='melodic')
-@click.option('--device', 'device_name', help='Device ID of the Device where Network will run (device only)')
+              type=click.Choice(['kinetic', 'melodic', 'noetic']),
+              default='melodic')
+@click.option('--device', 'device_name',
+              help='Device ID of the Device where Network will run (device only)')
 @click.option('--cpu', help='cpu limit for Network (cloud only) ', type=float)
-@click.option('--memory', help='memory limit for Network (cloud only) ', type=int)
+@click.option('--memory', help='memory limit for Network (cloud only) ',
+              type=int)
 @click.option('--network-interface', '-nic', type=str,
               help='Network Interface on which Network will listen (device only)')
-@click.option('--restart-policy', help='Restart policy for the Network (device only)',
-              type=click.Choice(['always', 'no', 'on-failure']), default='always')
+@click.option('--restart-policy',
+              help='Restart policy for the Network (device only)',
+              type=click.Choice(['always', 'no', 'on-failure']),
+              default='always')
 @device_name_to_guid
 def create_network(name: str, network: str, **kwargs: typing.Any) -> None:
     """
     Create a new network
     """
     try:
         if network == 'routed':
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/delete.py` & `rapyuta-io-cli-4.0.0/riocli/network/delete.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,73 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
+from yaspin.api import Yaspin
 
 from riocli.config import new_client
+from riocli.constants import Colors, Symbols
 from riocli.network.util import name_to_guid
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('delete')
-@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation', type=bool)
-@click.option('--network', 'network_type', help='Type of Network', default=None,
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--force', '-f', is_flag=True, default=False,
+              help='Skip confirmation', type=bool)
+@click.option('--network', 'network_type', help='Type of Network',
+              default=None,
               type=click.Choice(['routed', 'native']))
 @click.argument('network-name', type=str)
 @name_to_guid
-def delete_network(force: bool, network_name: str, network_guid: str, network_type: str) -> None:
+@with_spinner(text='Deleting network...')
+def delete_network(
+        force: bool,
+        network_name: str,
+        network_guid: str,
+        network_type: str,
+        spinner: Yaspin = None
+) -> None:
     """
-    Delete the network from the Platform
+    Deletes a network
     """
-
     if not force:
-        click.confirm('Deleting {} network {} ({})'.
-                      format(network_type, network_name, network_guid), abort=True)
+        with spinner.hidden():
+            click.confirm(
+                'Deleting {} network {} ({})'.
+                format(network_type, network_name, network_guid),
+                abort=True)
 
     try:
         client = new_client()
-        with spinner():
-            if network_type == 'routed':
-                # TODO: Implement and use the delete_routed_network of client directly.
-                rn = client.get_routed_network(network_guid)
-                rn.delete()
-            elif network_type == 'native':
-                client.delete_native_network(network_guid)
-        click.secho('{} Network deleted successfully!'.format(network_type.capitalize()), fg='green')
+
+        if network_type == 'routed':
+            client.delete_routed_network(network_guid)
+        elif network_type == 'native':
+            client.delete_native_network(network_guid)
+        else:
+            raise Exception('invalid network type')
+
+        spinner.text = click.style(
+            '{} deleted successfully!'.format(network_type.capitalize()),
+            fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        spinner.text = click.style('Failed to delete network: {}'.format(e),
+                                   fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/list.py` & `rapyuta-io-cli-4.0.0/riocli/network/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,39 +10,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
+from click_help_colors import HelpColorsCommand
 from rapyuta_io import DeploymentPhaseConstants
 from rapyuta_io.clients.native_network import NativeNetwork
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.utils import tabulate_data
 
 
-@click.command('list')
+@click.command(
+    'list',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--network', help='Type of Network',
               type=click.Choice(['routed', 'native', 'both']), default='both')
 def list_networks(network: str) -> None:
     """
     List the networks in the selected project
     """
     try:
         client = new_client()
+
         networks = []
         if network in ['routed', 'both']:
             networks += client.get_all_routed_networks()
 
         if network in ['native', 'both']:
             networks += client.list_native_networks()
 
         networks = sorted(networks, key=lambda n: n.name.lower())
+
         _display_network_list(networks, show_header=True)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
 
 
 def _display_network_list(
@@ -62,10 +71,11 @@
             phase = network.phase
         elif isinstance(network, NativeNetwork):
             network_type = 'native'
             phase = network.internal_deployment_status.phase
 
         if phase and phase == DeploymentPhaseConstants.DEPLOYMENT_STOPPED.value:
             continue
-        data.append([network.guid, network.name, network.runtime, network_type, phase])
+        data.append(
+            [network.guid, network.name, network.runtime, network_type, phase])
 
     tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/logs.py` & `rapyuta-io-cli-4.0.0/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/model.py` & `rapyuta-io-cli-4.0.0/riocli/network/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,84 +23,94 @@
 
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 from riocli.network.util import find_network_name, NetworkNotFound
 
 
 class Network(Model):
-
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
         try:
-            network, _ = find_network_name(client, self.metadata.name, self.spec.type, is_resolve_conflict=False)
+            network, _ = find_network_name(client, self.metadata.name,
+                                           self.spec.type,
+                                           is_resolve_conflict=False)
             return network
         except NetworkNotFound:
             return False
 
-    def create_object(self, client: Client) -> Union[NativeNetwork, RoutedNetwork]:
+    def create_object(self, client: Client, **kwargs) -> Union[NativeNetwork, RoutedNetwork]:
+        retry_count = int(kwargs.get('retry_count'))
+        retry_interval = int(kwargs.get('retry_interval'))
         if self.spec.type == 'routed':
             network = self._create_routed_network(client)
-            network.poll_routed_network_till_ready()
+            network.poll_routed_network_till_ready(retry_count=retry_count, sleep_interval=retry_interval)
             return network
 
         network = client.create_native_network(self.to_v1(client))
-        network.poll_native_network_till_ready()
+        network.poll_native_network_till_ready(retry_count=retry_count, sleep_interval=retry_interval)
         return network
 
-    def update_object(self, client: Client, obj: Union[RoutedNetwork, NativeNetwork]) -> Any:
-        # try:
-        #     obj.delete()
-        #     self.create_object(client)
-        # except Exception as e:
-        #     click.secho(str(e), fg='red')
-        #     raise SystemExit(1)
+    def update_object(self, client: Client,
+                      obj: Union[RoutedNetwork, NativeNetwork]) -> Any:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         obj.delete()
 
     @classmethod
     def pre_process(cls, client: Client, d: Dict) -> None:
         pass
 
-
     def to_v1(self, client: Client) -> NativeNetwork:
         if self.spec.runtime == 'cloud':
             limits = self._get_limits()
             parameters = NativeNetworkParameters(limits=limits)
         else:
             device = client.get_device(self.spec.deviceGUID)
-            parameters = NativeNetworkParameters(device=device,
-                                                 network_interface=self.spec.networkInterface)
-
-        return NativeNetwork(self.metadata.name, self.spec.runtime.lower(), self.spec.rosDistro, parameters=parameters)
+            parameters = NativeNetworkParameters(
+                device=device,
+                network_interface=self.spec.networkInterface)
+
+        return NativeNetwork(
+            self.metadata.name,
+            self.spec.runtime.lower(),
+            self.spec.rosDistro,
+            parameters=parameters
+        )
 
     def _get_limits(self):
-        return Limits(self.spec.resourceLimits['cpu'], self.spec.resourceLimits['memory'])
+        return Limits(self.spec.resourceLimits['cpu'],
+                      self.spec.resourceLimits['memory'])
 
     def _create_routed_network(self, client: Client) -> RoutedNetwork:
         if self.spec.runtime == 'cloud':
             network = self._create_cloud_routed_network(client)
         else:
             network = self._create_device_routed_network(client)
 
         return network
 
     def _create_cloud_routed_network(self, client: Client) -> RoutedNetwork:
         limits = self._get_limits()
         parameters = RoutedNetworkParameters(limits)
-        return client.create_cloud_routed_network(self.metadata.name, self.spec.rosDistro, True, parameters=parameters)
+        return client.create_cloud_routed_network(self.metadata.name,
+                                                  self.spec.rosDistro, True,
+                                                  parameters=parameters)
 
     def _create_device_routed_network(self, client: Client) -> RoutedNetwork:
         device = client.get_device(self.spec.deviceGUID)
-        return client.create_device_routed_network(name=self.metadata.name, ros_distro=self.spec.rosDistro, shared=True,
-                                                   device=device,
-                                                   network_interface=self.spec.networkInterface)
+        return client.create_device_routed_network(
+            name=self.metadata.name,
+            ros_distro=self.spec.rosDistro,
+            shared=True,
+            device=device,
+            network_interface=self.spec.networkInterface,
+        )
 
     @staticmethod
     def validate(data):
         """
         Validates if network data is matching with its corresponding schema
         """
         schema = load_schema('network')
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/native_network.py` & `rapyuta-io-cli-4.0.0/riocli/network/native_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,45 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
-from click_spinner import spinner
+from rapyuta_io.clients.common_models import Limits
 from rapyuta_io.clients.native_network import NativeNetwork, Parameters
 from rapyuta_io.clients.package import Runtime, ROSDistro
-from rapyuta_io.clients.common_models import Limits
+
 from riocli.config import new_client
 
 
-def create_native_network(name: str, ros: str, device_guid: str = None, network_interface: str = None,
-                          cpu: float = 0, memory: int = 0, restart_policy: str = None, **kwargs: typing.Any) -> None:
+def create_native_network(name: str, ros: str, device_guid: str = None,
+                          network_interface: str = None,
+                          cpu: float = 0, memory: int = 0,
+                          restart_policy: str = None,
+                          **kwargs: typing.Any) -> None:
     client = new_client()
 
     ros_distro = ROSDistro(ros)
     runtime = Runtime.CLOUD
 
     limit = None
     if cpu or memory:
         if device_guid:
-            raise Exception('Native network for device does not support cpu or memory')
+            raise Exception(
+                'Native network for device does not support cpu or memory')
         limit = Limits(cpu, memory)
 
     device = None
     if device_guid:
         runtime = Runtime.DEVICE
         device = client.get_device(device_id=device_guid)
 
-    parameters = Parameters(limits=limit, device=device, network_interface=network_interface,
+    parameters = Parameters(limits=limit, device=device,
+                            network_interface=network_interface,
                             restart_policy=restart_policy)
-    with spinner():
-        client.create_native_network(NativeNetwork(name, runtime=runtime,
-                                                   ros_distro=ros_distro,
-                                                   parameters=parameters))
+
+    client.create_native_network(NativeNetwork(name, runtime=runtime,
+                                               ros_distro=ros_distro,
+                                               parameters=parameters))
 
     click.secho('Native Network created successfully!', fg='green')
 
 
 def inspect_native_network(network_guid: str) -> dict:
     client = new_client()
     network = client.get_native_network(network_guid)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/routed_network.py` & `rapyuta-io-cli-4.0.0/riocli/network/routed_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,47 +10,52 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
-from click_spinner import spinner
 from rapyuta_io import ROSDistro
+from rapyuta_io.clients.common_models import Limits
 from rapyuta_io.clients.package import RestartPolicy
 from rapyuta_io.clients.routed_network import Parameters
-from rapyuta_io.clients.common_models import Limits
+
 from riocli.config import new_client
 
 
-def create_routed_network(name: str, ros: str, device_guid: str = None, network_interface: str = None,
-                          cpu: float = 0, memory: int = 0, restart_policy: str = None, **kwargs: typing.Any) -> None:
+def create_routed_network(name: str, ros: str, device_guid: str = None,
+                          network_interface: str = None,
+                          cpu: float = 0, memory: int = 0,
+                          restart_policy: str = None,
+                          **kwargs: typing.Any) -> None:
     client = new_client()
     ros_distro = ROSDistro(ros)
 
     limit = None
     if cpu or memory:
         if device_guid:
-            raise Exception('Routed network for device does not support cpu or memory')
+            raise Exception(
+                'Routed network for device does not support cpu or memory')
         limit = Limits(cpu, memory)
 
     if restart_policy:
         restart_policy = RestartPolicy(restart_policy)
 
-    with spinner():
-        if device_guid:
-            device = client.get_device(device_id=device_guid)
-            client.create_device_routed_network(name=name, ros_distro=ros_distro, shared=False,
-                                                device=device,
-                                                network_interface=network_interface,
-                                                restart_policy=restart_policy)
-        else:
-            parameters = None if not limit else Parameters(limit)
-            client.create_cloud_routed_network(name, ros_distro=ros_distro, shared=False,
-                                               parameters=parameters)
+    if device_guid:
+        device = client.get_device(device_id=device_guid)
+        client.create_device_routed_network(name=name, ros_distro=ros_distro,
+                                            shared=False,
+                                            device=device,
+                                            network_interface=network_interface,
+                                            restart_policy=restart_policy)
+    else:
+        parameters = None if not limit else Parameters(limit)
+        client.create_cloud_routed_network(name, ros_distro=ros_distro,
+                                           shared=False,
+                                           parameters=parameters)
 
     click.secho('Routed Network created successfully!', fg='green')
 
 
 def inspect_routed_network(network_guid: str) -> dict:
     client = new_client()
     network = client.get_routed_network(network_guid)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/network/util.py` & `rapyuta-io-cli-4.0.0/riocli/network/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,14 +16,15 @@
 
 import click
 from rapyuta_io import DeploymentPhaseConstants, Client
 from rapyuta_io.clients.native_network import NativeNetwork
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.utils.selector import show_selection
 
 
 def name_to_guid(f: Callable) -> Callable:
     @functools.wraps(f)
     def decorated(**kwargs: Any):
         client = new_client()
@@ -32,21 +33,27 @@
         network_type = kwargs.pop('network', None)
         guid = None
 
         if name.startswith('net-'):
             guid = name
             name = None
 
-        if guid:
-            network, network_type = find_network_guid(client, guid, network_type)
-            name = network.name
-
-        if name:
-            network, network_type = find_network_name(client, name, network_type)
-            guid = network.guid
+        try:
+            if guid:
+                network, network_type = find_network_guid(
+                    client, guid, network_type)
+                name = network.name
+
+            if name:
+                network, network_type = find_network_name(
+                    client, name, network_type)
+                guid = network.guid
+        except Exception as e:
+            click.secho(str(e), fg=Colors.RED)
+            raise SystemExit(1) from e
 
         kwargs['network_type'] = network_type
         kwargs['network_name'] = name
         kwargs['network_guid'] = guid
         f(**kwargs)
 
     return decorated
@@ -89,25 +96,27 @@
 
     if network_type in [None, 'native']:
         native = find_native_network_name(client, name)
 
     return resolve_conflict(routed, native, network_type, is_resolve_conflict)
 
 
-def find_native_network_name(client: Client, name: str) -> Optional[NativeNetwork]:
+def find_native_network_name(client: Client, name: str) -> Optional[
+    NativeNetwork]:
     native_networks = client.list_native_networks()
     for network in native_networks:
         phase = network.internal_deployment_status.phase
         if phase == DeploymentPhaseConstants.DEPLOYMENT_STOPPED.value:
             continue
         if network.name == name:
             return network
 
 
-def find_routed_network_name(client: Client, name: str) -> Optional[RoutedNetwork]:
+def find_routed_network_name(client: Client, name: str) -> Optional[
+    RoutedNetwork]:
     routed_networks = client.get_all_routed_networks()
     for network in routed_networks:
         if network.phase == DeploymentPhaseConstants.DEPLOYMENT_STOPPED.value:
             continue
         if network.name == name:
             return network
 
@@ -136,23 +145,24 @@
         choice = network_type
     else:
         # Ask user to help us resolve conflict by selecting one network
         options = {
             'routed': '{} ({})'.format(routed.name, routed.guid),
             'native': '{} ({})'.format(native.name, native.guid),
         }
-        choice = show_selection(options, header='Both Routed and Native networks were found with '
-                                                'the same name')
+        choice = show_selection(options,
+                                header='Both Routed and Native networks were found with '
+                                       'the same name')
 
     if choice == 'routed':
         return routed, choice
     elif choice == 'native':
         return native, choice
     else:
-        click.secho('Invalid choice. Try again', fg='red')
+        click.secho('Invalid choice. Try again', fg=Colors.RED)
         raise SystemExit(1)
 
 
 def get_network(
         client: Client,
         network_guid: str,
         network_type: str,
@@ -176,10 +186,11 @@
 class NetworkNotFound(Exception):
     def __init__(self, message='network not found!'):
         self.message = message
         super().__init__(self.message)
 
 
 class NetworkConflict(Exception):
-    def __init__(self, message='both routed and native networks exist with the same name!'):
+    def __init__(self,
+                 message='both routed and native networks exist with the same name!'):
         self.message = message
         super().__init__(self.message)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/organization/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/organization/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.constants import Colors
 from riocli.organization.list import list_organizations
 from riocli.organization.select import select_organization
+from riocli.organization.users import list_users
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def organization() -> None:
     """
     Organizations in rapyuta.io
     """
     pass
 
 
+organization.add_command(list_users)
 organization.add_command(list_organizations)
 organization.add_command(select_organization)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/organization/list.py` & `rapyuta-io-cli-4.0.0/riocli/vpn/disconnect.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,49 +9,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
+from click_help_colors import HelpColorsCommand
 
-from riocli.config import new_client
-from riocli.utils import tabulate_data
-
-
-@click.command('list')
+from riocli.constants import Colors, Symbols
+from riocli.vpn.util import (
+    install_vpn_tools,
+    is_tailscale_up,
+    stop_tailscale
+)
+
+
+@click.command(
+    'disconnect',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.pass_context
-def list_organizations(ctx: click.Context) -> None:
+def disconnect(ctx: click.Context):
     """
-    List all the organizations that you are a part of
-
-    Example:
-
-        rio organization list
+    Disconnect from the project's VPN network
     """
     try:
-        client = new_client(with_project=False)
-        organizations = client.get_user_organizations()
-        current = ctx.obj.data['organization_id']
-        print_organizations(organizations, current)
+        install_vpn_tools()
+
+        if is_tailscale_up() and not stop_tailscale():
+            click.secho(
+                '{} Failed to disconnect from VPN. '
+                'Although, trying again may work.'.format(Symbols.ERROR),
+                fg=Colors.RED)
+            raise SystemExit(1)
+
+        click.secho(
+            '{} You have been disconnected from the project\'s VPN'.format(
+                Symbols.SUCCESS),
+            fg=Colors.GREEN)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1) from e
-
-
-def print_organizations(organizations, current):
-    organizations = sorted(organizations, key=lambda o: o.name)
-
-    headers = ["Name", "GUID", "Creator", "Short GUID"]
-
-    data = []
-    for org in organizations:
-        fg = None
-        if org.guid == current:
-            fg = 'green'
-        data.append([
-            click.style(v, fg=fg)
-            for v in (org.name, org.guid,
-                      org.creator, org.short_guid)
-        ])
-
-    tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/organization/select.py` & `rapyuta-io-cli-4.0.0/riocli/organization/select.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,40 +7,63 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import sys
+
 import click
+from click_help_colors import HelpColorsCommand
 
 from riocli.auth.util import select_project
+from riocli.constants import Colors
 from riocli.project.util import name_to_organization_guid
 from riocli.utils.context import get_root_context
 
 
-@click.command('select')
+@click.command(
+    'select',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('organization-name', type=str)
+@click.option('--interactive/--no-interactive', '--interactive/--silent',
+              is_flag=True, type=bool, default=True,
+              help='Make the selection interactive')
 @click.pass_context
 @name_to_organization_guid
-def select_organization(ctx: click.Context, organization_name: str, organization_guid: str) -> None:
+def select_organization(
+        ctx: click.Context,
+        organization_name: str,
+        organization_guid: str,
+        interactive: bool,
+) -> None:
     """
     Sets the current organization to the one provided
     in the argument and prompts you to select a new project
     in the changed organization
 
     Example:
 
         rio organization select other-org
     """
     ctx = get_root_context(ctx)
 
     if ctx.obj.data['organization_id'] == organization_guid:
-        click.secho("You are already in the '{}' organization".format(organization_name), fg='green')
+        click.secho("You are already in the '{}' organization".format(
+            organization_name), fg=Colors.GREEN)
         return
 
     ctx.obj.data['organization_id'] = organization_guid
     ctx.obj.data['organization_name'] = organization_name
 
-    select_project(ctx.obj, organization=organization_guid)
+    if sys.stdout.isatty() and interactive:
+        select_project(ctx.obj, organization=organization_guid)
+    else:
+        click.secho(
+            "Your organization has been set to '{}'".format(organization_name),
+            fg=Colors.GREEN)
 
     ctx.obj.save()
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/create.py` & `rapyuta-io-cli-4.0.0/riocli/parameter/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-import json
-
 import click
-import yaml
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
+from rapyuta_io.utils.rest_client import HttpMethod
 
-from riocli.config import new_client
+from riocli.constants import Colors
+from riocli.parameter.utils import _api_call
+from riocli.utils import tabulate_data
 
 
-@click.command('create', hidden=True)
-@click.option('--manifest', type=click.File(mode='r', lazy=True),
-              help='Path for the manifest file')
-@click.option('--format', 'format_type', default='json',
-              type=click.Choice(['json', 'yaml'], case_sensitive=False))
-def create_package(manifest: click.File, format_type: str) -> None:
+@click.command(
+    'list',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+def list_configuration_trees() -> None:
     """
-    Create a new package
+    List the Configuration Parameter Trees.
     """
-    data = manifest.read()
-    if format_type == 'json':
-        package = json.loads(data)
-    else:
-        package = yaml.load(data)
-
     try:
-        client = new_client()
-        with spinner():
-            client.create_package(package)
-        click.secho('Package created successfully!', fg='green')
+        data = _api_call(HttpMethod.GET)
+        if 'data' not in data:
+            raise Exception('Failed to list configurations')
+
+        trees = [[tree] for tree in data['data']]
+
+        tabulate_data(trees, headers=['Tree Name'])
+
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/delete.py` & `rapyuta-io-cli-4.0.0/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/deployment.py` & `rapyuta-io-cli-4.0.0/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/list.py` & `rapyuta-io-cli-4.0.0/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/model.py` & `rapyuta-io-cli-4.0.0/riocli/package/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         guid, obj = self.rc.find_depends({"kind": self.kind.lower(), "nameOrGUID": self.metadata.name},
                                          self.metadata.version)
         if not guid:
             return False
 
         return obj
 
-    def create_object(self, client: Client):
+    def create_object(self, client: Client, **kwargs):
         pkg_object = munchify({
             'name': 'default',
             'packageVersion': 'v1.0.0',
             'apiVersion': "2.1.0",
             'description': '',
             'bindable': True,
             'plans': [
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/package/util.py` & `rapyuta-io-cli-4.0.0/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/parameter/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,38 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.constants import Colors
 from riocli.parameter.apply import apply_configurations
 from riocli.parameter.delete import delete_configurations
 from riocli.parameter.diff import diff_configurations
 from riocli.parameter.download import download_configurations
 from riocli.parameter.list import list_configuration_trees
 from riocli.parameter.upload import upload_configurations
 
 
-# from riocli.parameter.diff import diff_configurations
-# from riocli.parameter.download import download_configurations
-
-
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def parameter() -> None:
     """
-    Define groups of executables to deploy together
+    Manage configuration parameters for your devices and deployments
     """
     pass
 
 
-parameter.add_command(upload_configurations)
-parameter.add_command(download_configurations)
 parameter.add_command(diff_configurations)
 parameter.add_command(apply_configurations)
-parameter.add_command(list_configuration_trees)
 parameter.add_command(delete_configurations)
+parameter.add_command(upload_configurations)
+parameter.add_command(download_configurations)
+parameter.add_command(list_configuration_trees)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/apply.py` & `rapyuta-io-cli-4.0.0/riocli/usergroup/delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,60 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-import typing
 
 import click
+from click_help_colors import HelpColorsCommand
+from yaspin.api import Yaspin
 
 from riocli.config import new_client
-from riocli.utils import tabulate_data, print_separator
-
-
-@click.command('apply')
-@click.option('--devices', type=click.STRING, multiple=True, default=(),
-              help='Device names to apply configurations')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None,
-              help='Tree names to apply')
-@click.option('--retry-limit', type=click.INT, default=0,
-              help='Retry limit')
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
-              help="Skip confirmation")
-def apply_configurations(devices: typing.List, tree_names: str = None, retry_limit: int = 0,
-                         silent: bool = False) -> None:
+from riocli.constants import Colors, Symbols
+from riocli.usergroup.util import name_to_guid
+from riocli.utils.spinner import with_spinner
+
+
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--force', '-f', '--silent', 'force', is_flag=True,
+              default=False, help='Skip confirmation')
+@click.argument('group-name')
+@click.pass_context
+@with_spinner(text="Deleting user group...")
+@name_to_guid
+def delete_usergroup(
+        ctx: click.Context,
+        group_name: str,
+        group_guid: str,
+        force: bool,
+        spinner: Yaspin = None,
+) -> None:
     """
-    Apply a set of configurations to a list of devices
+    Delete usergroup from organization
     """
+    if not force:
+        with spinner.hidden():
+            click.confirm('Deleting usergroup {} ({})'.format(group_name, group_guid), abort=True)
+
     try:
         client = new_client()
-
-        online_devices = client.get_all_devices(online_device=True)
-        device_map = {d.name: d for d in online_devices}
-
-        if devices:
-            device_ids = {device_map[d].uuid: d for d in devices if d in device_map}
-        else:
-            device_ids = {v.uuid: k for k, v in device_map.items()}
-
-        if not device_ids:
-            click.secho("invalid devices or no device is currently online", fg='red')
-            raise SystemExit(1)
-
-        click.secho('Online Devices: {}'.format(','.join(device_ids.values())), fg='green')
-
-        printable_tree_names = ','.join(tree_names) if tree_names != "" else "*all*"
-        click.secho('Config Trees: {}'.format(printable_tree_names), fg='green')
-
-        if not silent:
-            click.confirm(
-                "Do you want to apply the configurations?",
-                default=True, abort=True)
-
-        response = client.apply_parameters(list(device_ids.keys()),
-                                           list(tree_names),
-                                           retry_limit)
-
-        print_separator()
-
-        result = []
-        for device in response:
-            device_name = device_ids[device['device_id']]
-            success = device['success'] or "Partial"
-            result.append([device_name, success])
-
-        tabulate_data(result, headers=["Device", "Success"])
-    except IOError as e:
-        click.secho(str(e.__traceback__), fg='red')
-        click.secho(str(e), fg='red')
+        org_guid = ctx.obj.data.get('organization_id')
+        client.delete_usergroup(org_guid, group_guid)
+        spinner.text = click.style('User group deleted successfully.', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
+    except Exception as e:
+        spinner.text = click.style('Failed to delete usergroup: {}'.format(e), Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/delete.py` & `rapyuta-io-cli-4.0.0/riocli/disk/delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-
 import click
+from click_help_colors import HelpColorsCommand
 from rapyuta_io.utils.rest_client import HttpMethod
 
-from riocli.parameter.utils import _api_call
-
-
-@click.command('delete')
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, default=False,
-              help="Skip confirmation")
-@click.argument('tree', type=click.STRING)
-def delete_configurations(tree: str, silent: bool = False) -> None:
+from riocli.constants import Symbols, Colors
+from riocli.disk.util import name_to_guid, _api_call
+from riocli.utils.spinner import with_spinner
+
+
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--force', '-f', 'force', is_flag=True, default=False,
+              help='Skip confirmation')
+@click.argument('disk-name', required=True, type=str)
+@name_to_guid
+@with_spinner(text="Deleting disk...")
+def delete_disk(
+        disk_name: str,
+        disk_guid: str,
+        force: bool,
+        spinner=None
+) -> None:
     """
-    Deletes the Configuration Parameter Tree.
+    Delete a disk
     """
-    click.secho('Configuration Parameter {} will be deleted'.format(tree))
-
-    if not silent:
-        click.confirm('Do you want to proceed?', default=True, abort=True)
+    with spinner.hidden():
+        if not force:
+            click.confirm(
+                'Deleting disk {} ({})'.format(disk_name, disk_guid), abort=True)
 
     try:
-        data = _api_call(HttpMethod.DELETE, name=tree)
-        if data.get('data') != 'ok':
-            raise Exception('Something went wrong!')
+        _api_call(HttpMethod.DELETE, guid=disk_guid, load_response=False)
 
-    except IOError as e:
-        click.secho(str(e.__traceback__), fg='red')
-        click.secho(str(e), fg='red')
+        spinner.text = click.style('Disk deleted successfully.', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
+    except Exception as e:
+        spinner.text = click.style('Failed to delete disk: {}'.format(str(e)), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/diff.py` & `rapyuta-io-cli-4.0.0/riocli/parameter/diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,77 +20,96 @@
 import os.path
 from difflib import unified_diff
 from filecmp import dircmp
 from tempfile import TemporaryDirectory
 from typing import Tuple
 
 import click
+from click_help_colors import HelpColorsCommand
 from rapyuta_io.utils.error import APIError, InternalServerError
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.parameter.utils import filter_trees
 
 
-@click.command('diff')
+@click.command(
+    'diff',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--tree-names', type=click.STRING, multiple=True, default=None,
               help='Tree names to fetch')
 @click.argument('path', type=click.Path(exists=True), required=False)
 def diff_configurations(path: str, tree_names: Tuple = None) -> None:
     """
-    Diff between the Local and Cloud Configuration Trees.
+    Diff between the local and cloud configuration trees.
     """
     trees = filter_trees(path, tree_names)
 
     try:
         client = new_client()
         with TemporaryDirectory(prefix='riocli-') as tmp_path:
-            client.download_configurations(tmp_path, tree_names=list(tree_names))
+            client.download_configurations(tmp_path,
+                                           tree_names=list(tree_names))
 
             for tree in trees:
-                left_tree, right_tree = os.path.join(tmp_path, tree), os.path.join(path, tree)
+                left_tree = os.path.join(tmp_path, tree)
+                right_tree = os.path.join(path, tree)
                 diff_tree(left_tree, right_tree)
     except (APIError, InternalServerError) as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
 
 
 def diff_tree(left: str, right: str) -> None:
     comp = dircmp(left, right)
 
+    for f in comp.common_dirs:
+        remote_dir, local_dir = os.path.join(comp.left, f), os.path.join(
+            comp.right, f)
+        diff_tree(remote_dir, local_dir)
+
     for f in comp.diff_files:
-        remote_file, local_file = os.path.join(comp.left, f), os.path.join(comp.right, f)
+        remote_file, local_file = os.path.join(comp.left, f), os.path.join(
+            comp.right, f)
         diff_file(remote_file, local_file)
 
     for f in comp.right_only:
-        remote_file, local_file = os.path.join(comp.left, f), os.path.join(comp.right, f)
+        remote_file, local_file = os.path.join(comp.left, f), os.path.join(
+            comp.right, f)
         changed_file(remote_file, local_file, right_only=True)
 
     for f in comp.left_only:
-        remote_file, local_file = os.path.join(comp.left, f), os.path.join(comp.right, f)
+        remote_file, local_file = os.path.join(comp.left, f), os.path.join(
+            comp.right, f)
         changed_file(remote_file, local_file, left_only=True)
 
 
 def diff_file(left: str, right: str):
     try:
         with open(left, 'r', encoding='utf-8') as left_f:
             left_lines = left_f.readlines()
 
         with open(right, 'r', encoding='utf-8') as right_f:
             right_lines = right_f.readlines()
     except UnicodeDecodeError:
         changed_file(left, right, binary=True)
         return
 
-    diff = unified_diff(left_lines, right_lines, fromfile=left, tofile=right, lineterm='')
+    diff = unified_diff(left_lines, right_lines, fromfile=left, tofile=right,
+                        lineterm='\n')
 
     for line in diff:
-        click.secho(line)
+        click.secho(line, nl=False)
 
 
-def changed_file(left: str, right: str, left_only: bool = False, right_only: bool = False, binary: bool = False):
+def changed_file(left: str, right: str, left_only: bool = False,
+                 right_only: bool = False, binary: bool = False):
     click.secho('--- {}'.format(left))
     click.secho('+++ {}'.format(right))
 
     if left_only:
         click.secho('deleted file')
         click.secho()
     elif right_only:
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/download.py` & `rapyuta-io-cli-4.0.0/riocli/parameter/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,51 +8,71 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
+from os.path import abspath
 from tempfile import mkdtemp
-from xmlrpc.client import Boolean
 
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
-from riocli.parameter.utils import display_trees
+from riocli.constants import Symbols, Colors
+from riocli.utils.spinner import with_spinner
 
 
 # -----------------------------------------------------------------------------
 #
 # Configurations
 # Args
 #    path,  tree_names,  delete_existing=True|False
 # -----------------------------------------------------------------------------
 
 
-@click.command('download')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None, help='Tree names to fetch')
-@click.option('--overwrite', '--delete-existing', 'delete_existing', is_flag=True,
+@click.command(
+    'download',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--tree-names', type=click.STRING, multiple=True, default=None,
+              help='Tree names to fetch')
+@click.option('--overwrite', '--delete-existing', 'delete_existing',
+              is_flag=True,
               help='Overwrite existing parameter tree')
 @click.argument('path', type=click.Path(exists=True), required=False)
-def download_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: Boolean = False) -> None:
+@with_spinner(text='Download configurations...', timer=True)
+def download_configurations(
+        path: str,
+        tree_names: typing.Tuple[str] = None,
+        delete_existing: bool = False,
+        spinner=None
+) -> None:
     """
-    Download the Configuration Parameter trees.
+    Download configuration parameter trees from rapyuta.io
     """
     if path is None:
-        # Not using the Context Manager because we need to persist the Temporary directory.
+        # Not using the Context Manager because
+        # we need to persist the temporary directory.
         path = mkdtemp()
 
-    click.secho('Downloading at {}'.format(path))
+    spinner.write('Downloading at {}'.format(abspath(path)))
 
     try:
         client = new_client()
 
-        with spinner():
-            client.download_configurations(path, tree_names=list(tree_names),
-                                           delete_existing_trees=delete_existing)
-
-        click.secho('✅ Configuration Parameters downloaded successfully', fg='green')
+        client.download_configurations(
+            path,
+            tree_names=list(tree_names),
+            delete_existing_trees=delete_existing
+        )
+
+        spinner.text = click.style("Configurations downloaded successfully.",
+                                   fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(e, fg='red')
+        spinner.text = click.style(e, fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/upload.py` & `rapyuta-io-cli-4.0.0/riocli/shell/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,74 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
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
-
-import typing
+import os
 
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
+from click_repl import repl
+from prompt_toolkit.history import FileHistory, ThreadedHistory
+
+from riocli.config import Configuration
+from riocli.shell.prompt import prompt_callback
+
 
-from riocli.config import new_client
-from riocli.parameter.utils import filter_trees, display_trees
+@click.command(
+    cls=HelpColorsCommand,
+    help_headers_color='yellow',
+    help_options_color='green',
+)
+@click.pass_context
+def shell(ctx: click.Context):
+    """
+    Interactive Shell for Rapyuta.io
+    """
+    start_shell(ctx)
 
 
-@click.command('upload')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=[], help='Directory names to upload')
-@click.option('--recreate', '--delete-existing', 'delete_existing', is_flag=True,
-              help='Overwrite existing parameter tree')
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, default=False, help="Skip confirmation")
-@click.argument('path', type=click.Path(exists=True))
-def upload_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: bool = False,
-                          silent: bool = False) -> None:
+@click.command(
+    'repl',
+    cls=HelpColorsCommand,
+    help_headers_color='yellow',
+    help_options_color='green',
+    hidden=True
+)
+@click.pass_context
+def deprecated_repl(ctx: click.Context):
     """
-    Upload a set of Configuration Parameter directory trees.
+    [Deprecated] Use "rio shell" instead
     """
-    trees = filter_trees(path, tree_names)
+    start_shell(ctx)
+
+
+def start_shell(ctx: click.Context):
+    prompt_config = _parse_config(ctx.obj)
+    while True:
+        try:
+            repl(click.get_current_context(), prompt_kwargs=prompt_config)
+        except Exception as e:
+            click.secho(str(e), fg='red')
+        else:
+            break
+
+
+def _parse_config(config: Configuration) -> dict:
+    history_path = os.path.join(click.get_app_dir(config.APP_NAME), "history")
+    default_prompt_kwargs = {
+        'history': ThreadedHistory(FileHistory(history_path)),
+        'message': prompt_callback,
+        'enable_suspend': True
+    }
+
+    shell_config = config.data.get('shell', {})
 
-    click.secho('Following Trees will be uploaded')
-    click.secho('')
-    display_trees(path, trees)
-
-    if not silent:
-        click.confirm('Do you want to proceed?', default=True, abort=True)
-
-    try:
-        client = new_client()
-        with spinner():
-            client.upload_configurations(rootdir=path, tree_names=trees, delete_existing_trees=delete_existing,
-                                         as_folder=True)
-
-        click.secho('✅ Configuration parameters uploaded successfully', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+    return {**default_prompt_kwargs, **shell_config}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/parameter/utils.py` & `rapyuta-io-cli-4.0.0/riocli/parameter/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 from filecmp import dircmp
 
 import click
 from directory_tree import display_tree
 from rapyuta_io.utils import RestClient
 
 from riocli.config import Configuration
+from riocli.constants import Colors
 
 
-def filter_trees(root_dir: str, tree_names: typing.Tuple[str]) -> typing.List[str]:
+def filter_trees(
+        root_dir: str,
+        tree_names: typing.Tuple[str]
+) -> typing.List[str]:
     trees = []
     for each in os.listdir(root_dir):
         full_path = os.path.join(root_dir, each)
 
         if not os.path.isdir(full_path):
             continue
 
@@ -39,31 +43,36 @@
 
     if tree_names and not trees:
         raise Exception('specified tree names are invalid')
 
     return trees
 
 
-def display_trees(root_dir: str, trees: typing.List[str] = []) -> None:
+def display_trees(root_dir: str, trees: typing.List[str]) -> None:
+    trees = trees or []
     for each in trees:
         tree_out = display_tree(os.path.join(root_dir, each), string_rep=True)
-        click.secho(tree_out, fg='yellow')
+        click.secho(tree_out, fg=Colors.YELLOW)
 
 
-def _api_call(method: str, name: typing.Union[str, None] = None,
-              payload: typing.Union[typing.Dict, None] = None, load_response: bool = True,
-              ) -> typing.Any:
+def _api_call(
+        method: str,
+        name: typing.Union[str, None] = None,
+        payload: typing.Union[typing.Dict, None] = None,
+        load_response: bool = True,
+) -> typing.Any:
     config = Configuration()
     catalog_host = config.data.get(
         'core_api_host', 'https://gaapiserver.apps.rapyuta.io')
     url = '{}/api/paramserver/tree'.format(catalog_host)
     if name:
         url = '{}/{}'.format(url, name)
     headers = config.get_auth_header()
-    response = RestClient(url).method(method).headers( headers).execute(payload=payload)
+    response = RestClient(url).method(method).headers(headers).execute(
+        payload=payload)
     data = None
     err_msg = 'error in the api call'
     if load_response:
         data = json.loads(response.text)
 
     if not response.ok:
         err_msg = data.get('error')
@@ -73,9 +82,12 @@
 
 class DeepDirCmp(dircmp):
 
     def phase3(self) -> None:
         # shallow=False enables the behaviour of matching the File content. The
         # original dircmp Class only compares os.Stat between the files, and
         # gives no way to modify the behaviour.
-        f_comp = filecmp.cmpfiles(self.left, self.right, self.common_files, shallow=False)
+        f_comp = filecmp.cmpfiles(self.left,
+                                  self.right,
+                                  self.common_files,
+                                  shallow=False)
         self.same_files, self.diff_files, self.funny_files = f_comp
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/create.py` & `rapyuta-io-cli-4.0.0/riocli/project/create.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_v2_client
+from riocli.constants import Symbols, Colors
 from riocli.project.util import name_to_organization_guid
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('create')
+@click.command(
+    'create',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('project-name', type=str)
 @click.option('--organization', 'organization_name',
               help='Pass organization name for which project needs to be created. Default will be current organization')
 @click.pass_context
 @name_to_organization_guid
-def create_project(ctx: click.Context, project_name: str,
-                   organization_guid: str, organization_name: str) -> None:
+@with_spinner(text="Creating project...")
+def create_project(
+        ctx: click.Context,
+        project_name: str,
+        organization_guid: str,
+        organization_name: str,
+        spinner=None,
+) -> None:
     """
     Creates a new project
     """
     if not organization_guid:
         organization_guid = ctx.obj.data.get('organization_id')
 
     payload = {
@@ -41,13 +54,16 @@
             }
         },
         "spec": {}
     }
 
     try:
         client = new_v2_client(with_project=False)
-        with spinner():
-            client.create_project(payload)
-        click.secho('Project created successfully!', fg='green')
+        client.create_project(payload)
+        spinner.text = click.style(
+            'Project created successfully.', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho('failed to create project: {}'.format(e), fg='red')
+        spinner.text = click.style(
+            'Failed to create project: {}'.format(e), Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/delete.py` & `rapyuta-io-cli-4.0.0/riocli/project/select.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
-from riocli.config import new_v2_client
+from riocli.constants import Colors, Symbols
 from riocli.project.util import name_to_guid
+from riocli.utils.context import get_root_context
 
 
-@click.command('delete')
-@click.option('--force', '-f', '--silent', 'force', is_flag=True,
-              help='Skip confirmation')
+@click.command(
+    'select',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('project-name', type=str)
 @name_to_guid
-def delete_project(force: bool, project_name: str, project_guid: str) -> None:
+@click.pass_context
+def select_project(
+        ctx: click.Context,
+        project_name: str,
+        project_guid: str,
+) -> None:
     """
-    Deletes the project from the Platform
+    Sets the given project in the CLI context. All other resources use this project to act upon.
     """
-    if not force:
-        click.confirm(
-            'Deleting project {} ({})'.format(project_name, project_guid),
-            abort=True)
+    ctx = get_root_context(ctx)
 
-    try:
-        client = new_v2_client()
-        with spinner():
-            client.delete_project(project_guid)
-        click.secho('Project deleted successfully!', fg='green')
-    except Exception as e:
-        click.secho('failed to delete project: {}'.format(e), fg='red')
-        raise SystemExit(1)
+    ctx.obj.data['project_id'] = project_guid
+    ctx.obj.data['project_name'] = project_name
+    ctx.obj.save()
+
+    click.secho('{} Project {} ({}) is selected!'.format(
+        Symbols.SUCCESS,
+        project_name,
+        project_guid),
+        fg=Colors.GREEN)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/features/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/secret/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,24 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
-from riocli.project.features.vpn import vpn
+from riocli.constants import Colors
+from riocli.secret.create import create_secret
+from riocli.secret.delete import delete_secret
+from riocli.secret.import_secret import import_secret
+from riocli.secret.inspect import inspect_secret
+from riocli.secret.list import list_secrets
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
-def features():
+def secret() -> None:
     """
-    Toggle features on a project
+    Credentials for Git Hosting or Container Registries
     """
     pass
 
 
-features.add_command(vpn)
+secret.add_command(create_secret)
+secret.add_command(delete_secret)
+secret.add_command(list_secrets)
+secret.add_command(inspect_secret)
+secret.add_command(import_secret)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/features/vpn.py` & `rapyuta-io-cli-4.0.0/riocli/project/features/vpn.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,24 +8,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_v2_client
+from riocli.constants import Colors, Symbols
 from riocli.project.util import name_to_guid
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('vpn')
+@click.command(
+    'vpn',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('project-name', type=str)
 @click.argument('enable', type=bool)
 @name_to_guid
-def vpn(project_name: str, project_guid: str, enable: bool) -> None:
+@with_spinner()
+def vpn(
+        project_name: str,
+        project_guid: str,
+        enable: bool,
+        spinner=None,
+) -> None:
     """
     Enable or disable VPN on a project
 
     Example: rio project features vpn "my-project" true
     """
     client = new_v2_client(with_project=False)
 
@@ -36,14 +50,18 @@
         "spec": {
             "features": {
                 "vpn": enable
             }
         }
     }
 
+    state = 'Enabling' if enable else 'Disabling'
+    spinner.text = click.style('{} VPN...'.format(state), fg=Colors.YELLOW)
+
     try:
-        r = client.update_project(project_guid, body)
+        client.update_project(project_guid, body)
+        spinner.text = click.style('Done', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho("❌ Failed: {}".format(e), fg='red')
+        spinner.text = click.style("Failed: {}".format(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1) from e
-
-    click.secho("✅ VPN has been {}".format("enabled" if enable else "disabled"), fg='green')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/project/inspect.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,31 +8,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
+from click_help_colors import HelpColorsCommand
 from munch import unmunchify
 
 from riocli.config import new_v2_client
+from riocli.constants import Colors
 from riocli.project.util import name_to_guid
 from riocli.utils import inspect_with_format
 
 
-@click.command('inspect')
+@click.command(
+    'inspect',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--format', '-f', 'format_type', default='yaml',
               type=click.Choice(['json', 'yaml'], case_sensitive=False))
 @click.argument('project-name', type=str)
 @name_to_guid
 def inspect_project(format_type: str, project_name: str,
                     project_guid: str) -> None:
     """
     Inspect the project resource
     """
     try:
         client = new_v2_client(with_project=False)
         project = client.get_project(project_guid)
         inspect_with_format(unmunchify(project), format_type)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/list.py` & `rapyuta-io-cli-4.0.0/riocli/project/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
+from click_help_colors import HelpColorsCommand
 from munch import unmunchify
 from rapyuta_io import Project
 
 from riocli.config import new_v2_client
+from riocli.constants import Colors
 from riocli.project.util import name_to_organization_guid
 from riocli.utils import tabulate_data
 
 
-@click.command('list')
+@click.command(
+    'list',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--organization', 'organization_name',
               help='Pass organization name for which project needs to be created. Default will be current organization')
 @click.option('--wide', '-w', is_flag=True, default=False,
               help='Print more details', type=bool)
 @click.pass_context
 @name_to_organization_guid
 def list_project(ctx: click.Context = None, organization_guid: str = None,
@@ -37,15 +44,15 @@
     try:
         client = new_v2_client(with_project=False)
         projects = client.list_projects(organization_guid=organization_guid)
         projects = sorted(projects, key=lambda p: p.metadata.name.lower())
         current = ctx.obj.data.get('project_id', None)
         _display_project_list(projects, current, show_header=True, wide=wide)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
 
 
 def _display_project_list(projects: typing.List[Project], current: str = None,
                           show_header: bool = True,
                           wide: bool = False) -> None:
     headers = []
@@ -53,18 +60,18 @@
         headers = ['Project ID', 'Project Name', 'Status']
         if wide:
             headers.extend(['Created At', 'Creator', "Features"])
 
     data = []
     for project in projects:
         metadata = project.metadata
-        fg = None
+        fg, bold = None, False
         if metadata.guid == current:
-            fg = 'green'
-
+            fg = Colors.GREEN
+            bold = True
         row = [metadata.guid, metadata.name, project.status.status]
         if wide:
             row.extend([metadata.createdAt, metadata.creatorGUID,
                         unmunchify(project.spec.features)])
-        data.append([click.style(v, fg=fg) for v in row])
+        data.append([click.style(v, fg=fg, bold=bold) for v in row])
 
     tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/model.py` & `rapyuta-io-cli-4.0.0/riocli/project/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,44 +19,46 @@
 
 from riocli.config import new_v2_client, Configuration
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 
 PROJECT_READY_TIMEOUT = 150
 
+
 class Project(Model):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
         guid, obj = self.rc.find_depends(
             {"kind": "project", "nameOrGUID": self.metadata.name})
         if not guid:
             return False
 
         return obj
 
-    def create_object(self, client: Client) -> typing.Any:
+    def create_object(self, client: Client, **kwargs) -> typing.Any:
         client = new_v2_client()
 
         # convert to a dict and remove the ResolverCache
         # field since it's not JSON serializable
         project = unmunchify(self)
         project.pop("rc", None)
 
         # set organizationGUID irrespective of it being present in the manifest
         project['metadata']['organizationGUID'] = Configuration().data[
             'organization_id']
 
         r = client.create_project(project)
 
         try:
-            wait(self.is_ready, timeout_seconds=PROJECT_READY_TIMEOUT, sleep_seconds=(1, 30, 2))
+            wait(self.is_ready, timeout_seconds=PROJECT_READY_TIMEOUT,
+                 sleep_seconds=(1, 30, 2))
         except TimeoutExpired as e:
             raise e
 
         return unmunchify(r)
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         client = new_v2_client()
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/project/util.py` & `rapyuta-io-cli-4.0.0/riocli/project/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import functools
 import typing
 
 import click
 from rapyuta_io import Client
 
 from riocli.config import new_client, new_v2_client
+from riocli.constants import Colors
 from riocli.utils.selector import show_selection
 from riocli.v2client import Client as v2Client
 
 
 def name_to_guid(f: typing.Callable) -> typing.Callable:
     @functools.wraps(f)
     def decorated(**kwargs: typing.Any):
@@ -36,15 +37,15 @@
         if name is None:
             name = get_project_name(client, guid)
 
         if guid is None:
             try:
                 guid = find_project_guid(client, name)
             except Exception as e:
-                click.secho(str(e), fg='red')
+                click.secho(str(e), fg=Colors.RED)
                 raise SystemExit(1)
 
         kwargs['project_name'] = name
         kwargs['project_guid'] = guid
         f(**kwargs)
 
     return decorated
@@ -106,15 +107,15 @@
             try:
                 if name.startswith('org-'):
                     guid = name
                     name = get_organization_name(client, guid)
                 else:
                     guid = find_organization_guid(client, name)
             except Exception as e:
-                click.secho(str(e), fg='red')
+                click.secho(str(e), fg=Colors.RED)
                 raise SystemExit(1)
         kwargs['organization_name'] = name
         kwargs['organization_guid'] = guid
         f(*args, **kwargs)
 
     return decorated
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/rosbag/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/rosbag/blob.py` & `rapyuta-io-cli-4.0.0/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/rosbag/job.py` & `rapyuta-io-cli-4.0.0/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/create.py` & `rapyuta-io-cli-4.0.0/riocli/secret/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/delete.py` & `rapyuta-io-cli-4.0.0/riocli/project/delete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,58 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
-from riocli.config import new_client
-from riocli.secret.util import name_to_guid
+from riocli.config import new_v2_client
+from riocli.constants import Symbols, Colors
+from riocli.project.util import name_to_guid
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('delete')
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--force', '-f', '--silent', 'force', is_flag=True,
-              default=False, help='Skip confirmation')
-@click.argument('secret-name', type=str)
+              help='Skip confirmation')
+@click.argument('project-name', type=str)
 @name_to_guid
-def delete_secret(force: str, secret_name: str, secret_guid: str) -> None:
+@with_spinner(text="Deleting project...")
+def delete_project(
+        force: bool,
+        project_name: str,
+        project_guid: str,
+        spinner=None,
+) -> None:
     """
-    Deletes the secret resource from the Platform
+    Deletes a project
     """
     if not force:
-        click.confirm('Deleting secret {} ({})'.format(secret_name, secret_guid), abort=True)
+        with spinner.hidden():
+            click.confirm('Deleting project {} ({})'.format(
+                project_name, project_guid), abort=True)
 
     try:
-        client = new_client()
-        with spinner():
-            client.delete_secret(secret_guid)
-        click.secho('Secret deleted successfully!', fg='green')
+        client = new_v2_client()
+        client.delete_project(project_guid)
+        spinner.text = click.style(
+            'Project deleted successfully.', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.text = click.style(
+            'Failed to delete project: {}'.format(e), Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/import_secret.py` & `rapyuta-io-cli-4.0.0/riocli/secret/import_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/secret/inspect.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
+from click_help_colors import HelpColorsCommand
 from rapyuta_io import Secret
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.secret.util import name_to_guid
 from riocli.utils import inspect_with_format
 
 
-@click.command('inspect')
+@click.command(
+    'inspect',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--format', '-f', 'format_type', default='yaml',
               type=click.Choice(['json', 'yaml'], case_sensitive=False))
 @click.argument('secret-name', type=str)
 @name_to_guid
 def inspect_secret(format_type: str, secret_name: str, secret_guid: str) -> None:
     """
-    Inspect the secret resource
+    Inspect a secret
     """
     try:
         client = new_client()
         secret = client.get_secret(secret_guid)
         data = make_secret_inspectable(secret)
         inspect_with_format(data, format_type)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
 
 
 def make_secret_inspectable(obj: Secret) -> dict:
     return {
         'created_at': obj.created_at,
         'creator': obj.creator,
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/list.py` & `rapyuta-io-cli-4.0.0/riocli/secret/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,30 +14,36 @@
 import typing
 
 import click
 from rapyuta_io import Secret
 
 from riocli.config import new_client
 from riocli.utils import tabulate_data
+from riocli.constants import Colors
+from click_help_colors import HelpColorsCommand
 
-
-@click.command('list')
+@click.command(
+    'list',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--secret-type', '-t', default=['docker', 'source'], multiple=True,
               help='Types to filter the list of Secret [default: docker,source]')
 def list_secrets(secret_type: typing.Union[str, typing.Tuple[str]]) -> None:
     """
     List the secrets in the selected project
     """
     try:
         client = new_client()
         secrets = client.list_secrets()
         secrets = sorted(secrets, key=lambda s: s.name.lower())
         _display_secret_list(secrets, secret_type, show_header=True)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
 
 
 def _display_secret_list(
         secrets: typing.List[Secret],
         secret_type: typing.Union[str, typing.Tuple[str]],
         show_header: bool = True,
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/model.py` & `rapyuta-io-cli-4.0.0/riocli/secret/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import typing
 
-from rapyuta_io import Secret as v1Secret, SecretConfigDocker, \
-    SecretConfigSourceBasicAuth, \
-    SecretConfigSourceSSHAuth, Client
+from rapyuta_io import (
+    Client,
+    Secret as v1Secret,
+    SecretConfigDocker,
+    SecretConfigSourceBasicAuth,
+    SecretConfigSourceSSHAuth,
+)
 
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 
 
 class Secret(Model):
-
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        _, secret = self.rc.find_depends(
-            {'kind': 'secret', 'nameOrGUID': self.metadata.name})
+        _, secret = self.rc.find_depends({
+            'kind': 'secret',
+            'nameOrGUID': self.metadata.name
+        })
+
         if not secret:
             return False
 
         return secret
 
-    def create_object(self, client: Client) -> v1Secret:
+    def create_object(self, client: Client, **kwargs) -> v1Secret:
         secret = client.create_secret(self.to_v1())
         return secret
 
     def update_object(self, client: Client, obj: typing.Any) -> None:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
@@ -47,24 +53,32 @@
     def to_v1(self) -> v1Secret:
         if self.spec.type == 'Docker':
             return self._docker_secret_to_v1()
         else:
             return self._git_secret_to_v1()
 
     def _docker_secret_to_v1(self) -> v1Secret:
-        config = SecretConfigDocker(self.spec.docker.username, self.spec.docker.password, self.spec.docker.email,
-                                    self.spec.docker.registry)
+        config = SecretConfigDocker(
+            self.spec.docker.username,
+            self.spec.docker.password,
+            self.spec.docker.email,
+            self.spec.docker.registry,
+        )
         return v1Secret(self.metadata.name, config)
 
     def _git_secret_to_v1(self) -> v1Secret:
         if self.spec.git.authMethod == 'SSH Auth':
             config = SecretConfigSourceSSHAuth(self.spec.git.privateKey)
         elif self.spec.git.authMethod == 'HTTP/S Basic Auth':
             ca_cert = self.spec.git.get('ca_cert', None)
-            config = SecretConfigSourceBasicAuth(self.spec.git.username, self.spec.git.password, ca_cert=ca_cert)
+            config = SecretConfigSourceBasicAuth(
+                self.spec.git.username,
+                self.spec.git.password,
+                ca_cert=ca_cert
+            )
         elif self.spec.git.authMethod == 'HTTP/S Token Auth':
             # TODO(ankit): Implement it once SDK has support for it.
             raise Exception('token-based secret is not supported yet!')
         else:
             raise Exception('invalid gitAuthMethod for secret!')
 
         return v1Secret(self.metadata.name, config)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/source_secret.py` & `rapyuta-io-cli-4.0.0/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/secret/util.py` & `rapyuta-io-cli-4.0.0/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/shell/prompt.py` & `rapyuta-io-cli-4.0.0/riocli/constants/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
-import click
 
+from riocli.constants.colors import Colors
+from riocli.constants.symbols import Symbols
 
-@click.pass_context
-def prompt_callback(ctx: click.Context) -> str:
-    organization_name = ctx.obj.data['organization_name']
-    project_name = ctx.obj.data['project_name']
-    return '{}:{} > '.format(organization_name, project_name)
+__all__ = [Colors, Symbols]
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/static_route/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/static_route/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.constants import Colors
 from riocli.static_route.create import create_static_route
 from riocli.static_route.delete import delete_static_route
 from riocli.static_route.inspect import inspect_static_route
 from riocli.static_route.list import list_static_routes
 from riocli.static_route.open import open_static_route
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
 )
 def static_route() -> None:
     """
     Named routes for the deployments with exposed endpoints
     """
     pass
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/static_route/create.py` & `rapyuta-io-cli-4.0.0/riocli/static_route/create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
+from riocli.constants import Colors, Symbols
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('create')
+@click.command(
+    'create',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('prefix', type=str)
-def create_static_route(prefix: str) -> None:
+@with_spinner(text="Creating static route...")
+def create_static_route(prefix: str, spinner=None) -> None:
     """
-    Creates a new instance of static route
+    Creates a new static route
     """
     try:
         client = new_client()
-        with spinner():
-            route = client.create_static_route(prefix)
-        click.secho("Static Route created successfully for URL {}".format(route.urlString), fg='green')
+        route = client.create_static_route(prefix)
+        spinner.text = click.style(
+            'Static Route created successfully for URL {}'.format(route.urlString), fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.text = click.style('Failed to create static route: {}'.format(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/static_route/delete.py` & `rapyuta-io-cli-4.0.0/riocli/static_route/open.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
+from riocli.constants import Colors
 from riocli.static_route.util import name_to_guid
 
 
-@click.command('delete')
-@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
+@click.command(
+    'open',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.argument('static-route', type=str)
 @name_to_guid
-def delete_static_route(static_route: str, static_route_guid: str, force: bool) -> None:
+def open_static_route(static_route, static_route_guid) -> None:
     """
-    Deletes the static route resource from the Platform
+    Opens the static route in the default browser
     """
-
-    if not force:
-        click.confirm('Deleting static route {} ({})'.format(static_route, static_route_guid),
-                      abort=True)
-
     try:
         client = new_client()
-        with spinner():
-            client.delete_static_route(static_route_guid)
-        click.secho('Static Route deleted successfully!', fg='green')
+        route = client.get_static_route(static_route_guid)
+        click.launch(url='https://{}'.format(route.urlString), wait=False)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/static_route/inspect.py` & `rapyuta-io-cli-4.0.0/riocli/static_route/delete.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
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
 import click
-from rapyuta_io.clients.static_route import StaticRoute
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_client
+from riocli.constants import Colors, Symbols
 from riocli.static_route.util import name_to_guid
-from riocli.utils import inspect_with_format
+from riocli.utils.spinner import with_spinner
 
 
-@click.command('inspect')
-@click.option('--format', '-f', 'format_type',
-              type=click.Choice(['json', 'yaml'], case_sensitive=True), default='yaml')
+@click.command(
+    'delete',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
 @click.argument('static-route', type=str)
 @name_to_guid
-def inspect_static_route(format_type: str, static_route: str, static_route_guid: str) -> None:
+@with_spinner(text="Deleting static route...")
+def delete_static_route(
+        static_route: str,
+        static_route_guid: str,
+        force: bool,
+        spinner=None,
+) -> None:
     """
-    Inspect the static route resource
+    Deletes a static route
     """
+    with spinner.hidden():
+        if not force:
+            click.confirm(
+                'Deleting static route {} ({})'.format(
+                    static_route, static_route_guid), abort=True)
+
     try:
         client = new_client()
-        route = client.get_static_route(static_route_guid)
-        data = make_static_route_inspectable(route)
-        inspect_with_format(data, format_type)
+        client.delete_static_route(static_route_guid)
+        spinner.text = click.style(
+            'Static Route deleted successfully ', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.text = click.style('Failed to delete static route: {}'.format(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1)
-
-
-def make_static_route_inspectable(static_route_data: StaticRoute) -> dict:
-    return {
-        'created_at': static_route_data.CreatedAt,
-        'updated_at': static_route_data.UpdatedAt,
-        'deleted_at': static_route_data.DeletedAt,
-        'guid': static_route_data.guid,
-        'url_prefix': static_route_data.urlPrefix,
-        'url': static_route_data.urlString,
-        'creator': static_route_data.creator,
-        'project': static_route_data.projectGUID,
-        'metadata': static_route_data.metadata.__dict__,
-    }
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/static_route/model.py` & `rapyuta-io-cli-4.0.0/riocli/static_route/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,22 +21,25 @@
 
 
 class StaticRoute(Model):
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        _, static_route = self.rc.find_depends({'kind': 'staticroute',
-                                                'nameOrGUID': self.metadata.name})
+        _, static_route = self.rc.find_depends({
+            'kind': 'staticroute',
+            'nameOrGUID': self.metadata.name
+        })
+
         if not static_route:
             return False
 
         return static_route
 
-    def create_object(self, client: Client) -> v1StaticRoute:
+    def create_object(self, client: Client, **kwargs) -> v1StaticRoute:
         static_route = client.create_static_route(self.metadata.name)
         return static_route
 
     def update_object(self, client: Client, obj: typing.Any) -> None:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any):
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/static_route/util.py` & `rapyuta-io-cli-4.0.0/riocli/static_route/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 import typing
 
-import click
 from rapyuta_io import Client
-from rapyuta_io.clients.static_route import StaticRoute
 
 from riocli.config import new_client
 
 
 def name_to_guid(f: typing.Callable) -> typing.Callable:
     @functools.wraps(f)
     def decorated(**kwargs: typing.Any):
@@ -55,27 +53,10 @@
     for route in routes:
         if route.urlPrefix == name or route.urlString == name:
             return route.guid
 
     raise StaticRouteNotFound()
 
 
-def repr_static_routes(routes: typing.List[StaticRoute]) -> None:
-    header = '{:<36} {:<25} {:36} {:36} {:32}'.format(
-        'Static Route ID',
-        'Name',
-        'Full URL',
-        'Creator',
-        'Created At',
-    )
-    click.echo(click.style(header, fg='yellow'))
-    for route in routes:
-        click.secho(
-            '{:<36} {:<25} {:36} {:36} {:32}'.
-            format(route.guid, route.urlPrefix, route.urlString, route.creator,
-                   route.CreatedAt))
-
-
 class StaticRouteNotFound(Exception):
-    def __init__(self, message='secret not found'):
-        self.message = message
-        super().__init__(self.message)
+    def __init__(self):
+        super().__init__('static route not found')
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/utils/execute.py` & `rapyuta-io-cli-4.0.0/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/utils/mermaid.py` & `rapyuta-io-cli-4.0.0/riocli/auth/logout.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,43 +7,35 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import click
+from click_help_colors import HelpColorsCommand
 
-import base64
-import json
+from riocli.constants import Colors, Symbols
 
 
-def mermaid_safe(s: str):
-    return s.replace(" ", "_")
+@click.command(
+    'logout',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.pass_context
+def logout(ctx: click.Context):
+    """
+    Log out from the Rapyuta.io account using the CLI.
+    """
+
+    if not ctx.obj.exists:
+        return
+
+    ctx.obj.data.pop('auth_token', None)
+    ctx.obj.data.pop('password', None)
+    ctx.obj.data.pop('email_id', None)
+    ctx.obj.data.pop('project_id', None)
+    ctx.obj.save()
 
-
-def js_string_to_byte(data: str):
-    return bytes(data, 'iso-8859-1')
-
-
-def js_bytes_to_string(data: bytes):
-    return data.decode('iso-8859-1')
-
-
-def js_btoa(data: bytes):
-    return base64.b64encode(data)
-
-
-def mermaid_link(diagram):
-    obj = {
-        "code": diagram,
-        "mermaid": {
-            "theme": "default"
-        },
-        "updateEditor": False,
-        "autoSync": True,
-        "updateDiagram": False
-    }
-    json_str = json.dumps(obj)
-    json_bytes = js_string_to_byte(json_str)
-    encoded_uri = js_btoa(json_bytes)
-    return 'https://mermaid.live/view#base64:{}'.format(
-        js_bytes_to_string(encoded_uri))
+    click.secho('{} Logged out successfully.'.format(Symbols.SUCCESS), fg=Colors.GREEN)
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/utils/selector.py` & `rapyuta-io-cli-4.0.0/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/utils/spinner.py` & `rapyuta-io-cli-4.0.0/riocli/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-4.0.0/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/v2client/client.py` & `rapyuta-io-cli-4.0.0/riocli/v2client/client.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/vpn/__init__.py` & `rapyuta-io-cli-4.0.0/riocli/vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.1.0/riocli/vpn/connect.py` & `rapyuta-io-cli-4.0.0/riocli/vpn/connect.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,96 +13,126 @@
 # limitations under the License.
 
 import getpass
 import time
 from datetime import datetime, timedelta
 
 import click
+from click_help_colors import HelpColorsCommand
 from munch import Munch
+from yaspin.api import Yaspin
 
 from riocli.config import new_v2_client
+from riocli.constants import Colors, Symbols
 from riocli.utils import run_bash_with_return_code
+from riocli.utils.spinner import with_spinner
 from riocli.v2client import Client as v2Client
 from riocli.vpn.util import (
-    is_tailscale_installed,
     is_tailscale_up,
     stop_tailscale,
     install_vpn_tools,
     get_host_name,
     get_host_ip,
     is_vpn_enabled_in_project
 )
 
 
-@click.command('connect')
+@click.command(
+    'connect',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.pass_context
-def connect(ctx: click.Context):
+@with_spinner(text="Connecting...")
+def connect(ctx: click.Context, spinner: Yaspin = None):
     """
     Connect to the current project's VPN network
     """
     try:
-        if not is_tailscale_installed():
-            click.confirm(
-                click.style('VPN tools are not installed. Do you want '
-                            'to install them now?', fg='yellow'),
-                default=True, abort=True)
+        with spinner.hidden():
             install_vpn_tools()
 
         client = new_v2_client()
 
         if not is_vpn_enabled_in_project(
                 client, ctx.obj.data.get('project_id')):
-            click.secho('⚠ VPN is not enabled in the project. '
-                        'Please ask the organization or project '
-                        'creator to enable VPN', fg='yellow')
+            spinner.write(
+                click.style('{} VPN is not enabled in the project. '
+                            'Please ask the organization or project '
+                            'creator to enable VPN'.format(Symbols.WAITING),
+                            fg=Colors.YELLOW))
             raise SystemExit(1)
 
-        if is_tailscale_up():
-            click.confirm('The VPN client is already running. '
-                          'Do you want to stop it and connect to the VPN of '
-                          'the current project?', default=False, abort=True)
-            success = stop_tailscale()
-            if not success:
-                msg = ('❌ Failed to stop tailscale. Please run the following '
-                       'commands manually\n sudo tailscale down\n sudo '
-                       'tailscale logout')
-                click.secho(msg, fg='yellow')
-                raise SystemExit(1)
-
-        click.secho('🛈 VPN is enabled in the project ({})'.format(
-            ctx.obj.data.get('project_name')), fg='cyan')
-
-        if not start_tailscale(ctx, client):
-            click.secho('❌ Failed to connect to the project VPN', fg='red')
+        with spinner.hidden():
+            if is_tailscale_up():
+                click.confirm(
+                    '{} The VPN client is already running. '
+                    'Do you want to stop it and connect to the VPN of '
+                    'the current project?'.format(Symbols.WARNING),
+                    default=False, abort=True)
+                success = stop_tailscale()
+                if not success:
+                    msg = (
+                        '{} Failed to stop tailscale. Please run the '
+                        'following commands manually\n sudo tailscale down\n '
+                        'sudo tailscale logout'.format(Symbols.ERROR))
+                    click.secho(msg, fg=Colors.YELLOW)
+                    raise SystemExit(1)
+
+        spinner.write(
+            click.style(
+                '{} VPN is enabled in the project ({})'.format(
+                    Symbols.INFO, ctx.obj.data.get('project_name')),
+                fg=Colors.CYAN))
+
+        if not start_tailscale(ctx, client, spinner):
+            click.secho('{} Failed to connect to the project VPN'.format(
+                Symbols.ERROR), fg=Colors.RED)
             raise SystemExit(1)
 
-        click.secho('✅ You are now connected to the project\'s VPN',
-                    fg='green')
+        spinner.green.text = 'You are now connected to the project\'s VPN'
+        spinner.green.ok(Symbols.SUCCESS)
+    except click.exceptions.Abort as e:
+        spinner.red.text = 'Aborted!'
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.red.text = str(e)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1) from e
 
 
-def start_tailscale(ctx: click.Context, client: v2Client) -> bool:
+def start_tailscale(
+        ctx: click.Context,
+        client: v2Client,
+        spinner: Yaspin,
+) -> bool:
     cmd = ('sudo tailscale up --auth-key={} --login-server={}'
            ' --reset --force-reauth --accept-routes --accept-dns'
            ' --advertise-tags={} --timeout=30s')
-    args = generate_tailscale_args(ctx, client)
+    args = generate_tailscale_args(ctx, client, spinner)
     command = cmd.format(args.HEADSCALE_PRE_AUTH_KEY,
                          args.HEADSCALE_URL,
                          args.HEADSCALE_ACL_TAG)
     output, code = run_bash_with_return_code(command)
     if code != 0:
-        click.secho('❌ Failed to start vpn client', fg='red')
+        spinner.write(
+            click.style('{} Failed to start vpn client'.format(Symbols.ERROR),
+                        fg=Colors.RED))
         return False
 
     return True
 
 
-def generate_tailscale_args(ctx: click.Context, client: v2Client) -> Munch:
+def generate_tailscale_args(
+        ctx: click.Context,
+        client: v2Client,
+        spinner: Yaspin,
+) -> Munch:
     vpn_instance = 'rio-internal-headscale'
     binding_name = '{}-{}'.format(ctx.obj.machine_id, int(time.time()))
 
     body = {
         'metadata': {
             'name': binding_name,
             'labels': {
@@ -120,22 +150,22 @@
                 'ephemeral': True,
                 'throwaway': True,
                 'expirationTime': get_key_expiry_time(),
             }
         }
     }
 
-    click.secho('⌛ Generating a token to join the network...')
+    spinner.text = 'Generating a token to join the network...'
+
     try:
         # We may end up creating multiple throwaway tokens in the database.
         # But that's okay and something that we can live with
         binding = client.create_instance_binding(vpn_instance, binding=body)
         return binding.spec.environment
     except Exception as e:
-        click.secho(str(e), fg='red')
         raise SystemExit(1) from e
 
 
 def get_key_expiry_time() -> str:
     expiry = datetime.utcnow()
     expiry = expiry + timedelta(minutes=10)
     return expiry.isoformat('T') + 'Z'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/vpn/disconnect.py` & `rapyuta-io-cli-4.0.0/riocli/vpn/ping.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,36 +9,69 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
+from click_help_colors import HelpColorsCommand
+from yaspin.api import Yaspin
 
-from riocli.vpn.util import is_tailscale_installed, install_vpn_tools, \
-    is_tailscale_up, stop_tailscale
-
-
-@click.command('disconnect')
+from riocli.constants import Colors, Symbols
+from riocli.utils.spinner import with_spinner
+from riocli.vpn.util import (
+    install_vpn_tools,
+    is_tailscale_up,
+    get_tailscale_status,
+    tailscale_ping
+)
+
+
+@click.command(
+    'ping-all',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.pass_context
-def disconnect(ctx: click.Context):
+@with_spinner(text="Pinging all peers...")
+def ping_all(ctx: click.Context, spinner: Yaspin = None):
     """
-    Disconnect from the project's VPN network
+    Ping all the peers in the network
     """
     try:
-        if not is_tailscale_installed():
-            click.confirm(
-                click.style('VPN tools are not installed. Do you want '
-                            'to install them now?', fg='yellow'),
-                default=True, abort=True)
+        with spinner.hidden():
             install_vpn_tools()
 
-        if is_tailscale_up() and not stop_tailscale():
-            click.secho('❌ Failed to disconnect from VPN. '
-                        'Although, trying again may work.',
-                        fg='red')
-            raise SystemExit(1)
+        if not is_tailscale_up():
+            spinner.text = click.style(
+                'You are not connected to the VPN', fg=Colors.YELLOW)
+            spinner.yellow.ok(Symbols.WARNING)
+            return
 
-        click.secho("✅ You have been disconnected from the project's VPN", fg='green')
+        ping_all_peers(spinner)
+
+        spinner.text = click.style('Ping complete', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        spinner.text = click.style(str(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1) from e
+
+
+def ping_all_peers(spinner: Yaspin):
+    s = get_tailscale_status()
+
+    peers = s.get('Peer', {})
+
+    for _, v in peers.items():
+        # Do not waste time pinging
+        # offline nodes
+        if not v.get('Online'):
+            continue
+
+        spinner.text = 'Pinging: {}...'.format(
+            click.style(v.get('HostName'), italic=True)
+        )
+        ips = v.get('TailscaleIPs')
+        for ip in ips:
+            tailscale_ping(ip)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/vpn/status.py` & `rapyuta-io-cli-4.0.0/riocli/vpn/status.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,64 +9,71 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
+from click_help_colors import HelpColorsCommand
 
 from riocli.config import new_v2_client
+from riocli.constants import Colors, Symbols
 from riocli.utils import tabulate_data
 from riocli.vpn.util import (
     install_vpn_tools,
-    is_tailscale_installed,
     is_tailscale_up,
     get_tailscale_status,
     is_vpn_enabled_in_project,
 )
 
 
-@click.command('status')
+@click.command(
+    'status',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
 @click.option('--wide', '-w', is_flag=True, default=False,
               help='Print more details', type=bool)
 @click.pass_context
 def status(ctx: click.Context, wide: bool = False):
     """
     Check VPN status
     """
     try:
-        if not is_tailscale_installed():
-            click.confirm(click.style(
-                'VPN tools are not installed. '
-                'Do you want to install them now?',
-                fg='yellow'), default=True, abort=True)
-            install_vpn_tools()
+        install_vpn_tools()
 
         client = new_v2_client()
 
         if not is_vpn_enabled_in_project(
                 client, ctx.obj.data.get('project_id')):
-            click.secho('⚠ VPN is not enabled in the project. '
+            click.secho('{} VPN is not enabled in the project. '
                         'Please ask the organization or project '
-                        'creator to enable VPN', fg='yellow')
+                        'creator to enable VPN'.format(Symbols.WARNING),
+                        fg=Colors.YELLOW)
             raise SystemExit(1)
 
-        click.secho('🛈 VPN is enabled in the project ({})'.format(
-            ctx.obj.data.get('project_name')), fg='cyan')
+        click.secho(
+            '{} VPN is enabled in the project ({})'.format(
+                Symbols.INFO, ctx.obj.data.get('project_name')),
+            fg=Colors.CYAN)
         click.echo()
 
         if not is_tailscale_up():
-            click.secho('You are not connected to the VPN', fg='green')
+            click.secho(
+                '{} You are not connected to the VPN'.format(Symbols.WARNING),
+                fg=Colors.YELLOW)
             return
 
         display_vpn_status(wide)
 
-        click.secho('🛈 You are connected to the VPN.', fg='green')
+        click.secho('{} You are connected to the VPN.'.format(Symbols.INFO),
+                    fg=Colors.GREEN)
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg=Colors.RED)
         raise SystemExit(1) from e
 
 
 def display_vpn_status(wide: bool = False):
     s = get_tailscale_status()
 
     nodes = s.get('Peer', {})
@@ -91,15 +98,15 @@
             row.extend([
                 v.get('Relay'),
                 v.get('Created'),
                 v.get('LastSeen'),
             ])
 
         if k == 'me':
-            row = [click.style(i, fg='bright_blue') for i in row]
+            row = [click.style(i, fg=Colors.BRIGHT_BLUE) for i in row]
 
         data.append(row)
 
     tabulate_data(data, headers)
     click.echo()
     click.secho('DNS Suffix: {}'.format(s.get('MagicDNSSuffix')))
     click.echo()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-3.1.0/riocli/vpn/util.py` & `rapyuta-io-cli-4.0.0/riocli/vpn/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import tempfile
 from os.path import exists, join
 from shutil import move, which
 from sys import platform
 
 import click
 
+from riocli.constants import Colors, Symbols
 from riocli.utils import run_bash, run_bash_with_return_code
 from riocli.v2client import Client as v2Client
 
 
 def get_host_ip() -> str:
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         s.connect(('8.8.8.8', 80))
@@ -69,24 +70,34 @@
 
 def get_tailscale_status() -> dict:
     output, _ = run_bash_with_return_code("tailscale status --json")
     return json.loads(output)
 
 
 def install_vpn_tools() -> None:
+    if is_tailscale_installed():
+        return
+
+    click.confirm(
+        click.style(
+            '{} VPN tools are not installed. Do you want '
+            'to install them now?'.format(Symbols.INFO),
+            fg=Colors.YELLOW),
+        default=True, abort=True)
+
     if not is_linux():
-        click.secho('Only linux is supported', fg='yellow')
+        click.secho('Only linux is supported', fg=Colors.YELLOW)
         raise SystemExit(1)
 
     if is_tailscale_installed():
-        click.secho('VPN tools already installed', fg='green')
+        click.secho('VPN tools already installed', fg=Colors.GREEN)
         return
 
     if not is_curl_installed():
-        click.secho('Please install `curl`', fg='red')
+        click.secho('Please install `curl`', fg=Colors.RED)
         raise SystemExit(1)
 
     # download the tailscale install script
     run_bash('curl -sLO https://tailscale.com/install.sh')
 
     with tempfile.TemporaryDirectory() as tmp_dir:
         script_path = join(tmp_dir, 'install.sh')
@@ -96,17 +107,18 @@
 
         if not exists(script_path):
             raise FileNotFoundError
 
         run_bash('sh {}'.format(script_path))
 
     if not is_tailscale_installed():
-        raise Exception('Failed to install VPN tools')
+        raise Exception('{} Failed to install VPN tools'.format(Symbols.ERROR))
 
-    click.secho('VPN tools installed', fg='green')
+    click.secho('{} VPN tools installed'.format(Symbols.SUCCESS),
+                fg=Colors.GREEN)
 
 
 def tailscale_ping(tailscale_peer_ip):
     cmd = 'tailscale ping --icmp --tsmp --peerapi {}'.format(tailscale_peer_ip)
     return run_bash_with_return_code(cmd)
```

### Comparing `rapyuta-io-cli-3.1.0/setup.py` & `rapyuta-io-cli-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,22 @@
         "dictdiffer>=0.9.0",
         "graphlib-backport>=1.0.3",
         "jinja2>=3.0.1",
         "munch>=2.4.0",
         "python-dateutil>=2.8.2",
         "pytz",
         "pyyaml>=5.4.1",
-        "rapyuta-io>=1.10.0",
+        "rapyuta-io>=1.11.1",
         "requests>=2.20.0",
         "setuptools",
         "six>=1.13.0",
         "tabulate>=0.8.0",
         "urllib3>=1.23",
         "pyrfc3339>=1.1",
         "directory-tree>=0.0.3.1",
         "yaspin>=2.3.0",
         "jsonschema>=4.0.0",
-        "waiting>=1.4.1"
+        "waiting>=1.4.1",
+        "semver>=3.0.0",
     ],
     setup_requires=["flake8"],
 )
```

