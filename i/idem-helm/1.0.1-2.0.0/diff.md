# Comparing `tmp/idem-helm-1.0.1.tar.gz` & `tmp/idem-helm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-helm-1.0.1.tar", last modified: Thu Jul 13 21:14:20 2023, max compression
+gzip compressed data, was "idem-helm-2.0.0.tar", last modified: Thu Aug  3 00:21:32 2023, max compression
```

## Comparing `idem-helm-1.0.1.tar` & `idem-helm-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-07-13 21:14:06.000000 idem-helm-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5330 2023-07-13 21:14:20.980510 idem-helm-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4526 2023-07-13 21:14:06.000000 idem-helm-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/acct/helm/
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/acct/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     1275 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/exec/helm/
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/exec/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/exec/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/states/helm/
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/states/helm/init.py
--rw-r--r--   0 root         (0) root         (0)    14946 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/states/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm/tool/helm/
--rw-r--r--   0 root         (0) root         (0)     3403 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/tool/helm/command_utils.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/tool/helm/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/tool/helm/release_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-07-13 21:14:06.000000 idem-helm-1.0.1/idem_helm/tool/helm/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:14:20.980510 idem-helm-1.0.1/idem_helm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5330 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 21:14:20.000000 idem-helm-1.0.1/idem_helm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 21:14:20.980510 idem-helm-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2719 2023-07-13 21:14:06.000000 idem-helm-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-08-03 00:21:17.000000 idem-helm-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-08-03 00:21:32.224386 idem-helm-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-08-03 00:21:17.000000 idem-helm-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.220386 idem-helm-2.0.0/idem_helm/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/acct/helm/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/acct/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.220386 idem-helm-2.0.0/idem_helm/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/exec/helm/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/exec/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/exec/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/states/helm/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/states/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)    14946 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/states/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm/tool/helm/
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/tool/helm/command_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/tool/helm/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/tool/helm/release_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-08-03 00:21:17.000000 idem-helm-2.0.0/idem_helm/tool/helm/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 00:21:31.000000 idem-helm-2.0.0/idem_helm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:21:32.224386 idem-helm-2.0.0/idem_helm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-08-03 00:21:32.000000 idem-helm-2.0.0/idem_helm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-08-03 00:21:32.000000 idem-helm-2.0.0/idem_helm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:21:32.000000 idem-helm-2.0.0/idem_helm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-03 00:21:32.000000 idem-helm-2.0.0/idem_helm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-08-03 00:21:32.000000 idem-helm-2.0.0/idem_helm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 00:21:32.000000 idem-helm-2.0.0/idem_helm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-03 00:21:32.224386 idem-helm-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-08-03 00:21:17.000000 idem-helm-2.0.0/setup.py
```

### Comparing `idem-helm-1.0.1/LICENSE` & `idem-helm-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/PKG-INFO` & `idem-helm-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 1.0.1
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =========
 idem-helm
 =========
```

### Comparing `idem-helm-1.0.1/README.rst` & `idem-helm-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/acct/helm/init.py` & `idem-helm-2.0.0/idem_helm/acct/helm/init.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/conf.py` & `idem-helm-2.0.0/idem_helm/conf.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/exec/helm/release.py` & `idem-helm-2.0.0/idem_helm/exec/helm/release.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/states/helm/release.py` & `idem-helm-2.0.0/idem_helm/states/helm/release.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/tool/helm/command_utils.py` & `idem-helm-2.0.0/idem_helm/tool/helm/command_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/tool/helm/comment_utils.py` & `idem-helm-2.0.0/idem_helm/tool/helm/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/tool/helm/release_utils.py` & `idem-helm-2.0.0/idem_helm/tool/helm/release_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm/tool/helm/test_state_utils.py` & `idem-helm-2.0.0/idem_helm/tool/helm/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/idem_helm.egg-info/PKG-INFO` & `idem-helm-2.0.0/idem_helm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 1.0.1
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =========
 idem-helm
 =========
```

### Comparing `idem-helm-1.0.1/idem_helm.egg-info/SOURCES.txt` & `idem-helm-2.0.0/idem_helm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-helm-1.0.1/setup.py` & `idem-helm-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,25 +70,25 @@
     url="",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
 )
```

