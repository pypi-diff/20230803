# Comparing `tmp/pulumi_rabbitmq-3.4.0a1690968008.tar.gz` & `tmp/pulumi_rabbitmq-3.4.0a1691043773.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rabbitmq-3.4.0a1690968008.tar", last modified: Wed Aug  2 09:24:22 2023, max compression
+gzip compressed data, was "pulumi_rabbitmq-3.4.0a1691043773.tar", last modified: Thu Aug  3 06:42:21 2023, max compression
```

## Comparing `pulumi_rabbitmq-3.4.0a1690968008.tar` & `pulumi_rabbitmq-3.4.0a1691043773.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:24:22.027804 pulumi_rabbitmq-3.4.0a1690968008/
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-02 09:24:22.027804 pulumi_rabbitmq-3.4.0a1690968008/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:24:22.027804 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:24:22.027804 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/federation_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/get_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/get_v_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/operator_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/shovel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/topic_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/v_host.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:24:22.027804 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-02 09:24:22.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-02 09:24:22.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:24:22.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:24:22.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 09:24:22.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 09:24:22.000000 pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:24:22.027804 pulumi_rabbitmq-3.4.0a1690968008/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-02 09:24:21.000000 pulumi_rabbitmq-3.4.0a1690968008/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:42:21.217446 pulumi_rabbitmq-3.4.0a1691043773/
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-03 06:42:21.217446 pulumi_rabbitmq-3.4.0a1691043773/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:42:21.213446 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:42:21.217446 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/federation_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/get_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/get_v_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/operator_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/shovel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/topic_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/v_host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:42:21.217446 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:42:21.217446 pulumi_rabbitmq-3.4.0a1691043773/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 06:42:21.000000 pulumi_rabbitmq-3.4.0a1691043773/setup.py
```

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1691043773/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1690968008
+Version: 3.4.0a1691043773
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi rabbitmq
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/README.md` & `pulumi_rabbitmq-3.4.0a1691043773/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/__init__.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/_inputs.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/_utilities.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/binding.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/config/vars.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/exchange.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/federation_upstream.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/federation_upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/get_exchange.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/get_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/get_user.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/get_v_host.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/get_v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/operator_policy.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/operator_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/outputs.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/permissions.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/policy.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/provider.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/queue.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/shovel.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/shovel.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/topic_permissions.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/topic_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/user.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq/v_host.py` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq/v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rabbitmq
-Version: 3.4.0a1690968008
+Version: 3.4.0a1691043773
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi rabbitmq
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/pulumi_rabbitmq.egg-info/SOURCES.txt` & `pulumi_rabbitmq-3.4.0a1691043773/pulumi_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1690968008/setup.py` & `pulumi_rabbitmq-3.4.0a1691043773/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.4.0a1690968008"
-PLUGIN_VERSION = "3.4.0-alpha.1690968008+0fff9f6e"
+VERSION = "3.4.0a1691043773"
+PLUGIN_VERSION = "3.4.0-alpha.1691043773+9f571849"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rabbitmq', PLUGIN_VERSION])
         except OSError as error:
```

