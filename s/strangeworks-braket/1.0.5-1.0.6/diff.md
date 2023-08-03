# Comparing `tmp/strangeworks_braket-1.0.5.tar.gz` & `tmp/strangeworks_braket-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_braket-1.0.5.tar", max compression
+gzip compressed data, was "strangeworks_braket-1.0.6.tar", max compression
```

## Comparing `strangeworks_braket-1.0.5.tar` & `strangeworks_braket-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      457 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/LICENSE
--rw-r--r--   0        0        0     1394 2023-07-18 13:19:14.111787 strangeworks_braket-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      286 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/__init__.py
--rw-r--r--   0        0        0     7279 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/device.py
--rw-r--r--   0        0        0     8503 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/job.py
--rw-r--r--   0        0        0    10554 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/task.py
--rw-r--r--   0        0        0      691 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/utils/serializer.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-08-03 15:56:06.575252 strangeworks_braket-1.0.6/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-08-03 15:56:06.575252 strangeworks_braket-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1394 2023-08-03 15:56:28.360614 strangeworks_braket-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-08-03 15:56:06.579252 strangeworks_braket-1.0.6/strangeworks_braket/__init__.py
+-rw-r--r--   0        0        0     7283 2023-08-03 15:56:06.579252 strangeworks_braket-1.0.6/strangeworks_braket/device.py
+-rw-r--r--   0        0        0     8503 2023-08-03 15:56:06.579252 strangeworks_braket-1.0.6/strangeworks_braket/job.py
+-rw-r--r--   0        0        0    10554 2023-08-03 15:56:06.579252 strangeworks_braket-1.0.6/strangeworks_braket/task.py
+-rw-r--r--   0        0        0      691 2023-08-03 15:56:06.579252 strangeworks_braket-1.0.6/strangeworks_braket/utils/serializer.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.6/PKG-INFO
```

### Comparing `strangeworks_braket-1.0.5/LICENSE` & `strangeworks_braket-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.5/pyproject.toml` & `strangeworks_braket-1.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-braket"
-version = "1.0.5"
+version = "1.0.6"
 description = "Strangeworks Braket SDK extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_braket"},
 ]
```

### Comparing `strangeworks_braket-1.0.5/strangeworks_braket/device.py` & `strangeworks_braket-1.0.6/strangeworks_braket/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import json
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import strangeworks as sw
 from braket.annealing.problem import Problem
 from braket.aws.aws_device import Device
 from braket.circuits import Circuit
 from braket.device_schema import DeviceCapabilities
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.tasks.quantum_task import QuantumTask
 from braket.tasks.quantum_task_batch import QuantumTaskBatch
+from strangeworks_core.errors.error import StrangeworksError
 
 from strangeworks_braket.job import StrangeworksQuantumJob
 from strangeworks_braket.task import StrangeworksQuantumTask
 from strangeworks_braket.utils.serializer import pickle_deserializer
 
 
 class StrangeworksDevice(Device):
@@ -122,24 +123,22 @@
                 )
             )
 
         return devices
 
     def run_batch(
         self,
-        task_specifications: Circuit | Problem | List[Circuit | Problem],
+        task_specifications: Circuit | Problem | list[Circuit | Problem],
         shots: int | None,
         max_parallel: int | None,
-        inputs: Dict[str, float] | List[Dict[str, float]] | None,
+        inputs: Dict[str, float] | list[Dict[str, float]] | None,
         *args,
         **kwargs,
     ) -> QuantumTaskBatch:
-        return super().run_batch(
-            task_specifications, shots, max_parallel, inputs, *args, **kwargs
-        )
+        raise StrangeworksError("currently not implemented/supported")
 
     @property
     def properties(self) -> DeviceCapabilities:
         if self._properties is None:
             payload = {
                 "aws_device_arn": self.arn,
             }
```

### Comparing `strangeworks_braket-1.0.5/strangeworks_braket/job.py` & `strangeworks_braket-1.0.6/strangeworks_braket/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.5/strangeworks_braket/task.py` & `strangeworks_braket-1.0.6/strangeworks_braket/task.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.5/strangeworks_braket/utils/serializer.py` & `strangeworks_braket-1.0.6/strangeworks_braket/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.5/PKG-INFO` & `strangeworks_braket-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-braket
-Version: 1.0.5
+Version: 1.0.6
 Summary: Strangeworks Braket SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<3.11.4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

