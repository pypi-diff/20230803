# Comparing `tmp/dvelopdmspy-1.0.2.tar.gz` & `tmp/dvelopdmspy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvelopdmspy-1.0.2.tar", last modified: Mon Jul  3 13:46:15 2023, max compression
+gzip compressed data, was "dvelopdmspy-1.0.3.tar", last modified: Thu Aug  3 13:29:22 2023, max compression
```

## Comparing `dvelopdmspy-1.0.2.tar` & `dvelopdmspy-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:46:15.339555 dvelopdmspy-1.0.2/
--rw-rw-rw-   0        0        0    35817 2023-06-30 10:23:56.000000 dvelopdmspy-1.0.2/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-30 10:23:56.000000 dvelopdmspy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1126 2023-07-03 13:46:15.339555 dvelopdmspy-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 13:46:15.324597 dvelopdmspy-1.0.2/dvelopdmspy/
--rw-rw-rw-   0        0        0        0 2023-06-30 10:18:01.000000 dvelopdmspy-1.0.2/dvelopdmspy/__init__.py
--rw-rw-rw-   0        0        0     4841 2023-07-03 13:43:40.000000 dvelopdmspy-1.0.2/dvelopdmspy/dvelopdmspy.py
--rw-rw-rw-   0        0        0       50 2023-06-30 10:23:56.000000 dvelopdmspy-1.0.2/dvelopdmspy/exceptions.py
--rw-rw-rw-   0        0        0     4794 2023-07-03 12:44:25.000000 dvelopdmspy-1.0.2/dvelopdmspy/models.py
--rw-rw-rw-   0        0        0     4808 2023-07-03 12:54:42.000000 dvelopdmspy-1.0.2/dvelopdmspy/rest_adapter.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:46:15.338558 dvelopdmspy-1.0.2/dvelopdmspy.egg-info/
--rw-rw-rw-   0        0        0     1126 2023-07-03 13:46:15.000000 dvelopdmspy-1.0.2/dvelopdmspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-07-03 13:46:15.000000 dvelopdmspy-1.0.2/dvelopdmspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:46:15.000000 dvelopdmspy-1.0.2/dvelopdmspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-03 13:46:15.000000 dvelopdmspy-1.0.2/dvelopdmspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 13:46:15.000000 dvelopdmspy-1.0.2/dvelopdmspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 13:46:15.340552 dvelopdmspy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-07-03 13:46:10.000000 dvelopdmspy-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:29:22.708608 dvelopdmspy-1.0.3/
+-rw-rw-rw-   0        0        0    35817 2023-06-30 10:23:56.000000 dvelopdmspy-1.0.3/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-30 10:23:56.000000 dvelopdmspy-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1126 2023-08-03 13:29:22.707611 dvelopdmspy-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 13:29:22.689664 dvelopdmspy-1.0.3/dvelopdmspy/
+-rw-rw-rw-   0        0        0        0 2023-06-30 10:18:01.000000 dvelopdmspy-1.0.3/dvelopdmspy/__init__.py
+-rw-rw-rw-   0        0        0     6756 2023-08-03 13:27:38.000000 dvelopdmspy-1.0.3/dvelopdmspy/dvelopdmspy.py
+-rw-rw-rw-   0        0        0       50 2023-06-30 10:23:56.000000 dvelopdmspy-1.0.3/dvelopdmspy/exceptions.py
+-rw-rw-rw-   0        0        0     4934 2023-08-03 12:30:41.000000 dvelopdmspy-1.0.3/dvelopdmspy/models.py
+-rw-rw-rw-   0        0        0     5929 2023-08-03 13:28:17.000000 dvelopdmspy-1.0.3/dvelopdmspy/rest_adapter.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:29:22.706614 dvelopdmspy-1.0.3/dvelopdmspy.egg-info/
+-rw-rw-rw-   0        0        0     1126 2023-08-03 13:29:22.000000 dvelopdmspy-1.0.3/dvelopdmspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-08-03 13:29:22.000000 dvelopdmspy-1.0.3/dvelopdmspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 13:29:22.000000 dvelopdmspy-1.0.3/dvelopdmspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-03 13:29:22.000000 dvelopdmspy-1.0.3/dvelopdmspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 13:29:22.000000 dvelopdmspy-1.0.3/dvelopdmspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 13:29:22.708608 dvelopdmspy-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-08-03 13:29:09.000000 dvelopdmspy-1.0.3/setup.py
```

### Comparing `dvelopdmspy-1.0.2/COPYING` & `dvelopdmspy-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `dvelopdmspy-1.0.2/LICENSE` & `dvelopdmspy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvelopdmspy-1.0.2/PKG-INFO` & `dvelopdmspy-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvelopdmspy
-Version: 1.0.2
+Version: 1.0.3
 Summary: d.velop DMS API wrapper for python
 Home-page: https://github.com/seb-bau/dvelop_dms_py
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dvelopdmspy-1.0.2/dvelopdmspy/dvelopdmspy.py` & `dvelopdmspy-1.0.3/dvelopdmspy/dvelopdmspy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import os
 
 import humps
 from dvelopdmspy.rest_adapter import RestAdapter
 from dvelopdmspy.exceptions import DvelopDMSPyException
 from dvelopdmspy.models import *
 
 
@@ -42,21 +43,74 @@
             pdict = {}
         t_key = self._get_property_key_from_name(display_name)
         if type(pvalue) != list:
             pvalue = [pvalue]
         pdict[t_key] = pvalue
         return pdict
 
+    def add_upload_property(self, display_name: str, pvalue, plist: list = None) -> list:
+        if plist is None:
+            plist = []
+        t_key = self._get_property_key_from_name(display_name)
+        if type(pvalue) != list:
+            pvalue = [pvalue]
+        plist.append({
+            'key': t_key,
+            'values': pvalue
+        })
+        return plist
+
     def add_category(self, display_name, plist: list = None) -> list:
         if plist is None:
             plist = []
         t_key = self._get_category_key_from_name(display_name)
         plist.append(t_key)
         return plist
 
+    def archive_file(self,
+                     filepath: str,
+                     category_id: str,
+                     properties: list[dict]) -> str | bool:
+        # Blob Upload
+        blob_endpoint = "blob/chunk/"
+        result = self._rest_adapter.post(endpoint=blob_endpoint, binary_upload=True, upload_file_path=filepath)
+        if result.status_code != 201 or "location" not in result.headers:
+            raise DvelopDMSPyException("BLOB upload failed. No blob location detected")
+        blob_location = result.headers["location"]
+
+        # Archivdokument erstellen und mit Blob verbinden
+        blob_to_doc_endpoint = "o2m"
+
+        release_property = {
+            'key': 'property_state',
+            'values': [
+                'Release'
+            ]
+        }
+        properties.append(release_property)
+
+        post_body = {
+            'filename': os.path.basename(filepath),
+            'sourceCategory': category_id,
+            'sourceId': f'/dms/r/{self._rest_adapter.repository}/source',
+            'contentLocationUri': blob_location,
+            'sourceProperties': {
+                'properties': properties
+            }
+        }
+
+        result = self._rest_adapter.post(endpoint=blob_to_doc_endpoint, data=post_body)
+        try:
+            t_loc = result.headers.get("Location")
+            t_doc_id = t_loc.split('?')[0].split('/')[-1]
+        except (KeyError, ValueError):
+            t_doc_id = "unknown"
+
+        return t_doc_id
+
     def get_documents(self,
                       properties: dict[SearchProperty] = None,
                       categories: list[str] = None,
                       limit: int = None,
                       doc_id: str = None) -> List[DmsDocument]:
         ret_docs = []
         params = {
@@ -124,8 +178,7 @@
         prop_key = self._get_property_key_from_name(prop_display_name)
         for prop in doc_obj.source_properties:
             if prop.key == prop_key:
                 if prop.values is None:
                     return prop.value
                 else:
                     return prop.values
-
```

### Comparing `dvelopdmspy-1.0.2/dvelopdmspy/models.py` & `dvelopdmspy-1.0.3/dvelopdmspy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import List, Dict, Optional
 from uuid import UUID
 from enum import Enum
 
 import requests
+from requests.structures import CaseInsensitiveDict
 
 
 class Result:
-    def __init__(self, status_code: int, message: str = '', data: List[Dict] = None, raw: requests.Response = None):
+    def __init__(self, status_code: int, message: str = '', data: List[Dict] = None, raw: requests.Response = None,
+                 headers: CaseInsensitiveDict = None):
         self.status_code = int(status_code)
         self.message = str(message)
         self.data = data if data else []
         self.raw = raw
+        self.headers = headers
 
 
 class Links:
     links_self: str
     preview_readonly: Optional[str]
     delete_with_reason: Optional[str]
     mainblobcontent: str
```

### Comparing `dvelopdmspy-1.0.2/dvelopdmspy/rest_adapter.py` & `dvelopdmspy-1.0.3/dvelopdmspy/rest_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,22 +34,25 @@
         print(f"Repository {self.repository}")
 
     def get(self, endpoint: str, ep_params: Dict = None, base_url: str = None, binary: bool = False,
             limit: int = None) -> Result:
         return self._do(http_method='GET', endpoint=endpoint, ep_params=ep_params, base_url=base_url, binary=binary,
                         limit=limit)
 
-    def post(self, endpoint: str, ep_params: Dict = None, data: Dict = None) -> Result:
-        return self._do(http_method='POST', endpoint=endpoint, ep_params=ep_params, data=data)
+    def post(self, endpoint: str, ep_params: Dict = None, data: Dict = None, binary_upload: bool = False,
+             upload_file_path: str = None) -> Result:
+        return self._do(http_method='POST', endpoint=endpoint, ep_params=ep_params, data=data,
+                        binary_upload=binary_upload, upload_file_path=upload_file_path)
 
     def delete(self, endpoint: str, ep_params: Dict = None, data: Dict = None) -> Result:
         return self._do(http_method='DELETE', endpoint=endpoint, ep_params=ep_params, data=data)
 
     def _do(self, http_method: str, endpoint: str, ep_params: Dict = None, data: Dict = None,
-            base_url: str = None, binary: bool = False, limit: int = None) -> Result:
+            base_url: str = None, binary: bool = False, limit: int = None, binary_upload: bool = False,
+            upload_file_path: str = None) -> Result:
 
         if base_url is None:
             base_url = self.url
 
         if ep_params is None:
             ep_params = {}
 
@@ -61,54 +64,76 @@
         }
 
         if binary:
             headers['Accept'] = 'application/octet-stream'
         else:
             headers['Accept'] = 'application/hal+json'
 
+        if http_method == 'POST':
+            headers['Origin'] = f'https://{self.host_base}'
+
+        blobdata = None
+        if binary_upload:
+            headers['Content-Type'] = 'application/octet-stream'
+
+            try:
+                with open(upload_file_path, 'rb') as f:
+                    blobdata = f.read()
+            except IOError as e:
+                self._logger.error(msg=(str(e)))
+                raise DvelopDMSPyException("Blob upload failed") from e
+
         log_line_pre = f"method={http_method}, url={full_url}"
         log_line_post = ', '.join((log_line_pre, "success={}, status_code={}, message={}"))
         merge_schema = {"mergeStrategy": "append"}
         merger = Merger(schema=merge_schema)
 
         try:
             self._logger.debug(msg=log_line_pre)
-            response = requests.request(method=http_method, url=full_url, headers=headers, params=ep_params, json=data)
+            response = requests.request(method=http_method, url=full_url, headers=headers, params=ep_params, json=data,
+                                        data=blobdata)
         except requests.exceptions.RequestException as e:
             self._logger.error(msg=(str(e)))
             raise DvelopDMSPyException("Request failed") from e
 
-        if not binary:
+        if not binary and not binary_upload:
+            data_out = None
             try:
-                if "items" in response.json().keys():
-                    data_out = response.json().get("items")
-                else:
-                    data_out = response.json()
-            except (ValueError, JSONDecodeError) as e:
-                self._logger.error(msg=log_line_post.format(False, None, e))
-                raise DvelopDMSPyException("Bad JSON in response") from e
-
-            if "_links" in response.json().keys():
-                doc_count = len(data_out)
-                while "next" in response.json()['_links']:
-                    if limit is not None and doc_count >= limit:
-                        break
-                    response = requests.request(method=http_method,
-                                                url=f"https://"
-                                                    f"{self.host_base}{response.json()['_links']['next']['href']}",
-                                                headers=headers)
-                    data_out = merger.merge(data_out, response.json()['items'])
+                jsresp = response.json()
+                data_out = jsresp
+                try:
+                    if "items" in jsresp.keys():
+                        data_out = jsresp.get("items")
+                    else:
+                        data_out = jsresp
+                except (ValueError, JSONDecodeError) as e:
+                    self._logger.info(msg=log_line_post.format(False, None, e))
+                    raise DvelopDMSPyException(f"Bad JSON in response --> {response.text}") from e
+
+                if "_links" in jsresp.keys():
                     doc_count = len(data_out)
+                    while "next" in response.json()['_links']:
+                        if limit is not None and doc_count >= limit:
+                            break
+                        response = requests.request(method=http_method,
+                                                    url=f"https://"
+                                                        f"{self.host_base}{response.json()['_links']['next']['href']}",
+                                                    headers=headers)
+                        data_out = merger.merge(data_out, response.json()['items'])
+                        doc_count = len(data_out)
+            except JSONDecodeError:
+                pass
         else:
             data_out = None
 
         is_success = 200 <= response.status_code <= 299
         log_line = log_line_post.format(is_success, response.status_code, response.reason)
         if is_success:
             self._logger.debug(msg=log_line)
             if binary:
                 raw = response
             else:
                 raw = None
-            return Result(response.status_code, message=response.reason, data=data_out, raw=raw)
+            return Result(response.status_code, message=response.reason, data=data_out, raw=raw,
+                          headers=response.headers)
         self._logger.error(msg=log_line)
-        raise DvelopDMSPyException(f"{response.status_code}: {response.reason}")
+        raise DvelopDMSPyException(f"{response.status_code}: {response.reason} --> {response.text}")
```

### Comparing `dvelopdmspy-1.0.2/dvelopdmspy.egg-info/PKG-INFO` & `dvelopdmspy-1.0.3/dvelopdmspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvelopdmspy
-Version: 1.0.2
+Version: 1.0.3
 Summary: d.velop DMS API wrapper for python
 Home-page: https://github.com/seb-bau/dvelop_dms_py
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dvelopdmspy-1.0.2/setup.py` & `dvelopdmspy-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dvelopdmspy',
-    version='1.0.2',
+    version='1.0.3',
     description='d.velop DMS API wrapper for python',
     url='https://github.com/seb-bau/dvelop_dms_py',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['dvelopdmspy'],
     install_requires=['requests>=2.0',
@@ -29,8 +29,8 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
-)
+)
```

