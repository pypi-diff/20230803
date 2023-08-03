# Comparing `tmp/robotcode_debugger-0.48.0.tar.gz` & `tmp/robotcode_debugger-0.49.0.tar.gz`

## Comparing `robotcode_debugger-0.48.0.tar` & `robotcode_debugger-0.49.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    25779 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    64963 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15579 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/README.md
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.48.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    25779 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    64963 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15579 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/README.md
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.49.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.49.0/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/.gitignore` & `robotcode_debugger-0.49.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/LICENSE.txt` & `robotcode_debugger-0.49.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/README.md` & `robotcode_debugger-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.48.0/pyproject.toml` & `robotcode_debugger-0.49.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.48.0",
-  "robotcode-runner==0.48.0",
+  "robotcode-jsonrpc2==0.49.0",
+  "robotcode-runner==0.49.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.48.0/PKG-INFO` & `robotcode_debugger-0.49.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.48.0
+Version: 0.49.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.48.0
-Requires-Dist: robotcode-runner==0.48.0
+Requires-Dist: robotcode-jsonrpc2==0.49.0
+Requires-Dist: robotcode-runner==0.49.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

