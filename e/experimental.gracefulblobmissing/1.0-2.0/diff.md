# Comparing `tmp/experimental.gracefulblobmissing-1.0.tar.gz` & `tmp/experimental.gracefulblobmissing-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimental.gracefulblobmissing-1.0.tar", last modified: Fri Mar 11 14:40:38 2022, max compression
+gzip compressed data, was "experimental.gracefulblobmissing-2.0.tar", last modified: Thu Aug  3 14:00:20 2023, max compression
```

## Comparing `experimental.gracefulblobmissing-1.0.tar` & `experimental.gracefulblobmissing-2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 thet      (1000) thet      (1000)        0 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/
--rw-rw-r--   0 thet      (1000) thet      (1000)     1216 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/CHANGES.rst
--rw-rw-r--   0 thet      (1000) thet      (1000)       95 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/MANIFEST.in
--rw-rw-r--   0 thet      (1000) thet      (1000)     4719 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/PKG-INFO
--rw-rw-r--   0 thet      (1000) thet      (1000)     1721 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/README.rst
-drwxrwxr-x   0 thet      (1000) thet      (1000)        0 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/docs/
--rw-rw-r--   0 thet      (1000) thet      (1000)     1392 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/docs/INSTALL.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)    17987 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/docs/LICENSE.GPL
--rw-rw-r--   0 thet      (1000) thet      (1000)      769 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/docs/LICENSE.txt
-drwxrwxr-x   0 thet      (1000) thet      (1000)        0 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/experimental/
--rw-rw-r--   0 thet      (1000) thet      (1000)      244 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/experimental/__init__.py
-drwxrwxr-x   0 thet      (1000) thet      (1000)        0 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/
--rw-rw-r--   0 thet      (1000) thet      (1000)       36 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/__init__.py
--rw-rw-r--   0 thet      (1000) thet      (1000)     3054 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/configure.zcml
-drwxrwxr-x   0 thet      (1000) thet      (1000)        0 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/dummies/
--rw-rw-r--   0 thet      (1000) thet      (1000)     2192 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/dummies/blob.png
--rw-rw-r--   0 thet      (1000) thet      (1000)     8682 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/patches.py
--rw-rw-r--   0 thet      (1000) thet      (1000)     1573 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/tests.py
-drwxrwxr-x   0 thet      (1000) thet      (1000)        0 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/
--rw-rw-r--   0 thet      (1000) thet      (1000)     4719 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/PKG-INFO
--rw-rw-r--   0 thet      (1000) thet      (1000)      806 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/SOURCES.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)        1 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/dependency_links.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)       89 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/entry_points.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)       13 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/namespace_packages.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)        1 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/not-zip-safe
--rw-rw-r--   0 thet      (1000) thet      (1000)       41 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/requires.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)       13 2022-03-11 14:40:38.000000 experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/top_level.txt
--rw-rw-r--   0 thet      (1000) thet      (1000)       38 2022-03-11 14:40:38.459601 experimental.gracefulblobmissing-1.0/setup.cfg
--rw-rw-r--   0 thet      (1000) thet      (1000)     1520 2022-03-11 14:40:37.000000 experimental.gracefulblobmissing-1.0/setup.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-08-03 14:00:20.618111 experimental.gracefulblobmissing-2.0/
+-rw-r--r--   0 thet      (1000) thet      (1000)     1302 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/CHANGES.rst
+-rw-r--r--   0 thet      (1000) thet      (1000)       95 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/MANIFEST.in
+-rw-r--r--   0 thet      (1000) thet      (1000)     3797 2023-08-03 14:00:20.618111 experimental.gracefulblobmissing-2.0/PKG-INFO
+-rw-r--r--   0 thet      (1000) thet      (1000)     1590 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/README.rst
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-08-03 14:00:20.614111 experimental.gracefulblobmissing-2.0/docs/
+-rw-r--r--   0 thet      (1000) thet      (1000)     1392 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/docs/INSTALL.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)    17987 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/docs/LICENSE.GPL
+-rw-r--r--   0 thet      (1000) thet      (1000)      769 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/docs/LICENSE.txt
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-08-03 14:00:20.614111 experimental.gracefulblobmissing-2.0/experimental/
+-rw-r--r--   0 thet      (1000) thet      (1000)      244 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental/__init__.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-08-03 14:00:20.618111 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/
+-rw-r--r--   0 thet      (1000) thet      (1000)       36 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/__init__.py
+-rw-r--r--   0 thet      (1000) thet      (1000)     1407 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/configure.zcml
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-08-03 14:00:20.618111 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/dummies/
+-rw-r--r--   0 thet      (1000) thet      (1000)     2192 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/dummies/blob.png
+-rw-r--r--   0 thet      (1000) thet      (1000)     5187 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/patches.py
+-rw-r--r--   0 thet      (1000) thet      (1000)     1573 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/tests.py
+drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-08-03 14:00:20.614111 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/
+-rw-r--r--   0 thet      (1000) thet      (1000)     3797 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/PKG-INFO
+-rw-r--r--   0 thet      (1000) thet      (1000)      806 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/SOURCES.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)        1 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/dependency_links.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)       40 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/entry_points.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)       13 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/namespace_packages.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)        1 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/not-zip-safe
+-rw-r--r--   0 thet      (1000) thet      (1000)       41 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/requires.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)       13 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/top_level.txt
+-rw-r--r--   0 thet      (1000) thet      (1000)       38 2023-08-03 14:00:20.618111 experimental.gracefulblobmissing-2.0/setup.cfg
+-rw-r--r--   0 thet      (1000) thet      (1000)     1593 2023-08-03 14:00:20.000000 experimental.gracefulblobmissing-2.0/setup.py
```

### Comparing `experimental.gracefulblobmissing-1.0/CHANGES.rst` & `experimental.gracefulblobmissing-2.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0 (2023-08-03)
+----------------
+
+- Remove Archetypes compatibility code.
+  [thet]
+
+
 1.0 (2022-03-11)
 ----------------
 
 - Add support for relstorage.
   [pbauer]
 
 - Create dummy image blobs on the fly.
```

### Comparing `experimental.gracefulblobmissing-1.0/README.rst` & `experimental.gracefulblobmissing-2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -12,33 +12,23 @@
 For developers this can be a little bit boring.
 It's quite common to copy a production ``Data.fs`` for developing using production data, but you don't always want to copy all blobs.
 
 This product monkey-patches parts of Plone, so that visiting objects that store content in the blob storage without having the BLOB available will not lead to errors.
 Instead a file only containing the string "File created by experimental.gracefulblobmissing." is created in the place where the blob-file should be.
 
 
-Catalog
--------
-
-This product also patches the ``SearchableText`` Archetypes method, so you can reindex you catalog without errors.
-
-
 Requirements
 ============
 
 This product has been tested on:
 
-* Plone 4.0
-* Plone 4.1
-* Plone 4.2
-* Plone 4.3
-* Plone 5.0
 * Plone 5.1
 * Plone 5.2
 
+For Plone 4 / Archetypes compatibility stay below version 2.0.
 For Plone 3 compatiblity stay on version 0.3.0 or lower.
 
 
 Warning
 =======
 
 This is designed only for **development/staging** environment. *Do not use in production* if you are not 100% sure of what you are doing!
```

### Comparing `experimental.gracefulblobmissing-1.0/docs/INSTALL.txt` & `experimental.gracefulblobmissing-2.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `experimental.gracefulblobmissing-1.0/docs/LICENSE.GPL` & `experimental.gracefulblobmissing-2.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `experimental.gracefulblobmissing-1.0/docs/LICENSE.txt` & `experimental.gracefulblobmissing-2.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/dummies/blob.png` & `experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/dummies/blob.png`

 * *Files identical despite different names*

### Comparing `experimental.gracefulblobmissing-1.0/experimental/gracefulblobmissing/tests.py` & `experimental.gracefulblobmissing-2.0/experimental/gracefulblobmissing/tests.py`

 * *Files identical despite different names*

### Comparing `experimental.gracefulblobmissing-1.0/experimental.gracefulblobmissing.egg-info/SOURCES.txt` & `experimental.gracefulblobmissing-2.0/experimental.gracefulblobmissing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experimental.gracefulblobmissing-1.0/setup.py` & `experimental.gracefulblobmissing-2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "1.0"
+version = "2.0"
 
 setup(
     name="experimental.gracefulblobmissing",
     version=version,
     description=(
         "Patch for Plone. "
         "Don't raise errors for file contents with missing BLOB file"
@@ -14,24 +14,25 @@
     long_description=open("README.rst").read()
     + "\n"
     + open("CHANGES.rst").read(),
     # Get more strings from
     # http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Framework :: Plone",
-        "Framework :: Plone :: 4.0",
-        "Framework :: Plone :: 4.1",
-        "Framework :: Plone :: 4.2",
-        "Framework :: Plone :: 4.3",
+        'Framework :: Plone :: 5.1',
+        'Framework :: Plone :: 5.2',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         "Programming Language :: Python",
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     keywords="plone blob patch",
     author="RedTurtle Technology",
     author_email="sviluppoplone@redturtle.it",
     url="http://plone.org/products/experimental.gracefulblobmissing",
     license="GPL",
     packages=find_packages(exclude=["ez_setup"]),
```

