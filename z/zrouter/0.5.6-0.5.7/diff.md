# Comparing `tmp/zrouter-0.5.6.tar.gz` & `tmp/zrouter-0.5.7.tar.gz`

## Comparing `zrouter-0.5.6.tar` & `zrouter-0.5.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/restful.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/router.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.6/LICENSE
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.6/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.7/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.7/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.7/PKG-INFO
```

### Comparing `zrouter-0.5.6/src/zrouter/restful.py` & `zrouter-0.5.7/src/zrouter/restful.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from typing import Optional
 
 
-def R(mapper_class):
-    def get(id: Optional[int] = None, page_num: Optional[int] = None, page_size: Optional[int] = None, **kwargs):
+class R:
+    @classmethod
+    def get(cls, id: Optional[int] = None, page_num: Optional[int] = None, page_size: Optional[int] = None, **kwargs):
         if id:
-            return mapper_class.get_json(id)
+            return cls.get_json(id)
         else:
-            return mapper_class.get_jsons(page_num=page_num, page_size=page_size)
+            return cls.get_jsons(page_num=page_num, page_size=page_size)
 
-    def post(data: dict, id: Optional[int] = None):
-        if id:
-            mapper_class.save(id, data)
-        else:
-            mapper_class.add(data)
+    @classmethod
+    def post(cls, data: dict):
+        cls.add(data)
 
-    def delete(id: int):
-        mapper_class.delete(id=id)
+    @classmethod
+    def put(cls, id: int, data: dict):
+        cls.save(id, data)
 
-    method_dict = {
-        'get': get,
-        'post': post,
-        'delete': delete
-    }
+    @classmethod
+    def delete(cls, id: int):
+        cls.delete(id=id)
 
-    return type('Resource', (object,), method_dict)
-    
+
```

### Comparing `zrouter-0.5.6/src/zrouter/router.py` & `zrouter-0.5.7/src/zrouter/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from zrouter.exceptions import MessagePrompt
 from zrouter.utils.json import to_lowcase, iter_lowcase, iter_camel
 from flask import Blueprint, request
 from jsonschema.exceptions import ValidationError
-from functools import wraps
+import functools
 import random
 
 
 class ParamMixin:
     @staticmethod
     def get_params():
         if request.method in ['GET', 'DELETE']:
@@ -48,15 +48,15 @@
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
         return wrapper
     
     def wrap_view_func(self, func, direct=False, open=False):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             params = self.clean_params(self.get_params())
             if not self.verify_user() and not open:
                 return {'code': 401, 'msg': '用户无权限'}
             try:
                 data = self.decorator(func)(**params)
             except MessagePrompt as e:
@@ -76,15 +76,15 @@
         return wrapper
 
     def add_resource(self, rule, resource_class):
         http_methods = ['get', 'post', 'put', 'delete']
 
         for method_name in http_methods:
             if method_name in dir(resource_class):
-                method =getattr(resource_class, method_name)
+                method = functools.partial(getattr(resource_class, method_name))
                 open = getattr(method, 'open', False)
                 direct = getattr(method, 'direct', False)
                 endpoint = str(random.randint(10000000, 99999999))
                 self.add_url_rule(rule, endpoint, self.wrap_view_func(method,
                     open=open, direct=direct), methods=[method_name.upper()])
 
     def add_resources(self, resource_map):
```

### Comparing `zrouter-0.5.6/src/zrouter/utils/json.py` & `zrouter-0.5.7/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.6/LICENSE` & `zrouter-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.6/README.md` & `zrouter-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.6/pyproject.toml` & `zrouter-0.5.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.5.6/PKG-INFO` & `zrouter-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.5.6
+Version: 0.5.7
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

