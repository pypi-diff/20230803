# Comparing `tmp/zrouter-0.5.7.tar.gz` & `tmp/zrouter-0.5.8.tar.gz`

## Comparing `zrouter-0.5.7.tar` & `zrouter-0.5.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/restful.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/router.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.7/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.7/LICENSE
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.7/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.8/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.8/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.8/PKG-INFO
```

### Comparing `zrouter-0.5.7/src/zrouter/__init__.py` & `zrouter-0.5.8/src/zrouter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from zrouter.router import Router
-from flask import request 
+from flask import Flask, request 
 from flask.json import JSONEncoder
 import decimal
 
 
 class JsonEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, decimal.Decimal):
```

### Comparing `zrouter-0.5.7/src/zrouter/restful.py` & `zrouter-0.5.8/src/zrouter/restful.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.7/src/zrouter/router.py` & `zrouter-0.5.8/src/zrouter/router.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.7/src/zrouter/utils/json.py` & `zrouter-0.5.8/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.7/LICENSE` & `zrouter-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.7/README.md` & `zrouter-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.7/pyproject.toml` & `zrouter-0.5.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.7"
+version = "0.5.8"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.5.7/PKG-INFO` & `zrouter-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.5.7
+Version: 0.5.8
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

