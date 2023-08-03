# Comparing `tmp/fcw_service-0.4.3.tar.gz` & `tmp/fcw_service-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcw_service-0.4.3.tar", max compression
+gzip compressed data, was "fcw_service-0.4.4.tar", max compression
```

## Comparing `fcw_service-0.4.3.tar` & `fcw_service-0.4.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.110833 fcw_service-0.4.3/fcw_service/__init__.py
--rw-r--r--   0        0        0     4949 2023-07-19 16:26:45.757392 fcw_service-0.4.3/fcw_service/collision_worker.py
--rw-r--r--   0        0        0    10596 2023-07-19 16:36:40.134861 fcw_service-0.4.3/fcw_service/interface.py
--rw-r--r--   0        0        0      778 2023-07-19 17:36:57.093772 fcw_service-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      236 2023-07-19 16:34:58.047966 fcw_service-0.4.3/README.md
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 fcw_service-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.110833 fcw_service-0.4.4/fcw_service/__init__.py
+-rw-r--r--   0        0        0     4949 2023-07-19 16:26:45.757392 fcw_service-0.4.4/fcw_service/collision_worker.py
+-rw-r--r--   0        0        0    10790 2023-08-03 15:32:41.899142 fcw_service-0.4.4/fcw_service/interface.py
+-rw-r--r--   0        0        0      778 2023-08-03 15:37:31.214535 fcw_service-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      236 2023-07-19 16:34:58.047966 fcw_service-0.4.4/README.md
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 fcw_service-0.4.4/PKG-INFO
```

### Comparing `fcw_service-0.4.3/fcw_service/collision_worker.py` & `fcw_service-0.4.4/fcw_service/collision_worker.py`

 * *Files identical despite different names*

### Comparing `fcw_service-0.4.3/fcw_service/interface.py` & `fcw_service-0.4.4/fcw_service/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import threading
 import cv2
 from flask import Flask
 import logging
 import sys
 
 from fcw_service.collision_worker import CollisionWorker
+from fcw_core.yolo_detector import YOLODetector
 
 from era_5g_interface.task_handler import TaskHandler
 from era_5g_interface.task_handler_internal_q import TaskHandlerInternalQ
 from era_5g_interface.h264_decoder import H264Decoder
 import era_5g_interface.interface_helpers
 from era_5g_interface.interface_helpers import HeartBeatSender
 from era_5g_interface.dataclasses.control_command import ControlCommand, ControlCmdType
@@ -304,14 +305,18 @@
 
 def main(args=None):
     parser = argparse.ArgumentParser(description='Standalone variant of Forward Collision Warning NetApp')
     args = parser.parse_args()
 
     logger.info(f"The size of the queue set to: {NETAPP_INPUT_QUEUE}")
 
+    logger.info("Initializing default object detector for faster first startup")
+    detector = YOLODetector.from_dict({})
+    del detector
+
     # runs the flask server
     # allow_unsafe_werkzeug needs to be true to run inside the docker
     # TODO: use better webserver
     app.run(port=NETAPP_PORT, host='0.0.0.0')
 
 
 if __name__ == '__main__':
```

### Comparing `fcw_service-0.4.3/pyproject.toml` & `fcw_service-0.4.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fcw-service"
-version = "0.4.3"
+version = "0.4.4"
 description = "Early collision warning Network Application for Transportation use case - service part"
 authors = ["Petr Kleparnik <pkleparnik@cognitechna.cz>", "Roman Juranek <rjuranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CollisionWarningService"
 packages = [{include = "fcw_service"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fcw_service-0.4.3/PKG-INFO` & `fcw_service-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcw-service
-Version: 0.4.3
+Version: 0.4.4
 Summary: Early collision warning Network Application for Transportation use case - service part
 Home-page: https://github.com/5G-ERA/CollisionWarningService
 Author: Petr Kleparnik
 Author-email: pkleparnik@cognitechna.cz
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

