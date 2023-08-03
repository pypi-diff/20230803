# Comparing `tmp/nemusicapi-0.0.4a5.tar.gz` & `tmp/nemusicapi-0.0.4a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.4a5.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.4a6.tar", max compression
```

## Comparing `nemusicapi-0.0.4a5.tar` & `nemusicapi-0.0.4a6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a5/LICENSE
--rw-r--r--   0        0        0      264 2023-08-03 07:50:32.099164 nemusicapi-0.0.4a5/NEmusicApi/__init__.py
--rw-r--r--   0        0        0     4829 2023-08-03 07:51:21.885707 nemusicapi-0.0.4a5/NEmusicApi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a5/NEmusicApi/exception.py
--rw-r--r--   0        0        0      238 2023-08-03 07:46:02.369612 nemusicapi-0.0.4a5/NEmusicApi/type.py
--rw-r--r--   0        0        0      466 2023-08-03 07:51:34.134907 nemusicapi-0.0.4a5/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.4a5/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a5/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a6/LICENSE
+-rw-r--r--   0        0        0      264 2023-08-03 08:15:45.913944 nemusicapi-0.0.4a6/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     4829 2023-08-03 08:15:45.913944 nemusicapi-0.0.4a6/nemusicapi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a6/nemusicapi/exception.py
+-rw-r--r--   0        0        0      338 2023-08-03 08:13:25.809448 nemusicapi-0.0.4a6/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-03 08:16:29.181517 nemusicapi-0.0.4a6/pyproject.toml
+-rw-r--r--   0        0        0     1285 2023-08-03 08:27:02.179801 nemusicapi-0.0.4a6/README.md
+-rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a6/PKG-INFO
```

### Comparing `nemusicapi-0.0.4a5/LICENSE` & `nemusicapi-0.0.4a6/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.4a5/NEmusicApi/api.py` & `nemusicapi-0.0.4a6/nemusicapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import base64
 import codecs
 
 import requests
 from Crypto.Cipher import AES
 import urllib3
 
-from NEmusicApi.exception import NoDownloadDirException
-from NEmusicApi.type import QualityLevel, EncodeType
+from nemusicapi.exception import NoDownloadDirException
+from nemusicapi.type import QualityLevel, EncodeType
 
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def aes_encrypt(text, key):
     iv = '0102030405060708'.encode('utf-8')  # iv偏移量
```

