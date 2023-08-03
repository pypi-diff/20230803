# Comparing `tmp/dash-enterprise-auth-0.1.0.tar.gz` & `tmp/dash-enterprise-auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dash-enterprise-auth-0.1.0.tar", last modified: Wed Jun 22 18:48:08 2022, max compression
+gzip compressed data, was "dash-enterprise-auth-0.1.1.tar", last modified: Thu Mar  9 17:11:57 2023, max compression
```

## Comparing `dash-enterprise-auth-0.1.0.tar` & `dash-enterprise-auth-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3895 2022-06-22 18:47:58.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4835 2022-06-22 18:47:58.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth/_api_requests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2022-06-22 18:47:58.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      352 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-06-22 18:47:58.000000 dash-enterprise-auth-0.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2022-06-22 18:47:58.000000 dash-enterprise-auth-0.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1169 2022-06-22 18:47:58.000000 dash-enterprise-auth-0.1.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-06-22 18:48:08.000000 dash-enterprise-auth-0.1.0/setup.cfg
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-03-09 17:11:57.231995 dash-enterprise-auth-0.1.1/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       18 2022-05-11 23:24:25.000000 dash-enterprise-auth-0.1.1/MANIFEST.in
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      807 2023-03-09 17:11:57.231995 dash-enterprise-auth-0.1.1/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       58 2022-05-11 23:24:25.000000 dash-enterprise-auth-0.1.1/README.md
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-03-09 17:11:57.231995 dash-enterprise-auth-0.1.1/dash_enterprise_auth/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     4498 2023-03-09 17:06:36.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth/__init__.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     4835 2022-05-11 23:24:25.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth/_api_requests.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       22 2023-03-09 17:06:36.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth/version.py
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-03-09 17:11:57.231995 dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      807 2023-03-09 17:11:57.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      352 2023-03-09 17:11:57.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        1 2023-03-09 17:11:57.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       52 2023-03-09 17:11:57.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/requires.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       21 2023-03-09 17:11:57.000000 dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/top_level.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       38 2023-03-09 17:11:57.231995 dash-enterprise-auth-0.1.1/setup.cfg
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1169 2022-05-30 17:39:11.000000 dash-enterprise-auth-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dash-enterprise-auth-0.1.0/dash_enterprise_auth/__init__.py` & `dash-enterprise-auth-0.1.1/dash_enterprise_auth/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import base64 as _b64
 import functools as _ft
 import json as _json
 import jwt as _jwt
 import urllib as _urllib
 from typing import Any
 
+import requests as _requests
+
 import dash as _dash
 if hasattr(_dash, "dcc"):
     _dcc = _dash.dcc
 else:
     import dash_core_components as _dcc
 if hasattr(_dash, "html"):
     _html = _dash.html
@@ -83,35 +85,55 @@
             style={'textDecoration': 'none'}
         ),
         className='dash-logout-frame',
         style=btn_style
     )
 
 
+def _get_decoded_token(name):
+    token = _flask.request.cookies.get(name)
+    return _b64.b64decode(token)
+
+
 @_need_request_context
 def get_user_data():
     jwks_url = _os.getenv('DASH_JWKS_URL')
+    info_url = _os.getenv('DASH_USER_INFO_URL')
     if not jwks_url:
         return _json.loads(_flask.request.headers.get('Plotly-User-Data', "{}"))
     try:
         jwks_client = UaPyJWKClient(jwks_url)
 
-        b64token = _flask.request.cookies.get('kcIdToken')
-        token = _b64.b64decode(b64token)
+        token = _get_decoded_token('kcIdToken')
         signing_key = jwks_client.get_signing_key_from_jwt(token)
 
-        return _jwt.decode(
+        info = _jwt.decode(
             token,
             signing_key.key,
             algorithms=[signing_key._jwk_data.get('alg', 'RSA256')],
             audience=_os.getenv('DASH_AUD', "dash"),
-            options={"verify_exp": True},
+            options={'verify_exp': True},
         )
+        if info_url:
+            tok = _get_decoded_token('kcToken')
+            authorization = f'Bearer {tok.decode()}'
+            response = _requests.get(
+                info_url,
+                headers={
+                    'User-Agent': ua_string,
+                    'Authorization': authorization,
+                }
+            )
+            response.raise_for_status()
+            data = response.json()
+            info.update(data)
+
+        return info
     except Exception as e:
-        print("JWT decode error: " + repr(e))
+        print('JWT decode error: ' + repr(e))
     return {}
 
 
 @_need_request_context
 def get_username():
     """
     Get the current user.
```

### Comparing `dash-enterprise-auth-0.1.0/dash_enterprise_auth/_api_requests.py` & `dash-enterprise-auth-0.1.1/dash_enterprise_auth/_api_requests.py`

 * *Files identical despite different names*

### Comparing `dash-enterprise-auth-0.1.0/dash_enterprise_auth.egg-info/PKG-INFO` & `dash-enterprise-auth-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dash-enterprise-auth
-Version: 0.1.0
+Version: 0.1.1
 Summary: Authentication integrations for dash apps using dash-deployment-server
 Home-page: UNKNOWN
 Author: Antoine Roy-Gobeil
 Author-email: antoine@plotly.com
 License: UNKNOWN
-Description: # dash-enterprise-auth
-        Authentication for dash enterprise
-        
 Keywords: dash dash-enterprise dash-auth plotly
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
+
+# dash-enterprise-auth
+Authentication for dash enterprise
+
+
```

### Comparing `dash-enterprise-auth-0.1.0/setup.py` & `dash-enterprise-auth-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dash-enterprise-auth-0.1.0/PKG-INFO` & `dash-enterprise-auth-0.1.1/dash_enterprise_auth.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dash-enterprise-auth
-Version: 0.1.0
+Version: 0.1.1
 Summary: Authentication integrations for dash apps using dash-deployment-server
 Home-page: UNKNOWN
 Author: Antoine Roy-Gobeil
 Author-email: antoine@plotly.com
 License: UNKNOWN
-Description: # dash-enterprise-auth
-        Authentication for dash enterprise
-        
 Keywords: dash dash-enterprise dash-auth plotly
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
+
+# dash-enterprise-auth
+Authentication for dash enterprise
+
+
```

