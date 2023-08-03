# Comparing `tmp/alibabacloud_bailian20230601-1.1.1.tar.gz` & `tmp/alibabacloud_bailian20230601-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bailian20230601-1.1.1.tar", last modified: Fri Jul 21 03:19:08 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bailian20230601-1.1.2.tar", last modified: Thu Aug  3 03:23:59 2023, max compression
```

## Comparing `alibabacloud_bailian20230601-1.1.1.tar` & `alibabacloud_bailian20230601-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:19:08.000000 alibabacloud_bailian20230601-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      138 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-21 03:19:08.000000 alibabacloud_bailian20230601-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:19:08.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33175 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601/client.py
--rw-r--r--   0 root         (0) root         (0)    50155 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:19:08.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 03:19:08.000000 alibabacloud_bailian20230601-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2631 2023-07-21 03:19:07.000000 alibabacloud_bailian20230601-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      198 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37089 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601/client.py
+-rw-r--r--   0 root         (0) root         (0)    58692 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-08-03 03:23:59.000000 alibabacloud_bailian20230601-1.1.2/setup.py
```

### Comparing `alibabacloud_bailian20230601-1.1.1/LICENSE` & `alibabacloud_bailian20230601-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bailian20230601-1.1.1/PKG-INFO` & `alibabacloud_bailian20230601-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bailian20230601
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud bailian (20230601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bailian20230601-1.1.1/README-CN.md` & `alibabacloud_bailian20230601-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bailian20230601-1.1.1/README.md` & `alibabacloud_bailian20230601-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601/client.py` & `alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,16 @@
             body['BaseModel'] = request.base_model
         if not UtilClient.is_unset(request.hyper_parameters_shrink):
             body['HyperParameters'] = request.hyper_parameters_shrink
         if not UtilClient.is_unset(request.model_name):
             body['ModelName'] = request.model_name
         if not UtilClient.is_unset(request.training_files_shrink):
             body['TrainingFiles'] = request.training_files_shrink
+        if not UtilClient.is_unset(request.training_type):
+            body['TrainingType'] = request.training_type
         if not UtilClient.is_unset(request.validation_files_shrink):
             body['ValidationFiles'] = request.validation_files_shrink
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -189,14 +191,16 @@
             body['BaseModel'] = request.base_model
         if not UtilClient.is_unset(request.hyper_parameters_shrink):
             body['HyperParameters'] = request.hyper_parameters_shrink
         if not UtilClient.is_unset(request.model_name):
             body['ModelName'] = request.model_name
         if not UtilClient.is_unset(request.training_files_shrink):
             body['TrainingFiles'] = request.training_files_shrink
+        if not UtilClient.is_unset(request.training_type):
+            body['TrainingType'] = request.training_type
         if not UtilClient.is_unset(request.validation_files_shrink):
             body['ValidationFiles'] = request.validation_files_shrink
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -303,14 +307,100 @@
     async def create_service_async(
         self,
         request: bailian_20230601_models.CreateServiceRequest,
     ) -> bailian_20230601_models.CreateServiceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_service_with_options_async(request, runtime)
 
+    def create_text_embeddings_with_options(
+        self,
+        tmp_req: bailian_20230601_models.CreateTextEmbeddingsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> bailian_20230601_models.CreateTextEmbeddingsResponse:
+        UtilClient.validate_model(tmp_req)
+        request = bailian_20230601_models.CreateTextEmbeddingsShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.input):
+            request.input_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input, 'Input', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.agent_key):
+            query['AgentKey'] = request.agent_key
+        if not UtilClient.is_unset(request.input_shrink):
+            query['Input'] = request.input_shrink
+        if not UtilClient.is_unset(request.text_type):
+            query['TextType'] = request.text_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateTextEmbeddings',
+            version='2023-06-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            bailian_20230601_models.CreateTextEmbeddingsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_text_embeddings_with_options_async(
+        self,
+        tmp_req: bailian_20230601_models.CreateTextEmbeddingsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> bailian_20230601_models.CreateTextEmbeddingsResponse:
+        UtilClient.validate_model(tmp_req)
+        request = bailian_20230601_models.CreateTextEmbeddingsShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.input):
+            request.input_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input, 'Input', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.agent_key):
+            query['AgentKey'] = request.agent_key
+        if not UtilClient.is_unset(request.input_shrink):
+            query['Input'] = request.input_shrink
+        if not UtilClient.is_unset(request.text_type):
+            query['TextType'] = request.text_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateTextEmbeddings',
+            version='2023-06-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            bailian_20230601_models.CreateTextEmbeddingsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_text_embeddings(
+        self,
+        request: bailian_20230601_models.CreateTextEmbeddingsRequest,
+    ) -> bailian_20230601_models.CreateTextEmbeddingsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_text_embeddings_with_options(request, runtime)
+
+    async def create_text_embeddings_async(
+        self,
+        request: bailian_20230601_models.CreateTextEmbeddingsRequest,
+    ) -> bailian_20230601_models.CreateTextEmbeddingsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_text_embeddings_with_options_async(request, runtime)
+
     def create_token_with_options(
         self,
         request: bailian_20230601_models.CreateTokenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> bailian_20230601_models.CreateTokenResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601/models.py` & `alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,21 +163,23 @@
     def __init__(
         self,
         agent_key: str = None,
         base_model: str = None,
         hyper_parameters: CreateFineTuneJobRequestHyperParameters = None,
         model_name: str = None,
         training_files: List[str] = None,
+        training_type: str = None,
         validation_files: List[str] = None,
     ):
         self.agent_key = agent_key
         self.base_model = base_model
         self.hyper_parameters = hyper_parameters
         self.model_name = model_name
         self.training_files = training_files
+        self.training_type = training_type
         self.validation_files = validation_files
 
     def validate(self):
         if self.hyper_parameters:
             self.hyper_parameters.validate()
 
     def to_map(self):
@@ -192,14 +194,16 @@
             result['BaseModel'] = self.base_model
         if self.hyper_parameters is not None:
             result['HyperParameters'] = self.hyper_parameters.to_map()
         if self.model_name is not None:
             result['ModelName'] = self.model_name
         if self.training_files is not None:
             result['TrainingFiles'] = self.training_files
+        if self.training_type is not None:
+            result['TrainingType'] = self.training_type
         if self.validation_files is not None:
             result['ValidationFiles'] = self.validation_files
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AgentKey') is not None:
@@ -209,34 +213,38 @@
         if m.get('HyperParameters') is not None:
             temp_model = CreateFineTuneJobRequestHyperParameters()
             self.hyper_parameters = temp_model.from_map(m['HyperParameters'])
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
         if m.get('TrainingFiles') is not None:
             self.training_files = m.get('TrainingFiles')
+        if m.get('TrainingType') is not None:
+            self.training_type = m.get('TrainingType')
         if m.get('ValidationFiles') is not None:
             self.validation_files = m.get('ValidationFiles')
         return self
 
 
 class CreateFineTuneJobShrinkRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         base_model: str = None,
         hyper_parameters_shrink: str = None,
         model_name: str = None,
         training_files_shrink: str = None,
+        training_type: str = None,
         validation_files_shrink: str = None,
     ):
         self.agent_key = agent_key
         self.base_model = base_model
         self.hyper_parameters_shrink = hyper_parameters_shrink
         self.model_name = model_name
         self.training_files_shrink = training_files_shrink
+        self.training_type = training_type
         self.validation_files_shrink = validation_files_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -250,14 +258,16 @@
             result['BaseModel'] = self.base_model
         if self.hyper_parameters_shrink is not None:
             result['HyperParameters'] = self.hyper_parameters_shrink
         if self.model_name is not None:
             result['ModelName'] = self.model_name
         if self.training_files_shrink is not None:
             result['TrainingFiles'] = self.training_files_shrink
+        if self.training_type is not None:
+            result['TrainingType'] = self.training_type
         if self.validation_files_shrink is not None:
             result['ValidationFiles'] = self.validation_files_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AgentKey') is not None:
@@ -266,14 +276,16 @@
             self.base_model = m.get('BaseModel')
         if m.get('HyperParameters') is not None:
             self.hyper_parameters_shrink = m.get('HyperParameters')
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
         if m.get('TrainingFiles') is not None:
             self.training_files_shrink = m.get('TrainingFiles')
+        if m.get('TrainingType') is not None:
+            self.training_type = m.get('TrainingType')
         if m.get('ValidationFiles') is not None:
             self.validation_files_shrink = m.get('ValidationFiles')
         return self
 
 
 class CreateFineTuneJobResponseBody(TeaModel):
     def __init__(
@@ -464,14 +476,263 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTextEmbeddingsRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        input: List[str] = None,
+        text_type: str = None,
+    ):
+        self.agent_key = agent_key
+        self.input = input
+        self.text_type = text_type
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
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.input is not None:
+            result['Input'] = self.input
+        if self.text_type is not None:
+            result['TextType'] = self.text_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('Input') is not None:
+            self.input = m.get('Input')
+        if m.get('TextType') is not None:
+            self.text_type = m.get('TextType')
+        return self
+
+
+class CreateTextEmbeddingsShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        input_shrink: str = None,
+        text_type: str = None,
+    ):
+        self.agent_key = agent_key
+        self.input_shrink = input_shrink
+        self.text_type = text_type
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
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.input_shrink is not None:
+            result['Input'] = self.input_shrink
+        if self.text_type is not None:
+            result['TextType'] = self.text_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('Input') is not None:
+            self.input_shrink = m.get('Input')
+        if m.get('TextType') is not None:
+            self.text_type = m.get('TextType')
+        return self
+
+
+class CreateTextEmbeddingsResponseBodyDataEmbeddings(TeaModel):
+    def __init__(
+        self,
+        embedding: List[float] = None,
+        text_index: int = None,
+    ):
+        self.embedding = embedding
+        self.text_index = text_index
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
+        if self.embedding is not None:
+            result['Embedding'] = self.embedding
+        if self.text_index is not None:
+            result['TextIndex'] = self.text_index
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Embedding') is not None:
+            self.embedding = m.get('Embedding')
+        if m.get('TextIndex') is not None:
+            self.text_index = m.get('TextIndex')
+        return self
+
+
+class CreateTextEmbeddingsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        embeddings: List[CreateTextEmbeddingsResponseBodyDataEmbeddings] = None,
+    ):
+        self.embeddings = embeddings
+
+    def validate(self):
+        if self.embeddings:
+            for k in self.embeddings:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Embeddings'] = []
+        if self.embeddings is not None:
+            for k in self.embeddings:
+                result['Embeddings'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.embeddings = []
+        if m.get('Embeddings') is not None:
+            for k in m.get('Embeddings'):
+                temp_model = CreateTextEmbeddingsResponseBodyDataEmbeddings()
+                self.embeddings.append(temp_model.from_map(k))
+        return self
+
+
+class CreateTextEmbeddingsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: CreateTextEmbeddingsResponseBodyData = None,
+        http_status_code: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
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
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
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
+            temp_model = CreateTextEmbeddingsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateTextEmbeddingsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateTextEmbeddingsResponseBody = None,
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
+            temp_model = CreateTextEmbeddingsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateTokenRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
         self.agent_key = agent_key
 
@@ -938,25 +1199,27 @@
         hyper_parameters: DescribeFineTuneJobResponseBodyHyperParameters = None,
         job_id: str = None,
         message: str = None,
         model_name: str = None,
         request_id: str = None,
         status: str = None,
         training_files: List[str] = None,
+        training_type: str = None,
         validation_files: List[str] = None,
     ):
         self.base_model = base_model
         self.fine_tuned_model = fine_tuned_model
         self.hyper_parameters = hyper_parameters
         self.job_id = job_id
         self.message = message
         self.model_name = model_name
         self.request_id = request_id
         self.status = status
         self.training_files = training_files
+        self.training_type = training_type
         self.validation_files = validation_files
 
     def validate(self):
         if self.hyper_parameters:
             self.hyper_parameters.validate()
 
     def to_map(self):
@@ -979,14 +1242,16 @@
             result['ModelName'] = self.model_name
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.status is not None:
             result['Status'] = self.status
         if self.training_files is not None:
             result['TrainingFiles'] = self.training_files
+        if self.training_type is not None:
+            result['TrainingType'] = self.training_type
         if self.validation_files is not None:
             result['ValidationFiles'] = self.validation_files
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BaseModel') is not None:
@@ -1004,14 +1269,16 @@
             self.model_name = m.get('ModelName')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TrainingFiles') is not None:
             self.training_files = m.get('TrainingFiles')
+        if m.get('TrainingType') is not None:
+            self.training_type = m.get('TrainingType')
         if m.get('ValidationFiles') is not None:
             self.validation_files = m.get('ValidationFiles')
         return self
 
 
 class DescribeFineTuneJobResponse(TeaModel):
     def __init__(
@@ -1270,24 +1537,26 @@
         fine_tuned_model: str = None,
         hyper_parameters: ListFineTuneJobsResponseBodyJobsHyperParameters = None,
         job_id: str = None,
         message: str = None,
         model_name: str = None,
         status: str = None,
         training_files: List[str] = None,
+        training_type: str = None,
         validation_files: List[str] = None,
     ):
         self.base_model = base_model
         self.fine_tuned_model = fine_tuned_model
         self.hyper_parameters = hyper_parameters
         self.job_id = job_id
         self.message = message
         self.model_name = model_name
         self.status = status
         self.training_files = training_files
+        self.training_type = training_type
         self.validation_files = validation_files
 
     def validate(self):
         if self.hyper_parameters:
             self.hyper_parameters.validate()
 
     def to_map(self):
@@ -1308,14 +1577,16 @@
             result['Message'] = self.message
         if self.model_name is not None:
             result['ModelName'] = self.model_name
         if self.status is not None:
             result['Status'] = self.status
         if self.training_files is not None:
             result['TrainingFiles'] = self.training_files
+        if self.training_type is not None:
+            result['TrainingType'] = self.training_type
         if self.validation_files is not None:
             result['ValidationFiles'] = self.validation_files
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BaseModel') is not None:
@@ -1331,14 +1602,16 @@
             self.message = m.get('Message')
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TrainingFiles') is not None:
             self.training_files = m.get('TrainingFiles')
+        if m.get('TrainingType') is not None:
+            self.training_type = m.get('TrainingType')
         if m.get('ValidationFiles') is not None:
             self.validation_files = m.get('ValidationFiles')
         return self
 
 
 class ListFineTuneJobsResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_bailian20230601-1.1.1/alibabacloud_bailian20230601.egg-info/PKG-INFO` & `alibabacloud_bailian20230601-1.1.2/alibabacloud_bailian20230601.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bailian20230601
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud bailian (20230601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bailian20230601-1.1.1/setup.py` & `alibabacloud_bailian20230601-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bailian20230601.
 
-Created on 21/07/2023
+Created on 03/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bailian20230601"
 NAME = "alibabacloud_bailian20230601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud bailian (20230601) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.10, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

