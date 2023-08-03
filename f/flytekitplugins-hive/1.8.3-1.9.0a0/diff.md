# Comparing `tmp/flytekitplugins-hive-1.8.3.tar.gz` & `tmp/flytekitplugins-hive-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-hive-1.8.3.tar", last modified: Thu Aug  3 17:08:13 2023, max compression
+gzip compressed data, was "flytekitplugins-hive-1.9.0a0.tar", last modified: Thu Jul 20 18:58:19 2023, max compression
```

## Comparing `flytekitplugins-hive-1.8.3.tar` & `flytekitplugins-hive-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:13.296314 flytekitplugins-hive-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 17:08:13.296314 flytekitplugins-hive-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-03 17:07:50.000000 flytekitplugins-hive-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:13.296314 flytekitplugins-hive-1.8.3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:13.296314 flytekitplugins-hive-1.8.3/flytekitplugins/hive/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 17:07:50.000000 flytekitplugins-hive-1.8.3/flytekitplugins/hive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-08-03 17:07:50.000000 flytekitplugins-hive-1.8.3/flytekitplugins/hive/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:13.296314 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 17:08:13.000000 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-03 17:08:13.000000 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:08:13.000000 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:13.000000 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 17:08:13.000000 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:13.000000 flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:08:13.296314 flytekitplugins-hive-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-03 17:08:08.000000 flytekitplugins-hive-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.172678 flytekitplugins-hive-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 18:58:19.172678 flytekitplugins-hive-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 18:57:54.000000 flytekitplugins-hive-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.168677 flytekitplugins-hive-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.168677 flytekitplugins-hive-1.9.0a0/flytekitplugins/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 18:57:54.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-20 18:57:54.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins/hive/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.172678 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 18:58:19.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 18:58:19.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:19.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:19.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 18:58:19.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:19.000000 flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:19.172678 flytekitplugins-hive-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-20 18:58:12.000000 flytekitplugins-hive-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-hive-1.8.3/PKG-INFO` & `flytekitplugins-hive-1.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-hive
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: This package holds Hive plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-hive-1.8.3/flytekitplugins/hive/task.py` & `flytekitplugins-hive-1.9.0a0/flytekitplugins/hive/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-hive-1.8.3/flytekitplugins_hive.egg-info/PKG-INFO` & `flytekitplugins-hive-1.9.0a0/flytekitplugins_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-hive
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: This package holds Hive plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-hive-1.8.3/setup.py` & `flytekitplugins-hive-1.9.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "hive"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds Hive plugins for flytekit",
```

