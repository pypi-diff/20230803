# Comparing `tmp/scoamp-0.4.0a3-py3-none-any.whl.zip` & `tmp/scoamp-0.5.0a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 26687 bytes, number of entries: 22
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-21 10:35 scoamp/__init__.py
--rw-r--r--  2.0 unx     7991 b- defN 23-Jul-14 11:03 scoamp/api.py
--rw-r--r--  2.0 unx     2212 b- defN 23-Jul-13 12:34 scoamp/globals.py
--rw-r--r--  2.0 unx    15216 b- defN 23-Jul-21 10:32 scoamp/toolkit.py
+Zip file size: 27635 bytes, number of entries: 22
+-rw-r--r--  2.0 unx       24 b- defN 23-Aug-03 12:14 scoamp/__init__.py
+-rw-r--r--  2.0 unx     8052 b- defN 23-Aug-03 07:34 scoamp/api.py
+-rw-r--r--  2.0 unx     2212 b- defN 23-Jul-28 10:27 scoamp/globals.py
+-rw-r--r--  2.0 unx    19171 b- defN 23-Aug-03 12:10 scoamp/toolkit.py
 -rw-r--r--  2.0 unx      486 b- defN 23-Jun-06 04:20 scoamp/commands/__init__.py
--rw-r--r--  2.0 unx     4381 b- defN 23-Jul-21 09:46 scoamp/commands/api.py
+-rw-r--r--  2.0 unx     4608 b- defN 23-Aug-03 12:12 scoamp/commands/api.py
 -rw-r--r--  2.0 unx     7581 b- defN 23-Jun-06 04:20 scoamp/commands/lfs.py
 -rw-r--r--  2.0 unx     2135 b- defN 23-Jun-06 04:20 scoamp/schema/public-model-meta.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 04:20 scoamp/utils/__init__.py
 -rw-r--r--  2.0 unx     5080 b- defN 23-Jun-27 08:29 scoamp/utils/api_utils.py
--rw-r--r--  2.0 unx      501 b- defN 23-Jul-13 08:00 scoamp/utils/decrypt.py
--rw-r--r--  2.0 unx     1779 b- defN 23-Jul-20 09:14 scoamp/utils/error.py
+-rw-r--r--  2.0 unx      501 b- defN 23-Jul-28 10:27 scoamp/utils/decrypt.py
+-rw-r--r--  2.0 unx     1779 b- defN 23-Jul-28 10:27 scoamp/utils/error.py
 -rw-r--r--  2.0 unx     5150 b- defN 23-Jul-13 07:42 scoamp/utils/helper.py
--rw-r--r--  2.0 unx      421 b- defN 23-Jul-20 09:08 scoamp/utils/logger.py
+-rw-r--r--  2.0 unx      421 b- defN 23-Jul-28 10:27 scoamp/utils/logger.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 08:29 tests/__init__.py
 -rw-r--r--  2.0 unx     9110 b- defN 23-Jun-27 08:29 tests/test_utils_helper.py
--rw-r--r--  2.0 unx    11334 b- defN 23-Jul-21 10:36 scoamp-0.4.0a3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1239 b- defN 23-Jul-21 10:36 scoamp-0.4.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 10:36 scoamp-0.4.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-21 10:36 scoamp-0.4.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-21 10:36 scoamp-0.4.0a3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1742 b- defN 23-Jul-21 10:36 scoamp-0.4.0a3.dist-info/RECORD
-22 files, 76534 bytes uncompressed, 23879 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx    11334 b- defN 23-Aug-03 12:15 scoamp-0.5.0a0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1239 b- defN 23-Aug-03 12:15 scoamp-0.5.0a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 12:15 scoamp-0.5.0a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Aug-03 12:15 scoamp-0.5.0a0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-03 12:15 scoamp-0.5.0a0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1742 b- defN 23-Aug-03 12:15 scoamp-0.5.0a0.dist-info/RECORD
+22 files, 80777 bytes uncompressed, 24827 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_utils_helper.py
 Comment: 
 
-Filename: scoamp-0.4.0a3.dist-info/LICENSE
+Filename: scoamp-0.5.0a0.dist-info/LICENSE
 Comment: 
 
-Filename: scoamp-0.4.0a3.dist-info/METADATA
+Filename: scoamp-0.5.0a0.dist-info/METADATA
 Comment: 
 
-Filename: scoamp-0.4.0a3.dist-info/WHEEL
+Filename: scoamp-0.5.0a0.dist-info/WHEEL
 Comment: 
 
-Filename: scoamp-0.4.0a3.dist-info/entry_points.txt
+Filename: scoamp-0.5.0a0.dist-info/entry_points.txt
 Comment: 
 
-Filename: scoamp-0.4.0a3.dist-info/top_level.txt
+Filename: scoamp-0.5.0a0.dist-info/top_level.txt
 Comment: 
 
-Filename: scoamp-0.4.0a3.dist-info/RECORD
+Filename: scoamp-0.5.0a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scoamp/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.4.0a3'
+__version__ = '0.5.0a0'
```

## scoamp/api.py

```diff
@@ -182,15 +182,15 @@
         url = self._amp_url(f'/v1/public/models/{model_id}/meta')
 
         resp = make_request(self.ak, self.sk, method, url, json=meta, headers=self._amp_headers())
         amp_raise_for_status(resp)
         return resp.json()
 
     def download_file(self, model_id: str, file_path: str, revision: Optional[str]=None, is_public: bool=False,
-                      resume_size: Optional[int]=None, timeout: Optional[float]=None):
+                      resume_size: Optional[int]=None, allow_redirects: bool=True, timeout: Optional[float]=None):
         method = 'GET'
         url = self._amp_url(f'/v1/download/file')
         params = {
             'model_name': model_id,
             'path': file_path,
             'type': 'PUBLICMODEL' if is_public else 'MODEL',
         }
@@ -198,10 +198,10 @@
             params['ref'] = revision
 
         headers = self._amp_headers()
         if resume_size:
             headers['Range'] = f'bytes={resume_size}-'
 
         resp = make_request(self.ak, self.sk, method, url, params=params, headers=headers,
-                            stream=True, timeout=timeout)
+                            stream=True, allow_redirects=allow_redirects, timeout=timeout)
         amp_raise_for_status(resp)
         return resp
```

## scoamp/toolkit.py

```diff
@@ -1,26 +1,38 @@
 import os
 import io
 import re
 import tempfile
 import subprocess
+import requests
+from concurrent import futures
 from functools import partial
 from contextlib import contextmanager
 from typing import Optional, Generator, BinaryIO, Union, List
 from pathlib import Path
 from filelock import FileLock
 from requests.adapters import Retry
 from tqdm import tqdm
 from urllib.parse import urlparse, urlunparse
 
+
 from scoamp.globals import global_api as api
 from scoamp.globals import Environment
 from scoamp.utils.error import FileDownloadError, APIError, SubprocessError
 from scoamp.utils.logger import get_logger
 
+
+# constants
+API_FILE_DOWNLOAD_RETRY_TIMES = 3
+API_FILE_DOWNLOAD_TIMEOUT = 60 * 5
+API_FILE_DOWNLOAD_READ_CHUNK_SIZE = 1 * 1024 * 1024
+API_FILE_DOWNLOAD_PARALLEL_THRESHOLD = 500 * 1024 * 1024
+API_FILE_DOWNLOAD_PARALLELS = 4
+API_FILE_DOWNLOAD_PARALLEL_PART_SIE = 200 * 1024 * 1024
+
 logger = get_logger()
 
 def model_file_list(
     model_id: str,
     *,
     is_public: bool = False,
     revision: Optional[str] = None,
@@ -49,16 +61,17 @@
     model_id: str,
     file_path: str,
     *,
     is_public: bool = False,
     revision: Optional[str] = None,
     local_dir: Optional[str] = None,
     force_download: bool = False,
-    resume_download: bool = True,
+    resume_download: bool = False,
     remote_validate: bool = True,
+    parallels: int = API_FILE_DOWNLOAD_PARALLELS,
 ) -> str:
     """Download a given file from amp server
     Args:
         model_id (`str`):
             model id.
         file_path (`str`):
             file path in the repo, with subfolder.
@@ -70,20 +83,36 @@
         local_dir (`str` or `Path`, *optional*):
             If provided, the downloaded file will be placed under this directory
         force_download (`bool`, *optional*, defaults to `False`):
             Whether the file should be downloaded even if it already exists in
             the local dir.
         resume_download (`bool`, *optional*, defaults to `False`):
             If `True`, resume a previously interrupted download.
-        remote_validate (`bool`, *optional*, defaults to `False`):
+        remote_validate (`bool`, *optional*, defaults to `True`):
             If `True`, validate remote model access and file exists before downloading
+        parallels(`int`, *optional*, defaults to `4`):
+            if set to > 1, will use parallel downloading, and must set `resume_download` to `False` at the same time,
+            otherwise Exception will be raised.
 
     Returns:
         Local path (string) of file
     """
+    if parallels:
+        if not isinstance(parallels, int):
+            raise ValueError('parallel shoud be int type')
+        if parallels < 1:
+            parallels = 1
+        elif parallels > API_FILE_DOWNLOAD_PARALLELS:
+            parallels = API_FILE_DOWNLOAD_PARALLELS
+    else:
+        parallels = 1
+    
+    if parallels > 1 and resume_download:
+        raise ValueError('condition conflict: parallels > 1 while set resume_download=True')
+    
     if not model_id:
         raise ValueError('model_id shoud not be empty')
 
     if not file_path:
         raise ValueError('file_path should not be empty')
 
     if not local_dir:
@@ -134,14 +163,15 @@
                 temp_file_name = temp_file.name
                 _http_get_model_file(
                     temp_file,
                     model_id,
                     file_path,
                     is_public = is_public,
                     revision = revision,
+                    parallels=parallels,
                 )
 
             os.replace(temp_file.name, local_file_path)
     finally: # gc
         # clear lock file
         try:
             lock_path.unlink()
@@ -150,63 +180,118 @@
 
         # clear temp file
         if not resume_download and os.path.exists(temp_file_name):
             os.remove(temp_file_name)
 
     return str(local_file_path)
 
-API_FILE_DOWNLOAD_RETRY_TIMES = 3
-API_FILE_DOWNLOAD_TIMEOUT = 60 * 5
-API_FILE_DOWNLOAD_CHUNK_SIZE = 1024 * 1024
-
 def _http_get_model_file(
     temp_file: BinaryIO,
     model_id: str,
     file_path: str,
     *,
     is_public: bool = False,
     revision: Optional[str] = None,
+    parallels: int = 1,
 ):
     # TODO retry policy
     ## retry sleep 0.5s, 1s, 2s
     #retry = Retry(
     #    total= API_FILE_DOWNLOAD_RETRY_TIMES,
     #    backoff_factor=1,
     #    allowed_methods=['GET'])
 
     downloaded_size = temp_file.tell()
+    if downloaded_size > 0 and parallels > 1:
+        raise ValueError(f'conflict condition: parallels > 1 while using resume downloading')
+
     r = api.download_file(
             model_id,
             file_path,
             revision=revision,
             is_public=is_public,
             resume_size=downloaded_size,
+            allow_redirects=False,
             timeout=API_FILE_DOWNLOAD_TIMEOUT,
         )
-    content_length = r.headers.get('Content-Length')
+    
+    parallel_flag = False
+    real_url = ''
+    if r.status_code < 300:
+        content_length = r.headers.get('Content-Length')
+    else:
+        # LFS file
+        content_length = r.headers['X-Linked-Size']
+        real_url = r.headers['Location']
+        if int(content_length) <= API_FILE_DOWNLOAD_PARALLEL_THRESHOLD or parallels <= 1:
+            r = requests.get(real_url, stream=True, timeout=API_FILE_DOWNLOAD_TIMEOUT)
+            r.raise_for_status()
+        else:
+            parallel_flag = True
+
     total = downloaded_size + int(content_length) if content_length is not None else None
 
     desc_file_name = file_path
     if len(desc_file_name) > 22:
         desc_file_name = f"(…){desc_file_name[-20:]}"
 
     progress = tqdm(
         unit='B',
         unit_scale=True,
         unit_divisor=1024,
         total=total,
         initial=downloaded_size,
         desc=f'Downloading {desc_file_name}',
+        ascii='.#',
     )
-    for chunk in r.iter_content(chunk_size=API_FILE_DOWNLOAD_CHUNK_SIZE):
-        if chunk:  # filter out keep-alive new chunks
-            progress.update(len(chunk))
-            temp_file.write(chunk)
+    if not parallel_flag:
+        for chunk in r.iter_content(chunk_size=API_FILE_DOWNLOAD_READ_CHUNK_SIZE):
+            if chunk:  # filter out keep-alive new chunks
+                temp_file.write(chunk)
+                progress.update(len(chunk))
+        temp_file.flush()
+    else:
+        # parallel download
+        def _download_part(start, end):
+            headers = {}
+            headers['Range'] = 'bytes=%s-%s' % (start, end)
+            with open(temp_file.name, 'rb+') as f:
+                f.seek(start)
+                r = requests.get(real_url, stream=True, headers=headers, allow_redirects=True, timeout=API_FILE_DOWNLOAD_TIMEOUT)
+                r.raise_for_status()
+                for chunk in r.iter_content(chunk_size=API_FILE_DOWNLOAD_READ_CHUNK_SIZE):
+                    if chunk:
+                        f.write(chunk)
+                        progress.update(len(chunk))
+                f.flush()
+
+        executor = futures.ThreadPoolExecutor(max_workers=parallels)
+        part_size = API_FILE_DOWNLOAD_PARALLEL_PART_SIE 
+        tasks = []
+        for i in range(int((total + part_size - 1) / part_size)):
+            start = i * part_size
+            end = start + part_size - 1
+            tasks.append(executor.submit(_download_part, start, end))
+
+         # wait for first exception or all completed
+        done, _ = futures.wait(tasks, return_when=futures.FIRST_EXCEPTION)
+
+        # raise from failed task
+        try:
+            for task in done:
+                task.result()
+        except Exception as exc:
+            # set err flag to notice running futures to terminate immediatly
+            executor.shutdown(wait=False)
+            raise exc
+        else:
+            executor.shutdown(wait=True)
+            
+
     progress.close()
-    temp_file.flush()
 
     downloaded_length = os.path.getsize(temp_file.name)
     if total and total != downloaded_length:
         msg = f"download file '{file_path}' from model '{model_id}' error: expect file size is '{total}', but download size is '{downloaded_length}'"
         raise FileDownloadError(msg)
 
     return downloaded_length
@@ -218,16 +303,17 @@
 def snapshot_download(
     model_id: str,
     local_dir: str,
     *,
     is_public: bool = False,
     revision: Optional[str] = None,
     force_download: bool = False,
-    resume_download: bool = True,
+    resume_download: bool = False,
     ignore_patterns: Optional[Union[List[str], str]] = None,
+    parallels: int = API_FILE_DOWNLOAD_PARALLELS,
 ) -> str:
     """Download repo files.
 
     Download a whole snapshot of a repo's files at the specified revision. This is useful when you want all files from
     a repo, because you don't know which ones you will need a priori. All files are nested inside a folder in order
     to keep their actual filename relative to that folder. You can also filter which files to download using
     `allow_patterns` and `ignore_patterns`.
@@ -247,14 +333,17 @@
             commit hash.
         force_download (`bool`, *optional*, defaults to `False`):
             Whether the file should be downloaded even if it already exists in the local dir.
         resume_download (`bool`, *optional*, defaults to `False):
             If `True`, resume a previously interrupted download.
         ignore_patterns (`List[str]` or `str`, *optional*):
             If provided, files matching any of the patterns are not downloaded.
+        parallels(`int`, *optional*, defaults to `4`):
+            if set to > 1, will use parallel downloading, and must set `resume_download` to `False` at the same time,
+            otherwise Exception will be raised.
 
     Returns:
         Local folder path (string) of repo snapshot
 
     <Tip>
 
     Raises the following errors:
@@ -264,14 +353,27 @@
     - [`OSError`](https://docs.python.org/3/library/exceptions.html#OSError) if
       ETag cannot be determined.
     - [`ValueError`](https://docs.python.org/3/library/exceptions.html#ValueError)
       if some parameter value is invalid
 
     </Tip>
     """
+    if parallels:
+        if not isinstance(parallels, int):
+            raise ValueError('parallel shoud be int type')
+        if parallels < 1:
+            parallels = 1
+        elif parallels > API_FILE_DOWNLOAD_PARALLELS:
+            parallels = API_FILE_DOWNLOAD_PARALLELS
+    else:
+        parallels = 1
+    
+    if parallels > 1 and resume_download:
+        raise ValueError('condition conflict: parallels > 1 while set resume_download=True')
+ 
     if not model_id:
         raise ValueError('model_id shoud not be empty')
 
     if not local_dir:
         raise ValueError('local_dir shoud be specified')
     local_dir_path = Path(local_dir).expanduser()
     if not local_dir_path.exists():
@@ -302,14 +404,15 @@
             file_path,
             is_public=is_public,
             revision=revision,
             local_dir=local_dir,
             force_download=force_download,
             resume_download=resume_download,
             remote_validate=False,
+            parallels=parallels,
         )
     return local_dir
 
 
 def create_and_upload_model(
     model_id: str,
     local_dir: str,
```

## scoamp/commands/api.py

```diff
@@ -121,13 +121,23 @@
 
     # make request
     #from scoamp.api import set_auth_info, set_endpoint
     #set_endpoint(auth.endpoint)
     #set_auth_info(auth.access_key, auth.secret_key)
 
     from scoamp.globals import global_api
-    space_name = 'a520a4e0-b4a3-4746-8117-ee81925ab272'
-    from scoamp.toolkit import create_and_upload_model
-    r = create_and_upload_model('test-0721-1', 'example/model1', space_name, allow_exist=True)
+    from scoamp.toolkit import model_file_download, snapshot_download
+    model_id = 'test-0714-2'
+    file_path = 'mock1.bin'
+    local_dir = 'data/model'
+    is_public = False
+    #r = model_file_download(
+    #    model_id=model_id,
+    #    file_path=file_path,
+    #    local_dir=local_dir,
+    #    remote_validate=False,
+    #    is_public=is_public,
+    #) 
+    r = snapshot_download(model_id=model_id, local_dir=local_dir,)
     print(r)
```

## Comparing `scoamp-0.4.0a3.dist-info/LICENSE` & `scoamp-0.5.0a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scoamp-0.4.0a3.dist-info/METADATA` & `scoamp-0.5.0a0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoamp
-Version: 0.4.0a3
+Version: 0.5.0a0
 Summary: SenseCore AI Model Platform Command Line Tool
 Author: SenseTime, Inc.
 Author-email: hpan@sensetime.com
 License: Apache 2.0
 Keywords: machine-learning deep-learning models
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

## Comparing `scoamp-0.4.0a3.dist-info/RECORD` & `scoamp-0.5.0a0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-scoamp/__init__.py,sha256=grwYdZgmq_CjrYrqng6OLRTMVDWfoVSGwTqiOZ0qvq4,24
-scoamp/api.py,sha256=uJNzWsra5PVxCNSd2XysKNffAxR7f_lXoswDgeua4jA,7991
+scoamp/__init__.py,sha256=C55E3q6EEHsiDCJvdvMsJD3Hv9Rxxd9RNfMZdqcFFc4,24
+scoamp/api.py,sha256=31h4x68wUgFPgtSEJt_7cRU6WyrO_tRgCxAMkOaB9Mg,8052
 scoamp/globals.py,sha256=5YSnbgclYWmPEcgQZK0mUXqqijb7-MMK5HeIeeshK4o,2212
-scoamp/toolkit.py,sha256=U0XDgyfyR_5FD-_pH6bLXV5jvuWXFcB5skeDHYUEUT4,15216
+scoamp/toolkit.py,sha256=nr6mwgAUaUQS0_-EGbT77qQEEphpMNX5vK7d6hRO4rg,19171
 scoamp/commands/__init__.py,sha256=y1F-rP1F_zPOEYhMd_wRmC9a6ZZyr9QcE4GWkIbT0og,486
-scoamp/commands/api.py,sha256=gL_0BFSJi0hw3umtSRPY5h2cgDnKDOqYQpTGrthYxZE,4381
+scoamp/commands/api.py,sha256=vTCfpcxbjHjshkvKG54mHn3pVU4RCGJWvgV6sozffs8,4608
 scoamp/commands/lfs.py,sha256=YA4Zj7W7lzoYQF-ulcG1bRgnJ0TXyi_D0JE4aLNNJzU,7581
 scoamp/schema/public-model-meta.json,sha256=EIQMSVftVNCt6GS6-x9XbKirK-SS75mJRKMsFQWCsEg,2135
 scoamp/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scoamp/utils/api_utils.py,sha256=P9JHJl2KHOqspJrHMOsLvJl-FY3CpjBWDjglNncGQHU,5080
 scoamp/utils/decrypt.py,sha256=EUaCTnBnp2aoh5RXwGB9-Gd81W-j23Zubmh68Rv_To8,501
 scoamp/utils/error.py,sha256=oLeuhUsB-pc3pi8o5kZNpB4lZcK-H4JtSjDdIMOjE_Q,1779
 scoamp/utils/helper.py,sha256=KLH089HaSyENxYb0c0o9b1aUJgvnGWL6GYInAfEdEF0,5150
 scoamp/utils/logger.py,sha256=YpQWJbDfWtGG9kpRcGefULZVLYu34zXkCDjPvZTeZLY,421
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_utils_helper.py,sha256=gFx9h7jjiCao2hbZoT_ES08xtrFRizfPLIvp17uronQ,9110
-scoamp-0.4.0a3.dist-info/LICENSE,sha256=R-z_qud7owqMORJyRv9VAVEhRkcRWJOyCJnyCG4Ds5E,11334
-scoamp-0.4.0a3.dist-info/METADATA,sha256=duUCP5JHNvO6pP6hLsetSV0K2EmuS_oU6Rslb2vj6sQ,1239
-scoamp-0.4.0a3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-scoamp-0.4.0a3.dist-info/entry_points.txt,sha256=2_nLlE4zJ0B1KOQHAxdSH7jHNesWCZXKXSCmtlSBm1A,47
-scoamp-0.4.0a3.dist-info/top_level.txt,sha256=R-1KO00uSz-w1PWLRS6mRHjNP5yFJIKSrafHwVzvYBU,13
-scoamp-0.4.0a3.dist-info/RECORD,,
+scoamp-0.5.0a0.dist-info/LICENSE,sha256=R-z_qud7owqMORJyRv9VAVEhRkcRWJOyCJnyCG4Ds5E,11334
+scoamp-0.5.0a0.dist-info/METADATA,sha256=UmzJeYfowzzMwhhp0c10QPhTS_l1HDmzrnzzXJC2bzY,1239
+scoamp-0.5.0a0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+scoamp-0.5.0a0.dist-info/entry_points.txt,sha256=2_nLlE4zJ0B1KOQHAxdSH7jHNesWCZXKXSCmtlSBm1A,47
+scoamp-0.5.0a0.dist-info/top_level.txt,sha256=R-1KO00uSz-w1PWLRS6mRHjNP5yFJIKSrafHwVzvYBU,13
+scoamp-0.5.0a0.dist-info/RECORD,,
```

