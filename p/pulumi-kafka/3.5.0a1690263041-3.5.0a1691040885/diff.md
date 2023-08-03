# Comparing `tmp/pulumi_kafka-3.5.0a1690263041.tar.gz` & `tmp/pulumi_kafka-3.5.0a1691040885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.5.0a1690263041.tar", last modified: Tue Jul 25 05:39:42 2023, max compression
+gzip compressed data, was "pulumi_kafka-3.5.0a1691040885.tar", last modified: Thu Aug  3 05:47:28 2023, max compression
```

## Comparing `pulumi_kafka-3.5.0a1690263041.tar` & `pulumi_kafka-3.5.0a1691040885.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:39:42.796289 pulumi_kafka-3.5.0a1690263041/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-25 05:39:42.796289 pulumi_kafka-3.5.0a1690263041/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:39:42.792289 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:39:42.796289 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:39:42.796289 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:39:42.796289 pulumi_kafka-3.5.0a1690263041/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-25 05:39:42.000000 pulumi_kafka-3.5.0a1690263041/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:47:28.081592 pulumi_kafka-3.5.0a1691040885/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-03 05:47:28.081592 pulumi_kafka-3.5.0a1691040885/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:47:28.081592 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:47:28.081592 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:47:28.081592 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-03 05:47:28.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-03 05:47:28.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:47:28.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:47:28.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 05:47:28.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 05:47:28.000000 pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 05:47:28.081592 pulumi_kafka-3.5.0a1691040885/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-03 05:47:27.000000 pulumi_kafka-3.5.0a1691040885/setup.py
```

### Comparing `pulumi_kafka-3.5.0a1690263041/PKG-INFO` & `pulumi_kafka-3.5.0a1691040885/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.5.0a1690263041
+Version: 3.5.0a1691040885
 Summary: A Pulumi package for creating and managing Kafka.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi kafka
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.5.0a1690263041/README.md` & `pulumi_kafka-3.5.0a1691040885/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/__init__.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/acl.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/provider.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/quota.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka/topic.py` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-kafka
-Version: 3.5.0a1690263041
+Version: 3.5.0a1691040885
 Summary: A Pulumi package for creating and managing Kafka.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi kafka
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.5.0a1690263041/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.5.0a1691040885/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1690263041/setup.py` & `pulumi_kafka-3.5.0a1691040885/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.5.0a1690263041"
-PLUGIN_VERSION = "3.5.0-alpha.1690263041+ddd18138"
+VERSION = "3.5.0a1691040885"
+PLUGIN_VERSION = "3.5.0-alpha.1691040885+57f96087"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'kafka', PLUGIN_VERSION])
         except OSError as error:
```

