# Comparing `tmp/pulumi_slack-0.4.3a1690910723.tar.gz` & `tmp/pulumi_slack-0.4.3a1691044596.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.3a1690910723.tar", last modified: Tue Aug  1 17:29:18 2023, max compression
+gzip compressed data, was "pulumi_slack-0.4.3a1691044596.tar", last modified: Thu Aug  3 06:50:59 2023, max compression
```

## Comparing `pulumi_slack-0.4.3a1690910723.tar` & `pulumi_slack-0.4.3a1691044596.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:29:18.655189 pulumi_slack-0.4.3a1690910723/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 17:29:18.655189 pulumi_slack-0.4.3a1690910723/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:29:18.655189 pulumi_slack-0.4.3a1690910723/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:29:18.655189 pulumi_slack-0.4.3a1690910723/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:29:18.655189 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:29:18.655189 pulumi_slack-0.4.3a1690910723/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-01 17:29:18.000000 pulumi_slack-0.4.3a1690910723/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:50:59.193387 pulumi_slack-0.4.3a1691044596/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-03 06:50:59.193387 pulumi_slack-0.4.3a1691044596/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:50:59.193387 pulumi_slack-0.4.3a1691044596/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:50:59.193387 pulumi_slack-0.4.3a1691044596/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:50:59.193387 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-03 06:50:59.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-03 06:50:59.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:50:59.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:50:59.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 06:50:59.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 06:50:59.000000 pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:50:59.193387 pulumi_slack-0.4.3a1691044596/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-03 06:50:58.000000 pulumi_slack-0.4.3a1691044596/setup.py
```

### Comparing `pulumi_slack-0.4.3a1690910723/PKG-INFO` & `pulumi_slack-0.4.3a1691044596/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.3a1690910723
+Version: 0.4.3a1691044596
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_slack-0.4.3a1690910723/README.md` & `pulumi_slack-0.4.3a1691044596/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/__init__.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/conversation.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/get_conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/get_user.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/get_usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/provider.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.3a1691044596/pulumi_slack/usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-slack
-Version: 0.4.3a1690910723
+Version: 0.4.3a1691044596
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_slack-0.4.3a1690910723/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.3a1691044596/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690910723/setup.py` & `pulumi_slack-0.4.3a1691044596/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.3a1690910723"
-PLUGIN_VERSION = "0.4.3-alpha.1690910723+530d0de2"
+VERSION = "0.4.3a1691044596"
+PLUGIN_VERSION = "0.4.3-alpha.1691044596+7d53565d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'slack', PLUGIN_VERSION])
         except OSError as error:
```

