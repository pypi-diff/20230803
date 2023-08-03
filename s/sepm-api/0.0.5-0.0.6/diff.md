# Comparing `tmp/sepm-api-0.0.5.tar.gz` & `tmp/sepm-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sepm-api-0.0.5.tar", last modified: Fri Jun 23 23:31:38 2023, max compression
+gzip compressed data, was "/Users/aalmero/source/python3-projects/sepm-api/dist/.tmp-3r9c7k1z/sepm-api-0.0.6.tar", last modified: Thu Aug  3 19:48:33 2023, max compression
```

## Comparing `sepm-api-0.0.5.tar` & `sepm-api-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.252851 sepm-api-0.0.5/
--rw-r--r--   0 aalmero    (501) staff       (20)     1077 2023-01-23 20:35:31.000000 sepm-api-0.0.5/LICENSE
--rw-r--r--   0 aalmero    (501) staff       (20)     1911 2023-06-23 23:31:38.252460 sepm-api-0.0.5/PKG-INFO
--rw-r--r--   0 aalmero    (501) staff       (20)     1524 2023-06-23 22:55:18.000000 sepm-api-0.0.5/README.rst
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.211078 sepm-api-0.0.5/sepm/
--rw-r--r--   0 aalmero    (501) staff       (20)     5536 2023-06-23 22:49:41.000000 sepm-api-0.0.5/sepm/__init__.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1090 2023-04-26 19:25:54.000000 sepm-api-0.0.5/sepm/config.py
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.247334 sepm-api-0.0.5/sepm/endpoints/
--rw-r--r--   0 aalmero    (501) staff       (20)        0 2023-01-25 18:19:20.000000 sepm-api-0.0.5/sepm/endpoints/__init__.py
--rw-r--r--   0 aalmero    (501) staff       (20)    11653 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/administrators.py
--rw-r--r--   0 aalmero    (501) staff       (20)     4708 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/blacklist.py
--rw-r--r--   0 aalmero    (501) staff       (20)     4780 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/cloud.py
--rw-r--r--   0 aalmero    (501) staff       (20)    17544 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/commands.py
--rw-r--r--   0 aalmero    (501) staff       (20)     6805 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/computers.py
--rw-r--r--   0 aalmero    (501) staff       (20)      905 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/content.py
--rw-r--r--   0 aalmero    (501) staff       (20)     4591 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/domains.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1448 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/events.py
--rw-r--r--   0 aalmero    (501) staff       (20)      784 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/group_update_provider.py
--rw-r--r--   0 aalmero    (501) staff       (20)    38197 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/groups.py
--rw-r--r--   0 aalmero    (501) staff       (20)     2243 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/identity.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1054 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/notifications.py
--rw-r--r--   0 aalmero    (501) staff       (20)    25446 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/policies.py
--rw-r--r--   0 aalmero    (501) staff       (20)     2460 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/replication.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1135 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/reporting.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1267 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/requested_files.py
--rw-r--r--   0 aalmero    (501) staff       (20)     8058 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/statistics.py
--rw-r--r--   0 aalmero    (501) staff       (20)     6198 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/threat_defense_for_active_directory.py
--rw-r--r--   0 aalmero    (501) staff       (20)      800 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/version.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1108 2023-01-25 18:47:14.000000 sepm-api-0.0.5/sepm/exceptions.py
--rw-r--r--   0 aalmero    (501) staff       (20)     7836 2023-06-23 23:27:54.000000 sepm-api-0.0.5/sepm/rest_api_session.py
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.250637 sepm-api-0.0.5/sepm_api.egg-info/
--rw-r--r--   0 aalmero    (501) staff       (20)     1911 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/PKG-INFO
--rw-r--r--   0 aalmero    (501) staff       (20)      848 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/SOURCES.txt
--rw-r--r--   0 aalmero    (501) staff       (20)        1 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/dependency_links.txt
--rw-r--r--   0 aalmero    (501) staff       (20)        5 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/top_level.txt
--rw-r--r--   0 aalmero    (501) staff       (20)       38 2023-06-23 23:31:38.252968 sepm-api-0.0.5/setup.cfg
--rw-r--r--   0 aalmero    (501) staff       (20)      893 2023-06-23 22:49:41.000000 sepm-api-0.0.5/setup.py
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.251142 sepm-api-0.0.5/tests/
--rw-r--r--   0 aalmero    (501) staff       (20)       98 2023-01-23 20:35:31.000000 sepm-api-0.0.5/tests/test_sample.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-08-03 19:48:33.000000 sepm-api-0.0.6/
+-rw-r--r--   0 aalmero    (501) staff       (20)     1077 2023-01-23 20:35:31.000000 sepm-api-0.0.6/LICENSE
+-rw-r--r--   0 aalmero    (501) staff       (20)     2140 2023-08-03 19:48:33.000000 sepm-api-0.0.6/PKG-INFO
+-rw-r--r--   0 aalmero    (501) staff       (20)     1506 2023-06-23 23:45:20.000000 sepm-api-0.0.6/README.rst
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm/
+-rw-r--r--   0 aalmero    (501) staff       (20)     5536 2023-06-23 22:49:41.000000 sepm-api-0.0.6/sepm/__init__.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1091 2023-08-03 19:01:52.000000 sepm-api-0.0.6/sepm/config.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm/endpoints/
+-rw-r--r--   0 aalmero    (501) staff       (20)        0 2023-01-25 18:19:20.000000 sepm-api-0.0.6/sepm/endpoints/__init__.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    11672 2023-08-03 12:45:00.000000 sepm-api-0.0.6/sepm/endpoints/administrators.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     4708 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/blacklist.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     4780 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/cloud.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    17544 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/commands.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     6824 2023-08-03 12:45:00.000000 sepm-api-0.0.6/sepm/endpoints/computers.py
+-rw-r--r--   0 aalmero    (501) staff       (20)      905 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/content.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     4591 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/domains.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1448 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/events.py
+-rw-r--r--   0 aalmero    (501) staff       (20)      784 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/group_update_provider.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    38197 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/groups.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     2243 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/identity.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1054 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/notifications.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    25446 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/policies.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     2460 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/replication.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1135 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/reporting.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1267 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/requested_files.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     8058 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/statistics.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     6198 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/threat_defense_for_active_directory.py
+-rw-r--r--   0 aalmero    (501) staff       (20)      800 2023-04-25 15:56:27.000000 sepm-api-0.0.6/sepm/endpoints/version.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1108 2023-01-25 18:47:14.000000 sepm-api-0.0.6/sepm/exceptions.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     7836 2023-06-23 23:27:54.000000 sepm-api-0.0.6/sepm/rest_api_session.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm_api.egg-info/
+-rw-r--r--   0 aalmero    (501) staff       (20)     2140 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm_api.egg-info/PKG-INFO
+-rw-r--r--   0 aalmero    (501) staff       (20)      848 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 aalmero    (501) staff       (20)        1 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 aalmero    (501) staff       (20)        5 2023-08-03 19:48:33.000000 sepm-api-0.0.6/sepm_api.egg-info/top_level.txt
+-rw-r--r--   0 aalmero    (501) staff       (20)       38 2023-08-03 19:48:33.000000 sepm-api-0.0.6/setup.cfg
+-rw-r--r--   0 aalmero    (501) staff       (20)     1134 2023-08-03 19:48:24.000000 sepm-api-0.0.6/setup.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-08-03 19:48:33.000000 sepm-api-0.0.6/tests/
+-rw-r--r--   0 aalmero    (501) staff       (20)       98 2023-01-23 20:35:31.000000 sepm-api-0.0.6/tests/test_sample.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sepm-api-0.0.5/LICENSE` & `sepm-api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/PKG-INFO` & `sepm-api-0.0.6/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: sepm-api
-Version: 0.0.5
-Summary: Symantec Endpoint Protection Manager API
-Home-page: https://github.com/aalmero/sepm-api
-Author: Alex Almero
-Author-email: aalmero@gmail.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
 sepm-api
 ========
 
 .. image:: https://img.shields.io/pypi/v/sepm-api.svg
     :target: https://pypi.python.org/pypi/sepm-api
     :alt: Latest PyPI version
 
@@ -28,15 +15,15 @@
 | If you find any bugs please open an issue or a pull request.
 
 NOTE: The Python wrapper API is work in progress and should be treated as a software in beta, especially regarding the "undocumented" API endpoints.
 
 Usage
 -----
 
-    **Usages can be found in the `examples <https://github.com/aalmero/sepm-api/tree/main/examples>`_ folder.**
+    Refer to the `examples <https://github.com/aalmero/sepm-api/tree/main/examples>`_ folder.
 
 
 Installation
 ------------
 
 >>>pip install sepm-api
 
@@ -64,8 +51,8 @@
 Authors
 -------
 
 `sepm-api` was written by `Alex Almero <aalmero@gmail.com>`_.
 
 Disclaimers
 -----------
-I am in no way affiliated with Broadcom. Symantec is a registered trademark by Broadcom.
+I am in no way affiliated with Broadcom. Symantec is a registered trademark by Broadcom.
```

### Comparing `sepm-api-0.0.5/README.rst` & `sepm-api-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sepm-api
+Version: 0.0.6
+Summary: Symantec Endpoint Protection Manager API
+Home-page: https://github.com/aalmero/sepm-api
+Author: Alex Almero
+Author-email: aalmero@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
 sepm-api
 ========
 
 .. image:: https://img.shields.io/pypi/v/sepm-api.svg
     :target: https://pypi.python.org/pypi/sepm-api
     :alt: Latest PyPI version
 
@@ -15,15 +33,15 @@
 | If you find any bugs please open an issue or a pull request.
 
 NOTE: The Python wrapper API is work in progress and should be treated as a software in beta, especially regarding the "undocumented" API endpoints.
 
 Usage
 -----
 
-    **Usages can be found in the `examples <https://github.com/aalmero/sepm-api/tree/main/examples>`_ folder.**
+    Refer to the `examples <https://github.com/aalmero/sepm-api/tree/main/examples>`_ folder.
 
 
 Installation
 ------------
 
 >>>pip install sepm-api
 
@@ -51,8 +69,8 @@
 Authors
 -------
 
 `sepm-api` was written by `Alex Almero <aalmero@gmail.com>`_.
 
 Disclaimers
 -----------
-I am in no way affiliated with Broadcom. Symantec is a registered trademark by Broadcom.
+I am in no way affiliated with Broadcom. Symantec is a registered trademark by Broadcom.
```

### Comparing `sepm-api-0.0.5/sepm/__init__.py` & `sepm-api-0.0.6/sepm/__init__.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/config.py` & `sepm-api-0.0.6/sepm/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Enable/Disable Logging
 SUPPRESS_LOGGING = False
 
 #inherit an external logger instance.
 INHERIT_LOGGING_CONFIG = False
 
 # Simulate POST/PUT/DELETE calls
-SIMULATE_API = True
+SIMULATE_API = False
 
 # Retry if encountering other 4XX error (besides 429)?
 RETRY_4XX_ERROR = False
 
 # Other 4XX error retry wait time
 RETRY_4XX_ERROR_WAIT_TIME = 60
```

### Comparing `sepm-api-0.0.5/sepm/endpoints/administrators.py` & `sepm-api-0.0.6/sepm/endpoints/administrators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import urllib.parse
 
 class Administrators(object):
     """
     The Administrators APIs lets you perform the following administrative functions:
 
         Manage your administrator accounts.
         Access information about your servers and databases.
```

### Comparing `sepm-api-0.0.5/sepm/endpoints/blacklist.py` & `sepm-api-0.0.6/sepm/endpoints/blacklist.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/cloud.py` & `sepm-api-0.0.6/sepm/endpoints/cloud.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/commands.py` & `sepm-api-0.0.6/sepm/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/computers.py` & `sepm-api-0.0.6/sepm/endpoints/computers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import urllib.parse
 
 class Computers(object):
     """
     The Computers APIs let you manage your computers in a specified domain.
 
     A system administrator account is required for this API.
```

### Comparing `sepm-api-0.0.5/sepm/endpoints/content.py` & `sepm-api-0.0.6/sepm/endpoints/content.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/domains.py` & `sepm-api-0.0.6/sepm/endpoints/domains.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/events.py` & `sepm-api-0.0.6/sepm/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/group_update_provider.py` & `sepm-api-0.0.6/sepm/endpoints/group_update_provider.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/groups.py` & `sepm-api-0.0.6/sepm/endpoints/groups.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/identity.py` & `sepm-api-0.0.6/sepm/endpoints/identity.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/notifications.py` & `sepm-api-0.0.6/sepm/endpoints/notifications.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/policies.py` & `sepm-api-0.0.6/sepm/endpoints/policies.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/replication.py` & `sepm-api-0.0.6/sepm/endpoints/replication.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/reporting.py` & `sepm-api-0.0.6/sepm/endpoints/reporting.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/requested_files.py` & `sepm-api-0.0.6/sepm/endpoints/requested_files.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/statistics.py` & `sepm-api-0.0.6/sepm/endpoints/statistics.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/threat_defense_for_active_directory.py` & `sepm-api-0.0.6/sepm/endpoints/threat_defense_for_active_directory.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/endpoints/version.py` & `sepm-api-0.0.6/sepm/endpoints/version.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/exceptions.py` & `sepm-api-0.0.6/sepm/exceptions.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm/rest_api_session.py` & `sepm-api-0.0.6/sepm/rest_api_session.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/sepm_api.egg-info/PKG-INFO` & `sepm-api-0.0.6/sepm_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: sepm-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: Symantec Endpoint Protection Manager API
 Home-page: https://github.com/aalmero/sepm-api
 Author: Alex Almero
 Author-email: aalmero@gmail.com
 License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 sepm-api
 ========
 
 .. image:: https://img.shields.io/pypi/v/sepm-api.svg
     :target: https://pypi.python.org/pypi/sepm-api
@@ -28,15 +33,15 @@
 | If you find any bugs please open an issue or a pull request.
 
 NOTE: The Python wrapper API is work in progress and should be treated as a software in beta, especially regarding the "undocumented" API endpoints.
 
 Usage
 -----
 
-    **Usages can be found in the `examples <https://github.com/aalmero/sepm-api/tree/main/examples>`_ folder.**
+    Refer to the `examples <https://github.com/aalmero/sepm-api/tree/main/examples>`_ folder.
 
 
 Installation
 ------------
 
 >>>pip install sepm-api
```

### Comparing `sepm-api-0.0.5/sepm_api.egg-info/SOURCES.txt` & `sepm-api-0.0.6/sepm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.5/setup.py` & `sepm-api-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,27 +11,32 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="sepm-api",
-    version="0.0.5",
+    version="0.0.6",
     url="https://github.com/aalmero/sepm-api",
     license='MIT',
 
     author="Alex Almero",
     author_email="aalmero@gmail.com",
 
     description="Symantec Endpoint Protection Manager API",
     long_description=read("README.rst"),
 
     packages=find_packages(exclude=('tests',)),
 
     install_requires=[],
 
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
 )
```

