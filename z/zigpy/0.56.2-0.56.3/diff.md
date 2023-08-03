# Comparing `tmp/zigpy-0.56.2.tar.gz` & `tmp/zigpy-0.56.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.56.2.tar", last modified: Thu Jul  6 21:30:46 2023, max compression
+gzip compressed data, was "zigpy-0.56.3.tar", last modified: Wed Jul 26 18:25:45 2023, max compression
```

## Comparing `zigpy-0.56.2.tar` & `zigpy-0.56.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.084423 zigpy-0.56.2/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 21:30:35.000000 zigpy-0.56.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-06 21:30:35.000000 zigpy-0.56.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-06 21:30:46.084423 zigpy-0.56.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-06 21:30:35.000000 zigpy-0.56.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-06 21:30:35.000000 zigpy-0.56.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:30:46.084423 zigpy-0.56.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 21:30:35.000000 zigpy-0.56.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.072422 zigpy-0.56.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_app_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_appdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_appdb_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_appdb_pysqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    43780 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    19107 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_quirks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_quirks_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    37037 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zcl_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zcl_foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zdo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zdo_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zigbee_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.076422 zigpy-0.56.2/zigpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45445 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v12.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/zgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/quirks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.084423 zigpy-0.56.2/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.084423 zigpy-0.56.2/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.076422 zigpy-0.56.2/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.335592 zigpy-0.56.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-26 18:25:31.000000 zigpy-0.56.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 18:25:31.000000 zigpy-0.56.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-26 18:25:45.335592 zigpy-0.56.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-26 18:25:31.000000 zigpy-0.56.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-26 18:25:31.000000 zigpy-0.56.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:25:45.335592 zigpy-0.56.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 18:25:31.000000 zigpy-0.56.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.323592 zigpy-0.56.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_app_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_appdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_appdb_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_appdb_pysqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43780 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_ota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_ota_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19107 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_ota_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_ota_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_quirks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_quirks_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37037 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_zcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_zcl_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_zcl_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_zdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_zdo_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-07-26 18:25:31.000000 zigpy-0.56.3/tests/test_zigbee_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.323592 zigpy-0.56.3/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45445 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.327592 zigpy-0.56.3/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.327592 zigpy-0.56.3/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.331592 zigpy-0.56.3/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29669 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/ota/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.331592 zigpy-0.56.3/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/profiles/zgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.331592 zigpy-0.56.3/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/quirks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.331592 zigpy-0.56.3/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.331592 zigpy-0.56.3/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.335592 zigpy-0.56.3/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.335592 zigpy-0.56.3/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-07-26 18:25:31.000000 zigpy-0.56.3/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:25:45.327592 zigpy-0.56.3/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-26 18:25:45.000000 zigpy-0.56.3/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-26 18:25:45.000000 zigpy-0.56.3/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:25:45.000000 zigpy-0.56.3/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-26 18:25:45.000000 zigpy-0.56.3/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 18:25:45.000000 zigpy-0.56.3/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.56.2/COPYING` & `zigpy-0.56.3/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/LICENSE` & `zigpy-0.56.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/PKG-INFO` & `zigpy-0.56.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.56.2
+Version: 0.56.3
 Summary: Library implementing a Zigbee stack
 Author-email: Russell Cloran <rcloran@gmail.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zigpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `zigpy-0.56.2/README.md` & `zigpy-0.56.3/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/pyproject.toml` & `zigpy-0.56.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "coverage[toml]",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-timeout",
     "freezegun",
     "ruff==0.0.261",
-    'pysqlite3-binary; platform_system=="Linux"',
+    'pysqlite3-binary; platform_system=="Linux" and python_version<"3.12"',
 ]
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
```

### Comparing `zigpy-0.56.2/tests/test_app_state.py` & `zigpy-0.56.3/tests/test_app_state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_appdb.py` & `zigpy-0.56.3/tests/test_appdb.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_appdb_migration.py` & `zigpy-0.56.3/tests/test_appdb_migration.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_appdb_pysqlite.py` & `zigpy-0.56.3/tests/test_appdb_pysqlite.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_application.py` & `zigpy-0.56.3/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_backups.py` & `zigpy-0.56.3/tests/test_backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_config.py` & `zigpy-0.56.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_device.py` & `zigpy-0.56.3/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_endpoint.py` & `zigpy-0.56.3/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_group.py` & `zigpy-0.56.3/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_listeners.py` & `zigpy-0.56.3/tests/test_listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_ota.py` & `zigpy-0.56.3/tests/test_ota.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_ota_image.py` & `zigpy-0.56.3/tests/test_ota_image.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_ota_provider.py` & `zigpy-0.56.3/tests/test_ota_provider.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_ota_validators.py` & `zigpy-0.56.3/tests/test_ota_validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_quirks.py` & `zigpy-0.56.3/tests/test_quirks.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_quirks_registry.py` & `zigpy-0.56.3/tests/test_quirks_registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_serial.py` & `zigpy-0.56.3/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_struct.py` & `zigpy-0.56.3/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_topology.py` & `zigpy-0.56.3/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_types.py` & `zigpy-0.56.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_zcl.py` & `zigpy-0.56.3/tests/test_zcl.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_zcl_clusters.py` & `zigpy-0.56.3/tests/test_zcl_clusters.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_zcl_foundation.py` & `zigpy-0.56.3/tests/test_zcl_foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_zdo.py` & `zigpy-0.56.3/tests/test_zdo.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_zdo_types.py` & `zigpy-0.56.3/tests/test_zdo_types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/tests/test_zigbee_util.py` & `zigpy-0.56.3/tests/test_zigbee_util.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb.py` & `zigpy-0.56.3/zigpy/appdb.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v12.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v12.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.56.3/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/application.py` & `zigpy-0.56.3/zigpy/application.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/backups.py` & `zigpy-0.56.3/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/config/__init__.py` & `zigpy-0.56.3/zigpy/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 CONF_OTA_IKEA_URL = "ikea_update_url"
 CONF_OTA_INOVELLI = "inovelli_provider"
 CONF_OTA_LEDVANCE = "ledvance_provider"
 CONF_OTA_SALUS = "salus_provider"
 CONF_OTA_SONOFF = "sonoff_provider"
 CONF_OTA_SONOFF_URL = "sonoff_update_url"
 CONF_OTA_THIRDREALITY = "thirdreality_provider"
+CONF_OTA_REMOTE_PROVIDERS = "remote_providers"
+CONF_OTA_PROVIDER_URL = "url"
+CONF_OTA_PROVIDER_MANUF_IDS = "manufacturer_ids"
 CONF_SOURCE_ROUTING = "source_routing"
 CONF_STARTUP_ENERGY_SCAN = "startup_energy_scan"
 CONF_TOPO_SCAN_PERIOD = "topology_scan_period"
 CONF_TOPO_SCAN_ENABLED = "topology_scan_enabled"
 CONF_TOPO_SKIP_COORDINATOR = "topology_scan_skip_coordinator"
 
 
@@ -101,25 +104,34 @@
             CONF_NWK_TC_LINK_KEY, default=CONF_NWK_TC_LINK_KEY_DEFAULT
         ): cv_key,
         vol.Optional(CONF_NWK_UPDATE_ID, default=CONF_NWK_UPDATE_ID_DEFAULT): vol.All(
             cv_hex, vol.Range(min=0, max=255)
         ),
     }
 )
+
+SCHEMA_OTA_PROVIDER = vol.Schema(
+    {
+        vol.Required(CONF_OTA_PROVIDER_URL): str,
+        vol.Optional(CONF_OTA_PROVIDER_MANUF_IDS, default=[]): [cv_hex],
+    }
+)
+
 SCHEMA_OTA = {
     vol.Optional(CONF_OTA_DIR, default=CONF_OTA_OTAU_DIR_DEFAULT): vol.Any(None, str),
     vol.Optional(CONF_OTA_IKEA, default=CONF_OTA_IKEA_DEFAULT): cv_boolean,
     vol.Optional(CONF_OTA_INOVELLI, default=CONF_OTA_INOVELLI_DEFAULT): cv_boolean,
     vol.Optional(CONF_OTA_LEDVANCE, default=CONF_OTA_LEDVANCE_DEFAULT): cv_boolean,
     vol.Optional(CONF_OTA_SALUS, default=CONF_OTA_SALUS_DEFAULT): cv_boolean,
     vol.Optional(CONF_OTA_SONOFF, default=CONF_OTA_SONOFF_DEFAULT): cv_boolean,
     vol.Optional(CONF_OTA_SONOFF_URL): vol.Url(),
     vol.Optional(
         CONF_OTA_THIRDREALITY, default=CONF_OTA_THIRDREALITY_DEFAULT
     ): cv_boolean,
+    vol.Optional(CONF_OTA_REMOTE_PROVIDERS, default=[]): [SCHEMA_OTA_PROVIDER],
     # Deprecated keys
     vol.Optional(CONF_OTA_IKEA_URL): vol.All(
         cv_deprecated("The `ikea_update_url` key is deprecated and should be removed"),
         vol.Url(),
     ),
 }
```

### Comparing `zigpy-0.56.2/zigpy/config/defaults.py` & `zigpy-0.56.3/zigpy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/config/validators.py` & `zigpy-0.56.3/zigpy/config/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/const.py` & `zigpy-0.56.3/zigpy/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/device.py` & `zigpy-0.56.3/zigpy/device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/endpoint.py` & `zigpy-0.56.3/zigpy/endpoint.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/exceptions.py` & `zigpy-0.56.3/zigpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/group.py` & `zigpy-0.56.3/zigpy/group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/listeners.py` & `zigpy-0.56.3/zigpy/listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/ota/__init__.py` & `zigpy-0.56.3/zigpy/ota/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 from zigpy.config import (
     CONF_OTA,
     CONF_OTA_DIR,
     CONF_OTA_IKEA,
     CONF_OTA_INOVELLI,
     CONF_OTA_LEDVANCE,
+    CONF_OTA_PROVIDER_MANUF_IDS,
+    CONF_OTA_PROVIDER_URL,
+    CONF_OTA_REMOTE_PROVIDERS,
     CONF_OTA_SALUS,
     CONF_OTA_SONOFF,
     CONF_OTA_THIRDREALITY,
 )
 from zigpy.ota.image import BaseOTAImage, ImageKey, OTAImageHeader
 import zigpy.ota.provider
 from zigpy.ota.validators import check_invalid
@@ -125,14 +128,22 @@
         if ota_config[CONF_OTA_SALUS]:
             self.add_listener(zigpy.ota.provider.Salus())
         if ota_config[CONF_OTA_SONOFF]:
             self.add_listener(zigpy.ota.provider.Sonoff())
         if ota_config[CONF_OTA_THIRDREALITY]:
             self.add_listener(zigpy.ota.provider.ThirdReality())
 
+        for provider_config in ota_config[CONF_OTA_REMOTE_PROVIDERS]:
+            self.add_listener(
+                zigpy.ota.provider.RemoteProvider(
+                    url=provider_config[CONF_OTA_PROVIDER_URL],
+                    manufacturer_ids=provider_config[CONF_OTA_PROVIDER_MANUF_IDS],
+                )
+            )
+
     async def initialize(self) -> None:
         await self.async_event("initialize_provider", self._app.config[CONF_OTA])
         self._not_initialized = False
 
     async def get_ota_image(
         self,
         manufacturer_id: t.uint16_t,
```

### Comparing `zigpy-0.56.2/zigpy/ota/image.py` & `zigpy-0.56.3/zigpy/ota/image.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/ota/provider.py` & `zigpy-0.56.3/zigpy/ota/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """OTA Firmware providers."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 import asyncio
 from collections import defaultdict
 import datetime
+import hashlib
 import io
 import logging
 import os
 import os.path
 import tarfile
 import typing
 import urllib.parse
@@ -792,7 +793,111 @@
             img = ThirdRealityImage.from_json(firmware)
             self._cache[img.key] = img
 
         self.update_expiration()
 
     async def filter_get_image(self, key: ImageKey) -> bool:
         return key.manufacturer_id not in self.MANUFACTURER_IDS
+
+
+@attr.s
+class RemoteImage:
+    binary_url = attr.ib()
+    file_version = attr.ib()
+    image_type = attr.ib()
+    manufacturer_id = attr.ib()
+    changelog = attr.ib()
+    checksum = attr.ib()
+
+    # Optional
+    min_hardware_version = attr.ib()
+    max_hardware_version = attr.ib()
+    min_current_file_version = attr.ib()
+    max_current_file_version = attr.ib()
+
+    @classmethod
+    def from_json(cls, obj: dict[str, typing.Any]) -> RemoteImage:
+        return cls(
+            binary_url=obj["binary_url"],
+            file_version=obj["file_version"],
+            image_type=obj["image_type"],
+            manufacturer_id=obj["manufacturer_id"],
+            changelog=obj["changelog"],
+            checksum=obj["checksum"],
+            min_hardware_version=obj.get("min_hardware_version"),
+            max_hardware_version=obj.get("max_hardware_version"),
+            min_current_file_version=obj.get("min_current_file_version"),
+            max_current_file_version=obj.get("max_current_file_version"),
+        )
+
+    @property
+    def key(self) -> ImageKey:
+        return ImageKey(self.manufacturer_id, self.image_type)
+
+    async def fetch_image(self) -> BaseOTAImage:
+        async with aiohttp.ClientSession() as req:
+            LOGGER.debug("Downloading %s for %s", self.binary_url, self.key)
+            async with req.get(self.binary_url) as rsp:
+                data = await rsp.read()
+
+        algorithm, checksum = self.checksum.split(":")
+        hasher = hashlib.new(algorithm)
+        await asyncio.get_running_loop().run_in_executor(None, hasher.update, data)
+
+        if hasher.hexdigest() != checksum:
+            raise ValueError(
+                f"Image checksum is invalid: expected {self.checksum},"
+                f" got {hasher.hexdigest()}"
+            )
+
+        ota_image, _ = parse_ota_image(data)
+
+        LOGGER.debug("Finished downloading %s", self)
+        return ota_image
+
+
+class RemoteProvider(Basic):
+    """Generic zigpy OTA URL provider."""
+
+    HEADERS = {"accept": "application/json"}
+
+    def __init__(self, url: str, manufacturer_ids: list[int] | None) -> None:
+        super().__init__()
+
+        self.url = url
+        self.manufacturer_ids = manufacturer_ids
+
+    async def initialize_provider(self, ota_config: dict) -> None:
+        self.info("OTA provider enabled")
+        await self.refresh_firmware_list()
+        self.enable()
+
+    async def refresh_firmware_list(self) -> None:
+        if self._locks[LOCK_REFRESH].locked():
+            return
+
+        async with self._locks[LOCK_REFRESH]:
+            async with aiohttp.ClientSession(headers=self.HEADERS) as req:
+                async with req.get(self.url) as rsp:
+                    if not (200 <= rsp.status <= 299):
+                        self.warning(
+                            "Couldn't download '%s': %s/%s",
+                            rsp.url,
+                            rsp.status,
+                            rsp.reason,
+                        )
+                        return
+                    fw_lst = await rsp.json()
+
+        self.debug("Finished downloading firmware update list")
+        self._cache.clear()
+        for obj in fw_lst:
+            img = RemoteImage.from_json(obj)
+            self._cache[img.key] = img
+
+        self.update_expiration()
+
+    async def filter_get_image(self, key: ImageKey) -> bool:
+        if not self.manufacturer_ids:
+            return False
+
+        return key.manufacturer_id not in self.manufacturer_ids
```

### Comparing `zigpy-0.56.2/zigpy/ota/validators.py` & `zigpy-0.56.3/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/profiles/zgp.py` & `zigpy-0.56.3/zigpy/profiles/zgp.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/profiles/zha.py` & `zigpy-0.56.3/zigpy/profiles/zha.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/profiles/zll.py` & `zigpy-0.56.3/zigpy/profiles/zll.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/quirks/__init__.py` & `zigpy-0.56.3/zigpy/quirks/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/quirks/registry.py` & `zigpy-0.56.3/zigpy/quirks/registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/serial.py` & `zigpy-0.56.3/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/state.py` & `zigpy-0.56.3/zigpy/state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/topology.py` & `zigpy-0.56.3/zigpy/topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/types/basic.py` & `zigpy-0.56.3/zigpy/types/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,18 +141,21 @@
             raise ValueError(f"Invalid repr value {repr!r}. Must be either hex or bin")
 
         if byteorder is not NOT_SET:
             cls._byteorder = byteorder
         elif cls._byteorder is None:
             cls._byteorder = "little"
 
-        # XXX: The enum module uses the first class with __new__ in its __dict__ as the
-        #      member type. We have to ensure this is true for every subclass.
-        if "__new__" not in cls.__dict__:
-            cls.__new__ = cls.__new__
+        if sys.version_info < (3, 10):
+            # XXX: The enum module uses the first class with __new__ in its __dict__
+            #      as the member type. We have to ensure this is true for
+            #      every subclass.
+            # Fixed with https://github.com/python/cpython/pull/26658
+            if "__new__" not in cls.__dict__:
+                cls.__new__ = cls.__new__
 
         # XXX: The enum module sabotages pickling using the same logic.
         if "__reduce_ex__" not in cls.__dict__:
             cls.__reduce_ex__ = cls.__reduce_ex__
 
     def bits(self) -> Bits:
         return Bits([(self >> n) & 0b1 for n in range(self._bits - 1, -1, -1)])
@@ -354,15 +357,22 @@
     pass
 
 
 class uint64_t_be(uint_t_be, bits=64):
     pass
 
 
-class _IntEnumMeta(enum.EnumMeta):
+class AlwaysCreateEnumType(enum.EnumMeta):
+    """Enum metaclass that skips the functional creation API."""
+
+    def __call__(cls, value, names=None, *values) -> type[enum.Enum]:  # type: ignore
+        return cls.__new__(cls, value)  # type: ignore
+
+
+class _IntEnumMeta(AlwaysCreateEnumType):
     def __call__(cls, value, names=None, *args, **kwargs):
         if isinstance(value, str):
             if value.startswith("0x"):
                 value = int(value, base=16)
             elif value.isnumeric():
                 value = int(value)
             elif value.startswith(cls.__name__ + "."):
@@ -375,15 +385,21 @@
 def bitmap_factory(int_type: CALLABLE_T) -> CALLABLE_T:
     """Mixins are broken by Python 3.8.6 so we must dynamically create the enum with the
     appropriate methods but with only one non-Enum parent class.
     """
 
     if sys.version_info >= (3, 11):
 
-        class _NewEnum(int_type, enum.ReprEnum, enum.Flag, boundary=enum.KEEP):
+        class _NewEnum(
+            int_type,
+            enum.ReprEnum,
+            enum.Flag,
+            boundary=enum.KEEP,
+            metaclass=AlwaysCreateEnumType,
+        ):
             pass
 
     else:
 
         class _NewEnum(int_type, enum.Flag):
             # Rebind classmethods to our own class
             _missing_ = classmethod(enum.IntFlag._missing_.__func__)
```

### Comparing `zigpy-0.56.2/zigpy/types/named.py` & `zigpy-0.56.3/zigpy/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/types/struct.py` & `zigpy-0.56.3/zigpy/types/struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/typing.py` & `zigpy-0.56.3/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/util.py` & `zigpy-0.56.3/zigpy/util.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/__init__.py` & `zigpy-0.56.3/zigpy/zcl/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/__init__.py` & `zigpy-0.56.3/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/closures.py` & `zigpy-0.56.3/zigpy/zcl/clusters/closures.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/general.py` & `zigpy-0.56.3/zigpy/zcl/clusters/general.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/homeautomation.py` & `zigpy-0.56.3/zigpy/zcl/clusters/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/hvac.py` & `zigpy-0.56.3/zigpy/zcl/clusters/hvac.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/lighting.py` & `zigpy-0.56.3/zigpy/zcl/clusters/lighting.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.56.3/zigpy/zcl/clusters/lightlink.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/measurement.py` & `zigpy-0.56.3/zigpy/zcl/clusters/measurement.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/protocol.py` & `zigpy-0.56.3/zigpy/zcl/clusters/protocol.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/security.py` & `zigpy-0.56.3/zigpy/zcl/clusters/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.56.3/zigpy/zcl/clusters/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zcl/foundation.py` & `zigpy-0.56.3/zigpy/zcl/foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zdo/__init__.py` & `zigpy-0.56.3/zigpy/zdo/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy/zdo/types.py` & `zigpy-0.56.3/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.2/zigpy.egg-info/PKG-INFO` & `zigpy-0.56.3/zigpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.56.2
+Version: 0.56.3
 Summary: Library implementing a Zigbee stack
 Author-email: Russell Cloran <rcloran@gmail.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zigpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `zigpy-0.56.2/zigpy.egg-info/SOURCES.txt` & `zigpy-0.56.3/zigpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

