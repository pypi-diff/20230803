# Comparing `tmp/snitch-protos-0.0.55.tar.gz` & `tmp/snitch-protos-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.55.tar", last modified: Mon Jul 31 01:31:56 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.56.tar", last modified: Thu Aug  3 17:21:01 2023, max compression
```

## Comparing `snitch-protos-0.0.55.tar` & `snitch-protos-0.0.56.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    34904 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.55/PKG-INFO` & `snitch-protos-0.0.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.55
+Version: 0.0.56
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.55/setup.py` & `snitch-protos-0.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.55',
+    version='0.0.56',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.55/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.56/snitch_protos/protos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,17 @@
     """
     Name of the component the SDK is interacting with (ie. kafka-$topic-name)
     """
 
     operation_type: "OperationType" = betterproto.enum_field(3)
     """Consumer or Producer"""
 
+    operation_name: str = betterproto.string_field(4)
+    """Name for the consumer or producer"""
+
 
 @dataclass(eq=False, repr=False)
 class Pipeline(betterproto.Message):
     """
     Pipeline is a structure that holds one or more pipeline steps. This
     structure is intended to be immutable; clients are expected to generate
     WASMRequest's that contain a pipeline step.
```

### Comparing `snitch-protos-0.0.55/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.56/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.55/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.56/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.55
+Version: 0.0.56
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

