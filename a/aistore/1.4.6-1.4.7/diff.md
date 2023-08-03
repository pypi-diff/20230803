# Comparing `tmp/aistore-1.4.6.tar.gz` & `tmp/aistore-1.4.7.tar.gz`

## Comparing `aistore-1.4.6.tar` & `aistore-1.4.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/client.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/common_requirements
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/version.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/botocore_patch/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/botocore_patch/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/botocore_patch/botocore.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/botocore_patch/botocore_requirements
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/pytorch/README.md
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/pytorch/__init__.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/pytorch/aisio.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/pytorch/dataset.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/pytorch/dev_requirements
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/pytorch/utils.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/README.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/__init__.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/ais_source.py
--rw-r--r--   0        0        0    32585 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/bucket.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/client.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/cluster.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/const.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/dsort.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/dsort_types.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/errors.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/etl.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/etl_const.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/etl_templates.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/job.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/list_object_flag.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/namespace.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/object.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/object_attributes.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/object_iterator.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/object_reader.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/request_client.py
--rw-r--r--   0        0        0    11317 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/types.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/utils.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/multiobj/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/multiobj/object_collection.py
--rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/multiobj/object_group.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/multiobj/object_names.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/multiobj/object_range.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.4.6/aistore/sdk/multiobj/object_template.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.4.6/LICENSE
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.4.6/.gitignore
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.4.6/README.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aistore-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aistore-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/client.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/common_requirements
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/version.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/botocore_patch/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/botocore_patch/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/botocore_patch/botocore.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/botocore_patch/botocore_requirements
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/pytorch/README.md
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/pytorch/__init__.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/pytorch/aisio.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/pytorch/dataset.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/pytorch/dev_requirements
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/pytorch/utils.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/README.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/ais_source.py
+-rw-r--r--   0        0        0    32585 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/bucket.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/client.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/cluster.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/const.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/dsort.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/dsort_types.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/errors.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/etl.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/etl_const.py
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/etl_templates.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/job.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/list_object_flag.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/namespace.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/object.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/object_attributes.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/object_iterator.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/object_reader.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/request_client.py
+-rw-r--r--   0        0        0    11317 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/types.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/utils.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/multiobj/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/multiobj/object_collection.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/multiobj/object_group.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/multiobj/object_names.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/multiobj/object_range.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.4.7/aistore/sdk/multiobj/object_template.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.4.7/LICENSE
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.4.7/.gitignore
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.4.7/README.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aistore-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aistore-1.4.7/PKG-INFO
```

### Comparing `aistore-1.4.6/aistore/botocore_patch/README.md` & `aistore-1.4.7/aistore/botocore_patch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/botocore_patch/botocore.py` & `aistore-1.4.7/aistore/botocore_patch/botocore.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/pytorch/README.md` & `aistore-1.4.7/aistore/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/pytorch/aisio.py` & `aistore-1.4.7/aistore/pytorch/aisio.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/pytorch/dataset.py` & `aistore-1.4.7/aistore/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/pytorch/utils.py` & `aistore-1.4.7/aistore/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/README.md` & `aistore-1.4.7/aistore/sdk/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/ais_source.py` & `aistore-1.4.7/aistore/sdk/ais_source.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/bucket.py` & `aistore-1.4.7/aistore/sdk/bucket.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/client.py` & `aistore-1.4.7/aistore/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/cluster.py` & `aistore-1.4.7/aistore/sdk/cluster.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/const.py` & `aistore-1.4.7/aistore/sdk/const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/dsort.py` & `aistore-1.4.7/aistore/sdk/dsort.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/dsort_types.py` & `aistore-1.4.7/aistore/sdk/dsort_types.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/errors.py` & `aistore-1.4.7/aistore/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/etl.py` & `aistore-1.4.7/aistore/sdk/etl.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/etl_const.py` & `aistore-1.4.7/aistore/sdk/etl_const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/etl_templates.py` & `aistore-1.4.7/aistore/sdk/etl_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,27 +167,27 @@
 """
 
 # pylint: disable=unused-variable
 KERAS_TRANSFORMER = """
 apiVersion: v1
 kind: Pod
 metadata:
-  name: transformer-compress
+  name: transformer-keras
   annotations:
     communication_type: "{communication_type}://"
     wait_timeout: 5m
 spec:
   containers:
     - name: server
       image: aistorage/transformer_keras:latest
       imagePullPolicy: Always
       ports:
         - name: default
           containerPort: 80
-      command: ['/code/server.py', '--listen', '0.0.0.0', '--port', '80']
+      command: ["gunicorn", "--bind", "0.0.0.0:80", "app:app"]
       env:
         - name: FORMAT
           value: "{format}"
         - name: TRANSFORM
           value: '{transform}'
       readinessProbe:
         httpGet:
```

### Comparing `aistore-1.4.6/aistore/sdk/job.py` & `aistore-1.4.7/aistore/sdk/job.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/list_object_flag.py` & `aistore-1.4.7/aistore/sdk/list_object_flag.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/object.py` & `aistore-1.4.7/aistore/sdk/object.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/object_attributes.py` & `aistore-1.4.7/aistore/sdk/object_attributes.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/object_iterator.py` & `aistore-1.4.7/aistore/sdk/object_iterator.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/object_reader.py` & `aistore-1.4.7/aistore/sdk/object_reader.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/request_client.py` & `aistore-1.4.7/aistore/sdk/request_client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/types.py` & `aistore-1.4.7/aistore/sdk/types.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/utils.py` & `aistore-1.4.7/aistore/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/multiobj/object_collection.py` & `aistore-1.4.7/aistore/sdk/multiobj/object_collection.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/multiobj/object_group.py` & `aistore-1.4.7/aistore/sdk/multiobj/object_group.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/multiobj/object_names.py` & `aistore-1.4.7/aistore/sdk/multiobj/object_names.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/multiobj/object_range.py` & `aistore-1.4.7/aistore/sdk/multiobj/object_range.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/aistore/sdk/multiobj/object_template.py` & `aistore-1.4.7/aistore/sdk/multiobj/object_template.py`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/LICENSE` & `aistore-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/.gitignore` & `aistore-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/README.md` & `aistore-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/pyproject.toml` & `aistore-1.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aistore-1.4.6/PKG-INFO` & `aistore-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistore
-Version: 1.4.6
+Version: 1.4.7
 Summary: A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore.
 Project-URL: Homepage, https://aiatscale.org
 Project-URL: Download, https://github.com/NVIDIA/aistore/tags
 Project-URL: Documentation, https://aiatscale.org/docs/
 Project-URL: Release notes, https://github.com/NVIDIA/aistore/releases/
 Project-URL: Source, https://github.com/NVIDIA/aistore/
 Author-email: AIStore Team <ais@exchange.nvidia.com>
```

