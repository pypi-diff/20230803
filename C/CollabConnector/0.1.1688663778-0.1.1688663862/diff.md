# Comparing `tmp/CollabConnector-0.1.1688663778.tar.gz` & `tmp/CollabConnector-0.1.1688663862.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CollabConnector-0.1.1688663778.tar", last modified: Thu Jul  6 17:16:25 2023, max compression
+gzip compressed data, was "CollabConnector-0.1.1688663862.tar", last modified: Thu Jul  6 17:17:49 2023, max compression
```

## Comparing `CollabConnector-0.1.1688663778.tar` & `CollabConnector-0.1.1688663862.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.982961 CollabConnector-0.1.1688663778/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1688663778/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-07-06 17:16:25.983075 CollabConnector-0.1.1688663778/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1688663778/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1688663778/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-07-06 17:16:25.983623 CollabConnector-0.1.1688663778/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.785198 CollabConnector-0.1.1688663778/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.795378 CollabConnector-0.1.1688663778/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.798191 CollabConnector-0.1.1688663778/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.799111 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.800345 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10787 2023-07-06 17:10:27.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.801596 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/AXL.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.804624 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Add/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Add/Add.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Add/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.805667 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Do/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Do/Do.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Do/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.807839 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Get/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Get/Get.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Get/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.810178 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/List/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/List/List.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/List/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.811536 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Remove/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Remove/Remove.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Remove/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.813502 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Update/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Update/Update.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Update/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.789926 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.819537 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.832473 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.848018 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.860424 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.872624 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.895960 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.901573 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.920311 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.924940 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.937419 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.950344 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.961076 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.969417 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20618 2023-01-24 14:18:53.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13357 2023-07-06 17:15:47.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.970490 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.971322 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.972366 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.973379 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.974534 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.975177 CollabConnector-0.1.1688663778/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15084 2023-07-06 17:15:47.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.975938 CollabConnector-0.1.1688663778/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.977213 CollabConnector-0.1.1688663778/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1688663778/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1688663778/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.978156 CollabConnector-0.1.1688663778/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.979490 CollabConnector-0.1.1688663778/src/CollabConnector/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30949 2023-02-22 19:35:02.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.980488 CollabConnector-0.1.1688663778/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8550 2023-02-22 19:34:41.000000 CollabConnector-0.1.1688663778/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.982716 CollabConnector-0.1.1688663778/src/CollabConnector/Webex/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Webex/CallControl.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9430 2023-05-12 11:49:22.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Webex/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Webex/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     7891 2023-05-12 11:50:53.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663778/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1688663778/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:16:25.797543 CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-07-06 17:16:25.000000 CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4444 2023-07-06 17:16:25.000000 CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-07-06 17:16:25.000000 CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-07-06 17:16:25.000000 CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-07-06 17:16:25.000000 CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.543061 CollabConnector-0.1.1688663862/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1688663862/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-07-06 17:17:49.543180 CollabConnector-0.1.1688663862/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1688663862/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1688663862/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-07-06 17:17:49.543728 CollabConnector-0.1.1688663862/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.311089 CollabConnector-0.1.1688663862/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.321435 CollabConnector-0.1.1688663862/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.325069 CollabConnector-0.1.1688663862/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.326714 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.327988 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10787 2023-07-06 17:10:27.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.329289 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/AXL.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.332126 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Add/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Add/Add.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Add/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.333164 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Do/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Do/Do.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Do/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.335725 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Get/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Get/Get.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Get/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.338521 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/List/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/List/List.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/List/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.340129 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Remove/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Remove/Remove.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Remove/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.342442 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Update/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Update/Update.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Update/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.316013 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.348599 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.364761 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.383191 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.399443 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.414548 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.447410 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.453840 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.474857 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.480263 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.492515 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.505910 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.520259 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.529200 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20618 2023-01-24 14:18:53.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13357 2023-07-06 17:15:47.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.530394 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.531412 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.532400 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.533406 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.534531 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.535580 CollabConnector-0.1.1688663862/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15084 2023-07-06 17:15:47.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.536579 CollabConnector-0.1.1688663862/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.537918 CollabConnector-0.1.1688663862/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1688663862/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1688663862/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.538893 CollabConnector-0.1.1688663862/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.539774 CollabConnector-0.1.1688663862/src/CollabConnector/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.540554 CollabConnector-0.1.1688663862/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 CollabConnector-0.1.1688663862/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.542858 CollabConnector-0.1.1688663862/src/CollabConnector/Webex/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Webex/CallControl.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9430 2023-05-12 11:49:22.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Webex/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Webex/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     7891 2023-05-12 11:50:53.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663862/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1688663862/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:17:49.323858 CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-07-06 17:17:49.000000 CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4444 2023-07-06 17:17:49.000000 CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-07-06 17:17:49.000000 CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-07-06 17:17:49.000000 CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-07-06 17:17:49.000000 CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `CollabConnector-0.1.1688663778/LICENSE` & `CollabConnector-0.1.1688663862/LICENSE`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/PKG-INFO` & `CollabConnector-0.1.1688663862/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1688663778
+Version: 0.1.1688663862
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1688663778/README.md` & `CollabConnector-0.1.1688663862/README.md`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/setup.cfg` & `CollabConnector-0.1.1688663862/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1688663778
+version = 0.1.1688663862
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CER/CER.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AST/AST.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/AXL.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Add/Add.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Add/Add.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Do/Do.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Do/Do.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Get/Get.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Get/Get.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/List/List.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/List/List.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Remove/Remove.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Remove/Remove.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/Update/Update.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/Update/Update.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CDR/CDR.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/CUCM.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/DIME/DIME.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Logs/Logs.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Risport/Risport.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCM/UDS/UDS.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/CUCX/CUCX.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/Expressway/Expressway.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/IOS/IOS.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/PAWS/PAWS.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/Phone/Phone.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/Phone/Phone.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import sys
 import ssl
 import time
 import html
 import os
 
 requests.packages.urllib3.disable_warnings()
-requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 try:
     requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
+    requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 except AttributeError:
     # no pyopenssl support used / needed / available
     pass
 
 
 class Connect():
     device_html = None
```

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/UCCX/UCCX.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/UCCX/UCCX.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import sys
 import re
 import json
 import urllib
 import socket
 
 requests.packages.urllib3.disable_warnings()
-requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 try:
     requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
+    requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 except AttributeError:
     # no pyopenssl support used / needed / available
     pass
 
 class Connect:
 
     # initialize object set system type and build DB connectors as needed
```

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/Webex/CallControl.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/Webex/CallControl.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/Webex/ContactCenter.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/Webex/ContactCenter.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/Webex/OutputStyle.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/Webex/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector/Webex/Webex.py` & `CollabConnector-0.1.1688663862/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/PKG-INFO` & `CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1688663778
+Version: 0.1.1688663862
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1688663778/src/CollabConnector.egg-info/SOURCES.txt` & `CollabConnector-0.1.1688663862/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

