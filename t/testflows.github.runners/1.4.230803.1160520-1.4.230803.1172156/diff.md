# Comparing `tmp/testflows.github.runners-1.4.230803.1160520.tar.gz` & `tmp/testflows.github.runners-1.4.230803.1172156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.4.230803.1160520.tar", last modified: Thu Aug  3 16:05:20 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.4.230803.1172156.tar", last modified: Thu Aug  3 17:21:57 2023, max compression
```

## Comparing `testflows.github.runners-1.4.230803.1160520.tar` & `testflows.github.runners-1.4.230803.1172156.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-03 02:12:02.000000 testflows.github.runners-1.4.230803.1160520/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3019 2023-08-02 18:47:51.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    26388 2023-08-03 15:50:11.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13655 2023-08-03 16:01:48.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4481 2023-08-03 15:50:11.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    15656 2023-08-02 20:33:51.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    27664 2023-08-03 15:50:11.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3032 2023-08-02 20:36:59.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5553 2023-08-03 15:50:11.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230803.1160520/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 16:05:20.791744 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-03 16:05:20.000000 testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-03 02:12:02.000000 testflows.github.runners-1.4.230803.1172156/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.017770 testflows.github.runners-1.4.230803.1172156/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.017770 testflows.github.runners-1.4.230803.1172156/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3019 2023-08-02 18:47:51.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    26203 2023-08-03 17:09:40.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13640 2023-08-03 17:20:44.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5270 2023-08-03 17:10:08.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15656 2023-08-02 20:33:51.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27693 2023-08-03 16:56:37.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3032 2023-08-02 20:36:59.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230803.1172156/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:21:57.021770 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-03 17:21:56.000000 testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.4.230803.1160520/LICENSE` & `testflows.github.runners-1.4.230803.1172156/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/PKG-INFO` & `testflows.github.runners-1.4.230803.1172156/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230803.1160520
+Version: 1.4.230803.1172156
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.4.230803.1160520/README.rst` & `testflows.github.runners-1.4.230803.1172156/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/setup.py` & `testflows.github.runners-1.4.230803.1172156/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.4.230803.1160520",
+    version="1.4.230803.1172156",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/__init__.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.4.230803.1160520"
+__version__ = "1.4.230803.1172156"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/actions.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/args.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.api_watch import api_watch
 from testflows.github.runners.scripts import Scripts, scripts
 from testflows.github.runners.logger import logger
-from testflows.github.runners.config import Config, check_image
+from testflows.github.runners.config import Config, check_image, check_ssh_key
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 import testflows.github.runners.delete as delete
 
 from requests_cache import DO_NOT_CACHE, EXPIRE_IMMEDIATELY, install_cache
@@ -633,54 +633,49 @@
         yield
 
 
 def main(
     config, scripts: Scripts, worker_pool: ThreadPoolExecutor, terminate_timeout=30
 ):
     """Auto-scale runners service."""
-
+    user_ssh_keys: list[SSHKey] = []
     terminate = threading.Event()
 
     try:
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action("Logging in to GitHub"):
             github = Github(login_or_token=config.github_token, per_page=100)
 
         with Action(f"Getting repository {config.github_repository}"):
             repo: Repository = github.get_repo(config.github_repository)
 
         with Action("Checking if default image exists"):
-            config.default_image = check_image(
-                client=client, image=config.default_image
-            )
+            config.default_image = check_image(client, config.default_image)
 
         with Action(f"Checking if SSH key exists"):
-            with open(config.ssh_key, "r", encoding="utf-8") as ssh_key_file:
-                public_key = ssh_key_file.read()
-            key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
-            ssh_key = SSHKey(name=key_name, public_key=public_key)
-
-            if not client.ssh_keys.get_by_name(name=ssh_key.name):
-                with Action(f"Creating SSH key {ssh_key.name}"):
-                    client.ssh_keys.create(
-                        name=ssh_key.name, public_key=ssh_key.public_key
-                    )
+            ssh_key: SSHKey = check_ssh_key(client, config.ssh_key)
+
+        if config.user_ssh_keys:
+            with Action(f"Checking if user SSH keys exist"):
+                for user_ssh_key in config.user_ssh_keys:
+                    user_ssh_keys.append(check_ssh_key(client, user_ssh_key))
 
         try:
             with Action("Creating scale up service"):
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
                     recycle=config.recycle,
                     server_prices=config.server_prices,
                     with_label=config.with_label,
                     scripts=scripts,
                     ssh_key=ssh_key,
+                    user_ssh_keys=user_ssh_keys,
                     default_server_type=config.default_server_type,
                     default_image=config.default_image,
                     default_location=config.default_location,
                     worker_pool=worker_pool,
                     hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/cloud.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,20 +199,21 @@
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Installing service"):
         command = f"\"su - ubuntu -c '"
-        command += f"GITHUB_TOKEN={config.github_token} "
-        command += f"GITHUB_REPOSITORY={config.github_repository} "
-        command += f"HETZNER_TOKEN={config.hetzner_token}; "
-
         command += "github-runners"
-        command += command_options(config)
+        command += command_options(
+            config,
+            github_token=config.github_token,
+            github_repository=config.github_repository,
+            hetzner_token=config.hetzner_token,
+        )
         command += " service install -f'\""
 
         ssh(server, command)
 
 
 def upgrade(args, config: Config):
     """Upgrade github-runners application on a cloud instance."""
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/delete.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/logger.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/request.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scale_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,15 @@
     server_location: Location,
     server_image: Image,
     startup_script: str,
     setup_script: str,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
+    user_ssh_keys: list[SSHKey],
     timeout=60,
 ):
     """Create specified number of server instances."""
     client = Client(token=hetzner_token)
 
     server_labels = {
         f"github-runner-label-{i}": value for i, value in enumerate(labels)
@@ -216,15 +217,15 @@
 
     with Action(f"Creating server {name} with labels {labels}"):
         response = client.servers.create(
             name=name,
             server_type=server_type,
             location=server_location,
             image=server_image,
-            ssh_keys=[ssh_key],
+            ssh_keys=[ssh_key] + user_ssh_keys,
             labels=server_labels,
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server {server.name} to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
@@ -342,25 +343,43 @@
                 f"Maximum number of servers {max_servers_in_workflow_run} for {run_id} has been reached",
                 stacklevel=3,
             ):
                 return True
     return False
 
 
+def recyclable_server_match(
+    server: BoundServer,
+    server_type: ServerType,
+    server_location: Location,
+    ssh_key: SSHKey,
+):
+    """Check if a recyclable server matches for the specified
+    server type, location and ssh key."""
+    if server.server_type.name != server_type.name:
+        return False
+
+    if server_location and server.server_location.name != server_location.name:
+        return False
+
+    return ssh_key.name == server.server.labels.get(server_ssh_key_label)
+
+
 def scale_up(
     terminate: threading.Event,
     recycle: bool,
     server_prices: dict[str, float],
     with_label: str,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     hetzner_token: str,
     ssh_key: SSHKey,
+    user_ssh_keys: list[SSHKey],
     default_server_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
     max_servers_in_workflow_run: int,
     max_server_ready_time: int,
@@ -386,47 +405,36 @@
         server_location = get_server_location(labels=labels, default=default_location)
         server_image = get_server_image(
             client=client, labels=labels, default=default_image
         )
         startup_script = get_startup_script(server_type=server_type, scripts=scripts)
 
         with Action(
-            f"Trying to create server {name}, "
-            f"type: {server_type.name}, "
-            f"location: {server_location.name if server_location else 'any'}, "
-            f"ssh-key: {ssh_key.name}",
+            f"Trying to create server {name}",
             stacklevel=3,
             level=logging.DEBUG,
         ):
             pass
 
         if recycle:
             for server in servers:
                 if server.name.startswith(recycle_server_name_prefix):
                     recyclable_servers.append(server)
                     with Action(
-                        f"Trying to see if we can recycle {server.name}, "
-                        f"type: {server.server_type.name}, "
-                        f"location: {server.server_location.name}, "
-                        f"labels: {server.server.labels}",
+                        f"Checking if we can recycle {server.name}",
                         stacklevel=3,
                         level=logging.DEBUG,
                     ):
                         pass
 
-                    if (
-                        (server.server_type.name == server_type.name)
-                        and (
-                            server_location is None
-                            or server.server_location.name == server_location.name
-                        )
-                        and (
-                            server.server.labels.get("github-runner-ssh-key")
-                            == ssh_key.name
-                        )
+                    if recyclable_server_match(
+                        server=server,
+                        server_type=server_type,
+                        server_location=server_location,
+                        ssh_key=ssh_key,
                     ):
                         future = worker_pool.submit(
                             recycle_server,
                             server_name=server.name,
                             hetzner_token=hetzner_token,
                             setup_worker_pool=setup_worker_pool,
                             labels=labels,
@@ -512,14 +520,15 @@
             server_location=server_location,
             server_image=server_image,
             setup_script=scripts.setup,
             startup_script=startup_script,
             github_token=github_token,
             github_repository=github_repository,
             ssh_key=ssh_key,
+            user_ssh_keys=user_ssh_keys,
             timeout=max_server_ready_time,
         )
         future.server_name = name
         futures.append(future)
         servers.append(
             RunnerServer(
                 name=name,
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/server.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/service.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,31 @@
 
 NAME = "github-runners"
 SERVICE = f"/etc/systemd/system/{NAME}.service"
 
 from .actions import Action
 
 
-def command_options(config):
+def command_options(
+    config,
+    github_token="$GITHUB_TOKEN",
+    github_repository="$GITHUB_REPOSITORY",
+    hetzner_token="$HETZNER_TOKEN",
+):
     """Build service install command options not including:
 
     --github-token
     --github-repository
     --hetzner-token
     --ssh-key
     """
     command = ""
-    command += f" --github-token $GITHUB_TOKEN"
-    command += f" --github-repository $GITHUB_REPOSITORY"
-    command += f" --hetzner-token $HETZNER_TOKEN"
+    command += f" --github-token {github_token}"
+    command += f" --github-repository {github_repository}"
+    command += f" --hetzner-token {hetzner_token}"
     command += f" --config {config.config_file}" if config.config_file else ""
     command += f" --recycle " + "on" if config.recycle else "off"
     command += f" --end-of-life {config.end_of_life}" if config.end_of_life else ""
     command += f" --with-label {config.with_label}" if config.with_label else ""
     command += f" --workers {config.workers}"
     command += f" --default-type {config.default_server_type.name}"
     command += (
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows/github/runners/shell.py` & `testflows.github.runners-1.4.230803.1172156/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230803.1160520
+Version: 1.4.230803.1172156
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.4.230803.1160520/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.4.230803.1172156/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

