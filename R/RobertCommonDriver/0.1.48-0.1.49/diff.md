# Comparing `tmp/RobertCommonDriver-0.1.48.tar.gz` & `tmp/RobertCommonDriver-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.48.tar", last modified: Wed Aug  2 02:37:18 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.49.tar", last modified: Thu Aug  3 05:41:08 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.48.tar` & `RobertCommonDriver-0.1.49.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.830673 RobertCommonDriver-0.1.48/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.48/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.48/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2023-08-02 02:37:18.829437 RobertCommonDriver-0.1.48/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.48/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.763157 RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2023-08-02 02:37:18.000000 RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-08-02 02:37:18.000000 RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 02:37:18.000000 RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2023-08-02 02:37:18.000000 RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 02:37:18.000000 RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2023-07-29 08:14:49.000000 RobertCommonDriver-0.1.48/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.764154 RobertCommonDriver-0.1.48/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.48/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.765356 RobertCommonDriver-0.1.48/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.777361 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33507 2023-08-02 02:36:46.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.794685 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    69640 2023-07-28 15:24:15.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0   101229 2023-07-27 06:16:09.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    78958 2023-08-02 02:31:15.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    34947 2023-07-31 04:04:12.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    45078 2023-07-31 03:14:23.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-08-02 02:37:18.830673 RobertCommonDriver-0.1.48/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-08-02 02:37:09.000000 RobertCommonDriver-0.1.48/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.795685 RobertCommonDriver-0.1.48/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.48/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.796686 RobertCommonDriver-0.1.48/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.48/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.808985 RobertCommonDriver-0.1.48/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:37:18.828437 RobertCommonDriver-0.1.48/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     4147 2023-07-27 06:18:04.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9674 2023-07-31 03:26:47.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4145 2023-07-27 06:41:53.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.222014 RobertCommonDriver-0.1.49/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.49/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.49/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-08-03 05:41:08.221013 RobertCommonDriver-0.1.49/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.49/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.122538 RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-08-03 05:41:07.000000 RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-08-03 05:41:07.000000 RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 05:41:07.000000 RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2023-08-03 05:41:07.000000 RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 05:41:07.000000 RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2023-07-29 08:14:49.000000 RobertCommonDriver-0.1.49/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.125048 RobertCommonDriver-0.1.49/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.49/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.128384 RobertCommonDriver-0.1.49/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.146720 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33507 2023-08-02 02:36:46.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.166720 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    69811 2023-08-03 05:32:48.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65703 2023-08-03 05:32:48.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566114 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0   101237 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34022 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18276 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    78966 2023-08-03 05:39:12.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    25248 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43255 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51501 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41517 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    35275 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    45086 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12932 2023-08-03 05:36:11.000000 RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 05:41:08.223234 RobertCommonDriver-0.1.49/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-08-03 02:49:10.000000 RobertCommonDriver-0.1.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.168719 RobertCommonDriver-0.1.49/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.49/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.169722 RobertCommonDriver-0.1.49/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.49/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.182188 RobertCommonDriver-0.1.49/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:41:08.211252 RobertCommonDriver-0.1.49/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     4147 2023-07-27 06:18:04.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9682 2023-08-03 02:37:35.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4145 2023-07-27 06:41:53.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.48/LICENSE` & `RobertCommonDriver-0.1.49/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/PKG-INFO` & `RobertCommonDriver-0.1.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.48
+Version: 0.1.49
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.48
+Version: 0.1.49
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.48/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.49/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1635,14 +1635,18 @@
         return 'read_quality'
 
     @property
     def get_read_result(self):
         return 'point_value'
 
     @property
+    def get_read_result_type(self):
+        return 'point_type'
+
+    @property
     def get_write_quality(self):
         return 'write_quality'
 
     @property
     def get_write_result(self):
         return 'write_result'
 
@@ -1659,22 +1663,22 @@
                 if quality is True:
                     self.results['success'][name] = result
                 else:
                     if result not in self.results['error'].keys():
                         self.results['error'][result] = []
                     self.results['error'][result].append(name)
 
-    def get_results(self, show_error: bool = True) -> dict:
+    def get_results(self, show_error: bool = True, **kwargs) -> dict:
         """获取结果集"""
         now = IOTBaseCommon.get_datetime()
         start = self.results.get('start', now)
         success = self.results.get('success', {})
         error = self.results.get('error', {})
         count = self.results.get('count', 0)
         self.update_info(read=count, response=success, cost='{:.2f}'.format((now - start).total_seconds()))
 
         if show_error:
             for err, names in error.items():
                 names = sorted(list(set(names)))
-                self.logging(content=f"get value({len(names)}-[{','.join(names)[:100]}]) fail({err})", level='ERROR', source=','.join(names), pos=self.stack_pos)
+                self.logging(content=f"{'' if kwargs.get('task_name') is None else f'''{kwargs.get('task_name')} '''}get value({len(names)}-[{','.join(names)[:100]}]) fail({err})", level='ERROR', source=','.join(names), pos=self.stack_pos)
 
         return success
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1108,15 +1108,15 @@
                 point_property = point.get('point_property', 'presentValue')
                 value = self._get_value(name, target_address, object_type, instance_number, point_property)
                 if value is not None:
                     self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
 
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files 0% similar despite different names*

```diff
@@ -12106,15 +12106,15 @@
                 point_property = point.get('point_property', 'presentValue')
                 value = self._get_value(name, target_address, object_type, instance_number, point_property)
                 if value is not None:
                     self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
 
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_iec104.py`

 * *Files 0% similar despite different names*

```diff
@@ -2391,15 +2391,15 @@
                 address = point.get('point_address')  # 点地址
                 if type is not None and address is not None:
                     value = self._get_value(name, f"{self.configs.get('host')}:{self.configs.get('port')}", address, type)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_modbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                 data_order = point.get('point_data_order', 0)
                 if device_address is not None and slave_id is not None and fun_code is not None and address is not None and data_type is not None and data_length is not None:
                     value = self.get_value(name, device_address, slave_id, fun_code, address, data_length, data_type, data_order)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_obix.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 point_url = point.get('point_url')
                 point_type = point.get('point_type')
                 value = self.get_value(name, point_url, point_type)
                 if value is not None:
                     self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1603,15 +1603,15 @@
             if point:
                 tag = point.get('point_tag')
                 value = self._get_value(name, tag)
                 if value is not None:
                     self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         write_items = {}
         values = kwargs.get('values', {})
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_opcua.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                     value = self.get_value(name, node_id)
                     if value is not None:
                         if isinstance(value, list):
                             value = value[0]
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
@@ -300,15 +300,15 @@
                     self.logging(content=f"scan {len(results)} point({path})", pos=self.stack_pos)
 
     def _datachange_notification(self, node, val, data):
         try:
             if data.monitored_item.Value.StatusCode.is_good():
                 if val is not None:
                     self.logging(content=f"datachange {node.nodeid.to_string()}({str(val_to_string(val))})")
-                    self.update_device(self.configs.get('endpoint'), node.nodeid.to_string(), **self.gen_read_write_result(True, str(val_to_string(val)), point_time=IOTBaseCommon.get_datetime_str()))
+                    self.update_device(self.configs.get('endpoint'), node.nodeid.to_string(), **self.gen_read_write_result(True, str(val_to_string(val)), point_time=IOTBaseCommon.get_datetime_str(), point_type=data.monitored_item.Value.Value.VariantType.value))
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(f"{data.monitored_item.Value.StatusCode}")
         except Exception as e:
             self.update_device(self.configs.get('endpoint'), node.nodeid.to_string(), **self.gen_read_write_result(False, e.__str__()))
 
@@ -364,15 +364,20 @@
                 self._release_client()
                 for item in read_items:
                     self.update_device(self.configs.get('endpoint'), item, **self.gen_read_write_result(False, e.__str__()))
 
     def _write(self, node, value):
         try:
             if self._get_client():
-                self._get_client().get_node(node).set_value(ua.Variant(value))
+                result = self.get_device_property(self.configs.get('endpoint'), node,[self.get_read_quality, self.get_read_result_type])
+                if isinstance(result, list) and len(result) >= 2 and result[0] is True:
+                    self._get_client().get_node(node).set_value(
+                        ua.DataValue(ua.Variant(value, ua.VariantType(result[1]))))
+                else:
+                    self._get_client().get_node(node).set_value(ua.Variant(value))
                 self.update_device(self.configs.get('endpoint'), node, **self.gen_read_write_result(True, None, False))
         except Exception as e:
             self.update_device(self.configs.get('endpoint'), node, **self.gen_read_write_result(False, e.__str__(), False))
 
     def _get_server(self):
         if self.server is None:
             server = Server()
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,15 +686,15 @@
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,15 @@
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,15 +606,15 @@
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from ctypes import create_string_buffer as ctypes_create_string_buffer, c_int32 as ctypes_c_int32, pointer as ctypes_pointer, cast as ctypes_cast, POINTER, c_uint8 as ctypes_c_uint8, c_uint16 as ctypes_c_uint16, string_at as ctypes_string_at
 from enum import Enum
 from snap7.common import error_text, load_library, check_error
-from snap7.types import S7DataItem, S7WLByte, SendTimeout, RecvTimeout, wordlen_to_ctypes
+from snap7.types import S7DataItem, S7WLByte, SendTimeout, RecvTimeout, RemotePort, wordlen_to_ctypes
 from snap7 import util as snap7_util, client as snap7_client, server as snap7_server
 
 from typing import List, Dict, Any, Optional
 
 from .base import IOTBaseCommon, IOTDriver, IOTSimulateObject
 
 '''
@@ -67,14 +67,25 @@
     
 rack是机架号，slot卡槽号
     s7-200 0, 1
     s7-300 0, 2
     s7-400 具体看硬件组态
     s7-1200/1500 0, 0/1
     
+    
+    配置
+        S7_200Smart	
+            IP/Port/0/0/2
+                STSAP	RTSAP
+                0100    0300
+        S7_200	
+            IP/Port/19799/19799/1
+                STSAP	RTSAP
+                4D57    4D57
+    
 connection_type:
     PG=1
     OP=2
     S7-Basic=3/10
     
 dbnumber:
     地址编号（int），只适用于DB区和200samart的V区，其它区全默认0，V区只能填1
@@ -113,15 +124,15 @@
     DB2,REAL10,VT_R4,192.168.0.2,1,3
     I0.6
 
 '''
 
 
 '''
-    pip install python-snap7==0.10
+    pip install python-snap7==1.3
 '''
 
 
 class IOTPlcS7(IOTDriver):
 
     # 西门子PLC的类型对象
     class S7Version(Enum):
@@ -318,15 +329,15 @@
                 address = point.get('point_address')
                 if device_address is not None and address is not None:
                     value = self.get_value(name, device_address, address)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
@@ -429,14 +440,15 @@
                     if client:
                         if self.configs.get('send_timeout', 15) > 0:
                             client.set_param(SendTimeout, self.configs.get('send_timeout'))
                         if self.configs.get('rec_timeout', 3500) > 0:
                             client.set_param(RecvTimeout, self.configs.get('rec_timeout'))
 
                     if info['type'] == IOTPlcS7.S7Version.S7_200:
+                        client.set_param(RemotePort, info['port'])
                         client._library.Cli_SetConnectionParams(client._pointer, info['host'].encode(), ctypes_c_uint16(info['rack']), ctypes_c_uint16(info['slot']))
                         result = client._library.Cli_Connect(client._pointer)
                         check_error(result, context="client")
                     elif info['type'] == IOTPlcS7.S7Version.S7_200Smart:
                         client.set_connection_type(3)   # 设置连接资源类型，即客户端,连接到PLC   默认情况下，客户端连接为PG（编程控制台），使用此功能可以将连接资源类型更改为OP（西门子HMI面板）或S7 Basic（通用数据传输连接）
                         client.connect(info['host'], info['rack'], info['slot'], info['port'])
                     else:
@@ -551,15 +563,14 @@
                 elif infos[1].startswith('X'):
                     type = IOTBaseCommon.DataTransform.TypeFormat.BOOL
                     length = 1
                     pos = infos[1].find('.')
                     if pos >= 1:
                         start = int(float(infos[1][1:pos]))
                         addr = int(float(infos[1][pos + 1:]))
-
         else:   # I2.0 VD200
             db = 1 if address[0] == 'V' else 0
             if address[1] == 'B':   # BYTE
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT8
                 length = 1
             elif address[1] == 'W':
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT16
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,15 @@
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
```

### Comparing `RobertCommonDriver-0.1.48/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.49/robertcommondriver/system/iot/iot_snmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,15 @@
                 device_host = point.get('point_device_address')  # 192.168.1.200/161/v1/public/private
                 if oid is not None and device_host is not None:
                     value = self._get_value(name, device_host, oid)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
-        return self.get_results()
-
+        return self.get_results(**kwargs)
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
```

### Comparing `RobertCommonDriver-0.1.48/setup.py` & `RobertCommonDriver-0.1.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.48'
-DATE = '2023-08-02'
+VERSION = '0.1.49'
+DATE = '2023-08-03'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
 def test_read_200():
     dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'send_timeout': 15, 'rec_timeout': 3500}
     dict_point = {}
-    dict_point['PMPower_DHU_B1_4F_13'] = {'point_writable': True, 'point_name': 'PMPower_DHU_B1_4F_13', 'point_device_address': '192.168.1.184/102/0/1/2', 'point_address': 'DB1,REAL3000', 'point_scale': '1'}
+    dict_point['PMPower_DHU_B1_4F_13'] = {'point_writable': True, 'point_name': 'PMPower_DHU_B1_4F_13', 'point_device_address': '192.168.1.184/102/19799/19799/1', 'point_address': 'DB1,REAL3000', 'point_scale': '1'}
     client = IOTPlcS7(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
             re = client.read()
             print(re)
         except Exception as e:
```

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.48/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.49/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

