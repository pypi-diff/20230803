# Comparing `tmp/nemusicapi-0.0.4a1.tar.gz` & `tmp/nemusicapi-0.0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.4a1.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.4a2.tar", max compression
```

## Comparing `nemusicapi-0.0.4a1.tar` & `nemusicapi-0.0.4a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a1/LICENSE
--rw-r--r--   0        0        0       82 2023-08-03 06:16:56.349661 nemusicapi-0.0.4a1/NEmusicApi/__init__.py
--rw-r--r--   0        0        0     4934 2023-08-03 06:48:24.991639 nemusicapi-0.0.4a1/NEmusicApi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a1/NEmusicApi/exception.py
--rw-r--r--   0        0        0      466 2023-08-03 06:48:52.865161 nemusicapi-0.0.4a1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.4a1/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a2/LICENSE
+-rw-r--r--   0        0        0      170 2023-08-03 07:21:59.213880 nemusicapi-0.0.4a2/NEmusicApi/__init__.py
+-rw-r--r--   0        0        0     5063 2023-08-03 07:17:36.717893 nemusicapi-0.0.4a2/NEmusicApi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a2/NEmusicApi/exception.py
+-rw-r--r--   0        0        0      466 2023-08-03 07:21:22.338905 nemusicapi-0.0.4a2/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.4a2/README.md
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a2/PKG-INFO
```

### Comparing `nemusicapi-0.0.4a1/LICENSE` & `nemusicapi-0.0.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.4a1/NEmusicApi/api.py` & `nemusicapi-0.0.4a2/NEmusicApi/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import random
 import base64
 import codecs
+from enum import Enum
 
 import requests
 from Crypto.Cipher import AES
 import urllib3
 
 from NEmusicApi.exception import NoDownloadDirException
 
@@ -38,14 +39,22 @@
     random_str = ''.join(random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789', 16))
     encText = aes_encrypt(raw_params, '0CoJUm6Qyw8W8jud')
     params = aes_encrypt(encText, random_str)
     encSecKey = rsa_encrypt(random_str, '010001', '00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b3ece0462db0a22b8e7')  # RSA加密后获得encSecKey
     return params, encSecKey
 
 
+class QualityLevel(Enum):
+    standard = 'standard'
+    higher = 'higher'
+    exhigh = 'exhigh'
+    lossless = 'lossless'
+    hires = 'hires'
+
+
 class RawApi:
     def __init__(self, *,
                  cookie=''
                  ):
         self.cookie = cookie
         
 
@@ -72,23 +81,22 @@
             'total': total,
             'limit': limit
         }
         url = 'https://music.163.com/weapi/cloudsearch/get/web'
         res = self._get_data(url, params)
         return res
     
-    def get_song_url(self, song_id: int, *, level='standard', encodeType='flac'):
+    def get_song_url(self, song_id: int, level: QualityLevel, *, encodeType='flac'):
         """
-        level: standard标准 higher较高 exhigh极高 lossless无损 hires
         encodeType: aac flac
         """
         url = f'https://music.163.com/weapi/song/enhance/player/url/v1'
         params = {
             'ids': '["' + str(song_id) + '"]',
-            'level': level,
+            'level': level.value,
             'encodeType': encodeType
         }
         res = self._get_data(url, params)
         return res
 
 
 class Api(RawApi):
@@ -109,16 +117,16 @@
         if res['result']['songCount'] == 0:
             return
         song_id = res['result']['songs'][0]['id']
         song_name = res['result']['songs'][0]['name']
         return song_id, song_name
 
 
-    def get_song_file_data(self, song_id: int) -> tuple[str, str] | None:
-        res = self.get_song_url(song_id, level='hires')
+    def get_song_file_data(self, song_id: int, level = QualityLevel.standard) -> tuple[str, str] | None:
+        res = self.get_song_url(song_id, level)
         if res['data'][0]['url'] is None:
             return
         song_url = res['data'][0]['url']
         song_type = res['data'][0]['type']
         return song_url, song_type
```

### Comparing `nemusicapi-0.0.4a1/PKG-INFO` & `nemusicapi-0.0.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.4a1
+Version: 0.0.4a2
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

