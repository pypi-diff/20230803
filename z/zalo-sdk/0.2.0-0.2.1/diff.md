# Comparing `tmp/zalo_sdk-0.2.0-py3-none-any.whl.zip` & `tmp/zalo_sdk-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9653 bytes, number of entries: 14
+Zip file size: 9673 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     6828 b- defN 23-May-16 15:21 zalo_sdk/BaseClient.py
 -rw-r--r--  2.0 unx      345 b- defN 23-May-16 15:21 zalo_sdk/ZaloException.py
--rw-r--r--  2.0 unx     2399 b- defN 23-May-16 15:21 zalo_sdk/ZaloOAException.py
+-rw-r--r--  2.0 unx     2471 b- defN 23-Aug-03 04:05 zalo_sdk/ZaloOAException.py
 -rw-r--r--  2.0 unx      106 b- defN 23-May-16 15:21 zalo_sdk/__init__.py
 -rw-r--r--  2.0 unx     1629 b- defN 23-Jun-29 02:33 zalo_sdk/oa/Client.py
 -rw-r--r--  2.0 unx     5414 b- defN 23-Apr-19 02:06 zalo_sdk/oa/ZaloMessage.py
 -rw-r--r--  2.0 unx       48 b- defN 23-May-16 15:21 zalo_sdk/oa/__init__.py
 -rw-r--r--  2.0 unx     1691 b- defN 23-May-16 15:21 zalo_sdk/zns/Client.py
 -rw-r--r--  2.0 unx       21 b- defN 23-May-16 15:21 zalo_sdk/zns/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Jun-29 02:35 zalo_sdk-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1779 b- defN 23-Jun-29 02:35 zalo_sdk-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 02:35 zalo_sdk-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-29 02:35 zalo_sdk-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1107 b- defN 23-Jun-29 02:35 zalo_sdk-0.2.0.dist-info/RECORD
-14 files, 22532 bytes uncompressed, 7819 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1064 b- defN 23-Aug-03 04:06 zalo_sdk-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1779 b- defN 23-Aug-03 04:06 zalo_sdk-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 04:06 zalo_sdk-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-03 04:06 zalo_sdk-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Aug-03 04:06 zalo_sdk-0.2.1.dist-info/RECORD
+14 files, 22604 bytes uncompressed, 7839 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: zalo_sdk/zns/Client.py
 Comment: 
 
 Filename: zalo_sdk/zns/__init__.py
 Comment: 
 
-Filename: zalo_sdk-0.2.0.dist-info/LICENSE
+Filename: zalo_sdk-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: zalo_sdk-0.2.0.dist-info/METADATA
+Filename: zalo_sdk-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: zalo_sdk-0.2.0.dist-info/WHEEL
+Filename: zalo_sdk-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: zalo_sdk-0.2.0.dist-info/top_level.txt
+Filename: zalo_sdk-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zalo_sdk-0.2.0.dist-info/RECORD
+Filename: zalo_sdk-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zalo_sdk/ZaloOAException.py

```diff
@@ -27,14 +27,15 @@
         -216: "Invalid Access Token",
         -217: "User blocked invitation to follow",
         -218: "Out of quota for receiving",
         -221: "Official Account has not been authenticated",
         -222: "User account has been blocked or not active for more than 45 days",
         -224: "Official Account has not subscribe to the service package",
         -227: "User account has been blocked or not active for more than 45 days",
+        -230: "User has not interacted with the OA in the past 7 days",
         -305: "Offical Account cannot response to user after 48 hours",
         -311: "Out of quota for responding to user message",
         -320: "Application needs to link with Zalo Business Account to use paid features",
         -321: "Zalo Business Account linked with the Application is low on balance or cannot make payment"
     }
 
     def __init__(self, code, custom_message=None):
```

## Comparing `zalo_sdk-0.2.0.dist-info/LICENSE` & `zalo_sdk-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zalo_sdk-0.2.0.dist-info/METADATA` & `zalo_sdk-0.2.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Zalo SDK
 Home-page: https://github.com/connext-biz/zalo_integration
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
```

