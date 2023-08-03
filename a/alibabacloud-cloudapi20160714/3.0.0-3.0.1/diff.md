# Comparing `tmp/alibabacloud_cloudapi20160714-3.0.0.tar.gz` & `tmp/alibabacloud_cloudapi20160714-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudapi20160714-3.0.0.tar", last modified: Mon Jul 31 02:29:31 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cloudapi20160714-3.0.1.tar", last modified: Thu Aug  3 10:39:24 2023, max compression
```

## Comparing `alibabacloud_cloudapi20160714-3.0.0.tar` & `alibabacloud_cloudapi20160714-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     2278 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/__init__.py
--rw-r--r--   0 root         (0) root         (0)   710306 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/client.py
--rw-r--r--   0 root         (0) root         (0)  1396813 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   713764 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714/client.py
+-rw-r--r--   0 root         (0) root         (0)  1402778 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-08-03 10:39:24.000000 alibabacloud_cloudapi20160714-3.0.1/setup.py
```

### Comparing `alibabacloud_cloudapi20160714-3.0.0/ChangeLog.md` & `alibabacloud_cloudapi20160714-3.0.1/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2023-07-31 Version: 3.0.0
+- CreateApp add Extend parameter.
+- DescribeAppAttributes add Extend parameter.
+- DescribeApp add Extend parameter.
+- ModifyApp add Extend parameter.
+
 2023-06-19 Version: 2.2.20
 - Republish.
 
 2023-06-19 Version: 2.2.19
 - Update DescribeApiGroup and DescribeInstances.
 - Add DescribeSummaryData.
```

### Comparing `alibabacloud_cloudapi20160714-3.0.0/LICENSE` & `alibabacloud_cloudapi20160714-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714-3.0.0/PKG-INFO` & `alibabacloud_cloudapi20160714-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudapi20160714
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714-3.0.0/README-CN.md` & `alibabacloud_cloudapi20160714-3.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714-3.0.0/README.md` & `alibabacloud_cloudapi20160714-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/client.py` & `alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8139,14 +8139,100 @@
         
         @param request: DescribeDomainRequest
         @return: DescribeDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_with_options_async(request, runtime)
 
+    def describe_group_qps_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeGroupQpsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeGroupQpsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeGroupQps',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeGroupQpsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_group_qps_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeGroupQpsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeGroupQpsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeGroupQps',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeGroupQpsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_group_qps(
+        self,
+        request: cloud_api20160714_models.DescribeGroupQpsRequest,
+    ) -> cloud_api20160714_models.DescribeGroupQpsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_group_qps_with_options(request, runtime)
+
+    async def describe_group_qps_async(
+        self,
+        request: cloud_api20160714_models.DescribeGroupQpsRequest,
+    ) -> cloud_api20160714_models.DescribeGroupQpsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_group_qps_with_options_async(request, runtime)
+
     def describe_history_apis_with_options(
         self,
         request: cloud_api20160714_models.DescribeHistoryApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeHistoryApisResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/models.py` & `alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -22069,14 +22069,212 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeGroupQpsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        group_id: str = None,
+        security_token: str = None,
+        stage_name: str = None,
+        start_time: str = None,
+    ):
+        self.end_time = end_time
+        self.group_id = group_id
+        self.security_token = security_token
+        self.stage_name = stage_name
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeGroupQpsResponseBodyGroupQpsMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        self.item_time = item_time
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeGroupQpsResponseBodyGroupQps(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeGroupQpsResponseBodyGroupQpsMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeGroupQpsResponseBodyGroupQpsMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeGroupQpsResponseBody(TeaModel):
+    def __init__(
+        self,
+        group_qps: DescribeGroupQpsResponseBodyGroupQps = None,
+        request_id: str = None,
+    ):
+        self.group_qps = group_qps
+        self.request_id = request_id
+
+    def validate(self):
+        if self.group_qps:
+            self.group_qps.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.group_qps is not None:
+            result['GroupQps'] = self.group_qps.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupQps') is not None:
+            temp_model = DescribeGroupQpsResponseBodyGroupQps()
+            self.group_qps = temp_model.from_map(m['GroupQps'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeGroupQpsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeGroupQpsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeGroupQpsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeHistoryApisRequest(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         api_name: str = None,
         group_id: str = None,
         page_number: str = None,
```

### Comparing `alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/PKG-INFO` & `alibabacloud_cloudapi20160714-3.0.1/alibabacloud_cloudapi20160714.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudapi20160714
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714-3.0.0/setup.py` & `alibabacloud_cloudapi20160714-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudapi20160714.
 
-Created on 31/07/2023
+Created on 03/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudapi20160714"
 NAME = "alibabacloud_cloudapi20160714" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CloudAPI (20160714) SDK Library for Python"
```

