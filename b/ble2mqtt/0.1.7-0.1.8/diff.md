# Comparing `tmp/ble2mqtt-0.1.7.tar.gz` & `tmp/ble2mqtt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ble2mqtt-0.1.7.tar", last modified: Tue May 30 10:18:21 2023, max compression
+gzip compressed data, was "ble2mqtt-0.1.8.tar", last modified: Thu Aug  3 18:14:55 2023, max compression
```

## Comparing `ble2mqtt-0.1.7.tar` & `ble2mqtt-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.165963 ble2mqtt-0.1.7/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1086 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/LICENSE
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/MANIFEST.in
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-30 10:18:21.166038 ble2mqtt-0.1.7/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9346 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/README.md
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.161230 ble2mqtt-0.1.7/ble2mqtt/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4599 2023-05-21 11:18:54.000000 ble2mqtt-0.1.7/ble2mqtt/__main__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       18 2023-05-30 10:16:34.000000 ble2mqtt-0.1.7/ble2mqtt/__version__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    39910 2023-05-30 10:17:41.000000 ble2mqtt-0.1.7/ble2mqtt/ble2mqtt.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      574 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/compat.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.164582 ble2mqtt-0.1.7/ble2mqtt/devices/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      911 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1901 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/atom_fast.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    27177 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/base.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4834 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/bulb_avea.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11419 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/cooker_redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4603 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/cover_am43.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7158 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/cover_soma.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11248 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/kettle_redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6571 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/kettle_xiaomi.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2579 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/presence.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1526 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/qingping_cgdk2.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7154 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/thermostat_ensto.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      349 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/uuids.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1571 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/voltage_bm2.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3438 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/vson_air_wp6003.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1434 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_base.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2568 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_ht.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1076 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2273 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03_atc.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.165832 ble2mqtt-0.1.7/ble2mqtt/protocols/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4624 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/am43.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5266 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/avea.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3819 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/base.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6596 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/ensto.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    16297 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6441 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/soma.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2618 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/wp6003.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10322 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/xiaomi.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1692 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/utils.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.162031 ble2mqtt-0.1.7/ble2mqtt.egg-info/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1232 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       52 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/requires.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/top_level.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       99 2023-05-30 10:18:21.166316 ble2mqtt-0.1.7/setup.cfg
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1089 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/setup.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-08-03 18:14:55.576295 ble2mqtt-0.1.8/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1086 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/LICENSE
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/MANIFEST.in
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10291 2023-08-03 18:14:55.576419 ble2mqtt-0.1.8/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9727 2023-08-03 18:08:57.000000 ble2mqtt-0.1.8/README.md
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-08-03 18:14:55.568721 ble2mqtt-0.1.8/ble2mqtt/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5458 2023-08-03 18:11:36.000000 ble2mqtt-0.1.8/ble2mqtt/__main__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       18 2023-08-03 18:13:34.000000 ble2mqtt-0.1.8/ble2mqtt/__version__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    40174 2023-08-03 18:08:57.000000 ble2mqtt-0.1.8/ble2mqtt/ble2mqtt.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      574 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/compat.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-08-03 18:14:55.574469 ble2mqtt-0.1.8/ble2mqtt/devices/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      972 2023-08-03 18:08:57.000000 ble2mqtt-0.1.8/ble2mqtt/devices/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1901 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/atom_fast.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    27485 2023-08-03 18:11:24.000000 ble2mqtt-0.1.8/ble2mqtt/devices/base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4834 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/bulb_avea.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11419 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/cooker_redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4603 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/cover_am43.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7158 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/cover_soma.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2945 2023-08-03 18:10:55.000000 ble2mqtt-0.1.8/ble2mqtt/devices/flower_mclh09.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11248 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/kettle_redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6571 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/kettle_xiaomi.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2579 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/presence.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1526 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/qingping_cgdk2.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7154 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/thermostat_ensto.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      349 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/uuids.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1579 2023-08-03 18:11:52.000000 ble2mqtt-0.1.8/ble2mqtt/devices/voltage_bm2.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3438 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/vson_air_wp6003.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1434 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2568 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_ht.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1076 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_lywsd03.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2273 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_lywsd03_atc.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-08-03 18:14:55.576120 ble2mqtt-0.1.8/ble2mqtt/protocols/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4624 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/am43.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5266 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/avea.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3819 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6596 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/ensto.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    16297 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6441 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/soma.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2618 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/wp6003.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10322 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/ble2mqtt/protocols/xiaomi.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1692 2023-05-13 11:58:13.000000 ble2mqtt-0.1.8/ble2mqtt/utils.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-08-03 18:14:55.569646 ble2mqtt-0.1.8/ble2mqtt.egg-info/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10291 2023-08-03 18:14:55.000000 ble2mqtt-0.1.8/ble2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1266 2023-08-03 18:14:55.000000 ble2mqtt-0.1.8/ble2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-08-03 18:14:55.000000 ble2mqtt-0.1.8/ble2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       52 2023-08-03 18:14:55.000000 ble2mqtt-0.1.8/ble2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-08-03 18:14:55.000000 ble2mqtt-0.1.8/ble2mqtt.egg-info/requires.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-08-03 18:14:55.000000 ble2mqtt-0.1.8/ble2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       99 2023-08-03 18:14:55.576767 ble2mqtt-0.1.8/setup.cfg
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1089 2023-06-04 19:58:07.000000 ble2mqtt-0.1.8/setup.py
```

### Comparing `ble2mqtt-0.1.7/LICENSE` & `ble2mqtt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/PKG-INFO` & `ble2mqtt-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: ble2mqtt
-Version: 0.1.7
-Summary: BLE to MQTT bridge
-Home-page: https://github.com/devbis/ble2mqtt/
-Author: Ivan Belokobylskiy
-Author-email: belokobylskij@gmail.com
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
-
 # BLE2MQTT
 ### Control your Bluetooth devices with smart home
 
 ![ble2mqtt devices](./ble2mqtt.png)
 
 ## Supported devices:
 
@@ -88,14 +71,20 @@
   use this feature in the official app while ble2mqtt is working.
 
 ### Battery voltage meters
 
 - **BM2 car battery voltage meter (type: voltage_bm2)**
 
 
+### Plant sensors:
+
+- **LifeControl MCLH-09 (type: mclh09)**
+
+  optionally, reconnection interval can be configured with `interval` parameter in seconds
+
 By default, a device works in the passive mode without connection by 
 listening to advertisement packets from a device.
 To use connection to the device provide `"passive": false` parameter.
 
 **Supported devices in passive mode:**
 - Xiaomi MJ_HT_V1 (xiaomihtv1)
 - Xiaomi LYWSD03MMC with custom ATC firmware (xiaomilywsd_atc)
@@ -133,14 +122,18 @@
 ```
 [CHG] Device 90:FD:00:00:00:01 Paired: yes
 Pairing successful
 ```
 You can proceed with the next configuration steps now.
 
 
+## Selinux issues
+
+If using SELinux and you are experience issues, see [README.md](selinux/README.md).
+
 ### Known issues:
 - *High cpu usage due to underlying library to work with bluetooth*
 
 **Use this software at your own risk.**
 
 ## Configuration
 
@@ -212,14 +205,19 @@
         {
             "address": "11:22:33:aa:aa:aa",
             "type": "atomfast"
         },
         {
             "address": "11:22:33:aa:aa:bb",
             "type": "voltage_bm2"
+        },
+        {
+            "address": "11:22:33:aa:aa:bv",
+            "type": "mclh09",
+            "interval": 600
         }
     ]
 }
 ```
 
 You can omit a line, then default value will be used.
```

### Comparing `ble2mqtt-0.1.7/README.md` & `ble2mqtt-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: ble2mqtt
+Version: 0.1.8
+Summary: BLE to MQTT bridge
+Home-page: https://github.com/devbis/ble2mqtt/
+Author: Ivan Belokobylskiy
+Author-email: belokobylskij@gmail.com
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+Provides-Extra: full
+License-File: LICENSE
+
 # BLE2MQTT
 ### Control your Bluetooth devices with smart home
 
 ![ble2mqtt devices](./ble2mqtt.png)
 
 ## Supported devices:
 
@@ -71,14 +88,20 @@
   use this feature in the official app while ble2mqtt is working.
 
 ### Battery voltage meters
 
 - **BM2 car battery voltage meter (type: voltage_bm2)**
 
 
+### Plant sensors:
+
+- **LifeControl MCLH-09 (type: mclh09)**
+
+  optionally, reconnection interval can be configured with `interval` parameter in seconds
+
 By default, a device works in the passive mode without connection by 
 listening to advertisement packets from a device.
 To use connection to the device provide `"passive": false` parameter.
 
 **Supported devices in passive mode:**
 - Xiaomi MJ_HT_V1 (xiaomihtv1)
 - Xiaomi LYWSD03MMC with custom ATC firmware (xiaomilywsd_atc)
@@ -116,14 +139,18 @@
 ```
 [CHG] Device 90:FD:00:00:00:01 Paired: yes
 Pairing successful
 ```
 You can proceed with the next configuration steps now.
 
 
+## Selinux issues
+
+If using SELinux and you are experience issues, see [README.md](selinux/README.md).
+
 ### Known issues:
 - *High cpu usage due to underlying library to work with bluetooth*
 
 **Use this software at your own risk.**
 
 ## Configuration
 
@@ -195,14 +222,19 @@
         {
             "address": "11:22:33:aa:aa:aa",
             "type": "atomfast"
         },
         {
             "address": "11:22:33:aa:aa:bb",
             "type": "voltage_bm2"
+        },
+        {
+            "address": "11:22:33:aa:aa:bv",
+            "type": "mclh09",
+            "interval": 600
         }
     ]
 }
 ```
 
 You can omit a line, then default value will be used.
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt/__main__.py` & `ble2mqtt-0.1.8/ble2mqtt/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,24 +67,50 @@
         _LOGGER.info("Ignore this exception.")
         return
 
     _LOGGER.info("Shutting down...")
     aio.create_task(shutdown(loop, service))
 
 
+def get_ssl_context(config):
+    if config.get('mqtt_tls') != "True":
+        return None
+    import ssl
+    ca_cert = config.get('mqtt_ca')
+    client_cert = config.get('mqtt_cert')
+    client_keyfile = config.get('mqtt_key')
+    client_keyfile_password = config.get('mqtt_key_password')
+    ca_verify = config.get('mqtt_ca_verify') != "False"
+    context = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
+    if ca_cert is not None:
+        context.load_verify_locations(ca_cert)
+    else:
+        context.load_default_certs()
+    context.check_hostname = ca_verify
+    context.verify_mode = ssl.CERT_REQUIRED if ca_verify else ssl.CERT_NONE
+    if client_keyfile is not None:
+        context.load_cert_chain(
+            client_cert,
+            client_keyfile,
+            client_keyfile_password,
+        )
+    return context
+
+
 async def amain(config):
     loop = aio.get_running_loop()
 
     service = Ble2Mqtt(
         reconnection_interval=10,
         loop=loop,
         host=config['mqtt_host'],
         port=config['mqtt_port'],
         user=config.get('mqtt_user'),
         password=config.get('mqtt_password'),
+        ssl=get_ssl_context(config),
         base_topic=config['base_topic'],
         mqtt_config_prefix=config['mqtt_config_prefix'],
         hci_adapter=config['hci_adapter'],
     )
 
     loop.set_exception_handler(
         lambda *args: handle_exception(*args, service=service),
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt/ble2mqtt.py` & `ble2mqtt-0.1.8/ble2mqtt/ble2mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -666,15 +666,15 @@
                 # the bluetooth chip
                 if missing_device_count >= device.CONNECTION_FAILURES_LIMIT:
                     _LOGGER.error(
                         f'Device {device} was not found for '
                         f'{missing_device_count} times. Restarting bluetooth.',
                     )
                     missing_device_count = 0
-                    await restart_bluetooth()
+                    await restart_bluetooth(self._hci_adapter)
             finally:
                 if self.device.ACTIVE_CONNECTION_MODE not in (
                     ConnectionMode.ACTIVE_POLL_WITH_DISCONNECT,
                     ConnectionMode.ON_DEMAND_CONNECTION,
                 ):
                     try:
                         await aio.wait_for(
@@ -702,15 +702,15 @@
                             pass
                 except aio.CancelledError:
                     raise
                 except Exception:
                     pass
 
             if failure_count >= FAILURE_LIMIT:
-                await restart_bluetooth()
+                await restart_bluetooth(self._hci_adapter)
                 failure_count = 0
             try:
                 if not device.disconnected_event.is_set():
                     await aio.wait_for(
                         device.disconnected_event.wait(),
                         timeout=10,
                     )
@@ -721,14 +721,15 @@
 
 class Ble2Mqtt:
     TOPIC_ROOT = 'ble2mqtt'
     BRIDGE_TOPIC = 'bridge'
 
     def __init__(
             self,
+            ssl,
             host: str,
             port: int = None,
             user: ty.Optional[str] = None,
             password: ty.Optional[str] = None,
             reconnection_interval: int = 10,
             loop: ty.Optional[aio.AbstractEventLoop] = None,
             *,
@@ -739,14 +740,15 @@
         global BLUETOOTH_RESTARTING
 
         self._hci_adapter = hci_adapter
         self._mqtt_host = host
         self._mqtt_port = port
         self._mqtt_user = user
         self._mqtt_password = password
+        self._ssl = ssl
         self._base_topic = base_topic
         self._mqtt_config_prefix = mqtt_config_prefix
 
         self._reconnection_interval = reconnection_interval
         self._loop = loop or aio.get_event_loop()
         BLUETOOTH_RESTARTING = aio.Lock()
 
@@ -860,17 +862,21 @@
             except Exception:
                 _LOGGER.exception(
                     f'Problem on closing dev manager {manager.device}')
 
     def device_detection_callback(self, device: BLEDevice, advertisement_data):
         for reg_device in self.device_registry:
             if reg_device.mac.lower() == device.address.lower():
-                if device.rssi:
+                if hasattr(advertisement_data, 'rssi'):
+                    rssi = advertisement_data.rssi
+                else:
+                    rssi = device.rssi
+                if rssi:
                     # update rssi for all devices if available
-                    reg_device.rssi = device.rssi
+                    reg_device.rssi = rssi
                 if reg_device.is_passive:
                     if device.name:
                         reg_device._model = device.name
                     reg_device.handle_advert(device, advertisement_data)
                 else:
                     _LOGGER.debug(
                         f'active device seen: {reg_device} '
@@ -968,14 +974,15 @@
         while True:
             try:
                 mqtt_connection = await aio.wait_for(self._mqtt_client.connect(
                     host=self._mqtt_host,
                     port=self._mqtt_port,
                     username=self._mqtt_user,
                     password=self._mqtt_password,
+                    ssl=self._ssl,
                     client_id=f'ble2mqtt_{dev_id}',
                     will_message=aio_mqtt.PublishableMessage(
                         topic_name=self.availability_topic,
                         payload='offline',
                         qos=aio_mqtt.QOSLevel.QOS_1,
                         retain=True,
                     ),
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt/compat.py` & `ble2mqtt-0.1.8/ble2mqtt/compat.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/__init__.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .atom_fast import AtomFast  # noqa: F401
 from .base import registered_device_types  # noqa: F401
 from .bulb_avea import AveaBulb  # noqa: F401
 from .cooker_redmond import RedmondCooker  # noqa: F401
 from .cover_am43 import AM43Cover  # noqa: F401
 from .cover_soma import SomaCover  # noqa: F401
+from .flower_mclh09 import FlowerMonitorMCLH09  # noqa: F401
 from .kettle_redmond import RedmondKettle  # noqa: F401
 from .kettle_xiaomi import XiaomiKettle  # noqa: F401
 from .presence import Presence  # noqa: F401
 from .qingping_cgdk2 import QingpingTempRHMonitorLite  # noqa: F401
 from .thermostat_ensto import EnstoThermostat  # noqa: F401
 from .voltage_bm2 import VoltageTesterBM2  # noqa: F401
 from .vson_air_wp6003 import VsonWP6003  # noqa: F401
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/atom_fast.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/atom_fast.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/base.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,14 @@
         raise NotImplementedError()
 
     def handle_advert(self, scanned_device: BLEDevice, adv_data):
         raise NotImplementedError()
 
 
 class Device(BaseDevice, abc.ABC):
-    MQTT_VALUES = None
     SET_POSTFIX: str = 'set'
     SET_POSITION_POSTFIX: str = 'set_position'  # for covers. Consider rework
     SET_MODE_POSTFIX: str = 'set_mode'  # for climate
     SET_TARGET_TEMPERATURE_POSTFIX: str = 'set_temperature'  # for climate
     MAC_TYPE: str = 'public'
     MANUFACTURER: str = None  # type: ignore
     CONNECTION_FAILURES_LIMIT = 100
@@ -530,14 +529,23 @@
         while True:
             await self.update_device_data(send_config)
             if not self.READ_DATA_IN_ACTIVE_LOOP and not self._state:
                 await aio.sleep(self.NOT_READY_SLEEP_INTERVAL)
                 continue
 
             await self.do_active_loop(publish_topic)
+            if (
+                self.ACTIVE_CONNECTION_MODE ==
+                ConnectionMode.ACTIVE_POLL_WITH_DISCONNECT
+            ):
+                if self.client.is_connected:
+                    await self.client.disconnect()
+                # let DeviceManager.manage_device() handle reconnections
+                return
+
             await aio.sleep(self.ACTIVE_SLEEP_INTERVAL)
 
     async def handle_passive(self, publish_topic, send_config, *args, **kwargs):
         while True:
             if not self._state:
                 await aio.sleep(self.NOT_READY_SLEEP_INTERVAL)
                 continue
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/bulb_avea.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/bulb_avea.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/cooker_redmond.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/cooker_redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/cover_am43.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/cover_am43.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/cover_soma.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/cover_soma.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/kettle_redmond.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/kettle_redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/kettle_xiaomi.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/kettle_xiaomi.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/presence.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/presence.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/qingping_cgdk2.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/qingping_cgdk2.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/thermostat_ensto.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/thermostat_ensto.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/voltage_bm2.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/voltage_bm2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 
-from ..devices.base import SENSOR_DOMAIN, Sensor, SubscribeAndSetDataMixin, ConnectionMode
+from ..devices.base import (
+    SENSOR_DOMAIN, Sensor, SubscribeAndSetDataMixin, ConnectionMode
+)
 
 UUID_KEY_READ = "0000fff4-0000-1000-8000-00805f9b34fb"
 KEY = b"\x6c\x65\x61\x67\x65\x6e\x64\xff\xfe\x31\x38\x38\x32\x34\x36\x36"
 
 
 def create_aes():
     try:
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/vson_air_wp6003.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/vson_air_wp6003.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_base.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_ht.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_ht.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_lywsd03.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03_atc.py` & `ble2mqtt-0.1.8/ble2mqtt/devices/xiaomi_lywsd03_atc.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/am43.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/am43.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/avea.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/avea.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/base.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/ensto.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/ensto.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/redmond.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/soma.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/soma.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/wp6003.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/wp6003.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/protocols/xiaomi.py` & `ble2mqtt-0.1.8/ble2mqtt/protocols/xiaomi.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt/utils.py` & `ble2mqtt-0.1.8/ble2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.7/ble2mqtt.egg-info/PKG-INFO` & `ble2mqtt-0.1.8/ble2mqtt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ble2mqtt
-Version: 0.1.7
+Version: 0.1.8
 Summary: BLE to MQTT bridge
 Home-page: https://github.com/devbis/ble2mqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -88,14 +88,20 @@
   use this feature in the official app while ble2mqtt is working.
 
 ### Battery voltage meters
 
 - **BM2 car battery voltage meter (type: voltage_bm2)**
 
 
+### Plant sensors:
+
+- **LifeControl MCLH-09 (type: mclh09)**
+
+  optionally, reconnection interval can be configured with `interval` parameter in seconds
+
 By default, a device works in the passive mode without connection by 
 listening to advertisement packets from a device.
 To use connection to the device provide `"passive": false` parameter.
 
 **Supported devices in passive mode:**
 - Xiaomi MJ_HT_V1 (xiaomihtv1)
 - Xiaomi LYWSD03MMC with custom ATC firmware (xiaomilywsd_atc)
@@ -133,14 +139,18 @@
 ```
 [CHG] Device 90:FD:00:00:00:01 Paired: yes
 Pairing successful
 ```
 You can proceed with the next configuration steps now.
 
 
+## Selinux issues
+
+If using SELinux and you are experience issues, see [README.md](selinux/README.md).
+
 ### Known issues:
 - *High cpu usage due to underlying library to work with bluetooth*
 
 **Use this software at your own risk.**
 
 ## Configuration
 
@@ -212,14 +222,19 @@
         {
             "address": "11:22:33:aa:aa:aa",
             "type": "atomfast"
         },
         {
             "address": "11:22:33:aa:aa:bb",
             "type": "voltage_bm2"
+        },
+        {
+            "address": "11:22:33:aa:aa:bv",
+            "type": "mclh09",
+            "interval": 600
         }
     ]
 }
 ```
 
 You can omit a line, then default value will be used.
```

### Comparing `ble2mqtt-0.1.7/ble2mqtt.egg-info/SOURCES.txt` & `ble2mqtt-0.1.8/ble2mqtt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ble2mqtt/devices/__init__.py
 ble2mqtt/devices/atom_fast.py
 ble2mqtt/devices/base.py
 ble2mqtt/devices/bulb_avea.py
 ble2mqtt/devices/cooker_redmond.py
 ble2mqtt/devices/cover_am43.py
 ble2mqtt/devices/cover_soma.py
+ble2mqtt/devices/flower_mclh09.py
 ble2mqtt/devices/kettle_redmond.py
 ble2mqtt/devices/kettle_xiaomi.py
 ble2mqtt/devices/presence.py
 ble2mqtt/devices/qingping_cgdk2.py
 ble2mqtt/devices/thermostat_ensto.py
 ble2mqtt/devices/uuids.py
 ble2mqtt/devices/voltage_bm2.py
```

### Comparing `ble2mqtt-0.1.7/setup.py` & `ble2mqtt-0.1.8/setup.py`

 * *Files identical despite different names*

