# Comparing `tmp/cortex_xdr_client-1.8.5.tar.gz` & `tmp/cortex_xdr_client-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_xdr_client-1.8.5.tar", max compression
+gzip compressed data, was "cortex_xdr_client-1.8.6.tar", max compression
```

## Comparing `cortex_xdr_client-1.8.5.tar` & `cortex_xdr_client-1.8.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/LICENSE
--rw-r--r--   0        0        0     3617 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/README.rst
--rw-r--r--   0        0        0       61 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/__init__.py
--rw-r--r--   0        0        0     2059 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/actions_api.py
--rw-r--r--   0        0        0     3387 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/alerts_api.py
--rw-r--r--   0        0        0     1544 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/authentication.py
--rw-r--r--   0        0        0     2376 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/base_api.py
--rw-r--r--   0        0        0     1037 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/download_api.py
--rw-r--r--   0        0        0    15639 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/endpoints_api.py
--rw-r--r--   0        0        0     5261 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/incidents_api.py
--rw-r--r--   0        0        0        0 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/__init__.py
--rw-r--r--   0        0        0      390 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/action_status.py
--rw-r--r--   0        0        0     5902 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/alerts.py
--rw-r--r--   0        0        0     2721 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/endpoints.py
--rw-r--r--   0        0        0      692 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/exceptions.py
--rw-r--r--   0        0        0     2835 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/filters.py
--rw-r--r--   0        0        0     7770 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/incidents.py
--rw-r--r--   0        0        0     2392 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/scripts.py
--rw-r--r--   0        0        0    12326 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/scripts_api.py
--rw-r--r--   0        0        0     5414 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/xql_api.py
--rw-r--r--   0        0        0     2341 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/client.py
--rw-r--r--   0        0        0      646 2023-06-12 08:48:31.307594 cortex_xdr_client-1.8.5/pyproject.toml
--rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/LICENSE
+-rw-r--r--   0        0        0     3059 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/README.rst
+-rw-r--r--   0        0        0       61 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/__init__.py
+-rw-r--r--   0        0        0     2059 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/actions_api.py
+-rw-r--r--   0        0        0     3387 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/alerts_api.py
+-rw-r--r--   0        0        0     1544 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/authentication.py
+-rw-r--r--   0        0        0     2376 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/base_api.py
+-rw-r--r--   0        0        0     1037 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/download_api.py
+-rw-r--r--   0        0        0    15639 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/endpoints_api.py
+-rw-r--r--   0        0        0     5261 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/incidents_api.py
+-rw-r--r--   0        0        0     1175 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/ioc_api.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/__init__.py
+-rw-r--r--   0        0        0      390 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/action_status.py
+-rw-r--r--   0        0        0     5902 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/alerts.py
+-rw-r--r--   0        0        0     2721 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/endpoints.py
+-rw-r--r--   0        0        0      692 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/exceptions.py
+-rw-r--r--   0        0        0     2835 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/filters.py
+-rw-r--r--   0        0        0     7770 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/incidents.py
+-rw-r--r--   0        0        0     2617 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/ioc.py
+-rw-r--r--   0        0        0     2392 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/scripts.py
+-rw-r--r--   0        0        0    12326 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/scripts_api.py
+-rw-r--r--   0        0        0     5414 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/xql_api.py
+-rw-r--r--   0        0        0     2547 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/client.py
+-rw-r--r--   0        0        0      646 2023-08-03 17:44:59.971677 cortex_xdr_client-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.6/PKG-INFO
```

### Comparing `cortex_xdr_client-1.8.5/LICENSE` & `cortex_xdr_client-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/actions_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/alerts_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/authentication.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/authentication.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/base_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/base_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/download_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/download_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/endpoints_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/endpoints_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/incidents_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/alerts.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/endpoints.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/exceptions.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/filters.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/filters.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/incidents.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/incidents.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/scripts.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/scripts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/scripts_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/scripts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/api/xql_api.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/api/xql_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.5/cortex_xdr_client/client.py` & `cortex_xdr_client-1.8.6/cortex_xdr_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import Tuple
 
 from cortex_xdr_client.api.actions_api import ActionsAPI
 from cortex_xdr_client.api.alerts_api import AlertsAPI
 from cortex_xdr_client.api.authentication import Authentication
+from cortex_xdr_client.api.download_api import DownloadAPI
 from cortex_xdr_client.api.endpoints_api import EndpointsAPI
 from cortex_xdr_client.api.incidents_api import IncidentsAPI
+from cortex_xdr_client.api.ioc_api import IocAPI
 from cortex_xdr_client.api.scripts_api import ScriptsAPI
 from cortex_xdr_client.api.xql_api import XQLAPI
-from cortex_xdr_client.api.download_api import DownloadAPI
 
 
 class CortexXDRClient(object):
     incidents_api: IncidentsAPI
     alerts_api: AlertsAPI
     endpoints_api: EndpointsAPI
     scripts_api: ScriptsAPI
     xql_api: XQLAPI
     actions_api: ActionsAPI
     download_api: DownloadAPI
+    ioc_api: IocAPI
 
     def __init__(self, auth: Authentication, fqdn: str, default_timeout: Tuple[int, int] = (10, 60)) -> None:
         """
         Constructor of the CortexXDRClient class. This class is used to interact with the Cortex XDR API.
         :param auth: The Authentication object containing type
         :param api_key: The API key value to use.
         :param fqdn: The fully qualified domain name of the Cortex XDR server.
@@ -44,7 +46,10 @@
                               timeout=default_timeout)
         self.actions_api = ActionsAPI(auth=auth,
                                       fqdn=fqdn,
                                       timeout=default_timeout)
         self.download_api = DownloadAPI(auth=auth,
                                       fqdn=fqdn,
                                       timeout=default_timeout)
+        self.ioc_api = IocAPI(auth=auth,
+                              fqdn=fqdn,
+                              timeout=default_timeout)
```

### Comparing `cortex_xdr_client-1.8.5/pyproject.toml` & `cortex_xdr_client-1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "cortex-xdr-client"
 packages= [
     { include = "cortex_xdr_client", from="." },
 ]
-version = "v1.8.5"
+version = "v1.8.6"
 description = "API client for Cortex XDR Prevent"
 authors = ["ebarti"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ebarti/cortex-xdr-client"
 repository = "https://github.com/ebarti/cortex-xdr-client"
```

