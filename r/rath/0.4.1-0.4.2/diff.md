# Comparing `tmp/rath-0.4.1.tar.gz` & `tmp/rath-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rath-0.4.1.tar", max compression
+gzip compressed data, was "rath-0.4.2.tar", max compression
```

## Comparing `rath-0.4.1.tar` & `rath-0.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     4921 2022-11-21 12:07:57.958148 rath-0.4.1/README.md
--rw-r--r--   0        0        0     1467 2023-08-03 10:47:52.944108 rath-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       43 2022-04-12 10:04:18.856216 rath-0.4.1/rath/__init__.py
--rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.4.1/rath/contrib/fakts/__init__.py
--rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.4.1/rath/contrib/fakts/links/__init__.py
--rw-r--r--   0        0        0     1188 2023-08-02 10:24:16.092036 rath-0.4.1/rath/contrib/fakts/links/aiohttp.py
--rw-r--r--   0        0        0      836 2023-08-02 11:51:30.163471 rath-0.4.1/rath/contrib/fakts/links/graphql_ws.py
--rw-r--r--   0        0        0      836 2023-08-02 10:25:04.696296 rath-0.4.1/rath/contrib/fakts/links/httpx.py
--rw-r--r--   0        0        0      965 2023-08-02 11:51:35.203500 rath-0.4.1/rath/contrib/fakts/links/subscription_transport_ws.py
--rw-r--r--   0        0        0      410 2023-08-02 10:25:47.464525 rath-0.4.1/rath/contrib/herre/links/auth.py
--rw-r--r--   0        0        0      429 2023-08-02 09:25:39.868383 rath-0.4.1/rath/errors.py
--rw-r--r--   0        0        0       86 2022-04-12 10:04:18.856216 rath-0.4.1/rath/links/__init__.py
--rw-r--r--   0        0        0     5117 2023-08-02 09:25:17.348258 rath-0.4.1/rath/links/aiohttp.py
--rw-r--r--   0        0        0     3128 2023-08-03 10:43:56.262732 rath-0.4.1/rath/links/auth.py
--rw-r--r--   0        0        0     2624 2023-08-02 09:26:14.480573 rath-0.4.1/rath/links/base.py
--rw-r--r--   0        0        0     3680 2023-08-02 09:26:26.408638 rath-0.4.1/rath/links/compose.py
--rw-r--r--   0        0        0     1733 2023-08-02 09:24:27.551981 rath-0.4.1/rath/links/dictinglink.py
--rw-r--r--   0        0        0      658 2023-08-02 09:24:27.535981 rath-0.4.1/rath/links/errors.py
--rw-r--r--   0        0        0     2402 2022-11-21 12:38:21.551691 rath-0.4.1/rath/links/file.py
--rw-r--r--   0        0        0      758 2023-07-31 15:05:51.639285 rath-0.4.1/rath/links/foward.py
--rw-r--r--   0        0        0    12157 2023-08-02 09:24:00.691830 rath-0.4.1/rath/links/graphql_ws.py
--rw-r--r--   0        0        0     3083 2023-08-02 09:26:31.284665 rath-0.4.1/rath/links/httpx.py
--rw-r--r--   0        0        0      755 2023-08-02 09:26:38.880706 rath-0.4.1/rath/links/log.py
--rw-r--r--   0        0        0      628 2023-08-02 09:24:27.535981 rath-0.4.1/rath/links/parsing.py
--rw-r--r--   0        0        0     1688 2023-05-28 12:40:04.463984 rath-0.4.1/rath/links/retry.py
--rw-r--r--   0        0        0      735 2023-08-02 09:24:27.539981 rath-0.4.1/rath/links/shrink.py
--rw-r--r--   0        0        0     1716 2023-08-03 10:46:11.747521 rath-0.4.1/rath/links/sign_local_link.py
--rw-r--r--   0        0        0     1947 2023-07-31 14:50:32.714120 rath-0.4.1/rath/links/split.py
--rw-r--r--   0        0        0    11681 2023-08-02 09:26:43.452731 rath-0.4.1/rath/links/subscription_transport_ws.py
--rw-r--r--   0        0        0        0 2022-02-18 09:52:41.143787 rath-0.4.1/rath/links/testing/__init__.py
--rw-r--r--   0        0        0      538 2023-08-03 09:54:16.948890 rath-0.4.1/rath/links/testing/assert_link.py
--rw-r--r--   0        0        0       91 2022-03-14 16:31:19.964012 rath-0.4.1/rath/links/testing/check.py
--rw-r--r--   0        0        0     4441 2022-04-12 10:04:18.856216 rath-0.4.1/rath/links/testing/mock.py
--rw-r--r--   0        0        0     7576 2023-08-02 09:27:12.180888 rath-0.4.1/rath/links/testing/statefulmock.py
--rw-r--r--   0        0        0      434 2023-08-03 10:00:49.883349 rath-0.4.1/rath/links/testing/utils.py
--rw-r--r--   0        0        0     9937 2023-08-02 09:29:11.489529 rath-0.4.1/rath/links/transpile.py
--rw-r--r--   0        0        0     3109 2022-04-12 10:04:18.856216 rath-0.4.1/rath/links/utils.py
--rw-r--r--   0        0        0     4022 2023-08-02 09:24:27.583981 rath-0.4.1/rath/links/validate.py
--rw-r--r--   0        0        0     2973 2023-07-31 15:17:57.763465 rath-0.4.1/rath/operation.py
--rw-r--r--   0        0        0       60 2022-04-12 10:04:18.856216 rath-0.4.1/rath/qt/__init__.py
--rw-r--r--   0        0        0      839 2022-09-23 09:27:15.868008 rath-0.4.1/rath/qt/helpers.py
--rw-r--r--   0        0        0     6889 2023-07-31 16:51:14.008216 rath-0.4.1/rath/rath.py
--rw-r--r--   0        0        0     1029 2022-07-24 12:46:45.543098 rath-0.4.1/rath/scalars.py
--rw-r--r--   0        0        0        0 2022-01-28 15:19:12.944704 rath-0.4.1/rath/turms/__init__.py
--rw-r--r--   0        0        0      826 2022-04-12 10:04:18.856216 rath-0.4.1/rath/turms/funcs.py
--rw-r--r--   0        0        0        0 2022-03-14 16:31:19.964012 rath-0.4.1/rath/turms/plugins/__init__.py
--rw-r--r--   0        0        0     1350 2022-08-25 12:16:33.053621 rath-0.4.1/rath/turms/plugins/funcs.py
--rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 rath-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4921 2022-11-21 12:07:57.958148 rath-0.4.2/README.md
+-rw-r--r--   0        0        0     1467 2023-08-03 11:23:40.948075 rath-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2022-04-12 10:04:18.856216 rath-0.4.2/rath/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.4.2/rath/contrib/fakts/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.4.2/rath/contrib/fakts/links/__init__.py
+-rw-r--r--   0        0        0     1188 2023-08-02 10:24:16.092036 rath-0.4.2/rath/contrib/fakts/links/aiohttp.py
+-rw-r--r--   0        0        0      836 2023-08-02 11:51:30.163471 rath-0.4.2/rath/contrib/fakts/links/graphql_ws.py
+-rw-r--r--   0        0        0      836 2023-08-02 10:25:04.696296 rath-0.4.2/rath/contrib/fakts/links/httpx.py
+-rw-r--r--   0        0        0      965 2023-08-02 11:51:35.203500 rath-0.4.2/rath/contrib/fakts/links/subscription_transport_ws.py
+-rw-r--r--   0        0        0      410 2023-08-02 10:25:47.464525 rath-0.4.2/rath/contrib/herre/links/auth.py
+-rw-r--r--   0        0        0      429 2023-08-02 09:25:39.868383 rath-0.4.2/rath/errors.py
+-rw-r--r--   0        0        0       86 2022-04-12 10:04:18.856216 rath-0.4.2/rath/links/__init__.py
+-rw-r--r--   0        0        0     5117 2023-08-02 09:25:17.348258 rath-0.4.2/rath/links/aiohttp.py
+-rw-r--r--   0        0        0     3128 2023-08-03 10:43:56.262732 rath-0.4.2/rath/links/auth.py
+-rw-r--r--   0        0        0     2624 2023-08-02 09:26:14.480573 rath-0.4.2/rath/links/base.py
+-rw-r--r--   0        0        0     3680 2023-08-02 09:26:26.408638 rath-0.4.2/rath/links/compose.py
+-rw-r--r--   0        0        0     1733 2023-08-02 09:24:27.551981 rath-0.4.2/rath/links/dictinglink.py
+-rw-r--r--   0        0        0      658 2023-08-02 09:24:27.535981 rath-0.4.2/rath/links/errors.py
+-rw-r--r--   0        0        0     2402 2022-11-21 12:38:21.551691 rath-0.4.2/rath/links/file.py
+-rw-r--r--   0        0        0      758 2023-07-31 15:05:51.639285 rath-0.4.2/rath/links/foward.py
+-rw-r--r--   0        0        0    12157 2023-08-02 09:24:00.691830 rath-0.4.2/rath/links/graphql_ws.py
+-rw-r--r--   0        0        0     3083 2023-08-02 09:26:31.284665 rath-0.4.2/rath/links/httpx.py
+-rw-r--r--   0        0        0      755 2023-08-02 09:26:38.880706 rath-0.4.2/rath/links/log.py
+-rw-r--r--   0        0        0      628 2023-08-02 09:24:27.535981 rath-0.4.2/rath/links/parsing.py
+-rw-r--r--   0        0        0     1688 2023-05-28 12:40:04.463984 rath-0.4.2/rath/links/retry.py
+-rw-r--r--   0        0        0      735 2023-08-02 09:24:27.539981 rath-0.4.2/rath/links/shrink.py
+-rw-r--r--   0        0        0     1816 2023-08-03 11:23:39.676068 rath-0.4.2/rath/links/sign_local_link.py
+-rw-r--r--   0        0        0     1947 2023-07-31 14:50:32.714120 rath-0.4.2/rath/links/split.py
+-rw-r--r--   0        0        0    11681 2023-08-02 09:26:43.452731 rath-0.4.2/rath/links/subscription_transport_ws.py
+-rw-r--r--   0        0        0        0 2022-02-18 09:52:41.143787 rath-0.4.2/rath/links/testing/__init__.py
+-rw-r--r--   0        0        0      538 2023-08-03 09:54:16.948890 rath-0.4.2/rath/links/testing/assert_link.py
+-rw-r--r--   0        0        0       91 2022-03-14 16:31:19.964012 rath-0.4.2/rath/links/testing/check.py
+-rw-r--r--   0        0        0     4441 2022-04-12 10:04:18.856216 rath-0.4.2/rath/links/testing/mock.py
+-rw-r--r--   0        0        0     7576 2023-08-02 09:27:12.180888 rath-0.4.2/rath/links/testing/statefulmock.py
+-rw-r--r--   0        0        0      434 2023-08-03 10:00:49.883349 rath-0.4.2/rath/links/testing/utils.py
+-rw-r--r--   0        0        0     9937 2023-08-02 09:29:11.489529 rath-0.4.2/rath/links/transpile.py
+-rw-r--r--   0        0        0     3109 2022-04-12 10:04:18.856216 rath-0.4.2/rath/links/utils.py
+-rw-r--r--   0        0        0     4022 2023-08-02 09:24:27.583981 rath-0.4.2/rath/links/validate.py
+-rw-r--r--   0        0        0     2973 2023-07-31 15:17:57.763465 rath-0.4.2/rath/operation.py
+-rw-r--r--   0        0        0       60 2022-04-12 10:04:18.856216 rath-0.4.2/rath/qt/__init__.py
+-rw-r--r--   0        0        0      839 2022-09-23 09:27:15.868008 rath-0.4.2/rath/qt/helpers.py
+-rw-r--r--   0        0        0     6889 2023-07-31 16:51:14.008216 rath-0.4.2/rath/rath.py
+-rw-r--r--   0        0        0     1029 2022-07-24 12:46:45.543098 rath-0.4.2/rath/scalars.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:19:12.944704 rath-0.4.2/rath/turms/__init__.py
+-rw-r--r--   0        0        0      826 2022-04-12 10:04:18.856216 rath-0.4.2/rath/turms/funcs.py
+-rw-r--r--   0        0        0        0 2022-03-14 16:31:19.964012 rath-0.4.2/rath/turms/plugins/__init__.py
+-rw-r--r--   0        0        0     1350 2022-08-25 12:16:33.053621 rath-0.4.2/rath/turms/plugins/funcs.py
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 rath-0.4.2/PKG-INFO
```

### Comparing `rath-0.4.1/README.md` & `rath-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/pyproject.toml` & `rath-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rath"
-version = "0.4.1"
+version = "0.4.2"
 description = "async transport-agnostic graphql client"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "rath" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `rath-0.4.1/rath/contrib/fakts/links/aiohttp.py` & `rath-0.4.2/rath/contrib/fakts/links/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/contrib/fakts/links/graphql_ws.py` & `rath-0.4.2/rath/contrib/fakts/links/graphql_ws.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/contrib/fakts/links/httpx.py` & `rath-0.4.2/rath/contrib/fakts/links/httpx.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/contrib/fakts/links/subscription_transport_ws.py` & `rath-0.4.2/rath/contrib/fakts/links/subscription_transport_ws.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/aiohttp.py` & `rath-0.4.2/rath/links/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/auth.py` & `rath-0.4.2/rath/links/auth.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/base.py` & `rath-0.4.2/rath/links/base.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/compose.py` & `rath-0.4.2/rath/links/compose.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/dictinglink.py` & `rath-0.4.2/rath/links/dictinglink.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/errors.py` & `rath-0.4.2/rath/links/errors.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/file.py` & `rath-0.4.2/rath/links/file.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/foward.py` & `rath-0.4.2/rath/links/foward.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/graphql_ws.py` & `rath-0.4.2/rath/links/graphql_ws.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/httpx.py` & `rath-0.4.2/rath/links/httpx.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/log.py` & `rath-0.4.2/rath/links/log.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/parsing.py` & `rath-0.4.2/rath/links/parsing.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/retry.py` & `rath-0.4.2/rath/links/retry.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/shrink.py` & `rath-0.4.2/rath/links/shrink.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/sign_local_link.py` & `rath-0.4.2/rath/links/sign_local_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from .auth import AuthTokenLink
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
-from pydantic import validator, ValidationError
+from pydantic import validator
 from cryptography.hazmat.primitives.asymmetric import rsa
 from typing import Any, Callable, Awaitable, Dict
 import jwt
 import datetime
 from rath.operation import Operation
 
 
 class SignLocalLink(AuthTokenLink):
     private_key: rsa.RSAPrivateKey
 
     @validator("private_key", pre=True, always=True)
     def must_be_valid_pem_key(cls, v: Any) -> str:
         try:
-            if isinstance(v, str):
-                with open(v, "rb") as f:
-                    v = f.read()
+            try:
+                if isinstance(v, str):
+                    with open(v, "rb") as f:
+                        v = f.read()
+            except Exception as e:
+                raise ValueError("Could not read file") from e
 
             key = serialization.load_pem_private_key(
                 v, password=None, backend=default_backend()
             )
 
             # Check if it is an RSA key
             if not isinstance(key, rsa.RSAPrivateKey):
-                raise ValidationError("PEM key is not an RSA Private key.")
+                raise ValueError("PEM key is not an RSA Private key.")
 
             return key
         except Exception as e:
-            raise ValidationError(f"Not a valid PEM key. {str(e)}")
+            raise ValueError(f"Not a valid PEM key. {str(e)}")
 
     async def aretrieve_payload(self, Operation):
         raise NotImplementedError("Please implement this method.")
 
     async def aload_token(self, operation: Operation):
         payload = await self.aretrieve_payload(operation)
         token = jwt.encode(payload, key=self.private_key, algorithm="RS256")
```

### Comparing `rath-0.4.1/rath/links/split.py` & `rath-0.4.2/rath/links/split.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/subscription_transport_ws.py` & `rath-0.4.2/rath/links/subscription_transport_ws.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/testing/assert_link.py` & `rath-0.4.2/rath/links/testing/assert_link.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/testing/mock.py` & `rath-0.4.2/rath/links/testing/mock.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/testing/statefulmock.py` & `rath-0.4.2/rath/links/testing/statefulmock.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/transpile.py` & `rath-0.4.2/rath/links/transpile.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/utils.py` & `rath-0.4.2/rath/links/utils.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/links/validate.py` & `rath-0.4.2/rath/links/validate.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/operation.py` & `rath-0.4.2/rath/operation.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/qt/helpers.py` & `rath-0.4.2/rath/qt/helpers.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/rath.py` & `rath-0.4.2/rath/rath.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/scalars.py` & `rath-0.4.2/rath/scalars.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/turms/funcs.py` & `rath-0.4.2/rath/turms/funcs.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/rath/turms/plugins/funcs.py` & `rath-0.4.2/rath/turms/plugins/funcs.py`

 * *Files identical despite different names*

### Comparing `rath-0.4.1/PKG-INFO` & `rath-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rath
-Version: 0.4.1
+Version: 0.4.2
 Summary: async transport-agnostic graphql client
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

