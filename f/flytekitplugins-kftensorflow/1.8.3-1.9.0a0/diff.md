# Comparing `tmp/flytekitplugins-kftensorflow-1.8.3.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.8.3.tar", last modified: Thu Aug  3 17:08:15 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.9.0a0.tar", last modified: Thu Jul 20 18:58:21 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.8.3.tar` & `flytekitplugins-kftensorflow-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:15.208361 flytekitplugins-kftensorflow-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-03 17:08:15.208361 flytekitplugins-kftensorflow-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-03 17:07:50.000000 flytekitplugins-kftensorflow-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:15.208361 flytekitplugins-kftensorflow-1.8.3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:15.208361 flytekitplugins-kftensorflow-1.8.3/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 17:07:50.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-08-03 17:07:50.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:15.208361 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-03 17:08:15.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-03 17:08:15.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:08:15.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:15.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:15.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:15.000000 flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:08:15.208361 flytekitplugins-kftensorflow-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-03 17:08:08.000000 flytekitplugins-kftensorflow-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.628701 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-20 18:58:12.000000 flytekitplugins-kftensorflow-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.8.3/PKG-INFO` & `flytekitplugins-kftensorflow-1.9.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.8.3/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.8.3/setup.py` & `flytekitplugins-kftensorflow-1.9.0a0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit>=1.6.1"]
+# TODO: Requirements are missing, add them back in later.
+plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```

