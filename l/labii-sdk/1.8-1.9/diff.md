# Comparing `tmp/labii-sdk-1.8.tar.gz` & `tmp/labii-sdk-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labii-sdk-1.8.tar", last modified: Mon Feb 28 10:57:16 2022, max compression
+gzip compressed data, was "labii-sdk-1.9.tar", last modified: Wed Apr 20 10:15:06 2022, max compression
```

## Comparing `labii-sdk-1.8.tar` & `labii-sdk-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yongganwu   (501) staff       (20)        0 2022-02-28 10:57:16.261273 labii-sdk-1.8/
--rw-r--r--   0 yongganwu   (501) staff       (20)      755 2022-02-22 22:31:03.000000 labii-sdk-1.8/LICENSE
-drwxr-xr-x   0 yongganwu   (501) staff       (20)        0 2022-02-28 10:57:16.260044 labii-sdk-1.8/Labii_SDK.egg-info/
--rw-r--r--   0 yongganwu   (501) staff       (20)     2317 2022-02-28 10:57:16.000000 labii-sdk-1.8/Labii_SDK.egg-info/PKG-INFO
--rw-r--r--   0 yongganwu   (501) staff       (20)      619 2022-02-28 10:57:16.000000 labii-sdk-1.8/Labii_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 yongganwu   (501) staff       (20)        1 2022-02-28 10:57:16.000000 labii-sdk-1.8/Labii_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 yongganwu   (501) staff       (20)       32 2022-02-28 10:57:16.000000 labii-sdk-1.8/Labii_SDK.egg-info/requires.txt
--rw-r--r--   0 yongganwu   (501) staff       (20)       10 2022-02-28 10:57:16.000000 labii-sdk-1.8/Labii_SDK.egg-info/top_level.txt
--rw-r--r--   0 yongganwu   (501) staff       (20)       19 2022-02-23 07:25:42.000000 labii-sdk-1.8/MANIFEST.in
--rw-r--r--   0 yongganwu   (501) staff       (20)     2317 2022-02-28 10:57:16.261105 labii-sdk-1.8/PKG-INFO
--rw-r--r--   0 yongganwu   (501) staff       (20)     1813 2022-02-28 10:55:15.000000 labii-sdk-1.8/README.md
--rw-r--r--   0 yongganwu   (501) staff       (20)     1132 2022-02-28 10:55:25.000000 labii-sdk-1.8/VERSION.md
-drwxr-xr-x   0 yongganwu   (501) staff       (20)        0 2022-02-28 10:57:16.260662 labii-sdk-1.8/labii_sdk/
--rw-r--r--   0 yongganwu   (501) staff       (20)        0 2022-02-22 22:31:03.000000 labii-sdk-1.8/labii_sdk/__init__.py
--rw-r--r--   0 yongganwu   (501) staff       (20)     9224 2022-02-28 10:55:15.000000 labii-sdk-1.8/labii_sdk/api_client.py
--rw-r--r--   0 yongganwu   (501) staff       (20)     6769 2022-02-28 10:55:15.000000 labii-sdk-1.8/labii_sdk/sdk.py
--rw-r--r--   0 yongganwu   (501) staff       (20)      177 2022-02-23 07:25:42.000000 labii-sdk-1.8/pyproject.toml
--rw-r--r--   0 yongganwu   (501) staff       (20)       38 2022-02-28 10:57:16.261333 labii-sdk-1.8/setup.cfg
--rw-r--r--   0 yongganwu   (501) staff       (20)     1046 2022-02-23 07:25:42.000000 labii-sdk-1.8/setup.py
+drwxr-xr-x   0 yongganwu   (501) staff       (20)        0 2022-04-20 10:15:06.552828 labii-sdk-1.9/
+-rw-r--r--   0 yongganwu   (501) staff       (20)      755 2022-02-22 22:31:03.000000 labii-sdk-1.9/LICENSE
+drwxr-xr-x   0 yongganwu   (501) staff       (20)        0 2022-04-20 10:15:06.551185 labii-sdk-1.9/Labii_SDK.egg-info/
+-rw-r--r--   0 yongganwu   (501) staff       (20)     2317 2022-04-20 10:15:06.000000 labii-sdk-1.9/Labii_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 yongganwu   (501) staff       (20)      619 2022-04-20 10:15:06.000000 labii-sdk-1.9/Labii_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 yongganwu   (501) staff       (20)        1 2022-04-20 10:15:06.000000 labii-sdk-1.9/Labii_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 yongganwu   (501) staff       (20)       32 2022-04-20 10:15:06.000000 labii-sdk-1.9/Labii_SDK.egg-info/requires.txt
+-rw-r--r--   0 yongganwu   (501) staff       (20)       10 2022-04-20 10:15:06.000000 labii-sdk-1.9/Labii_SDK.egg-info/top_level.txt
+-rw-r--r--   0 yongganwu   (501) staff       (20)       19 2022-02-23 07:25:42.000000 labii-sdk-1.9/MANIFEST.in
+-rw-r--r--   0 yongganwu   (501) staff       (20)     2317 2022-04-20 10:15:06.552639 labii-sdk-1.9/PKG-INFO
+-rw-r--r--   0 yongganwu   (501) staff       (20)     1813 2022-02-28 10:55:15.000000 labii-sdk-1.9/README.md
+-rw-r--r--   0 yongganwu   (501) staff       (20)     1177 2022-04-20 10:13:58.000000 labii-sdk-1.9/VERSION.md
+drwxr-xr-x   0 yongganwu   (501) staff       (20)        0 2022-04-20 10:15:06.552076 labii-sdk-1.9/labii_sdk/
+-rw-r--r--   0 yongganwu   (501) staff       (20)        0 2022-02-22 22:31:03.000000 labii-sdk-1.9/labii_sdk/__init__.py
+-rw-r--r--   0 yongganwu   (501) staff       (20)     9262 2022-04-20 10:13:47.000000 labii-sdk-1.9/labii_sdk/api_client.py
+-rw-r--r--   0 yongganwu   (501) staff       (20)    10469 2022-04-20 10:13:47.000000 labii-sdk-1.9/labii_sdk/sdk.py
+-rw-r--r--   0 yongganwu   (501) staff       (20)      177 2022-02-23 07:25:42.000000 labii-sdk-1.9/pyproject.toml
+-rw-r--r--   0 yongganwu   (501) staff       (20)       38 2022-04-20 10:15:06.552885 labii-sdk-1.9/setup.cfg
+-rw-r--r--   0 yongganwu   (501) staff       (20)     1046 2022-02-23 07:25:42.000000 labii-sdk-1.9/setup.py
```

### Comparing `labii-sdk-1.8/LICENSE` & `labii-sdk-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `labii-sdk-1.8/Labii_SDK.egg-info/PKG-INFO` & `labii-sdk-1.9/Labii_SDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labii-sdk
-Version: 1.8
+Version: 1.9
 Summary: An SDK for the Labii ELN & LIMS platform (https://www.labii.com) that provides interaction with the Labii API.
 Home-page: https://gitlab.com/labii-dev/labii-sdk
 Author: Labii Inc.
 Author-email: developer@labii.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://gitlab.com/labii-dev/labii-sdk/-/issues?sort=created_date&state=opened
 Platform: UNKNOWN
```

### Comparing `labii-sdk-1.8/Labii_SDK.egg-info/SOURCES.txt` & `labii-sdk-1.9/Labii_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labii-sdk-1.8/PKG-INFO` & `labii-sdk-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labii-sdk
-Version: 1.8
+Version: 1.9
 Summary: An SDK for the Labii ELN & LIMS platform (https://www.labii.com) that provides interaction with the Labii API.
 Home-page: https://gitlab.com/labii-dev/labii-sdk
 Author: Labii Inc.
 Author-email: developer@labii.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://gitlab.com/labii-dev/labii-sdk/-/issues?sort=created_date&state=opened
 Platform: UNKNOWN
```

### Comparing `labii-sdk-1.8/README.md` & `labii-sdk-1.9/README.md`

 * *Files identical despite different names*

### Comparing `labii-sdk-1.8/VERSION.md` & `labii-sdk-1.9/VERSION.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 |2022-02-22|__v1.02__|updated readme links||
 |2022-02-22|__v1.03__|support more objects||
 |2022-02-22|__v1.04__|support more models||
 |2022-02-22|__v1.05__|fixed a bug to load all pages||
 |2022-02-23|__v1.06__|fixed bug to load user info||
 |2022-02-23|__v1.07__|support query in sdk methods||
 |2022-02-28|__v1.08__|support file uploading||
+|2022-04-20|__v1.09__|support folder watch||
```

### Comparing `labii-sdk-1.8/labii_sdk/api_client.py` & `labii-sdk-1.9/labii_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,18 @@
         else:
             raise RuntimeError(response)
 
     def check_token(self):
         """Check if the exist token is valid. If not valid, it will genereate a new token
             Labii token expires after 30 minutes of no activity. If your program take more than 30 minutes to run. Use this function to get a new token.
         """
-        data = self.get("/accounts/checktoken/")
-        if data["detail"] != "Valid token.":
+        try:
+            data = self.get("/accounts/checktoken/")
+        except:
+            #if data["detail"] != "Valid token.":
             self.login()
 
     ######
     # api post
     def post(self, url, data, is_authorized=True):
         """A function to do POST for labii api
```

### Comparing `labii-sdk-1.8/setup.py` & `labii-sdk-1.9/setup.py`

 * *Files identical despite different names*

