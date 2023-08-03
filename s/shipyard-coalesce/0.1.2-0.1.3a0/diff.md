# Comparing `tmp/shipyard_coalesce-0.1.2.tar.gz` & `tmp/shipyard_coalesce-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_coalesce-0.1.2.tar", max compression
+gzip compressed data, was "shipyard_coalesce-0.1.3a0.tar", max compression
```

## Comparing `shipyard_coalesce-0.1.2.tar` & `shipyard_coalesce-0.1.3a0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1098 2023-05-04 18:37:25.928580 shipyard_coalesce-0.1.2/README.md
--rw-r--r--   0        0        0      557 2023-05-05 02:20:31.274384 shipyard_coalesce-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-04 17:02:13.445484 shipyard_coalesce-0.1.2/shipyard_coalesce/__init__.py
--rw-r--r--   0        0        0     1182 2023-05-04 21:20:43.160884 shipyard_coalesce-0.1.2/shipyard_coalesce/cli/determine_status.py
--rw-r--r--   0        0        0     2492 2023-05-05 00:03:51.253151 shipyard_coalesce-0.1.2/shipyard_coalesce/cli/trigger_sync.py
--rw-r--r--   0        0        0     5678 2023-05-05 02:19:47.302622 shipyard_coalesce-0.1.2/shipyard_coalesce/coalesce.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-12 18:48:21.826104 shipyard_coalesce-0.1.3a0/README.md
+-rw-r--r--   0        0        0      559 2023-08-03 19:23:49.387830 shipyard_coalesce-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-12 18:48:21.826398 shipyard_coalesce-0.1.3a0/shipyard_coalesce/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-28 00:25:41.245643 shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/authtest.py
+-rw-r--r--   0        0        0     1212 2023-05-12 18:48:21.826571 shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/determine_status.py
+-rw-r--r--   0        0        0     3761 2023-08-03 19:22:47.195084 shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/trigger_sync.py
+-rw-r--r--   0        0        0     6424 2023-08-03 19:24:04.784231 shipyard_coalesce-0.1.3a0/shipyard_coalesce/coalesce.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.3a0/PKG-INFO
```

### Comparing `shipyard_coalesce-0.1.2/README.md` & `shipyard_coalesce-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.2/pyproject.toml` & `shipyard_coalesce-0.1.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-coalesce"
-version = "0.1.2"
+version = "0.1.3a0"
 description = "A local client for connecting and working with Coalesce"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_coalesce"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_coalesce-0.1.2/shipyard_coalesce/cli/determine_status.py` & `shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/determine_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import shipyard_bp_utils as shipyard
+import sys
 from shipyard_coalesce import CoalesceClient
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument("--run-id", dest="run_id", required=False, default=None)
@@ -19,19 +20,19 @@
     base_folder_name = shipyard.logs.determine_base_artifact_folder("coalesce")
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
         base_folder_name
     )
     shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
 
     # check if the job id was provided, if not then read it from the artifacts folder
-    if run_id is None:
+    if run_id is None or run_id == '':
         response = shipyard.logs.read_pickle_file(
             artifact_subfolder_paths, "coalesce_response"
         )
         run_id = response["runCounter"]
     # fetch the status and return the exit code
     status = client.determine_sync_status(run_id)
-    return status
+    sys.exit(status)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_coalesce-0.1.2/shipyard_coalesce/coalesce.py` & `shipyard_coalesce-0.1.3a0/shipyard_coalesce/coalesce.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 class CoalesceClient(Etl):
     def __init__(self, access_token: str):
         self.base_url = "https://app.coalescesoftware.io/scheduler"
         super().__init__(access_token)
 
     def trigger_sync(
-        self,
-        environment_id: str,
-        job_id: str,
-        snowflake_username: str,
-        snowflake_password: str,
-        snowflake_role: str,
-        snowflake_warehouse: str = None,
-        parallelism: int = 16,
-        include_nodes_selector: str = None,
-        exclude_nodes_selector=None,
+            self,
+            environment_id: str,
+            job_id: str,
+            snowflake_username: str,
+            snowflake_password: str,
+            snowflake_role: str,
+            snowflake_warehouse: str = None,
+            parallelism: int = 16,
+            include_nodes_selector: str = None,
+            exclude_nodes_selector=None,
     ) -> dict[any, any]:
         """
         # reference is available here: https://docs.coalesce.io/reference/startrun
         Args:
             exclude_nodes_selector (): nodes excluded for a job
             environment_id:  the environment being refreshed
             job_id: the ID of a job to be run
@@ -63,20 +63,20 @@
 
         payload = {"runDetails": details, "userCredentials": credentials}
 
         response = requests.post(url=url, json=payload, headers=headers)
 
         if response.status_code == 200:
             self.logger.info("Successfully triggered job")
-
+            return response.json()
         else:
             self.logger.error(f"Error message: {response.json()['error']['errorString']}")
             self.logger.error(f"Error details: {response.json()['error']['errorDetail']}")
-
-        return response.json()
+            raise Exception(
+                f"Error occurred when attempting to trigger sync: {response.json()['error']['errorString']}")
 
     def get_run_status(self, run_counter: int) -> requests.Response:
         """Returns the HTTP response for a Coalesce job status
 
         Args:
             run_counter (int): The specific run in which to fetch the status
 
@@ -117,14 +117,17 @@
                 return self.EXIT_CODE_SYNC_ALREADY_RUNNING
             elif status == "timeout":
                 self.logger.info("Status: timeout")
                 return self.EXIT_CODE_FINAL_STATUS_INCOMPLETE
             elif status == "canceled":
                 self.logger.info("Status: canceled")
                 return self.EXIT_CODE_FINAL_STATUS_CANCELLED
+            elif status == "failed":
+                self.logger.info("Status: failed")
+                return self.EXIT_CODE_FINAL_STATUS_ERRORED
             else:
                 self.logger.info(f"Status: {status}")
                 return self.EXIT_CODE_UNKNOWN_STATUS
 
         elif response.status_code == 400:
             self.logger.error(
                 f"There was an error when attempting to fetch the status of the job. The message returned from the API is {json['error']['errorString']}"
@@ -132,7 +135,19 @@
             return self.EXIT_CODE_BAD_REQUEST
 
         elif response.status_code == 401:
             self.logger.error(
                 "Error occurred when attempting to authenticate, please ensure that the token provided is valid"
             )
             return self.EXIT_CODE_INVALID_CREDENTIALS
+
+    def connect(self):
+        """ 
+        Connects to the Coalesce API and returns the response
+        """
+        url = "https://app.coalescesoftware.io/scheduler/runStatus?runCounter=1"
+        headers = {
+            "accept": "application/json",
+            "Authorization": f"Bearer {self.access_token}",
+        }
+        response = requests.get(url=url, headers=headers)
+        return response.status_code
```

### Comparing `shipyard_coalesce-0.1.2/PKG-INFO` & `shipyard_coalesce-0.1.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-coalesce
-Version: 0.1.2
+Version: 0.1.3a0
 Summary: A local client for connecting and working with Coalesce
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

