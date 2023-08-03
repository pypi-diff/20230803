# Comparing `tmp/hypergo-0.1.7.tar.gz` & `tmp/hypergo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.7.tar", last modified: Wed Aug  2 17:55:03 2023, max compression
+gzip compressed data, was "hypergo-0.1.8.tar", last modified: Thu Aug  3 02:44:56 2023, max compression
```

## Comparing `hypergo-0.1.7.tar` & `hypergo-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:03.822800 hypergo-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:03.814800 hypergo-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:03.818800 hypergo-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 17:54:51.000000 hypergo-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-02 17:54:51.000000 hypergo-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 17:54:51.000000 hypergo-0.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 17:54:51.000000 hypergo-0.1.7/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:54:51.000000 hypergo-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-02 17:55:03.822800 hypergo-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 17:54:51.000000 hypergo-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-02 17:54:51.000000 hypergo-0.1.7/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 17:54:51.000000 hypergo-0.1.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:03.822800 hypergo-0.1.7/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/hypergo_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/hypergo_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/hypergo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/stdio_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-02 17:54:51.000000 hypergo-0.1.7/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:03.822800 hypergo-0.1.7/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-02 17:55:03.000000 hypergo-0.1.7/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-02 17:55:03.000000 hypergo-0.1.7/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:55:03.000000 hypergo-0.1.7/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 17:55:03.000000 hypergo-0.1.7/hypergo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-02 17:55:03.000000 hypergo-0.1.7/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 17:55:03.000000 hypergo-0.1.7/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-02 17:54:51.000000 hypergo-0.1.7/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 17:54:51.000000 hypergo-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 17:55:03.826799 hypergo-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 17:54:51.000000 hypergo-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:03.822800 hypergo-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-02 17:54:51.000000 hypergo-0.1.7/tests/test_utility_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.534507 hypergo-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.514506 hypergo-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.522507 hypergo-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 02:44:43.000000 hypergo-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-03 02:44:43.000000 hypergo-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 02:44:43.000000 hypergo-0.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 02:44:43.000000 hypergo-0.1.8/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:43.000000 hypergo-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 02:44:56.534507 hypergo-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-03 02:44:43.000000 hypergo-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-03 02:44:43.000000 hypergo-0.1.8/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 02:44:43.000000 hypergo-0.1.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.530507 hypergo-0.1.8/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.530507 hypergo-0.1.8/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-03 02:44:43.000000 hypergo-0.1.8/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 02:44:43.000000 hypergo-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 02:44:56.534507 hypergo-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-03 02:44:43.000000 hypergo-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.534507 hypergo-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.1.7/.github/workflows/python-publish.yml` & `hypergo-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/.gitignore` & `hypergo-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/BACKLOG.md` & `hypergo-0.1.8/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/RELEASE_NOTES.md` & `hypergo-0.1.8/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.8/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/config.py` & `hypergo-0.1.8/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/executor.py` & `hypergo-0.1.8/hypergo/executor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/graph.py` & `hypergo-0.1.8/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/hypergo_cli.py` & `hypergo-0.1.8/hypergo/hypergo_cli.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/hypergo_click.py` & `hypergo-0.1.8/hypergo/hypergo_click.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/hypergo_cmd.py` & `hypergo-0.1.8/hypergo/hypergo_cmd.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/local_storage.py` & `hypergo-0.1.8/hypergo/local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/message.py` & `hypergo-0.1.8/hypergo/message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/service_bus_connection.py` & `hypergo-0.1.8/hypergo/service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/stdio_connection.py` & `hypergo-0.1.8/hypergo/stdio_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/storage.py` & `hypergo-0.1.8/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/transform.py` & `hypergo-0.1.8/hypergo/transform.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo/utility.py` & `hypergo-0.1.8/hypergo/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         if not serialized:
             return serialized
         try:
             utfencoded: bytes = serialized.encode("utf-8")
             decoded: bytes = base64.b64decode(utfencoded)
             deserialized: Any = dill.loads(decoded)
             return deserialized
-        except (binascii.Error, dill.UnpicklingError, AttributeError):
+        except (binascii.Error, dill.UnpicklingError, AttributeError, ValueError):
             return serialized
 
     @staticmethod
     def compress(data: Any, key: Optional[str] = None) -> Any:
         root_data = {"root": data}
         root_key = f"root.{key}" if key else "root"
         Utility.deep_set(
```

### Comparing `hypergo-0.1.7/hypergo/version.py` & `hypergo-0.1.8/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.8/hypergo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/lint.sh` & `hypergo-0.1.8/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/setup.py` & `hypergo-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test.json` & `hypergo-0.1.8/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test.yaml` & `hypergo-0.1.8/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_dynamic_input_bindings.py` & `hypergo-0.1.8/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_dynamic_routing_key.py` & `hypergo-0.1.8/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_local_storage.py` & `hypergo-0.1.8/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_message.py` & `hypergo-0.1.8/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_storage.py` & `hypergo-0.1.8/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_utility.py` & `hypergo-0.1.8/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.7/tests/test_utility_serialization.py` & `hypergo-0.1.8/tests/test_utility_serialization.py`

 * *Files identical despite different names*

