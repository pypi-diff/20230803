# Comparing `tmp/somanet_test_suite-1.0.1.tar.gz` & `tmp/somanet_test_suite-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somanet_test_suite-1.0.1.tar", last modified: Mon Nov  8 15:17:24 2021, max compression
+gzip compressed data, was "somanet_test_suite-1.1.2.tar", last modified: Thu Aug  3 11:05:40 2023, max compression
```

## Comparing `somanet_test_suite-1.0.1.tar` & `somanet_test_suite-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,51 @@
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.092941 somanet_test_suite-1.0.1/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     1098 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/LICENSE
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)      119 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/MANIFEST.in
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     9599 2021-11-08 15:17:24.092941 somanet_test_suite-1.0.1/PKG-INFO
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     7002 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/README.rst
--rwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)     2549 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/install.sh
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)       38 2020-09-11 10:04:50.000000 somanet_test_suite-1.0.1/requirements.txt
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)       38 2021-11-08 15:17:24.092941 somanet_test_suite-1.0.1/setup.cfg
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     1935 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/setup.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.084941 somanet_test_suite-1.0.1/src/
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)      641 2021-11-08 15:15:00.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/__init__.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)        0 2020-09-11 10:04:50.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/__init__.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/ethercat/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)    18046 2021-11-08 15:15:00.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/ethercat/EtherCATMaster.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     4230 2021-11-08 14:21:27.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/ethercat/SOEMMaster.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)      125 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/ethercat/__init__.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/uart/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)        0 2020-09-11 10:04:50.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/uart/__init__.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     8250 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/communication/uart/uart.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite/daq/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)      141 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/daq/__init__.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)    44506 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/daq/daq_labjack.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite/hardware_description_builder/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)        0 2020-09-11 10:04:50.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/hardware_description_builder/__init__.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)    10327 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/hardware_description_builder/build_hardware_description_json.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)    14084 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/hardware_description_builder/dataformat.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)     5096 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/hardware_description_builder/somanet_hw_description_builder
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.092941 somanet_test_suite-1.0.1/src/somanet_test_suite/psu/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)      988 2020-09-11 10:04:50.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/psu/99-ea-psu.rules
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)       51 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/psu/__init__.py
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)    33038 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/psu/psu_ea.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.092941 somanet_test_suite-1.0.1/src/somanet_test_suite/sanssouci/
--rw-rw-r--   0 hstroetgen  (1000) hstroetgen  (1000)        0 2020-09-11 10:04:50.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/sanssouci/__init__.py
--rwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)     7734 2021-10-21 07:34:01.000000 somanet_test_suite-1.0.1/src/somanet_test_suite/sanssouci/sanssouci.py
-drwxrwxr-x   0 hstroetgen  (1000) hstroetgen  (1000)        0 2021-11-08 15:17:24.088941 somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/
--rw-r--r--   0 hstroetgen  (1000) hstroetgen  (1000)     9599 2021-11-08 15:17:23.000000 somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/PKG-INFO
--rw-r--r--   0 hstroetgen  (1000) hstroetgen  (1000)     1257 2021-11-08 15:17:24.000000 somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/SOURCES.txt
--rw-r--r--   0 hstroetgen  (1000) hstroetgen  (1000)        1 2021-11-08 15:17:23.000000 somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/dependency_links.txt
--rw-r--r--   0 hstroetgen  (1000) hstroetgen  (1000)       39 2021-11-08 15:17:23.000000 somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/requires.txt
--rw-r--r--   0 hstroetgen  (1000) hstroetgen  (1000)       19 2021-11-08 15:17:23.000000 somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.127400 somanet_test_suite-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-08-03 11:05:40.127400 somanet_test_suite-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2549 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:05:40.127400 somanet_test_suite-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.115400 somanet_test_suite-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.115400 somanet_test_suite-1.1.2/src/somanet_test_suite/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.123400 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/BaseCANOpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/BaseEtherCAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/BaseFileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.123400 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/can/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/can/CANMaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/esi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.123400 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/ethercat/
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/ethercat/IgHMaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37126 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/ethercat/SOEMMaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/ethercat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.123400 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/uart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/uart/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16424 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/uart/somanet_bootloader_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/communication/uart/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.123400 somanet_test_suite-1.1.2/src/somanet_test_suite/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48495 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/daq/daq_labjack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.127400 somanet_test_suite-1.1.2/src/somanet_test_suite/hardware_description_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/hardware_description_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/hardware_description_builder/build_hardware_description_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/hardware_description_builder/dataformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/hardware_description_builder/somanet_hw_description_builder
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.127400 somanet_test_suite-1.1.2/src/somanet_test_suite/psu/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/psu/99-ea-psu.rules
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/psu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/psu/psu_controller
+-rw-r--r--   0 runner    (1001) docker     (123)    36746 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/psu/psu_ea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.127400 somanet_test_suite-1.1.2/src/somanet_test_suite/sanssouci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/sanssouci/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7735 2023-08-03 11:05:26.000000 somanet_test_suite-1.1.2/src/somanet_test_suite/sanssouci/sanssouci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:40.119400 somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-08-03 11:05:40.000000 somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-03 11:05:40.000000 somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:05:40.000000 somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 11:05:40.000000 somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:05:40.000000 somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/top_level.txt
```

### Comparing `somanet_test_suite-1.0.1/LICENSE` & `somanet_test_suite-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `somanet_test_suite-1.0.1/PKG-INFO` & `somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,280 +1,281 @@
-Metadata-Version: 1.1
-Name: somanet_test_suite
-Version: 1.0.1
+Metadata-Version: 2.1
+Name: somanet-test-suite
+Version: 1.1.2
 Summary: A collection of different scripts and drivers (PSU, EtherCAT, Labjack,...)
-Home-page: UNKNOWN
 Author: Synapticon GmbH
 Author-email: hstroetgen@synapticon.com
 License: MIT
-Description: SOMANET Test Suite
-        ==================
-        
-        All modules to make successful and complete testing of SOMANET modules possible.
-        
-        Even though this suite is written for Linux, at least the Elektronik Automation Power Supply Driver also runs under Windows.
-        
-        Installation
-        ------------
-        
-        1) Install non-python tools (only Linux)
-            ``sudo ./install.sh -a -m <MAC_OF_ETHERCAT_INTERFACE>``
-        
-            This will install:
-                - IgH EtherCAT Master
-                - UDEV rules for power supplies
-                - LabJack driver and Kipling
-                - SOEM EtherCAT Master
-        
-            If one of these tools are already installed, the script will skip the installation
-            and continue with the next tool.
-            Call "-h" to show the help text.
-        
-        2) Install python script
-            ``python setup.py install``
-        
-        
-        Usage
-        -----
-        
-        1. PSU
-        ^^^^^^
-        Import module
-        """""""""""""
-            ``import somanet_test_suite as sts``
-        
-        Create object
-        """""""""""""
-        To connect to a specific PSU, you can call
-        
-        Linux: ``psu = sts.PsuEA(comport='ttyACM0')`` or ``psu = sts.PsuEA(comport='usb-EA_Elektro-Automatik_PS_2042-10B_2815450332-if00')``
-        
-        Windows: ``psu = sts.PsuEA(comport='COM1')`` or as com port description: ``psu = sts.PsuEA(comport='PS 2000 B')``
-        
-        If you added the device rule and you connected only one PSU, there is no need to provide a device name:
-        
-            ``psu = sts.PsuEA()``
-        
-        Also possible is:
-        
-            ``psu = sts.PsuEA(comport='ea-ps-20xx-xx-0')``
-        
-        | If there is more then one PSU connected to the host, the script will connect to the first device found.
-        | It is also possible to take the S/N written on the back of the PSU and call:
-        
-            ``psu = sts.PsuEA(sn='0123456789')``
-        
-        or to use the device designator:
-        
-            ``psu = sts.PsuEA(desi='PS 2142-10B')``
-        
-        
-        Dis/connect to power supply for controlling
-        """""""""""""""""""""""""""""""""""""""""""
-            ``psu.remote_on()``
-        
-            ``psu.remote_off()``
-        
-        For multi output devices most functions provide an additional output argument:
-        
-            ``psu.remote_on(output_num=0)``
-        
-            ``psu.remote_on(output_num=1)``
-        
-        | It's only necessary to call ``remote_on()``, when you want to control the PSU.
-        | If you just want to read device information, you don't need to.
-        
-        Power on and off output
-        """"""""""""""""""""""""""
-            ``psu.output_on()``
-        
-            ``psu.output_off()``
-        
-        or
-        
-            ``psu.output_on(output_num=1)``
-        
-            ``psu.output_off(output_num=1)``
-        
-        Set parameters
-        """"""""""""""""""""""""""
-        Arguments can be int or float.
-        
-            ``psu.set_voltage(24, output_num=0)``
-        
-            ``psu.set_current(0.5, output_num=0)``
-        
-            ``psu.set_ovp(30, output_num=0)``
-        
-            ``psu.set_ocp(8, output_num=0)``
-        
-        The script will always set the maximum possible values in dependency of the nominal power.
-        
-        | For example:
-        | Nominal power = 160 W
-        | When you set the voltage to 40 V, it's not possible to set a higher current than 4 A (=160W/40V),
-        | regardless of the maximum current output of the device.
-        | If you want to set a higher current, you must first reduce the voltage.
-        
-        | Also this script treats voltage with a higher priority.
-        | It will decrease the current, if the maximum power is reached.
-        | For example:
-        | Nominal power = 160 W, set current = 10 A
-        | When you set the voltage to 32 V, it'll results in a maximum current of 5 A.
-        
-        
-        Get parameters
-        """"""""""""""""""""""""""
-        Return argument: float.
-        
-            ``psu.get_voltage(output_num: int)``
-        
-            ``psu.get_current(output_num: int)``
-        
-            ``psu.get_power(output_num: int)``
-        
-        Maximum sampling rate is ~10 Hz.
-        
-        
-        Nominal values:
-        
-        If update is true, the value will be pulled directly from the device.
-        
-            ``psu.get_nominal_voltage(output_num: int, update: bool)``
-        
-            ``psu.get_nominal_current(output_num: int, update: bool)``
-        
-            ``psu.get_nominal_power(output_num: int, update: bool)``
-        
-        
-        Reset error
-        """""""""""""
-        If an overcurrent, overvoltage, overpower or overtemperature protection error happens,
-        you can reset the error with:
-        
-            ``psu.reset_error(output_num: int)``
-        
-        
-        Tracking
-        """""""""""""
-        (Only 3-port devices).
-        Tracking disables the controlling of output 2. Output 1 controls then also output 2.
-        
-            ``psu.tracking_on()``
-        
-            ``psu.tracking_off()``
-        
-        
-        Get status
-        """""""""""""
-        Return argument: dictionary
-        
-            ``psu.get_status(update: bool)``
-        
-        List of dictionary containing the following keys (index is output number):
-        
-        - 'output' (int)
-        - 'remote on' (bool)
-        - 'output on' (bool)
-        - 'controller state' ('CV', 'CC')
-        - 'tracking active' (bool)
-        - 'OVP activ' (bool)
-        - 'OCP activ' (bool)
-        - 'OPP activ' (bool)
-        - 'OTP activ' (bool)
-        - 'act voltage' (float)
-        - 'act current' (float)
-        
-        
-        Get device description
-        """"""""""""""""""""""""""
-        Return argument: tuple (name, SN)
-        
-            ``psu.get_device_description(update : bool)``
-        
-        
-        Close connection
-        """"""""""""""""""""""""""
-        To close the connection, call:
-        
-            ``psu.close()``
-        
-        This will just stop the communication, the PSU outputs will remain in their current states.
-        
-        
-        
-        2. SANSSOUCI - So(manet) Se(nsor) Si(mulator)
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        A framework to simulate different sensors (Hall, QEI, ...).
-        Currently only velocity is supported for Hall and QEI.
-        
-        Preperation
-        """"""""""""""""""""""""""
-        What you need:
-         - LabJack
-         - SN75174 Differential Line Driver (for RS-422 communication and as level shifter 3.3V -> 5V)
-        
-        Connection
-        """"""""""""""""""""""""""
-        See also: https://doc.synapticon.com/hardware/drive/drive_1000/d3/docs/index.html#encoder-port-1
-        
-        +--------------+------------------+
-        | Pin SN75174  | Encoder/Labjack  |
-        +==============+==================+
-        | 1            | LJ: FIO0         |
-        +--------------+------------------+
-        | 2            | A+               |
-        +--------------+------------------+
-        | 3            | A-               |
-        +--------------+------------------+
-        | 4            | Connect with     |
-        |              | 10kOhm to Vcc    |
-        |              | or NC            |
-        +--------------+------------------+
-        | 5            | B-               |
-        +--------------+------------------+
-        | 6            | B+               |
-        +--------------+------------------+
-        | 7            | LJ: FIO01        |
-        +--------------+------------------+
-        | 8            | GND of LJ and    |
-        |              | Encoder          |
-        +--------------+------------------+
-        | 9            | LJ: FIO2         |
-        +--------------+------------------+
-        | 10           | I+               |
-        +--------------+------------------+
-        | 11           | I-               |
-        +--------------+------------------+
-        | 12           | Connect with     |
-        |              | 10kOhm to Vcc    |
-        |              | or NC            |
-        +--------------+------------------+
-        | 13           | N.C.             |
-        +--------------+------------------+
-        | 14           | N.C.             |
-        +--------------+------------------+
-        | 15           | N.C.             |
-        +--------------+------------------+
-        | 16           | Vcc (5V)         |
-        +--------------+------------------+
-        
-        Usage
-        """"""""""""""""""""""""""
-        
-        **Hall**
-        
-            ``sensor = Sanssouci(printer.write, 'HALL', pole_pairs=7)``
-        
-            ``sensor.set_velocity(20)``
-        
-        **QEI**
-        
-            ``sensor = Sanssouci(printer.write, 'QEI', resolution=100)``
-        
-            ``sensor.set_velocity(20)``
-        
-Keywords: power supply unit,psu,daq,Labjack,Elektronik-Automation,EtherCAT,IgH,Synapticon
-Platform: UNKNOWN
+Keywords: power supply unit,psu,daq,Labjack,Elektro-Automation,EtherCAT,IgH,Synapticon,CANopen,CANSOEM
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: System :: Hardware :: Hardware Drivers
+Requires-Python: >=3.6
+License-File: LICENSE
+
+SOMANET Test Suite
+==================
+
+All modules to make successful and complete testing of SOMANET modules possible.
+
+Even though this suite is written for Linux, at least the Elektronik Automation Power Supply Driver also runs under Windows.
+
+Installation
+------------
+
+1) Install non-python tools (only Linux)
+    ``sudo ./install.sh -a -m <MAC_OF_ETHERCAT_INTERFACE>``
+
+    This will install:
+        - IgH EtherCAT Master
+        - UDEV rules for power supplies
+        - LabJack driver and Kipling
+        - SOEM EtherCAT Master
+
+    If one of these tools are already installed, the script will skip the installation
+    and continue with the next tool.
+    Call "-h" to show the help text.
+
+2) Install python script
+    ``python setup.py install``
+
+
+Usage
+-----
+
+1. PSU
+^^^^^^
+Import module
+"""""""""""""
+    ``import somanet_test_suite as sts``
+
+Create object
+"""""""""""""
+To connect to a specific PSU, you can call
+
+Linux: ``psu = sts.PsuEA(comport='ttyACM0')`` or ``psu = sts.PsuEA(comport='usb-EA_Elektro-Automatik_PS_2042-10B_2815450332-if00')``
+
+Windows: ``psu = sts.PsuEA(comport='COM1')`` or as com port description: ``psu = sts.PsuEA(comport='PS 2000 B')``
+
+If you added the device rule and you connected only one PSU, there is no need to provide a device name:
+
+    ``psu = sts.PsuEA()``
+
+Also possible is:
+
+    ``psu = sts.PsuEA(comport='ea-ps-20xx-xx-0')``
+
+| If there is more then one PSU connected to the host, the script will connect to the first device found.
+| It is also possible to take the S/N written on the back of the PSU and call:
+
+    ``psu = sts.PsuEA(sn='0123456789')``
+
+or to use the device designator:
+
+    ``psu = sts.PsuEA(desi='PS 2142-10B')``
+
+
+Dis/connect to power supply for controlling
+"""""""""""""""""""""""""""""""""""""""""""
+    ``psu.remote_on()``
+
+    ``psu.remote_off()``
+
+For multi output devices most functions provide an additional output argument:
+
+    ``psu.remote_on(output_num=0)``
+
+    ``psu.remote_on(output_num=1)``
+
+| It's only necessary to call ``remote_on()``, when you want to control the PSU.
+| If you just want to read device information, you don't need to.
+
+Power on and off output
+""""""""""""""""""""""""""
+    ``psu.output_on()``
+
+    ``psu.output_off()``
+
+or
+
+    ``psu.output_on(output_num=1)``
+
+    ``psu.output_off(output_num=1)``
+
+Set parameters
+""""""""""""""""""""""""""
+Arguments can be int or float.
+
+    ``psu.set_voltage(24, output_num=0)``
+
+    ``psu.set_current(0.5, output_num=0)``
+
+    ``psu.set_ovp(30, output_num=0)``
+
+    ``psu.set_ocp(8, output_num=0)``
+
+The script will always set the maximum possible values in dependency of the nominal power.
+
+| For example:
+| Nominal power = 160 W
+| When you set the voltage to 40 V, it's not possible to set a higher current than 4 A (=160W/40V),
+| regardless of the maximum current output of the device.
+| If you want to set a higher current, you must first reduce the voltage.
+
+| Also this script treats voltage with a higher priority.
+| It will decrease the current, if the maximum power is reached.
+| For example:
+| Nominal power = 160 W, set current = 10 A
+| When you set the voltage to 32 V, it'll results in a maximum current of 5 A.
+
+
+Get parameters
+""""""""""""""""""""""""""
+Return argument: float.
+
+    ``psu.get_voltage(output_num: int)``
+
+    ``psu.get_current(output_num: int)``
+
+    ``psu.get_power(output_num: int)``
+
+Maximum sampling rate is ~10 Hz.
+
+
+Nominal values:
+
+If update is true, the value will be pulled directly from the device.
+
+    ``psu.get_nominal_voltage(output_num: int, update: bool)``
+
+    ``psu.get_nominal_current(output_num: int, update: bool)``
+
+    ``psu.get_nominal_power(output_num: int, update: bool)``
+
+
+Reset error
+"""""""""""""
+If an overcurrent, overvoltage, overpower or overtemperature protection error happens,
+you can reset the error with:
+
+    ``psu.reset_error(output_num: int)``
+
+
+Tracking
+"""""""""""""
+(Only 3-port devices).
+Tracking disables the controlling of output 2. Output 1 controls then also output 2.
+
+    ``psu.tracking_on()``
+
+    ``psu.tracking_off()``
+
+
+Get status
+"""""""""""""
+Return argument: dictionary
+
+    ``psu.get_status(update: bool)``
+
+List of dictionary containing the following keys (index is output number):
+
+- 'output' (int)
+- 'remote on' (bool)
+- 'output on' (bool)
+- 'controller state' ('CV', 'CC')
+- 'tracking active' (bool)
+- 'OVP activ' (bool)
+- 'OCP activ' (bool)
+- 'OPP activ' (bool)
+- 'OTP activ' (bool)
+- 'act voltage' (float)
+- 'act current' (float)
+
+
+Get device description
+""""""""""""""""""""""""""
+Return argument: tuple (name, SN)
+
+    ``psu.get_device_description(update : bool)``
+
+
+Close connection
+""""""""""""""""""""""""""
+To close the connection, call:
+
+    ``psu.close()``
+
+This will just stop the communication, the PSU outputs will remain in their current states.
+
+
+
+2. SANSSOUCI - So(manet) Se(nsor) Si(mulator)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+A framework to simulate different sensors (Hall, QEI, ...).
+Currently only velocity is supported for Hall and QEI.
+
+Preperation
+""""""""""""""""""""""""""
+What you need:
+ - LabJack
+ - SN75174 Differential Line Driver (for RS-422 communication and as level shifter 3.3V -> 5V)
+
+Connection
+""""""""""""""""""""""""""
+See also: https://doc.synapticon.com/hardware/drive/drive_1000/d3/docs/index.html#encoder-port-1
+
++--------------+------------------+
+| Pin SN75174  | Encoder/Labjack  |
++==============+==================+
+| 1            | LJ: FIO0         |
++--------------+------------------+
+| 2            | A+               |
++--------------+------------------+
+| 3            | A-               |
++--------------+------------------+
+| 4            | Connect with     |
+|              | 10kOhm to Vcc    |
+|              | or NC            |
++--------------+------------------+
+| 5            | B-               |
++--------------+------------------+
+| 6            | B+               |
++--------------+------------------+
+| 7            | LJ: FIO01        |
++--------------+------------------+
+| 8            | GND of LJ and    |
+|              | Encoder          |
++--------------+------------------+
+| 9            | LJ: FIO2         |
++--------------+------------------+
+| 10           | I+               |
++--------------+------------------+
+| 11           | I-               |
++--------------+------------------+
+| 12           | Connect with     |
+|              | 10kOhm to Vcc    |
+|              | or NC            |
++--------------+------------------+
+| 13           | N.C.             |
++--------------+------------------+
+| 14           | N.C.             |
++--------------+------------------+
+| 15           | N.C.             |
++--------------+------------------+
+| 16           | Vcc (5V)         |
++--------------+------------------+
+
+Usage
+""""""""""""""""""""""""""
+
+**Hall**
+
+    ``sensor = Sanssouci(printer.write, 'HALL', pole_pairs=7)``
+
+    ``sensor.set_velocity(20)``
+
+**QEI**
+
+    ``sensor = Sanssouci(printer.write, 'QEI', resolution=100)``
+
+    ``sensor.set_velocity(20)``
```

### Comparing `somanet_test_suite-1.0.1/README.rst` & `somanet_test_suite-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `somanet_test_suite-1.0.1/install.sh` & `somanet_test_suite-1.1.2/install.sh`

 * *Files identical despite different names*

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/__init__.py` & `somanet_test_suite-1.1.2/src/somanet_test_suite/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from .daq import daq_labjack
 from .daq.daq_labjack import *
 
-from .communication.ethercat.EtherCATMaster import *
-from .communication import ethercat
+from .communication.BaseEtherCAT import ExceptionEtherCAT
+from .communication.ethercat.IgHMaster import IgHMaster, EcTypes
+from .communication import ethercat, esi
 from .communication.ethercat.SOEMMaster import SOEMMaster
 
+
+from .communication import can
+from .communication.can.CANMaster import CANMaster
+from .communication.can.CANMaster import States as CANStates
+from .communication.BaseCANOpen import EcStates
+
 from .psu.psu_ea import *
 from .psu import psu_ea
 
 from .communication.uart.uart import *
 
 from .sanssouci.sanssouci import Sanssouci, DAQCallback, Encoders
 
-from .hardware_description_builder.build_hardware_description_json import BuildHardwareDescription, JSONInfo
+from .hardware_description_builder.build_hardware_description_json import BuildHardwareDescription
 
 __author__ = "Synapticon GmbH"
 __copyright__ = "Copyright 2021, Synapticon GmbH"
 __license__ = "MIT"
 __email__ = "hstroetgen@synapticon.com"
-__version__ = '1.0.1'
+__version__ = '1.1.2'
```

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/communication/ethercat/EtherCATMaster.py` & `somanet_test_suite-1.1.2/src/somanet_test_suite/communication/ethercat/IgHMaster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-import glob
 import logging
 import os
 import re
 import subprocess as sp
 import sys
-import tempfile
 import time
-import zipfile
-from typing import Union, List, Dict, Type
+from typing import Union, Type, List, Literal
+
+from ..esi import ESI
+from ..BaseEtherCAT import BaseEtherCAT, ExceptionEtherCAT, EcStates, EcTypes, WatchdogRegs
 
 __all__ = [
-    "ExceptionIgH",
-    "EtherCATMaster",
+    "IgHMaster",
+    "EcTypes"
 ]
 
 logger = logging.getLogger(__file__)
 logging.basicConfig(format='[%(levelname)s] %(message)s')
 
 if sys.platform != 'linux':
     exit(1)
 
 # start / stop ethercat kernel module (run as root!)
 # IgH EtherCAT master must be installed
 ecat_master = "/etc/init.d/ethercat"
 
 # ethercat control command
 ETHERCAT_PATH = "/opt/etherlab/bin/ethercat"
-ETHERCAT_CMDS = ["master", "slaves", "sii_read", "sii_write"]
-
-
-class ExceptionIgH(Exception):
-    pass
 
 
 if not os.path.isfile(ETHERCAT_PATH):
     logger.warning('EtherCAT Master IgH is not installed.\n'
                    'To install IgH go to "https://github.com/synapticon/Etherlab_EtherCAT_Master/releases".')
 
 SyncManager = {
@@ -43,55 +38,45 @@
     "BufferIn":  2,
     "BufferOut": 3
 }
 
 ECAT_TIMEOUT = 10  # seconds
 
 
-class EtherCATMaster:
+class IgHMaster(BaseEtherCAT):
     """
     Base Class to communicate with the IgH EtherCAT Master. This class supports
     start and stop of the kernel modules and accesses low level EtherCAT functions.
 
     Dependencies:
     - IgH EtherCAT Master (with Synapticon patches)
     - Synapticons siitool
     """
 
-    types_ = (
-        "bool",
-        "int8", "int16", "int32", "int64",
-        "uint8", "uint16", "uint32", "uint64",
-        "float", "double",
-        "string", "octet_string", "unicode_string",
-        "sm8", "sm16", "sm32", "sm64",
-    )
-
-    states = (
-        "INIT", "PREOP", "BOOT", "SAFEOP", "OP",
-    )
+    ETHERCAT_PATH: str = ETHERCAT_PATH
 
-    def __init__(self, debug: bool = False):
+    def __init__(self, esi_file: str = None):
         """
         Init Ethercat Module.
         Prints error (No exception on purpose), if IgH is not installed
 
         """
-        if not os.path.isfile(ETHERCAT_PATH):
+        super().__init__(False, False)
+
+        if not os.path.isfile(self.ETHERCAT_PATH):
             logger.error('EtherCAT Master IgH is not installed.\n'
                          'To install IgH go to "https://github.com/synapticon/Etherlab_EtherCAT_Master/releases".')
 
-        if debug:
-            logger.setLevel(logging.DEBUG)
+        if esi_file is not None:
+            self.esi = ESI(esi_file)
 
         self.active = False
         self.siiprint = ""
-
-        self.re_int_value = re.compile(r'(0x\w+ )(-?\d+)')
-        self.re_float_value = re.compile(r'(-?\d+\.[\de+-]+)')
+        self._re_int_value = re.compile(r'(0x\w+ )?(-?\d+)')
+        self._re_float_value = re.compile(r'(-?\d+.\d+)')
 
     def start(self) -> None:
         """
         Starts IgH Ethercat Master
         """
         self.active = sp.call(["sudo", ecat_master, "start"], stdout=sp.DEVNULL)
 
@@ -105,115 +90,112 @@
     def restart(self) -> None:
         """
         Restarts IgH Ethercat Master
         """
         self.stop()
         self.start()
 
-    @staticmethod
-    def is_active() -> bool:
+    def is_active(self) -> bool:
         """
         Tests, if the communication is active.
 
         Returns
         -------
         bool
             True, if communication with slave is possible.
         """
 
-        command = f"sudo {ETHERCAT_PATH} slaves"
+        command = f"sudo {self.ETHERCAT_PATH} slaves"
         try:
             res_str = sp.check_output(command, shell=True, stderr=sp.STDOUT)
         except sp.CalledProcessError as e:
             res_str = e.output
 
         return 'Failed' not in res_str.decode()
 
-    def set_state(self, state: str, ignore_timeout: bool = False, slaveid: int = 0) -> bool:
+    def set_state(self, state: EcStates, timeout: int = 10, slaveid: int = 0) -> bool:
         """
-        Set Ethercat state. Possible states are "INIT", "PREOP", "BOOT", "SAFEOP" or "OP".
+        Set Ethercat state. Possible EcStates are "INIT", "PREOP", "BOOT", "SAFEOP" or "OP".
 
         Parameters
         ----------
         state : str
             Desired state.
-        ignore_timeout : bool
-            Ignore timeout. Exit function without verifying, if the state was reached.
+        timeout : int
+            Amount of seconds when timeout hits.
         slaveid : int
             Slave ID. First slave = 0.
 
         Raises
         ------
-            ExceptionIgH: If invalid state was requested.
-            ExceptionIgH: If not able to set the state.
-            ExceptionIgH: If timeout occured.
+            ExceptionEtherCAT: If invalid state was requested.
+            ExceptionEtherCAT: If not able to set the state.
+            ExceptionEtherCAT: If timeout occurred.
 
         Returns
         -------
         bool
-            True, if new state was setted.
+            True, if new state was set.
 
         """
-        _state = state.upper()
-        if not _state in self.states:
-            raise ExceptionIgH(f"Invalid state {_state}")
 
-        command = f"sudo {ETHERCAT_PATH} state -p {slaveid} {_state}"
+        command = f"sudo {self.ETHERCAT_PATH} state -p {slaveid} {state.name}"
 
         t0 = time.time()
-        act_state = None
-        while act_state != _state:
+        act_state = EcStates.NONE
+        while act_state != state:
             if sp.call(command, stdout=sp.DEVNULL, shell=True) != 0:
-                raise ExceptionIgH(f'Set State {_state}')
+                raise ExceptionEtherCAT(f'Set State {state.name}')
 
             act_state = self.get_state(slaveid)
-            if time.time() - t0 > ECAT_TIMEOUT:
-                raise ExceptionIgH(f'Timeout: Set State {_state}')
 
-            if ignore_timeout:
-                return True
+            if timeout == 0:
+                return act_state == state
+
+            if time.time() - t0 > timeout:
+                raise ExceptionEtherCAT(f'Timeout: Set State {state.name}')
 
-        return act_state == _state
+        return act_state == state
 
-    @staticmethod
-    def get_state(slaveid: int = 0) -> str:
+    def get_state(self, slaveid: int = 0) -> EcStates:
         """
         Get current state of specific slave.
 
         Parameters
         ----------
         slaveid : int
             Slave ID
 
         Returns
         -------
         str
             Current state.
 
         """
-        command = f"sudo {ETHERCAT_PATH} slaves -p {slaveid}"
+        command = f"sudo {self.ETHERCAT_PATH} slaves -p {slaveid}"
         state_string = sp.check_output(command,
                                        universal_newlines=True,
                                        shell=True)
         res = re.match(r'\d *\d+:\d+ +(.+?) +. (.+$)', state_string)
         if res:
             state = res.group(1)
-            return state.upper()
-        return 'None'
+            if state.lower() == "init+error":
+                state = "INIT"
+            return EcStates[state]
+        return EcStates.NONE
 
-    @staticmethod
-    def slaves() -> int:
+    def slaves(self) -> int:
         """
         Return amount of connected slaves.
 
         Returns
         -------
         int
         """
-        command = f"sudo {ETHERCAT_PATH} slaves | wc -l"
+        command = f"sudo {self.ETHERCAT_PATH} slaves | wc -l"
         slavecount = sp.check_output(command,
                                      universal_newlines=True,
                                      shell=True)
         return int(slavecount)
 
     def sii_read(self, slaveid: int = 0) -> str:
         """
@@ -226,421 +208,330 @@
 
         Returns
         -------
         str
             Output from siitool.
 
         """
-        command = f"sudo {ETHERCAT_PATH} sii_read -p {slaveid} | siitool -p"
+        command = f"sudo {self.ETHERCAT_PATH} sii_read -p {slaveid} | siitool -p"
         self.siiprint = sp.check_output(command, universal_newlines=True, shell=True)
 
         return self.siiprint
 
-    @staticmethod
-    def sii_write(filepath: str = "somanet_cia402.sii", slaveid: int = 0) -> bool:
+    def sii_write(self, filepath: str = "somanet_cia402.sii", slaveid: int = 0) -> bool:
         """
         Writes SII file to EtherCAT IC.
 
         Parameters
         ----------
         filepath : str
             Path to SII file.
         slaveid : int
             Slave ID
 
         Raises
         ------
-            ExceptionIgH: If file does not exists.
-            ExceptionIgH: If not able to set the alias.
+            ExceptionEtherCAT: If file does not exist.
+            ExceptionEtherCAT: If not able to set the alias.
 
         Returns
         -------
         bool
             True, if successfully written.
 
         """
         if not os.path.exists(filepath):
-            raise ExceptionIgH(f"File '{filepath}' not found.")
+            raise ExceptionEtherCAT(f"File '{filepath}' not found.")
 
-        command = f"sudo {ETHERCAT_PATH} alias -f -p {slaveid} 0"
+        command = f"sudo {self.ETHERCAT_PATH} alias -f -p {slaveid} 0"
 
         if sp.call(command, stdout=sp.DEVNULL, shell=True, timeout=20) != 0:
-            raise ExceptionIgH("Cannot set alias")
+            raise ExceptionEtherCAT("Cannot set alias")
 
-        command = f"sudo {ETHERCAT_PATH} sii_write -f -p {slaveid} {filepath}"
+        command = f"sudo {self.ETHERCAT_PATH} sii_write -f -p {slaveid} {filepath}"
 
         return sp.call(command, stdout=sp.DEVNULL, shell=True, timeout=60) == 0
 
-    @staticmethod
-    def foe_write(filepath: str, filename: str = None, slaveid: int = 0) -> bool:
+    def file_write(self, filepath: str, filename: str = None, slaveid: int = 0) -> bool:
         """
         Writes file to EtherCAT slave.
 
         Parameters
         ----------
         filepath : str
             File path.
         filename : str
             Alternative file name on target slave.
         slaveid : int
             Slave ID
 
         Raises
         ------
-            ExceptionIgH: If file not exists.
-            ExceptionIgH: If path leads not to a file.
+            ExceptionEtherCAT: If file not exists.
+            ExceptionEtherCAT: If path leads not to a file.
 
         Returns
         -------
         bool
             True, if successfully written.
 
         """
         if not os.path.exists(filepath):
-            raise ExceptionIgH(f"No valid file path: {filepath}")
+            raise ExceptionEtherCAT(f"No valid file path: {filepath}")
 
         if not os.path.isfile(filepath):
-            raise ExceptionIgH(f"Not a valid file: {filepath}")
+            raise ExceptionEtherCAT(f"Not a valid file: {filepath}")
 
-        command = f"sudo {ETHERCAT_PATH} foe_write -p {slaveid} {filepath}"
+        command = f"sudo {self.ETHERCAT_PATH} foe_write -p {slaveid} {filepath}"
 
         if filename is not None:
             command += f' -o {filename}'
 
         logger.debug(f"[foe_write] Command: {command}")
 
         return sp.call(command, stdout=sp.DEVNULL, shell=True) == 0
 
-    @staticmethod
-    def foe_read(cmd: str, output: Union[Type[str], Type[bytes]] = None, slaveid: int = 0) -> Union[bool, bytes, str]:
+    def file_read(self, cmd: str, output: Union[Type[str], Type[bytes]] = bytes, slaveid: int = 0) -> Union[bool, bytes, str]:
+
         """
         Reads file from EtherCAT slave.
 
         Parameters
         ----------
         cmd : str
             Read command or file name.
         output : Union[Type[str], Type[bytes]]
             Output format. Use literal str/bytes objects. If None, returns bool
         slaveid : int
             Slave ID
 
         Raises
         ------
-            ExceptionIgH: If reading file failed
-            ExceptionIgH: If output type is unknown.
+            ExceptionEtherCAT: If reading file failed
+            ExceptionEtherCAT: If output type is unknown.
 
         Returns
         -------
         Union[bool, bytes, str]
             True, if no output is required and file was successfully read.
             Otherwise output in bytes or str
         """
-        command = f"sudo {ETHERCAT_PATH} foe_read -p {slaveid} {cmd}"
+        command = f"sudo {self.ETHERCAT_PATH} foe_read -p {slaveid} {cmd}"
         logger.debug(f"[foe_read] Command: {command}")
         if output is not None:
             try:
-                f = sp.check_output(command, shell=True)
+                f = sp.check_output(command, shell=True, stderr=sp.STDOUT)
             except sp.CalledProcessError as e:
-                raise ExceptionIgH(e)
+                raise ExceptionEtherCAT(e.output.decode())
 
             if output is str:
                 return f.decode()
             elif output is bytes:
                 return f
             else:
-                raise ExceptionIgH(f"Unknown output type {output}")
+                raise ExceptionEtherCAT(f"Unknown output type {output}")
         else:
             return sp.call(command, stdout=sp.DEVNULL, shell=True) == 0
 
-    def flash_fw(self, filepath: str, slaveid: int = 0) -> bool:
-        """
-        Flash firmware to EtherCAT Slave. Set's automatically state BOOT.
-
-        Parameters
-        ----------
-        filepath : str
-            Path to firmware file. Can be the binary file with pattern "app.*.bin" or a SOMANET package
-            (Will only flash the firmware binary).
-        slaveid : int
-            Slave ID
-
-        Raises
-        ------
-            ExceptionIgH: If firmware file does not exists
-            ExceptionIgH: If firmware is not a valid SOMANET firmware.
-
-        Returns
-        -------
-        bool
-            True, if successfully written.
-
-        """
-        if not os.path.exists(filepath):
-            raise ExceptionIgH(f'File does not exists')
-
-        file_name = os.path.basename(filepath)
-
-        if re.match(r"^package.+\.zip$", file_name, re.M):
-            # Unzip package to a temporary directory.
-            dtemp = tempfile.mkdtemp(None, 'EtherCATMaster-')
-            with zipfile.ZipFile(filepath) as zf:
-                zf.extractall(dtemp)
-            filepath = glob.glob(os.path.join(dtemp, '*.bin'))[0]
-
-        elif not re.match(r'^app.+\.bin$', file_name, re.M):
-            raise ExceptionIgH(f'{file_name}" is not a valid SOMANET firmware')
-
-        logger.debug("Set BOOT state...")
-
-        self.set_state("BOOT")
-
-        time.sleep(0.1)
-        logger.debug("Flash firmware...")
-
-        return self.foe_write(slaveid=slaveid, filepath=filepath)
-
-    def upload(self, index: int, subindex: int, type: str = None, error: bool = False, slaveid: int = 0) -> Union[int, float, str]:
+    def upload(self, index: int, subindex: int, type: EcTypes = None, error: bool = True, slaveid: int = 0) -> Union[int, float, str, bytes]:
         """
         Reads object from object dictionary.
         Converts int or float objects to corresponding types.
 
         Parameters
         ----------
         index : int
             Dictionary index
         subindex : int
             Dictionary subindex
-        type : str
+        type : EcTypes
             Dictionary data type.
         error : bool
             If True, then show error message during upload.
         slaveid : int
             Slave ID
 
         Raises
         ------
-            ExceptionIgH: If data type is invalid.
+            ExceptionEtherCAT: If data type is invalid.
 
         Returns
         -------
         Union[int, float, str]
             Integer, floating point or string object.
 
         """
         _type = ""
-        if isinstance(type, str):
-            if type not in self.types_:
-                raise ExceptionIgH(f"Type '{type}' is not valid. These are valid types: {self.types_}")
-
-            _type = f"--type {type}"
+        if type is not None:
+            _type = f"--type {type.name}"
+        elif hasattr(self, "esi"):
+            esi_type = self.esi[index][subindex].Type
+            _type = f"--type {esi_type}"
 
-        command = f"sudo {ETHERCAT_PATH} upload -p {slaveid} 0x{index:x} {subindex} {_type}"
+        command = f"sudo {self.ETHERCAT_PATH} upload -p {slaveid} 0x{index:x} {subindex} {_type}"
 
         if error:
             _err = sp.STDOUT
         else:
             _err = sp.DEVNULL
 
-        # Run and try it 5 times, if it fails
-        excp = None
-        for i in range(5):
-            try:
-                output = sp.check_output(command, shell=True, stderr=_err)
-            except Exception as e:
-                excp = e
-                continue
-            else:
-                break
-
-        if excp:
-            raise excp
+        try:
+            output = sp.check_output(command, shell=True, stderr=_err)
+        except sp.CalledProcessError as e:
+            msg = f"{e.output.decode().strip()}: 0x{index:x}:{subindex}"
+            raise ExceptionEtherCAT(msg)
 
-        logger.debug(f"Output: {output}")
+        if type == EcTypes.OCTET_STRING:
+            return output
 
         # Try to decode the output. If not possible return the output directly. Then it's no string.
         try:
-            output = output.decode().strip()
+            output = output.decode().strip().strip("\x00")
         except UnicodeDecodeError:
             return output
 
-        # Check if output is a float.
-        res = self.re_float_value.match(output)
-        if res:
-            return float(res.group(1))
+        if type == EcTypes.STRING:
+            return output
 
         # Check if output is a integer.
-        res = self.re_int_value.match(output)
+        res = self._re_int_value.match(output)
         if res:
             # return Int value
             return int(res.group(2))
 
+        # Check if output is a float.
+        res = self._re_float_value.match(output)
+        if res:
+            return float(res.group(1))
+
         # Return string.
-        return output.rstrip("\x00")
+        return output.strip()
 
-    def download(self, index: int, subindex: int, value: Union[str, int, float], type: str = None, slaveid: int = 0) -> bool:
+    def download(self, index: int, subindex: int, value: Union[str, int, float, bytes], type: EcTypes = None, slaveid: int = 0) -> bool:
         """
         Write new value to object dictionary.
 
         Parameters
         ----------
         index : int
             Dictionary index
         subindex : int
             Dictionary subindex
         value : Union[str, int, float]
             New value.
-        type : str
+        type : EcTypes
             Dictionary data type.
         slaveid : int
             Slave ID
 
         Raises
         ------
-            ExceptionIgH: If data type is invalid.
+            ExceptionEtherCAT: If data type is invalid.
 
         Returns
         -------
         bool
             True, if successfully written.
 
         """
         _type = ""
-        if isinstance(type, str):
-            if type not in self.types_:
-                raise ExceptionIgH(f"Type '{type}' is not valid. These are valid types: {self.types_}")
-
-            _type = f"--type {type}"
-
-        command = f"sudo {ETHERCAT_PATH} download -p {slaveid} 0x{index:x} {subindex} {value} {_type}"
-
-        return sp.call(command, stdout=sp.DEVNULL, shell=True) == 0
-
-    def get_bootloader_version(self, slaveid: int = 0) -> str:
-        """
-        Returns the bootloader version. Sets automatically the BOOT state.
-
-        Parameters
-        ----------
-        slaveid : int
-            Slave ID
-
-        Returns
-        -------
-        str
-            Bootloader version as string.
-        """
+        if type is not None:
+            _type = f"--type {type.name}"
+        elif hasattr(self, "esi"):
+            esi_type = self.esi[index][subindex].Type
+            _type = f"--type {esi_type}"
 
-        self.set_state("BOOT", slaveid=slaveid)
-        return self.foe_read(cmd="bversion", slaveid=slaveid, output=str).strip()
-
-    def get_bootloader_help(self, slaveid: int = 0) -> str:
-        """
-        Returns the bootloader help text. Sets automatically the BOOT state.
-
-        Parameters
-        ----------
-        slaveid : int
-            Slave ID
+        if isinstance(value, bytes):
+            value = "0x" + "".join(f"{b:02x}" for b in reversed(value))
 
-        Returns
-        -------
-        str
-            Bootloader help text.
-        """
+        command = f"sudo {self.ETHERCAT_PATH} download -p {slaveid} 0x{index:x} {subindex} {value} {_type}"
 
-        self.set_state("BOOT", slaveid=slaveid)
-        return self.foe_read(cmd="help", slaveid=slaveid, output=str).strip()
+        try:
+            res = sp.call(command, stdout=sp.DEVNULL, stderr=sp.STDOUT, shell=True) == 0
+        except sp.CalledProcessError as e:
+            msg = f"{e.output.decode().strip()}: 0x{index:x}:{subindex}"
+            raise ExceptionEtherCAT(msg)
+        return res
 
-    def ls(self, slaveid: int = 0) -> List[Dict[str, Union[str, int]]]:
+    def reg_write(self, address: int, data: int, type: EcTypes = None, slaveid: int = 0) -> bool:
         """
-        Returns the bootloader version. Sets automatically the BOOT state.
+        Write to register on EtherCAT IC.
 
         Parameters
         ----------
+        address : int
+            Start address
+        data : Union[int, bytes]
+            Data to written to register.
+        type : EcTypes
+            Data type of "data"
         slaveid : int
-            Slave ID
+            Slave ID / position in the ethercat chain.
 
         Returns
         -------
-        List[Dict[str, Union[str, int]]]
-            List with dictionary with items name:str and size:int in bytes.
+        bool
+            True, otherwise an exception will rise.
         """
-        res = list()
-        _list = self.foe_read(cmd="fs-getlist", slaveid=slaveid, output=str).strip()
-        file_list = re.findall(r'(.+), size: (.+)', _list)
+        _type = ""
+        if type is not None:
+            _type = f"--type {type.name}"
 
-        for name, size in file_list:
-            res.append({"name": name, "size": int(size)})
+        command = f"sudo {self.ETHERCAT_PATH} reg_write -p {slaveid} 0x{address:x} {data} {_type}"
 
+        try:
+            res = sp.call(command, stdout=sp.DEVNULL, stderr=sp.STDOUT, shell=True) == 0
+        except sp.CalledProcessError as e:
+            raise ExceptionEtherCAT(e.output.decode())
         return res
 
-    def rm(self, filename: str, slaveid: int = 0) -> str:
+    def reg_read(self, address: int, byte_amount: int, slaveid: int = 0) -> bytes:
         """
-        Removes file from file system.
+        Read register on EtherCAT IC.
 
         Parameters
         ----------
-        filename: str
-            Name of file, which will be removed.
+        address : int
+            Start address
+        size : int
+            Amount of bytes
         slaveid : int
-            Slave ID
+            Slave ID / position in the ethercat chain.
 
         Returns
         -------
-        str
-            Response message.
-        """
-
-        return self.foe_read(cmd=f"fs-remove={filename}", slaveid=slaveid, output=str).strip()
+        bytes
+            Read register content
 
-    def filesystem_unlock(self, password: str, slaveid: int = 0) -> str:
         """
-        Unlocks the file protection. Necessary when deleting hidden files (.filename).
-
-        Parameters
-        ----------
-        password: str
-            Password to unlock the protection.
-        slaveid : int
-            Slave ID
+        command = f"sudo {self.ETHERCAT_PATH} reg_read -p {slaveid} 0x{address:x} {byte_amount}"
 
-        Returns
-        -------
-        str
-            Response message.
-        """
+        try:
+            output = sp.check_output(command, shell=True, stderr=sp.STDOUT)
+        except sp.CalledProcessError as e:
+            raise ExceptionEtherCAT(e.output.decode())
 
-        return self.foe_read(cmd=f"fs-stackunlock={password}", slaveid=slaveid, output=str).strip()
+        return b"".join([int(byte, 16).to_bytes(1, "little") for byte in output.decode().split()])
 
-    def get_filesystem_info(self, slaveid: int = 0) -> Dict[str, int]:
+    def set_watchdog(self, wd_type: Literal["pdi", "processdata"], wd_time_ms: float, slaveid: int = 0):
         """
-        Returns total, used and free memory on filesystem in bytes.
+        Set watchdog timer.
 
         Parameters
         ----------
+        wd_type : Literal["pdi", "processdata"]
+            Either "pdi" or "processdata"
+        wd_time_ms : float
+            Watchdog time in milliseconds
         slaveid : int
-            Slave ID
-
-        Raises
-        ------
-            ExceptionIgH: If not possible, to parse filesystem info message.
-
-        Returns
-        -------
-        Dict[str, int]
-            Dict with total and used amount of bytes.
+            Slave ID / position in the ethercat chain.
         """
-        info = self.foe_read(cmd=f"fs-info", slaveid=slaveid, output=str).strip()
-        res = re.findall(r'(\d+)', info)
-        if not res:
-            raise ExceptionIgH("Could not parse filesystem info message")
-
-        return {"total": int(res[0]), "used": int(res[1]), "free": int(res[0]) - int(res[1])}
-
+        wd_div = int.from_bytes(self.reg_read(int(WatchdogRegs.WD_DIV.value), 2, slaveid),
+                                byteorder="little", signed=False)
 
-    def get_sdos(self, slaveid: int = 0) -> str:
-
-        command = f"sudo {ETHERCAT_PATH} sdos -p {slaveid}"
-        output = sp.check_output(command, shell=True, stderr=sp.DEVNULL)
-
-        return output.decode()
+        wd_div_ns = 40 * (wd_div + 2)
+        wd_time_reg = int((wd_time_ms * 1_000_000.0) / wd_div_ns)
+        if wd_type == "pdi":
+            wd_reg = WatchdogRegs.WD_TIME_PDI
+        else:
+            wd_reg = WatchdogRegs.WD_TIME_PROCESSDATA
+        self.reg_write(int(wd_reg.value), wd_time_reg, EcTypes.UINT16, slaveid)
```

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/communication/uart/uart.py` & `somanet_test_suite-1.1.2/src/somanet_test_suite/communication/uart/uart.py`

 * *Files identical despite different names*

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/daq/daq_labjack.py` & `somanet_test_suite-1.1.2/src/somanet_test_suite/daq/daq_labjack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
     Collection of useful functions and wrapper for the Labjacks T4 and T7
 """
 import logging
 import math
 import os
 import time
-from typing import List, Tuple, Union, Dict
+from typing import List, Tuple, Union, Dict, Callable
+from enum import Enum
 
 import numpy as np
 
 __all__ = [
     "ExceptionDAQ",
     "ExceptionNoAcknowledgement",
     "DAQLabJack",
     "LJMError",
 ]
 
 logger = logging.getLogger(__file__)
 
 try:
     from labjack import ljm
+    from labjack.ljm import constants
     from labjack.ljm import LJMError
 except Exception as exc:
     logger.warning(str(exc))
 
 LIB_PATH = '/usr/local/lib'
 
 
@@ -41,14 +43,27 @@
 
 
 # Need to be defined outside, because used as argument default values
 _POSITIVE_EDGES: int = 3
 _ONE_SHOT: int = 0
 
 
+class DeviceTypes(Enum):
+    T7 = constants.dtT7
+    T4 = constants.dtT4
+    DIGIT = constants.dtDIGIT
+
+
+class ConnectionTypes(Enum):
+    USB = constants.ctUSB
+    TCP = constants.ctTCP
+    ETHERNET = constants.ctETHERNET
+    WIFI = constants.ctWIFI
+
+
 class DAQLabJack:
     TRIG_FALLING: int = 0
     TRIG_RISING: int = 1
 
     POSITIVE_EDGES: int = _POSITIVE_EDGES
     NEGATIVE_EDGES: int = 4
 
@@ -94,32 +109,34 @@
         "AIN12": 'AIN12',
         "AIN13": 'AIN13',
         "DAC0":  'DAC0',
         "DAC1":  'DAC1',
     }
 
     # Pins that can sample frequency
-    PINS_FREQUENCY_IN: Dict[str, Tuple[str]] = {
-        'T7': ('DIO0', 'DIO1'),
-        'T4': ('DIO4', 'DIO5'),
+    PINS_FREQUENCY_IN: Dict[DeviceTypes, Tuple[str]] = {
+        DeviceTypes.T7: ('DIO0', 'DIO1'),
+        DeviceTypes.T4: ('DIO4', 'DIO5'),
     }
-    PINS_PULSE_OUT: Dict[str, Tuple[str]] = {
-        'T7': ('DIO0', 'DIO2', 'DIO3', 'DIO4', 'DIO5'),
-        'T4': ('DIO6', 'DIO7'),
+    PINS_PULSE_OUT: Dict[DeviceTypes, Tuple[str]] = {
+        DeviceTypes.T7: ('DIO0', 'DIO2', 'DIO3', 'DIO4', 'DIO5'),
+        DeviceTypes.T4: ('DIO6', 'DIO7'),
     }
 
-    MAX_SCAN_RATE: Dict[str, int] = {
-        'T4': 59880,
-        'T7': 100000,
+    MAX_SCAN_RATE: Dict[DeviceTypes, int] = {
+        DeviceTypes.T4: 59880,
+        DeviceTypes.T7: 100000,
     }
 
     PRECISION: int = 6
 
     CORE_FREQ: int = 80e6
 
+    MAX_BUFFER_SIZE: int = 32768
+
     list_types: Tuple[Union[list, tuple]] = (list, tuple)
 
     UART_INIT_REGISTER = (
         'ASYNCH_ENABLE',  # Deactivate Uart and configure it
         'ASYNCH_TX_DIONUM',
         'ASYNCH_RX_DIONUM',
         'ASYNCH_BAUD',
@@ -162,33 +179,29 @@
 
         if log or debug:
             logging.basicConfig(format='[%(levelname)s] (%(asctime)s.%(msecs)03d) {%(module)s:%(lineno)d}> %(message)s')
             logger.setLevel(logging.INFO)
             if debug:
                 logger.setLevel(logging.DEBUG)
 
-        self._id = id
-        self._conn = connection_type
-        self._device = device
-        self._handle = None
         self._clock1_enabled = False
         self._clock2_enabled = False
 
         self.connect(device, connection_type, id, handle)
 
     def __str__(self) -> str:
         """
         String representation.
 
         Returns
         -------
         str
         """
 
-        return f'LJ-{self._device}-{self._id}'
+        return f'LJ-{self._device.value}-{self._id}'
 
     def connect(self, device: str, connection_type: str, id: str, handle: int = None):
         """
         Connects to Labjack.
 
         Parameters
         ----------
@@ -203,58 +216,85 @@
             Device handle. If a handle is used, device, connection_type and id are not needed.
         """
         if handle is not None:
             self._handle = handle
         else:
             self._handle = ljm.openS(device, connection_type, id)
 
+        info = ljm.getHandleInfo(self._handle)
+
+        self._device = DeviceTypes(info[0])
+        self._conn = ConnectionTypes(info[1])
+        self._id = info[2]
+        self._ip = ljm.numberToIP(info[3])
+        self._port = info[4]
+        self._maxBytesPerMB = info[5]
+
+    def get_info(self) -> Dict:
+        """
+        Get device information
+
+        Returns
+        -------
+        Dict
+            device information
+        """
+        return {
+            "deviceType":     self._device.name,
+            "connectionType": self._conn.name,
+            "serialNumber":   self._id,
+            "ipAddress":      self._ip,
+            "port":           self._port,
+            "maxBytesPerMB":  self._maxBytesPerMB
+        }
+
     def close(self):
         """
         Close Labjack connection.
         """
         if self._handle is not None:
             ljm.close(self._handle)
 
-    def scan(self, connection_type: str = None) -> Tuple:
+    def scan(self, device_type: str = "ANY", connection_type: str = "USB") -> Tuple:
         """
         Scan for available Labjacks.
         Parameters
         ----------
         connection_type : str
             Can be: "ANY", "USB", "TCP", "ETHERNET", and "WIFI".
 
         Returns
         -------
         A tuple containing:
         (numFound, aDeviceTypes, aConnectionTypes, aSerialNumbers,
          aIPAddresses)
 
-        numFound: Number of devices found.
+        numFound: Number of devices found. 
         aDeviceTypes: List of device types for each of the numFound
             devices.
         aConnectionTypes: List of connection types for each of the
             numFound devices.
         aSerialNumbers: List of serial numbers for each of the numFound
             devices.
         aIPAddresses: List of IP addresses for each of the numFound
             devices, but only if the connection type is TCP-based. For
             each corresponding device for which aIPAddresses[i] is not
             TCP-based, aIPAddresses[i] will be
             labjack.ljm.constants.NO_IP_ADDRESS.
         """
-        return ljm.listAllS(self._device, connection_type or self._conn)
+        return ljm.listAllS(device_type, connection_type)
 
     def write(self, ports: Union[List[str], Tuple[str], List[Tuple[str, int]], str],
               values: Union[List[Union[int, float]], Tuple[Union[int, float]], int, float] = None):
         """
         Write to one or multiple ports
         Parameters
         ----------
         ports : List, Tuple, str
-            Port name(s). Can also be a list of tuples with port name and value. E.g: [("DIO1", 1),..]
+            Port name(s). Can also be a list of tuples with ports name and value. E.g: [("DIO1", 1),..]
             Argument values shall be None then.
         values : List, Tuple, int, float
             Values to write
 
         Raises
         ------
             ExceptionDAQ: If ports and values have not the same length
@@ -267,24 +307,24 @@
             if len(ports) != len(values):
                 raise ExceptionDAQ('Amount of names and values are not the same')
 
             ljm.eWriteNames(self._handle, len(ports), ports, values)
         else:
             ljm.eWriteName(self._handle, ports, values)
 
-    def read(self, ports: Union[str, List[str], Tuple[str]]) -> Union[List[Union[int, float]], int, float]:
+    def read(self, ports: Union[str, List[str], Tuple[str]]) -> Union[List[Union[int, float]], Tuple[Union[int, float]], int, float]:
         """
-        Read one port or many.
+        Read one ports or many.
         Parameters
         ----------
         ports : Union[str, List[str], Tuple[str]])
 
         Returns
         -------
-        Union[List[Union[int,float]], int, float]
+        Union[List[Union[int, float]], Tuple[Union[int, float]], int, float]
             Read values.
 
         """
         if isinstance(ports, self.list_types):
             return ljm.eReadNames(self._handle, len(ports), ports)
         else:
             return ljm.eReadName(self._handle, ports)
@@ -341,20 +381,20 @@
         config_c : Union[int, float]
             Not used.
         config_d : Union[int, float]
             Not used.
 
         Raises
         ------
-            ExceptionDAQ: If requested port is not supporting PWM.
+            ExceptionDAQ: If requested ports is not supporting PWM.
 
         """
 
         if not self.DIO_NAME_MAP[port] in self.PINS_PULSE_OUT[self._device]:
-            raise ExceptionDAQ(f'"{port}/{self.DIO_NAME_MAP[port]}" cannot generate "Pulse Out" on "{self._device}". Use "{self.PINS_PULSE_OUT[self._device]}" instead.')
+            raise ExceptionDAQ(f'"{port}/{self.DIO_NAME_MAP[port]}" cannot generate "Pulse Out" on "{self._device.name}". Use "{self.PINS_PULSE_OUT[self._device]}" instead.')
 
         # Deactivate all clocks
         config = [
             ("DIO_EF_CLOCK0_ENABLE", 0),
             ("DIO_EF_CLOCK1_ENABLE", 0),
             ("DIO_EF_CLOCK2_ENABLE", 0)
         ]
@@ -365,15 +405,15 @@
             self._clock1_enabled = False
             self._clock2_enabled = False
         if clock_source == 1:
             self._clock1_enabled = True
         if clock_source == 2:
             self._clock2_enabled = True
 
-        # Turn the output port off
+        # Turn the output ports off
         self.write(self.DIO_NAME_MAP[port], 0)
 
         # Configure the signal to be generated
         _config_name_template = "{}_EF_CONFIG_{}"
         config_register = [(_config_name_template.format(self.DIO_NAME_MAP[port], 'A'), config_a)]
 
         for name, conf in zip(['B', 'C', 'D'], [config_b, config_c, config_d]):
@@ -406,196 +446,353 @@
         if not self._clock1_enabled and not self._clock2_enabled:
             config.append(("DIO_EF_CLOCK0_ENABLE", 1))
 
         config.append((f"{self.DIO_NAME_MAP[port]}_EF_ENABLE", 1))
 
         self.write(config)
 
-    def _stream_port(self, port: str, num_scans: int = 20, scan_rate: int = 2000) -> np.ndarray:
+    def config_stream_trigger(self, port: str, enable: bool = True) -> None:
         """
+        Configures trigger for stream port.
+
+        stream_trigger = 0,  no trigger. Stream will start when Enabled
+        stream_trigger = 2000,  DIO0_EF will start stream
+        stream_trigger = 2001,  DIO1_EF will start stream
+        stream_trigger = 2002,  DIO2_EF will start stream...to DIO7_EF
+
+        keep in mind that scanRate of streamBurst has to be >= (numScans + 1) * 2 * frequency of triggering signal
 
         Parameters
         ----------
-        port :
-        num_scans :
-        scan_rate :
+        port : str
+            Port name
+        enable : bool
+            Enable or disable stream trigger
 
         Returns
         -------
+        None
 
         """
-        """
-        Acquire a number of samples from a port and average the return.
-        :param port:
-        :param num_scans: number of samples to acquire
-        :type num_scans: int
-        :param scan_rate: sampling frequency in Hz
-        :type scan_rate: int
-        :return:
-        """
+        stream_trigger = 2000 + int(self.DIO_NAME_MAP[port][3:])
+        if not enable:
+            stream_trigger = 0
+        # Configure LJM for unpredictable stream timing
+        ljm.writeLibraryConfigStringS("LJM_STREAM_SCANS_RETURN", "LJM_STREAM_SCANS_RETURN_ALL")
+        ljm.writeLibraryConfigS("LJM_STREAM_RECEIVE_TIMEOUT_MS", 0)
 
-        port_address = ljm.nameToAddress(port)[0]  # returns (Address, DataType)
-        # self.write("STREAM_RESOLUTION_INDEX", 2)
+        self.write(port, 0)
 
-        # In order to acquire the correct value:
-        #    1. shift multiplexer to desired port by reading from it, and ignore
-        #    2. introduce delay: wait for input's dynamic response to equalize
-        #    3. sample desired port again
+        # 2001 sets DIO1 / FIO1 as the stream trigger
+        self.write("STREAM_TRIGGER_INDEX", stream_trigger)
 
-        sampled_data_throwaway = self.read(port)
-        time.sleep(0.01)  # delay in seconds
+        # DIO%s_EF_ENABLE: Clear any previous DIO0_EF settings [0]
+        # DIO%s_EF_INDEX: 12 enables conditional reset used for triggered acquisition [12]
+        # DIO%s_EF_CONFIG_A:
+        #       Bit 0: Edge select; 0:falling, 1:rising.
+        #       Bit 1: reserved
+        #       Bit 2: 0=OneShot; 1 = only reset once. 0 = reset every n edges. [1 or 5]
+        config = [
+            (f"{self.DIO_NAME_MAP[port]}_EF_ENABLE", 0),
+            (f"{self.DIO_NAME_MAP[port]}_EF_INDEX", 12),
+            (f"{self.DIO_NAME_MAP[port]}_EF_CONFIG_A", 1),
+            (f"{self.DIO_NAME_MAP[port]}_EF_ENABLE", 1)
+        ]
 
-        # returns tuple (ScanRate, samples_acquired)
-        sampled_data = ljm.streamBurst(self._handle, 1, [port_address], scan_rate, num_scans)[1]
+        self.write(config)
 
-        logger.debug(f"Sampled data: {sampled_data}")
-        # Labjack very occasionally returns bogus value, such as -4496.733 or -506.242, etc.
-        # their support does not know the reason, this is a workaround SW fix
-        mean_value = np.mean(sampled_data)
-        if abs(mean_value) > 100:
-            sampled_data = ljm.streamBurst(self._handle, 1, [port_address], scan_rate, num_scans)[1]
-            logger.debug(f"Sampled data (previous were bogus): {sampled_data}")
-            mean_value = np.mean(sampled_data)
+    def set_stream_callback(self, callback: Callable):
+        """
+        Sets a callback that is called by LJM when the stream has
+        collected scansPerRead scans (see stream_start) or if an error has
+        occurred.
 
-        return mean_value
+        Parameters
+        ----------
+        callback : Callable
+            The callback function for LJM's stream thread to call
+            when stream data is ready, which should call
+            stream_read to acquire data. The handle will be the
+            single argument of the callback.
+
+        Returns
+        -------
 
-    def read_average_voltage(self, ports: Union[str, List, Tuple], num_scans: int = 20, scan_rate: int = 2000) -> Union[np.ndarray, List[np.ndarray]]:
         """
+        ljm.setStreamCallback(self._handle, callback)
+
+    def stream_start(self, ports: Union[str, List[str]], scans_per_read: int, scan_rate: int, stream_resolution_index: int = 0):
+        """
+        Prepare stream and starts sampling.
 
         Parameters
         ----------
-        ports :
-        num_scans :
-        scan_rate :
+        ports : Union[str, List[str]]
+        scans_per_read : int
+            Number of scans returned by each call to the
+            eStreamRead function. This is not tied to the maximum
+            packet size for the device.
+        scan_rate : int
+            Scan rate in Hz
+        stream_resolution_index : int
+            The resolution index for stream readings. A larger resolution index generally results in lower noise and longer sample times.
+            T7:
+                Valid values: 0-8. Default value of 0 corresponds to an index of 1.
+            T4:
+                Valid values: 0-5. Default value of 0 corresponds to an index of 1.
+        """
+
+        if scan_rate > self.MAX_SCAN_RATE[self._device]:
+            scan_rate = self.MAX_SCAN_RATE[self._device]
+            logger.warning(f'Scan rate too high. Set it to "{scan_rate}"')
+
+        if not isinstance(ports, self.list_types):
+            ports = [ports]
+
+        self.write('STREAM_BUFFER_SIZE_BYTES', self.MAX_BUFFER_SIZE)  # maximum size, default is 4096
+
+        port_address = []
+        for p in ports:
+            port_address.append(ljm.nameToAddress(p)[0])  # returns (Address, DataType)
+
+        self.stream_read_ports = ports
+
+        self.write("STREAM_RESOLUTION_INDEX", stream_resolution_index)
+
+        return ljm.eStreamStart(self._handle, scans_per_read, len(port_address), port_address, scan_rate)
+
+    def stream_read(self) -> Tuple[Dict[str, List[float]], int, int]:
+        """
+        Reads sampled data from device.
 
         Returns
         -------
+        Tuple[Dict[str, List[float]], int, int]
+            (order_sampled_data, deviceScanBacklog, ljmScanBackLog)
+            - order_sampled_data: Dict with sampled data sorted by port name
+            - deviceScanBacklog: The number of scans left in the device
+                buffer, as measured from when data was last collected from
+                the device. This should usually be near zero and not
+                growing.
+            - ljmScanBacklog: The number of scans left in the LJM buffer, as
+                measured from after the data returned from this function is
+                removed from the LJM buffer. This should usually be near
+                zero and not growing.
 
         """
+        stream_data = ljm.eStreamRead(self._handle)
+
+        deviceScanBacklog = stream_data[1]
+        ljmScanBacklog = stream_data[2]
+        sample_data = stream_data[0]
+
+        order_sampled_data = {}
+        for i, name in enumerate(self.stream_read_ports):
+            order_sampled_data[name] = sample_data[i::len(self.stream_read_ports)]
+
+        return order_sampled_data, deviceScanBacklog, ljmScanBacklog
+
+    def stream_stop(self):
         """
-        Acquire a number of samples from one or multiple ports and average the return.
-        :param ports:
-        :param num_scans: number of samples to acquire
-        :type num_scans: int
-        :param scan_rate: sampling frequency in Hz
-        :type scan_rate: int
-        :return:
+        Stop streaming
         """
-        if isinstance(ports, self.list_types):
-            sampled_data_ave = []
-            for port in ports:
-                sampled_data_ave.append(self._stream_port(port, num_scans, scan_rate))
-            return sampled_data_ave
-        else:
-            return self._stream_port(ports, num_scans, scan_rate)
+        del self.stream_read_ports
+        ljm.eStreamStop(self._handle)
 
-    def get_frequency_max_min_voltage(self, port: str, voltage_range: float = 10.0, num_scans: int = 6000, scan_rate: int = 100e3) -> (float, float, float):
+    def stream_burst_ports(self, ports: Union[str, List[str]], num_scans: int = 20, scan_rate: int = 2000,
+                           stream_resolution_index: int = 0) -> Dict[str, np.ndarray]:
         """
+        Samples one or more ports.
+        Blocking for min. num_scans/scan_rate seconds
 
         Parameters
         ----------
-        port :
-        voltage_range :
-        num_scans :
-        scan_rate :
+        ports : Union[str, List[str]]
+            One or multiple ports
+        num_scans : int
+            Amount of scans
+        scan_rate : int
+            Scan rate in Hz
+        stream_resolution_index : int
+            The resolution index for stream readings. A larger resolution index generally results in lower noise and longer sample times.
+            T7:
+                Valid values: 0-8. Default value of 0 corresponds to an index of 1.
+            T4:
+                Valid values: 0-5. Default value of 0 corresponds to an index of 1.
 
         Returns
         -------
+        Dict[str: list]
+
 
-        """
-        """
-        Sample the analog signal and extract frequency, maximum voltage and minimum voltage.
-        :param port: pin name
-        :type port: str
-        :param voltage_range: voltage range of the analog input (ex. 10 refers to +/-10V input).
-                              Supported ranges: 10, 1, 0.1, 0.01
-        :type voltage_range: int
-        :param num_scans: number of samples to acquire
-        :type num_scans: int
-        :param scan_rate: sampling frequency in Hz
-        :type scan_rate: int
-        :return: list [frequency, average max, average min]
         """
 
         if scan_rate > self.MAX_SCAN_RATE[self._device]:
             scan_rate = self.MAX_SCAN_RATE[self._device]
             logger.warning(f'Scan rate too high. Set it to "{scan_rate}"')
 
-        port_address = ljm.nameToAddress(port)[0]  # returns (Address, DataType)
+        if not isinstance(ports, self.list_types):
+            ports = [ports]
+
         self.write('STREAM_BUFFER_SIZE_BYTES', 32768)  # maximum size, default is 4096
-        self.write(f'{port}_RANGE', voltage_range)
+
+        port_address = [ljm.nameToAddress(p)[0] for p in ports] # returns (Address, DataType)
+
+        self.write("STREAM_RESOLUTION_INDEX", stream_resolution_index)
+
+        # In order to acquire the correct value:
+        #    1. shift multiplexer to desired ports by reading from it, and ignore
+        #    2. introduce delay: wait for input's dynamic response to equalize
+        #    3. sample desired ports again
+
+        sampled_data_throwaway = self.read(ports)
+        time.sleep(0.01)  # delay in seconds
 
         cnt = 5
         while True:
             try:
-                # returns tuple (ScanRate, samples_acquired)
-                sampled_data = ljm.streamBurst(self._handle, 1, [port_address], scan_rate, num_scans)[1]
+                sampled_data = ljm.streamBurst(self._handle, len(port_address), port_address, scan_rate, num_scans)[1]
                 break
             except ljm.LJMError as e:
                 cnt -= 1
                 if cnt == 0:
                     logger.error(e)
-                    raise ljm.LJMError('Not able to sample signal')
+                    raise e
 
-        # recovering the frequency of the sampled signal
-        a = sampled_data
-        a = a - np.mean(a)
-        sampling_freq_of_dac = scan_rate  # maximum sampling freq=100kHz
+        order_sampled_data = {}
 
-        a_f = np.abs(np.real(np.fft.fft(a)))  # performing FFT on the data acquired, saving only real-absolute values
-        a_f_trunk = a_f[1:int(len(a) / 2)]  # truncating the mirrored data from FFT
+        """
+        Interleaved Channels
+            aData returns interleaved data. For example, when streaming two channels, AIN0 and AIN1, aData will look like this:
+            
+            aData[0] contains the first AIN0 sample
+            aData[1] contains the first AIN1 sample
+            aData[2] contains the second AIN0 sample
+            aData[3] contains the second AIN1 sample
+            ...
+            ...
+        """
+        # list contains all data, so sort it
+        for i, name in enumerate(ports):
+            order_sampled_data[name] = np.array(sampled_data[i::len(ports)])
 
-        threshold = np.max(a_f_trunk) - 5  # threshold of where to search for the frequency peaks
+        logger.debug(f"Sampled data: {order_sampled_data}")
 
-        freq_peak_index = np.where(a_f_trunk > threshold)[0]  # boolean comparison, finding indices
-        freq_of_sig = round(freq_peak_index[0] / len(a) * sampling_freq_of_dac, self.PRECISION)
+        return order_sampled_data
 
-        sorted_samples = np.sort(sampled_data)
+    def read_average_voltage(self, ports: Union[str, List, Tuple], num_scans: int = 20, scan_rate: int = 2000) -> Dict[str, np.ndarray]:
+        """
+        Acquire a number of samples from one or multiple ports and average the return.
 
-        range_percent = 5  # percent
-        # to avoid bursts or outliers ignore to highest and lowest 1 or whatever percent
-        range_ignore_percent = 0.5  # percent
+        Parameters
+        ----------
+        ports : Union[str, List, Tuple]
+            Port name as str or list/tuple
+        num_scans : int
+            Amount of scans
+        scan_rate : int
+            Scan rate in Hz
 
-        range_ignore_index = int(range_ignore_percent * len(sorted_samples) / 100)
-        range_index = int(range_percent * len(sorted_samples) / 100)
+        Returns
+        -------
+        Dict[str: np.ndarray]
 
-        min_values = sorted_samples[range_ignore_index:range_index]
-        max_values = sorted_samples[-range_index:-range_ignore_index]
+        """
+
+        sampled_data = self.stream_burst_ports(ports, scan_rate=scan_rate, num_scans=num_scans)
 
-        # round off the trailing numbers
-        max_value = round(float(np.mean(max_values)), self.PRECISION)
-        min_value = round(float(np.mean(min_values)), self.PRECISION)
+        for key, values in sampled_data.items():
+            sampled_data[key] = np.mean(values)
 
-        return freq_of_sig, max_value, min_value
+        return sampled_data
 
-    def get_average_max_min_voltage(self, port: str, num_scans: int = 6000, scan_rate: int = 100e3) -> List[float]:
+    def get_frequency_max_min_voltage(self, ports: Union[str, List, Tuple], voltage_range: float = 10.0,
+                                      num_scans: int = 6000, scan_rate: int = 100e3) -> Dict[str, Tuple[float, float, float]]:
         """
+        Sample the analog signal and extract frequency, maximum voltage and minimum voltage.
 
         Parameters
         ----------
-        port :
-        num_scans :
-        scan_rate :
-
+        port : str
+            Port name
+        voltage_range : float
+            voltage range of the analog input (ex. 10 refers to +/-10V input).
+                              Supported ranges: 10, 1, 0.1, 0.01
+        num_scans : int
+            number of samples to acquire
+        scan_rate : int
+            sampling frequency in Hz
         Returns
         -------
-
+        Dict[str: Tuple[float, float, float]]
+            Dict of tuple. {"port_name": (frequency, average max, average min)}
         """
+        if isinstance(ports, str):
+            ports = [ports]
+
+        for p in ports:
+            self.write(f'{p}_RANGE', voltage_range)
+
+        sampled_data = self.stream_burst_ports(ports, num_scans, scan_rate)
+
+        ret = {}
+
+        for p, sdata in sampled_data.items():
+            # recovering the frequency of the sampled signal
+            a = sampled_data
+            a = a - np.mean(a)
+            sampling_freq_of_dac = scan_rate  # maximum sampling freq=100kHz
+
+            a_f = np.abs(np.real(np.fft.fft(a)))  # performing FFT on the data acquired, saving only real-absolute values
+            a_f_trunk = a_f[1:int(len(a) / 2)]  # truncating the mirrored data from FFT
+
+            threshold = np.max(a_f_trunk) - 5  # threshold of where to search for the frequency peaks
+
+            freq_peak_index = np.where(a_f_trunk > threshold)[0]  # boolean comparison, finding indices
+            freq_of_sig = round(freq_peak_index[0] / len(a) * sampling_freq_of_dac, self.PRECISION)
+
+            sorted_samples = np.sort(sampled_data)
+
+            range_percent = 5  # percent
+            # to avoid bursts or outliers ignore to highest and lowest 1 or whatever percent
+            range_ignore_percent = 0.5  # percent
+
+            range_ignore_index = int(range_ignore_percent * len(sorted_samples) / 100)
+            range_index = int(range_percent * len(sorted_samples) / 100)
+
+            min_values = sorted_samples[range_ignore_index:range_index]
+            max_values = sorted_samples[-range_index:-range_ignore_index]
+
+            # round off the trailing numbers
+            max_value = round(float(np.mean(max_values)), self.PRECISION)
+            min_value = round(float(np.mean(min_values)), self.PRECISION)
+
+            ret[p] = (freq_of_sig, max_value, min_value)
+
+        return ret
+
+    def get_average_max_min_voltage(self, port: str, num_scans: int = 6000, scan_rate: int = 100e3) -> Tuple[float, float, float]:
         """
         Get average, maximum and minimum voltage of an analog signal using build-in functions of Labjack.
-        :param port: Analog port
-        :type port: str
-        :param num_scans: Number of scans
-        :type num_scans: int
-        :param scan_rate: Scan rate in Hertz
-        :type scan_rate: int
-        :return: Measured values, Tuple of (average, max, min) voltage
-        :rtype: tuple
-        """
 
+        Parameters
+        ----------
+        port : str
+            Analog ports
+        num_scans : int
+            Amount of scans
+        scan_rate : int
+            Scan rate in Hz
+
+        Returns
+        -------
+        Tuple[float, float, float]
+            Measured values, Tuple of (average, max, min) voltage
+
+        """
         config = [
             (f'{port}_EF_INDEX', 3),
             (f'{port}_EF_CONFIG_A', num_scans),
             (f'{port}_EF_CONFIG_D', scan_rate),
         ]
 
         self.write(config)
@@ -604,39 +801,39 @@
             f'{port}_EF_READ_A',
             f'{port}_EF_READ_B',
             f'{port}_EF_READ_C',
         ]
 
         return self.read(result)
 
-    def config_read_frequency(self, port: str, clock_source: int = 0, edge: int = _POSITIVE_EDGES, config: int = _ONE_SHOT):
+    def config_read_frequency(self, port: str, clock_source: int = 0, edge: int = _POSITIVE_EDGES, config: int = _ONE_SHOT) -> None:
         """
+        Configure Labjack to sample frequency
 
         Parameters
         ----------
-        port :
-        clock_source :
-        edge :
-        config :
+        port : str
+            Port name
+        clock_source :  int
+            Clock source index, 0 (32bit), 1 (16bit), or 2 (16bit)
+        edge : int
+            Sampling positive or negative edges
+            POSITIVE_EDGES: int = 3
+            NEGATIVE_EDGES: int = 4
+
+        config : int
+            Configure, if frequency is measured once (ONE_SHOT) or constantly (CONTINUOUS)
+            ONE_SHOT: int = 0
+            CONTINUOUS: int = 1
 
         Returns
         -------
-
-        """
-        """
-        Configure Labjack to sample frequency
-        :param port: pin name
-        :type port: str
-        :param clock_source: Clock source index, 0 (32bit), 1 (16bit), or 2 (16bit)
-        :type clock_source: int
-        :param edge: Sampling positive or negative edges
-        :type edge: int
-        :param config: Configure, if frequency is measured once (ONE_SHOT) or constantly (CONTINUOUS)
-        :type config: int
+        None
         """
+
         if not self.DIO_NAME_MAP[port] in self.PINS_FREQUENCY_IN[self._device]:
             raise ExceptionDAQ(f'Error! "{port}/{self.DIO_NAME_MAP[port]}" cannot sample frequency. Use {self.PINS_FREQUENCY_IN[self._device]} instead.')
 
         if clock_source == 0:
             self._clock1_enabled = False
             self._clock2_enabled = False
         if clock_source == 1:
@@ -668,132 +865,48 @@
 
             _config.append((f"{self.DIO_NAME_MAP[port]}_EF_ENABLE", 1))
 
         self.write(_config)
 
     def read_frequency(self, port: str) -> float:
         """
+        Sample frequency on digital input
 
         Parameters
         ----------
-        port :
+        port : str
+            Port name
 
         Returns
         -------
+        float
+            Frequency in Hertz
 
         """
-        """
-        Sample frequency on digital input
-        :param port: digital port name
-        :type port: str
-        :return: Frequency in Hertz
-        :rtype: int
-        """
+
         if not self.DIO_NAME_MAP[port] in self.PINS_FREQUENCY_IN[self._device]:
             raise ExceptionDAQ(f'"{port}/{self.DIO_NAME_MAP[port]}" cannot sample frequency. Use {self.PINS_FREQUENCY_IN[self._device]} instead.')
 
-        # register = '%s_EF_READ_A_F_AND_RESET' % self.DIO_NAME_MAP[port]
+        # register = '%s_EF_READ_A_F_AND_RESET' % self.DIO_NAME_MAP[ports]
         register = f'{self.DIO_NAME_MAP[port]}_EF_READ_A_F'
 
         cnt_try = 50
 
+        freq = 0.0
+
         while cnt_try > 0:
             res = self.read(register)
             if res != 0.0:
-                return 1 / res
+                freq = 1 / res
+                break
             cnt_try -= 1
-        return 0.0
-
-    def config_stream_trigger(self, port: str, enable: int = 1):
-        """
-
-        Parameters
-        ----------
-        port :
-        enable :
-
-        Returns
-        -------
-
-        """
-        """
-        stream_trigger = 0,  no trigger. Stream will start when Enabled
-        stream_trigger = 2000,  DIO0_EF will start stream
-        stream_trigger = 2001,  DIO1_EF will start stream
-        stream_trigger = 2002,  DIO2_EF will start stream...to DIO7_EF
-
-        keep in mind that scanRate of streamBurst has to be >= (numScans + 1) * 2 * frequency of triggering signal
-        """
-        stream_trigger = 2000 + int(self.DIO_NAME_MAP[port][3:])
-        if enable == 0:
-            stream_trigger = 0
-        # Configure LJM for unpredictable stream timing
-        ljm.writeLibraryConfigStringS("LJM_STREAM_SCANS_RETURN", "LJM_STREAM_SCANS_RETURN_ALL")
-        ljm.writeLibraryConfigS("LJM_STREAM_RECEIVE_TIMEOUT_MS", 0)
-
-        self.write(port, 0)
-
-        # 2001 sets DIO1 / FIO1 as the stream trigger
-        self.write("STREAM_TRIGGER_INDEX", stream_trigger)
-
-        # DIO%s_EF_ENABLE: Clear any previous DIO0_EF settings [0]
-        # DIO%s_EF_INDEX: 12 enables conditional reset used for triggered acquisition [12]
-        # DIO%s_EF_CONFIG_A:
-        #       Bit 0: Edge select; 0:falling, 1:rising.
-        #       Bit 1: reserved
-        #       Bit 2: 0=OneShot; 1 = only reset once. 0 = reset every n edges. [1 or 5]
-        config = [
-            (f"{self.DIO_NAME_MAP[port]}_EF_ENABLE", 0),
-            (f"{self.DIO_NAME_MAP[port]}_EF_INDEX", 12),
-            (f"{self.DIO_NAME_MAP[port]}_EF_CONFIG_A", 1),
-            (f"{self.DIO_NAME_MAP[port]}_EF_ENABLE", 1)
-        ]
 
-        self.write(config)
+        return freq
 
-    def read_average_voltage_triggered(self, port: Union[List[str], Tuple[str], str], num_scans: int = 20, scan_rate: int = 2000) -> List[np.ndarray]:
-        """
-        Sample analog port and return the average voltage.
-
-        The maximum possible sample time is 180 ms.
-        Sample time is the number of samples divided by the sample frequency. For example, the period is 16.7 ms when using a scan rate of 6000 Hz and 100 samples:
-
-        100 samples / 6000 samples per second = 16.7 ms
-
-        If the signal has a known periodic component, then setting the sample time to an even multiple of the period will generally improve results.
-
-        Parameters
-        ----------
-        port : Union[List[str], Tuple[str], str]
-            Port names
-        num_scans : int
-            Number of scans
-        scan_rate : int
-            Scan frequency in Hz
-
-        Returns
-        -------
-        List[np.ndarray]
-
-        """
-        if not isinstance(port, self.list_types):
-            port = [port]
-        num_ports = len(port)
-        port_addresses = ljm.namesToAddresses(num_ports, port)[0]  # returns (Address, DataType)
-        # self.write('STREAM_SETTLING_US', 2000)  # stream settling time in microseconds, max = 4400
-        sampled_data = ljm.streamBurst(self._handle, num_ports, port_addresses, float(scan_rate), num_scans)[1]  # returns tuple (ScanRate, samples_acquired)
-
-        sampled_data_ave = []
-        for i in range(1, num_ports + 1):
-            sampled_data_per_channel = [i for i in sampled_data[i - 1::num_ports]]
-            sampled_data_ave.append(np.mean(sampled_data_per_channel))
-
-        return sampled_data_ave
-
-    def set_voltage_range(self, port: str, voltage_range: int):
+    def set_voltage_range(self, port: str, voltage_range: int) -> None:
         """
         Applies the amplification on selected analog input. Default range is 10V, meaning analog input range is +/-10V.
         IMPORTANT: AIN are first mux'ed and then they are amplified. Therefore, when using MUX80, the same gain is applied to the set of mux'ed signals.
 
         Parameters
         ----------
         port : str
@@ -805,15 +918,15 @@
             1       : sets gain=x10, so that the analog input range is ±1 volts.
             0.1     : sets gain=x100, so that the analog input range is ±0.1 volts.
             0.01    : sets gain=x1000, so that the analog input range is ±0.01 volts
         Raises
         ------
             ExceptionDAQ: If device is not T7
         """
-        if self._device != 'T7':
+        if self._device != DeviceTypes.T7:
             raise ExceptionDAQ('Set voltage range only available on T7!')
 
         self.write(f'{port}_RANGE', voltage_range)
 
     def generate_pwm(self, port: str, frequency: int, clock_source: int = 0, duty_cycle: int = 0, phase_shift: int = None, num_pulses: int = None):
         """
         Generate PWM signal with controllable phase shift and controllable number of pulses.
@@ -888,41 +1001,42 @@
     def disable_waveforms(self, *port: str):
         """
         Disable internal Labjack registers from any preconfigured states
 
         Parameters
         ----------
         port : str
-            One or multiple port names. Is actually a tuple.
+            One or multiple ports names. Is actually a tuple.
 
         Raises
         ------
-            ExceptionDAQ: If port tuple is empty
+            ExceptionDAQ: If ports tuple is empty
 
         """
         if not port:
             raise ExceptionDAQ("Port names list is empty")
 
         for p in port:
             self.write(p, 0)
             self.write(f"{self.DIO_NAME_MAP[p]}_EF_ENABLE", 0)
 
-    def read_differential(self, port: str, reference_port: str = None) -> np.ndarray:
+    def read_differential(self, port: str, reference_port: str = None, read_average: bool = False,
+                          num_scans: int = 20, scan_rate: int = 2000) -> np.ndarray:
         """
         Differential readings use a second AIN as a reference point (a.k.a. negative AIN channel).
         For AIN in extended range, positive channels can be in the following ranges:
                 AIN16 to AIN23
                 AIN32 to AIN39
                 AIN48 to AIN55
                 AIN64 to AIN71
                 AIN80 to AIN87
                 AIN96 to AIN103
                 AIN112 to AIN119
                 The negative channel is 8 higher than the positive channel. (ex. pos_ch: AIN48, neg_ch: AIN56).
-        If reference_port is None, it takes the number of "port" (e.g AIN16 -> 16) and adds 8 to it (-> 24)
+        If reference_port is None, it takes the number of "ports" (e.g AIN16 -> 16) and adds 8 to it (-> 24)
 
         Parameters
         ----------
         port : str
             Port name
 
         reference_port : str
@@ -934,30 +1048,36 @@
             ExceptionDAQ: If device is not T7
 
         Returns
         -------
         np.ndarray
             Differential value read with reference to reference_port
         """
-        if self._device != 'T7':
+        if self._device != DeviceTypes.T7:
             raise ExceptionDAQ('Differential analog in only available on T7')
 
         single_ended = 199
 
         if isinstance(reference_port, str):
             reference_port = int(reference_port[3:])
 
         if reference_port is None:
             reference_port = int(port[3:]) + 8
 
+        logger.debug(f'Set {port}_NEGATIVE_CH to {reference_port}')
+
         self.write(f'{port}_NEGATIVE_CH', reference_port)
-        diff_value_read = self.read_average_voltage(port)
+        if read_average:
+            diff_value_read = self.read_average_voltage(port, num_scans, scan_rate)
+            value = diff_value_read[port]
+        else:
+            value = self.read(port)
         # return to single_ended
         self.write(f'{port}_NEGATIVE_CH', single_ended)
-        return diff_value_read
+        return value
 
     def adc_config(self, clk_ch: str, cs_ch: str, mosi_ch: str, spi_mode: int = 0, clk_speed: int = 0, options: int = 0):
         """
         Configures the ADC on a Drive Module via SPI.
 
         Parameters
         ----------
@@ -1253,17 +1373,17 @@
         Init UART on Labjack.
 
         Parameters
         ----------
         baud_rate : int
             Baud rate of UART communication.
         port_tx : str
-            Transceiver port name
+            Transceiver ports name
         port_rx : str
-            Receiver port name
+            Receiver ports name
         """
 
         self.UART_INIT_VALUE[1] = int(self.DIO_NAME_MAP[port_tx][3:])
         self.UART_INIT_VALUE[2] = int(self.DIO_NAME_MAP[port_rx][3:])
         self.UART_INIT_VALUE[3] = baud_rate
 
         self.write(self.UART_INIT_REGISTER, self.UART_INIT_VALUE)
```

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/hardware_description_builder/somanet_hw_description_builder` & `somanet_test_suite-1.1.2/src/somanet_test_suite/hardware_description_builder/somanet_hw_description_builder`

 * *Files identical despite different names*

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/psu/99-ea-psu.rules` & `somanet_test_suite-1.1.2/src/somanet_test_suite/psu/99-ea-psu.rules`

 * *Files identical despite different names*

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/psu/psu_ea.py` & `somanet_test_suite-1.1.2/src/somanet_test_suite/psu/psu_ea.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,24 @@
-import serial
-import serial.tools.list_ports
-import struct
-import time
+import logging
 import os
 import platform
-import logging
+import struct
+import time
+from dataclasses import dataclass
 from typing import List, Tuple, Union, Dict, Any
-from pathlib import Path
+
+import serial
+import serial.tools.list_ports
 
 __all__ = [
     "ExceptionPSU",
     "ExceptionTimeout",
     "PsuEA",
 ]
 
-# Telegram Header
-SEND = 0xC0 + 0x20 + 0x10
-RECEIVE = 0x40 + 0x20 + 0x10
-
-STANDARD_HEADER = [SEND + 1, 0x0, 0x36]
-#            Header  Output Obj  Mask   Command
-REMOTE_MSG = STANDARD_HEADER + [0x10, 0x10]
-OUTPUT_MSG = STANDARD_HEADER + [0x01, 0x01]
-
-TRACKING_ON = STANDARD_HEADER + [0xF0, 0xF0]
-TRACKING_OFF = STANDARD_HEADER + [0xF0, 0xE0]
-
-ACKNOWLEDGE_ALARM = STANDARD_HEADER + [0x0A, 0x0A]
-
 ERR_STRINGS = {
     0x0:  'NO ERROR',
 
     # Communication Error
     0x3:  'CHECKSUM WRONG',
     0x4:  'STARTDELIMITER WRONG',
     0x5:  'WRONG OUTPUT',
@@ -41,25 +28,81 @@
     0x8:  'OBJECT LENGTH INCORRECT',
     0x9:  'NO RW ACCESS',
     0xf:  'DEVICE IN LOCK STATE',
     0x30: 'UPPER LIMIT OF OBJECT EXCEEDED',
     0x31: 'LOWER LIMIT OF OBJECT EXCEEDED'
 }
 
-OBJ_DEV_TYPE = 0x0
-OBJ_SERIAL = 0x1
-OBJ_NOM_U = 0x2
-OBJ_NOM_I = 0x3
-OBJ_NOM_P = 0x4
-OBJ_DEV_CLASS = 0x13
-OBJ_OVP_THRESHOLD = 0x26
-OBJ_OCP_THRESHOLD = 0x27
-OBJ_SET_U = 0x32
-OBJ_SET_I = 0x33
-OBJ_STATUS = 0x47
+
+@dataclass()
+class ObjectEntry:
+    index: int
+    length: int
+    datatype: str
+
+
+@dataclass()
+class Objects:
+    DEV_TYPE: ObjectEntry = ObjectEntry(0x0, 16, 's')
+    SERIAL: ObjectEntry = ObjectEntry(0x1, 16, 's')
+    NOM_U: ObjectEntry = ObjectEntry(0x2, 4, '>f')
+    NOM_I: ObjectEntry = ObjectEntry(0x3, 4, '>f')
+    NOM_P: ObjectEntry = ObjectEntry(0x4, 4, '>f')
+    DEV_ARTICLE_NO: ObjectEntry = ObjectEntry(0x6, 16, 's')
+    MANUFACTURER: ObjectEntry = ObjectEntry(0x8, 16, 's')
+    SW_VERSION: ObjectEntry = ObjectEntry(0x9, 16, 's')
+    DEV_CLASS: ObjectEntry = ObjectEntry(0x13, 2, '>BB')
+    OVP_THRESHOLD: ObjectEntry = ObjectEntry(0x26, 2, '>H')
+    OCP_THRESHOLD: ObjectEntry = ObjectEntry(0x27, 2, '>H')
+    SET_U: ObjectEntry = ObjectEntry(0x32, 2, '>H')
+    SET_I: ObjectEntry = ObjectEntry(0x33, 2, '>H')
+    CONTROL: ObjectEntry = ObjectEntry(0x36, 2, '>BB')
+    STATUS_ACTUAL: ObjectEntry = ObjectEntry(0x47, 6, '>BBHH')
+    STATUS_TARGET: ObjectEntry = ObjectEntry(0x48, 6, '>BBHH')
+
+
+# Telegram Headers #
+SEND_MSG = 0xC0
+RECEIVE_MSG = 0x40
+
+DIRECTION_MSG = 0x10  # From PC to device
+CAST_TYPE = 0x20  # for sending/querying it must be set to 1, in answers it will be 0
+
+# Telegram Header
+SEND_HEADER = SEND_MSG + CAST_TYPE + DIRECTION_MSG
+RECEIVE_HEADER = RECEIVE_MSG + CAST_TYPE + DIRECTION_MSG
+
+CONTROL_HEADER = [SEND_HEADER + 1, 0x0, Objects.CONTROL.index]
+#            Header  Output Obj  Mask   Command
+REMOTE_MSG = CONTROL_HEADER + [0x10, 0x10]
+OUTPUT_MSG = CONTROL_HEADER + [0x01, 0x01]
+
+TRACKING_ON = CONTROL_HEADER + [0xF0, 0xF0]
+TRACKING_OFF = CONTROL_HEADER + [0xF0, 0xE0]
+
+ACKNOWLEDGE_ALARM = CONTROL_HEADER + [0x0A, 0x0A]
+
+# Indexes #
+IDX_DN = 1  # For Triple: Device output number, else always 0
+IDX_OBJ = 2
+IDX_DATA = 3
+IDX_DATA_MASK = IDX_DATA
+IDX_DATA_VALUE = IDX_DATA_MASK + 1
+
+
+@dataclass()
+class PSUQuantities:
+    # Nominal values
+    nom_voltage: float = 0.0
+    nom_current: float = 0.0
+    nom_power: float = 0.0
+    # Actual PSU voltage
+    act_voltage: float = 0.0
+    # Maximum possible current supported by this PSU and the set voltage
+    max_current: float = 0.0
 
 
 class ExceptionPSU(Exception):
     pass
 
 
 class ExceptionTimeout(Exception):
@@ -69,50 +112,46 @@
 class PsuEA:
     OUTPUT_1 = 0x0
     OUTPUT_2 = 0x1
 
     CV = 0x0
     CC = 0x2
 
-    OUTPUT_OFF = 0b01
-    REMOTE_OFF = 0b10
+    OUTPUT_ON = 0x01
+    OUTPUT_OFF = 0x00
+    REMOTE_ON = 0x10
+    REMOTE_OFF = 0x00
 
-    PSU_DEVICE_LIST: Dict[str, Tuple[str]] = {
-        "Linux":   (
-            "ea-ps-2",
-            "usb-EA_Elektro-Automatik",
-        ),
-        "Windows": (
-            'PS 2000 B',
-        ),
-    }
+    SCALING_FACTOR = 25600.0
+    DECIMAL_PLACES = 3
 
+    VENDOR_ID = 0x232e
     DEVICE_CLASS_SINGLE = 0x10
     DEVICE_CLASS_TRIPLE = 0x18
 
-    PATH_DEV = '/dev'
-    PATH_SERIAL = '/dev/serial/by-id'
-
-    def __init__(self, comport: str = None, sn: str = None, desi: str = None, baudrate: int = 115200, log: bool = False, debug: bool = False):
+    def __init__(self, comport: str = None, sn: str = None, designator: str = None,
+                 baudrate: int = 115200, log: bool = False, debug: bool = False):
         """
-        :brief: Class to control PSUs from Elektro Automatik
-                Tested with: EA PS 2042 - 06B,
-                             EA PS 2342 - 10B
-        :param comport: Linux: ttyUSBx or ttyACMx
-                        Windows: COMx
-        :type comport: str
-        :param sn:  Serial number of PSU.
-        :type sn: str
-        :param desi: Designator of PSU.
-        :type desi: str
-        :param baudrate: Should stay to this value. Not changeable on PSU
-        :type baudrate: int
+        Driver to control PSUs from Elektro Automatik's PS series.
 
+        Parameters
+        ----------
+        comport : str
+            Comport name
+        sn : str
+            Serial number of the PSU
+        designator : str
+            Name of the PSU
+        baudrate : int
+            Baud rate. Don't change.
+        log : bool
+            If true show logs.
+        debug : bool
+            If true show debug logs.
         """
-
         ch_console = logging.StreamHandler()
         if debug:
             logger_level = logging.DEBUG
         else:
             logger_level = logging.INFO
         log_handler = [ch_console]
         logging.basicConfig(format='[%(levelname)s] %(asctime)s.%(msecs)03d - L%(lineno)d > %(message)s',
@@ -125,14 +164,17 @@
         self._port = None
         self._baud = baudrate
 
         self.psu = None
 
         self.desc = {'name':                 '-',
                      'serial':               '-',
+                     'manufacturer':         '-',
+                     'software version':     '-',
+                     'device article no':    '-',
                      'controllable_outputs': 1
                      }
 
         _d_state = {'output':           self.OUTPUT_1,
                     'remote on':        False,
                     'output on':        False,
                     'controller state': 'CV',
@@ -144,783 +186,962 @@
                     'act voltage':      0.0,
                     'act current':      0.0
                     }
 
         self.__output_state: List[Dict] = [_d_state, _d_state.copy()]
         self.__output_state[self.OUTPUT_2]['output'] = self.OUTPUT_2
 
-        self.__nom_voltage: float = 0.0
-        self.__nom_current: float = 0.0
-        self.__nom_power: float = 0.0
-        self.__act_voltage: float = 0.0
-        self.__max_current: float = 0.0
+        self.__quantities = PSUQuantities()
 
-        self.__find_devices(comport, sn, desi)
+        self.__find_devices(comport, sn, designator)
 
         if self._port:
             self.get_status()
 
     def __del__(self):
         self.close()
 
-    @staticmethod
-    def __error_handling(res: int) -> Union[str, int]:
-        """
-        Error handling
-        :param res: response number
-        :type res: int
-        :return: Error string
-        :rtype: string or int
+    def __find_devices(self, comport: str, sn: str, designator: str):
         """
-        if ERR_STRINGS[res] != 'NO ERROR':
-            return 'Error: ' + ERR_STRINGS[res]
-        else:
-            return res
+        Find device and connect to them or list a help string.
+        If no value is provided and only one PSU is connected, it will connect to this one.
 
-    @staticmethod
-    def __save_devices(dev_dict: dict, path: str, device_ids: Tuple[str]):
-        """
-        Save all found PSUs and group them by symlink target.
         Parameters
         ----------
-        dev_dict : dict
-            Device dictionary
-        path : str
-            Path to /dev or /dev/serial
-        device_ids : tuple
-            Device iDs by system (Linux, Windows)
-
-        Returns
-        -------
+        comport : str
+            Path to port
+        sn : str
+            Serial number
+        designator : str
+            PSU name
 
+        Raises
+        ------
+        ExceptionPSU: If no PSU could be found.
+        ExceptionPSU: If multiple PSUs where found, but arguments are None.
         """
-        for dev in os.listdir(path):
-            if not any(dev.startswith(id_) for id_ in device_ids):
-                continue
 
-            complete_path = os.path.join(path, dev)
-            resovled_path = str(Path(complete_path).resolve())
-
-            if not dev_dict.get(resovled_path):
-                dev_dict[resovled_path] = [complete_path]
-            else:
-                dev_dict[resovled_path].append(complete_path)
-
-    def __find_devices(self, comport: str, sn: str, desi: str):
-        """
-        Find device and connect to them or list a help string.
-        :param comport: Comport
-        :type comport: string
-        :param sn: serial number of PSU
-        :type sn: string
-        :param desi: Designator of PSU
-        :type desi: string
-        """
-        found = {}
-        _dev = None
-        system = platform.system()
-        device_ids = self.PSU_DEVICE_LIST[system]
-        devs = {}
+        filter_value = None
 
         # Get Device list
-        if system == 'Linux':
-            self.__save_devices(devs, self.PATH_DEV, device_ids)
-            if os.path.isdir(self.PATH_SERIAL):
-                self.__save_devices(devs, self.PATH_SERIAL, device_ids)
-
-        elif system == 'Windows':
-            dev_list = serial.tools.list_ports.comports()
-            devs.fromkeys(list(filter(lambda d: any(id_ in d for id_ in device_ids), dev_list)))
-        else:
-            raise ExceptionPSU("Not supported system architecture")
-
-        # If comport is none, search all compatible PSUs.
-        if comport is None:
-            for dev in devs.keys():
-                self.close()
-                self.logger.debug("Found device at port {}".format(dev))
-                self._port = dev
-                desc = self.connect()
-                desc['port'] = self._port
-
-                # If list contains one device and no Sn or designator are specified, take this device
-                if not sn and not desi and len(devs.keys()) == 1:
-                    self.logger.debug("Take device {}".format(desc))
-                    return
-
-                # If SN or designator is specified and in the device list, take this device.
-                if sn == desc['serial'] or desi == desc['name']:
-                    self.logger.debug("Found corresponding device {}".format(desc))
-                    return
-                else:
-                    # Collect found devices
-                    if not desc["serial"] in found.keys():
-                        found[desc["serial"]] = desc
-
-            # Create help output
-            if len(found) > 1:
-                help_str = [' Found these PSUs:']
-                for psu in found.values():
-                    _outputs = psu['controllable_outputs']
-                    _help = '{}) {} (SN: {}, Output{}: {}), Port: {}'.format(
-                        len(help_str),
-                        psu['name'],
-                        psu['serial'],
-                        "s" if _outputs > 1 else "",
-                        _outputs,
-                        [os.path.basename(p) for p in devs[psu['port']]]
-                    )
-
-                    help_str.append(_help)
-                help_str = '\n'.join(help_str)
-                self.close()
-
-                if sn or desi:
-                    raise ExceptionPSU('ERROR: No PSU with {} "{}" found.{}'.format('S/N' if sn else 'designator',
-                                                                                    sn if sn else desi, help_str))
-                raise ExceptionPSU('No PSU specified.{}'.format(help_str))
-            elif len(found) == 1:
-                return
-            else:
-                raise ExceptionPSU('ERROR: No PSU found')
+        dev_list = list(filter(lambda p: p.vid == self.VENDOR_ID, serial.tools.list_ports.comports()))
 
+        if comport:
+            if not os.path.exists(comport):
+                raise ExceptionPSU(f"Port {comport} does not exists")
+            filter_value = comport
+            if os.path.islink(comport):
+                # resolve symlink and return absolute path to target
+                filter_value = os.path.realpath(comport)
+
+            filtered_dev_list = list(filter(lambda p: filter_value in p.device, dev_list))
+        elif sn:
+            filter_value = str(sn)
+            filtered_dev_list = list(filter(lambda p: filter_value == p.serial_number, dev_list))
+        elif designator:
+            filter_value = designator
+            filtered_dev_list = list(filter(lambda p: designator == p.description, dev_list))
+        elif not comport and not sn and not designator and len(dev_list) == 1:
+            filtered_dev_list = dev_list
         else:
-            p = None
-            if system == 'Linux':
-                p_list = list(filter(lambda port: os.path.basename(comport) in [os.path.basename(p) for p in port], devs.values()))
-                if p_list:
-                    p = p_list[0]
-            elif system == 'Windows':
-                p = list(filter(lambda port: comport in port.description, devs.keys()))
-
-            if not p:
-                raise ExceptionPSU('ERROR: No PSU at port "{}" found.'.format(comport))
-
-            self._port = p[0]
-            self.connect()
+            # Create help output
+            help_str = [' Found these PSUs:']
+            for idx, _dev in enumerate(dev_list):
+                outputs = 1 if _dev.pid == self.DEVICE_CLASS_SINGLE else 3
+                plural = "s" if outputs > 1 else ""
+                help_ = f'{idx + 1}) {_dev.description}, SN: {_dev.serial_number}, Output{plural}: {outputs}, Port: {_dev.device}'
+                help_str.append(help_)
+            help_str = '\n'.join(help_str)
+
+            raise ExceptionPSU(f'No PSU specified.{help_str}')
+
+        if len(filtered_dev_list) > 1:
+            raise ExceptionPSU(f"Found more than one PSU for {filter_value}")
+
+        if not filtered_dev_list:
+            additional_info = ""
+            if filter_value:
+                additional_info = f" for {filter_value}"
+
+            raise ExceptionPSU('ERROR: No PSU found' + additional_info)
+
+        dev = filtered_dev_list[0]
+        self._port = dev.device
+        self.connect()
 
     @staticmethod
     def __pack_list(_list: List[int]) -> bytes:
         """
         Pack list of bytes to bytestring
-        :param _list: list of bytes
-        :type _list: list
-        :return: bytes
-        :rtype: bytes
+
+        Parameters
+        ----------
+        _list : List[int]
+            Telegram for PSU.
+
+        Returns
+        -------
+        bytes
+            Telegram as bytes
         """
         return struct.pack(f'{len(_list)}B', *_list)
 
     @staticmethod
     def __int_to_bytes(num: int, num_bytes: int) -> List[int]:
         """
-        Convert int to bytes
-        :param num: Value to convert
-        :type num: int
-        :param num_bytes: Amount of requested bytes
-        :type num_bytes: int
-        :return: list of bytes
-        :rtype: list
+        Convert a number into bytes
+
+        Parameters
+        ----------
+        num : int
+            Number to convert
+        num_bytes : int
+            Amount of bytes.
+
+        Returns
+        -------
+        List[int]
+            List of bytes.
+
         """
+
         _list = [8 * i for i in reversed(range(num_bytes))]
         return [(num >> i & 0xff) for i in _list]
 
     def __calc_checksum(self, cmd_list: List[int]) -> List[int]:
         """
+        Calculate the checksum.
+        It's just the sum of all bytes in the message. 16 bit long.
 
-        :param cmd_list:
-        :type cmd_list:
-        :return:
-        :rtype:
+        Parameters
+        ----------
+        cmd_list : List[int]
+            Telegram,
+        Returns
+        -------
+        List[int]
+            Checksum
         """
         checksum = 0
         for byte in cmd_list:
             checksum += byte
         return self.__int_to_bytes(checksum, 2)
 
     @staticmethod
-    def __get_response(package: List[int]) -> List[int]:
+    def __get_message(response: bytes) -> bytes:
         """
-        Get response
-        :param package: received message list
-        :type package: list
-        :return: sub list
-        :rtype: list
-        """
-        return package[3:-2]
-
-    def __tx_rx(self, cmd: List[int], expect_length: int) -> List[int]:
-        """
-        Send and receive message from device
-        :param cmd: cmd list
-        :type cmd: list
-        :param expect_length:
-        :type expect_length:
-        :return: Response
-        :rtype: bytes
-        """
-        if self.psu:
-            checksum = self.__calc_checksum(cmd)
-            output = self.__pack_list(cmd + checksum)
-            self.psu.write(output)
-            time.sleep(0.005)
-            num = 0
-            t0 = time.time()
-            while num < (expect_length + 5):
-                num = self.psu.inWaiting()
-                if time.time() - t0 > 1:
-                    raise ExceptionTimeout('Didn\'t receive %d bytes in time.' % (expect_length + 5))
-            res = self.__get_response(self.psu.read(num))
-            time.sleep(0.04)
-            return res
-        raise ExceptionPSU('No PSU connected')
+        Get actual message from response.
+
+        Parameters
+        ----------
+        response : bytes
+            Message without frame.
+
+        Returns
+        -------
+        bytes
+            Message
+        """
+        return response[3:-2]
+
+    def __tx_rx(self, cmd: List[int], expect_length: int) -> bytes:
+        """
+        Send a telegram and receive response.
+
+        Parameters
+        ----------
+        cmd : List[int]
+            Telegram
+        expect_length : int
+            Expected length of response.
+        Returns
+        -------
+        bytes
+            Response message.
+        """
+        timeout = 2
+
+        if not self.psu:
+            raise ExceptionPSU('No PSU connected')
+
+        self.psu.reset_input_buffer()
+        checksum = self.__calc_checksum(cmd)
+        output = self.__pack_list(cmd + checksum)
+        self.psu.write(output)
+        time.sleep(0.005)
+
+        _amount_bytes = 0
+        response = b""
+        t0 = time.time()
+
+        while self.psu.in_waiting == 0:
+            if time.time() - t0 > timeout:
+                raise ExceptionTimeout(f'Didn\'t receive any bytes in time.')
+
+        while self.psu.in_waiting:
+            _recv_bytes = self.psu.in_waiting
+            _amount_bytes += _recv_bytes
+            response += self.psu.read(_recv_bytes)
+
+        # Look at last data byte. Shall be a zero byte if it's a string. Some strings are too short
+        if response[-3] != 0 and _amount_bytes < expect_length:
+            raise ExceptionPSU(f"No proper response: {response}")
+
+        res = self.__get_message(response)
+        time.sleep(0.04)
+        return res
 
     def _check_outputs(self, output_num: int):
         """
         Check, if requested output number is in range of actual available outputs.
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :raise ExceptionPSU, if device has only one output
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Raises
+        -------
+        ExceptionPSU : If device has only one output and output_num is > 0.
+        ExceptionPSU : If tracking is active.
         """
+
         existing_outputs = self.desc['controllable_outputs']
         if output_num > 0 and output_num >= existing_outputs:
-            raise ExceptionPSU('Error: PSU has only {} output{}.'.format(existing_outputs,
-                                                                         's' if existing_outputs > 1 else ''))
-        elif self.__output_state[output_num]["tracking active"] and output_num > 0:
+            raise ExceptionPSU(f'Error: PSU has only {existing_outputs} output{"s" if existing_outputs > 1 else ""}.')
+
+        if self.__output_state[output_num]["tracking active"] and output_num > 0:
             raise ExceptionPSU('Error: Tracking is active. Second output is not controllable!')
 
-    def __set_value(self, value: Union[int, float], max_value: Union[int, float], obj_num: int, output: int):
+    def __set_value(self, value: Union[int, float], max_value: Union[int, float], obj: ObjectEntry, output: int):
         """
         Set value on device
-        :param value: voltage or current value
-        :type value: int or float
-        :param max_value: Max value (nominal value)
-        :type max_value: int or float
-        :param obj_num: object index
-        :type obj_num: int
-        :param output: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output: int
+
+        Parameters
+        ----------
+        value : Union[int, float]
+            voltage or current value
+        max_value : Union[int, float]
+            Max value (nominal value)
+        obj : ObjectEntry
+            Object entry
+        output : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Raises
+        ------
+        ExceptionPSU : if max_value is Zero
+        ExceptionPSU : If an error occurs.
         """
+
         self._check_outputs(output)
 
         if not self.__output_state[output]['remote on']:
             self.remote_on(output)
 
         if max_value == 0.0:
             raise ExceptionPSU('Error: "Max Value" in "set_value()" is zero.')
 
-        value_percent = int((value * 25600.0) / max_value)
-        value_bytes = self.__int_to_bytes(value_percent, 2)
-        packet = [SEND + len(value_bytes) - 1, output, obj_num] + value_bytes
-        error = struct.unpack('B', self.__tx_rx(packet, 1))[0]
-        if error != 0x0:
-            raise ExceptionPSU(ERR_STRINGS[error])
+        value_percent = int((value * self.SCALING_FACTOR) / max_value)
+        value_bytes = self.__int_to_bytes(value_percent, obj.length)
+        packet = [SEND_HEADER + obj.length - 1, output, obj.index] + value_bytes
+        res = self.__tx_rx(packet, 1)
+        self._check_for_error(res)
 
-    def __get_value(self, obj: int, exp_len: int, pattern: str, output: int) -> Union[List[int], Tuple[Any]]:
+    def __get_value(self, obj: ObjectEntry, output: int) -> Union[bytes, Tuple[Any]]:
         """
-        Get int value
-        :param obj: object index
-        :type obj: int
-        :param exp_len: Expected message length in byte
-        :type exp_len: int
-        :param pattern: struct pattern string
-        :type pattern: str
-        :param output: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output: int
-        :return: response list
-        :rtype: Union[List[int], Tuple[Any]]
+        Get integer value from device.
+
+        Parameters
+        ----------
+        obj : ObjectEntry
+            Object entry
+        output : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        Union[bytes, Tuple[Any]]
+            Response from device.
         """
+
         self._check_outputs(output)
 
         if not self.__output_state[output]['remote on']:
             self.remote_on(output)
 
-        packet = [RECEIVE, output, obj]
-        res = self.__tx_rx(packet, exp_len)
+        packet = [RECEIVE_HEADER + obj.length - 1, output, obj.index]
+        res = self.__tx_rx(packet, obj.length)
 
-        if pattern == 's':
+        if obj.datatype == 's':
             return res
-        return struct.unpack(pattern, res)
+        return struct.unpack(obj.datatype, res)
 
-    def __get_float(self, obj: int, output: int) -> Tuple[Any]:
+    def __get_float(self, obj: ObjectEntry, output: int) -> Tuple[Any]:
         """
         Get Float value from device
-        :param obj: object index
-        :type obj: int
-        :param output: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output: int
-        :return: values from device
-        :rtype: Tuple[Any]
+
+        Parameters
+        ----------
+        obj : ObjectEntry
+            Object entry
+        output : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        Tuple[Any]
+            Response from device.
         """
+
         self._check_outputs(output)
 
-        packet = [RECEIVE, output, obj]
-        res = self.__tx_rx(packet, 4)
+        packet = [RECEIVE_HEADER, output, obj.index]
+        res = self.__tx_rx(packet, obj.length)
         return struct.unpack('>f', res)
 
-    @staticmethod
-    def _calculate_value(value: Union[int, float], nom_value: Union[int, float]) -> float:
+    def __get_string(self, obj: ObjectEntry) -> str:
+        """
+        Get string value from device
+        Parameters
+        ----------
+        obj : ObjectEntry
+            Object entry
+
+        Returns
+        -------
+        str
+            Response string
+        """
+        msg = self.__get_value(obj, 0)
+        # Check if last byte is a null byte
+        if msg[-1] == 0:
+            # Remove it
+            msg = msg[:-1]
+        return msg.decode('ascii')
+
+    def _check_for_error(self, response: bytes):
+        """
+        Check if device responses with an error.
+        Parameters
+        ----------
+        response : bytes
+            Response from device
+
+        Raises
+        ------
+        ExceptionPSU : If error is not Zero.
+        """
+        error = struct.unpack('B', response)[0]
+        if error != 0x0:
+            raise ExceptionPSU(ERR_STRINGS[error])
+
+    def _calculate_value(self, value: Union[int, float], nom_value: Union[int, float]) -> float:
         """
         Calculate the voltage or current coming from device.
-        :param value: value from device
-        :type value: int
-        :param nom_value: nominal value
-        :type nom_value: int or float
-        :return: Actual voltage/current
-        :rtype: float
+
+        Parameters
+        ----------
+        value : Union[int, float]
+            value from device
+        nom_value : Union[int, float]
+            Nominal value.
+
+        Returns
+        -------
+        float
+            Actual readable voltage / current
+        """
+
+        return round((value * nom_value) / self.SCALING_FACTOR, self.DECIMAL_PLACES)
+
+    def __send_msg(self, msg: List[int], state_name: str = None):
+        """
+        Send message to PSU and throw error if a problem occurs.
+
+        Parameters
+        ----------
+        msg : List[int]
+            Telegram message for PSU
+        state_name : str
+            State names in dict to set the new value there.
+
+        Raises
+        ------
+            ExceptionPSU: If error is not null
+            ExceptionPSU: If sending message failed 5 times
         """
-        return round((value * nom_value) / 25600.0, 3)
+        counter = 5
+
+        output_num = msg[IDX_DN]
+        value = msg[IDX_DATA_VALUE]
+
+        while True:
+            res = self.__tx_rx(msg, 1)
+            if len(res) == 1:
+                self._check_for_error(res)
+
+                if state_name:
+                    self.__output_state[output_num][state_name] = bool(value)
+                break
+
+            if counter == 0:
+                raise ExceptionPSU(f'ERROR: Did not received ACK for {state_name.upper()}: {value}')
+
+            counter -= 1
+
+    def _send_remote(self, value: int, output_num: int, init: bool):
+        """
+        Send remote message (on/off)
+
+        Parameters
+        ----------
+        value : int
+            1 or 0 (on or off)
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+        init : bool
+        Init device first (only for remote_on())
+        Returns
+        -------
+
+        """
+
+        self.logger.debug("send_remote({})".format(output_num))
+
+        self._check_outputs(output_num)
+
+        REMOTE_MSG[IDX_DN] = output_num
+        REMOTE_MSG[IDX_DATA_VALUE] = value
+
+        self.__send_msg(REMOTE_MSG, 'remote on')
+
+        if init:
+            self._init_device(output_num)
+
+    def _send_output(self, value: int, output_num: int):
+        """
+        Turn on or off power output on device.
+
+        Parameters
+        ----------
+        value : int
+            1 or 0 (On or Off)
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+        """
+
+        self._check_outputs(output_num)
+
+        OUTPUT_MSG[IDX_DN] = output_num
+        OUTPUT_MSG[IDX_DATA_VALUE] = value
+
+        self.__send_msg(OUTPUT_MSG, 'output on')
 
     def _init_device(self, output_num: int = 0):
         """
-        Init device
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
+        Initialize device.
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+
         """
         self.get_nominal_values(output_num, True)
-        self.set_ovp(self.__nom_voltage, output_num)
-        self.set_ocp(self.__nom_current, output_num)
+        self.set_ovp(self.__quantities.nom_voltage, output_num)
+        self.set_ocp(self.__quantities.nom_current, output_num)
 
     def connect(self, comport: str = None) -> Dict[str, Union[str, int]]:
         """
-        :brief Connect with PSU
-        :param comport: COM port name
-        :type comport: str
-        :return: Device Description
-        :rtype: Dict[str, Union[str, int]]
+        Connect with PSU
+
+        Parameters
+        ----------
+        comport : str
+            Path to comport.
+
+        Returns
+        -------
+        Dict[str, Union[str, int]]
+            Device description
         """
+
         port = ''
         if platform.system() == 'Windows':
             port = comport or self._port.device
         elif platform.system() == 'Linux':
             port = comport or self._port
         self.psu = serial.Serial(port, self._baud, timeout=5)
         return self.get_device_description(True)
 
     def close(self):
         """
-        :brief Closes the serial connection.
+        Closes the serial connection.
         """
-        if self.psu:
+        if hasattr(self, "psu") and self.psu is not None:
             for output in range(self.desc['controllable_outputs']):
                 if output > self.OUTPUT_1 and self.__output_state[output]['tracking active']:
                     continue
                 self.remote_off(output)
 
             self.psu.close()
         self.psu = None
         self._port = None
 
     def get_status(self, update: bool = True) -> List[Dict]:
         """
-        :brief: Get status from device. See programming Guide for further information page 11
-        :param update: If True, update state dictionary from device
-        :param update: bool
-        :return: Dictionary with current states.
-        :rtype: dict
+        Get status from device. See programming Guide for further information page 11.
+
+        Parameters
+        ----------
+        update : bool
+            Pull information from device.
+
+        Returns
+        -------
+        List[Dict]
+            Status information
         """
+
         if update:
             outputs = self.desc['controllable_outputs']
-            self.logger.debug("get_status(), Controllable outputs: {}".format(outputs))
+            self.logger.debug("get_status(), Controllable outputs: %d", outputs)
             output_state = []
-            status = list()
+            status = []
             for output_num in range(outputs):
                 output_state.append({})
                 # if tracking active and this is the second output, skip getting value and use status from first output.
                 if output_num == self.OUTPUT_2 and output_state[0]['tracking active']:
                     self.logger.debug("Tracking is active")
                 else:
-                    status = self.__get_value(OBJ_STATUS, 6, '>BBHH', output_num)
+                    status = self.__get_value(Objects.STATUS_ACTUAL, output_num)
 
                 remote_on = status[0]
                 status_byte = status[1]
                 output_state[output_num]['remote on'] = remote_on == 1
                 output_state[output_num]['output on'] = (status_byte & 0x1) == 1
                 output_state[output_num]['controller state'] = 'CV' if (status_byte >> 1) & 0x3 == self.CV else 'CC'
                 output_state[output_num]['tracking active'] = ((status_byte >> 3) & 0x1) == 1
                 output_state[output_num]['OVP active'] = ((status_byte >> 4) & 0x1) == 1
                 output_state[output_num]['OCP active'] = ((status_byte >> 5) & 0x1) == 1
                 output_state[output_num]['OPP active'] = ((status_byte >> 6) & 0x1) == 1
                 output_state[output_num]['OTP active'] = ((status_byte >> 7) & 0x1) == 1
-                output_state[output_num]['act voltage'] = self._calculate_value(status[2], self.__nom_voltage)
-                output_state[output_num]['act current'] = self._calculate_value(status[3], self.__nom_current)
+                output_state[output_num]['act voltage'] = self._calculate_value(status[2], self.__quantities.nom_voltage)
+                output_state[output_num]['act current'] = self._calculate_value(status[3], self.__quantities.nom_current)
             self.__output_state = output_state
         return self.__output_state
 
     def get_device_description(self, update: bool = False) -> Dict[str, Union[str, int]]:
         """
-        :brief Get device name
-        :return: Device name
-        :rtype: Dict[str, Union[str, int]]
-        """
-        self.logger.debug("get_device_description()")
-        if self.desc['name'] == '-' or update:
-            self.logger.debug("get_device_description(): Update")
-            self.desc['name'] = self.__get_value(OBJ_DEV_TYPE, 12, 's', 0)[:-1].decode('ascii')
-            self.desc['serial'] = self.__get_value(OBJ_SERIAL, 11, 's', 0)[:-1].decode('ascii')
-            self.desc['controllable_outputs'] = 1 if self.__get_value(OBJ_DEV_CLASS, 2, '>BB', 0)[1] == self.DEVICE_CLASS_SINGLE else 2
-        return self.desc.copy()
+        Get device description
 
-    def __send_msg(self, msg: List[int], state_name: str = None):
-        """
-        Send message to PSU and throw error if a problem occurs.
         Parameters
         ----------
-        msg : List[int]
-            Telegram message for PSU
-        state_name : str
-            State name in dict to set the new value there.
+        update : bool
+            Pull information from device.
 
-        Raises
-        ------
-            ExceptionPSU: If error is not null
-            ExceptionPSU: If sending message failed 5 times
+        Returns
+        -------
+        Dict[str, Union[str, int]]
+            Description dictionary
         """
-        counter = 5
-
-        output_num = msg[1]
-        value = msg[4]
-
-        while True:
-            res = self.__tx_rx(msg, 1)
-            if len(res) == 1:
-                error = struct.unpack('B', res)[0]
-                if error != 0x0:
-                    raise ExceptionPSU(ERR_STRINGS[error])
-                else:
-                    if state_name:
-                        self.__output_state[output_num][state_name] = bool(value)
-                    break
-
-            if counter == 0:
-                raise ExceptionPSU(f'ERROR: Did not received ACK for {state_name.upper()}: {value}')
 
-            counter -= 1
+        self.logger.debug("get_device_description()")
+        if self.desc['name'] == '-' or update:
+            self.logger.debug("get_device_description(): Update")
+            self.desc['name'] = self.__get_string(Objects.DEV_TYPE)
+            self.desc['serial'] = self.__get_string(Objects.SERIAL)
+            self.desc['manufacturer'] = self.__get_string(Objects.MANUFACTURER)
+            self.desc['software version'] = self.__get_string(Objects.SW_VERSION)
+            self.desc['device article no'] = self.__get_string(Objects.DEV_ARTICLE_NO)
+            self.desc['controllable_outputs'] = 1 if self.__get_value(Objects.DEV_CLASS, 0)[1] == self.DEVICE_CLASS_SINGLE else 2
+        return self.desc.copy()
 
-    def _send_remote(self, value: int, output_num: int, init: bool):
+    def remote_on(self, output_num: int = 0, init: bool = True):
         """
-        Send remote message (on/off)
-        :param value: 1 or 0 (on or off)
-        :type value: int
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :param init: Init device first (only for remote_on())
-        :type init: bool
+        Activates remote mode on device
 
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+        init : bool
+            if True, initialize the output.
         """
-        self.logger.debug("send_remote({})".format(output_num))
 
-        self._check_outputs(output_num)
-
-        REMOTE_MSG[1] = output_num
-        REMOTE_MSG[4] = value
-
-        self.__send_msg(REMOTE_MSG, 'remote on')
+        self._send_remote(self.REMOTE_ON, output_num, init)
 
-        if init:
-            self._init_device(output_num)
-
-    def _send_output(self, value: int, output_num: int):
-        """
-        :brief Turn on or off power output on device
-        :param value: 1 or 0 (On or Off)
-        :type value: int
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Device return message/ack
-        :rtype: byte str
+    def remote_off(self, output_num: int = 0):
         """
-        self._check_outputs(output_num)
+        Deactivates remote mode on device
 
-        OUTPUT_MSG[1] = output_num
-        OUTPUT_MSG[4] = value
-
-        self.__send_msg(OUTPUT_MSG, 'output on')
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
 
-    def remote_on(self, output_num: int = 0, init: bool = True):
         """
-        :brief Activates remote mode on device
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :param init: if True, initialize the output.
-        :type init: bool
-        :return: Device return message/ack
-        :rtype: byte str
-        """
-        self._send_remote(0x10, output_num, init)
 
-    def remote_off(self, output_num: int = 0):
-        """
-        :brief Deactivates remote mode on device
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Device return message/ack
-        :rtype: byte str
-        """
         if not self.__output_state[output_num]["remote on"]:
             self.logger.debug("Remote already off")
             return
-        self._send_remote(0x00, output_num, False)
+        self._send_remote(self.REMOTE_OFF, output_num, False)
 
     def get_nominal_voltage(self, output_num: int = 0, update: bool = False) -> float:
         """
         Get nominal voltage from device.
 
         Parameters
         ----------
         output_num : int
-            Output index
+            Output number for multi output devices (e.g. PS 2342-10B) int
+
         update : bool
-            Update nom. values. If true, get it from PSU. Otherwise use cached value.
+            Update nom. values. If true, get it from PSU. Otherwise, use cached value.
 
         Returns
         -------
         float
-            Nominal voltage
+            Nominal voltage in V
         """
 
-        if not self.__nom_voltage or update:
-            self.__nom_voltage = self.__get_float(OBJ_NOM_U, output_num)[0]
-            self.logger.debug(f"Get from PSU nom voltage: {self.__nom_voltage}")
-        return self.__nom_voltage
+        if not self.__quantities.nom_voltage or update:
+            self.__quantities.nom_voltage = self.__get_float(Objects.NOM_U, output_num)[0]
+            self.logger.debug("Get from PSU nom voltage: %f", self.__quantities.nom_voltage)
+        return self.__quantities.nom_voltage
 
     def get_nominal_current(self, output_num: int = 0, update: bool = False) -> float:
         """
         Get nominal current from device.
 
         Parameters
         ----------
         output_num : int
-            Output index
+            Output number for multi output devices (e.g. PS 2342-10B) int
+
         update : bool
-            Update nom. values. If true, get it from PSU. Otherwise use cached value.
+            Update nom. values. If true, get it from PSU. Otherwise, use cached value.
 
         Returns
         -------
         float
-            Nominal current
+            Nominal current in A
         """
-        if not self.__nom_current or update:
-            self.__nom_current = self.__get_float(OBJ_NOM_I, output_num)[0]
-            self.logger.debug(f"Get from PSU nom current: {self.__nom_current}")
-        return self.__nom_current
+        if not self.__quantities.nom_current or update:
+            self.__quantities.nom_current = self.__get_float(Objects.NOM_I, output_num)[0]
+            self.logger.debug("Get from PSU nom current: %f", self.__quantities.nom_current)
+        return self.__quantities.nom_current
 
     def get_nominal_power(self, output_num: int = 0, update: bool = False) -> float:
         """
         Get nominal power from device.
 
         Parameters
         ----------
         output_num : int
-            Output index
+            Output number for multi output devices (e.g. PS 2342-10B) int
+
         update : bool
-            Update nom. values. If true, get it from PSU. Otherwise use cached value.
+            Update nom. values. If true, get it from PSU. Otherwise, use cached value.
 
         Returns
         -------
         float
-            Nominal power
+            Nominal power in W
         """
-        if not self.__nom_power or update:
-            self.__nom_power = self.__get_float(OBJ_NOM_P, output_num)[0]
-            self.logger.debug(f"Get from PSU nom power: {self.__nom_power}")
-        return self.__nom_power
+        if not self.__quantities.nom_power or update:
+            self.__quantities.nom_power = self.__get_float(Objects.NOM_P, output_num)[0]
+            self.logger.debug("Get from PSU nom power: %f", self.__quantities.nom_power)
+        return self.__quantities.nom_power
 
     def get_nominal_values(self, output_num: int = 0, update: bool = False) -> (float, float, float):
         """
         Get nominal voltage, current and power from device.
 
         Parameters
         ----------
         output_num : int
-            Output index
+            Output number for multi output devices (e.g. PS 2342-10B) int
+
         update : bool
-            Update nom. values. If true, get it from PSU. Otherwise use cached value.
+            Update nom. values. If true, get it from PSU. Otherwise, use cached value.
 
         Returns
         -------
         (float, float, float)
             Voltage, Current, Power
         """
         self.get_nominal_voltage(output_num, update)
         self.get_nominal_current(output_num, update)
         self.get_nominal_power(output_num, update)
-        self.logger.debug(f"Nom Values: U: {self.__nom_voltage}, I: {self.__nom_current}, P: {self.__nom_power}")
-        return self.__nom_voltage, self.__nom_current, self.__nom_power
+        self.logger.debug("Nom Values: U: %f, I: %f, P: %f",
+                          self.__quantities.nom_voltage, self.__quantities.nom_current, self.__quantities.nom_power)
+        return self.__quantities.nom_voltage, self.__quantities.nom_current, self.__quantities.nom_power
 
     def set_voltage(self, voltage: Union[int, float], output_num: int = 0) -> float:
         """
-        :brief: Set output voltage on device
-        :param voltage: desired output voltage in V
-        :type voltage: int/float
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Device return message
-        :rtype: byte str
+        Set output voltage on <output_num>.
+        If requested voltage exceeds nominal voltage, it will set it to the nominal value.
+        If requested voltage and the current exceeds nominal power, it will respect the current value
+        and calculates the maximum possible voltage: set_voltage = nominal_power / actual_current.
+
+        Important: If you want to have maximum voltage, set voltage before current.
+
+        Parameters
+        ----------
+        voltage : Union[int, float]
+            Requested voltage in Volt
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            Actual set voltage in V
         """
+        if not isinstance(voltage, (int, float)):
+            raise ExceptionPSU("Voltage is not a number")
+
         # Calculate actual possible maximum current depending on maximum output power
         set_voltage = voltage
-        if set_voltage > self.__nom_voltage:
-            set_voltage = self.__nom_voltage
+        if set_voltage > self.__quantities.nom_voltage:
+            set_voltage = self.__quantities.nom_voltage
         try:
-            if set_voltage > self.__nom_power / self.__max_current:
-                set_voltage = self.__nom_power / self.__max_current
-                self.logger.info('Set voltage to {:.2f} V due to maximum power of {:.2f} W'.format(set_voltage, self.__nom_power))
+            if set_voltage > self.__quantities.nom_power / self.__quantities.max_current:
+                set_voltage = self.__quantities.nom_power / self.__quantities.max_current
+                self.logger.info(f'Set voltage to {set_voltage:.2f} V '
+                                 f'due to maximum power of {self.__quantities.nom_power:.2f} W')
         except ZeroDivisionError:
             pass
 
-        self.__act_voltage = float(set_voltage)
-        self.__set_value(set_voltage, self.__nom_voltage, OBJ_SET_U, output_num)
-        return self.__act_voltage
+        self.__quantities.act_voltage = float(set_voltage)
+        self.__set_value(set_voltage, self.__quantities.nom_voltage, Objects.SET_U, output_num)
+        return self.__quantities.act_voltage
 
     def set_current(self, current: Union[int, float], output_num: int = 0) -> float:
         """
-        :brief: Set maximum output current on device
-        :param current: desired output current in A
-        :type current: int/float
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Device return message
-        :rtype: byte str
+        Set output current on <output_num>.
+        If requested current exceeds nominal current, it will set it to the nominal value.
+        If requested current and the current voltage exceeds nominal power, it will respect the voltage value
+        and calculates the maximum possible current: set_current = nominal_power / actual_voltage
+
+        Important: If you want to have maximum current, set current before voltage.
+
+        Parameters
+        ----------
+        current : Union[int, float]
+            Requested current value in A
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            Actual set current in A
         """
+        if not isinstance(current, (int, float)):
+            raise ExceptionPSU("Current is not a number")
+
         # Calculate actual possible maximum current depending on maximum output power
         set_current = current
-        if set_current > self.__nom_current:
-            set_current = self.__nom_current
+        if set_current > self.__quantities.nom_current:
+            set_current = self.__quantities.nom_current
         try:
-            if set_current > self.__nom_power / self.__act_voltage:
-                set_current = self.__nom_power / self.__act_voltage
-                self.logger.info(f'Set current to {set_current:.2f} A due to maximum power of {self.__nom_power:.2f} W and current voltage of {self.__act_voltage:.2f} V')
+            if set_current > self.__quantities.nom_power / self.__quantities.act_voltage:
+                set_current = self.__quantities.nom_power / self.__quantities.act_voltage
+                self.logger.info(f'Set current to {set_current:.2f} A '
+                                 f'due to maximum power of {self.__quantities.nom_power:.2f} W '
+                                 f'and current voltage of {self.__quantities.act_voltage:.2f} V')
         except ZeroDivisionError:
             pass
 
-        self.__max_current = float(set_current)
-        self.__set_value(set_current, self.__nom_current, OBJ_SET_I, output_num)
-        return self.__max_current
+        self.__quantities.max_current = float(set_current)
+        self.__set_value(set_current, self.__quantities.nom_current, Objects.SET_I, output_num)
+        return self.__quantities.max_current
 
     def get_voltage(self, output_num: int = 0) -> float:
         """
-        :brief: Get current output voltage from device
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Voltage in V
-        :rtype: float
+        Get current output voltage from <output_num>
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            Voltage in Volt
         """
         self._check_outputs(output_num)
 
-        if self.__nom_voltage <= 0.0:
+        if self.__quantities.nom_voltage <= 0.0:
             self.get_nominal_voltage(output_num)
 
         status = self.get_status()
         if status:
             return status[output_num]['act voltage']
         self.logger.debug("Warning: Status is empty")
         return 0.0
 
     def get_current(self, output_num: int = 0) -> float:
         """
-        :brief: Get current of output_num
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Current in A
-        :rtype: float
+        Get current of <output_num>
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            Current in Ampere
         """
         self._check_outputs(output_num)
 
-        if self.__nom_current <= 0.0:
+        if self.__quantities.nom_current <= 0.0:
             self.get_nominal_current(output_num)
 
         status = self.get_status()
         if status:
             return status[output_num]['act current']
         self.logger.debug("Warning: Status is empty")
         return 0.0
 
     def get_power(self, output_num: int = 0) -> float:
         """
-        :brief: Get power of output_num
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: Power in W
-        :rtype: float
+        Get power of <output_num>
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            Power in Watt
         """
         self._check_outputs(output_num)
 
         status = self.get_status()
-        return round(status[output_num]['act voltage'] * status[output_num]['act current'], 3)
+        return round(status[output_num]['act voltage'] * status[output_num]['act current'], self.DECIMAL_PLACES)
 
-    def output_on(self, output_num: int = 0):
-        """
-        :brief Turn on power output on device
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
+    def output_on(self, output_num: int = 0, all_outputs: bool = False):
         """
-        self._send_output(1, output_num)
+        Turn on power output on device
 
-    def output_off(self, output_num: int = 0):
-        """
-        :brief Turn off power output on device
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+        all_outputs : bool
+            If true, turn all outputs off (for multi-port devices)
+        """
+        if all_outputs:
+            for i in range(self.desc['controllable_outputs']):
+                self._send_output(self.OUTPUT_ON, i)
+        else:
+            self._send_output(self.OUTPUT_ON, output_num)
+
+    def output_off(self, output_num: int = 0, all_outputs: bool = False):
         """
-        self._send_output(0, output_num)
+        Turn off power output on device
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+        all_outputs : bool
+            If true, turn all outputs off (for multi-port devices)
+        """
+        if all_outputs:
+            for i in range(self.desc['controllable_outputs']):
+                self._send_output(self.OUTPUT_OFF, i)
+        else:
+            self._send_output(self.OUTPUT_OFF, output_num)
 
-    def set_ovp(self, voltage, output_num: int = 0):
+    def set_ovp(self, voltage: float, output_num: int = 0):
         """
-        :brief: Set Over Voltage Protection
-        :param voltage: desired OVP voltage
-        :type voltage: float/int
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
+        Set Over-voltage Protection
+
+        Parameters
+        ----------
+        voltage : float
+            Voltage value
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
         """
-        self.__set_value(voltage, self.__nom_voltage, OBJ_OVP_THRESHOLD, output_num)
+        self.__set_value(voltage, self.__quantities.nom_voltage, Objects.OVP_THRESHOLD, output_num)
 
-    def set_ocp(self, current, output_num: int = 0):
+    def set_ocp(self, current: float, output_num: int = 0):
         """
-        :brief: Set Over Current Protection
-        :param current: desired OCP current
-        :type current: float/int
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
+        Set Over-current Protection
+
+        Parameters
+        ----------
+        current : float
+            Current value
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
         """
-        self.__set_value(current, self.__nom_current, OBJ_OCP_THRESHOLD, output_num)
+        self.__set_value(current, self.__quantities.nom_current, Objects.OCP_THRESHOLD, output_num)
 
     def get_ovp(self, output_num: int = 0) -> float:
         """
-        :brief: Get Over Voltage Protection value
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: OVP value
-        :rtype: float
+        Get Over-voltage Protection value
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            OVP value
         """
-        val = self.__get_value(OBJ_OVP_THRESHOLD, 2, '>H', output_num)
+        val = self.__get_value(Objects.OVP_THRESHOLD, output_num)
         return self._calculate_value(val[0], self.__nom_voltage)
 
     def get_ocp(self, output_num: int = 0) -> float:
         """
-        :brief: Get Over Current Protection value
-        :param output_num: Output number for multi output devices (e.g. PS 2342-10B)
-        :type output_num: int
-        :return: OCP value
-        :rtype: float
+        Get Over-current Protection value
+
+        Parameters
+        ----------
+        output_num : int
+            Output number for multi output devices (e.g. PS 2342-10B)
+
+        Returns
+        -------
+        float
+            OCP value
+
         """
-        val = self.__get_value(OBJ_OCP_THRESHOLD, 2, '>H', output_num)
+        val = self.__get_value(Objects.OCP_THRESHOLD, output_num)
         return self._calculate_value(val[0], self.__nom_current)
 
     def reset_error(self, output_num: int = 0):
         """
         Reset error (OVP, OCP, OPP, OTP).
         Resetting error turns off all outputs.
 
         Parameters
         ----------
         output_num : int
-            Output index
+            Output number for multi output devices (e.g. PS 2342-10B)
         """
 
-        ACKNOWLEDGE_ALARM[1] = output_num
+        ACKNOWLEDGE_ALARM[IDX_DN] = output_num
         self.__send_msg(ACKNOWLEDGE_ALARM)
 
     def tracking_on(self):
         """
         Turn tracking on. If tracking is on, output 2 control is disable and output 1 controls also output 2
 
         Raises
@@ -928,18 +1149,18 @@
             ExceptionPSU: If user tries to turn on tracking on single output PSU.
         """
         if self.desc["controllable_outputs"] == 1:
             raise ExceptionPSU("Tracking is only available on Triple Output PSUs")
 
         self.__send_msg(TRACKING_ON)
         # Set status manual, because we have to do it for both outputs
-        for o in range(self.desc["controllable_outputs"]):
-            self.__output_state[o]["tracking active"] = True
+        for idx in range(self.desc["controllable_outputs"]):
+            self.__output_state[idx]["tracking active"] = True
 
     def tracking_off(self):
         """
         Turn tracking off.
         """
         self.__send_msg(TRACKING_OFF)
         # Set status manual, because we have to do it for both outputs
-        for o in range(self.desc["controllable_outputs"]):
-            self.__output_state[o]["tracking active"] = False
+        for idx in range(self.desc["controllable_outputs"]):
+            self.__output_state[idx]["tracking active"] = False
```

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite/sanssouci/sanssouci.py` & `somanet_test_suite-1.1.2/src/somanet_test_suite/sanssouci/sanssouci.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import threading
 import time
 from typing import Callable
 from enum import Enum, unique
 
 from ..daq.daq_labjack import DAQLabJack
 
+
 @unique
 class Encoders(Enum):
     HALL = 0
     QEI = 1
 
 
 class DAQCallback:
```

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/PKG-INFO` & `somanet_test_suite-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,280 +1,281 @@
-Metadata-Version: 1.1
-Name: somanet-test-suite
-Version: 1.0.1
+Metadata-Version: 2.1
+Name: somanet_test_suite
+Version: 1.1.2
 Summary: A collection of different scripts and drivers (PSU, EtherCAT, Labjack,...)
-Home-page: UNKNOWN
 Author: Synapticon GmbH
 Author-email: hstroetgen@synapticon.com
 License: MIT
-Description: SOMANET Test Suite
-        ==================
-        
-        All modules to make successful and complete testing of SOMANET modules possible.
-        
-        Even though this suite is written for Linux, at least the Elektronik Automation Power Supply Driver also runs under Windows.
-        
-        Installation
-        ------------
-        
-        1) Install non-python tools (only Linux)
-            ``sudo ./install.sh -a -m <MAC_OF_ETHERCAT_INTERFACE>``
-        
-            This will install:
-                - IgH EtherCAT Master
-                - UDEV rules for power supplies
-                - LabJack driver and Kipling
-                - SOEM EtherCAT Master
-        
-            If one of these tools are already installed, the script will skip the installation
-            and continue with the next tool.
-            Call "-h" to show the help text.
-        
-        2) Install python script
-            ``python setup.py install``
-        
-        
-        Usage
-        -----
-        
-        1. PSU
-        ^^^^^^
-        Import module
-        """""""""""""
-            ``import somanet_test_suite as sts``
-        
-        Create object
-        """""""""""""
-        To connect to a specific PSU, you can call
-        
-        Linux: ``psu = sts.PsuEA(comport='ttyACM0')`` or ``psu = sts.PsuEA(comport='usb-EA_Elektro-Automatik_PS_2042-10B_2815450332-if00')``
-        
-        Windows: ``psu = sts.PsuEA(comport='COM1')`` or as com port description: ``psu = sts.PsuEA(comport='PS 2000 B')``
-        
-        If you added the device rule and you connected only one PSU, there is no need to provide a device name:
-        
-            ``psu = sts.PsuEA()``
-        
-        Also possible is:
-        
-            ``psu = sts.PsuEA(comport='ea-ps-20xx-xx-0')``
-        
-        | If there is more then one PSU connected to the host, the script will connect to the first device found.
-        | It is also possible to take the S/N written on the back of the PSU and call:
-        
-            ``psu = sts.PsuEA(sn='0123456789')``
-        
-        or to use the device designator:
-        
-            ``psu = sts.PsuEA(desi='PS 2142-10B')``
-        
-        
-        Dis/connect to power supply for controlling
-        """""""""""""""""""""""""""""""""""""""""""
-            ``psu.remote_on()``
-        
-            ``psu.remote_off()``
-        
-        For multi output devices most functions provide an additional output argument:
-        
-            ``psu.remote_on(output_num=0)``
-        
-            ``psu.remote_on(output_num=1)``
-        
-        | It's only necessary to call ``remote_on()``, when you want to control the PSU.
-        | If you just want to read device information, you don't need to.
-        
-        Power on and off output
-        """"""""""""""""""""""""""
-            ``psu.output_on()``
-        
-            ``psu.output_off()``
-        
-        or
-        
-            ``psu.output_on(output_num=1)``
-        
-            ``psu.output_off(output_num=1)``
-        
-        Set parameters
-        """"""""""""""""""""""""""
-        Arguments can be int or float.
-        
-            ``psu.set_voltage(24, output_num=0)``
-        
-            ``psu.set_current(0.5, output_num=0)``
-        
-            ``psu.set_ovp(30, output_num=0)``
-        
-            ``psu.set_ocp(8, output_num=0)``
-        
-        The script will always set the maximum possible values in dependency of the nominal power.
-        
-        | For example:
-        | Nominal power = 160 W
-        | When you set the voltage to 40 V, it's not possible to set a higher current than 4 A (=160W/40V),
-        | regardless of the maximum current output of the device.
-        | If you want to set a higher current, you must first reduce the voltage.
-        
-        | Also this script treats voltage with a higher priority.
-        | It will decrease the current, if the maximum power is reached.
-        | For example:
-        | Nominal power = 160 W, set current = 10 A
-        | When you set the voltage to 32 V, it'll results in a maximum current of 5 A.
-        
-        
-        Get parameters
-        """"""""""""""""""""""""""
-        Return argument: float.
-        
-            ``psu.get_voltage(output_num: int)``
-        
-            ``psu.get_current(output_num: int)``
-        
-            ``psu.get_power(output_num: int)``
-        
-        Maximum sampling rate is ~10 Hz.
-        
-        
-        Nominal values:
-        
-        If update is true, the value will be pulled directly from the device.
-        
-            ``psu.get_nominal_voltage(output_num: int, update: bool)``
-        
-            ``psu.get_nominal_current(output_num: int, update: bool)``
-        
-            ``psu.get_nominal_power(output_num: int, update: bool)``
-        
-        
-        Reset error
-        """""""""""""
-        If an overcurrent, overvoltage, overpower or overtemperature protection error happens,
-        you can reset the error with:
-        
-            ``psu.reset_error(output_num: int)``
-        
-        
-        Tracking
-        """""""""""""
-        (Only 3-port devices).
-        Tracking disables the controlling of output 2. Output 1 controls then also output 2.
-        
-            ``psu.tracking_on()``
-        
-            ``psu.tracking_off()``
-        
-        
-        Get status
-        """""""""""""
-        Return argument: dictionary
-        
-            ``psu.get_status(update: bool)``
-        
-        List of dictionary containing the following keys (index is output number):
-        
-        - 'output' (int)
-        - 'remote on' (bool)
-        - 'output on' (bool)
-        - 'controller state' ('CV', 'CC')
-        - 'tracking active' (bool)
-        - 'OVP activ' (bool)
-        - 'OCP activ' (bool)
-        - 'OPP activ' (bool)
-        - 'OTP activ' (bool)
-        - 'act voltage' (float)
-        - 'act current' (float)
-        
-        
-        Get device description
-        """"""""""""""""""""""""""
-        Return argument: tuple (name, SN)
-        
-            ``psu.get_device_description(update : bool)``
-        
-        
-        Close connection
-        """"""""""""""""""""""""""
-        To close the connection, call:
-        
-            ``psu.close()``
-        
-        This will just stop the communication, the PSU outputs will remain in their current states.
-        
-        
-        
-        2. SANSSOUCI - So(manet) Se(nsor) Si(mulator)
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        A framework to simulate different sensors (Hall, QEI, ...).
-        Currently only velocity is supported for Hall and QEI.
-        
-        Preperation
-        """"""""""""""""""""""""""
-        What you need:
-         - LabJack
-         - SN75174 Differential Line Driver (for RS-422 communication and as level shifter 3.3V -> 5V)
-        
-        Connection
-        """"""""""""""""""""""""""
-        See also: https://doc.synapticon.com/hardware/drive/drive_1000/d3/docs/index.html#encoder-port-1
-        
-        +--------------+------------------+
-        | Pin SN75174  | Encoder/Labjack  |
-        +==============+==================+
-        | 1            | LJ: FIO0         |
-        +--------------+------------------+
-        | 2            | A+               |
-        +--------------+------------------+
-        | 3            | A-               |
-        +--------------+------------------+
-        | 4            | Connect with     |
-        |              | 10kOhm to Vcc    |
-        |              | or NC            |
-        +--------------+------------------+
-        | 5            | B-               |
-        +--------------+------------------+
-        | 6            | B+               |
-        +--------------+------------------+
-        | 7            | LJ: FIO01        |
-        +--------------+------------------+
-        | 8            | GND of LJ and    |
-        |              | Encoder          |
-        +--------------+------------------+
-        | 9            | LJ: FIO2         |
-        +--------------+------------------+
-        | 10           | I+               |
-        +--------------+------------------+
-        | 11           | I-               |
-        +--------------+------------------+
-        | 12           | Connect with     |
-        |              | 10kOhm to Vcc    |
-        |              | or NC            |
-        +--------------+------------------+
-        | 13           | N.C.             |
-        +--------------+------------------+
-        | 14           | N.C.             |
-        +--------------+------------------+
-        | 15           | N.C.             |
-        +--------------+------------------+
-        | 16           | Vcc (5V)         |
-        +--------------+------------------+
-        
-        Usage
-        """"""""""""""""""""""""""
-        
-        **Hall**
-        
-            ``sensor = Sanssouci(printer.write, 'HALL', pole_pairs=7)``
-        
-            ``sensor.set_velocity(20)``
-        
-        **QEI**
-        
-            ``sensor = Sanssouci(printer.write, 'QEI', resolution=100)``
-        
-            ``sensor.set_velocity(20)``
-        
-Keywords: power supply unit,psu,daq,Labjack,Elektronik-Automation,EtherCAT,IgH,Synapticon
-Platform: UNKNOWN
+Keywords: power supply unit,psu,daq,Labjack,Elektro-Automation,EtherCAT,IgH,Synapticon,CANopen,CANSOEM
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: System :: Hardware :: Hardware Drivers
+Requires-Python: >=3.6
+License-File: LICENSE
+
+SOMANET Test Suite
+==================
+
+All modules to make successful and complete testing of SOMANET modules possible.
+
+Even though this suite is written for Linux, at least the Elektronik Automation Power Supply Driver also runs under Windows.
+
+Installation
+------------
+
+1) Install non-python tools (only Linux)
+    ``sudo ./install.sh -a -m <MAC_OF_ETHERCAT_INTERFACE>``
+
+    This will install:
+        - IgH EtherCAT Master
+        - UDEV rules for power supplies
+        - LabJack driver and Kipling
+        - SOEM EtherCAT Master
+
+    If one of these tools are already installed, the script will skip the installation
+    and continue with the next tool.
+    Call "-h" to show the help text.
+
+2) Install python script
+    ``python setup.py install``
+
+
+Usage
+-----
+
+1. PSU
+^^^^^^
+Import module
+"""""""""""""
+    ``import somanet_test_suite as sts``
+
+Create object
+"""""""""""""
+To connect to a specific PSU, you can call
+
+Linux: ``psu = sts.PsuEA(comport='ttyACM0')`` or ``psu = sts.PsuEA(comport='usb-EA_Elektro-Automatik_PS_2042-10B_2815450332-if00')``
+
+Windows: ``psu = sts.PsuEA(comport='COM1')`` or as com port description: ``psu = sts.PsuEA(comport='PS 2000 B')``
+
+If you added the device rule and you connected only one PSU, there is no need to provide a device name:
+
+    ``psu = sts.PsuEA()``
+
+Also possible is:
+
+    ``psu = sts.PsuEA(comport='ea-ps-20xx-xx-0')``
+
+| If there is more then one PSU connected to the host, the script will connect to the first device found.
+| It is also possible to take the S/N written on the back of the PSU and call:
+
+    ``psu = sts.PsuEA(sn='0123456789')``
+
+or to use the device designator:
+
+    ``psu = sts.PsuEA(desi='PS 2142-10B')``
+
+
+Dis/connect to power supply for controlling
+"""""""""""""""""""""""""""""""""""""""""""
+    ``psu.remote_on()``
+
+    ``psu.remote_off()``
+
+For multi output devices most functions provide an additional output argument:
+
+    ``psu.remote_on(output_num=0)``
+
+    ``psu.remote_on(output_num=1)``
+
+| It's only necessary to call ``remote_on()``, when you want to control the PSU.
+| If you just want to read device information, you don't need to.
+
+Power on and off output
+""""""""""""""""""""""""""
+    ``psu.output_on()``
+
+    ``psu.output_off()``
+
+or
+
+    ``psu.output_on(output_num=1)``
+
+    ``psu.output_off(output_num=1)``
+
+Set parameters
+""""""""""""""""""""""""""
+Arguments can be int or float.
+
+    ``psu.set_voltage(24, output_num=0)``
+
+    ``psu.set_current(0.5, output_num=0)``
+
+    ``psu.set_ovp(30, output_num=0)``
+
+    ``psu.set_ocp(8, output_num=0)``
+
+The script will always set the maximum possible values in dependency of the nominal power.
+
+| For example:
+| Nominal power = 160 W
+| When you set the voltage to 40 V, it's not possible to set a higher current than 4 A (=160W/40V),
+| regardless of the maximum current output of the device.
+| If you want to set a higher current, you must first reduce the voltage.
+
+| Also this script treats voltage with a higher priority.
+| It will decrease the current, if the maximum power is reached.
+| For example:
+| Nominal power = 160 W, set current = 10 A
+| When you set the voltage to 32 V, it'll results in a maximum current of 5 A.
+
+
+Get parameters
+""""""""""""""""""""""""""
+Return argument: float.
+
+    ``psu.get_voltage(output_num: int)``
+
+    ``psu.get_current(output_num: int)``
+
+    ``psu.get_power(output_num: int)``
+
+Maximum sampling rate is ~10 Hz.
+
+
+Nominal values:
+
+If update is true, the value will be pulled directly from the device.
+
+    ``psu.get_nominal_voltage(output_num: int, update: bool)``
+
+    ``psu.get_nominal_current(output_num: int, update: bool)``
+
+    ``psu.get_nominal_power(output_num: int, update: bool)``
+
+
+Reset error
+"""""""""""""
+If an overcurrent, overvoltage, overpower or overtemperature protection error happens,
+you can reset the error with:
+
+    ``psu.reset_error(output_num: int)``
+
+
+Tracking
+"""""""""""""
+(Only 3-port devices).
+Tracking disables the controlling of output 2. Output 1 controls then also output 2.
+
+    ``psu.tracking_on()``
+
+    ``psu.tracking_off()``
+
+
+Get status
+"""""""""""""
+Return argument: dictionary
+
+    ``psu.get_status(update: bool)``
+
+List of dictionary containing the following keys (index is output number):
+
+- 'output' (int)
+- 'remote on' (bool)
+- 'output on' (bool)
+- 'controller state' ('CV', 'CC')
+- 'tracking active' (bool)
+- 'OVP activ' (bool)
+- 'OCP activ' (bool)
+- 'OPP activ' (bool)
+- 'OTP activ' (bool)
+- 'act voltage' (float)
+- 'act current' (float)
+
+
+Get device description
+""""""""""""""""""""""""""
+Return argument: tuple (name, SN)
+
+    ``psu.get_device_description(update : bool)``
+
+
+Close connection
+""""""""""""""""""""""""""
+To close the connection, call:
+
+    ``psu.close()``
+
+This will just stop the communication, the PSU outputs will remain in their current states.
+
+
+
+2. SANSSOUCI - So(manet) Se(nsor) Si(mulator)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+A framework to simulate different sensors (Hall, QEI, ...).
+Currently only velocity is supported for Hall and QEI.
+
+Preperation
+""""""""""""""""""""""""""
+What you need:
+ - LabJack
+ - SN75174 Differential Line Driver (for RS-422 communication and as level shifter 3.3V -> 5V)
+
+Connection
+""""""""""""""""""""""""""
+See also: https://doc.synapticon.com/hardware/drive/drive_1000/d3/docs/index.html#encoder-port-1
+
++--------------+------------------+
+| Pin SN75174  | Encoder/Labjack  |
++==============+==================+
+| 1            | LJ: FIO0         |
++--------------+------------------+
+| 2            | A+               |
++--------------+------------------+
+| 3            | A-               |
++--------------+------------------+
+| 4            | Connect with     |
+|              | 10kOhm to Vcc    |
+|              | or NC            |
++--------------+------------------+
+| 5            | B-               |
++--------------+------------------+
+| 6            | B+               |
++--------------+------------------+
+| 7            | LJ: FIO01        |
++--------------+------------------+
+| 8            | GND of LJ and    |
+|              | Encoder          |
++--------------+------------------+
+| 9            | LJ: FIO2         |
++--------------+------------------+
+| 10           | I+               |
++--------------+------------------+
+| 11           | I-               |
++--------------+------------------+
+| 12           | Connect with     |
+|              | 10kOhm to Vcc    |
+|              | or NC            |
++--------------+------------------+
+| 13           | N.C.             |
++--------------+------------------+
+| 14           | N.C.             |
++--------------+------------------+
+| 15           | N.C.             |
++--------------+------------------+
+| 16           | Vcc (5V)         |
++--------------+------------------+
+
+Usage
+""""""""""""""""""""""""""
+
+**Hall**
+
+    ``sensor = Sanssouci(printer.write, 'HALL', pole_pairs=7)``
+
+    ``sensor.set_velocity(20)``
+
+**QEI**
+
+    ``sensor = Sanssouci(printer.write, 'QEI', resolution=100)``
+
+    ``sensor.set_velocity(20)``
```

### Comparing `somanet_test_suite-1.0.1/src/somanet_test_suite.egg-info/SOURCES.txt` & `somanet_test_suite-1.1.2/src/somanet_test_suite.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,32 @@
 setup.py
 src/somanet_test_suite/__init__.py
 src/somanet_test_suite.egg-info/PKG-INFO
 src/somanet_test_suite.egg-info/SOURCES.txt
 src/somanet_test_suite.egg-info/dependency_links.txt
 src/somanet_test_suite.egg-info/requires.txt
 src/somanet_test_suite.egg-info/top_level.txt
+src/somanet_test_suite/communication/BaseCANOpen.py
+src/somanet_test_suite/communication/BaseEtherCAT.py
+src/somanet_test_suite/communication/BaseFileSystem.py
 src/somanet_test_suite/communication/__init__.py
-src/somanet_test_suite/communication/ethercat/EtherCATMaster.py
+src/somanet_test_suite/communication/esi.py
+src/somanet_test_suite/communication/can/CANMaster.py
+src/somanet_test_suite/communication/can/__init__.py
+src/somanet_test_suite/communication/ethercat/IgHMaster.py
 src/somanet_test_suite/communication/ethercat/SOEMMaster.py
 src/somanet_test_suite/communication/ethercat/__init__.py
 src/somanet_test_suite/communication/uart/__init__.py
+src/somanet_test_suite/communication/uart/somanet_bootloader_uart.py
 src/somanet_test_suite/communication/uart/uart.py
 src/somanet_test_suite/daq/__init__.py
 src/somanet_test_suite/daq/daq_labjack.py
 src/somanet_test_suite/hardware_description_builder/__init__.py
 src/somanet_test_suite/hardware_description_builder/build_hardware_description_json.py
 src/somanet_test_suite/hardware_description_builder/dataformat.py
 src/somanet_test_suite/hardware_description_builder/somanet_hw_description_builder
 src/somanet_test_suite/psu/99-ea-psu.rules
 src/somanet_test_suite/psu/__init__.py
+src/somanet_test_suite/psu/psu_controller
 src/somanet_test_suite/psu/psu_ea.py
 src/somanet_test_suite/sanssouci/__init__.py
 src/somanet_test_suite/sanssouci/sanssouci.py
```

