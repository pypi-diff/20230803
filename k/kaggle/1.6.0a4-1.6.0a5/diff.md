# Comparing `tmp/kaggle-1.6.0a4.tar.gz` & `tmp/kaggle-1.6.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaggle-1.6.0a4.tar", last modified: Fri Jul  7 20:19:38 2023, max compression
+gzip compressed data, was "kaggle-1.6.0a5.tar", last modified: Wed Aug  2 23:56:20 2023, max compression
```

## Comparing `kaggle-1.6.0a4.tar` & `kaggle-1.6.0a5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/
--rw-r--r--   0 root         (0) root         (0)    11541 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35600 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.792875 kaggle-1.6.0a4/kaggle/
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.792875 kaggle-1.6.0a4/kaggle/api/
--rw-r--r--   0 root         (0) root         (0)      742 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   189890 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/api/kaggle_api.py
--rw-r--r--   0 root         (0) root         (0)   171676 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 root         (0) root         (0)    25458 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/api_client.py
--rw-r--r--   0 root         (0) root         (0)    75664 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/cli.py
--rw-r--r--   0 root         (0) root         (0)     9163 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/kaggle/models/
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/api_blob_type.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/collaborator.py
--rw-r--r--   0 root         (0) root         (0)     5166 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/create_inbox_file_request.py
--rw-r--r--   0 root         (0) root         (0)     7424 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/dataset_column.py
--rw-r--r--   0 root         (0) root         (0)    12558 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/models/dataset_new_request.py
--rw-r--r--   0 root         (0) root         (0)     9991 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)    10114 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     4342 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/error.py
--rw-r--r--   0 root         (0) root         (0)     7791 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 root         (0) root         (0)    20199 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/models/kernel_push_request.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/license.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_instance_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_instance_update_request.py
--rw-r--r--   0 root         (0) root         (0)    12103 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_new_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    10055 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_new_request.py
--rw-r--r--   0 root         (0) root         (0)     9096 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_update_request.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/result.py
--rw-r--r--   0 root         (0) root         (0)     7844 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/start_blob_upload_request.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/start_blob_upload_response.py
--rw-r--r--   0 root         (0) root         (0)     5439 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/upload_file.py
--rw-r--r--   0 root         (0) root         (0)    13927 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/kaggle/test/
--rw-r--r--   0 root         (0) root         (0)      596 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/test/test_authenticate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.792875 kaggle-1.6.0a4/kaggle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1236 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-07 20:19:38.804876 kaggle-1.6.0a4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1680 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 23:56:20.547502 kaggle-1.6.0a5/
+-rw-r--r--   0 root         (0) root         (0)    11541 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      609 2023-08-02 23:56:20.547502 kaggle-1.6.0a5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35600 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 23:56:20.539502 kaggle-1.6.0a5/kaggle/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 23:56:20.539502 kaggle-1.6.0a5/kaggle/api/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   189890 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/api/kaggle_api.py
+-rw-r--r--   0 root         (0) root         (0)   171688 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/api/kaggle_api_extended.py
+-rw-r--r--   0 root         (0) root         (0)    25458 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    75747 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9163 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 23:56:20.547502 kaggle-1.6.0a5/kaggle/models/
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/api_blob_type.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/collaborator.py
+-rw-r--r--   0 root         (0) root         (0)     5166 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/create_inbox_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     7424 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/dataset_column.py
+-rw-r--r--   0 root         (0) root         (0)    12558 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/dataset_new_request.py
+-rw-r--r--   0 root         (0) root         (0)     9991 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/dataset_new_version_request.py
+-rw-r--r--   0 root         (0) root         (0)    10114 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/dataset_update_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     7791 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/kaggle_models_extended.py
+-rw-r--r--   0 root         (0) root         (0)    20199 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/kernel_push_request.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/license.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/model_instance_new_version_request.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/model_instance_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/model_new_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    10055 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/model_new_request.py
+-rw-r--r--   0 root         (0) root         (0)     9096 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/model_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/result.py
+-rw-r--r--   0 root         (0) root         (0)     7844 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/models/start_blob_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/start_blob_upload_response.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-08-02 23:56:16.000000 kaggle-1.6.0a5/kaggle/models/upload_file.py
+-rw-r--r--   0 root         (0) root         (0)    13927 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 23:56:20.547502 kaggle-1.6.0a5/kaggle/test/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/kaggle/test/test_authenticate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 23:56:20.539502 kaggle-1.6.0a5/kaggle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      609 2023-08-02 23:56:20.000000 kaggle-1.6.0a5/kaggle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-08-02 23:56:20.000000 kaggle-1.6.0a5/kaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 23:56:20.000000 kaggle-1.6.0a5/kaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-08-02 23:56:20.000000 kaggle-1.6.0a5/kaggle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-08-02 23:56:20.000000 kaggle-1.6.0a5/kaggle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-02 23:56:20.000000 kaggle-1.6.0a5/kaggle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-08-02 23:56:20.547502 kaggle-1.6.0a5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-08-02 23:56:17.000000 kaggle-1.6.0a5/setup.py
```

### Comparing `kaggle-1.6.0a4/LICENSE` & `kaggle-1.6.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/PKG-INFO` & `kaggle-1.6.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a4
+Version: 1.6.0a5
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a4/README.md` & `kaggle-1.6.0a5/README.md`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/__init__.py` & `kaggle-1.6.0a5/kaggle/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/api/__init__.py` & `kaggle-1.6.0a5/kaggle/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/api/kaggle_api.py` & `kaggle-1.6.0a5/kaggle/api/kaggle_api.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/api/kaggle_api_extended.py` & `kaggle-1.6.0a5/kaggle/api/kaggle_api_extended.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         return str(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
 
 class KaggleApi(KaggleApi):
-    __version__ = '1.6.0a4'
+    __version__ = '1.6.0a5'
 
     CONFIG_NAME_PROXY = 'proxy'
     CONFIG_NAME_COMPETITION = 'competition'
     CONFIG_NAME_PATH = 'path'
     CONFIG_NAME_USER = 'username'
     CONFIG_NAME_KEY = 'key'
     CONFIG_NAME_SSL_CA_CERT = 'ssl_ca_cert'
@@ -1831,15 +1831,15 @@
         outpath = os.path.dirname(outfile)
         if not os.path.exists(outpath):
             os.makedirs(outpath)
         size = int(response.headers['Content-Length'])
         size_read = 0
         open_mode = 'wb'
         remote_date = datetime.strptime(response.headers['Last-Modified'],
-                                        '%a, %d %b %Y %X %Z')
+                                        '%a, %d %b %Y %H:%M:%S %Z')
         remote_date_timestamp = time.mktime(remote_date.timetuple())
 
         if not quiet:
             print('Downloading ' + os.path.basename(outfile) + ' to ' +
                   outpath)
 
         file_exists = os.path.isfile(outfile)
@@ -3393,15 +3393,15 @@
             ==========
             response: the response from the API
             outfile: the output file to write to
             quiet: suppress verbose output (default is True)
         """
         try:
             remote_date = datetime.strptime(response.headers['Last-Modified'],
-                                            '%a, %d %b %Y %X %Z')
+                                            '%a, %d %b %Y %H:%M:%S %Z')
             file_exists = os.path.isfile(outfile)
             if file_exists:
                 local_date = datetime.fromtimestamp(os.path.getmtime(outfile))
                 remote_size = int(response.headers['Content-Length'])
                 local_size = os.path.getsize(outfile)
                 if local_size < remote_size:
                     return True
```

### Comparing `kaggle-1.6.0a4/kaggle/api_client.py` & `kaggle-1.6.0a5/kaggle/api_client.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/cli.py` & `kaggle-1.6.0a5/kaggle/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1322,20 +1322,21 @@
     ]
     model_instance_versions_choices = ['init', 'create', 'download', 'delete']
     files_choices = ['upload']
     config_choices = ['view', 'set', 'unset']
 
     kaggle = 'Use one of:\ncompetitions {' + ', '.join(
         competitions_choices) + '}\ndatasets {' + ', '.join(
-            datasets_choices) + '}\nmodels {' + ', '.join(
-                models_choices) + '}\nmodels instances {' + ', '.join(
-                    model_instances_choices
-                ) + '}\nmodels instances versions {' + ', '.join(
-                    model_instance_versions_choices
-                ) + '}\nconfig {' + ', '.join(config_choices) + '}'
+            datasets_choices) + '}\nkernels {' + ', '.join(
+                kernels_choices) + '}\nmodels {' + ', '.join(
+                    models_choices) + '}\nmodels instances {' + ', '.join(
+                        model_instances_choices
+                    ) + '}\nmodels instances versions {' + ', '.join(
+                        model_instance_versions_choices
+                    ) + '}\nconfig {' + ', '.join(config_choices) + '}'
 
     group_competitions = 'Commands related to Kaggle competitions'
     group_datasets = 'Commands related to Kaggle datasets'
     group_kernels = 'Commands related to Kaggle kernels'
     group_models = 'Commands related to Kaggle models'
     group_model_instances = 'Commands related to Kaggle model instances'
     group_model_instance_versions = 'Commands related to Kaggle model instance versions'
```

### Comparing `kaggle-1.6.0a4/kaggle/configuration.py` & `kaggle-1.6.0a5/kaggle/configuration.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/__init__.py` & `kaggle-1.6.0a5/kaggle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/api_blob_type.py` & `kaggle-1.6.0a5/kaggle/models/api_blob_type.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/collaborator.py` & `kaggle-1.6.0a5/kaggle/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/create_inbox_file_request.py` & `kaggle-1.6.0a5/kaggle/models/create_inbox_file_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/dataset_column.py` & `kaggle-1.6.0a5/kaggle/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/dataset_new_request.py` & `kaggle-1.6.0a5/kaggle/models/dataset_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/dataset_new_version_request.py` & `kaggle-1.6.0a5/kaggle/models/dataset_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/dataset_update_settings_request.py` & `kaggle-1.6.0a5/kaggle/models/dataset_update_settings_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/error.py` & `kaggle-1.6.0a5/kaggle/models/error.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/kaggle_models_extended.py` & `kaggle-1.6.0a5/kaggle/models/kaggle_models_extended.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/kernel_push_request.py` & `kaggle-1.6.0a5/kaggle/models/kernel_push_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/license.py` & `kaggle-1.6.0a5/kaggle/models/license.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/model_instance_new_version_request.py` & `kaggle-1.6.0a5/kaggle/models/model_instance_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/model_instance_update_request.py` & `kaggle-1.6.0a5/kaggle/models/model_instance_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/model_new_instance_request.py` & `kaggle-1.6.0a5/kaggle/models/model_new_instance_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         The framework of the model instance  # noqa: E501
 
         :param framework: The framework of this ModelNewInstanceRequest.  # noqa: E501
         :type: str
         """
         if framework is None:
             raise ValueError("Invalid value for `framework`, must not be `None`")  # noqa: E501
-        allowed_values = ["tensorFlow1", "tensorFlow2", "tfLite", "tfJs", "pyTorch", "jax", "coral", "scikitLearn", "mxnet", "onnx"]  # noqa: E501
+        allowed_values = ["tensorFlow1", "tensorFlow2", "tfLite", "tfJs", "pyTorch", "jax", "coral", "scikitLearn", "mxnet", "onnx", "keras"]  # noqa: E501
         if framework not in allowed_values:
             raise ValueError(
                 "Invalid value for `framework` ({0}), must be one of {1}"  # noqa: E501
                 .format(framework, allowed_values)
             )
 
         self._framework = framework
```

### Comparing `kaggle-1.6.0a4/kaggle/models/model_new_request.py` & `kaggle-1.6.0a5/kaggle/models/model_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/model_update_request.py` & `kaggle-1.6.0a5/kaggle/models/model_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/result.py` & `kaggle-1.6.0a5/kaggle/models/result.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/start_blob_upload_request.py` & `kaggle-1.6.0a5/kaggle/models/start_blob_upload_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/start_blob_upload_response.py` & `kaggle-1.6.0a5/kaggle/models/start_blob_upload_response.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/models/upload_file.py` & `kaggle-1.6.0a5/kaggle/models/upload_file.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/rest.py` & `kaggle-1.6.0a5/kaggle/rest.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/test/__init__.py` & `kaggle-1.6.0a5/kaggle/test/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle/test/test_authenticate.py` & `kaggle-1.6.0a5/kaggle/test/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/kaggle.egg-info/PKG-INFO` & `kaggle-1.6.0a5/kaggle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a4
+Version: 1.6.0a5
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a4/kaggle.egg-info/SOURCES.txt` & `kaggle-1.6.0a5/kaggle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a4/setup.py` & `kaggle-1.6.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='kaggle',
-    version='1.6.0a4',
+    version='1.6.0a5',
     description='Kaggle API',
     long_description=
     ('Official API for https://www.kaggle.com, accessible using a command line '
      'tool implemented in Python. Beta release - Kaggle reserves the right to '
      'modify the API functionality currently offered.'),
     author='Kaggle',
     author_email='support@kaggle.com',
```

