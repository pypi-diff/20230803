# Comparing `tmp/PythonMetaTrader5-1.0.4.tar.gz` & `tmp/PythonMetaTrader5-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonMetaTrader5-1.0.4.tar", last modified: Thu Aug  3 00:10:20 2023, max compression
+gzip compressed data, was "PythonMetaTrader5-1.0.5.tar", last modified: Thu Aug  3 00:23:13 2023, max compression
```

## Comparing `PythonMetaTrader5-1.0.4.tar` & `PythonMetaTrader5-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 00:10:20.131262 PythonMetaTrader5-1.0.4/
--rw-rw-rw-   0        0        0     3904 2023-08-03 00:10:20.131262 PythonMetaTrader5-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3396 2023-08-03 00:09:10.000000 PythonMetaTrader5-1.0.4/README.md
--rw-rw-rw-   0        0        0      112 2023-08-03 00:09:10.000000 PythonMetaTrader5-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      670 2023-08-03 00:10:20.133216 PythonMetaTrader5-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 00:10:20.109784 PythonMetaTrader5-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 00:10:20.119546 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5/
--rw-rw-rw-   0        0        0    11009 2023-08-03 00:09:11.000000 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:10:20.129310 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5.egg-info/
--rw-rw-rw-   0        0        0     3904 2023-08-03 00:10:20.000000 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-08-03 00:10:20.000000 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 00:10:20.000000 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-03 00:10:20.000000 PythonMetaTrader5-1.0.4/src/PythonMetaTrader5.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 00:23:13.408762 PythonMetaTrader5-1.0.5/
+-rw-rw-rw-   0        0        0     3904 2023-08-03 00:23:13.409739 PythonMetaTrader5-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3396 2023-08-03 00:09:10.000000 PythonMetaTrader5-1.0.5/README.md
+-rw-rw-rw-   0        0        0      112 2023-08-03 00:09:10.000000 PythonMetaTrader5-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      670 2023-08-03 00:23:13.410716 PythonMetaTrader5-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 00:23:13.389050 PythonMetaTrader5-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 00:23:13.397837 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5/
+-rw-rw-rw-   0        0        0    11009 2023-08-03 00:09:11.000000 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:23:13.406810 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5.egg-info/
+-rw-rw-rw-   0        0        0     3904 2023-08-03 00:23:13.000000 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-08-03 00:23:13.000000 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 00:23:13.000000 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-03 00:23:13.000000 PythonMetaTrader5-1.0.5/src/PythonMetaTrader5.egg-info/top_level.txt
```

### Comparing `PythonMetaTrader5-1.0.4/PKG-INFO` & `PythonMetaTrader5-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonMetaTrader5
-Version: 1.0.4
+Version: 1.0.5
 Summary: Connect MT5 with Python
 Home-page: https://github.com/Akinzou/MetaTrader5-Python
 Author: Wiktor Jelen
 Author-email: wiktorjn@gmail.com
 Project-URL: Bug Tracker, https://github.com/Akinzou/MetaTrader5-Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PythonMetaTrader5-1.0.4/README.md` & `PythonMetaTrader5-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PythonMetaTrader5-1.0.4/setup.cfg` & `PythonMetaTrader5-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7974 686f 6e4d 6574 6154 7261   = PythonMetaTra
 00000020: 6465 7235 0d0a 7665 7273 696f 6e20 3d20  der5..version = 
-00000030: 312e 302e 340d 0a61 7574 686f 7220 3d20  1.0.4..author = 
+00000030: 312e 302e 350d 0a61 7574 686f 7220 3d20  1.0.5..author = 
 00000040: 5769 6b74 6f72 204a 656c 656e 0d0a 6175  Wiktor Jelen..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2077 696b  thor_email = wik
 00000060: 746f 726a 6e40 676d 6169 6c2e 636f 6d0d  torjn@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2043  .description = C
 00000080: 6f6e 6e65 6374 204d 5435 2077 6974 6820  onnect MT5 with 
 00000090: 5079 7468 6f6e 0d0a 6c6f 6e67 5f64 6573  Python..long_des
 000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
```

### Comparing `PythonMetaTrader5-1.0.4/src/PythonMetaTrader5/__init__.py` & `PythonMetaTrader5-1.0.5/src/PythonMetaTrader5/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonMetaTrader5-1.0.4/src/PythonMetaTrader5.egg-info/PKG-INFO` & `PythonMetaTrader5-1.0.5/src/PythonMetaTrader5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonMetaTrader5
-Version: 1.0.4
+Version: 1.0.5
 Summary: Connect MT5 with Python
 Home-page: https://github.com/Akinzou/MetaTrader5-Python
 Author: Wiktor Jelen
 Author-email: wiktorjn@gmail.com
 Project-URL: Bug Tracker, https://github.com/Akinzou/MetaTrader5-Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

