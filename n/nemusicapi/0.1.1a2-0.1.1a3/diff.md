# Comparing `tmp/nemusicapi-0.1.1a2.tar.gz` & `tmp/nemusicapi-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.1.1a2.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.1a3.tar", max compression
```

## Comparing `nemusicapi-0.1.1a2.tar` & `nemusicapi-0.1.1a3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a2/LICENSE
--rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.1a2/nemusicapi/__init__.py
--rw-r--r--   0        0        0     4887 2023-08-03 09:36:07.886894 nemusicapi-0.1.1a2/nemusicapi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a2/nemusicapi/exception.py
--rw-r--r--   0        0        0      355 2023-08-03 09:37:41.904391 nemusicapi-0.1.1a2/nemusicapi/type.py
--rw-r--r--   0        0        0      466 2023-08-03 09:38:18.296723 nemusicapi-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     1285 2023-08-03 09:34:57.662330 nemusicapi-0.1.1a2/README.md
--rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.1a3/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     4883 2023-08-03 09:44:38.640178 nemusicapi-0.1.1a3/nemusicapi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a3/nemusicapi/exception.py
+-rw-r--r--   0        0        0      355 2023-08-03 09:37:41.904391 nemusicapi-0.1.1a3/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-03 09:44:53.732438 nemusicapi-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0     1285 2023-08-03 09:34:57.662330 nemusicapi-0.1.1a3/README.md
+-rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a3/PKG-INFO
```

### Comparing `nemusicapi-0.1.1a2/LICENSE` & `nemusicapi-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a2/nemusicapi/api.py` & `nemusicapi-0.1.1a3/nemusicapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,21 +105,21 @@
         if res['result']['songCount'] == 0:
             return
         song_id = res['result']['songs'][0]['id']
         song_name = res['result']['songs'][0]['name']
         return song_id, song_name
 
 
-    def get_song_download_data(self, song_id: int, *, level=QualityLevel.standard, encodeType=EncodeType.flac) -> tuple[str, QualityLevel] | None:
+    def get_song_download_data(self, song_id: int, *, level=QualityLevel.standard, encodeType=EncodeType.flac) -> tuple[str, EncodeType] | None:
         res = self.get_song_file_data(song_id, level=level, encodeType=encodeType)
         if res['data'][0]['url'] is None:
             return
         song_url = res['data'][0]['url']
         song_type = res['data'][0]['type']
-        return song_url, QualityLevel(song_type)
+        return song_url, EncodeType(song_type)
 
 
     def download_song(self, song_url: str, file_name: str):
         if self.download_dir == None:
             raise NoDownloadDirException
         
         file_path = os.path.join(self.download_dir, file_name)
```

### Comparing `nemusicapi-0.1.1a2/README.md` & `nemusicapi-0.1.1a3/README.md`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a2/PKG-INFO` & `nemusicapi-0.1.1a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

