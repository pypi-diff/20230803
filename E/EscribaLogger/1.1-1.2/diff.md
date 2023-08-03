# Comparing `tmp/escribalogger-1.1.tar.gz` & `tmp/escribalogger-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escribalogger-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "escribalogger-1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `escribalogger-1.1.tar` & `escribalogger-1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3852 2023-07-16 20:17:55.333708 escribalogger-1.1/README.md
--rw-r--r--   0        0        0      902 2023-07-16 22:39:27.743937 escribalogger-1.1/pyproject.toml
--rw-r--r--   0        0        0      267 2023-07-15 23:49:49.033618 escribalogger-1.1/src/EscribaLogger/DPSingleton.py
--rw-r--r--   0        0        0     3606 2023-07-16 18:25:32.945977 escribalogger-1.1/src/EscribaLogger/Log.py
--rw-r--r--   0        0        0       43 2023-07-15 23:53:52.869434 escribalogger-1.1/src/EscribaLogger/__init__.py
--rw-r--r--   0        0        0     1706 2023-07-16 18:27:07.438466 escribalogger-1.1/src/EscribaLogger/drivers.py
--rw-r--r--   0        0        0      286 2023-07-16 15:30:58.059955 escribalogger-1.1/src/EscribaLogger/process_extra_context.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 escribalogger-1.1/PKG-INFO
+-rw-r--r--   0        0        0     3852 2023-07-16 20:17:55.333708 escribalogger-1.2/README.md
+-rw-r--r--   0        0        0      902 2023-08-03 13:09:01.789713 escribalogger-1.2/pyproject.toml
+-rw-r--r--   0        0        0      267 2023-07-15 23:49:49.033618 escribalogger-1.2/src/EscribaLogger/DPSingleton.py
+-rw-r--r--   0        0        0     3606 2023-07-16 18:25:32.945977 escribalogger-1.2/src/EscribaLogger/Log.py
+-rw-r--r--   0        0        0       43 2023-07-15 23:53:52.869434 escribalogger-1.2/src/EscribaLogger/__init__.py
+-rw-r--r--   0        0        0     2254 2023-08-03 12:31:45.481615 escribalogger-1.2/src/EscribaLogger/drivers.py
+-rw-r--r--   0        0        0      286 2023-07-16 15:30:58.059955 escribalogger-1.2/src/EscribaLogger/process_extra_context.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 escribalogger-1.2/PKG-INFO
```

### Comparing `escribalogger-1.1/README.md` & `escribalogger-1.2/README.md`

 * *Files identical despite different names*

### Comparing `escribalogger-1.1/pyproject.toml` & `escribalogger-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "EscribaLogger"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Thiago Santa Clara Pereira", email="strovsk@outlook.com" },
 ]
 keywords = ["logging", "logger", "log", "logs", "drivers"]
 description = "A fast 'read to use' Logging system which provides stdout/file/custom stream with easy syntax and operation. It's a very simple approach of Laravel drivers sorts, by the way, handlers ands drivers are both the same"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `escribalogger-1.1/src/EscribaLogger/Log.py` & `escribalogger-1.2/src/EscribaLogger/Log.py`

 * *Files identical despite different names*

### Comparing `escribalogger-1.1/src/EscribaLogger/drivers.py` & `escribalogger-1.2/src/EscribaLogger/drivers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import logging
 import os
 from datetime import datetime
 from typing import Optional, TypedDict
 
+import graypy
 from rich.highlighter import Highlighter
 from rich.logging import RichHandler
 from rich.text import Text
 
 
 class DriverOption(TypedDict):
     file_location: Optional[str]
+    graylog_host: Optional[str]
+    graylog_port: Optional[int]
+    graylog_protocol: Optional[str]
 
 
 def driver_file(driver_option: DriverOption = None):
     if not driver_option:
         driver_option = {"file_location": "logs"}
 
     formatter_string = "[%(asctime)s] "
@@ -51,7 +55,18 @@
 
     formatter_string = "%(name)s - %(message)s"
 
     formatter = logging.Formatter(formatter_string)
     rich_handler.setFormatter(formatter)
 
     return rich_handler
+
+
+def driver_graylog(driver_options: DriverOption = None):
+    graylog_host = driver_options.get("graylog_host", "localhost")
+    graylog_port = driver_options.get("graylog_port", 12201)
+
+    formatter_string = "%(name)s.%(levelname)s - %(message)s"
+    formatter = logging.Formatter(formatter_string)
+    stream = graypy.GELFHTTPHandler(graylog_host, graylog_port)
+    stream.setFormatter(formatter)
+    return stream
```

### Comparing `escribalogger-1.1/PKG-INFO` & `escribalogger-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EscribaLogger
-Version: 1.1
+Version: 1.2
 Summary: A fast 'read to use' Logging system which provides stdout/file/custom stream with easy syntax and operation. It's a very simple approach of Laravel drivers sorts, by the way, handlers ands drivers are both the same
 Keywords: logging,logger,log,logs,drivers
 Author-email: Thiago Santa Clara Pereira <strovsk@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

