# Comparing `tmp/caveclient-5.7.0.tar.gz` & `tmp/caveclient-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.7.0.tar", last modified: Mon May 29 21:18:30 2023, max compression
+gzip compressed data, was "caveclient-5.8.0.tar", last modified: Thu Aug  3 15:58:30 2023, max compression
```

## Comparing `caveclient-5.7.0.tar` & `caveclient-5.8.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.933795 caveclient-5.7.0/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.7.0/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-29 21:18:30.929004 caveclient-5.7.0/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.7.0/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.900091 caveclient-5.7.0/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-29 21:17:44.000000 caveclient-5.7.0/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.7.0/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.7.0/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.7.0/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    39464 2023-05-29 21:15:16.000000 caveclient-5.7.0/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.7.0/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.7.0/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.7.0/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.7.0/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.7.0/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.7.0/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    91183 2023-05-19 22:16:03.000000 caveclient-5.7.0/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)      778 2023-05-19 14:30:34.000000 caveclient-5.7.0/caveclient/mytimer.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.7.0/caveclient/session_config.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.911890 caveclient-5.7.0/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.905964 caveclient-5.7.0/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      870 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.7.0/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-29 21:18:30.934331 caveclient-5.7.0/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.7.0/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.918129 caveclient-5.7.0/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.7.0/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.7.0/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.7.0/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.7.0/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.7.0/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.7.0/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-03 15:58:30.693181 caveclient-5.8.0/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.8.0/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-08-03 15:58:30.692956 caveclient-5.8.0/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.8.0/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-03 15:58:30.683479 caveclient-5.8.0/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-08-03 15:58:27.000000 caveclient-5.8.0/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.8.0/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.8.0/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.8.0/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    39497 2023-06-02 20:24:45.000000 caveclient-5.8.0/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.8.0/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.8.0/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.8.0/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.8.0/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.8.0/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.8.0/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.8.0/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3943 2023-06-07 19:45:31.000000 caveclient-5.8.0/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    91591 2023-08-03 15:57:53.000000 caveclient-5.8.0/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      778 2023-05-19 14:30:34.000000 caveclient-5.8.0/caveclient/mytimer.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.8.0/caveclient/session_config.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-03 15:58:30.689532 caveclient-5.8.0/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.8.0/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.8.0/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.8.0/caveclient/tools/stage.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    19422 2023-08-03 15:57:53.000000 caveclient-5.8.0/caveclient/tools/table_manager.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-03 15:58:30.687790 caveclient-5.8.0/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-08-03 15:58:30.000000 caveclient-5.8.0/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      904 2023-08-03 15:58:30.000000 caveclient-5.8.0/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-08-03 15:58:30.000000 caveclient-5.8.0/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-08-03 15:58:30.000000 caveclient-5.8.0/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-08-03 15:58:30.000000 caveclient-5.8.0/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.8.0/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-08-03 15:58:30.693396 caveclient-5.8.0/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.8.0/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-03 15:58:30.692397 caveclient-5.8.0/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.8.0/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.8.0/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.8.0/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.8.0/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.8.0/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.8.0/tests/test_materialization.py
```

### Comparing `caveclient-5.7.0/README.rst` & `caveclient-5.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/annotationengine.py` & `caveclient-5.8.0/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/auth.py` & `caveclient-5.8.0/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/base.py` & `caveclient-5.8.0/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/chunkedgraph.py` & `caveclient-5.8.0/caveclient/chunkedgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     return data
 
 
 def root_id_int_list_check(
     root_id,
     make_unique=False,
 ):
-    if isinstance(root_id, int) or isinstance(root_id, np.uint64):
+    if isinstance(root_id, int) or isinstance(root_id, np.uint64) or isinstance(root_id, np.int64):
         root_id = [root_id]
     elif isinstance(root_id, str):
         try:
             root_id = np.uint64(root_id)
         except ValueError as esc:
             raise ValueError(
                 "When passing a string for 'root_id' make sure the string can be converted to a uint64"
```

### Comparing `caveclient-5.7.0/caveclient/datastack_lookup.py` & `caveclient-5.8.0/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/emannotationschemas.py` & `caveclient-5.8.0/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/endpoints.py` & `caveclient-5.8.0/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/format_utils.py` & `caveclient-5.8.0/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/frameworkclient.py` & `caveclient-5.8.0/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/infoservice.py` & `caveclient-5.8.0/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/jsonservice.py` & `caveclient-5.8.0/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/l2cache.py` & `caveclient-5.8.0/caveclient/l2cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     table_name=None,
     auth_client=None,
     api_version="latest",
     max_retries=None,
     pool_maxsize=None,
     pool_block=None,
     over_client=None,
+    verify=True,
 ):
     if auth_client is None:
         auth_client = AuthClient()
 
     auth_header = auth_client.request_header
     endpoints, api_version = _api_endpoints(
         api_version,
@@ -39,14 +40,15 @@
         endpoints=endpoints,
         server_name=server_key,
         table_name=table_name,
         max_retries=max_retries,
         pool_maxsize=pool_maxsize,
         pool_block=pool_block,
         over_client=over_client,
+        verify=verify,
     )
 
 
 class L2CacheClientLegacy(ClientBase):
     def __init__(
         self,
         server_address,
@@ -55,25 +57,27 @@
         endpoints,
         server_name,
         table_name=None,
         max_retries=None,
         pool_maxsize=None,
         pool_block=None,
         over_client=None,
+        verify=True,
     ):
         super(L2CacheClientLegacy, self).__init__(
             server_address,
             auth_header,
             api_version,
             endpoints,
             server_name,
             max_retries=max_retries,
             pool_maxsize=pool_maxsize,
             pool_block=pool_block,
             over_client=over_client,
+            verify=verify,
         )
         self._default_url_mapping["table_id"] = table_name
         self._available_attributes = None
 
     @property
     def default_url_mapping(self):
         return self._default_url_mapping.copy()
```

### Comparing `caveclient-5.7.0/caveclient/materializationengine.py` & `caveclient-5.8.0/caveclient/materializationengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .base import (
     ClientBase,
     BaseEncoder,
     _api_endpoints,
     handle_response,
 )
 from cachetools import cached, TTLCache
+from .tools.table_manager import TableManager, ViewManager
 import logging
 
 logger = logging.getLogger(__name__)
 
 SERVER_KEY = "me_server_address"
 
 
@@ -227,14 +228,16 @@
         if cg_client is None:
             if self.fc is not None:
                 self.cg_client = self.fc.chunkedgraph
         else:
             self.cg_client = cg_client
         self.synapse_table = synapse_table
         self.desired_resolution = desired_resolution
+        self._tables = None
+        self._views = None
 
     @property
     def datastack_name(self):
         return self._datastack_name
 
     @property
     def version(self):
@@ -277,14 +280,27 @@
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["datastack_name"] = datastack_name
         url = self._endpoints["versions"].format_map(endpoint_mapping)
         response = self.session.get(url)
         self.raise_for_status(response)
         return response.json()
 
+
+    @property
+    def tables(self):
+        if self._tables is None:
+            self._tables = TableManager(self.fc)
+        return self._tables
+    
+    @property
+    def views(self):
+        if self._views is None:
+            self._views = ViewManager(self.fc)
+        return self._views
+
     def get_tables(self, datastack_name=None, version=None):
         """Gets a list of table names for a datastack
 
         Parameters
         ----------
         datastack_name : str or None, optional
             Name of the datastack, by default None.
```

### Comparing `caveclient-5.7.0/caveclient/mytimer.py` & `caveclient-5.8.0/caveclient/mytimer.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/session_config.py` & `caveclient-5.8.0/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/tools/caching.py` & `caveclient-5.8.0/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient/tools/stage.py` & `caveclient-5.8.0/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/caveclient.egg-info/SOURCES.txt` & `caveclient-5.8.0/caveclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,13 +22,14 @@
 caveclient.egg-info/SOURCES.txt
 caveclient.egg-info/dependency_links.txt
 caveclient.egg-info/requires.txt
 caveclient.egg-info/top_level.txt
 caveclient/tools/__init__.py
 caveclient/tools/caching.py
 caveclient/tools/stage.py
+caveclient/tools/table_manager.py
 tests/__init__.py
 tests/conftest.py
 tests/test_annotation.py
 tests/test_chunkedgraph.py
 tests/test_infoservice.py
 tests/test_materialization.py
```

### Comparing `caveclient-5.7.0/setup.py` & `caveclient-5.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/tests/conftest.py` & `caveclient-5.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/tests/test_annotation.py` & `caveclient-5.8.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/tests/test_chunkedgraph.py` & `caveclient-5.8.0/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/tests/test_infoservice.py` & `caveclient-5.8.0/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.7.0/tests/test_materialization.py` & `caveclient-5.8.0/tests/test_materialization.py`

 * *Files identical despite different names*

