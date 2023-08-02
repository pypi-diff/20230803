# Comparing `tmp/pytesdaq-0.3.4.tar.gz` & `tmp/pytesdaq-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesdaq-0.3.4.tar", last modified: Fri Jul 28 18:51:51 2023, max compression
+gzip compressed data, was "pytesdaq-0.3.6.tar", last modified: Wed Aug  2 22:16:41 2023, max compression
```

## Comparing `pytesdaq-0.3.4.tar` & `pytesdaq-0.3.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.292005 pytesdaq-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 18:51:51.292005 pytesdaq-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/analyzer/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/config/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27052 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/daq.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/nidaqtask.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/polaris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/display/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/display/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    78796 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/feb/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/feb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/feb/feb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/imacrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/macrtmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/keysight/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/keysight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/keysight/keysight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/lakeshore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/instruments/magnicon/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/magnicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/magnicon/magnicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/instruments/niadc/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/niadc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/niadc/nidevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/filter_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    70229 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63818 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/_process_iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/scope/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/scope/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/scope/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/sequencer/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45457 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:51:51.292005 pytesdaq-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.892578 pytesdaq-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 22:16:41.892578 pytesdaq-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.884577 pytesdaq-0.3.6/pytesdaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.884577 pytesdaq-0.3.6/pytesdaq/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/analyzer/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.884577 pytesdaq-0.3.6/pytesdaq/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27396 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/daq/daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/daq/nidaqtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/daq/polaris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/display/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/display/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79179 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/feb/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/feb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/feb/feb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/imacrt/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/imacrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/imacrt/imacrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/imacrt/macrtmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/keysight/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/keysight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/keysight/keysight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/lakeshore/lakeshore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/magnicon/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/magnicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/magnicon/magnicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/instruments/niadc/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/niadc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/instruments/niadc/nidevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/io/filter_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70229 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/io/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.888578 pytesdaq-0.3.6/pytesdaq/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63818 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/processing/_iv_didv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/processing/_iv_didv_tools_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/processing/_process_iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/processing/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.892578 pytesdaq-0.3.6/pytesdaq/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/scope/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/scope/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.892578 pytesdaq-0.3.6/pytesdaq/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/sequencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45457 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/sequencer/iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/sequencer/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/sequencer/tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.892578 pytesdaq-0.3.6/pytesdaq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/pytesdaq/utils/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:16:41.884577 pytesdaq-0.3.6/pytesdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 22:16:41.000000 pytesdaq-0.3.6/pytesdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 22:16:41.000000 pytesdaq-0.3.6/pytesdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:16:41.000000 pytesdaq-0.3.6/pytesdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:16:41.000000 pytesdaq-0.3.6/pytesdaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 22:16:41.000000 pytesdaq-0.3.6/pytesdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:16:41.000000 pytesdaq-0.3.6/pytesdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:16:41.892578 pytesdaq-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 22:16:32.000000 pytesdaq-0.3.6/setup.py
```

### Comparing `pytesdaq-0.3.4/PKG-INFO` & `pytesdaq-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.4
+Version: 0.3.6
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.3.4/README.md` & `pytesdaq-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/analyzer/analyzer.py` & `pytesdaq-0.3.6/pytesdaq/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/config/settings.py` & `pytesdaq-0.3.6/pytesdaq/config/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,28 +169,41 @@
 
         return output_setup 
 
 
   
     def get_squid_controller(self):
         """
-        get SQUID/TES controller device name
+        get SQUID controller device name
         
         Returns:
            str - no type conversion happens here!
         """
-        controller=str()
+        controller = str()
         try:
             controller =  self._get_setting('setup','squid_controller')
         except:
             pass
     
         return controller
 
-
+    def get_tes_controller(self):
+        """
+        get TES controller device name
+        
+        Returns:
+           str - no type conversion happens here!
+        """
+        controller = str()
+        try:
+            controller =  self._get_setting('setup','tes_controller')
+        except:
+            pass
+    
+        return controller
 
 
     def get_temperature_controllers(self):
         """
         get temperature controller device names
         (comma separated)
```

### Comparing `pytesdaq-0.3.4/pytesdaq/daq/daq.py` & `pytesdaq-0.3.6/pytesdaq/daq/daq.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/daq/nidaqtask.py` & `pytesdaq-0.3.6/pytesdaq/daq/nidaqtask.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/daq/polaris.py` & `pytesdaq-0.3.6/pytesdaq/daq/polaris.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/display/series.py` & `pytesdaq-0.3.6/pytesdaq/display/series.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/communication.py` & `pytesdaq-0.3.6/pytesdaq/instruments/communication.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/control.py` & `pytesdaq-0.3.6/pytesdaq/instruments/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,24 +36,30 @@
         # config
         self._setup_file = setup_file
         self._config = settings.Config(setup_file=setup_file)
       
         # signal connection map
         self._connection_table = self._config.get_adc_connections()
             
-        # TES/SQUID Controller
+        # SQUID Controller
         self._squid_controller_name = self._config.get_squid_controller()
-        self._readout_inst = None
-
+        self._squid_controller_inst = None
+        
+        # SQUID Controller
+        self._tes_controller_name = self._config.get_tes_controller()
+        self._tes_controller_inst = None
+        
         # Signal Generator Controller
         self._signal_generator_name = self._config.get_signal_generator()
         self._signal_generator_inst = None
         
         # Temperatuer controllers (multiple controller allowed)
-        self._temperature_controller_name_list = self._config.get_temperature_controllers()
+        self._temperature_controller_name_list = (
+            self._config.get_temperature_controllers()
+        )
         self._temperature_controller_insts = None
         self._resistance_channel_table = None
         self._heater_channel_table = None
         
         if not self._dummy_mode:
             self._connect_instruments()   
  
@@ -64,19 +70,20 @@
              self._redis_db = redis.RedisCore()
              self._redis_db.connect()
              
         # readback 
         self._enable_readback = self._config.enable_redis()
 
 
+        
+
     def __del__(self):
         """
         """
 
-
         # temperature controllers
         if self._temperature_controller_insts  is not None:
          for name, inst in self._temperature_controller_insts.items():
              inst.disconnect()
 
         
     @property
@@ -99,14 +106,18 @@
             self._read_from_redis=value
         
     @property
     def squid_controller_name(self):
         return self._squid_controller_name
 
     @property
+    def tes_controller_name(self):
+        return self._tes_controller_name
+    
+    @property
     def signal_generator_name(self):
         return self._signal_generator_name
 
     @property
     def temperature_controller_names(self):
         return self._temperature_controller_name_list
 
@@ -396,43 +407,44 @@
         
         
         
         if self._signal_generator_name == 'magnicon':
 
             # get readout controller ID and Channel (FIXME: Is it necessary)
             controller_id, controller_channel = (
-                connection_utils.get_controller_info(self._connection_table,
-                                                     tes_channel=tes_channel,
-                                                     detector_channel=detector_channel,
-                                                     adc_id=adc_id,
-                                                     adc_channel=adc_channel)
+                connection_utils.get_controller_info(
+                    self._connection_table,
+                    tes_channel=tes_channel,
+                    detector_channel=detector_channel,
+                    adc_id=adc_id,
+                    adc_channel=adc_channel)
             )
 
-
-                        
             mon_onoff = 'OFF'
             gen1_onoff = 'OFF'
             gen2_onoff = 'OFF'
             if signal_gen_num == 1:
                 gen1_onoff = on_off_flag.upper()
             else:
                 gen2_onoff = on_off_flag.upper()
 
 
             if gen1_onoff=='ON' or gen2_onoff=='ON':
                 mon_onoff = 'ON'
 
             rb_onoff1, rb_onoff, rb_mon_onoff = (
-                self._readout_inst.set_generator_onoff(controller_channel, 
-                                                       gen1_onoff, gen2_onoff, mon_onoff)
+                self._signal_generator_inst.set_generator_onoff(
+                    controller_channel, 
+                    gen1_onoff, gen2_onoff, mon_onoff)
             )
 
         else:
-            self._signal_generator_inst.set_generator_onoff(on_off_flag.lower(),
-                                                            source=signal_gen_num)
+            self._signal_generator_inst.set_generator_onoff(
+                on_off_flag.lower(),
+                source=signal_gen_num)
             
             
 
     
     def set_signal_gen_params(self, tes_channel=None,
                               detector_channel=None,
                               adc_id=None, adc_channel=None,
@@ -473,108 +485,104 @@
         # initialize readback values
         readback_amp = nan
         readback_freq = nan
 
         # magnicon
         if self._signal_generator_name == 'magnicon': 
 
-
-
             # get readout controller ID and Channel
             controller_id, controller_channel = (
                 connection_utils.get_controller_info(self._connection_table,
                                                      tes_channel=tes_channel,
                                                      detector_channel=detector_channel,
                                                      adc_id=adc_id,
                                                      adc_channel=adc_channel)
             )
-
-
-
-
             
             # convert some parameters
             source_magnicon = 'I'
             if source == 'feedback':
                 source_magnicon = 'Ib'
 
-
-
             readback_amp, readback_freq = (
-                self._readout_inst.set_generator_params(int(controller_channel), int(signal_gen_num), 
-                                                         float(frequency), source_magnicon, shape, 
-                                                         int(phase_shift), int(freq_div), half_pp_offset, 
-                                                         float(current))
-                )
+                self._signal_generator_inst.set_generator_params(
+                    int(controller_channel), int(signal_gen_num), 
+                    float(frequency), source_magnicon, shape, 
+                    int(phase_shift), int(freq_div), half_pp_offset, 
+                    float(current))
+            )
             
 
         # External function generator
         else:
 
-
             # shape
             if shape is not None:
                 if shape == 'sawtoothpos' or shape == 'sawtoothneg':
                     shape = 'ramp'
                 self._signal_generator_inst.set_shape(shape, source=signal_gen_num)
             
             # amplitude
             if voltage is None and current is not None:
                 resistance = float(self._config.get_signal_gen_tes_resistance())
                 voltage = resistance*current/1000
 
             if voltage is not None:
-                self._signal_generator_inst.set_amplitude(voltage, unit='mVpp',
-                                                          source=signal_gen_num)
+                self._signal_generator_inst.set_amplitude(
+                    voltage, unit='mVpp',
+                    source=signal_gen_num)
 
             # frequency
             if frequency is not None:
-                self._signal_generator_inst.set_frequency(frequency, unit='Hz',
-                                                          source=signal_gen_num)
-
+                self._signal_generator_inst.set_frequency(
+                    frequency, unit='Hz',
+                    source=signal_gen_num)
+                
 
             # offset
             if offset is not None:
-                self._signal_generator_inst.set_offset(offset, unit='mV', source=signal_gen_num)
+                self._signal_generator_inst.set_offset(
+                    offset, unit='mV', source=signal_gen_num)
 
 
                 
             # source
-            if source is not None and self._squid_controller_name == 'feb':
+            if source is not None:
 
-                
                 # get readout controller ID and Channel
                 controller_id, controller_channel = (
-                    connection_utils.get_controller_info(self._connection_table,
-                                                         tes_channel=tes_channel,
-                                                         detector_channel=detector_channel,
-                                                         adc_id=adc_id,
-                                                         adc_channel=adc_channel)
+                    connection_utils.get_controller_info(
+                        self._connection_table,
+                        tes_channel=tes_channel,
+                        detector_channel=detector_channel,
+                        adc_id=adc_id,
+                        adc_channel=adc_channel)
                 )
 
-
                 connect_to_tes = False
                 connect_to_feedback = False
                 
                 if source == 'tes':
                     connect_to_tes = True
                 if source == 'feedback':
                     connect_to_feedback = True
                     
-                self.connect_signal_gen_to_tes(connect_to_tes,
-                                               tes_channel=tes_channel,
-                                               detector_channel=detector_channel,
-                                               adc_id=adc_id,
-                                               adc_channel=adc_channel)
-                
-                self.connect_signal_gen_to_feedback(connect_to_feedback,
-                                                    tes_channel=tes_channel,
-                                                    detector_channel=detector_channel,
-                                                    adc_id=adc_id,
-                                                    adc_channel=adc_channel)
+                self.connect_signal_gen_to_tes(
+                    connect_to_tes,
+                    tes_channel=tes_channel,
+                    detector_channel=detector_channel,
+                    adc_id=adc_id,
+                    adc_channel=adc_channel)
+                
+                self.connect_signal_gen_to_feedback(
+                    connect_to_feedback,
+                    tes_channel=tes_channel,
+                    detector_channel=detector_channel,
+                    adc_id=adc_id,
+                    adc_channel=adc_channel)
                 
                             
             
             # phase shift, half_pp_offset, not implemented
                         
             
 
@@ -948,43 +956,50 @@
             print('ERROR getting signal generator connection')
             
         return is_connected
             
 
     
     def get_signal_gen_onoff(self, signal_gen_num=1, tes_channel=None,
-                             detector_channel=None, adc_id=None, adc_channel=None):
+                             detector_channel=None,
+                             adc_id=None, adc_channel=None):
 
         """
         Get signal gen state ("on"/"off")
         """
                    
 
         if self._dummy_mode:
             return "off"
             
         
         # get readout controller ID and Channel (FIXME: Is it necessary?)
-        controller_id, controller_channel = connection_utils.get_controller_info(self._connection_table,
-                                                                                 tes_channel=tes_channel,
-                                                                                 detector_channel=detector_channel,
-                                                                                 adc_id=adc_id,
-                                                                                 adc_channel=adc_channel)
+        controller_id, controller_channel = connection_utils.get_controller_info(
+            self._connection_table,
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id,
+            adc_channel=adc_channel)
         
 
         val = nan
         if self._signal_generator_name == 'magnicon':
-            gen1_onoff, gen2_onoff, mon_onoff = self._readout_inst.get_generator_onoff(controller_channel)
+            gen1_onoff, gen2_onoff, mon_onoff = (
+                self._squid_controller_inst.get_generator_onoff(
+                    controller_channel)
+                )
+            
             if signal_gen_num == 1:
                 val = gen1_onoff.lower()
             else:
                 val = gen2_onoff.lower()
 
         else:
-            val = self._signal_generator_inst.get_generator_onoff(source=signal_gen_num)
+            val = self._signal_generator_inst.get_generator_onoff(
+                source=signal_gen_num)
             
                         
 
         return val
 
         
 
@@ -992,15 +1007,16 @@
                          detector_channel=None, adc_id=None, adc_channel=None): 
 
         """
         Is signal generator on?
         Return: BOOL
         """
 
-        val = self.get_signal_gen_onoff(signal_gen_num=signal_gen_num, tes_channel=tes_channel,
+        val = self.get_signal_gen_onoff(signal_gen_num=signal_gen_num,
+                                        tes_channel=tes_channel,
                                         detector_channel=detector_channel, 
                                         adc_id=adc_id, adc_channel=adc_channel)
 
         val_bool = None
         if val == 'on':
             val_bool = True
         elif  val == 'off':
@@ -1048,34 +1064,36 @@
         
         # magnicon
         if self._signal_generator_name == 'magnicon':
 
 
             # get readout controller ID and Channel
             controller_id, controller_channel = (
-                connection_utils.get_controller_info(self._connection_table,
-                                                     tes_channel=tes_channel,
-                                                     detector_channel=detector_channel,
-                                                     adc_id=adc_id,
-                                                     adc_channel=adc_channel)
+                connection_utils.get_controller_info(
+                    self._connection_table,
+                    tes_channel=tes_channel,
+                    detector_channel=detector_channel,
+                    adc_id=adc_id,
+                    adc_channel=adc_channel)
             )
         
 
             if self._dummy_mode:
                 print('INFO: Getting signal generator #' + str(signal_gen_num) + ', ' + 
                       controller_id + ' channel ' + str(controller_channel))
                 return output_dict
             
             
             # convert some parameters
             source_magnicon = 'I'
            
             source, shape, freq, freq_div, shift, amp, offset = (
-                self._readout_inst.get_generator_params(controller_channel,
-                                                         signal_gen_num)
+                self._signal_generator_inst.get_generator_params(
+                    controller_channel,
+                    signal_gen_num)
             )
             
             # fill dictionary
             if source=='I':
                 output_dict['source'] = 'tes'
             elif source=='Ib':
                 output_dict['source'] = 'feedback'
@@ -1094,54 +1112,60 @@
 
         # external signal generator
         else:
 
             # signal generator parameter
             if not self._dummy_mode:
                 output_dict['voltage'] = float(
-                    self._signal_generator_inst.get_amplitude(source=signal_gen_num)
+                    self._signal_generator_inst.get_amplitude(
+                        source=signal_gen_num)
                 )
                 resistance = float(self._config.get_signal_gen_tes_resistance())
                 output_dict['current']  = float(output_dict['voltage']/resistance)
                 output_dict['frequency'] = float(
-                    self._signal_generator_inst.get_frequency(source=signal_gen_num)
+                    self._signal_generator_inst.get_frequency(
+                        source=signal_gen_num)
                 )
-                output_dict['shape'] = self._signal_generator_inst.get_shape(source=signal_gen_num)
+                output_dict['shape'] = self._signal_generator_inst.get_shape(
+                    source=signal_gen_num)
 
             # source
             if (is_channel_defined
                 and self._squid_controller_name=='feb'):
 
 
                 # get readout controller ID and Channel
                 controller_id, controller_channel = (
-                    connection_utils.get_controller_info(self._connection_table,
-                                                         tes_channel=tes_channel,
-                                                         detector_channel=detector_channel,
-                                                         adc_id=adc_id,
-                                                         adc_channel=adc_channel)
+                    connection_utils.get_controller_info(
+                        self._connection_table,
+                        tes_channel=tes_channel,
+                        detector_channel=detector_channel,
+                        adc_id=adc_id,
+                        adc_channel=adc_channel)
                 )
 
 
                 if self._dummy_mode:
                     print('INFO: Getting signal generator #' + str(signal_gen_num) + ', ' + 
                           controller_id + ' channel ' + str(controller_channel))
                     return output_dict
 
                 
                 is_connected_to_tes = (
-                    self.is_signal_gen_connected_to_tes(tes_channel=tes_channel,
-                                                        detector_channel=detector_channel,
-                                                        adc_id=adc_id, adc_channel=adc_channel)
+                    self.is_signal_gen_connected_to_tes(
+                        tes_channel=tes_channel,
+                        detector_channel=detector_channel,
+                        adc_id=adc_id, adc_channel=adc_channel)
                 )
 
                 is_connected_to_feedback = (
-                    self.is_signal_gen_connected_to_feedback(tes_channel=tes_channel,
-                                                             detector_channel=detector_channel,
-                                                             adc_id=adc_id, adc_channel=adc_channel)
+                    self.is_signal_gen_connected_to_feedback(
+                        tes_channel=tes_channel,
+                        detector_channel=detector_channel,
+                        adc_id=adc_id, adc_channel=adc_channel)
                 )
 
                 
                 if is_connected_to_tes and is_connected_to_feedback:
                     print('WARNING: Signal generator connected to both TES AND Feedback!')
                     
                 if is_connected_to_tes:
@@ -1168,19 +1192,19 @@
         
         """
         Is signal generator connected to TES line
         """
 
         is_connected = nan
         try:
-            is_connected = self._get_sensor_val('signal_gen_tes_connection',
-                                                tes_channel=tes_channel,
-                                                detector_channel=detector_channel,
-                                                adc_id=adc_id, adc_channel=adc_channel)
-            
+            is_connected = self._get_sensor_val(
+                'signal_gen_tes_connection',
+                tes_channel=tes_channel,
+                detector_channel=detector_channel,
+                adc_id=adc_id, adc_channel=adc_channel)
         except:
             print('ERROR getting signal generator connection')
             
         return is_connected
             
 
 
@@ -1197,18 +1221,19 @@
         feedback_resistance = nan
 
 
         # Magnicon: feedback resistance can be modifed and read
         if self._squid_controller_name == 'magnicon':
         
             try:
-                feedback_resistance = self._get_sensor_val('feedback_resistance',
-                                                           tes_channel=tes_channel,
-                                                           detector_channel=detector_channel,
-                                                           adc_id=adc_id, adc_channel=adc_channel)
+                feedback_resistance = self._get_sensor_val(
+                    'feedback_resistance',
+                    tes_channel=tes_channel,
+                    detector_channel=detector_channel,
+                    adc_id=adc_id, adc_channel=adc_channel)
             except:
                 print('ERROR getting feedback resistance')
 
             # convert from kOhms to Ohms
             feedback_resistance = feedback_resistance *1000
                 
         else:
@@ -1216,17 +1241,18 @@
             if (tes_channel is not None or  detector_channel is not None):
                 adc_id, adc_channel = connection_utils.get_adc_channel_info(
                     self._connection_table,
                     tes_channel=tes_channel,
                     detector_channel=detector_channel
                 )
             
-            detector_config = self._config.get_detector_config(adc_id=adc_id,
-                                                               adc_channel_list=[adc_channel])
-
+            detector_config = self._config.get_detector_config(
+                adc_id=adc_id,
+                adc_channel_list=[adc_channel])
+            
             if ('feedback_resistance' in  detector_config and
                 len(detector_config['feedback_resistance'])==1):
                 feedback_resistance = float(detector_config['feedback_resistance'][0])
                 
         
             
         return feedback_resistance
@@ -1247,17 +1273,18 @@
             adc_id, adc_channel = connection_utils.get_adc_channel_info(
                 self._connection_table,
                 tes_channel=tes_channel,
                 detector_channel=detector_channel
             )
 
         # get detector config
-        detector_config = self._config.get_detector_config(adc_id=adc_id,
-                                                           adc_channel_list=[adc_channel])
-
+        detector_config = self._config.get_detector_config(
+            adc_id=adc_id,
+            adc_channel_list=[adc_channel])
+        
         # extract shunt resistance
         if ('shunt_resistance' in  detector_config and
             len(detector_config['shunt_resistance'])==1):
             shunt_resistance = detector_config['shunt_resistance'][0]
                 
         return shunt_resistance
 
@@ -1277,17 +1304,18 @@
             adc_id, adc_channel = connection_utils.get_adc_channel_info(
                 self._connection_table,
                 tes_channel=tes_channel,
                 detector_channel=detector_channel
             )
 
         # get detector config
-        detector_config = self._config.get_detector_config(adc_id=adc_id,
-                                                           adc_channel_list=[adc_channel])
-
+        detector_config = self._config.get_detector_config(
+            adc_id=adc_id,
+            adc_channel_list=[adc_channel])
+        
         # extract shunt resistance
         if ('squid_turn_ratio' in  detector_config and
             len(detector_config['squid_turn_ratio'])==1):
             squid_turn_ratio = detector_config['squid_turn_ratio'][0]
                 
         return squid_turn_ratio
 
@@ -1299,34 +1327,37 @@
                                           adc_id=None, adc_channel=None):
         """
         get normalization to convert output volts to amps
         in close loop
         """
         
         # driver gain
-        output_total_gain = self.get_output_total_gain(tes_channel=tes_channel,
-                                                       detector_channel=detector_channel,
-                                                       adc_id=adc_id, adc_channel=adc_channel)
+        output_total_gain = self.get_output_total_gain(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
         
         
         # feedback resistance
-        feedback_resistance = self.get_feedback_resistance(tes_channel=tes_channel,
-                                                           detector_channel=detector_channel,
-                                                           adc_id=adc_id, adc_channel=adc_channel)
+        feedback_resistance = self.get_feedback_resistance(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
 
         if feedback_resistance == nan or feedback_resistance is None:
             print('ERROR: unable to find feedback resistance. It needs to be added in setup.ini file!')
             return None
         
         
         # squid loop turn ratio
-        squid_turn_ratio = self.get_squid_turn_ratio(tes_channel=tes_channel,
-                                                     detector_channel=detector_channel,
-                                                     adc_id=adc_id, adc_channel=adc_channel)
-     
+        squid_turn_ratio = self.get_squid_turn_ratio(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
+        
         if squid_turn_ratio == nan or squid_turn_ratio is None:
             print('ERROR: unable to find SQUID turn ratio. It needs to be added in setup.ini file!')
             return None
 
 
         # calculate normalization
         norm = output_total_gain*feedback_resistance*squid_turn_ratio
@@ -1341,23 +1372,25 @@
                                   adc_id=None, adc_channel=None):
         """
         get open loop preamp normalization 
         
         """
         
         # driver gain
-        output_total_gain = self.get_output_total_gain(tes_channel=tes_channel,
-                                                       detector_channel=detector_channel,
-                                                       adc_id=adc_id, adc_channel=adc_channel)
+        output_total_gain = self.get_output_total_gain(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
         
       
         # preamp gain
-        preamp_total_gain = self.get_preamp_total_gain(tes_channel=tes_channel,
-                                                       detector_channel=detector_channel,
-                                                       adc_id=adc_id, adc_channel=adc_channel)
+        preamp_total_gain = self.get_preamp_total_gain(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
         
 
         # calculate normalization
         norm = output_total_gain*preamp_total_gain
         return norm
         
 
@@ -1367,23 +1400,25 @@
                                 adc_id=None, adc_channel=None):
         """
         get open loop preamp normalization 
         
         """
         
         # driver gain
-        output_total_gain = self.get_output_total_gain(tes_channel=tes_channel,
-                                                       detector_channel=detector_channel,
-                                                       adc_id=adc_id, adc_channel=adc_channel)
+        output_total_gain = self.get_output_total_gain(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
         
       
         # preamp gain
-        loop_total_gain = self.get_squid_loop_total_gain(tes_channel=tes_channel,
-                                                           detector_channel=detector_channel,
-                                                           adc_id=adc_id, adc_channel=adc_channel)
+        loop_total_gain = self.get_squid_loop_total_gain(
+            tes_channel=tes_channel,
+            detector_channel=detector_channel,
+            adc_id=adc_id, adc_channel=adc_channel)
         
 
         
         # calculate normalization
         norm = output_total_gain*loop_total_gain
         return norm
 
@@ -1514,268 +1549,292 @@
                 
                 output_dict[param].append(val)  
             
                 # wait
                 time.sleep(0.1)
         
             # Signal generator
-            sig_gen_dict = self.get_signal_gen_params(signal_gen_num=1, tes_channel=tes_chan,
-                                                      detector_channel=detector_chan, 
-                                                      adc_id=adc_chan_id, adc_channel=adc_chan)
-          
-            onoff = self.get_signal_gen_onoff(signal_gen_num=1, tes_channel=tes_chan,
-                                              detector_channel=detector_chan, 
-                                              adc_id=adc_chan_id, adc_channel=adc_chan)
+            sig_gen_dict = self.get_signal_gen_params(
+                signal_gen_num=1, tes_channel=tes_chan,
+                detector_channel=detector_chan, 
+                adc_id=adc_chan_id, adc_channel=adc_chan)
+            
+            onoff = self.get_signal_gen_onoff(
+                signal_gen_num=1, tes_channel=tes_chan,
+                detector_channel=detector_chan, 
+                adc_id=adc_chan_id, adc_channel=adc_chan)
             
             output_dict['signal_gen_voltage'].append(sig_gen_dict['voltage'])
             output_dict['signal_gen_current'].append(sig_gen_dict['current'])
             output_dict['signal_gen_frequency'].append(sig_gen_dict['frequency'])
             output_dict['signal_gen_shape'].append(sig_gen_dict['shape'])
             output_dict['signal_gen_phase_shift'].append(sig_gen_dict['phase_shift'])
             output_dict['signal_gen_source'].append(sig_gen_dict['source'])
             output_dict['signal_gen_onoff'].append(onoff)
 
                         
             # other parameter
             output_dict['feedback_resistance'].append(
-                self.get_feedback_resistance(tes_channel=tes_chan, 
-                                             detector_channel=detector_chan, 
-                                             adc_id=adc_chan_id, adc_channel=adc_chan)
+                self.get_feedback_resistance(
+                    tes_channel=tes_chan, 
+                    detector_channel=detector_chan, 
+                    adc_id=adc_chan_id, adc_channel=adc_chan)
             )
             
             output_dict['close_loop_norm'].append(
-                self.get_volts_to_amps_close_loop_norm(tes_channel=tes_chan, 
-                                                       detector_channel=detector_chan, 
-                                                       adc_id=adc_chan_id, adc_channel=adc_chan)
+                self.get_volts_to_amps_close_loop_norm(
+                    tes_channel=tes_chan, 
+                    detector_channel=detector_chan, 
+                    adc_id=adc_chan_id, adc_channel=adc_chan)
             )
             
             output_dict['open_loop_preamp_norm'].append(
-                self.get_open_loop_preamp_norm(tes_channel=tes_chan, 
-                                               detector_channel=detector_chan, 
-                                               adc_id=adc_chan_id, adc_channel=adc_chan)
+                self.get_open_loop_preamp_norm(
+                    tes_channel=tes_chan, 
+                    detector_channel=detector_chan, 
+                    adc_id=adc_chan_id, adc_channel=adc_chan)
             )
             
             output_dict['open_loop_full_norm'].append(
-                self.get_open_loop_full_norm(tes_channel=tes_chan, 
-                                             detector_channel=detector_chan, 
-                                             adc_id=adc_chan_id, adc_channel=adc_chan)
+                self.get_open_loop_full_norm(
+                    tes_channel=tes_chan, 
+                    detector_channel=detector_chan, 
+                    adc_id=adc_chan_id, adc_channel=adc_chan)
             )
             
 
             output_dict['squid_turn_ratio'].append(
-                self.get_squid_turn_ratio(tes_channel=tes_chan, 
-                                          detector_channel=detector_chan, 
-                                          adc_id=adc_chan_id, adc_channel=adc_chan)
+                self.get_squid_turn_ratio(
+                    tes_channel=tes_chan, 
+                    detector_channel=detector_chan, 
+                    adc_id=adc_chan_id, adc_channel=adc_chan)
             )
 
             
             output_dict['shunt_resistance'].append(
-                self.get_shunt_resistance(tes_channel=tes_chan, 
-                                          detector_channel=detector_chan, 
-                                          adc_id=adc_chan_id, adc_channel=adc_chan)
+                self.get_shunt_resistance(
+                    tes_channel=tes_chan, 
+                    detector_channel=detector_chan, 
+                    adc_id=adc_chan_id, adc_channel=adc_chan)
             )
             
-            output_dict['signal_gen_tes_resistance'].append(self._config.get_signal_gen_tes_resistance())
+            output_dict['signal_gen_tes_resistance'].append(
+                self._config.get_signal_gen_tes_resistance())
             
         return output_dict
         
         
 
 
 
-    def _get_sensor_val(self,param_name, 
+    def _get_sensor_val(self, param_name, 
                         tes_channel=None,
                         detector_channel= None,
                         adc_id=None, adc_channel=None):
         
         
         if not self._dummy_mode and self._squid_controller_name is None:
             print('ERROR: No SQUID controller, check config')
             return nan
 
+        if self._dummy_mode:
+            return 1.0
+            
+
+        
         # get readout controller ID and Channel
         controller_id, controller_channel = (
-            connection_utils.get_controller_info(self._connection_table,
-                                                 tes_channel=tes_channel,
-                                                 detector_channel=detector_channel,
-                                                 adc_id=adc_id,
-                                                 adc_channel=adc_channel)
+            connection_utils.get_controller_info(
+                self._connection_table,
+                tes_channel=tes_channel,
+                detector_channel=detector_channel,
+                adc_id=adc_id,
+                adc_channel=adc_channel)
         )
 
         param_val = nan
-        if not self._read_from_redis:
-          
-            if ('feb' in controller_id
-                and self._squid_controller_name=='feb'):
 
-                # CDMS FEB device
+
+        # TES paramaters
+        if param_name == 'tes_bias':
+
+            if self._tes_controller_name=='feb':
+
+                # get channel info
                 feb_info = self._config.get_feb_subrack_slot(controller_id)
-              
                 subrack = int(feb_info[0])
                 slot = int(feb_info[1])
-            
+                
+                if self._verbose or self._debug:
+                    print('INFO: Getting "' + param_name + '" for channel '
+                          + controller_channel + ' from FEB')
                 if self._debug:
-                    print('INFO: Getting setting "'
-                          + param_name + '" from FEB')
                     print('(subrack = ' + str(subrack)
                           + ', slot = ' + str(slot) + 
                           ', channel = ' + str(controller_channel) + ')')
-                        
-                if self._dummy_mode:
-                    param_val= 1
-                else:
 
-                    if param_name == 'tes_bias':
-                        param_val = self._readout_inst.get_phonon_qet_bias(
-                            subrack, slot, controller_channel)
-
-                    elif param_name == 'squid_bias':
-                        param_val = self._readout_inst.get_phonon_squid_bias(
-                            subrack, slot, controller_channel
-                        )
-
-                    elif param_name == 'lock_point_voltage':
-                        param_val = self._readout_inst.get_phonon_lock_point(
-                            subrack, slot, controller_channel
-                        )
-
-                    elif param_name == 'preamp_gain':
-                        param_val = self._readout_inst.get_phonon_preamp_gain(
-                            subrack, slot, controller_channel
-                        )
-
-                    elif param_name == 'output_offset':
-                        param_val = self._readout_inst.get_phonon_offset(
-                            subrack, slot, controller_channel
-                        )
-
-                    elif param_name == 'output_gain':
-                        param_val = self._readout_inst.get_phonon_output_gain(
-                            subrack, slot, controller_channel
-                        )
-
-                    elif param_name == 'feedback_polarity':
-                        is_inverted = self._readout_inst.get_phonon_feedback_polarity(
-                            subrack, slot, controller_channel
-                        )
-                        param_val = 1
-                        if is_inverted:
-                            param_val = -1
-
-                    elif param_name == 'feedback_mode':
-                        is_open = self._readout_inst.is_phonon_feedback_open(
-                            subrack, slot,controller_channel
-                        )
-                        if is_open:
-                            param_val = 'open'
-                        else:
-                            param_val = 'close'
-                            
-                    elif param_name == 'signal_source':
-                        is_preamp = self._readout_inst.is_phonon_source_preamp(
-                            subrack, slot,controller_channel
-                        )
-                        if is_preamp:
-                            param_val = 'preamp'
-                        else:
-                            param_val = 'feedback'
-
-                    elif param_name == 'signal_gen_feedback_connection':
-                        param_val = self._readout_inst.is_signal_generator_feedback_connected(
-                            subrack, slot,controller_channel
-                        )
-                    
+                # get parameter
+                param_val = self._tes_controller_inst.get_phonon_qet_bias(
+                    subrack, slot, controller_channel)
 
-                    elif param_name == 'signal_gen_tes_connection':
-                        param_val = self._readout_inst.is_signal_generator_tes_connected(
-                            subrack, slot,controller_channel
-                        )
+            elif self._tes_controller_name=='magnicon':
 
-                    else:
-                        pass
-                
-            elif ('magnicon' in controller_id
-                  and self._squid_controller_name=='magnicon'):
+                param_val = self._tes_controller_inst.get_tes_current_bias(
+                    controller_channel)
+
+            else:
+                print('ERROR: Unknown TES controller!')
+
+            return param_val
+        
                 
-                if self._verbose:
-                    print('INFO: Getting "' + param_name + ' for channel ' 
-                          + str(controller_channel) + ' (Magnicon)')
+        # SQUID parameters
+        if self._squid_controller_name=='feb':
+            
+            # CDMS FEB device
+            feb_info = self._config.get_feb_subrack_slot(controller_id)
+              
+            subrack = int(feb_info[0])
+            slot = int(feb_info[1])
+            
+            if self._verbose or self._debug:
+                print('INFO: Getting "' + param_name + '" for channel '
+                      + controller_channel + ' using FEB')
+            if self._debug:
+                print('(subrack = ' + str(subrack)
+                      + ', slot = ' + str(slot) + 
+                      ', channel = ' + str(controller_channel) + ')')
+
+            if param_name == 'squid_bias':
+                param_val = self._squid_controller_inst.get_phonon_squid_bias(
+                    subrack, slot, controller_channel
+                )
+
+            elif param_name == 'lock_point_voltage':
+                param_val = self._squid_controller_inst.get_phonon_lock_point(
+                    subrack, slot, controller_channel
+                )
 
+            elif param_name == 'preamp_gain':
+                param_val = self._squid_controller_inst.get_phonon_preamp_gain(
+                    subrack, slot, controller_channel
+                )
+
+            elif param_name == 'output_offset':
+                param_val = self._squid_controller_inst.get_phonon_offset(
+                    subrack, slot, controller_channel
+                )
+
+            elif param_name == 'output_gain':
+                param_val = self._squid_controller_inst.get_phonon_output_gain(
+                    subrack, slot, controller_channel
+                )
+
+            elif param_name == 'feedback_polarity':
+                is_inverted = self._squid_controller_inst.get_phonon_feedback_polarity(
+                    subrack, slot, controller_channel
+                )
+                param_val = 1
+                if is_inverted:
+                    param_val = -1
+
+            elif param_name == 'feedback_mode':
+                is_open = self._squid_controller_inst.is_phonon_feedback_open(
+                    subrack, slot,controller_channel
+                )
+                if is_open:
+                    param_val = 'open'
+                else:
+                    param_val = 'close'
+                            
+            elif param_name == 'signal_source':
+                is_preamp = self._squid_controller_inst.is_phonon_source_preamp(
+                    subrack, slot,controller_channel
+                )
+                if is_preamp:
+                    param_val = 'preamp'
+                else:
+                    param_val = 'feedback'
 
-                if not self._dummy_mode:
+            elif param_name == 'signal_gen_feedback_connection':
+                param_val = self._squid_controller_inst.is_signal_generator_feedback_connected(
+                    subrack, slot,controller_channel
+                )
                     
-                    if param_name == 'tes_bias':
-                        param_val = self._readout_inst.get_tes_current_bias(
-                            controller_channel)
-
-                    elif param_name == 'squid_bias':
-                        param_val = self._readout_inst.get_squid_bias(
-                            controller_channel,'I')
-
-                    elif param_name == 'lock_point_voltage':
-                        param_val = self._readout_inst.get_squid_bias(
-                            controller_channel,'V')
-
-                    elif param_name == 'feedback_gain':
-                        param_val = self._readout_inst.get_GBP(
-                            controller_channel)
-
-                    elif param_name == 'output_offset':
-                        # No offset setting magnicon
-                        param_val = 0
+
+            elif param_name == 'signal_gen_tes_connection':
+                param_val = self._squid_controller_inst.is_signal_generator_tes_connected(
+                    subrack, slot,controller_channel
+                )
+
+            else:
+                pass
+                
+        elif self._squid_controller_name=='magnicon':
+            
+            if self._verbose:
+                print('INFO: Getting "' + param_name + '" for channel ' 
+                      + str(controller_channel) + ' using Magnicon')
+                            
+            if param_name == 'squid_bias':
+                param_val = self._squid_controller_inst.get_squid_bias(
+                    controller_channel,'I')
+                
+            elif param_name == 'lock_point_voltage':
+                param_val = self._squid_controller_inst.get_squid_bias(
+                    controller_channel,'V')
+
+            elif param_name == 'feedback_gain':
+                param_val = self._squid_controller_inst.get_GBP(
+                    controller_channel)
+
+            elif param_name == 'output_offset':
+                # No offset setting magnicon
+                param_val = 0
                         
-                    elif param_name == 'output_gain':
-                        # No output gain magnicon
-                        param_val = 1
+            elif param_name == 'output_gain':
+                # No output gain magnicon
+                param_val = 1
                         
-                    elif param_name == 'preamp_gain':
-                        amp, bw = self._readout_inst.get_amp_gain_bandwidth(controller_channel)
-                        param_val = amp
-
-                    elif param_name == 'preamp_bandwidth':
-                        amp, bw = self._readout_inst.get_amp_gain_bandwidth(controller_channel)
-                        param_val = bw
+            elif param_name == 'preamp_gain':
+                amp, bw = self._squid_controller_inst.get_amp_gain_bandwidth(controller_channel)
+                param_val = amp
+
+            elif param_name == 'preamp_bandwidth':
+                amp, bw = self._squid_controller_inst.get_amp_gain_bandwidth(controller_channel)
+                param_val = bw
                         
-                    elif param_name == 'feedback_polarity':
-                        param_val = self._readout_inst.get_squid_gain_sign(controller_channel)
-
-                    elif param_name == 'feedback_mode':
-                        val = self._readout_inst.get_amp_or_fll(controller_channel)
-                        if val=='AMP':
-                            param_val = 'open'
-                        elif val=='FLL':
-                            param_val = 'close'
-                        else:
-                            param_val = val
-
-                    elif param_name == 'signal_source':
-                        val = self._readout_inst.get_amp_or_fll(controller_channel)
-                        if val=='AMP':
-                            param_val = 'preamp'
-                        elif val=='FLL':
-                            param_val = 'feedback'
-                        else:
-                            param_val = val
-
-                    elif param_name == 'feedback_resistance':
-                        param_val = self._readout_inst.get_feedback_resistor(controller_channel)
+            elif param_name == 'feedback_polarity':
+                param_val = self._squid_controller_inst.get_squid_gain_sign(controller_channel)
+                
+            elif param_name == 'feedback_mode':
+                val = self._squid_controller_inst.get_amp_or_fll(controller_channel)
+                if val=='AMP':
+                    param_val = 'open'
+                elif val=='FLL':
+                    param_val = 'close'
+                else:
+                    param_val = val
 
-                    else:
-                        pass
+            elif param_name == 'signal_source':
+                val = self._squid_controller_inst.get_amp_or_fll(controller_channel)
+                if val=='AMP':
+                    param_val = 'preamp'
+                elif val=='FLL':
+                    param_val = 'feedback'
                 else:
-                    param_val= 1
+                    param_val = val
 
-            else:
-                param_val= 1
+            elif param_name == 'feedback_resistance':
+                param_val = self._squid_controller_inst.get_feedback_resistor(controller_channel)
 
-        else:
-            print('ERROR: Reading from redis N/A')
+            else:
+                pass
 
             
-            
         return param_val
 
 
         
         
     def _set_sensor_val(self,param_name, value, 
                         tes_channel=None,
@@ -1788,15 +1847,16 @@
         TBD
         """
 
         if not self._dummy_mode and self._squid_controller_name is None:
             print('ERROR: No SQUID controller, check config')
             return nan
             
-            
+        if self._dummy_mode:
+            return
 
         # get readout controller ID and Channel
         controller_id, controller_channel = (
             connection_utils.get_controller_info(
                 self._connection_table,
                 tes_channel=tes_channel,
                 detector_channel=detector_channel,
@@ -1807,143 +1867,183 @@
               
         # ================
         # Set value
         # ================
         
         readback_val = None
 
-        if ('feb' in controller_id and
-            self._squid_controller_name == 'feb'):
+        # TES controller
+        if param_name == 'tes_bias':
+
+            if self._tes_controller_name=='feb':
+
+                # get channel info
+                feb_info = self._config.get_feb_subrack_slot(controller_id)
+                subrack = int(feb_info[0])
+                slot = int(feb_info[1])
+                
+                if self._verbose or self._debug:
+                    print('INFO: Getting setting "'
+                          + param_name + '" from FEB')
+                if self._debug:
+                    print('(subrack = ' + str(subrack)
+                          + ', slot = ' + str(slot) + 
+                          ', channel = ' + str(controller_channel) + ')')
+
+                # set parameter
+                self._tes_controller_inst.set_phonon_qet_bias(
+                    subrack, slot, controller_channel, value)
+
+
+                # readback
+                if  self._enable_readback:
+                    time.sleep(0.5)
+                    readback_val = self._get_sensor_val(
+                        param_name,
+                        tes_channel=tes_channel,
+                        detector_channel=detector_channel,
+                        adc_id=adc_id, adc_channel=adc_channel)
+                
+             
+            elif self._tes_controller_name=='magnicon':
+                readback_val = self._tes_controller_inst.set_tes_current_bias(
+                    controller_channel, value, mode=None
+                )
+                
+            else:
+                raise ValueError('ERROR: Unknown TES controller!')
+
+
+            
+        elif self._squid_controller_name == 'feb':
+            
             # CDMS FEB device
             
             feb_info = self._config.get_feb_subrack_slot(controller_id)
             subrack = int(feb_info[0])
             slot = int(feb_info[1])
             
             if self._verbose or self._debug:
                 print('INFO: Setting ' + param_name
                       + ' to ' + str(value) + ' using FEB!')
             if self._debug:
                 print('DEBUG: FEB - subrack = ' + str(subrack)
                       + ', slot = ' + str(slot) + ', channel = '
                       + str(controller_channel))
-                 
-            if not self._dummy_mode:
-                if param_name == 'tes_bias':
-                    self._readout_inst.set_phonon_qet_bias(
-                        subrack, slot, controller_channel, value)
-            
-                elif param_name == 'squid_bias':
-                    self._readout_inst.set_phonon_squid_bias(
-                        subrack, slot, controller_channel, value)
-                
-                elif param_name == 'lock_point_voltage':
-                    self._readout_inst.set_phonon_lock_point(
-                        subrack, slot, controller_channel, value)
-                
-                elif param_name == 'preamp_gain':
-                    self._readout_inst.set_phonon_preamp_gain(
-                        subrack, slot, controller_channel, value)
-                
-                elif param_name == 'output_offset':
-                    self._readout_inst.set_phonon_offset(
-                        subrack, slot, controller_channel, value)
-                
-                elif param_name == 'output_gain':
-                    self._readout_inst.set_phonon_output_gain(
-                        subrack, slot, controller_channel, value)
-                
-                elif param_name == 'feedback_polarity':
-                    do_invert = False
-                    if val==-1:
-                        do_invert = True
-                    self._readout_inst.set_phonon_feedback_polarity(
-                        subrack, slot, controller_channel, do_invert
-                    )
+                
+            if param_name == 'squid_bias':
+                self._squid_controller_inst.set_phonon_squid_bias(
+                    subrack, slot, controller_channel, value)
+                
+            elif param_name == 'lock_point_voltage':
+                self._squid_controller_inst.set_phonon_lock_point(
+                    subrack, slot, controller_channel, value)
+                
+            elif param_name == 'preamp_gain':
+                self._squid_controller_inst.set_phonon_preamp_gain(
+                    subrack, slot, controller_channel, value)
+                
+            elif param_name == 'output_offset':
+                self._squid_controller_inst.set_phonon_offset(
+                    subrack, slot, controller_channel, value)
+                
+            elif param_name == 'output_gain':
+                self._squid_controller_inst.set_phonon_output_gain(
+                    subrack, slot, controller_channel, value)
+                
+            elif param_name == 'feedback_polarity':
+                do_invert = False
+                if val==-1:
+                    do_invert = True
+                self._squid_controller_inst.set_phonon_feedback_polarity(
+                    subrack, slot, controller_channel, do_invert
+                )
             
-                elif param_name == 'feedback_mode':
-                    do_open = False
-                    if value == 'open':
-                        do_open = True
-                    self._readout_inst.set_phonon_feedback_loop(subrack, slot, controller_channel, do_open)
-                
-                elif param_name == 'preamp_source':
-                    self._readout_inst.set_phonon_source_preamp(subrack, slot, controller_channel, value)
-                
-                elif param_name == 'signal_gen_feedback_connection':
-                    self._readout_inst.connect_signal_generator_feedback(
-                        subrack, slot, controller_channel, value
-                    )
+            elif param_name == 'feedback_mode':
+                do_open = False
+                if value == 'open':
+                    do_open = True
+                self._squid_controller_inst.set_phonon_feedback_loop(
+                    subrack, slot, controller_channel, do_open)
+                
+            elif param_name == 'preamp_source':
+                self._squid_controller_inst.set_phonon_source_preamp(
+                    subrack, slot, controller_channel, value)
+                
+            elif param_name == 'signal_gen_feedback_connection':
+                self._squid_controller_inst.connect_signal_generator_feedback(
+                    subrack, slot, controller_channel, value
+                )
                 
-                elif param_name == 'signal_gen_tes_connection':
-                    self._readout_inst.connect_signal_generator_tes(subrack, slot, controller_channel, value)
+            elif param_name == 'signal_gen_tes_connection':
+                self._squid_controller_inst.connect_signal_generator_tes(
+                    subrack, slot, controller_channel, value)
+
+
+            # readback
+            if  self._enable_readback:
+                time.sleep(0.5)
+                readback_val = self._get_sensor_val(
+                    param_name,
+                    tes_channel=tes_channel,
+                    detector_channel=detector_channel,
+                    adc_id=adc_id, adc_channel=adc_channel)
                            
 
-        elif ('magnicon' in controller_id and
-              self._squid_controller_name == 'magnicon'):
+        elif self._squid_controller_name == 'magnicon':
             
             if self._verbose or self._debug:
                 print('INFO: Setting "' + param_name + '" to ' + str(value) + ' for channel ' 
                       + str(controller_channel) + ' (Magnicon)!')
-
-            if not self._dummy_mode:
-                
-                if param_name == 'tes_bias':
-                    readback_val = self._readout_inst.set_tes_current_bias(
-                        controller_channel, value, mode=None
+                          
+                             
+            if param_name == 'squid_bias':
+                readback_val = self._squid_controller_inst.set_squid_bias(
+                    controller_channel, 'I', value)
+                
+            elif param_name == 'lock_point_voltage':
+                readback_val = self._squid_controller_inst.set_squid_bias(
+                    controller_channel, 'V', value)
+                
+            elif param_name == 'feedback_gain':
+                readback_val = self._squid_controller_inst.set_GBP(
+                    controller_channel, value)
+                    
+            elif param_name == 'feedback_polarity':
+                readback_val = self._squid_controller_inst.set_squid_gain_sign(
+                    controller_channel, value)
+                
+            elif param_name == 'preamp_gain':
+                if isinstance(value,tuple) and len(value)==2:
+                    amp, bw = self._squid_controller_inst.set_amp_gain_bandwidth(
+                        controller_channel, value[0], value[1]
                     )
-                
-                elif param_name == 'squid_bias':
-                    readback_val = self._readout_inst.set_squid_bias(controller_channel, 'I', value)
-                
-                elif param_name == 'lock_point_voltage':
-                    readback_val = self._readout_inst.set_squid_bias(controller_channel, 'V', value)
-                
-                elif param_name == 'feedback_gain':
-                    readback_val = self._readout_inst.set_GBP(controller_channel, value)
+                    readback_val = (amp,bw)
+                else:
+                    print('WARNING: a tuple with (amplitude, bandwidth) required'
+                          ' for magnicon preamp setting')
                     
-                elif param_name == 'feedback_polarity':
-                    readback_val = self._readout_inst.set_squid_gain_sign(controller_channel, value)
-                
-                elif param_name == 'preamp_gain':
-                    if isinstance(value,tuple) and len(value)==2:
-                        amp, bw = self._readout_inst.set_amp_gain_bandwidth(
-                            controller_channel, value[0], value[1]
-                        )
-                        readback_val = (amp,bw)
-                    else:
-                        print('WARNING: a tuple with (amplitude, bandwidth) required for magnicon preamp setting')
-
-                elif param_name == 'feedback_mode':
-                    mode = 'AMP'
-                    if value=='close':
-                        mode='FLL'
-                    readback_val = self._readout_inst.set_amp_or_fll(controller_channel, mode)
+            elif param_name == 'feedback_mode':
+                mode = 'AMP'
+                if value=='close':
+                    mode='FLL'
+                readback_val = self._squid_controller_inst.set_amp_or_fll(
+                    controller_channel, mode)
 
 
         else:
             print('ERROR: Unknow SQUID controller "' + 
                   self._squid_controller_name + '"!')
         
     
         # ================
-        # Read back
+        # Display read back
         # ================
-        time.sleep(0.2)
-
-        if  self._enable_readback and not self._dummy_mode:
+        if  self._enable_readback:
 
-            # FEB
-            if self._squid_controller_name == 'feb':
-                readback_val= self._get_sensor_val(param_name,
-                                                   tes_channel=tes_channel,
-                                                   detector_channel=detector_channel,
-                                                   adc_id=adc_id, adc_channel=adc_channel)
-             
-            
             if self._verbose:
                 print('INFO: Parameter ' + param_name)
                 print('Value set = ' + str(value))
                 print('Value readback = ' + str(value_readback))
         
         
         # ================
@@ -2143,33 +2243,52 @@
         if self._dummy_mode:
             print('WARNING: Dummy mode enabled. Not connecting instruments!')
             return
 
 
         # visa library
         visa_library = self._config.get_visa_library()
-        
-        # ----------
+
+        # -----------------
         # CDMS FEB
-        # ----------
-        if self._squid_controller_name == 'feb':
+        # -----------------
+
+        if (self._squid_controller_name == 'feb'
+            or self._tes_controller_name == 'feb'):
+            
             address = self._config.get_feb_address()
+            inst = None
             if address:
                 if self._verbose:
                     print('INFO: Instantiating FEB using address: ' + address)
-                self._readout_inst = FEB(address,
-                                         visa_library=visa_library,
-                                         verbose=self._verbose, raise_errors=self._raise_errors)
+                feb_inst = FEB(
+                    address,
+                    visa_library=visa_library,
+                    verbose=self._verbose,
+                    raise_errors=self._raise_errors)
             else:
                 raise ValueError('Unable to find GPIB address. It will not work!')
 
-        # ----------
+            # SQUID controller
+            if self._squid_controller_name == 'feb':
+                self._squid_controller_inst = feb_inst
+
+            # TES controller
+            if self._tes_controller_name == 'feb':
+                self._tes_controller_inst = feb_inst
+                
+            
+        # -----------------
         # Magnicon
-        # ----------
-        if (self._squid_controller_name == 'magnicon' or self._signal_generator_name == 'magnicon'):
+        # -----------------
+        
+        if (self._squid_controller_name == 'magnicon'
+            or self._signal_generator_name == 'magnicon'
+            or self._tes_controller_name == 'magnicon'):
+            
             mag_control_info = self._config.get_magnicon_controller_info()
             mag_conn_info = self._config.get_magnicon_connection_info()
             magnicon_inst = Magnicon(channel_list=mag_control_info['channel_list'],
                                      default_active=mag_control_info['default_active'],
                                      reset_active=mag_control_info['reset_active'],
                                      conn_info=mag_conn_info)
             
@@ -2194,34 +2313,41 @@
                     print('Default active channel:',
                           str(mag_control_info['default_active']))
                     print('Reset active channel after every step:',
                           str(mag_control_info['reset_active']))
    
 
             if self._squid_controller_name == 'magnicon':
-                self._readout_inst = magnicon_inst
+                self._squid_controller_inst = magnicon_inst
 
             if self._signal_generator_name == 'magnicon':
                 self._signal_generator_inst = magnicon_inst
+
+            if self._tes_controller_name == 'magnicon':
+                self._tes_controller_inst = magnicon_inst
+                
                     
         # ----------------
-        # Signal Generator
+        # Keysight
         # ----------------
+                  
         if self._signal_generator_name == 'keysight':
+
             address = self._config.get_signal_generator_visa_address('keysight')
             attenuation = self._config.get_signal_generator_attenuation('keysight')
             self._signal_generator_inst = (
                 KeysightFuncGenerator(address,
                                       visa_library=visa_library,
                                       attenuation=attenuation,
                                       verbose=self._verbose,
                                       raise_errors=self._raise_errors)
             )
 
 
+
             
         # ----------------
         # Temperature controllers
         # ----------------
         self._temperature_controller_insts = dict()
         
         # loop controllers
@@ -2250,8 +2376,22 @@
 
 
             
     def _disconnect_instruments(self):
         """
         Disconnect instruments
         """
-        return
+
+        if self._signal_generator_inst is not None:
+            self._signal_generator_inst.disconnect()
+            self._signal_generator_inst = None
+
+        if self._tes_controller_inst is not None:
+            self._tes_controller_inst.disconnect()
+            self._tes_controller_inst = None
+
+        if self._squid_controller_inst is not None:
+            if (self._squid_controller_name != self._tes_controller_name):
+                self._squid_controller_inst.disconnect()
+            self._squid_controller_inst = None
+            
+
```

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/feb/feb.py` & `pytesdaq-0.3.6/pytesdaq/instruments/feb/feb.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/imacrt/imacrt.py` & `pytesdaq-0.3.6/pytesdaq/instruments/imacrt/imacrt.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/imacrt/macrtmodule.py` & `pytesdaq-0.3.6/pytesdaq/instruments/imacrt/macrtmodule.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/keysight/keysight.py` & `pytesdaq-0.3.6/pytesdaq/instruments/keysight/keysight.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/lakeshore.py` & `pytesdaq-0.3.6/pytesdaq/instruments/lakeshore/lakeshore.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/magnicon/magnicon.py` & `pytesdaq-0.3.6/pytesdaq/instruments/magnicon/magnicon.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/instruments/niadc/nidevice.py` & `pytesdaq-0.3.6/pytesdaq/instruments/niadc/nidevice.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/io/filter_hdf5.py` & `pytesdaq-0.3.6/pytesdaq/io/filter_hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/io/hdf5.py` & `pytesdaq-0.3.6/pytesdaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/io/redis.py` & `pytesdaq-0.3.6/pytesdaq/io/redis.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools.py` & `pytesdaq-0.3.6/pytesdaq/processing/_iv_didv_tools.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools_plotting.py` & `pytesdaq-0.3.6/pytesdaq/processing/_iv_didv_tools_plotting.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/processing/_process_iv_didv.py` & `pytesdaq-0.3.6/pytesdaq/processing/_process_iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/processing/trigger.py` & `pytesdaq-0.3.6/pytesdaq/processing/trigger.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/scope/readout.py` & `pytesdaq-0.3.6/pytesdaq/scope/readout.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/scope/scope.py` & `pytesdaq-0.3.6/pytesdaq/scope/scope.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/sequencer/iv_didv.py` & `pytesdaq-0.3.6/pytesdaq/sequencer/iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/sequencer/sequencer.py` & `pytesdaq-0.3.6/pytesdaq/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/sequencer/tc.py` & `pytesdaq-0.3.6/pytesdaq/sequencer/tc.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/utils/arg_utils.py` & `pytesdaq-0.3.6/pytesdaq/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/utils/connection_utils.py` & `pytesdaq-0.3.6/pytesdaq/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/pytesdaq/utils/remote.py` & `pytesdaq-0.3.6/pytesdaq/utils/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 
 class Remote(object):
     """
     Use ssh connection to remote computer, using Python paramiko library
     """
 
-    def __init__(self, hostname='', port=22, username='', auth_method='rsa', auth_val='', log_file='demo.log'):
+    def __init__(self, hostname='', port=22, username='',
+                 auth_method='rsa', auth_val='',
+                 log_file='demo.log'):
         """
         Initialize class with hostname, port, username,
         authentication method (rsa, dss, or password),
         and Paramiko log file.
         Store auth_val if you want to set the RSA/DSS key or password.
         """
         self._hostname = hostname
@@ -167,15 +169,15 @@
                 keys = {}
 
             # check server's host key -- this is important.
             key = transport.get_remote_server_key()
             print('Known keys:')
             print(keys.keys())
             print('')
-            print('Our key:', keys['128.32.239.62'].keys())
+            #print('Our key:', keys['128.32.239.62'].keys())
             print('Server key:', key.get_name())
             print('')
             if self._hostname not in keys:
                 print("*** WARNING: Unknown host key!")
             elif key.get_name() not in keys[self._hostname]:
                 print("*** WARNING: Unknown host key!")
             elif keys[self._hostname][key.get_name()] != key:
```

### Comparing `pytesdaq-0.3.4/pytesdaq.egg-info/PKG-INFO` & `pytesdaq-0.3.6/pytesdaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.4
+Version: 0.3.6
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.3.4/pytesdaq.egg-info/SOURCES.txt` & `pytesdaq-0.3.6/pytesdaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.4/setup.py` & `pytesdaq-0.3.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
       long_description = f.read()
 
 
 setup(name='pytesdaq',
-      version='0.3.4',
+      version='0.3.6',
       description='DAQ and Intruments control for TES development',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Bruno Serfass',
       author_email='serfass@berkeley.edu',
       url="https://github.com/spice-herald/pytesdaq",
       zip_safe = False,
```

