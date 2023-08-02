# Comparing `tmp/neon-enclosure-1.6.1a1.tar.gz` & `tmp/neon-enclosure-1.6.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-enclosure-1.6.1a1.tar", last modified: Thu Jul 20 03:12:09 2023, max compression
+gzip compressed data, was "neon-enclosure-1.6.1a2.tar", last modified: Wed Aug  2 23:08:31 2023, max compression
```

## Comparing `neon-enclosure-1.6.1a1.tar` & `neon-enclosure-1.6.1a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:09.831804 neon-enclosure-1.6.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 03:12:09.831804 neon-enclosure-1.6.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:09.831804 neon-enclosure-1.6.1a1/neon_enclosure/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:09.831804 neon-enclosure-1.6.1a1/neon_enclosure/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/admin/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/neon_enclosure/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:09.831804 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 03:12:09.000000 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 03:12:09.000000 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:12:09.000000 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 03:12:09.000000 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 03:12:09.000000 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 03:12:09.000000 neon-enclosure-1.6.1a1/neon_enclosure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 03:12:09.831804 neon-enclosure-1.6.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-20 03:12:06.000000 neon-enclosure-1.6.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:08:31.353894 neon-enclosure-1.6.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-02 23:08:31.353894 neon-enclosure-1.6.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:08:31.353894 neon-enclosure-1.6.1a2/neon_enclosure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:08:31.353894 neon-enclosure-1.6.1a2/neon_enclosure/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/admin/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/neon_enclosure/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:08:31.353894 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-02 23:08:31.000000 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-02 23:08:31.000000 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:08:31.000000 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 23:08:31.000000 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 23:08:31.000000 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 23:08:31.000000 neon-enclosure-1.6.1a2/neon_enclosure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:08:31.353894 neon-enclosure-1.6.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-02 23:08:22.000000 neon-enclosure-1.6.1a2/setup.py
```

### Comparing `neon-enclosure-1.6.1a1/LICENSE.md` & `neon-enclosure-1.6.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/PKG-INFO` & `neon-enclosure-1.6.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.6.1a1
+Version: 1.6.1a2
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.6.1a1/README.md` & `neon-enclosure-1.6.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/__init__.py` & `neon-enclosure-1.6.1a2/neon_enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/__main__.py` & `neon-enclosure-1.6.1a2/neon_enclosure/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/admin/__init__.py` & `neon-enclosure-1.6.1a2/neon_enclosure/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/admin/__main__.py` & `neon-enclosure-1.6.1a2/neon_enclosure/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/admin/service.py` & `neon-enclosure-1.6.1a2/neon_enclosure/admin/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/cli.py` & `neon-enclosure-1.6.1a2/neon_enclosure/cli.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure/service.py` & `neon-enclosure-1.6.1a2/neon_enclosure/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.1a1/neon_enclosure.egg-info/PKG-INFO` & `neon-enclosure-1.6.1a2/neon_enclosure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.6.1a1
+Version: 1.6.1a2
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.6.1a1/setup.py` & `neon-enclosure-1.6.1a2/setup.py`

 * *Files identical despite different names*

