# Comparing `tmp/eros_cli-1.0.2.tar.gz` & `tmp/eros_cli-1.0.3.tar.gz`

## Comparing `eros_cli-1.0.2.tar` & `eros_cli-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 eros_cli-1.0.2/tempnotes
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 eros_cli-1.0.2/.github/workflows/build_binary.yml
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 eros_cli-1.0.2/.github/workflows/test_installation.yml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 eros_cli-1.0.2/.vscode/launch.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 eros_cli-1.0.2/docs/diagrams.drawio
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/__main__.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/entrypoint.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/app_cli.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/app_dump.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/app_log.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/app_machine_cli.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/app_perf.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/app_zmq.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/decorators.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/utils/eros_terminal.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/app/utils/transport_status_log.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/transport/drv_tcp.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/transport/drv_uart.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/transport/drv_udp.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 eros_cli-1.0.2/src/eros_cli/transport/drv_zmq.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 eros_cli-1.0.2/.gitignore
--rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 eros_cli-1.0.2/LICENCE
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 eros_cli-1.0.2/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 eros_cli-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 eros_cli-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 eros_cli-1.0.3/tempnotes
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 eros_cli-1.0.3/.github/workflows/build_binary.yml
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 eros_cli-1.0.3/.github/workflows/test_installation.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 eros_cli-1.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 eros_cli-1.0.3/docs/diagrams.drawio
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/__main__.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/entrypoint.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/app_cli.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/app_dump.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/app_log.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/app_machine_cli.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/app_perf.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/app_zmq.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/decorators.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/utils/eros_terminal.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/app/utils/transport_status_log.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/transport/drv_tcp.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/transport/drv_uart.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/transport/drv_udp.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 eros_cli-1.0.3/src/eros_cli/transport/drv_zmq.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 eros_cli-1.0.3/.gitignore
+-rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 eros_cli-1.0.3/LICENCE
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 eros_cli-1.0.3/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 eros_cli-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 eros_cli-1.0.3/PKG-INFO
```

### Comparing `eros_cli-1.0.2/.github/workflows/build_binary.yml` & `eros_cli-1.0.3/.github/workflows/build_binary.yml`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/.github/workflows/test_installation.yml` & `eros_cli-1.0.3/.github/workflows/test_installation.yml`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/.vscode/launch.json` & `eros_cli-1.0.3/.vscode/launch.json`

 * *Files 20% similar despite different names*

```diff
@@ -10,10 +10,29 @@
             "type": "python",
             "request": "launch",
             // "program": "src/eros_cli/entrypoint.py",
             "console": "integratedTerminal",
             "module": "eros_cli.entrypoint",
             "args": ["uart", "log", "--log_failed"],
             "justMyCode": false
+        },
+        {
+            "name": "eros uart cli",
+            "type": "python",
+            "request": "launch",
+            // "program": "src/eros_cli/entrypoint.py",
+            "console": "integratedTerminal",
+            "module": "eros_cli.entrypoint",
+            "args": ["uart", "cli"],
+            "justMyCode": false
+        },
+        {
+            "name": "eros udp cli",
+            "type": "python",
+            "request": "launch",
+            "console": "integratedTerminal",
+            "module": "eros_cli.entrypoint",
+            "args": ["udp --ip 10.172.255.27", "cli"],
+            "justMyCode": false
         }
     ]
 }
```

### Comparing `eros_cli-1.0.2/docs/diagrams.drawio` & `eros_cli-1.0.3/docs/diagrams.drawio`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/entrypoint.py` & `eros_cli-1.0.3/src/eros_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/app_cli.py` & `eros_cli-1.0.3/src/eros_cli/app/app_cli.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/app_dump.py` & `eros_cli-1.0.3/src/eros_cli/app/app_dump.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/app_log.py` & `eros_cli-1.0.3/src/eros_cli/app/app_log.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/app_machine_cli.py` & `eros_cli-1.0.3/src/eros_cli/app/app_machine_cli.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/app_perf.py` & `eros_cli-1.0.3/src/eros_cli/app/app_perf.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/app_zmq.py` & `eros_cli-1.0.3/src/eros_cli/app/app_zmq.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/utils/eros_terminal.py` & `eros_cli-1.0.3/src/eros_cli/app/utils/eros_terminal.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/app/utils/transport_status_log.py` & `eros_cli-1.0.3/src/eros_cli/app/utils/transport_status_log.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/transport/drv_tcp.py` & `eros_cli-1.0.3/src/eros_cli/transport/drv_tcp.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/src/eros_cli/transport/drv_uart.py` & `eros_cli-1.0.3/src/eros_cli/transport/drv_uart.py`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/LICENCE` & `eros_cli-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/README.md` & `eros_cli-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eros_cli-1.0.2/pyproject.toml` & `eros_cli-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
 
 dependencies = [
     "click==8.1.3",
-    "eros-core",
+    "eros-core == 1.0.5",
     "blessed",
     'si-prefix==1.2.2',
     'rich==13.4.2'
 ]
 
 dynamic = ["version"]
```

### Comparing `eros_cli-1.0.2/PKG-INFO` & `eros_cli-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: eros-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package to view EROS logs
 Author-email: Floris Vernieuwe <floris@vernieuwe.eu>
 License-File: LICENCE
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: blessed
 Requires-Dist: click==8.1.3
-Requires-Dist: eros-core
+Requires-Dist: eros-core==1.0.5
 Requires-Dist: rich==13.4.2
 Requires-Dist: si-prefix==1.2.2
 Description-Content-Type: text/markdown
 
 # Eros CLI Interface
 
 This is a terminal based interface to interact with eros. Its built ontop eros-core-python.
```

