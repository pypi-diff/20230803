# Comparing `tmp/nemusicapi-0.0.4a2.tar.gz` & `tmp/nemusicapi-0.0.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.4a2.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.4a3.tar", max compression
```

## Comparing `nemusicapi-0.0.4a2.tar` & `nemusicapi-0.0.4a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a2/LICENSE
--rw-r--r--   0        0        0      170 2023-08-03 07:21:59.213880 nemusicapi-0.0.4a2/NEmusicApi/__init__.py
--rw-r--r--   0        0        0     5063 2023-08-03 07:17:36.717893 nemusicapi-0.0.4a2/NEmusicApi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a2/NEmusicApi/exception.py
--rw-r--r--   0        0        0      466 2023-08-03 07:21:22.338905 nemusicapi-0.0.4a2/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.4a2/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.4a3/LICENSE
+-rw-r--r--   0        0        0      170 2023-08-03 07:21:59.213880 nemusicapi-0.0.4a3/NEmusicApi/__init__.py
+-rw-r--r--   0        0        0     4921 2023-08-03 07:29:52.710416 nemusicapi-0.0.4a3/NEmusicApi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.4a3/NEmusicApi/exception.py
+-rw-r--r--   0        0        0      466 2023-08-03 07:31:16.771146 nemusicapi-0.0.4a3/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.4a3/README.md
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.4a3/PKG-INFO
```

### Comparing `nemusicapi-0.0.4a2/LICENSE` & `nemusicapi-0.0.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.4a2/NEmusicApi/api.py` & `nemusicapi-0.0.4a3/NEmusicApi/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,21 +126,16 @@
         if res['data'][0]['url'] is None:
             return
         song_url = res['data'][0]['url']
         song_type = res['data'][0]['type']
         return song_url, song_type
 
 
-    def download_song(self, song_id: int):
+    def download_song(self, song_url: str, file_name: str):
         if self.download_dir == None:
             raise NoDownloadDirException
         
-        res = self.get_song_file_data(song_id)
-        if res is None:
-            return False
-        song_url, song_type = res
-        
-        file_path = os.path.join(self.download_dir, f'{song_id}.{song_type}')
+        file_path = os.path.join(self.download_dir, file_name)
         
         with open(file_path, 'wb') as f:
             f.write(requests.get(song_url).content)
         return True
```

### Comparing `nemusicapi-0.0.4a2/PKG-INFO` & `nemusicapi-0.0.4a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.4a2
+Version: 0.0.4a3
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

