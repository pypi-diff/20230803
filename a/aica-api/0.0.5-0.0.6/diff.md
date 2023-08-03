# Comparing `tmp/aica_api-0.0.5.tar.gz` & `tmp/aica_api-0.0.6.tar.gz`

## Comparing `aica_api-0.0.5.tar` & `aica_api-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.5/src/aica_api/__init__.py
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 aica_api-0.0.5/src/aica_api/client.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.5/src/aica_api/ws_client.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.5/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.5/LICENSE
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.5/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.6/src/aica_api/__init__.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 aica_api-0.0.6/src/aica_api/client.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.6/src/aica_api/ws_client.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.6/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.6/PKG-INFO
```

### Comparing `aica_api-0.0.5/src/aica_api/client.py` & `aica_api-0.0.6/src/aica_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         """
         Initialize the currently set application.
 
         :param auto_load_hardware: If true, load hardware interfaces automatically when initializing the application.
         """
         return requests.post(self._endpoint('init_application'), json={"auto_load_hardware": auto_load_hardware})
 
+    def get_application_state(self) -> requests.Response:
+        """
+        Get the application state
+        """
+        return requests.get(self._endpoint('application/state'))
+
     def load_component(self, component_name: str) -> requests.Response:
         """
         Load a component in the current application. If the component is already loaded, or if the component is not
         described in the application, nothing happens.
 
         :param component_name: The name of the component to load
         """
```

### Comparing `aica_api-0.0.5/src/aica_api/ws_client.py` & `aica_api-0.0.6/src/aica_api/ws_client.py`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.5/LICENSE` & `aica_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.5/README.md` & `aica_api-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.5/pyproject.toml` & `aica_api-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aica_api"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Enrico Eberhard", email="enrico@aica.tech" },
 ]
 description = "A client utility for the AICA API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `aica_api-0.0.5/PKG-INFO` & `aica_api-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aica_api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A client utility for the AICA API
 Project-URL: Homepage, https://github.com/aica-technology/api
 Project-URL: Bug Tracker, https://github.com/aica-technology/api/issues
 Author-email: Enrico Eberhard <enrico@aica.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

