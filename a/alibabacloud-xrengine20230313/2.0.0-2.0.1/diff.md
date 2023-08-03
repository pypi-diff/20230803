# Comparing `tmp/alibabacloud_xrengine20230313-2.0.0.tar.gz` & `tmp/alibabacloud_xrengine20230313-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.0.0.tar", last modified: Wed Aug  2 08:46:43 2023, max compression
+gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.0.1.tar", last modified: Thu Aug  3 09:19:00 2023, max compression
```

## Comparing `alibabacloud_xrengine20230313-2.0.0.tar` & `alibabacloud_xrengine20230313-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      164 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72515 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/client.py
--rw-r--r--   0 root         (0) root         (0)   245018 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      217 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81239 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/client.py
+-rw-r--r--   0 root         (0) root         (0)   271529 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/setup.py
```

### Comparing `alibabacloud_xrengine20230313-2.0.0/LICENSE` & `alibabacloud_xrengine20230313-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.0.0/PKG-INFO` & `alibabacloud_xrengine20230313-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_xrengine20230313
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-2.0.0/README-CN.md` & `alibabacloud_xrengine20230313-2.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.0.0/README.md` & `alibabacloud_xrengine20230313-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/client.py` & `alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -855,14 +855,84 @@
     async def pop_build_object_project_async(
         self,
         request: xr_engine_20230313_models.PopBuildObjectProjectRequest,
     ) -> xr_engine_20230313_models.PopBuildObjectProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_build_object_project_with_options_async(request, runtime)
 
+    def pop_build_pak_render_project_with_options(
+        self,
+        request: xr_engine_20230313_models.PopBuildPakRenderProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopBuildPakRenderProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.project_id):
+            body['ProjectId'] = request.project_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopBuildPakRenderProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopBuildPakRenderProjectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_build_pak_render_project_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopBuildPakRenderProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopBuildPakRenderProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.project_id):
+            body['ProjectId'] = request.project_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopBuildPakRenderProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopBuildPakRenderProjectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_build_pak_render_project(
+        self,
+        request: xr_engine_20230313_models.PopBuildPakRenderProjectRequest,
+    ) -> xr_engine_20230313_models.PopBuildPakRenderProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_build_pak_render_project_with_options(request, runtime)
+
+    async def pop_build_pak_render_project_async(
+        self,
+        request: xr_engine_20230313_models.PopBuildPakRenderProjectRequest,
+    ) -> xr_engine_20230313_models.PopBuildPakRenderProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_build_pak_render_project_with_options_async(request, runtime)
+
     def pop_build_text_to_avatar_project_with_options(
         self,
         request: xr_engine_20230313_models.PopBuildTextToAvatarProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1105,14 +1175,92 @@
     async def pop_create_object_project_async(
         self,
         request: xr_engine_20230313_models.PopCreateObjectProjectRequest,
     ) -> xr_engine_20230313_models.PopCreateObjectProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_create_object_project_with_options_async(request, runtime)
 
+    def pop_create_pak_render_project_with_options(
+        self,
+        request: xr_engine_20230313_models.PopCreatePakRenderProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopCreatePakRenderProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.ext_info):
+            body['ExtInfo'] = request.ext_info
+        if not UtilClient.is_unset(request.intro):
+            body['Intro'] = request.intro
+        if not UtilClient.is_unset(request.title):
+            body['Title'] = request.title
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopCreatePakRenderProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopCreatePakRenderProjectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_create_pak_render_project_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopCreatePakRenderProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopCreatePakRenderProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.ext_info):
+            body['ExtInfo'] = request.ext_info
+        if not UtilClient.is_unset(request.intro):
+            body['Intro'] = request.intro
+        if not UtilClient.is_unset(request.title):
+            body['Title'] = request.title
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopCreatePakRenderProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopCreatePakRenderProjectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_create_pak_render_project(
+        self,
+        request: xr_engine_20230313_models.PopCreatePakRenderProjectRequest,
+    ) -> xr_engine_20230313_models.PopCreatePakRenderProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_create_pak_render_project_with_options(request, runtime)
+
+    async def pop_create_pak_render_project_async(
+        self,
+        request: xr_engine_20230313_models.PopCreatePakRenderProjectRequest,
+    ) -> xr_engine_20230313_models.PopCreatePakRenderProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_create_pak_render_project_with_options_async(request, runtime)
+
     def pop_create_text_to_avatar_project_with_options(
         self,
         request: xr_engine_20230313_models.PopCreateTextToAvatarProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1703,14 +1851,84 @@
     async def pop_object_project_detail_async(
         self,
         request: xr_engine_20230313_models.PopObjectProjectDetailRequest,
     ) -> xr_engine_20230313_models.PopObjectProjectDetailResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_object_project_detail_with_options_async(request, runtime)
 
+    def pop_query_avatar_project_detail_with_options(
+        self,
+        request: xr_engine_20230313_models.PopQueryAvatarProjectDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopQueryAvatarProjectDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.project_id):
+            query['ProjectId'] = request.project_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PopQueryAvatarProjectDetail',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopQueryAvatarProjectDetailResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_query_avatar_project_detail_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopQueryAvatarProjectDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopQueryAvatarProjectDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.project_id):
+            query['ProjectId'] = request.project_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PopQueryAvatarProjectDetail',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopQueryAvatarProjectDetailResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_query_avatar_project_detail(
+        self,
+        request: xr_engine_20230313_models.PopQueryAvatarProjectDetailRequest,
+    ) -> xr_engine_20230313_models.PopQueryAvatarProjectDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_query_avatar_project_detail_with_options(request, runtime)
+
+    async def pop_query_avatar_project_detail_async(
+        self,
+        request: xr_engine_20230313_models.PopQueryAvatarProjectDetailRequest,
+    ) -> xr_engine_20230313_models.PopQueryAvatarProjectDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_query_avatar_project_detail_with_options_async(request, runtime)
+
     def pop_video_save_source_with_options(
         self,
         request: xr_engine_20230313_models.PopVideoSaveSourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/models.py` & `alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1642,14 +1642,130 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopBuildObjectProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopBuildPakRenderProjectRequest(TeaModel):
+    def __init__(
+        self,
+        project_id: str = None,
+    ):
+        self.project_id = project_id
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
+        if self.project_id is not None:
+            result['ProjectId'] = self.project_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ProjectId') is not None:
+            self.project_id = m.get('ProjectId')
+        return self
+
+
+class PopBuildPakRenderProjectResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class PopBuildPakRenderProjectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopBuildPakRenderProjectResponseBody = None,
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
+            temp_model = PopBuildPakRenderProjectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopBuildTextToAvatarProjectRequest(TeaModel):
     def __init__(
         self,
         project_id: str = None,
     ):
         self.project_id = project_id
 
@@ -3165,14 +3281,261 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopCreateObjectProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopCreatePakRenderProjectRequest(TeaModel):
+    def __init__(
+        self,
+        ext_info: str = None,
+        intro: str = None,
+        title: str = None,
+    ):
+        self.ext_info = ext_info
+        self.intro = intro
+        self.title = title
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
+        if self.ext_info is not None:
+            result['ExtInfo'] = self.ext_info
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.title is not None:
+            result['Title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExtInfo') is not None:
+            self.ext_info = m.get('ExtInfo')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        return self
+
+
+class PopCreatePakRenderProjectResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        auto_build: bool = None,
+        biz_usage: str = None,
+        check_status: str = None,
+        create_mode: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        dependencies: str = None,
+        ext: str = None,
+        id: str = None,
+        intro: str = None,
+        material_cover_url: str = None,
+        modified_time: str = None,
+        status: str = None,
+        title: str = None,
+        type: str = None,
+    ):
+        self.auto_build = auto_build
+        self.biz_usage = biz_usage
+        self.check_status = check_status
+        self.create_mode = create_mode
+        self.create_time = create_time
+        self.deleted = deleted
+        self.dependencies = dependencies
+        self.ext = ext
+        self.id = id
+        self.intro = intro
+        self.material_cover_url = material_cover_url
+        self.modified_time = modified_time
+        self.status = status
+        self.title = title
+        self.type = type
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
+        if self.auto_build is not None:
+            result['AutoBuild'] = self.auto_build
+        if self.biz_usage is not None:
+            result['BizUsage'] = self.biz_usage
+        if self.check_status is not None:
+            result['CheckStatus'] = self.check_status
+        if self.create_mode is not None:
+            result['CreateMode'] = self.create_mode
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.dependencies is not None:
+            result['Dependencies'] = self.dependencies
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.material_cover_url is not None:
+            result['MaterialCoverUrl'] = self.material_cover_url
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoBuild') is not None:
+            self.auto_build = m.get('AutoBuild')
+        if m.get('BizUsage') is not None:
+            self.biz_usage = m.get('BizUsage')
+        if m.get('CheckStatus') is not None:
+            self.check_status = m.get('CheckStatus')
+        if m.get('CreateMode') is not None:
+            self.create_mode = m.get('CreateMode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('Dependencies') is not None:
+            self.dependencies = m.get('Dependencies')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('MaterialCoverUrl') is not None:
+            self.material_cover_url = m.get('MaterialCoverUrl')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class PopCreatePakRenderProjectResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: PopCreatePakRenderProjectResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = PopCreatePakRenderProjectResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class PopCreatePakRenderProjectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopCreatePakRenderProjectResponseBody = None,
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
+            temp_model = PopCreatePakRenderProjectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopCreateTextToAvatarProjectRequest(TeaModel):
     def __init__(
         self,
         ext_info: str = None,
         intro: str = None,
         title: str = None,
     ):
@@ -7185,14 +7548,440 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopObjectProjectDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopQueryAvatarProjectDetailRequest(TeaModel):
+    def __init__(
+        self,
+        project_id: str = None,
+    ):
+        self.project_id = project_id
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
+        if self.project_id is not None:
+            result['ProjectId'] = self.project_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ProjectId') is not None:
+            self.project_id = m.get('ProjectId')
+        return self
+
+
+class PopQueryAvatarProjectDetailResponseBodyDataBuildDetail(TeaModel):
+    def __init__(
+        self,
+        completed_time: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        error_message: str = None,
+        estimated_duration: int = None,
+        modified_time: str = None,
+        running_time: str = None,
+        status: str = None,
+        submit_time: str = None,
+    ):
+        self.completed_time = completed_time
+        self.create_time = create_time
+        self.deleted = deleted
+        self.error_message = error_message
+        self.estimated_duration = estimated_duration
+        self.modified_time = modified_time
+        self.running_time = running_time
+        self.status = status
+        self.submit_time = submit_time
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
+        if self.completed_time is not None:
+            result['CompletedTime'] = self.completed_time
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.estimated_duration is not None:
+            result['EstimatedDuration'] = self.estimated_duration
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.running_time is not None:
+            result['RunningTime'] = self.running_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.submit_time is not None:
+            result['SubmitTime'] = self.submit_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CompletedTime') is not None:
+            self.completed_time = m.get('CompletedTime')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('EstimatedDuration') is not None:
+            self.estimated_duration = m.get('EstimatedDuration')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('RunningTime') is not None:
+            self.running_time = m.get('RunningTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('SubmitTime') is not None:
+            self.submit_time = m.get('SubmitTime')
+        return self
+
+
+class PopQueryAvatarProjectDetailResponseBodyDataDataset(TeaModel):
+    def __init__(
+        self,
+        build_result_url: Dict[str, Any] = None,
+        cover_url: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        error_code: str = None,
+        error_message: str = None,
+        glb_model_url: str = None,
+        model_url: str = None,
+        modified_time: str = None,
+        origin_result_url: str = None,
+        oss_key: str = None,
+        pose_url: str = None,
+        preview_url: str = None,
+    ):
+        self.build_result_url = build_result_url
+        self.cover_url = cover_url
+        self.create_time = create_time
+        self.deleted = deleted
+        self.error_code = error_code
+        self.error_message = error_message
+        self.glb_model_url = glb_model_url
+        self.model_url = model_url
+        self.modified_time = modified_time
+        self.origin_result_url = origin_result_url
+        self.oss_key = oss_key
+        self.pose_url = pose_url
+        self.preview_url = preview_url
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
+        if self.build_result_url is not None:
+            result['BuildResultUrl'] = self.build_result_url
+        if self.cover_url is not None:
+            result['CoverUrl'] = self.cover_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.glb_model_url is not None:
+            result['GlbModelUrl'] = self.glb_model_url
+        if self.model_url is not None:
+            result['ModelUrl'] = self.model_url
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.origin_result_url is not None:
+            result['OriginResultUrl'] = self.origin_result_url
+        if self.oss_key is not None:
+            result['OssKey'] = self.oss_key
+        if self.pose_url is not None:
+            result['PoseUrl'] = self.pose_url
+        if self.preview_url is not None:
+            result['PreviewUrl'] = self.preview_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BuildResultUrl') is not None:
+            self.build_result_url = m.get('BuildResultUrl')
+        if m.get('CoverUrl') is not None:
+            self.cover_url = m.get('CoverUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('GlbModelUrl') is not None:
+            self.glb_model_url = m.get('GlbModelUrl')
+        if m.get('ModelUrl') is not None:
+            self.model_url = m.get('ModelUrl')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('OriginResultUrl') is not None:
+            self.origin_result_url = m.get('OriginResultUrl')
+        if m.get('OssKey') is not None:
+            self.oss_key = m.get('OssKey')
+        if m.get('PoseUrl') is not None:
+            self.pose_url = m.get('PoseUrl')
+        if m.get('PreviewUrl') is not None:
+            self.preview_url = m.get('PreviewUrl')
+        return self
+
+
+class PopQueryAvatarProjectDetailResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        auto_build: bool = None,
+        biz_usage: str = None,
+        build_detail: PopQueryAvatarProjectDetailResponseBodyDataBuildDetail = None,
+        check_status: str = None,
+        create_mode: str = None,
+        create_time: str = None,
+        dataset: PopQueryAvatarProjectDetailResponseBodyDataDataset = None,
+        deleted: bool = None,
+        dependencies: str = None,
+        ext: str = None,
+        id: str = None,
+        intro: str = None,
+        material_cover_url: str = None,
+        modified_time: str = None,
+        status: str = None,
+        title: str = None,
+        type: str = None,
+    ):
+        self.auto_build = auto_build
+        self.biz_usage = biz_usage
+        self.build_detail = build_detail
+        self.check_status = check_status
+        self.create_mode = create_mode
+        self.create_time = create_time
+        self.dataset = dataset
+        self.deleted = deleted
+        self.dependencies = dependencies
+        self.ext = ext
+        self.id = id
+        self.intro = intro
+        self.material_cover_url = material_cover_url
+        self.modified_time = modified_time
+        self.status = status
+        self.title = title
+        self.type = type
+
+    def validate(self):
+        if self.build_detail:
+            self.build_detail.validate()
+        if self.dataset:
+            self.dataset.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_build is not None:
+            result['AutoBuild'] = self.auto_build
+        if self.biz_usage is not None:
+            result['BizUsage'] = self.biz_usage
+        if self.build_detail is not None:
+            result['BuildDetail'] = self.build_detail.to_map()
+        if self.check_status is not None:
+            result['CheckStatus'] = self.check_status
+        if self.create_mode is not None:
+            result['CreateMode'] = self.create_mode
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.dataset is not None:
+            result['Dataset'] = self.dataset.to_map()
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.dependencies is not None:
+            result['Dependencies'] = self.dependencies
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.material_cover_url is not None:
+            result['MaterialCoverUrl'] = self.material_cover_url
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoBuild') is not None:
+            self.auto_build = m.get('AutoBuild')
+        if m.get('BizUsage') is not None:
+            self.biz_usage = m.get('BizUsage')
+        if m.get('BuildDetail') is not None:
+            temp_model = PopQueryAvatarProjectDetailResponseBodyDataBuildDetail()
+            self.build_detail = temp_model.from_map(m['BuildDetail'])
+        if m.get('CheckStatus') is not None:
+            self.check_status = m.get('CheckStatus')
+        if m.get('CreateMode') is not None:
+            self.create_mode = m.get('CreateMode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Dataset') is not None:
+            temp_model = PopQueryAvatarProjectDetailResponseBodyDataDataset()
+            self.dataset = temp_model.from_map(m['Dataset'])
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('Dependencies') is not None:
+            self.dependencies = m.get('Dependencies')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('MaterialCoverUrl') is not None:
+            self.material_cover_url = m.get('MaterialCoverUrl')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class PopQueryAvatarProjectDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: PopQueryAvatarProjectDetailResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = PopQueryAvatarProjectDetailResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class PopQueryAvatarProjectDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopQueryAvatarProjectDetailResponseBody = None,
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
+            temp_model = PopQueryAvatarProjectDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopVideoSaveSourceRequest(TeaModel):
     def __init__(
         self,
         jwt_token: str = None,
         project_id: str = None,
         source_type: str = None,
     ):
```

### Comparing `alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/PKG-INFO` & `alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-xrengine20230313
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-2.0.0/setup.py` & `alibabacloud_xrengine20230313-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_xrengine20230313.
 
-Created on 02/08/2023
+Created on 03/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_xrengine20230313"
 NAME = "alibabacloud_xrengine20230313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud xrEngine (20230313) SDK Library for Python"
```

