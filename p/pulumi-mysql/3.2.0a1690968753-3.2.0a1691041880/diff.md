# Comparing `tmp/pulumi_mysql-3.2.0a1690968753.tar.gz` & `tmp/pulumi_mysql-3.2.0a1691041880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mysql-3.2.0a1690968753.tar", last modified: Wed Aug  2 09:36:35 2023, max compression
+gzip compressed data, was "pulumi_mysql-3.2.0a1691041880.tar", last modified: Thu Aug  3 06:01:45 2023, max compression
```

## Comparing `pulumi_mysql-3.2.0a1690968753.tar` & `pulumi_mysql-3.2.0a1691041880.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:36:35.266232 pulumi_mysql-3.2.0a1690968753/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-02 09:36:35.266232 pulumi_mysql-3.2.0a1690968753/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:36:35.262232 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:36:35.262232 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql/user_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:36:35.262232 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-02 09:36:35.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 09:36:35.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:36:35.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:36:35.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-02 09:36:35.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 09:36:35.000000 pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:36:35.266232 pulumi_mysql-3.2.0a1690968753/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 09:36:34.000000 pulumi_mysql-3.2.0a1690968753/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:01:45.696691 pulumi_mysql-3.2.0a1691041880/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-03 06:01:45.692691 pulumi_mysql-3.2.0a1691041880/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:01:45.692691 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:01:45.692691 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql/user_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:01:45.692691 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:01:45.696691 pulumi_mysql-3.2.0a1691041880/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-03 06:01:45.000000 pulumi_mysql-3.2.0a1691041880/setup.py
```

### Comparing `pulumi_mysql-3.2.0a1690968753/PKG-INFO` & `pulumi_mysql-3.2.0a1691041880/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.2.0a1690968753
+Version: 3.2.0a1691041880
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi mysql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.2.0a1690968753/README.md` & `pulumi_mysql-3.2.0a1691041880/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/__init__.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/_utilities.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/config/vars.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/database.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/grant.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/provider.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/role.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/user.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql/user_password.py` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql/user_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/PKG-INFO` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-mysql
-Version: 3.2.0a1690968753
+Version: 3.2.0a1691041880
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi mysql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.2.0a1690968753/pulumi_mysql.egg-info/SOURCES.txt` & `pulumi_mysql-3.2.0a1691041880/pulumi_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1690968753/setup.py` & `pulumi_mysql-3.2.0a1691041880/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.2.0a1690968753"
-PLUGIN_VERSION = "3.2.0-alpha.1690968753+ec780e18"
+VERSION = "3.2.0a1691041880"
+PLUGIN_VERSION = "3.2.0-alpha.1691041880+aeb4a135"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'mysql', PLUGIN_VERSION])
         except OSError as error:
```

