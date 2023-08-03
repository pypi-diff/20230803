# Comparing `tmp/atlas-consortia-clt-1.0.0.tar.gz` & `tmp/atlas-consortia-clt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-consortia-clt-1.0.0.tar", last modified: Wed Jul 19 19:27:06 2023, max compression
+gzip compressed data, was "atlas-consortia-clt-1.0.1.tar", last modified: Thu Aug  3 17:07:44 2023, max compression
```

## Comparing `atlas-consortia-clt-1.0.0.tar` & `atlas-consortia-clt-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.580614 atlas-consortia-clt-1.0.0/
--rw-r--r--   0 TJM159     (503) staff       (20)       46 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/MANIFEST.in
--rw-r--r--   0 TJM159     (503) staff       (20)     4090 2023-07-19 19:27:06.580263 atlas-consortia-clt-1.0.0/PKG-INFO
--rw-r--r--   0 TJM159     (503) staff       (20)     3426 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/README.md
--rw-r--r--   0 TJM159     (503) staff       (20)     1053 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/pyproject.toml
--rw-r--r--   0 TJM159     (503) staff       (20)      111 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/requirements.txt
--rw-r--r--   0 TJM159     (503) staff       (20)       38 2023-07-19 19:27:06.580694 atlas-consortia-clt-1.0.0/setup.cfg
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.549641 atlas-consortia-clt-1.0.0/src/
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.553424 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/
--rw-r--r--   0 TJM159     (503) staff       (20)       37 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/__init__.py
--rw-r--r--   0 TJM159     (503) staff       (20)       22 2023-07-11 17:17:36.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/__version__.py
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.574663 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/
--rw-r--r--   0 TJM159     (503) staff       (20)        0 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/__init__.py
--rw-r--r--   0 TJM159     (503) staff       (20)      119 2023-07-11 17:04:50.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/app.cfg
--rw-r--r--   0 TJM159     (503) staff       (20)     1011 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/config.py
--rw-r--r--   0 TJM159     (503) staff       (20)     3272 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/help.py
--rw-r--r--   0 TJM159     (503) staff       (20)    11988 2023-07-11 16:10:16.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/main.py
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.578260 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/hubmap_clt/
--rw-r--r--   0 TJM159     (503) staff       (20)      418 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/hubmap_clt/__init__.py
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.579542 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/sennet_clt/
--rw-r--r--   0 TJM159     (503) staff       (20)      418 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/sennet_clt/__init__.py
-drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-07-19 19:27:06.562449 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/
--rw-r--r--   0 TJM159     (503) staff       (20)     4090 2023-07-19 19:27:06.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/PKG-INFO
--rw-r--r--   0 TJM159     (503) staff       (20)      707 2023-07-19 19:27:06.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/SOURCES.txt
--rw-r--r--   0 TJM159     (503) staff       (20)        1 2023-07-19 19:27:06.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/dependency_links.txt
--rw-r--r--   0 TJM159     (503) staff       (20)      118 2023-07-19 19:27:06.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/entry_points.txt
--rw-r--r--   0 TJM159     (503) staff       (20)      112 2023-07-19 19:27:06.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/requires.txt
--rw-r--r--   0 TJM159     (503) staff       (20)       20 2023-07-19 19:27:06.000000 atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/top_level.txt
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.433260 atlas-consortia-clt-1.0.1/
+-rw-r--r--   0 TJM159     (503) staff       (20)       46 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/MANIFEST.in
+-rw-r--r--   0 TJM159     (503) staff       (20)     4090 2023-08-03 17:07:44.432889 atlas-consortia-clt-1.0.1/PKG-INFO
+-rw-r--r--   0 TJM159     (503) staff       (20)     3426 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/README.md
+-rw-r--r--   0 TJM159     (503) staff       (20)     1053 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/pyproject.toml
+-rw-r--r--   0 TJM159     (503) staff       (20)      111 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/requirements.txt
+-rw-r--r--   0 TJM159     (503) staff       (20)       38 2023-08-03 17:07:44.433322 atlas-consortia-clt-1.0.1/setup.cfg
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.395511 atlas-consortia-clt-1.0.1/src/
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.399478 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/
+-rw-r--r--   0 TJM159     (503) staff       (20)       37 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/__init__.py
+-rw-r--r--   0 TJM159     (503) staff       (20)       22 2023-08-03 17:04:03.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/__version__.py
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.426731 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/
+-rw-r--r--   0 TJM159     (503) staff       (20)        0 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/__init__.py
+-rw-r--r--   0 TJM159     (503) staff       (20)      119 2023-08-03 16:48:40.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/app.cfg
+-rw-r--r--   0 TJM159     (503) staff       (20)     1011 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/config.py
+-rw-r--r--   0 TJM159     (503) staff       (20)     3272 2023-07-10 13:00:52.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/help.py
+-rw-r--r--   0 TJM159     (503) staff       (20)    11508 2023-08-03 16:36:36.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/main.py
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.429910 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/hubmap_clt/
+-rw-r--r--   0 TJM159     (503) staff       (20)      407 2023-08-03 16:36:36.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/hubmap_clt/__init__.py
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.432180 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/sennet_clt/
+-rw-r--r--   0 TJM159     (503) staff       (20)      408 2023-08-03 16:36:36.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/sennet_clt/__init__.py
+drwxr-xr-x   0 TJM159     (503) staff       (20)        0 2023-08-03 17:07:44.411689 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/
+-rw-r--r--   0 TJM159     (503) staff       (20)     4090 2023-08-03 17:07:44.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/PKG-INFO
+-rw-r--r--   0 TJM159     (503) staff       (20)      707 2023-08-03 17:07:44.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/SOURCES.txt
+-rw-r--r--   0 TJM159     (503) staff       (20)        1 2023-08-03 17:07:44.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/dependency_links.txt
+-rw-r--r--   0 TJM159     (503) staff       (20)      118 2023-08-03 17:07:44.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/entry_points.txt
+-rw-r--r--   0 TJM159     (503) staff       (20)      112 2023-08-03 17:07:44.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/requires.txt
+-rw-r--r--   0 TJM159     (503) staff       (20)       20 2023-08-03 17:07:44.000000 atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/top_level.txt
```

### Comparing `atlas-consortia-clt-1.0.0/PKG-INFO` & `atlas-consortia-clt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-consortia-clt
-Version: 1.0.0
+Version: 1.0.1
 Summary: HuBMAP and SenNet command-line interface to download data using a manifest file.
 Author-email: Atlas Consortia <api-developers@hubmapconsortium.org>
 License: MIT
 Project-URL: Homepage, https://github.com/x-atlas-consortia/clt
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/clt/issues
 Keywords: HuBMAP CLT,SenNet CLT,HuBMAP,SenNet,CLT,Command Line Transfer,Manifest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atlas-consortia-clt-1.0.0/README.md` & `atlas-consortia-clt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `atlas-consortia-clt-1.0.0/pyproject.toml` & `atlas-consortia-clt-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/config.py` & `atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/config.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/help.py` & `atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/help.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-clt-1.0.0/src/atlas_consortia_clt/common/main.py` & `atlas-consortia-clt-1.0.1/src/atlas_consortia_clt/common/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import collections
 import os.path
 import re
 import requests
 import subprocess
 import sys
 import tempfile
 
@@ -80,78 +81,67 @@
     if endpoint_connected is False:
         print(f"The endpoint {local_id} \nis not active. Please consult the Globus Connect documentation  \n"
               f"to start the local endpoint. Once the endpoint is connected, try again")
         sys.exit(1)
 
     # Open the manifest file and verify the contents
     f = open(file_name, "r")
-    # A list of the ID's is necessary to send to the ingest webservice. The dictionary is used to map the output of the
-    # webservice back to the manifest entry it came from.
-    id_list = []
-    manifest_list = []
+
+    # A list of the ID's is necessary to send to the ingest webservice.
+    id_list = set()
+    # entity id: [specific path, specific path, ...]
+    manifest_lists = collections.defaultdict(list)
     for x in f:
         if x.startswith("dataset_id") is False:
             if x != "" and x != "\n":
                 pattern = "^(\\S+)[ \t]+([^\t\n]+)"
                 matches = re.search(pattern, x)
                 if matches is None:
                     print(f"There was a problem with one of the entries in {file_name}. Please review {file_name} and "
                           f"for any formatting errors")
                     sys.exit(1)
-                manifest_dict = {}
-                id_list.append(matches.group(1).strip('"'))
-                manifest_dict[matches.group(1).strip('"')] = matches.group(2).strip('"')
-                manifest_list.append(manifest_dict)
+                id_list.add(matches.group(1).strip('"'))
+                manifest_lists[matches.group(1).strip('"')].append(matches.group(2).strip('"'))
     if len(id_list) == 0:
         print(f"File {file_name} contained nothing or only blank lines. \n"
               f"Each line on the manifest must be the id for the dataset/upload, followed by its path and \n"
               f"separated with a space. Example: {config.entity_id} /expr.h5ad")
         sys.exit(1)
     # send the list of uuid's to the ingest webservice to retrieve the endpoint uuid and relative path.
-    r = requests.post(f"{config.ingest_url}/entities/file-system-rel-path", json=id_list)
+    r = requests.post(f"{config.ingest_url}/entities/file-system-rel-path", json=list(id_list))
     path_json = r.json()
     if r.status_code != 200:
         print(f"There were problems with {len(path_json)} dataset id's in {file_name}:\n")
         for each in path_json:
             print(f"{each['id']}: {each['message']} \n")
         sys.exit(1)
 
-    # Create a list of the unique endpoint uuid's. For each entry in the list, a separate call to globus transfer
-    # must be made
-    unique_globus_endpoint_ids = []
-    # Add the particular path from manifest_dict into path_dict
-    for each in path_json:
-        each_dict = {}
-        for item in manifest_list:
-            if each["id"] in item.keys():
-                each_dict = item
-                break
-        each["specific_path"] = each_dict[each["id"]].strip('"').strip()
-        if each["globus_endpoint_uuid"] not in unique_globus_endpoint_ids:
-            unique_globus_endpoint_ids.append(each["globus_endpoint_uuid"])
+    globus_endpoints = collections.defaultdict(list)
+    for item in path_json:
+        entity_id = item["id"]
+        manifest_items = [{**item, "specific_path": m} for m in manifest_lists[entity_id]]
+        globus_endpoints[item["globus_endpoint_uuid"]].extend(manifest_items)
+
     at_least_one_success = []
-    for each in unique_globus_endpoint_ids:
-        endpoint_list = []
-        for item in path_json:
-            if item["globus_endpoint_uuid"] == each:
-                endpoint_list.append(item)
-        is_successful = batch_transfer(endpoint_list, each, local_id, args, config)
+    for globus_endpoint_uuid in list(globus_endpoints.keys()):
+        endpoint_items = globus_endpoints[globus_endpoint_uuid]
+        is_successful = batch_transfer(endpoint_items, globus_endpoint_uuid, local_id, args, config)
         if is_successful:
-            at_least_one_success.append(each)
+            at_least_one_success.append(globus_endpoint_uuid)
     if len(at_least_one_success) > 0:
         destination = args.destination.replace("\\", os.sep)
         destination = destination.replace("/", os.sep)
         print(f"Globus transfer successfully initiated. Files to be downloaded to <Home-Folder>/{destination} where "
               f"Home-Folder is the default download\ndirectory designated by Globus Connect Personal. "
               f"For instructions on how to view the current GCP download directory, visit:\n"
               f"{config.docs_url}. \n\nDownloading from endpoint(s): ")
         for endpoint in at_least_one_success:
             print(f"\t{endpoint}")
-        print(f"\nThe status of the transfer(s) may be found at https://app.globus.org/activity. For more information,"
-              f" please consult the documentation")
+        print("\nThe status of the transfer(s) may be found at https://app.globus.org/activity. For more information,"
+              " please consult the documentation")
 
 
 # Construct the file used for the globus batch tranfer. Each source endpoint id needs a separate globus transfer.
 # This also allows each one to have a unique task id which is relayed back to the user. A temporary file is created
 # and lines from the incoming manifest file are transformed into how they are needed by globus
 def batch_transfer(endpoint_list, globus_endpoint_uuid, local_id, args, config: Config):
     temp = tempfile.NamedTemporaryFile(mode="w+t", delete=False)
@@ -197,14 +187,15 @@
     whoami_process = subprocess.Popen(["globus", "whoami"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     whoami_show = whoami_process.communicate()[0].decode("utf-8")
     if whoami_process.returncode == 0:
         print(whoami_show)
     else:
         print(f"You are not logged in. Login with '{config.name} login'")
 
+
 # Forces a login to globus through the default web browser
 def login(args, config: Config):
     # Check if the user is logged in
     whoami_process = subprocess.Popen(["globus", "whoami"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     whoami_show = whoami_process.communicate()[0].decode("utf-8").strip()
     if whoami_process.returncode == 0:
         print(f"You are already logged in as {whoami_show}. Logout with '{config.name} logout'")
@@ -222,15 +213,15 @@
 def logout(args, config: Config):
     # Check if the user is logged in
     whoami_process = subprocess.Popen(["globus", "whoami"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     whoami_process.communicate()[0].decode("utf-8").strip()
     if whoami_process.returncode != 0:
         print(f"You are not logged in. Login with '{config.name} login'")
         return
-    
+
     # Prompt the user to confirm that they want to logout
     user_input = None
     while user_input is None or user_input.lower() not in ["y", "n", ""]:
         user_input = input("Are you sure you want to logout? [y/N]: ")
 
     if user_input.lower() != "y":
         print("Logout cancelled.")
```

### Comparing `atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/PKG-INFO` & `atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-consortia-clt
-Version: 1.0.0
+Version: 1.0.1
 Summary: HuBMAP and SenNet command-line interface to download data using a manifest file.
 Author-email: Atlas Consortia <api-developers@hubmapconsortium.org>
 License: MIT
 Project-URL: Homepage, https://github.com/x-atlas-consortia/clt
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/clt/issues
 Keywords: HuBMAP CLT,SenNet CLT,HuBMAP,SenNet,CLT,Command Line Transfer,Manifest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atlas-consortia-clt-1.0.0/src/atlas_consortia_clt.egg-info/SOURCES.txt` & `atlas-consortia-clt-1.0.1/src/atlas_consortia_clt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

