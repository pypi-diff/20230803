# Comparing `tmp/tair-1.3.5.tar.gz` & `tmp/tair-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tair-1.3.5.tar", last modified: Wed Jul 19 09:27:01 2023, max compression
+gzip compressed data, was "tair-1.3.6.tar", last modified: Thu Aug  3 11:23:26 2023, max compression
```

## Comparing `tair-1.3.5.tar` & `tair-1.3.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.606902 tair-1.3.5/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.5/LICENSE
--rw-r--r--   0 yangbodong   (502) staff       (20)     4569 2023-07-19 09:27:01.606374 tair-1.3.5/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)     4288 2023-07-19 08:57:03.000000 tair-1.3.5/README.md
--rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-07-19 09:27:01.607028 tair-1.3.5/setup.cfg
--rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-07-19 09:24:03.000000 tair-1.3.5/setup.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.594006 tair-1.3.5/tair/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.5/tair/__init__.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.598028 tair-1.3.5/tair/asyncio/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.5/tair/asyncio/__init__.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.5/tair/asyncio/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.5/tair/asyncio/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.5/tair/asyncio/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.5/tair/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.5/tair/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.5/tair/commands.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.5/tair/exceptions.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.5/tair/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.5/tair/tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.5/tair/taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.5/tair/tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.5/tair/tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.5/tair/tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.5/tair/tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     6759 2023-04-10 02:26:45.000000 tair-1.3.5/tair/tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.5/tair/tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.5/tair/tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    18561 2023-07-19 08:58:48.000000 tair-1.3.5/tair/tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.5/tair/tairzset.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.5/tair/typing.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.595496 tair-1.3.5/tair.egg-info/
--rw-r--r--   0 yangbodong   (502) staff       (20)     4569 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/SOURCES.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/dependency_links.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/requires.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/top_level.txt
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.605825 tair-1.3.5/tests/
--rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.5/tests/test_from_url.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.5/tests/test_pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.5/tests/test_taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.5/tests/test_tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.5/tests/test_tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    18793 2023-04-10 02:26:45.000000 tair-1.3.5/tests/test_tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.5/tests/test_tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    24876 2023-07-19 08:58:48.000000 tair-1.3.5/tests/test_tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairzset.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-08-03 11:23:26.134708 tair-1.3.6/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.6/LICENSE
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4569 2023-08-03 11:23:26.134503 tair-1.3.6/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4288 2023-07-19 08:57:03.000000 tair-1.3.6/README.md
+-rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-08-03 11:23:26.134767 tair-1.3.6/setup.cfg
+-rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-08-03 11:22:10.000000 tair-1.3.6/setup.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-08-03 11:23:26.106677 tair-1.3.6/tair/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.6/tair/__init__.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-08-03 11:23:26.128419 tair-1.3.6/tair/asyncio/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.6/tair/asyncio/__init__.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.6/tair/asyncio/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.6/tair/asyncio/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.6/tair/asyncio/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.6/tair/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.6/tair/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5483 2023-08-01 02:52:30.000000 tair-1.3.6/tair/commands.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.6/tair/exceptions.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.6/tair/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.6/tair/tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.6/tair/taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.6/tair/tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.6/tair/tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.6/tair/tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.6/tair/tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     6837 2023-08-01 01:55:32.000000 tair-1.3.6/tair/tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.6/tair/tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.6/tair/tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    20538 2023-08-01 02:52:30.000000 tair-1.3.6/tair/tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.6/tair/tairzset.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.6/tair/typing.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-08-03 11:23:26.125571 tair-1.3.6/tair.egg-info/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4569 2023-08-03 11:23:26.000000 tair-1.3.6/tair.egg-info/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-08-03 11:23:26.000000 tair-1.3.6/tair.egg-info/SOURCES.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-08-03 11:23:26.000000 tair-1.3.6/tair.egg-info/dependency_links.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-08-03 11:23:26.000000 tair-1.3.6/tair.egg-info/requires.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-08-03 11:23:26.000000 tair-1.3.6/tair.egg-info/top_level.txt
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-08-03 11:23:26.134141 tair-1.3.6/tests/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.6/tests/test_from_url.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.6/tests/test_pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.6/tests/test_tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.6/tests/test_taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.6/tests/test_tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.6/tests/test_tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.6/tests/test_tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.6/tests/test_tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    18792 2023-08-01 01:55:32.000000 tair-1.3.6/tests/test_tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.6/tests/test_tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.6/tests/test_tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    28155 2023-08-01 02:52:30.000000 tair-1.3.6/tests/test_tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.6/tests/test_tairzset.py
```

### Comparing `tair-1.3.5/LICENSE` & `tair-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/PKG-INFO` & `tair-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tair-1.3.5/README.md` & `tair-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/__init__.py` & `tair-1.3.6/tair/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/asyncio/__init__.py` & `tair-1.3.6/tair/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/asyncio/client.py` & `tair-1.3.6/tair/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/asyncio/cluster.py` & `tair-1.3.6/tair/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/asyncio/pipeline.py` & `tair-1.3.6/tair/asyncio/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/client.py` & `tair-1.3.6/tair/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/cluster.py` & `tair-1.3.6/tair/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/commands.py` & `tair-1.3.6/tair/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     parse_exset,
 )
 from tair.tairts import TairTsCommands
 from tair.tairvector import (
     TairVectorCommands,
     parse_tvs_get_index_result,
     parse_tvs_get_result,
+    parse_tvs_hincrbyfloat_result,
     parse_tvs_hmget_result,
     parse_tvs_msearch_result,
     parse_tvs_search_result,
 )
 from tair.tairzset import TairZsetCommands, parse_tair_zset_items
 
 
@@ -151,13 +152,15 @@
     "TVS.HDEL": int_or_none,
     "TVS.HGETALL": parse_tvs_get_result,
     "TVS.HMGET": parse_tvs_hmget_result,
     "TVS.KNNSEARCH": parse_tvs_search_result,
     "TVS.MKNNSEARCH": parse_tvs_msearch_result,
     "TVS.MINDEXKNNSEARCH": parse_tvs_search_result,
     "TVS.MINDEXMKNNSEARCH": parse_tvs_msearch_result,
+    "TVS.HINCRBY": int_or_none,
+    "TVS.HINCRBYFLOAT": parse_tvs_hincrbyfloat_result,
 }
 
 
 def set_tair_response_callback(redis: Union[Redis, AsyncRedis]):
     for cmd, cb in TAIR_RESPONSE_CALLBACKS.items():
         redis.set_response_callback(cmd, cb)
```

### Comparing `tair-1.3.5/tair/pipeline.py` & `tair-1.3.6/tair/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairbloom.py` & `tair-1.3.6/tair/tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/taircpc.py` & `tair-1.3.6/tair/taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairdoc.py` & `tair-1.3.6/tair/tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairgis.py` & `tair-1.3.6/tair/tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairhash.py` & `tair-1.3.6/tair/tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairroaring.py` & `tair-1.3.6/tair/tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairsearch.py` & `tair-1.3.6/tair/tairsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,31 +149,40 @@
 
     def tft_search(self, index: KeyT, query: str, use_cache: bool = False) -> ResponseT:
         pieces: List[EncodableT] = [index, query]
         if use_cache:
             pieces.append("use_cache")
         return self.execute_command("TFT.SEARCH", *pieces)
 
-    def tft_msearch(self, index_count: int, index: Iterable[KeyT], query: str) -> ResponseT:
+    def tft_msearch(
+        self, index_count: int, index: Iterable[KeyT], query: str
+    ) -> ResponseT:
         return self.execute_command("TFT.MSEARCH", index_count, *index, query)
 
-    def tft_analyzer(self, analyzer_name: str, text: str, index: Optional[KeyT] = None,
-                     show_time: Optional[bool] = False) -> ResponseT:
+    def tft_analyzer(
+        self,
+        analyzer_name: str,
+        text: str,
+        index: Optional[KeyT] = None,
+        show_time: Optional[bool] = False,
+    ) -> ResponseT:
         pieces: List[EncodableT] = [analyzer_name, text]
         if index is not None:
             pieces.append("INDEX")
             pieces.append(index)
         if show_time:
             pieces.append("show_time")
         target_nodes = None
         if isinstance(self, tair.TairCluster):
             if index is None:
-                target_nodes = 'random'
+                target_nodes = "random"
             else:
-                target_nodes = self.nodes_manager.get_node_from_slot(self.keyslot(index))
+                target_nodes = self.nodes_manager.get_node_from_slot(
+                    self.keyslot(index)
+                )
         return self.execute_command("TFT.ANALYZER", *pieces, target_nodes=target_nodes)
 
     def tft_explaincost(self, index: KeyT, query: str) -> ResponseT:
         pieces: List[EncodableT] = [index, query]
         return self.execute_command("TFT.EXPLAINCOST", *pieces)
 
     def tft_addsug(self, index: KeyT, mapping: Dict[str, int]) -> ResponseT:
```

### Comparing `tair-1.3.5/tair/tairstring.py` & `tair-1.3.6/tair/tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairts.py` & `tair-1.3.6/tair/tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair/tairvector.py` & `tair-1.3.6/tair/tairvector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial, reduce
-from typing import Dict, List, Sequence, Tuple, Union, Optional, Iterable
+from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 from redis.client import pairs_to_dict
 from redis.utils import str_if_bytes
 
+from tair.typing import AbsExpiryT, CommandsProtocol, ExpiryT, ResponseT
 
 VectorType = Sequence[Union[int, float]]
 
 
 class DistanceMetric:
     Euclidean = "L2"  # an alias to L2
     L2 = "L2"
@@ -176,15 +177,15 @@
     def __str__(self):
         return "%s[%s]" % (self.name, self.params)
 
     def __repr__(self):
         return str(self)
 
 
-class TairVectorCommands:
+class TairVectorCommands(CommandsProtocol):
     encode_vector = TextVectorEncoder.encode
     decode_vector = TextVectorEncoder.decode
 
     CREATE_INDEX_CMD = "TVS.CREATEINDEX"
     GET_INDEX_CMD = "TVS.GETINDEX"
     DEL_INDEX_CMD = "TVS.DELINDEX"
     SCAN_INDEX_CMD = "TVS.SCANINDEX"
@@ -576,14 +577,53 @@
                         (float(result[i + 1]), result[i])
                         for i in range(0, len(result), 2)
                     ],
                 )
             queue = itertools.islice(queue, k)
             return [(key, score) for score, key in queue]
 
+    HINCRBY_CMD = "TVS.HINCRBY"
+    HINCRBYFLOAT_CMD = "TVS.HINCRBYFLOAT"
+
+    def tvs_hincrby(self, index: str, key: str, field: str, num: int):
+        """
+        increment the long value of a tairvector field by the given amount, not support field VECTOR
+        """
+        return self.execute_command(self.HINCRBY_CMD, index, key, field, num)
+
+    def tvs_hincrbyfloat(self, index: str, key: str, field: str, num: float):
+        """
+        increment the float value of a tairvector field by the given amount, not support field VECTOR
+        """
+        return self.execute_command(self.HINCRBYFLOAT_CMD, index, key, field, num)
+
+    def tvs_hexpire(self, index: str, key: str, ex: ExpiryT) -> ResponseT:
+        return self.execute_command("TVS.HEXPIRE", index, key, ex)
+
+    def tvs_hexpireat(self, index: str, key: str, exat: AbsExpiryT) -> ResponseT:
+        return self.execute_command("TVS.HEXPIREAT", index, key, exat)
+
+    def tvs_hpexpire(self, index: str, key: str, px: ExpiryT) -> ResponseT:
+        return self.execute_command("TVS.HPEXPIRE", index, key, px)
+
+    def tvs_hpexpireat(self, index: str, key: str, pxat: AbsExpiryT) -> ResponseT:
+        return self.execute_command("TVS.HPEXPIREAT", index, key, pxat)
+
+    def tvs_httl(self, index: str, key: str) -> ResponseT:
+        return self.execute_command("TVS.HTTL", index, key)
+
+    def tvs_hpttl(self, index: str, key: str) -> ResponseT:
+        return self.execute_command("TVS.HPTTL", index, key)
+
+    def tvs_hexpiretime(self, index: str, key: str) -> ResponseT:
+        return self.execute_command("TVS.HEXPIRETIME", index, key)
+
+    def tvs_hpexpiretime(self, index: str, key: str) -> ResponseT:
+        return self.execute_command("TVS.HPEXPIRETIME", index, key)
+
 
 def parse_tvs_get_index_result(resp) -> Union[Dict, None]:
     if len(resp) == 0:
         return None
     return pairs_to_dict(resp, decode_keys=True, decode_string_values=True)
 
 
@@ -606,7 +646,13 @@
 
 def parse_tvs_search_result(resp) -> List[Tuple]:
     return [(resp[i], float(resp[i + 1])) for i in range(0, len(resp), 2)]
 
 
 def parse_tvs_msearch_result(resp) -> List[List[Tuple]]:
     return [parse_tvs_search_result(r) for r in resp]
+
+
+def parse_tvs_hincrbyfloat_result(resp) -> Union[float, None]:
+    if resp is None:
+        return resp
+    return float(resp.decode())
```

### Comparing `tair-1.3.5/tair/tairzset.py` & `tair-1.3.6/tair/tairzset.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tair.egg-info/PKG-INFO` & `tair-1.3.6/tair.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tair-1.3.5/tair.egg-info/SOURCES.txt` & `tair-1.3.6/tair.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_from_url.py` & `tair-1.3.6/tests/test_from_url.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_pipeline.py` & `tair-1.3.6/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairbloom.py` & `tair-1.3.6/tests/test_tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_taircpc.py` & `tair-1.3.6/tests/test_taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairdoc.py` & `tair-1.3.6/tests/test_tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairgis.py` & `tair-1.3.6/tests/test_tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairhash.py` & `tair-1.3.6/tests/test_tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairroaring.py` & `tair-1.3.6/tests/test_tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairsearch.py` & `tair-1.3.6/tests/test_tairsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
   }
 }"""
 
         assert t.tft_createindex(index, mappings1)
         assert t.tft_updateindex(index, mappings2)
         t.delete(index)
 
-
     def test_tft_getindex(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
     "properties": {
@@ -451,15 +450,15 @@
   }}
 }}"""
         result = t.tft_search(index, '{"sort":[{"price":{"order":"desc"}}]}')
         assert json.loads(want) == json.loads(result)
         result = t.tft_search(index, '{"sort":[{"price":{"order":"desc"}}]}', True)
         assert json.loads(want) == json.loads(result)
         result = t.tft_explaincost(index, '{"sort":[{"price":{"order":"desc"}}]}')
-        assert json.loads(result)['QUERY_COST']
+        assert json.loads(result)["QUERY_COST"]
         t.delete(index)
 
     def test_tft_msearch(self, t: Tair):
         index1 = "{idx}_" + str(uuid.uuid4())
         index2 = "{idx}_" + str(uuid.uuid4())
         mappings = """
 {
@@ -476,20 +475,16 @@
         document1 = '{"product_id":"test1"}'
         document2 = '{"product_id":"test2"}'
         document3 = '{"product_id":"test3"}'
         document4 = '{"product_id":"test4"}'
 
         assert t.tft_createindex(index1, mappings)
         assert t.tft_createindex(index2, mappings)
-        assert t.tft_madddoc(
-            index1, {document1: "00001", document2: "00002"}
-        )
-        assert t.tft_madddoc(
-            index2, {document3: "00003", document4: "00004"}
-        )
+        assert t.tft_madddoc(index1, {document1: "00001", document2: "00002"})
+        assert t.tft_madddoc(index2, {document3: "00003", document4: "00004"})
 
         want = f"""{{
     "aux_info": {{"index_crc64": 5843875291690071373}},
     "hits": {{
         "hits": [
           {{
             "_id": "00001",
@@ -516,15 +511,17 @@
             "_source": {{ "product_id": "test4" }}
           }}
         ],
         "max_score": 1.0,
         "total": {{ "relation": "eq", "value": 4 }}
       }}
     }}"""
-        result = t.tft_msearch(2, {index1, index2}, '{"sort":[{"_doc":{"order":"asc"}}]}')
+        result = t.tft_msearch(
+            2, {index1, index2}, '{"sort":[{"_doc":{"order":"asc"}}]}'
+        )
         assert json.loads(want) == json.loads(result)
         t.delete(index1)
         t.delete(index2)
 
     def test_tft_analyzer(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
@@ -543,19 +540,21 @@
         "my_analyzer":{
           "type":"standard"
         }
       }
     }
   }
 }"""
-        text = 'This is tair-py.'
+        text = "This is tair-py."
 
         assert t.tft_createindex(index, mappings)
-        assert t.tft_analyzer("standard", text) == t.tft_analyzer("my_analyzer", text, index)
-        assert 'consuming time' in str(t.tft_analyzer("standard", text, None, True))
+        assert t.tft_analyzer("standard", text) == t.tft_analyzer(
+            "my_analyzer", text, index
+        )
+        assert "consuming time" in str(t.tft_analyzer("standard", text, None, True))
 
         t.delete(index)
 
     def test_tft_addsug(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
 
         assert (
```

### Comparing `tair-1.3.5/tests/test_tairstring.py` & `tair-1.3.6/tests/test_tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairts.py` & `tair-1.3.6/tests/test_tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.5/tests/test_tairvector.py` & `tair-1.3.6/tests/test_tairvector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # /user/bin/env python3
 import os
 import string
 import sys
+import time
 import unittest
 import uuid
 from random import choice, randint, random
 
+import pytest
 import redis
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from tair.tairvector import (
-    Constants,
-    DataType,
-    DistanceMetric,
-    TairVectorCommands,
-    TairVectorIndex,
-)
+from tair.tairvector import Constants, DataType, DistanceMetric, TairVectorIndex
 
 from .conftest import get_tair_client
 
 client = get_tair_client()
 
 dim = 16
 num_vectors = 100
@@ -171,15 +167,15 @@
             obj = client.tvs_hgetall("test", str(i))
             self.assertTrue(Constants.VECTOR_KEY in obj)
             self.assertTrue(vectorEqual(v, obj[Constants.VECTOR_KEY]))
             del obj[Constants.VECTOR_KEY]
             self.assertDictEqual(obj, test_attributes[i])
 
     def test_hmget(self):
-        self.assertTrue(client.tvs_create_index("test", dim, **self.index_params))
+        # self.assertTrue(client.tvs_create_index("test", dim, **self.index_params))
         vector = [randint(1, 100) for _ in range(dim)]
         key = "key_" + str(uuid.uuid4())
         value1 = "value_" + str(uuid.uuid4())
         value2 = "value_" + str(uuid.uuid4())
         ret = client.tvs_hset("test", key, vector=vector, field1=value1, field2=value2)
         self.assertTrue(ret)
         obj = client.tvs_hmget(
@@ -216,16 +212,28 @@
             self.assertEqual(client.tvs_hdel("test", str(i), *keys), len(keys))
 
     def test_7_delete(self):
         # delete inserted entries
         for i in range(len(test_vectors)):
             self.assertEqual(client.tvs_del("test", str(i)), 1)
 
-    def test_9_delete(self):
-        self.assertEqual(client.tvs_del_index("test"), 1)
+    def test_8_hincry(self):
+        key_tmp = "key_tmp1"
+        client.tvs_hset("test", key_tmp, field1=1)
+        self.assertEqual(client.tvs_hincrby("test", key_tmp, "field1", 1), 2)
+
+    def test_9_hincrbyfloat(self):
+        key_tmp = "key_tmp1"
+        client.tvs_hset("test", key_tmp, field2=1.1)
+        assert client.tvs_hincrbyfloat("test", key_tmp, "field2", 2.2) == pytest.approx(
+            3.3
+        )
+
+    def test_10_delete(self):
+        client.tvs_del_index("test")
 
 
 class SearchCommandsTest(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName=methodName)
         self.top_k = 10
         self.index_params = {
@@ -528,14 +536,15 @@
             client.tvs_scan(self.index_name, max_dist=50)
         with self.assertRaises(ValueError):
             client.tvs_scan(self.index_name, vector=[0, 0])
         result = [
             r for r in client.tvs_scan(self.index_name, vector=[0, 0], max_dist=50)
         ]
         result = sorted(result)
+        print(result)
         self.assertListEqual(result, [b"3", b"5", b"6"])
 
     def test_4_scan_with_both(self):
         result = [
             r
             for r in client.tvs_scan(
                 self.index_name, vector=[0, 0], max_dist=50, filter_str="age<30"
@@ -695,10 +704,96 @@
             self.assertLess(int(key), 500)
 
     def test_9_cleanup(self):
         ret = client.tvs_del_index(self.index_name)
         self.assertEqual(ret, 1)
 
 
+class VectorExpireTest(unittest.TestCase):
+    index_name = "expire_test"
+
+    def _check_index(self):
+        if client.tvs_get_index(self.index_name) is not None:
+            self.assertEqual(client.tvs_del_index(self.index_name), 1)
+        ret = client.tvs_create_index(
+            self.index_name,
+            dim,
+            distance_type=DistanceMetric.L2,
+        )
+        self.assertTrue(ret)
+
+    def test_tvs_hexpire(self):
+        self._check_index()
+        key = "key_" + str(uuid.uuid4())
+        vector = [random() for _ in range(dim)]
+        self.assertEqual(
+            client.tvs_hset(
+                self.index_name,
+                key,
+                vector,
+                field1=str(uuid.uuid4()),
+                field2=randint(0, 100),
+            ),
+            3,
+        )
+        self.assertEqual(client.tvs_hexpire(self.index_name, key, 100), 1)
+        assert 0 < client.tvs_httl(self.index_name, key) <= 100
+
+    def test_tvs_hpexpire(self):
+        self._check_index()
+        key = "key_" + str(uuid.uuid4())
+        vector = [random() for _ in range(dim)]
+        self.assertEqual(
+            client.tvs_hset(
+                self.index_name,
+                key,
+                vector,
+                field1=str(uuid.uuid4()),
+                field2=randint(0, 100),
+            ),
+            3,
+        )
+        self.assertEqual(client.tvs_hpexpire(self.index_name, key, 100), 1)
+        assert 0 < client.tvs_hpttl(self.index_name, key) <= 100
+
+    def test_tvs_hexpireat(self):
+        self._check_index()
+        key = "key_" + str(uuid.uuid4())
+        vector = [random() for _ in range(dim)]
+        abs_expire = int(time.time()) + 100
+        self.assertEqual(
+            client.tvs_hset(
+                self.index_name,
+                key,
+                vector,
+                field1=str(uuid.uuid4()),
+                field2=randint(0, 100),
+            ),
+            3,
+        )
+        self.assertEqual(client.tvs_hexpireat(self.index_name, key, abs_expire), 1)
+        assert 0 < client.tvs_httl(self.index_name, key) <= 100
+        self.assertEqual(client.tvs_hexpiretime(self.index_name, key), abs_expire)
+
+    def test_tvs_hpexpireat(self):
+        self._check_index()
+        key = "key_" + str(uuid.uuid4())
+        vector = [random() for _ in range(dim)]
+        abs_expire = int(time.time() * 1000) + 100
+        self.assertEqual(
+            client.tvs_hset(
+                self.index_name,
+                key,
+                vector,
+                field1=str(uuid.uuid4()),
+                field2=randint(0, 100),
+            ),
+            3,
+        )
+        self.assertEqual(client.tvs_hpexpireat(self.index_name, key, abs_expire), 1)
+        assert 0 < client.tvs_hpttl(self.index_name, key) <= 100
+        self.assertEqual(client.tvs_hpexpiretime(self.index_name, key), abs_expire)
+
+
 if __name__ == "__main__":
     unittest.main()
     client.close()
```

### Comparing `tair-1.3.5/tests/test_tairzset.py` & `tair-1.3.6/tests/test_tairzset.py`

 * *Files identical despite different names*

