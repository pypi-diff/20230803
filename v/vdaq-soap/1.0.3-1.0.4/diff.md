# Comparing `tmp/vdaq_soap-1.0.3.tar.gz` & `tmp/vdaq_soap-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdaq_soap-1.0.3.tar", last modified: Fri May 12 08:06:22 2023, max compression
+gzip compressed data, was "vdaq_soap-1.0.4.tar", last modified: Thu Aug  3 15:36:58 2023, max compression
```

## Comparing `vdaq_soap-1.0.3.tar` & `vdaq_soap-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 08:06:22.949044 vdaq_soap-1.0.3/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-05-12 08:06:22.948492 vdaq_soap-1.0.3/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.3/README.md
--rw-r--r--   0 lacasta    (503) staff       (20)      957 2023-05-12 08:06:12.000000 vdaq_soap-1.0.3/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-12 08:06:22.949241 vdaq_soap-1.0.3/setup.cfg
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 08:06:22.945071 vdaq_soap-1.0.3/vdaq_soap/
--rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-05-12 08:06:12.000000 vdaq_soap-1.0.3/vdaq_soap/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.3/vdaq_soap/analyzeHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.3/vdaq_soap/analyzeMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.3/vdaq_soap/data_utils.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    25156 2023-05-12 06:55:29.000000 vdaq_soap-1.0.3/vdaq_soap/soapCheckMadDaq.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2980 2023-05-12 06:51:08.000000 vdaq_soap-1.0.3/vdaq_soap/soapHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3073 2023-05-12 06:55:33.000000 vdaq_soap-1.0.3/vdaq_soap/soapMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3105 2023-05-12 07:44:42.000000 vdaq_soap-1.0.3/vdaq_soap/soapTestChannel.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 08:06:22.948010 vdaq_soap-1.0.3/vdaq_soap.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-05-12 08:06:22.000000 vdaq_soap-1.0.3/vdaq_soap.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-05-12 08:06:22.000000 vdaq_soap-1.0.3/vdaq_soap.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-12 08:06:22.000000 vdaq_soap-1.0.3/vdaq_soap.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      264 2023-05-12 08:06:22.000000 vdaq_soap-1.0.3/vdaq_soap.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-05-12 08:06:22.000000 vdaq_soap-1.0.3/vdaq_soap.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-12 08:06:22.000000 vdaq_soap-1.0.3/vdaq_soap.egg-info/top_level.txt
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-03 15:36:58.991579 vdaq_soap-1.0.4/
+-rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-08-03 15:36:58.991101 vdaq_soap-1.0.4/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.4/README.md
+-rw-r--r--   0 lacasta    (503) staff       (20)      957 2023-08-03 15:34:12.000000 vdaq_soap-1.0.4/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-08-03 15:36:58.991698 vdaq_soap-1.0.4/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-03 15:36:58.987291 vdaq_soap-1.0.4/vdaq_soap/
+-rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-08-03 15:34:12.000000 vdaq_soap-1.0.4/vdaq_soap/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.4/vdaq_soap/analyzeHoldDelay.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.4/vdaq_soap/analyzeMbias.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.4/vdaq_soap/data_utils.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    25156 2023-05-12 06:55:29.000000 vdaq_soap-1.0.4/vdaq_soap/soapCheckMadDaq.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3028 2023-08-03 11:21:38.000000 vdaq_soap-1.0.4/vdaq_soap/soapHoldDelay.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3121 2023-08-03 11:22:53.000000 vdaq_soap-1.0.4/vdaq_soap/soapMbias.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3153 2023-08-03 11:23:40.000000 vdaq_soap-1.0.4/vdaq_soap/soapTestChannel.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-03 15:36:58.990235 vdaq_soap-1.0.4/vdaq_soap.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      264 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/top_level.txt
```

### Comparing `vdaq_soap-1.0.3/PKG-INFO` & `vdaq_soap-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdaq_soap
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of python scripts to control VDaq.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `vdaq_soap-1.0.3/pyproject.toml` & `vdaq_soap-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vdaq_soap"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to control VDaq."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vdaq_soap-1.0.3/vdaq_soap/analyzeHoldDelay.py` & `vdaq_soap-1.0.4/vdaq_soap/analyzeHoldDelay.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.3/vdaq_soap/analyzeMbias.py` & `vdaq_soap-1.0.4/vdaq_soap/analyzeMbias.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.3/vdaq_soap/data_utils.py` & `vdaq_soap-1.0.4/vdaq_soap/data_utils.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.3/vdaq_soap/soapCheckMadDaq.py` & `vdaq_soap-1.0.4/vdaq_soap/soapCheckMadDaq.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.3/vdaq_soap/soapHoldDelay.py` & `vdaq_soap-1.0.4/vdaq_soap/soapHoldDelay.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     the_module = None
     modules = server.getAllModules()
     for md in modules:
         print("Module {}".format(md.name))
         if md.name == options.mid:
             md.setLocal(False, "main")
             the_module = md
+        else:
+            md.setLocal(True, "")
 
     if the_module is None:
         the_module = modules[0]
 
     if the_module is None:
         print("### CheckMadDaq Error: module {} not present")
         sys.exit()
```

### Comparing `vdaq_soap-1.0.3/vdaq_soap/soapMbias.py` & `vdaq_soap-1.0.4/vdaq_soap/soapMbias.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     the_module = None
     modules = server.getAllModules()
     for md in modules:
         print("Module {}".format(md.name))
         if md.name == options.mid:
             md.setLocal(False, "main")
             the_module = md
+        else:
+            md.setLocal(True, "")
 
     if the_module is None:
         the_module = modules[0]
 
     if the_module is None:
         print("### CheckMadDaq Error: module {} not present")
         sys.exit()
```

### Comparing `vdaq_soap-1.0.3/vdaq_soap/soapTestChannel.py` & `vdaq_soap-1.0.4/vdaq_soap/soapTestChannel.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     the_module = None
     modules = server.getAllModules()
     for md in modules:
         print("Module {}".format(md.name))
         if md.name == options.mid:
             md.setLocal(False, "main")
             the_module = md
+        else:
+            md.setLocal(True, "")
 
     if the_module is None:
         the_module = modules[0]
 
     if the_module is None:
         print("### CheckMadDaq Error: module {} not present")
         sys.exit()
```

### Comparing `vdaq_soap-1.0.3/vdaq_soap.egg-info/PKG-INFO` & `vdaq_soap-1.0.4/vdaq_soap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdaq-soap
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of python scripts to control VDaq.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

