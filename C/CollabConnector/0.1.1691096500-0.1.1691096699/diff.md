# Comparing `tmp/CollabConnector-0.1.1691096500.tar.gz` & `tmp/CollabConnector-0.1.1691096699.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CollabConnector-0.1.1691096500.tar", last modified: Thu Aug  3 21:01:48 2023, max compression
+gzip compressed data, was "CollabConnector-0.1.1691096699.tar", last modified: Thu Aug  3 21:05:07 2023, max compression
```

## Comparing `CollabConnector-0.1.1691096500.tar` & `CollabConnector-0.1.1691096699.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.229998 CollabConnector-0.1.1691096500/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1691096500/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-08-03 21:01:48.230118 CollabConnector-0.1.1691096500/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1691096500/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1691096500/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-08-03 21:01:48.230653 CollabConnector-0.1.1691096500/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.966004 CollabConnector-0.1.1691096500/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.977072 CollabConnector-0.1.1691096500/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.980139 CollabConnector-0.1.1691096500/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.981730 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.983089 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10787 2023-07-06 17:10:27.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.984574 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/AXL.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.987392 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Add/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Add/Add.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Add/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.988754 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Do/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Do/Do.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Do/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.991415 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Get/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Get/Get.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Get/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.994256 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/List/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/List/List.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/List/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.995942 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Remove/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Remove/Remove.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Remove/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.998377 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Update/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Update/Update.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Update/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.971112 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.003846 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.022274 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.043424 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.061219 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.083630 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.123784 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.130765 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.151045 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.156976 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.172546 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.185558 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.197709 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.207209 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13357 2023-07-06 17:15:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.208391 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.209420 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.210370 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.211430 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.212624 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.213626 CollabConnector-0.1.1691096500/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15084 2023-07-06 17:15:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.215210 CollabConnector-0.1.1691096500/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.217188 CollabConnector-0.1.1691096500/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1691096500/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1691096500/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.219019 CollabConnector-0.1.1691096500/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.221134 CollabConnector-0.1.1691096500/src/CollabConnector/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.222752 CollabConnector-0.1.1691096500/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 CollabConnector-0.1.1691096500/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.226892 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/CallControl.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9430 2023-05-12 11:49:22.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/ContactCenter.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:48.229424 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/
--rw-r--r--   0 jonsnipes   (501) staff       (20)      436 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/Chat.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4593 2023-08-03 21:01:38.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      886 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/Team.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4504 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/User.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      286 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     7953 2023-07-07 19:41:37.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096500/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1691096500/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:01:47.979150 CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-08-03 21:01:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4653 2023-08-03 21:01:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-08-03 21:01:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-08-03 21:01:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-08-03 21:01:47.000000 CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.792777 CollabConnector-0.1.1691096699/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1691096699/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-08-03 21:05:07.792903 CollabConnector-0.1.1691096699/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1691096699/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1691096699/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-08-03 21:05:07.793556 CollabConnector-0.1.1691096699/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.538586 CollabConnector-0.1.1691096699/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.546733 CollabConnector-0.1.1691096699/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.549567 CollabConnector-0.1.1691096699/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.551063 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.552436 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10787 2023-07-06 17:10:27.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.553753 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/AXL.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.556111 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Add/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Add/Add.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Add/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.557125 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Do/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Do/Do.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Do/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.559066 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Get/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Get/Get.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Get/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.561335 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/List/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/List/List.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/List/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.562811 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Remove/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Remove/Remove.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Remove/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.564963 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Update/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Update/Update.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Update/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.542532 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.571648 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.590837 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.609011 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.625910 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.648947 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.684429 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.690677 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.708560 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.714980 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.730024 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.744281 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.758300 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.768085 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13357 2023-07-06 17:15:47.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.769425 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.770633 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.771804 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.773382 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.774901 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.776559 CollabConnector-0.1.1691096699/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15084 2023-07-06 17:15:47.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.778950 CollabConnector-0.1.1691096699/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.781316 CollabConnector-0.1.1691096699/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1691096699/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1691096699/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.783050 CollabConnector-0.1.1691096699/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.784793 CollabConnector-0.1.1691096699/src/CollabConnector/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.786223 CollabConnector-0.1.1691096699/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 CollabConnector-0.1.1691096699/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.789231 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/CallControl.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9430 2023-05-12 11:49:22.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/ContactCenter.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.792196 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      436 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/Chat.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4593 2023-08-03 21:01:38.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      886 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/Team.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4504 2023-08-03 20:46:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/User.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      287 2023-08-03 21:04:52.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     7953 2023-07-07 19:41:37.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1691096699/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1691096699/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-08-03 21:05:07.548518 CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-08-03 21:05:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4653 2023-08-03 21:05:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-08-03 21:05:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-08-03 21:05:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-08-03 21:05:07.000000 CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `CollabConnector-0.1.1691096500/LICENSE` & `CollabConnector-0.1.1691096699/LICENSE`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/PKG-INFO` & `CollabConnector-0.1.1691096699/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1691096500
+Version: 0.1.1691096699
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1691096500/README.md` & `CollabConnector-0.1.1691096699/README.md`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/setup.cfg` & `CollabConnector-0.1.1691096699/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1691096500
+version = 0.1.1691096699
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CER/CER.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AST/AST.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/AXL.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Add/Add.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Add/Add.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Do/Do.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Do/Do.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Get/Get.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Get/Get.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/List/List.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/List/List.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Remove/Remove.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Remove/Remove.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/Update/Update.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/Update/Update.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CDR/CDR.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/CUCM.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/DIME/DIME.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Logs/Logs.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Risport/Risport.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCM/UDS/UDS.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/CUCX/CUCX.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Expressway/Expressway.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/IOS/IOS.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/PAWS/PAWS.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Phone/Phone.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/UCCX/UCCX.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/CallControl.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/CallControl.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/ContactCenter.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/ContactCenter.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/REST.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/REST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/Team.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/Team.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Engage/User.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Engage/User.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/OutputStyle.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector/Webex/Webex.py` & `CollabConnector-0.1.1691096699/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/PKG-INFO` & `CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1691096500
+Version: 0.1.1691096699
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1691096500/src/CollabConnector.egg-info/SOURCES.txt` & `CollabConnector-0.1.1691096699/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

