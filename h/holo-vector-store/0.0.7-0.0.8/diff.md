# Comparing `tmp/holo_vector_store-0.0.7.tar.gz` & `tmp/holo_vector_store-0.0.8.tar.gz`

## Comparing `holo_vector_store-0.0.7.tar` & `holo_vector_store-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/Develop.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/env.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/src/holo_vector_store/__about__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/src/holo_vector_store/__init__.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/src/holo_vector_store/holo_vector_store.py
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/src/holo_vector_store/hologres_wrapper.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/tests/test_holo_vector_store.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/README.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 holo_vector_store-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/Develop.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/env.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/src/holo_vector_store/__about__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/src/holo_vector_store/__init__.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/src/holo_vector_store/holo_vector_store.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/src/holo_vector_store/hologres_wrapper.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/tests/test_holo_vector_store.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/README.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 holo_vector_store-0.0.8/PKG-INFO
```

### Comparing `holo_vector_store-0.0.7/src/holo_vector_store/holo_vector_store.py` & `holo_vector_store-0.0.8/src/holo_vector_store/holo_vector_store.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.7/src/holo_vector_store/hologres_wrapper.py` & `holo_vector_store-0.0.8/src/holo_vector_store/hologres_wrapper.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.7/tests/test_holo_vector_store.py` & `holo_vector_store-0.0.8/tests/test_holo_vector_store.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.7/LICENSE.txt` & `holo_vector_store-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.7/README.md` & `holo_vector_store-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,19 +81,19 @@
 ```
 
     [{'id': '2', 'vector': [2.0, 2.0, 2.0, 2.0, 2.0], 'metadata': {}}]
 
 2. 近邻查询：根据向量从数据库中取最近邻
 
 ```python
-holo.search([0.1, 0.1, 0.1, 0.1, 0.1], k=2)
+holo.search([0.1, 0.1, 0.1, 0.1, 0.1], k=2, select_columns=['t'])
 ```
 
-    [{'id': '0', 'metadata': {'a': 'hello'}, 'distance': 0.05},
-     {'id': '1', 'metadata': {'b': 123}, 'distance': 4.05}]
+    [{'id': '0', 'metadata': {'a': 'hello'}, 'distance': 0.05, 't': 'text 0'},
+    {'id': '1', 'metadata': {'b': 123}, 'distance': 4.05, 't': 'text 1'}]
 
 3. 融合查询：根据向量从数据库中取最近邻，并用其他列查询条件约束
 
 ```python
 holo.search([0.1, 0.1, 0.1, 0.1, 0.1], k=2, schema_data_filters={'t': 'text 1'})
 ```
```

### Comparing `holo_vector_store-0.0.7/pyproject.toml` & `holo_vector_store-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.7/PKG-INFO` & `holo_vector_store-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holo-vector-store
-Version: 0.0.7
+Version: 0.0.8
 Project-URL: Documentation, https://github.com/unknown/holo-vector-store#readme
 Project-URL: Issues, https://github.com/unknown/holo-vector-store/issues
 Project-URL: Source, https://github.com/unknown/holo-vector-store
 Author-email: Changgeng Zhao <zhaochanggeng.zcg@alibaba-inc.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -105,19 +105,19 @@
 ```
 
     [{'id': '2', 'vector': [2.0, 2.0, 2.0, 2.0, 2.0], 'metadata': {}}]
 
 2. 近邻查询：根据向量从数据库中取最近邻
 
 ```python
-holo.search([0.1, 0.1, 0.1, 0.1, 0.1], k=2)
+holo.search([0.1, 0.1, 0.1, 0.1, 0.1], k=2, select_columns=['t'])
 ```
 
-    [{'id': '0', 'metadata': {'a': 'hello'}, 'distance': 0.05},
-     {'id': '1', 'metadata': {'b': 123}, 'distance': 4.05}]
+    [{'id': '0', 'metadata': {'a': 'hello'}, 'distance': 0.05, 't': 'text 0'},
+    {'id': '1', 'metadata': {'b': 123}, 'distance': 4.05, 't': 'text 1'}]
 
 3. 融合查询：根据向量从数据库中取最近邻，并用其他列查询条件约束
 
 ```python
 holo.search([0.1, 0.1, 0.1, 0.1, 0.1], k=2, schema_data_filters={'t': 'text 1'})
 ```
```

