# Comparing `tmp/inspursmsdk-2.1.1.tar.gz` & `tmp/inspursmsdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspursmsdk-2.1.1.tar", last modified: Tue Jul 25 09:31:32 2023, max compression
+gzip compressed data, was "dist/inspursmsdk-2.1.2.tar", last modified: Thu Aug  3 02:00:15 2023, max compression
```

## Comparing `inspursmsdk-2.1.1.tar` & `inspursmsdk-2.1.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/
--rw-r--r--   0 root         (0) root         (0)      991 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      888 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:24.000000 inspursmsdk-2.1.1/inspur_sm_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49818 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    21216 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   299718 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12152 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18131 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54444 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84520 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81800 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46178 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   360127 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   360290 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    66019 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    44074 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)      316 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA7_11308.py
--rw-r--r--   0 root         (0) root         (0)   744015 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   602520 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    18029 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16476 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   288628 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM7_13505.py
--rw-r--r--   0 root         (0) root         (0)    45791 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14826 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15217 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59696 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47115 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   120116 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4718 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:25.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/parameterConversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2682 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/ism.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)      991 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      888 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:16.000000 inspursmsdk-2.1.2/inspur_sm_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49818 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   300270 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12152 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18131 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54444 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84520 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81800 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46178 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   360127 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   360290 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66019 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/conf/
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/conf/NF5180M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/conf/NF5280M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/conf/SA5112M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/conf/SA5212M5.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44318 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      316 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744218 2023-08-03 01:58:18.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   604760 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    18029 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   288628 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45791 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59696 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47115 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   122296 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4718 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 01:58:16.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-08-03 01:58:17.000000 inspursmsdk-2.1.2/inspur_sm_sdk/util/parameterConversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/inspursmsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-08-03 02:00:14.000000 inspursmsdk-2.1.2/inspursmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-08-03 02:00:14.000000 inspursmsdk-2.1.2/inspursmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 02:00:14.000000 inspursmsdk-2.1.2/inspursmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-08-03 02:00:14.000000 inspursmsdk-2.1.2/inspursmsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 02:00:14.000000 inspursmsdk-2.1.2/inspursmsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/ism.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 02:00:15.000000 inspursmsdk-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-08-03 01:58:19.000000 inspursmsdk-2.1.2/setup.py
```

### Comparing `inspursmsdk-2.1.1/MANIFEST.in` & `inspursmsdk-2.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/PKG-INFO` & `inspursmsdk-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/IpmiFunc.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/IpmiFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/biosPostEventStr.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/commonInfoStr.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/eventLogString.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorEventStr.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/showSensorDesc.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/M5Log/showSensorDesc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/RedfishFunc.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/RestFunc.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/RestFunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -7770,14 +7770,29 @@
         JSON['data'] = ""
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("[PUT]api/settings/media/remotesession", response)
     return JSON
 
 
+def getHBAInfoByRest(client):
+    JSON = {}
+    response = client.request("GET", "api/status/hba_info", client.getHearder(), None, None, None, None)
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/status/hba_info, response is none'
+    elif response.status_code == 200:
+        result = response.json()
+        JSON['code'] = 0
+        JSON['data'] = result
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/status/hba_info", response)
+    return JSON
+
 class NF5280M5_SensorType():
     def __init__(self):
         self.getSensorTypeKey = getSensorTypeKey
 
     def getSensorType(self, var):
         return self.getSensorTypeKey("en", var)
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/backup.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/A7.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3180A6.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3280A6.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5468A5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5488A5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/command/restore.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5180M5.yml` & `inspursmsdk-2.1.2/inspur_sm_sdk/conf/NF5180M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5280M5.yml` & `inspursmsdk-2.1.2/inspur_sm_sdk/conf/NF5280M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5112M5.yml` & `inspursmsdk-2.1.2/inspur_sm_sdk/conf/SA5112M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5212M5.yml` & `inspursmsdk-2.1.2/inspur_sm_sdk/conf/SA5212M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/Base.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/Base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1427,25 +1427,35 @@
 
     def methods(self, client, args):
         return(list(filter(lambda m: not m.startswith("__") and not m.endswith("__") and callable(getattr(self, client, args, m)), dir(self, client, args))))
 
     def setbmclogcfg(self, client, args):
         result = ResultBean()
         result.State("Not Support")
+        result.Message([])
         return result
 
     def remoteFWUpdate(self, client, args):
         result = ResultBean()
         result.State("Not Support")
+        result.Message([])
         return result
 
     def updatepsu(self, client, args):
         result = ResultBean()
         result.State("Not Support")
+        result.Message([])
         return result
+
+    def gethba(self, client, args):
+        result = ResultBean()
+        result.State("Not Support")
+        result.Message([])
+        return result
+
 # Ascii转十六进制
 
 
 def ascii2hex(data, length):
     count = length - len(data)
     list_h = []
     for c in data:
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA5.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA6.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA7.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM5.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM5.py`

 * *Files 0% similar despite different names*

```diff
@@ -8954,14 +8954,20 @@
 
     def remoteFWUpdate(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M5 model does not support this feature.'])
         return result
 
+    def gethba(self, client, args):
+        result = ResultBean()
+        result.State("Not Support")
+        result.Message(['The M5 model does not support this feature.'])
+        return result
+
 
 def getWeek(binr):
     bin_dict = {1: 'Mon', 2: 'Tue', 3: 'Wed', 4: 'Thur', 5: 'Fri', 6: 'Sat', 7: 'Sun'}
     list = []
     for i in range(1, 7):
         weeki = binr[8 - i:9 - i]
         if weeki == '1':
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM6.py`

 * *Files 1% similar despite different names*

```diff
@@ -11794,14 +11794,63 @@
 
     def remoteFWUpdate(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M6 model does not support this feature.'])
         return result
 
+    def gethba(self, client, args):
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            login_res = ResultBean()
+            login_res.State("Failure")
+            login_res.Message(
+                ["login error, please check username/password/host/port"])
+            return login_res
+        client.setHearder(headers)
+        result = ResultBean()
+
+        hba_info = RestFunc.getHBAInfoByRest(client)
+        if hba_info == {}:
+            result.State('Failure')
+            result.Message(['get hba info failed'])
+        elif hba_info.get('code') == 0 and hba_info.get('data') is not None:
+            hba_data = hba_info.get('data')
+            hba_dict = {0: 'No', 1: 'Yes'}
+            hba_list = []
+            for hba in hba_data:
+                hba_result = HBABean()
+                hba_result.Id(hba.get('id', 0))
+                hba_result.Name(hba.get('Name', None))
+                hba_result.Manufacturer(hba.get('Manufacturer', None))
+                hba_result.HbaTemp(hba.get('Vendor', None))
+                hba_result.SN(hba.get('sn', 0))
+                hba_result.Present(hba_dict.get(hba.get('Present', 0)))
+                hba_result.PortCount(hba.get('PortCount', 0))
+                ports = hba.get('ports', [])
+                postList = []
+                for port in ports:
+                    hba_post = HBAPost()
+                    hba_post.Id(port.get('id', 0))
+                    hba_post.PortWWPN(port.get('PortWWPN', None))
+                    hba_post.PortWWNN(port.get('PortWWNN', None))
+                    hba_post.PortLinkState(port.get('PortLinkState', None))
+                    hba_post.PortLinkSpeed(port.get('PortLinkSpeed', 0))
+                    postList.append(hba_post.dict)
+                hba_result.HBAPost(postList)
+                hba_list.append(hba_result.dict)
+            result.State("Success")
+            result.Message(hba_list)
+        else:
+            result.State("Failure")
+            result.Message(["get hba info error, error code " + str(
+                hba_info.get('code')) + ", error info: " + str(hba_info.get('data'))])
+
+        RestFunc.logout(client)
+        return result
 
 
 # 检查日志进度，进度到100 后下载文件
 def getProgressAndDown(client, args):
     bmcres = ResultBean()
     state = 0
     count = 0
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_41401.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM6_41401.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_4140a.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM7.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/CommonM7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/I24M6.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/IBase.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/IBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,7 +561,13 @@
         """
 
     def cancletask(self, client, args):
         """
 
         :return:
         """
+
+    def gethba(self, client, args):
+        """
+
+        :return:
+        """
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5180M5.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_435.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_436.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NS5160M6.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/ResEntity.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/ResEntity.py`

 * *Files 0% similar despite different names*

```diff
@@ -5096,7 +5096,106 @@
 
     def GPUTemp(self):
         return self.dict['GPUTemp']
 
     def GPUTemp(self, value):
         self.dict['GPUTemp'] = value
 
+
+class HBABean():
+    def __init__(self):
+        self.dict = collections.OrderedDict()
+
+    def Id(self):
+        return self.dict['Id']
+
+    def Id(self, value):
+        self.dict['Id'] = value
+
+    def Name(self):
+        return self.dict['Name']
+
+    def Name(self, value):
+        self.dict['Name'] = value
+
+    def Pn(self):
+        return self.dict['Pn']
+
+    def Pn(self, value):
+        self.dict['Pn'] = value
+
+    def Manufacturer(self):
+        return self.dict['Manufacturer']
+
+    def Manufacturer(self, value):
+        self.dict['Manufacturer'] = value
+
+    def PortCount(self):
+        return self.dict['PortCount']
+
+    def PortCount(self, value):
+        self.dict['PortCount'] = value
+
+    def Present(self):
+        return self.dict['Present']
+
+    def Present(self, value):
+        self.dict['Present'] = value
+
+    def HbaTemp(self):
+        return self.dict['HbaTemp']
+
+    def HbaTemp(self, value):
+        self.dict['HbaTemp'] = value
+
+    def Vendor(self):
+        return self.dict['Vendor']
+
+    def Vendor(self, value):
+        self.dict['Vendor'] = value
+
+    def SN(self):
+        return self.dict['SN']
+
+    def SN(self, value):
+        self.dict['SN'] = value
+
+    def HBAPost(self):
+        return self.dict['Posts']
+
+    def HBAPost(self, value):
+        self.dict['Posts'] = value
+
+
+class HBAPost():
+    def __init__(self):
+        self.dict = collections.OrderedDict()
+
+    def Id(self):
+        return self.dict['Id']
+
+    def Id(self, value):
+        self.dict['Id'] = value
+
+    def PortWWPN(self):
+        return self.dict['PortWWPN']
+
+    def PortWWPN(self, value):
+        self.dict['PortWWPN'] = value
+
+    def PortWWNN(self):
+        return self.dict['PortWWNN']
+
+    def PortWWNN(self, value):
+        self.dict['PortWWNN'] = value
+
+    def PortLinkState(self):
+        return self.dict['PortLinkState']
+
+    def PortLinkState(self, value):
+        self.dict['PortLinkState'] = value
+
+    def PortLinkSpeed(self):
+        return self.dict['PortLinkSpeed']
+
+    def PortLinkSpeed(self, value):
+        self.dict['PortLinkSpeed'] = value
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/interface/SA5212M5Impl.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/interface/SA5212M5Impl.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/route/route.yml` & `inspursmsdk-2.1.2/inspur_sm_sdk/route/route.yml`

 * *Files 2% similar despite different names*

```diff
@@ -149,7 +149,10 @@
     1.3505: CommonM7_13505
 TS860M7:
     common: CommonM7
     1.3505: CommonM7_13505
 NF8480M7:
     common: CommonM7
     1.3505: CommonM7_13505
+NF5170M7:
+    common: CommonM7
+    1.3505: CommonM7_13505
```

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/HostTypeJudge.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/HostTypeJudge.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/RedfishClient.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/RegularCheckUtil.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/RequestClient.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/configUtil.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/fileUtil.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspur_sm_sdk/util/parameterConversion.py` & `inspursmsdk-2.1.2/inspur_sm_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/inspursmsdk.egg-info/PKG-INFO` & `inspursmsdk-2.1.2/inspursmsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.1.1/inspursmsdk.egg-info/SOURCES.txt` & `inspursmsdk-2.1.2/inspursmsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.1/ism.py` & `inspursmsdk-2.1.2/ism.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     ISM_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inspursmsdk-2.1.1/setup.py` & `inspursmsdk-2.1.2/setup.py`

 * *Files identical despite different names*

