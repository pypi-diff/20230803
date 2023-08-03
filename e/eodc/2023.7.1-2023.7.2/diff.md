# Comparing `tmp/eodc-2023.7.1.tar.gz` & `tmp/eodc-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.7.1.tar", max compression
+gzip compressed data, was "eodc-2023.7.2.tar", max compression
```

## Comparing `eodc-2023.7.1.tar` & `eodc-2023.7.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-07-27 07:03:14.034430 eodc-2023.7.1/README.md
--rw-r--r--   0        0        0      120 2023-07-27 07:03:14.034430 eodc-2023.7.1/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-07-27 07:03:14.034430 eodc-2023.7.1/eodc/dask.py
--rw-r--r--   0        0        0    11966 2023-07-27 07:03:14.034430 eodc-2023.7.1/eodc/faas.py
--rw-r--r--   0        0        0      537 2023-07-27 07:03:14.034430 eodc-2023.7.1/eodc/settings.py
--rw-r--r--   0        0        0     1198 2023-07-27 07:03:14.034430 eodc-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 eodc-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-08-03 13:58:22.081580 eodc-2023.7.2/README.md
+-rw-r--r--   0        0        0      120 2023-08-03 13:58:22.081580 eodc-2023.7.2/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-08-03 13:58:22.081580 eodc-2023.7.2/eodc/dask.py
+-rw-r--r--   0        0        0    11985 2023-08-03 13:58:22.085580 eodc-2023.7.2/eodc/faas.py
+-rw-r--r--   0        0        0      537 2023-08-03 13:58:22.085580 eodc-2023.7.2/eodc/settings.py
+-rw-r--r--   0        0        0     1198 2023-08-03 13:58:22.085580 eodc-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 eodc-2023.7.2/PKG-INFO
```

### Comparing `eodc-2023.7.1/README.md` & `eodc-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.7.1/eodc/dask.py` & `eodc-2023.7.2/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.7.1/eodc/faas.py` & `eodc-2023.7.2/eodc/faas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import asyncio
 import json
 import logging
 import re
-import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional
 from urllib.parse import urljoin
 
 import requests
@@ -104,32 +104,33 @@
                 name=self.processor_details.workflow_template_name
             ),
             workflows_service=self.workflows_service,
             namespace=settings.NAMESPACE,
             generate_name=f"{self.processor_details.name}-",
             arguments=arguments,
         )
+
         workflow.create()
 
         logger.info(
             f"Submitted {self.processor_details.name.upper()} workflow: {workflow.name}"
         )
         return workflow.name
 
-    def wait_for_completion(self, workflow_name, poll_interval=30):
+    async def wait_for_completion(self, workflow_name, poll_interval=30):
         wf = self.workflows_service.get_workflow(
             workflow_name, namespace=settings.NAMESPACE
         )
 
         # keep polling for workflow status until completed,
         # at the interval dictated by the user
         # While the workflow is still initialising, this comes back as None,
         # so have to accept that here too!
         while wf.status.phase in ("Pending", "Running", None):
-            time.sleep(poll_interval)
+            await asyncio.sleep(poll_interval)
             wf = self.workflows_service.get_workflow(
                 workflow_name, namespace=settings.NAMESPACE
             )
         return wf
 
     def get_workflow_status(self, workflow_name: str) -> dict:
         # TODO: Limit this response to only the required fields
```

### Comparing `eodc-2023.7.1/eodc/settings.py` & `eodc-2023.7.2/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.7.1/pyproject.toml` & `eodc-2023.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.7.1"
+version = "2023.7.2"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.7.1/PKG-INFO` & `eodc-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

