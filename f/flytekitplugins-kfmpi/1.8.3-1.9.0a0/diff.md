# Comparing `tmp/flytekitplugins-kfmpi-1.8.3.tar.gz` & `tmp/flytekitplugins-kfmpi-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfmpi-1.8.3.tar", last modified: Thu Aug  3 17:08:14 2023, max compression
+gzip compressed data, was "flytekitplugins-kfmpi-1.9.0a0.tar", last modified: Thu Jul 20 18:58:20 2023, max compression
```

## Comparing `flytekitplugins-kfmpi-1.8.3.tar` & `flytekitplugins-kfmpi-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:14.444342 flytekitplugins-kfmpi-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 17:08:14.444342 flytekitplugins-kfmpi-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-03 17:07:50.000000 flytekitplugins-kfmpi-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:14.444342 flytekitplugins-kfmpi-1.8.3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:14.444342 flytekitplugins-kfmpi-1.8.3/flytekitplugins/kfmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 17:07:50.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins/kfmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-08-03 17:07:50.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins/kfmpi/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:14.444342 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 17:08:14.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-03 17:08:14.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:08:14.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:14.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 17:08:14.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:14.000000 flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:08:14.444342 flytekitplugins-kfmpi-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-03 17:08:08.000000 flytekitplugins-kfmpi-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.652692 flytekitplugins-kfmpi-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 18:58:20.652692 flytekitplugins-kfmpi-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 18:57:54.000000 flytekitplugins-kfmpi-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.648692 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.652692 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins/kfmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 18:57:54.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins/kfmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-20 18:57:54.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins/kfmpi/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.652692 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 18:58:20.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-20 18:58:20.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:20.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:20.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 18:58:20.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:20.000000 flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:20.652692 flytekitplugins-kfmpi-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-20 18:58:12.000000 flytekitplugins-kfmpi-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-kfmpi-1.8.3/PKG-INFO` & `flytekitplugins-kfmpi-1.9.0a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.6
```

### Comparing `flytekitplugins-kfmpi-1.8.3/flytekitplugins_kfmpi.egg-info/PKG-INFO` & `flytekitplugins-kfmpi-1.9.0a0/flytekitplugins_kfmpi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.6
```

### Comparing `flytekitplugins-kfmpi-1.8.3/setup.py` & `flytekitplugins-kfmpi-1.9.0a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup
 
 PLUGIN_NAME = "kfmpi"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit>=1.6.1,<2.0.0"]
+plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "flyteidl>=0.21.4"]
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based MPI plugin for flytekit",
     namespace_packages=["flytekitplugins"],
     packages=[f"flytekitplugins.{PLUGIN_NAME}"],
     install_requires=plugin_requires,
     license="apache2",
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

