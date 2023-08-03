# Comparing `tmp/neuralpit-2.1.1.tar.gz` & `tmp/neuralpit-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-2.1.1.tar", last modified: Mon Jul 31 04:10:16 2023, max compression
+gzip compressed data, was "neuralpit-2.1.2.tar", last modified: Thu Aug  3 05:21:21 2023, max compression
```

## Comparing `neuralpit-2.1.1.tar` & `neuralpit-2.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.949526 neuralpit-2.1.1/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 04:09:48.000000 neuralpit-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-31 04:10:16.949526 neuralpit-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-31 04:09:48.000000 neuralpit-2.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-31 04:09:48.000000 neuralpit-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 04:10:16.949526 neuralpit-2.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.945526 neuralpit-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.949526 neuralpit-2.1.1/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      620 2023-07-31 04:09:48.000000 neuralpit-2.1.1/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.949526 neuralpit-2.1.1/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 04:09:48.000000 neuralpit-2.1.1/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4594 2023-07-31 04:09:48.000000 neuralpit-2.1.1/src/neuralpit/services/conversation.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-31 04:09:48.000000 neuralpit-2.1.1/src/neuralpit/services/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.949526 neuralpit-2.1.1/src/neuralpit/utils/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-31 04:09:48.000000 neuralpit-2.1.1/src/neuralpit/utils/streamer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.949526 neuralpit-2.1.1/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-31 04:10:16.000000 neuralpit-2.1.1/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 04:10:16.000000 neuralpit-2.1.1/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:10:16.000000 neuralpit-2.1.1/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-31 04:10:16.000000 neuralpit-2.1.1/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-31 04:10:16.000000 neuralpit-2.1.1/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:10:16.949526 neuralpit-2.1.1/test/
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-31 04:09:48.000000 neuralpit-2.1.1/test/testCreateConversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 05:20:52.000000 neuralpit-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-08-03 05:21:20.993473 neuralpit-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-03 05:20:52.000000 neuralpit-2.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-08-03 05:20:52.000000 neuralpit-2.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 05:21:20.993473 neuralpit-2.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/services/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/services/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit/utils/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/utils/streamer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-08-03 05:20:52.000000 neuralpit-2.1.2/test/testCreateConversation.py
```

### Comparing `neuralpit-2.1.1/PKG-INFO` & `neuralpit-2.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.1.1
+Version: 2.1.2
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `neuralpit-2.1.1/pyproject.toml` & `neuralpit-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "2.1.1"
+version = "2.1.2"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-2.1.1/src/neuralpit/__init__.py` & `neuralpit-2.1.2/src/neuralpit/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.1/src/neuralpit/services/conversation.py` & `neuralpit-2.1.2/src/neuralpit/services/conversation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,21 @@
     def addConversationDocumentFromS3(self, conversation_id, bucket, keys:List[str]):
         post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/s3_document')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         post_call = requests.post(post_url, headers = headers, json = [{'bucket': bucket, 'key': key} for key in keys])
         resp =  json.loads(post_call.content)
         return resp
     
+    def addConversationDocumentFromUrl(self, conversation_id, url:str, mode: str):
+        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/web_document')
+        headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
+        post_call = requests.post(post_url, headers = headers, json = {'url': url, 'mode': mode})
+        resp =  json.loads(post_call.content)
+        return resp
+    
     def deleteConversationDocument(self, conversation_id, document_id):
         delete_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/document/{document_id}')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         delete_call = requests.delete(delete_url, headers = headers)
         return True
     
     def listConversationDocument(self, conversation_id):
@@ -67,16 +74,16 @@
         delete_call = requests.delete(delete_url, headers = headers)
         return True
 
     
     def summarizeDocument(self, conversation_id, document_id, debug=False):
         get_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/document/{document_id}/summarize')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
-        post_call = requests.get(get_url, headers = headers, json = {'debug': debug})
-        return post_call.content
+        get_call = requests.get(get_url, headers = headers, json = {'debug': debug})
+        return get_call.content
     
     def queryConversation(self, conversation_id, question, debug=False, chunk_size=1024):
         post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/query')
         headers = {'x-api-key':self.api_key}
         with requests.post(post_url, headers = headers, json = {'question': question, 'debug': debug}, stream=True) as r:
             streamer = Streamer(r.iter_content(chunk_size))
             for item in streamer.iter_item():
```

### Comparing `neuralpit-2.1.1/src/neuralpit/services/conversion.py` & `neuralpit-2.1.2/src/neuralpit/services/conversion.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.1/src/neuralpit/utils/streamer.py` & `neuralpit-2.1.2/src/neuralpit/utils/streamer.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.1/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.1.2/src/neuralpit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.1.1
+Version: 2.1.2
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

