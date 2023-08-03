# Comparing `tmp/nemusicapi-0.0.3a2.tar.gz` & `tmp/nemusicapi-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.3a2.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.3a3.tar", max compression
```

## Comparing `nemusicapi-0.0.3a2.tar` & `nemusicapi-0.0.3a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.3a2/LICENSE
--rw-r--r--   0        0        0       82 2023-08-03 06:16:56.349661 nemusicapi-0.0.3a2/NEmusicApi/__init__.py
--rw-r--r--   0        0        0     4750 2023-08-03 05:41:17.034038 nemusicapi-0.0.3a2/NEmusicApi/api.py
--rw-r--r--   0        0        0      466 2023-08-03 06:15:59.534577 nemusicapi-0.0.3a2/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.3a2/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.3a2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.3a3/LICENSE
+-rw-r--r--   0        0        0       82 2023-08-03 06:16:56.349661 nemusicapi-0.0.3a3/NEmusicApi/__init__.py
+-rw-r--r--   0        0        0     4853 2023-08-03 06:35:13.308558 nemusicapi-0.0.3a3/NEmusicApi/api.py
+-rw-r--r--   0        0        0      466 2023-08-03 06:37:04.766166 nemusicapi-0.0.3a3/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.3a3/README.md
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.3a3/PKG-INFO
```

### Comparing `nemusicapi-0.0.3a2/LICENSE` & `nemusicapi-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.3a2/NEmusicApi/api.py` & `nemusicapi-0.0.3a3/NEmusicApi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,21 +88,22 @@
         res = self._get_data(url, params)
         return res
 
 
 class Api(RawApi):
     def __init__(self, *, 
                  cookie='',
-                 download_dir='./'
+                 download_dir=None
                  ):
         super().__init__(cookie=cookie)
-        
         self.download_dir = download_dir
-        if not os.path.exists(download_dir):
-            os.makedirs(download_dir)
+        
+        if download_dir:
+            if not os.path.exists(download_dir):
+                os.makedirs(download_dir)
     
     
     def refresh_song_data(self, raw_song_name: str) -> tuple[int, str] | None:
         res = self.search_music(raw_song_name)
         if res['result']['songCount'] == 0:
             return
         song_id = res['result']['songs'][0]['id']
@@ -116,14 +117,17 @@
             return
         song_url = res['data'][0]['url']
         song_type = res['data'][0]['type']
         return song_url, song_type
 
 
     def download_song(self, song_id: int):
+        if self.download_dir == None:
+            return
+        
         res = self.get_song_file_data(song_id)
         if res is None:
             return False
         song_url, song_type = res
         
         file_path = os.path.join(self.download_dir, f'{song_id}.{song_type}')
```

### Comparing `nemusicapi-0.0.3a2/PKG-INFO` & `nemusicapi-0.0.3a3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

