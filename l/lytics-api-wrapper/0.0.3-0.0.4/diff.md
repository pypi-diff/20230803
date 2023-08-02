# Comparing `tmp/lytics_api_wrapper-0.0.3.tar.gz` & `tmp/lytics_api_wrapper-0.0.4.tar.gz`

## Comparing `lytics_api_wrapper-0.0.3.tar` & `lytics_api_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.3/src/lytics_api_wrapper/__init__.py
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.3/src/lytics_api_wrapper/wrapper.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.3/LICENSE
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.3/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/src/lytics_api_wrapper/__init__.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/src/lytics_api_wrapper/wrapper.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/LICENSE
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 lytics_api_wrapper-0.0.4/PKG-INFO
```

### Comparing `lytics_api_wrapper-0.0.3/src/lytics_api_wrapper/wrapper.py` & `lytics_api_wrapper-0.0.4/src/lytics_api_wrapper/wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import requests
 import json
 from datetime import datetime
 
-
-def lyGenerator(aid, adminkey, env="prod"):
-    API = "https://stagingapik8s.lytics.io/"
-    if env == "prod":
-        API = "https://api.lytics.io/"
-    if env == "local":
-        API = "localhost:5353/"
-
-    r = requests.get(API+"api/account/{}".format(aid),
-                     params={"key": adminkey})
-
-    if r.status_code == 200:
-        data = json.loads(r.text)
-        return ly(data["data"]["apikey"])
-    else:
-        print("failed to create ly object: {}".format(r.status_code))
-
-
 class ly:
-    def __init__(self, key, env="prod"):
+    def __init__(self, key, aid, env="prod"):
         self.key = key
         if env == "prod":
             self.API = "https://api.lytics.io/"
         elif env == "local":
             self.API = "http://localhost:5353/"
         else:
             self.API = "https://stagingapik8s.lytics.io/"
 
+        r = requests.get(self.API+"api/account/{}".format(aid), params={"key": key})
+
+        if r.status_code != 200:
+            raise Exception(
+                "failed to create ly object with status code: {}".format(r.text))
+
+        data = json.loads(r.text)
+        self.aid = data["data"]["aid"]
+        self.name = data["data"]["name"]
+        self.account_id = data["data"]["id"]
+
+    def add_params(self, p):
+        p['key'] = self.key
+        p['account_id'] = self.account_id
+        return p
+
+    def __str__(self):
+        return "{} (AID {})".format(self.name, self.aid)
+
     def get(self, path, params={}, headers={}):
-        params['key'] = self.key
-        return requests.get(self.API+path, params=params, headers=headers)
+        
+        return requests.get(self.API+path, params=self.add_params(params), headers=headers)
 
     def post(self, path, stuff={}, params={}, headers={}):
         params['key'] = self.key
-        return requests.post(self.API+path, params=params, data=stuff, headers=headers)
+        return requests.post(self.API+path, params=self.add_params(params), data=stuff, headers=headers)
 
     def delete(self, path, params={}, headers={}):
         params['key'] = self.key
-        return requests.delete(self.API+path, params=params, headers=headers)
+        return requests.delete(self.API+path, params=self.add_params(params), headers=headers)
 
     def put(self, path, stuff={}, params={}, headers={}):
         params['key'] = self.key
-        return requests.put(self.API+path, params=params, data=stuff, headers=headers)
+        return requests.put(self.API+path, params=self.add_params(params), headers=headers)
 
     def scan(self, filter, limit=1000000000, gen=0):
         docs = []
         self.scan_helper(filter, "", docs, 0, limit, gen)
         return docs
 
     def size(self, filter):
@@ -96,15 +97,14 @@
                 "segment_scanner_version": "v2",
             }
         }
 
         r = self.post("api/work", json.dumps(config))
         print(r.text)
 
-    # TODO: add collections
     def rescore_content(self, filter):
         now = datetime.utcnow().isoformat()[:-7]+'Z'
 
         config = {
             "workflow_id": "23be8d80749b106513e83547e2c8bff1",
             "verbose_logging": True,
             "config": {
@@ -117,26 +117,28 @@
                 "rescore": True,
             }
         }
         r = self.post("api/work", json.dumps(config))
         j = json.loads(r.text)
         print(j['data']['id'])
 
-    def enrich_content(self, filter):
+    def enrich_content(self, filter, enrichers=["meta", "google_nlp", "diffbot_meta"]):
         now = datetime.utcnow().isoformat()[:-7]+'Z'
 
         config = {
             "workflow_id": "23be8d80749b106513e83547e2c8bff1",
             "verbose_logging": True,
             "config": {
                 "collection_id": filter,
                 "skip_sitemaps": True,
-                "enrich_epoch": {
-                    "meta": now,
-                    "google_nlp": now,
-                    "diffbot_meta": now
-                }
+                "enrich_epoch": {}
             }
         }
-        r = self.post("api/work", json.dumps(config))
-        j = json.loads(r.text)
-        print(j['data']['id'])
+
+        for e in enrichers:
+            config["config"]["enrich_epoch"][e] = now
+
+        print(config)
+
+        #r = self.post("api/work", json.dumps(config))
+        #j = json.loads(r.text)
+        # print(j['data']['id'])
```

### Comparing `lytics_api_wrapper-0.0.3/LICENSE` & `lytics_api_wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lytics_api_wrapper-0.0.3/pyproject.toml` & `lytics_api_wrapper-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lytics_api_wrapper"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Trace Andreason", email="tandreason@gmail.com" },
 ]
 description = "A python class wrapper around the Lytics API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `lytics_api_wrapper-0.0.3/PKG-INFO` & `lytics_api_wrapper-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytics_api_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python class wrapper around the Lytics API
 Project-URL: Homepage, https://github.com/tandreason/lytics-api-wrapper
 Project-URL: Bug Tracker, https://github.com/tandreason/lytics-api-wrapper/issues
 Author-email: Trace Andreason <tandreason@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Trace Andreason
@@ -22,14 +22,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Lytics API Wrapper
```

