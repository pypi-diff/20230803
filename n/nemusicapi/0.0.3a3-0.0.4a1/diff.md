# Comparing `tmp/nemusicapi-0.0.3a3.tar.gz` & `tmp/nemusicapi-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.3a3.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.4a1.tar", max compression
```

## Comparing `nemusicapi-0.0.3a3.tar` & `nemusicapi-0.0.4a1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.3a3/LICENSE
--rw-r--r--   0        0        0       82 2023-08-03 06:16:56.349661 nemusicapi-0.0.3a3/NEmusicApi/__init__.py
--rw-r--r--   0        0        0     4853 2023-08-03 06:35:13.308558 nemusicapi-0.0.3a3/NEmusicApi/api.py
--rw-r--r--   0        0        0      466 2023-08-03 06:37:04.766166 nemusicapi-0.0.3a3/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.3a3/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.3a3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a1/LICENSE
+-rw-r--r--   0        0        0       82 2023-08-03 06:16:56.349661 nemusicapi-0.0.4a1/NEmusicApi/__init__.py
+-rw-r--r--   0        0        0     4934 2023-08-03 06:48:24.991639 nemusicapi-0.0.4a1/NEmusicApi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a1/NEmusicApi/exception.py
+-rw-r--r--   0        0        0      466 2023-08-03 06:48:52.865161 nemusicapi-0.0.4a1/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.4a1/README.md
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a1/PKG-INFO
```

### Comparing `nemusicapi-0.0.3a3/LICENSE` & `nemusicapi-0.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.3a3/NEmusicApi/api.py` & `nemusicapi-0.0.4a1/NEmusicApi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import base64
 import codecs
 
 import requests
 from Crypto.Cipher import AES
 import urllib3
 
+from NEmusicApi.exception import NoDownloadDirException
+
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def aes_encrypt(text, key):
     iv = '0102030405060708'.encode('utf-8')  # iv偏移量
     text = text.encode('utf-8')  # 将明文转换为utf-8格式
@@ -118,15 +120,15 @@
         song_url = res['data'][0]['url']
         song_type = res['data'][0]['type']
         return song_url, song_type
 
 
     def download_song(self, song_id: int):
         if self.download_dir == None:
-            return
+            raise NoDownloadDirException
         
         res = self.get_song_file_data(song_id)
         if res is None:
             return False
         song_url, song_type = res
         
         file_path = os.path.join(self.download_dir, f'{song_id}.{song_type}')
```

### Comparing `nemusicapi-0.0.3a3/PKG-INFO` & `nemusicapi-0.0.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.3a3
+Version: 0.0.4a1
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

