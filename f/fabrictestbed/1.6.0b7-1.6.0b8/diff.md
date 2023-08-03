# Comparing `tmp/fabrictestbed-1.6.0b7.tar.gz` & `tmp/fabrictestbed-1.6.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.6.0b7.tar", last modified: Wed Jul 26 18:51:01 2023, max compression
+gzip compressed data, was "fabrictestbed-1.6.0b8.tar", last modified: Wed Jul 26 20:20:30 2023, max compression
```

## Comparing `fabrictestbed-1.6.0b7.tar` & `fabrictestbed-1.6.0b8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b7/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b7/LICENSE
--rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b7/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b7/README.md
--rw-r--r--   0        0        0       24 2023-07-26 14:20:56.916539 fabrictestbed-1.6.0b7/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b7/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    26823 2023-07-26 18:36:12.647647 fabrictestbed-1.6.0b7/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b7/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b7/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b7/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    22416 2023-07-26 18:28:39.429612 fabrictestbed-1.6.0b7/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b7/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1547 2023-07-26 18:11:43.403641 fabrictestbed-1.6.0b7/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     1693 2023-07-26 18:12:28.124750 fabrictestbed-1.6.0b7/fabrictestbed/util/utils.py
--rw-r--r--   0        0        0     1073 2023-07-26 18:49:56.349934 fabrictestbed-1.6.0b7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b7/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b7/test/test_cli.py
--rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b8/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b8/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b8/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b8/README.md
+-rw-r--r--   0        0        0       50 2023-07-26 20:20:23.437529 fabrictestbed-1.6.0b8/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b8/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    26823 2023-07-26 18:36:12.647647 fabrictestbed-1.6.0b8/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b8/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b8/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b8/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    22416 2023-07-26 18:28:39.429612 fabrictestbed-1.6.0b8/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b8/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-26 18:11:43.403641 fabrictestbed-1.6.0b8/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1693 2023-07-26 18:12:28.124750 fabrictestbed-1.6.0b8/fabrictestbed/util/utils.py
+-rw-r--r--   0        0        0     1073 2023-07-26 20:20:04.988280 fabrictestbed-1.6.0b8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b8/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b8/test/test_cli.py
+-rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b8/PKG-INFO
```

### Comparing `fabrictestbed-1.6.0b7/.gitignore` & `fabrictestbed-1.6.0b8/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/LICENSE` & `fabrictestbed-1.6.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/README.md` & `fabrictestbed-1.6.0b8/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/fabrictestbed/cli/cli.py` & `fabrictestbed-1.6.0b8/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.6.0b8/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.6.0b8/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.6.0b8/fabrictestbed/slice_manager/slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/fabrictestbed/util/constants.py` & `fabrictestbed-1.6.0b8/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/fabrictestbed/util/utils.py` & `fabrictestbed-1.6.0b8/fabrictestbed/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/pyproject.toml` & `fabrictestbed-1.6.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dynamic = ["version"]
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
-    "fabric-credmgr-client==1.6.0b8",
+    "fabric-credmgr-client==1.6.0b9",
     "fabric-orchestrator-client==1.6.0b3",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
```

### Comparing `fabrictestbed-1.6.0b7/test/test_cli.py` & `fabrictestbed-1.6.0b8/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b7/PKG-INFO` & `fabrictestbed-1.6.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.6.0b7
+Version: 1.6.0b8
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
-Requires-Dist: fabric-credmgr-client==1.6.0b8
+Requires-Dist: fabric-credmgr-client==1.6.0b9
 Requires-Dist: fabric-orchestrator-client==1.6.0b3
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
```

