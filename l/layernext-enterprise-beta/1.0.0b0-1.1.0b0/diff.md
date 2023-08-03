# Comparing `tmp/layernext-enterprise-beta-1.0.0b0.tar.gz` & `tmp/layernext-enterprise-beta-1.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layernext-enterprise-beta-1.0.0b0.tar", last modified: Wed Jul 19 08:25:29 2023, max compression
+gzip compressed data, was "layernext-enterprise-beta-1.1.0b0.tar", last modified: Thu Aug  3 10:10:55 2023, max compression
```

## Comparing `layernext-enterprise-beta-1.0.0b0.tar` & `layernext-enterprise-beta-1.1.0b0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-19 08:25:29.416654 layernext-enterprise-beta-1.0.0b0/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     5667 2023-07-19 08:25:29.416479 layernext-enterprise-beta-1.0.0b0/PKG-INFO
--rw-r--r--   0 channawijerathna   (501) staff       (20)     5046 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/README.md
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-19 08:25:29.408376 layernext-enterprise-beta-1.0.0b0/layernext/
--rw-r--r--   0 channawijerathna   (501) staff       (20)    49823 2023-07-13 20:01:43.000000 layernext-enterprise-beta-1.0.0b0/layernext/__init__.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-19 08:25:29.413250 layernext-enterprise-beta-1.0.0b0/layernext/datalake/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     9330 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/__init__.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     8820 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/annotation.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      873 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/aws_s3_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1001 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/azure_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      889 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/constants.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)    36049 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/datalakeinterface.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)        0 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/dataset.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      519 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/file_trash.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)    10724 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/file_upload.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      915 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/gcs_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1516 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/ground_truth.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1286 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/keys.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     3514 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/label.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/logger.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1801 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/metadata.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      849 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/model_run.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1301 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/query.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      287 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/storage_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     2566 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/storage_interface.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     7504 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/datalake/storage_upload.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-19 08:25:29.414240 layernext-enterprise-beta-1.0.0b0/layernext/dataset/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     3111 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/dataset/__init__.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     4790 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/dataset/dataset.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     8999 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/dataset/datasetinterface.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/dataset/logger.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)    15591 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/dataset/sync.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-19 08:25:29.415320 layernext-enterprise-beta-1.0.0b0/layernext/studio/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     2561 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/studio/__init__.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/studio/logger.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     3435 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/studio/project.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     9624 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.0.0b0/layernext/studio/studiointerface.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-19 08:25:29.416229 layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     5667 2023-07-19 08:25:29.000000 layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/PKG-INFO
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1216 2023-07-19 08:25:29.000000 layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/SOURCES.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)        1 2023-07-19 08:25:29.000000 layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/dependency_links.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)       47 2023-07-19 08:25:29.000000 layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/requires.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)       10 2023-07-19 08:25:29.000000 layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/top_level.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)       38 2023-07-19 08:25:29.416711 layernext-enterprise-beta-1.0.0b0/setup.cfg
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1681 2023-07-19 08:25:07.000000 layernext-enterprise-beta-1.0.0b0/setup.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-03 10:10:55.786012 layernext-enterprise-beta-1.1.0b0/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1073 2023-07-29 17:43:27.000000 layernext-enterprise-beta-1.1.0b0/LICENSE
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     5689 2023-08-03 10:10:55.785739 layernext-enterprise-beta-1.1.0b0/PKG-INFO
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     5046 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/README.md
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-03 10:10:55.709528 layernext-enterprise-beta-1.1.0b0/layernext/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    50190 2023-08-03 10:07:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/__init__.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-03 10:10:55.781140 layernext-enterprise-beta-1.1.0b0/layernext/datalake/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     9330 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     8820 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/annotation.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      873 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/aws_s3_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1001 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/azure_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      889 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/constants.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    36049 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/datalakeinterface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)        0 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/dataset.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      519 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/file_trash.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    10724 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/file_upload.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      915 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/gcs_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1516 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/ground_truth.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1286 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/keys.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3514 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/label.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1801 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/metadata.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      849 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/model_run.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1301 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/query.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      287 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/storage_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     2566 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/storage_interface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     7504 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/datalake/storage_upload.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-03 10:10:55.782568 layernext-enterprise-beta-1.1.0b0/layernext/dataset/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3111 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/dataset/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     4790 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/dataset/dataset.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     8999 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/dataset/datasetinterface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/dataset/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    15591 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/dataset/sync.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-03 10:10:55.783426 layernext-enterprise-beta-1.1.0b0/layernext/studio/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     2561 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/studio/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/studio/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3435 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/studio/project.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     9624 2023-07-13 19:59:20.000000 layernext-enterprise-beta-1.1.0b0/layernext/studio/studiointerface.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-03 10:10:55.785366 layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     5689 2023-08-03 10:10:55.000000 layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/PKG-INFO
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1224 2023-08-03 10:10:55.000000 layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)        1 2023-08-03 10:10:55.000000 layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       47 2023-08-03 10:10:55.000000 layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/requires.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       10 2023-08-03 10:10:55.000000 layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/top_level.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       38 2023-08-03 10:10:55.786102 layernext-enterprise-beta-1.1.0b0/setup.cfg
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1681 2023-08-03 10:08:33.000000 layernext-enterprise-beta-1.1.0b0/setup.py
```

### Comparing `layernext-enterprise-beta-1.0.0b0/PKG-INFO` & `layernext-enterprise-beta-1.1.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: layernext-enterprise-beta
-Version: 1.0.0b0
+Version: 1.1.0b0
 Summary: LayerNext Python SDK
 Home-page: UNKNOWN
 Author: LayerNext
 Author-email: <support@layernext.ai>
 License: UNKNOWN
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # layernext-python-sdk
 
 LayerNext Python API Client
 Sync (upload/download) with LayerNext stacks via APIs from your local machine
```

### Comparing `layernext-enterprise-beta-1.0.0b0/README.md` & `layernext-enterprise-beta-1.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/__init__.py` & `layernext-enterprise-beta-1.1.0b0/layernext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 
 from layernext import datalake, dataset, studio
 from layernext.datalake.constants import MediaType, ObjectType
 
-__version__ = '1.0.0b0'
+__version__ = '1.1.0b0'
 
 
 class LayerNextClient:
     """
     Python SDK of LayerNext
     """
 
@@ -34,14 +34,26 @@
             self,
             collection_base_path: str,
             operation_unique_id: str,
             json_data_file_path: str,
             shape_type: str,
             is_normalized: bool,
             is_model_run: bool,
+            destination_project_id: str = None
+    ):
+        return upload_annotations_for_folde()
+
+    def upload_annotations_for_folder(
+            self,
+            collection_base_path: str,
+            operation_unique_id: str,
+            json_data_file_path: str,
+            shape_type: str,
+            is_normalized: bool,
+            is_model_run: bool,
             destination_project_id: str = None
     ):
         """
         Upload annotation data from a json file
         """
         # init datalake client
         _datalake_client = datalake.DatalakeClient(
```

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/__init__.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/annotation.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/annotation.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/aws_s3_client.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/aws_s3_client.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/azure_client.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/azure_client.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/constants.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/constants.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/datalakeinterface.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/datalakeinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/file_trash.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/file_trash.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/file_upload.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/gcs_client.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/gcs_client.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/ground_truth.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/ground_truth.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/keys.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/keys.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/label.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/label.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/metadata.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/metadata.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/model_run.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/model_run.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/query.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/storage_interface.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/storage_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/datalake/storage_upload.py` & `layernext-enterprise-beta-1.1.0b0/layernext/datalake/storage_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/dataset/__init__.py` & `layernext-enterprise-beta-1.1.0b0/layernext/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/dataset/dataset.py` & `layernext-enterprise-beta-1.1.0b0/layernext/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/dataset/datasetinterface.py` & `layernext-enterprise-beta-1.1.0b0/layernext/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/dataset/sync.py` & `layernext-enterprise-beta-1.1.0b0/layernext/dataset/sync.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/studio/__init__.py` & `layernext-enterprise-beta-1.1.0b0/layernext/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/studio/project.py` & `layernext-enterprise-beta-1.1.0b0/layernext/studio/project.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext/studio/studiointerface.py` & `layernext-enterprise-beta-1.1.0b0/layernext/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/PKG-INFO` & `layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: layernext-enterprise-beta
-Version: 1.0.0b0
+Version: 1.1.0b0
 Summary: LayerNext Python SDK
 Home-page: UNKNOWN
 Author: LayerNext
 Author-email: <support@layernext.ai>
 License: UNKNOWN
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # layernext-python-sdk
 
 LayerNext Python API Client
 Sync (upload/download) with LayerNext stacks via APIs from your local machine
```

### Comparing `layernext-enterprise-beta-1.0.0b0/layernext_enterprise_beta.egg-info/SOURCES.txt` & `layernext-enterprise-beta-1.1.0b0/layernext_enterprise_beta.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 layernext/__init__.py
 layernext/datalake/__init__.py
 layernext/datalake/annotation.py
 layernext/datalake/aws_s3_client.py
 layernext/datalake/azure_client.py
```

### Comparing `layernext-enterprise-beta-1.0.0b0/setup.py` & `layernext-enterprise-beta-1.1.0b0/setup.py`

 * *Files identical despite different names*

