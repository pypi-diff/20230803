# Comparing `tmp/aica_api-0.0.4.tar.gz` & `tmp/aica_api-0.0.5.tar.gz`

## Comparing `aica_api-0.0.4.tar` & `aica_api-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.4/src/aica_api/__init__.py
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 aica_api-0.0.4/src/aica_api/client.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.4/src/aica_api/ws_client.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 aica_api-0.0.4/tests/test_api.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aica_api-0.0.4/tests/test_ws.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.4/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.4/LICENSE
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.4/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.5/src/aica_api/__init__.py
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 aica_api-0.0.5/src/aica_api/client.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.5/src/aica_api/ws_client.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.5/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.5/PKG-INFO
```

### Comparing `aica_api-0.0.4/src/aica_api/client.py` & `aica_api-0.0.5/src/aica_api/client.py`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.4/src/aica_api/ws_client.py` & `aica_api-0.0.5/src/aica_api/ws_client.py`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.4/LICENSE` & `aica_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.4/README.md` & `aica_api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.4/pyproject.toml` & `aica_api-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aica_api"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Enrico Eberhard", email="enrico@aica.tech" },
 ]
 description = "A client utility for the AICA API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `aica_api-0.0.4/PKG-INFO` & `aica_api-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aica_api
-Version: 0.0.4
+Version: 0.0.5
 Summary: A client utility for the AICA API
 Project-URL: Homepage, https://github.com/aica-technology/api
 Project-URL: Bug Tracker, https://github.com/aica-technology/api/issues
 Author-email: Enrico Eberhard <enrico@aica.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

