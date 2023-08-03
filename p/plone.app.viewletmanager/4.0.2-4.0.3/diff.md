# Comparing `tmp/plone.app.viewletmanager-4.0.2.tar.gz` & `tmp/plone.app.viewletmanager-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.viewletmanager-4.0.2.tar", last modified: Mon May 22 17:53:26 2023, max compression
+gzip compressed data, was "plone.app.viewletmanager-4.0.3.tar", last modified: Thu Aug  3 10:33:32 2023, max compression
```

## Comparing `plone.app.viewletmanager-4.0.2.tar` & `plone.app.viewletmanager-4.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.742431 plone.app.viewletmanager-4.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     6517 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     7944 2023-05-22 17:53:26.742568 plone.app.viewletmanager-4.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      409 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.734487 plone.app.viewletmanager-4.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      686 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.734793 plone.app.viewletmanager-4.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.737273 plone.app.viewletmanager-4.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.739720 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      528 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.740591 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      414 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9058 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)      847 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3539 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewletmanager.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1930 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewlets.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11776 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manager.py
--rw-r--r--   0 maurits    (501) staff       (20)     2024 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)      793 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.742120 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4306 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/manager.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/storage.rst
--rw-r--r--   0 maurits    (501) staff       (20)      478 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    20701 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/test_exportimport.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.736949 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7944 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1197 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      173 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1643 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 17:53:26.743088 plone.app.viewletmanager-4.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1816 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.505521 plone.app.viewletmanager-4.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     6871 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     8335 2023-08-03 10:33:32.505164 plone.app.viewletmanager-4.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      409 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.496851 plone.app.viewletmanager-4.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      686 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.497155 plone.app.viewletmanager-4.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.499609 plone.app.viewletmanager-4.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.501961 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      528 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.502810 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9058 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/exportimport/storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      847 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3626 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/manage-viewletmanager.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2395 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/manage-viewlets.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11776 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2024 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      793 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.504556 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4306 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/manager.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/storage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      478 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20701 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/test_exportimport.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-08-03 10:33:32.499303 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     8335 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1187 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      173 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-08-03 10:33:32.000000 plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4191 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-08-03 10:33:32.505607 plone.app.viewletmanager-4.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1955 2023-08-03 10:33:31.000000 plone.app.viewletmanager-4.0.3/setup.py
```

### Comparing `plone.app.viewletmanager-4.0.2/CHANGES.rst` & `plone.app.viewletmanager-4.0.3/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,34 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-08-03)
+------------------
+
+Bug fixes:
+
+
+- Fix styles when toolbar is on top.
+  [petschki] (#29)
+- Only show one Hide or Show button per viewlet on the manage-viewlets page.
+  Make it clear that a viewlet is hidden by making it more subdued / opaque.
+  [maurits] (#3831)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.0.2 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Remove transitive circular dependency on `plone.app.vocabularies`.
```

### Comparing `plone.app.viewletmanager-4.0.2/PKG-INFO` & `plone.app.viewletmanager-4.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.viewletmanager
-Version: 4.0.2
+Version: 4.0.3
 Summary: Configurable viewlet manager
 Home-page: https://pypi.org/project/plone.app.viewletmanager
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: viewlets
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Introduction
 ============
 
 by Florian Schulze <fschulze@jarn.com>.
 
@@ -42,14 +43,34 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-08-03)
+------------------
+
+Bug fixes:
+
+
+- Fix styles when toolbar is on top.
+  [petschki] (#29)
+- Only show one Hide or Show button per viewlet on the manage-viewlets page.
+  Make it clear that a viewlet is hidden by making it more subdued / opaque.
+  [maurits] (#3831)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.0.2 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Remove transitive circular dependency on `plone.app.vocabularies`.
```

### Comparing `plone.app.viewletmanager-4.0.2/docs/LICENSE.GPL` & `plone.app.viewletmanager-4.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/docs/LICENSE.txt` & `plone.app.viewletmanager-4.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/configure.zcml` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/storage.py` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/exportimport/storage.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/interfaces.py` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewletmanager.pt` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/manage-viewletmanager.pt`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 
     <div class="card"
          tal:define="
            auth_token context/@@authenticator/token | nothing;
          "
     >
 
-      <div class="card-header">
+      <div class="card-header"
+           i18n:ignore="true"
+      >
         ViewletManager
         <span class="text-muted"
               tal:content="view/name"
         >ViewletManager name</span>
         (<span tal:content="view/interface"></span>)
       </div>
 
       <div class="card-body">
 
-        <div class="${python:'viewlet %s' % ('hiddenViewlet' if viewlet['hidden'] else '')}"
+        <div class="${python:'viewlet %s' % ('opacity-50' if viewlet['hidden'] else '')}"
              tal:repeat="viewlet options/viewlets"
         >
 
           <div class="card mb-3">
 
             <div class="card-header d-flex">
 
-              <div class="me-auto">
+              <div class="me-auto"
+                   i18n:ignore="true"
+              >
                 Viewlet
                 <span class="text-muted"
                       tal:content="viewlet/name"
                 >Viewlet name</span>
                 (<span tal:replace="viewlet/index">Index</span>)
               </div>
 
@@ -69,19 +73,19 @@
                      width="16"
                 >
                   <path d="M8 4a.5.5 0 0 1 .5.5v5.793l2.146-2.147a.5.5 0 0 1 .708.708l-3 3a.5.5 0 0 1-.708 0l-3-3a.5.5 0 1 1 .708-.708L7.5 10.293V4.5A.5.5 0 0 1 8 4z"
                         fill-rule="evenodd"
                   ></path>
                 </svg>
               </a>
-              <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject ${python:'active' if not viewlet['hidden'] else ''}"
+              <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject ${python:'' if not viewlet['hidden'] else 'd-none'}"
                  href="${viewlet/hide_url}&amp;_authenticator=${auth_token}#${manager_id}"
                  i18n:translate="label_hide_item"
               >Hide</a>
-              <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject ${python:'active' if viewlet['hidden'] else ''}"
+              <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject ${python:'' if viewlet['hidden'] else 'd-none'}"
                  href="${viewlet/show_url}&amp;_authenticator=${auth_token}#${manager_id}"
                  i18n:translate="label_show_item"
               >Show</a>
 
             </div>
 
             <div class="card-body">
```

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manager.py` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/manager.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/storage.py` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/storage.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/testing.py` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/manager.rst` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/manager.rst`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/storage.rst` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/storage.rst`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/test_exportimport.py` & `plone.app.viewletmanager-4.0.3/plone/app/viewletmanager/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/PKG-INFO` & `plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.viewletmanager
-Version: 4.0.2
+Version: 4.0.3
 Summary: Configurable viewlet manager
 Home-page: https://pypi.org/project/plone.app.viewletmanager
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: viewlets
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Introduction
 ============
 
 by Florian Schulze <fschulze@jarn.com>.
 
@@ -42,14 +43,34 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-08-03)
+------------------
+
+Bug fixes:
+
+
+- Fix styles when toolbar is on top.
+  [petschki] (#29)
+- Only show one Hide or Show button per viewlet on the manage-viewlets page.
+  Make it clear that a viewlet is hidden by making it more subdued / opaque.
+  [maurits] (#3831)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.0.2 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Remove transitive circular dependency on `plone.app.vocabularies`.
```

### Comparing `plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/SOURCES.txt` & `plone.app.viewletmanager-4.0.3/plone.app.viewletmanager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.app.viewletmanager.egg-info/PKG-INFO
 plone.app.viewletmanager.egg-info/SOURCES.txt
 plone.app.viewletmanager.egg-info/dependency_links.txt
```

### Comparing `plone.app.viewletmanager-4.0.2/setup.py` & `plone.app.viewletmanager-4.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.2"
+version = "4.0.3"
 
-long_description = "{}\n{}".format(
-    open("README.rst").read(), open("CHANGES.rst").read()
+long_description = (
+    f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 extras_require = {
     "test": [
         "Products.CMFPlone",
         "plone.app.testing",
         "plone.testing",
@@ -28,14 +29,17 @@
 ]
 
 setup(
     name="plone.app.viewletmanager",
     version=version,
     description="Configurable viewlet manager",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope",
```

