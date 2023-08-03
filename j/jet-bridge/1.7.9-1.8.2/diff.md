# Comparing `tmp/jet-bridge-1.7.9.tar.gz` & `tmp/jet-bridge-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jet-bridge-1.7.9.tar", last modified: Thu Mar 16 07:39:18 2023, max compression
+gzip compressed data, was "dist/jet-bridge-1.8.2.tar", last modified: Thu Aug  3 11:16:24 2023, max compression
```

## Comparing `jet-bridge-1.7.9.tar` & `jet-bridge-1.8.2.tar`

### file list

```diff
@@ -1,52 +1,64 @@
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/
--rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)     1099 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/LICENSE
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/
--rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:48:56.000000 jet-bridge-1.7.9/jet_bridge.egg-info/not-zip-safe
--rw-r--r--   0 f1nal      (501) staff       (20)     1431 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       57 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/entry_points.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       68 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/requires.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/top_level.txt
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/dependency_links.txt
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/
--rw-r--r--   0 f1nal      (501) staff       (20)     5863 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/configuration.py
--rw-r--r--   0 f1nal      (501) staff       (20)       28 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/media.py
--rw-r--r--   0 f1nal      (501) staff       (20)       18 2023-03-16 02:56:11.000000 jet-bridge-1.7.9/jet_bridge/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)   229376 2022-11-24 06:42:37.000000 jet-bridge-1.7.9/jet_bridge/jet_bridge_store.db
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/utils/
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/utils/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1593 2021-08-31 19:06:46.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6817 2021-11-08 16:38:24.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      174 2021-08-31 19:06:46.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1948 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/utils/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)    13378 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/utils/create_config.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     3595 2023-02-16 15:32:25.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/app.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-31 19:06:46.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/media.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3205 2022-06-08 13:55:47.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/router.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5121 2023-02-16 15:32:23.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5369 2023-02-16 15:32:23.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/configuration.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      185 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6365 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3874 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/app.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/commands/
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/commands/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2896 2022-06-08 13:55:45.000000 jet-bridge-1.7.9/jet_bridge/router.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2299 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/__main__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/handlers/
--rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/handlers/temporary_redirect.py
--rw-r--r--   0 f1nal      (501) staff       (20)      224 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/handlers/not_found.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/handlers/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      611 2021-08-31 19:07:59.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5704 2023-02-16 15:32:26.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/view.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      613 2021-08-31 19:08:00.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      177 2021-08-31 19:07:59.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4644 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/handlers/view.py
--rw-r--r--   0 f1nal      (501) staff       (20)   106496 2023-02-22 06:44:49.000000 jet-bridge-1.7.9/jet_bridge/jet_bridge_store.sqlite3
--rw-r--r--   0 f1nal      (501) staff       (20)       65 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/MANIFEST.in
--rw-r--r--   0 f1nal      (501) staff       (20)    10270 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/README.md
--rw-r--r--   0 f1nal      (501) staff       (20)     1069 2023-03-16 02:56:11.000000 jet-bridge-1.7.9/setup.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/setup.cfg
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/
+-rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)     1099 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/LICENSE
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/
+-rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:48:56.000000 jet-bridge-1.8.2/jet_bridge.egg-info/not-zip-safe
+-rw-r--r--   0 f1nal      (501) staff       (20)     2045 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       57 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       68 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/requires.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/top_level.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge.egg-info/dependency_links.txt
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/
+-rw-r--r--   0 f1nal      (501) staff       (20)     6156 2023-07-27 17:17:30.000000 jet-bridge-1.8.2/jet_bridge/configuration.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       28 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/media.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       18 2023-08-03 09:34:59.000000 jet-bridge-1.8.2/jet_bridge/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)   229376 2022-11-24 06:42:37.000000 jet-bridge-1.8.2/jet_bridge/jet_bridge_store.db
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/utils/
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/utils/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/utils/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1593 2021-08-31 19:06:46.000000 jet-bridge-1.8.2/jet_bridge/utils/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6817 2021-11-08 16:38:24.000000 jet-bridge-1.8.2/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1597 2023-04-20 15:15:39.000000 jet-bridge-1.8.2/jet_bridge/utils/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      174 2021-08-31 19:06:46.000000 jet-bridge-1.8.2/jet_bridge/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      178 2023-04-20 15:15:39.000000 jet-bridge-1.8.2/jet_bridge/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1948 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/utils/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    13378 2023-02-14 16:01:58.000000 jet-bridge-1.8.2/jet_bridge/utils/create_config.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3845 2023-04-14 09:10:56.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/app.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-31 19:06:46.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/media.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      196 2023-04-20 15:15:39.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/media.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3849 2023-04-20 15:28:47.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/app.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3209 2023-04-20 15:28:47.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/router.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3388 2023-07-28 07:27:39.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/router.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5714 2023-07-27 17:36:56.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5253 2023-04-20 15:15:39.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5513 2023-07-27 17:36:56.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/configuration.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5430 2023-04-20 15:15:39.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/configuration.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      185 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      190 2023-04-20 15:30:49.000000 jet-bridge-1.8.2/jet_bridge/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7164 2023-07-27 17:18:30.000000 jet-bridge-1.8.2/jet_bridge/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4165 2023-04-14 09:10:54.000000 jet-bridge-1.8.2/jet_bridge/app.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/commands/
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/commands/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3236 2023-07-28 07:27:37.000000 jet-bridge-1.8.2/jet_bridge/router.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2542 2023-04-21 04:03:59.000000 jet-bridge-1.8.2/jet_bridge/__main__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/handlers/
+-rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/handlers/temporary_redirect.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      224 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/handlers/not_found.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/jet_bridge/handlers/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      615 2023-04-20 15:28:47.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      611 2021-08-31 19:07:59.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5708 2023-04-20 15:28:47.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/view.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5847 2023-07-28 07:34:44.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/view.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      613 2021-08-31 19:08:00.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      617 2023-04-20 15:28:47.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/not_found.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      177 2021-08-31 19:07:59.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      181 2023-04-20 15:28:47.000000 jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4909 2023-07-28 07:34:41.000000 jet-bridge-1.8.2/jet_bridge/handlers/view.py
+-rw-r--r--   0 f1nal      (501) staff       (20)   135168 2023-08-03 09:31:50.000000 jet-bridge-1.8.2/jet_bridge/jet_bridge_store.sqlite3
+-rw-r--r--   0 f1nal      (501) staff       (20)       65 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/MANIFEST.in
+-rw-r--r--   0 f1nal      (501) staff       (20)    10270 2021-08-25 15:07:30.000000 jet-bridge-1.8.2/README.md
+-rw-r--r--   0 f1nal      (501) staff       (20)     1069 2023-08-03 09:34:59.000000 jet-bridge-1.8.2/setup.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-08-03 11:16:24.000000 jet-bridge-1.8.2/setup.cfg
```

### Comparing `jet-bridge-1.7.9/PKG-INFO` & `jet-bridge-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-bridge
-Version: 1.7.9
+Version: 1.8.2
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-bridge
 Author: Denis Kildishev
 Author-email: support@jetadmin.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jet-bridge-1.7.9/LICENSE` & `jet-bridge-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge.egg-info/PKG-INFO` & `jet-bridge-1.8.2/jet_bridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-bridge
-Version: 1.7.9
+Version: 1.8.2
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-bridge
 Author: Denis Kildishev
 Author-email: support@jetadmin.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jet-bridge-1.7.9/jet_bridge.egg-info/SOURCES.txt` & `jet-bridge-1.8.2/jet_bridge.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,27 +15,39 @@
 jet_bridge.egg-info/SOURCES.txt
 jet_bridge.egg-info/dependency_links.txt
 jet_bridge.egg-info/entry_points.txt
 jet_bridge.egg-info/not-zip-safe
 jet_bridge.egg-info/requires.txt
 jet_bridge.egg-info/top_level.txt
 jet_bridge/__pycache__/__init__.cpython-36.pyc
+jet_bridge/__pycache__/__init__.cpython-37.pyc
 jet_bridge/__pycache__/app.cpython-36.pyc
+jet_bridge/__pycache__/app.cpython-37.pyc
 jet_bridge/__pycache__/configuration.cpython-36.pyc
+jet_bridge/__pycache__/configuration.cpython-37.pyc
 jet_bridge/__pycache__/media.cpython-36.pyc
+jet_bridge/__pycache__/media.cpython-37.pyc
 jet_bridge/__pycache__/router.cpython-36.pyc
+jet_bridge/__pycache__/router.cpython-37.pyc
 jet_bridge/__pycache__/settings.cpython-36.pyc
+jet_bridge/__pycache__/settings.cpython-37.pyc
 jet_bridge/commands/__init__.py
 jet_bridge/handlers/__init__.py
 jet_bridge/handlers/not_found.py
 jet_bridge/handlers/temporary_redirect.py
 jet_bridge/handlers/view.py
 jet_bridge/handlers/__pycache__/__init__.cpython-36.pyc
+jet_bridge/handlers/__pycache__/__init__.cpython-37.pyc
 jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc
+jet_bridge/handlers/__pycache__/not_found.cpython-37.pyc
 jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc
+jet_bridge/handlers/__pycache__/temporary_redirect.cpython-37.pyc
 jet_bridge/handlers/__pycache__/view.cpython-36.pyc
+jet_bridge/handlers/__pycache__/view.cpython-37.pyc
 jet_bridge/utils/__init__.py
 jet_bridge/utils/create_config.py
 jet_bridge/utils/settings.py
 jet_bridge/utils/__pycache__/__init__.cpython-36.pyc
+jet_bridge/utils/__pycache__/__init__.cpython-37.pyc
 jet_bridge/utils/__pycache__/create_config.cpython-36.pyc
-jet_bridge/utils/__pycache__/settings.cpython-36.pyc
+jet_bridge/utils/__pycache__/settings.cpython-36.pyc
+jet_bridge/utils/__pycache__/settings.cpython-37.pyc
```

### Comparing `jet-bridge-1.7.9/jet_bridge/configuration.py` & `jet-bridge-1.8.2/jet_bridge/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,19 @@
             'DATABASE_USER': settings.DATABASE_USER,
             'DATABASE_PASSWORD': settings.DATABASE_PASSWORD,
             'DATABASE_NAME': settings.DATABASE_NAME,
             'DATABASE_EXTRA': settings.DATABASE_EXTRA,
             'DATABASE_CONNECTIONS': settings.CONNECTIONS,
             'DATABASE_ONLY': settings.DATABASE_ONLY,
             'DATABASE_EXCEPT': settings.DATABASE_EXCEPT,
+            'DATABASE_MAX_TABLES': settings.DATABASE_MAX_TABLES,
             'DATABASE_SCHEMA': settings.DATABASE_SCHEMA,
+            'DATABASE_SSL_CA': settings.DATABASE_SSL_CA,
+            'DATABASE_SSL_CERT': settings.DATABASE_SSL_CERT,
+            'DATABASE_SSL_KEY': settings.DATABASE_SSL_KEY,
             'DATABASE_SSH_HOST': settings.DATABASE_SSH_HOST,
             'DATABASE_SSH_PORT': settings.DATABASE_SSH_PORT,
             'DATABASE_SSH_USER': settings.DATABASE_SSH_USER,
             'DATABASE_SSH_PRIVATE_KEY': settings.DATABASE_SSH_PRIVATE_KEY,
             'COOKIE_SAMESITE': settings.COOKIE_SAMESITE,
             'COOKIE_SECURE': settings.COOKIE_SECURE,
             'COOKIE_DOMAIN': settings.COOKIE_DOMAIN,
@@ -55,15 +59,16 @@
             'STORE_PATH': settings.STORE_PATH,
             'SSO_APPLICATIONS': self.clean_sso_applications(settings.SSO_APPLICATIONS),
             'ALLOW_ORIGIN': settings.ALLOW_ORIGIN,
             'TRACK_DATABASES': settings.TRACK_DATABASES,
             'TRACK_DATABASES_ENDPOINT': settings.TRACK_DATABASES_ENDPOINT,
             'TRACK_DATABASES_AUTH': settings.TRACK_DATABASES_AUTH,
             'TRACK_MODELS_ENDPOINT': settings.TRACK_MODELS_ENDPOINT,
-            'TRACK_MODELS_AUTH': settings.TRACK_MODELS_AUTH
+            'TRACK_MODELS_AUTH': settings.TRACK_MODELS_AUTH,
+            'DISABLE_AUTH': settings.DISABLE_AUTH
         }
 
     def media_get_available_name(self, path):
         dir_name, file_name = os.path.split(path)
         file_root, file_ext = os.path.splitext(file_name)
 
         while os.path.exists(os.path.join(settings.MEDIA_ROOT, path)):
```

### Comparing `jet-bridge-1.7.9/jet_bridge/jet_bridge_store.db` & `jet-bridge-1.8.2/jet_bridge/jet_bridge_store.db`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/utils/__pycache__/settings.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/utils/__pycache__/settings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/utils/settings.py` & `jet-bridge-1.8.2/jet_bridge/utils/settings.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/utils/create_config.py` & `jet-bridge-1.8.2/jet_bridge/utils/create_config.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/__pycache__/app.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/__pycache__/app.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 330d 0d0a 76b0 eb63 220f 0000 e300 0000  3...v..c".......
+00000000: 330d 0d0a 9e18 3964 4510 0000 e300 0000  3.....9dE.......
 00000010: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00000020: 0073 6401 0000 6400 6401 6c00 5a00 6400  .sd...d.d.l.Z.d.
+00000020: 0073 7c01 0000 6400 6401 6c00 5a00 6400  .s|...d.d.l.Z.d.
 00000030: 6401 6c01 5a02 6400 6401 6c03 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c0a 6d0b 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0d 6d0e 5a0e 0100 6400 6407 6c0f  d.l.m.Z...d.d.l.
 00000080: 6d10 5a10 0100 6400 6408 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
 00000090: 0100 6400 6409 6c13 6d14 5a14 0100 6400  ..d.d.l.m.Z...d.
@@ -14,212 +14,228 @@
 000000d0: 640e 6c1d 6d1e 5a1e 0100 6400 640f 6c1f  d.l.m.Z...d.d.l.
 000000e0: 6d20 5a20 0100 6400 6410 6c21 6d22 5a22  m Z ..d.d.l!m"Z"
 000000f0: 0100 6400 6411 6c23 6d24 5a24 0100 6400  ..d.d.l#m$Z$..d.
 00000100: 6412 6c25 6d26 5a26 0100 6400 6413 6c27  d.l%m&Z&..d.d.l'
 00000110: 6d28 5a28 0100 6400 6414 6c29 6d2a 5a2a  m(Z(..d.d.l)m*Z*
 00000120: 0100 6400 6415 6c2b 6d2c 5a2c 0100 6400  ..d.d.l+m,Z,..d.
 00000130: 6416 6c2d 6d2e 5a2e 0100 6400 6417 6c2f  d.l-m.Z...d.d.l/
-00000140: 6d0b 5a0b 6d30 5a30 6d31 5a31 0100 6400  m.Z.m0Z0m1Z1..d.
-00000150: 6418 6c32 6d33 5a33 0100 6400 6419 6c34  d.l2m3Z3..d.d.l4
+00000140: 6d30 5a30 0100 6400 6418 6c31 6d32 5a32  m0Z0..d.d.l1m2Z2
+00000150: 0100 6400 6419 6c33 6d0b 5a0b 6d34 5a34  ..d.d.l3m.Z.m4Z4
 00000160: 6d35 5a35 0100 6400 641a 6c36 6d37 5a37  m5Z5..d.d.l6m7Z7
-00000170: 0100 6400 641b 6c38 6d39 5a39 0100 641c  ..d.d.l8m9Z9..d.
-00000180: 641d 8400 5a3a 6401 5300 291e e900 0000  d...Z:d.S.).....
-00000190: 004e 2901 da18 5465 6d70 6f72 6172 7952  .N)...TemporaryR
-000001a0: 6564 6972 6563 7448 616e 646c 6572 2901  edirectHandler).
-000001b0: da11 7365 6e74 7279 5f63 6f6e 7472 6f6c  ..sentry_control
-000001c0: 6c65 7229 01da 0f73 6574 5f6d 6178 5f77  ler)...set_max_w
-000001d0: 6f72 6b65 7273 2901 da08 7365 7474 696e  orkers)...settin
-000001e0: 6773 2901 da07 4170 6956 6965 7729 01da  gs)...ApiView)..
-000001f0: 1845 7874 6572 6e61 6c41 7574 6843 6f6d  .ExternalAuthCom
-00000200: 706c 6574 6556 6965 7729 01da 1545 7874  pleteView)...Ext
-00000210: 6572 6e61 6c41 7574 684c 6f67 696e 5669  ernalAuthLoginVi
-00000220: 6577 2901 da0b 4772 6170 6851 4c56 6965  ew)...GraphQLVie
-00000230: 7729 01da 0f49 6d61 6765 5265 7369 7a65  w)...ImageResize
-00000240: 5669 6577 2901 da0e 4669 6c65 5570 6c6f  View)...FileUplo
-00000250: 6164 5669 6577 2901 da0b 4d65 7373 6167  adView)...Messag
-00000260: 6556 6965 7729 01da 0c4d 6f64 656c 5669  eView)...ModelVi
-00000270: 6577 5365 7429 01da 144d 6f64 656c 4465  ewSet)...ModelDe
-00000280: 7363 7269 7074 696f 6e56 6965 7729 01da  scriptionView)..
-00000290: 284d 6f64 656c 4465 7363 7269 7074 696f  (ModelDescriptio
-000002a0: 6e52 656c 6174 696f 6e73 6869 704f 7665  nRelationshipOve
-000002b0: 7272 6964 6556 6965 7729 01da 1050 726f  rrideView)...Pro
-000002c0: 7879 5265 7175 6573 7456 6965 7729 01da  xyRequestView)..
-000002d0: 0c52 6567 6973 7465 7256 6965 7729 01da  .RegisterView)..
-000002e0: 0a52 656c 6f61 6456 6965 7729 01da 0753  .ReloadView)...S
-000002f0: 716c 5669 6577 2901 da0a 5374 6174 7573  qlView)...Status
-00000300: 5669 6577 2901 da09 5461 626c 6556 6965  View)...TableVie
-00000310: 7729 01da 0f54 6162 6c65 436f 6c75 6d6e  w)...TableColumn
-00000320: 5669 6577 2903 7205 0000 00da 056d 6564  View).r......med
-00000330: 6961 da07 5645 5253 494f 4e29 01da 0c76  ia..VERSION)...v
-00000340: 6965 775f 6861 6e64 6c65 7229 01da 0f4e  iew_handler)...N
-00000350: 6f74 466f 756e 6448 616e 646c 6572 2901  otFoundHandler).
-00000360: da06 526f 7574 6572 2901 da14 5472 6967  ..Router)...Trig
-00000370: 6765 7245 7863 6570 7469 6f6e 5669 6577  gerExceptionView
-00000380: 6300 0000 0000 0000 0002 0000 0014 0000  c...............
-00000390: 0043 0000 0073 8a01 0000 7400 8300 7d00  .C...s....t...}.
-000003a0: 7c00 6a01 6401 7402 7403 8301 8302 0100  |.j.d.t.t.......
-000003b0: 7c00 6a01 6402 7402 7404 8301 8302 0100  |.j.d.t.t.......
-000003c0: 7c00 6a01 6403 7402 7405 8301 8302 0100  |.j.d.t.t.......
-000003d0: 6404 7406 6405 6406 6901 6603 6407 7402  d.t.d.d.i.f.d.t.
-000003e0: 7407 8301 6602 6406 7402 7408 8301 6602  t...f.d.t.t...f.
-000003f0: 6408 7402 7407 8301 6602 6409 7402 7409  d.t.t...f.d.t.t.
-00000400: 8301 6602 640a 7402 740a 8301 6602 640b  ..f.d.t.t...f.d.
-00000410: 7402 740b 8301 6602 640c 7402 740c 8301  t.t...f.d.t.t...
-00000420: 6602 640d 7402 740d 8301 6602 640e 7402  f.d.t.t...f.d.t.
-00000430: 740e 8301 6602 640f 7402 740f 8301 6602  t...f.d.t.t...f.
-00000440: 6410 7402 7410 8301 6602 6411 7402 7411  d.t.t...f.d.t.t.
-00000450: 8301 6602 6412 7412 6a13 6a14 6413 7415  ..f.d.t.j.j.d.t.
-00000460: 6a16 6901 6603 6414 7402 7417 8301 6602  j.i.f.d.t.t...f.
-00000470: 6415 7402 7418 8301 6602 6416 7402 7419  d.t.t...f.d.t.t.
-00000480: 8301 6602 6417 7402 741a 8301 6602 6712  ..f.d.t.t...f.g.
-00000490: 7d01 7c01 7c00 6a1b 3700 7d01 7415 6a1c  }.|.|.j.7.}.t.j.
-000004a0: 741d 6a1e 6b02 9001 722a 7c01 6a1f 6412  t.j.k...r*|.j.d.
-000004b0: 7412 6a13 6a14 6413 7415 6a16 6901 6603  t.j.j.d.t.j.i.f.
-000004c0: 8301 0100 7415 6a20 6400 6b09 9001 7240  ....t.j d.k...r@
-000004d0: 7421 7415 6a20 8301 0100 7415 6a22 9001  t!t.j ....t.j"..
-000004e0: 7260 7423 6a24 7415 6a22 6418 6a25 7426  r`t#j$t.j"d.j%t&
-000004f0: 8301 6419 641a 8d03 0100 7412 6a13 6a27  ..d.d.....t.j.j'
-00000500: 7c01 7415 6a28 7429 742a 6a2b 6a2c 742d  |.t.j(t)t*j+j,t-
-00000510: 6a2e 641b 8302 7415 6a28 7415 6a2f 641c  j.d...t.j(t.j/d.
-00000520: 8d06 5300 291d 4e7a 1d2f 6170 692f 6d6f  ..S.).Nz./api/mo
-00000530: 6465 6c73 2f28 3f50 3c6d 6f64 656c 3e5b  dels/(?P<model>[
-00000540: 5e2f 5d2b 292f 7a25 2f61 7069 2f74 6162  ^/]+)/z%/api/tab
-00000550: 6c65 732f 283f 503c 7461 626c 653e 5b5e  les/(?P<table>[^
-00000560: 2f5d 2b29 2f63 6f6c 756d 6e73 2f7a 0c2f  /]+)/columns/z./
-00000570: 6170 692f 7461 626c 6573 2ffa 012f da03  api/tables/../..
-00000580: 7572 6c7a 052f 6170 692f 7a0a 2f72 6567  urlz./api/z./reg
-00000590: 6973 7465 722f 7a0e 2f61 7069 2f72 6567  ister/z./api/reg
-000005a0: 6973 7465 722f 7a0d 2f61 7069 2f67 7261  ister/z./api/gra
-000005b0: 7068 716c 2f7a 2f2f 6170 692f 6d6f 6465  phql/z//api/mode
-000005c0: 6c5f 6465 7363 7269 7074 696f 6e73 2f72  l_descriptions/r
-000005d0: 656c 6174 696f 6e73 6869 705f 6f76 6572  elationship_over
-000005e0: 7269 6465 732f 7a18 2f61 7069 2f6d 6f64  rides/z./api/mod
-000005f0: 656c 5f64 6573 6372 6970 7469 6f6e 732f  el_descriptions/
-00000600: 7a09 2f61 7069 2f73 716c 2f7a 0e2f 6170  z./api/sql/z./ap
-00000610: 692f 6d65 7373 6167 6573 2f7a 112f 6170  i/messages/z./ap
-00000620: 692f 6669 6c65 5f75 706c 6f61 642f 7a12  i/file_upload/z.
-00000630: 2f61 7069 2f69 6d61 6765 5f72 6573 697a  /api/image_resiz
-00000640: 652f 7a0c 2f61 7069 2f72 656c 6f61 642f  e/z./api/reload/
-00000650: 7a13 2f61 7069 2f70 726f 7879 5f72 6571  z./api/proxy_req
-00000660: 7565 7374 2f7a 0b2f 6d65 6469 612f 282e  uest/z./media/(.
-00000670: 2a29 da04 7061 7468 7a28 2f61 7069 2f65  *)..pathz(/api/e
-00000680: 7874 6572 6e61 6c5f 6175 7468 2f6c 6f67  xternal_auth/log
-00000690: 696e 2f28 3f50 3c61 7070 3e5b 5e2f 5d2b  in/(?P<app>[^/]+
-000006a0: 292f 7a2b 2f61 7069 2f65 7874 6572 6e61  )/z+/api/externa
-000006b0: 6c5f 6175 7468 2f63 6f6d 706c 6574 652f  l_auth/complete/
-000006c0: 283f 503c 6170 703e 5b5e 2f5d 2b29 2f7a  (?P<app>[^/]+)/z
-000006d0: 0c2f 6170 692f 7374 6174 7573 2f7a 172f  ./api/status/z./
-000006e0: 6170 692f 7472 6967 6765 725f 6578 6365  api/trigger_exce
-000006f0: 7074 696f 6e2f 7a0d 6a65 742d 6272 6964  ption/z.jet-brid
-00000700: 6765 407b 7d54 2903 da03 6473 6eda 0772  ge@{}T)...dsn..r
-00000710: 656c 6561 7365 da07 746f 726e 6164 6f5a  elease..tornadoZ
-00000720: 0974 656d 706c 6174 6573 2906 da08 6861  .templates)...ha
-00000730: 6e64 6c65 7273 da05 6465 6275 675a 1564  ndlers..debugZ.d
-00000740: 6566 6175 6c74 5f68 616e 646c 6572 5f63  efault_handler_c
-00000750: 6c61 7373 5a0d 7465 6d70 6c61 7465 5f70  lassZ.template_p
-00000760: 6174 685a 0a61 7574 6f72 656c 6f61 645a  athZ.autoreloadZ
-00000770: 0d63 6f6f 6b69 655f 7365 6372 6574 2930  .cookie_secret)0
-00000780: 721b 0000 00da 0872 6567 6973 7465 7272  r......registerr
-00000790: 1900 0000 720d 0000 0072 1600 0000 7215  ....r....r....r.
-000007a0: 0000 0072 0200 0000 7211 0000 0072 0600  ...r....r....r..
-000007b0: 0000 7209 0000 0072 0f00 0000 720e 0000  ..r....r....r...
-000007c0: 0072 1300 0000 720c 0000 0072 0b00 0000  .r....r....r....
-000007d0: 720a 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
-000007e0: 2200 0000 5a03 7765 625a 1153 7461 7469  "...Z.webZ.Stati
-000007f0: 6346 696c 6548 616e 646c 6572 7205 0000  cFileHandlerr...
-00000800: 00da 0a4d 4544 4941 5f52 4f4f 5472 0800  ...MEDIA_ROOTr..
-00000810: 0000 7207 0000 0072 1400 0000 721c 0000  ..r....r....r...
-00000820: 00da 0475 726c 73da 0d4d 4544 4941 5f53  ...urls..MEDIA_S
-00000830: 544f 5241 4745 7217 0000 00da 124d 4544  TORAGEr......MED
-00000840: 4941 5f53 544f 5241 4745 5f46 494c 45da  IA_STORAGE_FILE.
-00000850: 0661 7070 656e 64da 0754 4852 4541 4453  .append..THREADS
-00000860: 7204 0000 00da 0a53 454e 5452 595f 4453  r......SENTRY_DS
-00000870: 4e72 0300 0000 da06 656e 6162 6c65 da06  Nr......enable..
-00000880: 666f 726d 6174 7218 0000 00da 0b41 7070  formatr......App
-00000890: 6c69 6361 7469 6f6e da05 4445 4255 4772  lication..DEBUGr
-000008a0: 1a00 0000 da02 6f73 721f 0000 00da 046a  ......osr......j
-000008b0: 6f69 6eda 0d62 6173 655f 7365 7474 696e  oin..base_settin
-000008c0: 6773 da08 4241 5345 5f44 4952 da05 544f  gs..BASE_DIR..TO
-000008d0: 4b45 4e29 025a 0672 6f75 7465 7272 2700  KEN).Z.routerr'.
-000008e0: 0000 a900 7236 0000 00fa 502f 5573 6572  ....r6....P/User
-000008f0: 732f 6631 6e61 6c2f 4472 6f70 626f 782f  s/f1nal/Dropbox/
-00000900: 7079 7468 6f6e 2f6a 6574 2d62 7269 6467  python/jet-bridg
-00000910: 652f 7372 632f 7061 636b 6167 6573 2f6a  e/src/packages/j
-00000920: 6574 5f62 7269 6467 652f 6a65 745f 6272  et_bridge/jet_br
-00000930: 6964 6765 2f61 7070 2e70 79da 086d 616b  idge/app.py..mak
-00000940: 655f 6170 7023 0000 0073 4e00 0000 0001  e_app#...sN.....
-00000950: 0602 1001 1001 1003 0c01 0a01 0a01 0a01  ................
-00000960: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00000970: 0a01 1201 0a01 0a01 0a01 0e02 0a02 0e01  ................
-00000980: 1a02 0c01 0a02 0801 0401 0401 0801 0803  ................
-00000990: 0601 0201 0401 0201 0e01 0401 7238 0000  ............r8..
-000009a0: 0029 3b72 3100 0000 da0e 746f 726e 6164  .);r1.....tornad
-000009b0: 6f2e 696f 6c6f 6f70 7222 0000 005a 0b74  o.ioloopr"...Z.t
-000009c0: 6f72 6e61 646f 2e77 6562 5a26 6a65 745f  ornado.webZ&jet_
-000009d0: 6272 6964 6765 2e68 616e 646c 6572 732e  bridge.handlers.
-000009e0: 7465 6d70 6f72 6172 795f 7265 6469 7265  temporary_redire
-000009f0: 6374 7202 0000 005a 166a 6574 5f62 7269  ctr....Z.jet_bri
-00000a00: 6467 655f 6261 7365 2e73 656e 7472 7972  dge_base.sentryr
-00000a10: 0300 0000 5a20 6a65 745f 6272 6964 6765  ....Z jet_bridge
-00000a20: 5f62 6173 652e 7574 696c 732e 6173 796e  _base.utils.asyn
-00000a30: 635f 6578 6563 7204 0000 00da 0f6a 6574  c_execr......jet
-00000a40: 5f62 7269 6467 655f 6261 7365 7205 0000  _bridge_baser...
-00000a50: 0072 3300 0000 5a19 6a65 745f 6272 6964  .r3...Z.jet_brid
-00000a60: 6765 5f62 6173 652e 7669 6577 732e 6170  ge_base.views.ap
-00000a70: 6972 0600 0000 5a2c 6a65 745f 6272 6964  ir....Z,jet_brid
-00000a80: 6765 5f62 6173 652e 7669 6577 732e 6578  ge_base.views.ex
-00000a90: 7465 726e 616c 5f61 7574 682e 636f 6d70  ternal_auth.comp
-00000aa0: 6c65 7465 7207 0000 005a 296a 6574 5f62  leter....Z)jet_b
-00000ab0: 7269 6467 655f 6261 7365 2e76 6965 7773  ridge_base.views
-00000ac0: 2e65 7874 6572 6e61 6c5f 6175 7468 2e6c  .external_auth.l
-00000ad0: 6f67 696e 7208 0000 005a 1d6a 6574 5f62  oginr....Z.jet_b
-00000ae0: 7269 6467 655f 6261 7365 2e76 6965 7773  ridge_base.views
-00000af0: 2e67 7261 7068 716c 7209 0000 005a 226a  .graphqlr....Z"j
-00000b00: 6574 5f62 7269 6467 655f 6261 7365 2e76  et_bridge_base.v
-00000b10: 6965 7773 2e69 6d61 6765 5f72 6573 697a  iews.image_resiz
-00000b20: 6572 0a00 0000 5a21 6a65 745f 6272 6964  er....Z!jet_brid
-00000b30: 6765 5f62 6173 652e 7669 6577 732e 6669  ge_base.views.fi
-00000b40: 6c65 5f75 706c 6f61 6472 0b00 0000 5a1d  le_uploadr....Z.
-00000b50: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00000b60: 7669 6577 732e 6d65 7373 6167 6572 0c00  views.messager..
-00000b70: 0000 5a1b 6a65 745f 6272 6964 6765 5f62  ..Z.jet_bridge_b
-00000b80: 6173 652e 7669 6577 732e 6d6f 6465 6c72  ase.views.modelr
-00000b90: 0d00 0000 5a27 6a65 745f 6272 6964 6765  ....Z'jet_bridge
-00000ba0: 5f62 6173 652e 7669 6577 732e 6d6f 6465  _base.views.mode
-00000bb0: 6c5f 6465 7363 7269 7074 696f 6e72 0e00  l_descriptionr..
-00000bc0: 0000 5a3d 6a65 745f 6272 6964 6765 5f62  ..Z=jet_bridge_b
-00000bd0: 6173 652e 7669 6577 732e 6d6f 6465 6c5f  ase.views.model_
-00000be0: 6465 7363 7269 7074 696f 6e5f 7265 6c61  description_rela
-00000bf0: 7469 6f6e 7368 6970 5f6f 7665 7272 6964  tionship_overrid
-00000c00: 6572 0f00 0000 5a23 6a65 745f 6272 6964  er....Z#jet_brid
-00000c10: 6765 5f62 6173 652e 7669 6577 732e 7072  ge_base.views.pr
-00000c20: 6f78 795f 7265 7175 6573 7472 1000 0000  oxy_requestr....
-00000c30: 5a1e 6a65 745f 6272 6964 6765 5f62 6173  Z.jet_bridge_bas
-00000c40: 652e 7669 6577 732e 7265 6769 7374 6572  e.views.register
-00000c50: 7211 0000 005a 1c6a 6574 5f62 7269 6467  r....Z.jet_bridg
-00000c60: 655f 6261 7365 2e76 6965 7773 2e72 656c  e_base.views.rel
-00000c70: 6f61 6472 1200 0000 5a19 6a65 745f 6272  oadr....Z.jet_br
-00000c80: 6964 6765 5f62 6173 652e 7669 6577 732e  idge_base.views.
-00000c90: 7371 6c72 1300 0000 5a1c 6a65 745f 6272  sqlr....Z.jet_br
-00000ca0: 6964 6765 5f62 6173 652e 7669 6577 732e  idge_base.views.
-00000cb0: 7374 6174 7573 7214 0000 005a 1b6a 6574  statusr....Z.jet
-00000cc0: 5f62 7269 6467 655f 6261 7365 2e76 6965  _bridge_base.vie
-00000cd0: 7773 2e74 6162 6c65 7215 0000 005a 226a  ws.tabler....Z"j
-00000ce0: 6574 5f62 7269 6467 655f 6261 7365 2e76  et_bridge_base.v
-00000cf0: 6965 7773 2e74 6162 6c65 5f63 6f6c 756d  iews.table_colum
-00000d00: 6e72 1600 0000 da0a 6a65 745f 6272 6964  nr......jet_brid
-00000d10: 6765 7217 0000 0072 1800 0000 5a18 6a65  ger....r....Z.je
-00000d20: 745f 6272 6964 6765 2e68 616e 646c 6572  t_bridge.handler
-00000d30: 732e 7669 6577 7219 0000 005a 1d6a 6574  s.viewr....Z.jet
-00000d40: 5f62 7269 6467 652e 6861 6e64 6c65 7273  _bridge.handlers
-00000d50: 2e6e 6f74 5f66 6f75 6e64 721a 0000 005a  .not_foundr....Z
-00000d60: 116a 6574 5f62 7269 6467 652e 726f 7574  .jet_bridge.rout
-00000d70: 6572 721b 0000 005a 276a 6574 5f62 7269  err....Z'jet_bri
-00000d80: 6467 655f 6261 7365 2e76 6965 7773 2e74  dge_base.views.t
-00000d90: 7269 6767 6572 5f65 7863 6570 7469 6f6e  rigger_exception
-00000da0: 721c 0000 0072 3800 0000 7236 0000 0072  r....r8...r6...r
-00000db0: 3600 0000 7236 0000 0072 3700 0000 da08  6...r6...r7.....
-00000dc0: 3c6d 6f64 756c 653e 0100 0000 733a 0000  <module>....s:..
-00000dd0: 0008 0208 0108 020c 010c 010c 010c 010c  ................
-00000de0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000df0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000e00: 0214 010c 010c 010c 010c 03              ...........
+00000170: 0100 6400 641b 6c38 6d39 5a39 0100 6400  ..d.d.l8m9Z9..d.
+00000180: 641c 6c3a 6d3b 5a3b 0100 6400 641d 6c3c  d.l:m;Z;..d.d.l<
+00000190: 6d3d 5a3d 0100 641e 641f 8400 5a3e 6401  m=Z=..d.d...Z>d.
+000001a0: 5300 2920 e900 0000 004e 2901 da18 5465  S.) .....N)...Te
+000001b0: 6d70 6f72 6172 7952 6564 6972 6563 7448  mporaryRedirectH
+000001c0: 616e 646c 6572 2901 da11 7365 6e74 7279  andler)...sentry
+000001d0: 5f63 6f6e 7472 6f6c 6c65 7229 01da 0f73  _controller)...s
+000001e0: 6574 5f6d 6178 5f77 6f72 6b65 7273 2901  et_max_workers).
+000001f0: da08 7365 7474 696e 6773 2901 da07 4170  ..settings)...Ap
+00000200: 6956 6965 7729 01da 1644 6973 636f 7665  iView)...Discove
+00000210: 7243 6f6e 6e65 6374 696f 6e56 6965 7729  rConnectionView)
+00000220: 01da 1144 6973 636f 7665 7254 6162 6c65  ...DiscoverTable
+00000230: 5669 6577 2901 da18 4578 7465 726e 616c  View)...External
+00000240: 4175 7468 436f 6d70 6c65 7465 5669 6577  AuthCompleteView
+00000250: 2901 da15 4578 7465 726e 616c 4175 7468  )...ExternalAuth
+00000260: 4c6f 6769 6e56 6965 7729 01da 0b47 7261  LoginView)...Gra
+00000270: 7068 514c 5669 6577 2901 da0f 496d 6167  phQLView)...Imag
+00000280: 6552 6573 697a 6556 6965 7729 01da 0e46  eResizeView)...F
+00000290: 696c 6555 706c 6f61 6456 6965 7729 01da  ileUploadView)..
+000002a0: 0b4d 6573 7361 6765 5669 6577 2901 da0c  .MessageView)...
+000002b0: 4d6f 6465 6c56 6965 7753 6574 2901 da14  ModelViewSet)...
+000002c0: 4d6f 6465 6c44 6573 6372 6970 7469 6f6e  ModelDescription
+000002d0: 5669 6577 2901 da28 4d6f 6465 6c44 6573  View)..(ModelDes
+000002e0: 6372 6970 7469 6f6e 5265 6c61 7469 6f6e  criptionRelation
+000002f0: 7368 6970 4f76 6572 7269 6465 5669 6577  shipOverrideView
+00000300: 2901 da10 5072 6f78 7952 6571 7565 7374  )...ProxyRequest
+00000310: 5669 6577 2901 da0c 5265 6769 7374 6572  View)...Register
+00000320: 5669 6577 2901 da0a 5265 6c6f 6164 5669  View)...ReloadVi
+00000330: 6577 2901 da07 5371 6c56 6965 7729 01da  ew)...SqlView)..
+00000340: 0a53 7461 7475 7356 6965 7729 01da 0954  .StatusView)...T
+00000350: 6162 6c65 5669 6577 2901 da0f 5461 626c  ableView)...Tabl
+00000360: 6543 6f6c 756d 6e56 6965 7729 0372 0500  eColumnView).r..
+00000370: 0000 da05 6d65 6469 61da 0756 4552 5349  ....media..VERSI
+00000380: 4f4e 2901 da0c 7669 6577 5f68 616e 646c  ON)...view_handl
+00000390: 6572 2901 da0f 4e6f 7446 6f75 6e64 4861  er)...NotFoundHa
+000003a0: 6e64 6c65 7229 01da 0652 6f75 7465 7229  ndler)...Router)
+000003b0: 01da 1454 7269 6767 6572 4578 6365 7074  ...TriggerExcept
+000003c0: 696f 6e56 6965 7763 0000 0000 0000 0000  ionViewc........
+000003d0: 0200 0000 1600 0000 4300 0000 739e 0100  ........C...s...
+000003e0: 0074 0083 007d 007c 006a 0164 0174 0274  .t...}.|.j.d.t.t
+000003f0: 0383 0183 0201 007c 006a 0164 0274 0274  .......|.j.d.t.t
+00000400: 0483 0183 0201 007c 006a 0164 0374 0274  .......|.j.d.t.t
+00000410: 0583 0183 0201 0064 0474 0664 0564 0669  .......d.t.d.d.i
+00000420: 0166 0364 0774 0274 0783 0166 0264 0674  .f.d.t.t...f.d.t
+00000430: 0274 0883 0166 0264 0874 0274 0783 0166  .t...f.d.t.t...f
+00000440: 0264 0974 0274 0983 0166 0264 0a74 0274  .d.t.t...f.d.t.t
+00000450: 0a83 0166 0264 0b74 0274 0b83 0166 0264  ...f.d.t.t...f.d
+00000460: 0c74 0274 0c83 0166 0264 0d74 0274 0d83  .t.t...f.d.t.t..
+00000470: 0166 0264 0e74 0274 0e83 0166 0264 0f74  .f.d.t.t...f.d.t
+00000480: 0274 0f83 0166 0264 1074 0274 1083 0166  .t...f.d.t.t...f
+00000490: 0264 1174 0274 1183 0166 0264 1274 0274  .d.t.t...f.d.t.t
+000004a0: 1283 0166 0264 1374 0274 1383 0166 0264  ...f.d.t.t...f.d
+000004b0: 1474 146a 156a 1664 1574 176a 1869 0166  .t.j.j.d.t.j.i.f
+000004c0: 0364 1674 0274 1983 0166 0264 1774 0274  .d.t.t...f.d.t.t
+000004d0: 1a83 0166 0264 1874 0274 1b83 0166 0264  ...f.d.t.t...f.d
+000004e0: 1974 0274 1c83 0166 0267 147d 017c 017c  .t.t...f.g.}.|.|
+000004f0: 006a 1d37 007d 0174 176a 1e74 1f6a 206b  .j.7.}.t.j.t.j k
+00000500: 0290 0172 3e7c 016a 2164 1474 146a 156a  ...r>|.j!d.t.j.j
+00000510: 1664 1574 176a 1869 0166 0383 0101 0074  .d.t.j.i.f.....t
+00000520: 176a 2264 006b 0990 0172 5474 2374 176a  .j"d.k...rTt#t.j
+00000530: 2283 0101 0074 176a 2490 0172 7474 256a  "....t.j$..rtt%j
+00000540: 2674 176a 2464 1a6a 2774 2883 0164 1b64  &t.j$d.j't(..d.d
+00000550: 1c8d 0301 0074 146a 156a 297c 0174 176a  .....t.j.j)|.t.j
+00000560: 2a74 2b74 2c6a 2d6a 2e74 2f6a 3064 1d83  *t+t,j-j.t/j0d..
+00000570: 0274 176a 2a74 176a 3164 1e8d 0653 0029  .t.j*t.j1d...S.)
+00000580: 1f4e 7a1d 2f61 7069 2f6d 6f64 656c 732f  .Nz./api/models/
+00000590: 283f 503c 6d6f 6465 6c3e 5b5e 2f5d 2b29  (?P<model>[^/]+)
+000005a0: 2f7a 252f 6170 692f 7461 626c 6573 2f28  /z%/api/tables/(
+000005b0: 3f50 3c74 6162 6c65 3e5b 5e2f 5d2b 292f  ?P<table>[^/]+)/
+000005c0: 636f 6c75 6d6e 732f 7a0c 2f61 7069 2f74  columns/z./api/t
+000005d0: 6162 6c65 732f fa01 2fda 0375 726c 7a05  ables/../..urlz.
+000005e0: 2f61 7069 2f7a 0a2f 7265 6769 7374 6572  /api/z./register
+000005f0: 2f7a 0e2f 6170 692f 7265 6769 7374 6572  /z./api/register
+00000600: 2f7a 0d2f 6170 692f 6772 6170 6871 6c2f  /z./api/graphql/
+00000610: 7a2f 2f61 7069 2f6d 6f64 656c 5f64 6573  z//api/model_des
+00000620: 6372 6970 7469 6f6e 732f 7265 6c61 7469  criptions/relati
+00000630: 6f6e 7368 6970 5f6f 7665 7272 6964 6573  onship_overrides
+00000640: 2f7a 182f 6170 692f 6d6f 6465 6c5f 6465  /z./api/model_de
+00000650: 7363 7269 7074 696f 6e73 2f7a 092f 6170  scriptions/z./ap
+00000660: 692f 7371 6c2f 7a0e 2f61 7069 2f6d 6573  i/sql/z./api/mes
+00000670: 7361 6765 732f 7a11 2f61 7069 2f66 696c  sages/z./api/fil
+00000680: 655f 7570 6c6f 6164 2f7a 122f 6170 692f  e_upload/z./api/
+00000690: 696d 6167 655f 7265 7369 7a65 2f7a 0c2f  image_resize/z./
+000006a0: 6170 692f 7265 6c6f 6164 2f7a 132f 6170  api/reload/z./ap
+000006b0: 692f 7072 6f78 795f 7265 7175 6573 742f  i/proxy_request/
+000006c0: 7a19 2f61 7069 2f64 6973 636f 7665 722f  z./api/discover/
+000006d0: 636f 6e6e 6563 7469 6f6e 2f7a 152f 6170  connection/z./ap
+000006e0: 692f 6469 7363 6f76 6572 2f74 6162 6c65  i/discover/table
+000006f0: 732f 7a0b 2f6d 6564 6961 2f28 2e2a 29da  s/z./media/(.*).
+00000700: 0470 6174 687a 282f 6170 692f 6578 7465  .pathz(/api/exte
+00000710: 726e 616c 5f61 7574 682f 6c6f 6769 6e2f  rnal_auth/login/
+00000720: 283f 503c 6170 703e 5b5e 2f5d 2b29 2f7a  (?P<app>[^/]+)/z
+00000730: 2b2f 6170 692f 6578 7465 726e 616c 5f61  +/api/external_a
+00000740: 7574 682f 636f 6d70 6c65 7465 2f28 3f50  uth/complete/(?P
+00000750: 3c61 7070 3e5b 5e2f 5d2b 292f 7a0c 2f61  <app>[^/]+)/z./a
+00000760: 7069 2f73 7461 7475 732f 7a17 2f61 7069  pi/status/z./api
+00000770: 2f74 7269 6767 6572 5f65 7863 6570 7469  /trigger_excepti
+00000780: 6f6e 2f7a 0d6a 6574 2d62 7269 6467 6540  on/z.jet-bridge@
+00000790: 7b7d 5429 03da 0364 736e da07 7265 6c65  {}T)...dsn..rele
+000007a0: 6173 65da 0774 6f72 6e61 646f 5a09 7465  ase..tornadoZ.te
+000007b0: 6d70 6c61 7465 7329 06da 0868 616e 646c  mplates)...handl
+000007c0: 6572 73da 0564 6562 7567 5a15 6465 6661  ers..debugZ.defa
+000007d0: 756c 745f 6861 6e64 6c65 725f 636c 6173  ult_handler_clas
+000007e0: 735a 0d74 656d 706c 6174 655f 7061 7468  sZ.template_path
+000007f0: 5a0a 6175 746f 7265 6c6f 6164 5a0d 636f  Z.autoreloadZ.co
+00000800: 6f6b 6965 5f73 6563 7265 7429 3272 1d00  okie_secret)2r..
+00000810: 0000 da08 7265 6769 7374 6572 721b 0000  ....registerr...
+00000820: 0072 0f00 0000 7218 0000 0072 1700 0000  .r....r....r....
+00000830: 7202 0000 0072 1300 0000 7206 0000 0072  r....r....r....r
+00000840: 0b00 0000 7211 0000 0072 1000 0000 7215  ....r....r....r.
+00000850: 0000 0072 0e00 0000 720d 0000 0072 0c00  ...r....r....r..
+00000860: 0000 7214 0000 0072 1200 0000 7207 0000  ..r....r....r...
+00000870: 0072 0800 0000 7224 0000 005a 0377 6562  .r....r$...Z.web
+00000880: 5a11 5374 6174 6963 4669 6c65 4861 6e64  Z.StaticFileHand
+00000890: 6c65 7272 0500 0000 da0a 4d45 4449 415f  lerr......MEDIA_
+000008a0: 524f 4f54 720a 0000 0072 0900 0000 7216  ROOTr....r....r.
+000008b0: 0000 0072 1e00 0000 da04 7572 6c73 da0d  ...r......urls..
+000008c0: 4d45 4449 415f 5354 4f52 4147 4572 1900  MEDIA_STORAGEr..
+000008d0: 0000 da12 4d45 4449 415f 5354 4f52 4147  ....MEDIA_STORAG
+000008e0: 455f 4649 4c45 da06 6170 7065 6e64 da07  E_FILE..append..
+000008f0: 5448 5245 4144 5372 0400 0000 da0a 5345  THREADSr......SE
+00000900: 4e54 5259 5f44 534e 7203 0000 00da 0665  NTRY_DSNr......e
+00000910: 6e61 626c 65da 0666 6f72 6d61 7472 1a00  nable..formatr..
+00000920: 0000 da0b 4170 706c 6963 6174 696f 6eda  ....Application.
+00000930: 0544 4542 5547 721c 0000 00da 026f 7372  .DEBUGr......osr
+00000940: 2100 0000 da04 6a6f 696e da0d 6261 7365  !.....join..base
+00000950: 5f73 6574 7469 6e67 73da 0842 4153 455f  _settings..BASE_
+00000960: 4449 52da 0554 4f4b 454e 2902 5a06 726f  DIR..TOKEN).Z.ro
+00000970: 7574 6572 7229 0000 00a9 0072 3800 0000  uterr).....r8...
+00000980: fa50 2f55 7365 7273 2f66 316e 616c 2f44  .P/Users/f1nal/D
+00000990: 726f 7062 6f78 2f70 7974 686f 6e2f 6a65  ropbox/python/je
+000009a0: 742d 6272 6964 6765 2f73 7263 2f70 6163  t-bridge/src/pac
+000009b0: 6b61 6765 732f 6a65 745f 6272 6964 6765  kages/jet_bridge
+000009c0: 2f6a 6574 5f62 7269 6467 652f 6170 702e  /jet_bridge/app.
+000009d0: 7079 da08 6d61 6b65 5f61 7070 2500 0000  py..make_app%...
+000009e0: 7352 0000 0000 0106 0210 0110 0110 030c  sR..............
+000009f0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00000a00: 010a 010a 010a 010a 010a 010a 0112 010a  ................
+00000a10: 010a 010a 010e 020a 020e 011a 020c 010a  ................
+00000a20: 0208 0104 0104 0108 0108 0306 0102 0104  ................
+00000a30: 0102 010e 0104 0172 3a00 0000 293f 7233  .......r:...)?r3
+00000a40: 0000 00da 0e74 6f72 6e61 646f 2e69 6f6c  .....tornado.iol
+00000a50: 6f6f 7072 2400 0000 5a0b 746f 726e 6164  oopr$...Z.tornad
+00000a60: 6f2e 7765 625a 266a 6574 5f62 7269 6467  o.webZ&jet_bridg
+00000a70: 652e 6861 6e64 6c65 7273 2e74 656d 706f  e.handlers.tempo
+00000a80: 7261 7279 5f72 6564 6972 6563 7472 0200  rary_redirectr..
+00000a90: 0000 5a16 6a65 745f 6272 6964 6765 5f62  ..Z.jet_bridge_b
+00000aa0: 6173 652e 7365 6e74 7279 7203 0000 005a  ase.sentryr....Z
+00000ab0: 206a 6574 5f62 7269 6467 655f 6261 7365   jet_bridge_base
+00000ac0: 2e75 7469 6c73 2e61 7379 6e63 5f65 7865  .utils.async_exe
+00000ad0: 6372 0400 0000 da0f 6a65 745f 6272 6964  cr......jet_brid
+00000ae0: 6765 5f62 6173 6572 0500 0000 7235 0000  ge_baser....r5..
+00000af0: 005a 196a 6574 5f62 7269 6467 655f 6261  .Z.jet_bridge_ba
+00000b00: 7365 2e76 6965 7773 2e61 7069 7206 0000  se.views.apir...
+00000b10: 005a 296a 6574 5f62 7269 6467 655f 6261  .Z)jet_bridge_ba
+00000b20: 7365 2e76 6965 7773 2e64 6973 636f 7665  se.views.discove
+00000b30: 725f 636f 6e6e 6563 7469 6f6e 7207 0000  r_connectionr...
+00000b40: 005a 246a 6574 5f62 7269 6467 655f 6261  .Z$jet_bridge_ba
+00000b50: 7365 2e76 6965 7773 2e64 6973 636f 7665  se.views.discove
+00000b60: 725f 7461 626c 6572 0800 0000 5a2c 6a65  r_tabler....Z,je
+00000b70: 745f 6272 6964 6765 5f62 6173 652e 7669  t_bridge_base.vi
+00000b80: 6577 732e 6578 7465 726e 616c 5f61 7574  ews.external_aut
+00000b90: 682e 636f 6d70 6c65 7465 7209 0000 005a  h.completer....Z
+00000ba0: 296a 6574 5f62 7269 6467 655f 6261 7365  )jet_bridge_base
+00000bb0: 2e76 6965 7773 2e65 7874 6572 6e61 6c5f  .views.external_
+00000bc0: 6175 7468 2e6c 6f67 696e 720a 0000 005a  auth.loginr....Z
+00000bd0: 1d6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
+00000be0: 2e76 6965 7773 2e67 7261 7068 716c 720b  .views.graphqlr.
+00000bf0: 0000 005a 226a 6574 5f62 7269 6467 655f  ...Z"jet_bridge_
+00000c00: 6261 7365 2e76 6965 7773 2e69 6d61 6765  base.views.image
+00000c10: 5f72 6573 697a 6572 0c00 0000 5a21 6a65  _resizer....Z!je
+00000c20: 745f 6272 6964 6765 5f62 6173 652e 7669  t_bridge_base.vi
+00000c30: 6577 732e 6669 6c65 5f75 706c 6f61 6472  ews.file_uploadr
+00000c40: 0d00 0000 5a1d 6a65 745f 6272 6964 6765  ....Z.jet_bridge
+00000c50: 5f62 6173 652e 7669 6577 732e 6d65 7373  _base.views.mess
+00000c60: 6167 6572 0e00 0000 5a1b 6a65 745f 6272  ager....Z.jet_br
+00000c70: 6964 6765 5f62 6173 652e 7669 6577 732e  idge_base.views.
+00000c80: 6d6f 6465 6c72 0f00 0000 5a27 6a65 745f  modelr....Z'jet_
+00000c90: 6272 6964 6765 5f62 6173 652e 7669 6577  bridge_base.view
+00000ca0: 732e 6d6f 6465 6c5f 6465 7363 7269 7074  s.model_descript
+00000cb0: 696f 6e72 1000 0000 5a3d 6a65 745f 6272  ionr....Z=jet_br
+00000cc0: 6964 6765 5f62 6173 652e 7669 6577 732e  idge_base.views.
+00000cd0: 6d6f 6465 6c5f 6465 7363 7269 7074 696f  model_descriptio
+00000ce0: 6e5f 7265 6c61 7469 6f6e 7368 6970 5f6f  n_relationship_o
+00000cf0: 7665 7272 6964 6572 1100 0000 5a23 6a65  verrider....Z#je
+00000d00: 745f 6272 6964 6765 5f62 6173 652e 7669  t_bridge_base.vi
+00000d10: 6577 732e 7072 6f78 795f 7265 7175 6573  ews.proxy_reques
+00000d20: 7472 1200 0000 5a1e 6a65 745f 6272 6964  tr....Z.jet_brid
+00000d30: 6765 5f62 6173 652e 7669 6577 732e 7265  ge_base.views.re
+00000d40: 6769 7374 6572 7213 0000 005a 1c6a 6574  gisterr....Z.jet
+00000d50: 5f62 7269 6467 655f 6261 7365 2e76 6965  _bridge_base.vie
+00000d60: 7773 2e72 656c 6f61 6472 1400 0000 5a19  ws.reloadr....Z.
+00000d70: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+00000d80: 7669 6577 732e 7371 6c72 1500 0000 5a1c  views.sqlr....Z.
+00000d90: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+00000da0: 7669 6577 732e 7374 6174 7573 7216 0000  views.statusr...
+00000db0: 005a 1b6a 6574 5f62 7269 6467 655f 6261  .Z.jet_bridge_ba
+00000dc0: 7365 2e76 6965 7773 2e74 6162 6c65 7217  se.views.tabler.
+00000dd0: 0000 005a 226a 6574 5f62 7269 6467 655f  ...Z"jet_bridge_
+00000de0: 6261 7365 2e76 6965 7773 2e74 6162 6c65  base.views.table
+00000df0: 5f63 6f6c 756d 6e72 1800 0000 da0a 6a65  _columnr......je
+00000e00: 745f 6272 6964 6765 7219 0000 0072 1a00  t_bridger....r..
+00000e10: 0000 5a18 6a65 745f 6272 6964 6765 2e68  ..Z.jet_bridge.h
+00000e20: 616e 646c 6572 732e 7669 6577 721b 0000  andlers.viewr...
+00000e30: 005a 1d6a 6574 5f62 7269 6467 652e 6861  .Z.jet_bridge.ha
+00000e40: 6e64 6c65 7273 2e6e 6f74 5f66 6f75 6e64  ndlers.not_found
+00000e50: 721c 0000 005a 116a 6574 5f62 7269 6467  r....Z.jet_bridg
+00000e60: 652e 726f 7574 6572 721d 0000 005a 276a  e.routerr....Z'j
+00000e70: 6574 5f62 7269 6467 655f 6261 7365 2e76  et_bridge_base.v
+00000e80: 6965 7773 2e74 7269 6767 6572 5f65 7863  iews.trigger_exc
+00000e90: 6570 7469 6f6e 721e 0000 0072 3a00 0000  eptionr....r:...
+00000ea0: 7238 0000 0072 3800 0000 7238 0000 0072  r8...r8...r8...r
+00000eb0: 3900 0000 da08 3c6d 6f64 756c 653e 0100  9.....<module>..
+00000ec0: 0000 733e 0000 0008 0208 0108 020c 010c  ..s>............
+00000ed0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00000ee0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00000ef0: 010c 010c 010c 010c 010c 0214 010c 010c  ................
+00000f00: 010c 010c 03                             .....
```

### Comparing `jet-bridge-1.7.9/jet_bridge/__pycache__/router.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/__pycache__/router.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-00000000: 330d 0d0a 61aa a062 500b 0000 e300 0000  3...a..bP.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4000 0000 6400 6401 6c00 5a00 6400  .s@...d.d.l.Z.d.
-00000030: 6402 6c00 6d01 5a01 0100 6400 6403 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 4700 6405 6406 8400 6406 6506 8303  ..G.d.d...d.e...
-00000060: 5a07 6401 5300 2907 e900 0000 004e 2901  Z.d.S.)......N).
-00000070: da03 6765 6e29 01da 0646 7574 7572 6529  ..gen)...Future)
-00000080: 01da 0961 735f 6675 7475 7265 6300 0000  ...as_futurec...
-00000090: 0000 0000 0000 0000 0007 0000 0040 0000  .............@..
-000000a0: 0073 5800 0000 6500 5a01 6400 5a02 6401  .sX...e.Z.d.Z.d.
-000000b0: 6402 6403 6404 9c02 6405 6406 9c03 6407  d.d.d...d.d...d.
-000000c0: 6408 6409 640a 640b 640c 9c04 640d 6406  d.d.d.d.d...d.d.
-000000d0: 9c03 6702 5a03 6700 5a04 640e 640f 8400  ..g.Z.g.Z.d.d...
-000000e0: 5a05 6410 6411 8400 5a06 6412 6413 8400  Z.d.d...Z.d.d...
-000000f0: 5a07 6414 6415 8400 5a08 6416 5300 2917  Z.d.d...Z.d.S.).
-00000100: da06 526f 7574 6572 da00 da04 6c69 7374  ..Router....list
-00000110: da06 6372 6561 7465 2902 da03 6765 74da  ..create)...get.
-00000120: 0470 6f73 7446 2903 da04 7061 7468 da0e  .postF)...path..
-00000130: 6d65 7468 6f64 5f6d 6170 7069 6e67 da06  method_mapping..
-00000140: 6465 7461 696c 7a0e 283f 503c 706b 3e5b  detailz.(?P<pk>[
-00000150: 5e2f 5d2b 292f da08 7265 7472 6965 7665  ^/]+)/..retrieve
-00000160: da06 7570 6461 7465 da0e 7061 7274 6961  ..update..partia
-00000170: 6c5f 7570 6461 7465 da07 6465 7374 726f  l_update..destro
-00000180: 7929 0472 0900 0000 da03 7075 74da 0570  y).r......put..p
-00000190: 6174 6368 da06 6465 6c65 7465 5463 0400  atch..deleteTc..
-000001a0: 0000 0000 0000 0900 0000 0500 0000 4300  ..............C.
-000001b0: 0000 7356 0000 0047 0064 0164 0284 0064  ..sV...G.d.d...d
-000001c0: 027c 0183 037d 0478 307c 036a 0083 0044  .|...}.x0|.j...D
-000001d0: 005d 245c 027d 057d 0664 0364 0484 007d  .]$\.}.}.d.d...}
-000001e0: 077c 077c 0683 017d 0874 017c 047c 057c  .|.|...}.t.|.|.|
-000001f0: 0883 0301 0071 1a57 007c 006a 026a 037c  .....q.W.|.j.j.|
-00000200: 027c 0466 0283 0101 0064 0053 0029 054e  .|.f.....d.S.).N
-00000210: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00000220: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000230: 5a02 6401 5300 2902 7a29 526f 7574 6572  Z.d.S.).z)Router
-00000240: 2e61 6464 5f68 616e 646c 6572 2e3c 6c6f  .add_handler.<lo
-00000250: 6361 6c73 3e2e 4163 7469 6f6e 4861 6e64  cals>.ActionHand
-00000260: 6c65 724e 2903 da08 5f5f 6e61 6d65 5f5f  lerN)...__name__
-00000270: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000280: 7175 616c 6e61 6d65 5f5f a900 7218 0000  qualname__..r...
-00000290: 0072 1800 0000 fa53 2f55 7365 7273 2f66  .r.....S/Users/f
-000002a0: 316e 616c 2f44 726f 7062 6f78 2f70 7974  1nal/Dropbox/pyt
-000002b0: 686f 6e2f 6a65 742d 6272 6964 6765 2f73  hon/jet-bridge/s
-000002c0: 7263 2f70 6163 6b61 6765 732f 6a65 745f  rc/packages/jet_
-000002d0: 6272 6964 6765 2f6a 6574 5f62 7269 6467  bridge/jet_bridg
-000002e0: 652f 726f 7574 6572 2e70 79da 0d41 6374  e/router.py..Act
-000002f0: 696f 6e48 616e 646c 6572 2000 0000 7302  ionHandler ...s.
-00000300: 0000 0008 0172 1a00 0000 6301 0000 0000  .....r....c.....
-00000310: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00000320: 1600 0000 7400 6a01 8700 6601 6401 6402  ....t.j...f.d.d.
-00000330: 8408 8301 7d01 7c01 5300 2903 4e63 0100  ....}.|.S.).Nc..
-00000340: 0000 0000 0000 0500 0000 0400 0000 3f00  ..............?.
-00000350: 0000 7334 0000 0087 0387 0087 0187 0266  ..s4...........f
-00000360: 0464 0164 0284 087d 0374 007c 0383 0156  .d.d...}.t.|...V
-00000370: 007d 0488 016a 017c 0483 0156 0001 0074  .}...j.|...V...t
-00000380: 026a 0383 0082 0164 0053 0029 034e 6300  .j.....d.S.).Nc.
-00000390: 0000 0000 0000 0002 0000 0003 0000 0013  ................
-000003a0: 0000 0073 3c00 0000 8802 6a00 8300 7d00  ...s<.....j...}.
-000003b0: 8800 7c00 5f01 8802 6a02 7c00 8301 0100  ..|._...j.|.....
-000003c0: 8802 6a03 6a04 8800 7c00 6602 8801 9e02  ..j.j...|.f.....
-000003d0: 8803 8e01 7d01 8802 6a05 7c00 8301 0100  ....}...j.|.....
-000003e0: 7c01 5300 2901 4e29 06da 0b67 6574 5f72  |.S.).N)...get_r
-000003f0: 6571 7565 7374 da06 6163 7469 6f6e da0f  equest..action..
-00000400: 6265 666f 7265 5f64 6973 7061 7463 68da  before_dispatch.
-00000410: 0476 6965 77da 0864 6973 7061 7463 68da  .view..dispatch.
-00000420: 0e61 6674 6572 5f64 6973 7061 7463 6829  .after_dispatch)
-00000430: 02da 0772 6571 7565 7374 da06 7265 7375  ...request..resu
-00000440: 6c74 2904 721c 0000 00da 0461 7267 73da  lt).r......args.
-00000450: 0a69 6e6e 6572 5f73 656c 66da 066b 7761  .inner_self..kwa
-00000460: 7267 7372 1800 0000 7219 0000 00da 0765  rgsr....r......e
-00000470: 7865 6375 7465 2800 0000 730c 0000 0000  xecute(...s.....
-00000480: 0108 0106 010a 0116 010a 017a 5852 6f75  ...........zXRou
-00000490: 7465 722e 6164 645f 6861 6e64 6c65 722e  ter.add_handler.
-000004a0: 3c6c 6f63 616c 733e 2e63 7265 6174 655f  <locals>.create_
-000004b0: 6163 7469 6f6e 5f6d 6574 686f 642e 3c6c  action_method.<l
-000004c0: 6f63 616c 733e 2e61 6374 696f 6e5f 6d65  ocals>.action_me
-000004d0: 7468 6f64 2e3c 6c6f 6361 6c73 3e2e 6578  thod.<locals>.ex
-000004e0: 6563 7574 6529 0472 0400 0000 da0e 7772  ecute).r......wr
-000004f0: 6974 655f 7265 7370 6f6e 7365 7202 0000  ite_responser...
-00000500: 00da 0652 6574 7572 6e29 0572 2400 0000  ...Return).r$...
-00000510: 7223 0000 0072 2500 0000 7226 0000 00da  r#...r%...r&....
-00000520: 0872 6573 706f 6e73 6529 0172 1c00 0000  .response).r....
-00000530: 2903 7223 0000 0072 2400 0000 7225 0000  ).r#...r$...r%..
-00000540: 0072 1900 0000 da0d 6163 7469 6f6e 5f6d  .r......action_m
-00000550: 6574 686f 6425 0000 0073 0800 0000 0003  ethod%...s......
-00000560: 1208 0a02 0c01 7a47 526f 7574 6572 2e61  ......zGRouter.a
-00000570: 6464 5f68 616e 646c 6572 2e3c 6c6f 6361  dd_handler.<loca
-00000580: 6c73 3e2e 6372 6561 7465 5f61 6374 696f  ls>.create_actio
-00000590: 6e5f 6d65 7468 6f64 2e3c 6c6f 6361 6c73  n_method.<locals
-000005a0: 3e2e 6163 7469 6f6e 5f6d 6574 686f 6429  >.action_method)
-000005b0: 0272 0200 0000 da09 636f 726f 7574 696e  .r......coroutin
-000005c0: 6529 0272 1c00 0000 722a 0000 0072 1800  e).r....r*...r..
-000005d0: 0000 2901 721c 0000 0072 1900 0000 da14  ..).r....r......
-000005e0: 6372 6561 7465 5f61 6374 696f 6e5f 6d65  create_action_me
-000005f0: 7468 6f64 2400 0000 7304 0000 0000 0112  thod$...s.......
-00000600: 107a 3052 6f75 7465 722e 6164 645f 6861  .z0Router.add_ha
-00000610: 6e64 6c65 722e 3c6c 6f63 616c 733e 2e63  ndler.<locals>.c
-00000620: 7265 6174 655f 6163 7469 6f6e 5f6d 6574  reate_action_met
-00000630: 686f 6429 04da 0569 7465 6d73 da07 7365  hod)...items..se
-00000640: 7461 7474 72da 0475 726c 73da 0661 7070  tattr..urls..app
-00000650: 656e 6429 09da 0473 656c 6672 1e00 0000  end)...selfr....
-00000660: da03 7572 6cda 0761 6374 696f 6e73 721a  ..url..actionsr.
-00000670: 0000 00da 066d 6574 686f 645a 0d6d 6574  .....methodZ.met
-00000680: 686f 645f 6163 7469 6f6e 722c 0000 00da  hod_actionr,....
-00000690: 0466 756e 6372 1800 0000 7218 0000 0072  .funcr....r....r
-000006a0: 1900 0000 da0b 6164 645f 6861 6e64 6c65  ......add_handle
-000006b0: 721f 0000 0073 0c00 0000 0001 1003 1201  r....s..........
-000006c0: 0813 0801 1002 7a12 526f 7574 6572 2e61  ......z.Router.a
-000006d0: 6464 5f68 616e 646c 6572 6304 0000 0000  dd_handlerc.....
-000006e0: 0000 0006 0000 0005 0000 0003 0000 0073  ...............s
-000006f0: 5a00 0000 7c01 6a00 8900 7c02 6401 1900  Z...|.j...|.d...
-00000700: 7d04 7401 7402 8700 6601 6402 6403 8408  }.t.t...f.d.d...
-00000710: 7c04 6a03 8300 8302 8301 7d04 7404 7c04  |.j.......}.t.|.
-00000720: 8301 6404 6b02 7238 6400 5300 6405 6a05  ..d.k.r8d.S.d.j.
-00000730: 7c03 7c02 6406 1900 8302 7d05 7c00 6a06  |.|.d.....}.|.j.
-00000740: 7c01 7c05 7c04 8303 0100 6400 5300 2907  |.|.|.....d.S.).
-00000750: 4e72 0c00 0000 6301 0000 0000 0000 0001  Nr....c.........
-00000760: 0000 0004 0000 0013 0000 0073 0e00 0000  ...........s....
-00000770: 7400 8800 7c00 6401 1900 8302 5300 2902  t...|.d.....S.).
-00000780: 4ee9 0100 0000 2901 da07 6861 7361 7474  N.....)...hasatt
-00000790: 7229 01da 0178 2901 da07 7669 6577 7365  r)...x)...viewse
-000007a0: 7472 1800 0000 7219 0000 00da 083c 6c61  tr....r......<la
-000007b0: 6d62 6461 3e3f 0000 0073 0000 0000 7a2a  mbda>?...s....z*
-000007c0: 526f 7574 6572 2e61 6464 5f72 6f75 7465  Router.add_route
-000007d0: 5f61 6374 696f 6e73 2e3c 6c6f 6361 6c73  _actions.<locals
-000007e0: 3e2e 3c6c 616d 6264 613e 7201 0000 007a  >.<lambda>r....z
-000007f0: 047b 7d7b 7d72 0b00 0000 2907 721e 0000  .{}{}r....).r...
-00000800: 00da 0464 6963 74da 0666 696c 7465 7272  ...dict..filterr
-00000810: 2d00 0000 da03 6c65 6eda 0666 6f72 6d61  -.....len..forma
-00000820: 7472 3600 0000 2906 7231 0000 0072 1e00  tr6...).r1...r..
-00000830: 0000 da05 726f 7574 65da 0670 7265 6669  ....route..prefi
-00000840: 7872 3300 0000 7232 0000 0072 1800 0000  xr3...r2...r....
-00000850: 2901 723a 0000 0072 1900 0000 da11 6164  ).r:...r......ad
-00000860: 645f 726f 7574 655f 6163 7469 6f6e 733c  d_route_actions<
-00000870: 0000 0073 0e00 0000 0001 0601 0801 1a02  ...s............
-00000880: 0c01 0402 1001 7a18 526f 7574 6572 2e61  ......z.Router.a
-00000890: 6464 5f72 6f75 7465 5f61 6374 696f 6e73  dd_route_actions
-000008a0: 6304 0000 0000 0000 000a 0000 0006 0000  c...............
-000008b0: 0003 0000 0073 8c00 0000 7c01 6a00 7d04  .....s....|.j.}.
-000008c0: 7880 7401 7c04 8301 4400 5d74 8900 7402  x.t.|...D.]t..t.
-000008d0: 7c04 8800 8302 7d05 7402 7c05 6401 6400  |.....}.t.|.d.d.
-000008e0: 8303 7d06 7c06 6400 6b08 7234 7110 7402  ..}.|.d.k.r4q.t.
-000008f0: 7c05 6402 6400 8303 7d07 7c07 7c02 6402  |.d.d...}.|.|.d.
-00000900: 1900 6b03 724e 7110 7403 7404 8700 6601  ..k.rNq.t.t...f.
-00000910: 6403 6404 8408 7c06 8302 8301 7d08 6405  d.d...|.....}.d.
-00000920: 6a05 7c03 7c02 6406 1900 8800 8303 7d09  j.|.|.d.......}.
-00000930: 7c00 6a06 7c01 7c09 7c08 8303 0100 7110  |.j.|.|.|.....q.
-00000940: 5700 6400 5300 2907 4eda 0f62 696e 645f  W.d.S.).N..bind_
-00000950: 746f 5f6d 6574 686f 6473 720d 0000 0063  to_methodsr....c
-00000960: 0100 0000 0000 0000 0100 0000 0200 0000  ................
-00000970: 1300 0000 7308 0000 007c 0088 0066 0253  ....s....|...f.S
-00000980: 0029 014e 7218 0000 0029 0172 3900 0000  .).Nr....).r9...
-00000990: 2901 da04 6174 7472 7218 0000 0072 1900  )...attrr....r..
-000009a0: 0000 723b 0000 0055 0000 0073 0000 0000  ..r;...U...s....
-000009b0: 7a30 526f 7574 6572 2e61 6464 5f72 6f75  z0Router.add_rou
-000009c0: 7465 5f65 7874 7261 5f61 6374 696f 6e73  te_extra_actions
-000009d0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-000009e0: 613e 7a07 7b7d 7b7d 7b7d 2f72 0b00 0000  a>z.{}{}{}/r....
-000009f0: 2907 721e 0000 00da 0364 6972 da07 6765  ).r......dir..ge
-00000a00: 7461 7474 7272 3c00 0000 da03 6d61 7072  tattrr<.....mapr
-00000a10: 3f00 0000 7236 0000 0029 0a72 3100 0000  ?...r6...).r1...
-00000a20: 721e 0000 0072 4000 0000 7241 0000 0072  r....r@...rA...r
-00000a30: 3a00 0000 7234 0000 0072 4300 0000 720d  :...r4...rC...r.
-00000a40: 0000 005a 0d65 7874 7261 5f61 6374 696f  ...Z.extra_actio
-00000a50: 6e73 7232 0000 0072 1800 0000 2901 7244  nsr2...r....).rD
-00000a60: 0000 0072 1900 0000 da17 6164 645f 726f  ...r......add_ro
-00000a70: 7574 655f 6578 7472 615f 6163 7469 6f6e  ute_extra_action
-00000a80: 7347 0000 0073 1800 0000 0001 0601 0e01  sG...s..........
-00000a90: 0a01 0c02 0801 0202 0c02 0c01 0202 1602  ................
-00000aa0: 1201 7a1e 526f 7574 6572 2e61 6464 5f72  ..z.Router.add_r
-00000ab0: 6f75 7465 5f65 7874 7261 5f61 6374 696f  oute_extra_actio
-00000ac0: 6e73 6303 0000 0000 0000 0004 0000 0005  nsc.............
-00000ad0: 0000 0043 0000 0073 4000 0000 781c 7c00  ...C...s@...x.|.
-00000ae0: 6a00 4400 5d12 7d03 7c00 6a01 7c02 7c03  j.D.].}.|.j.|.|.
-00000af0: 7c01 8303 0100 7108 5700 781c 7c00 6a00  |.....q.W.x.|.j.
-00000b00: 4400 5d12 7d03 7c00 6a02 7c02 7c03 7c01  D.].}.|.j.|.|.|.
-00000b10: 8303 0100 7126 5700 6400 5300 2901 4e29  ....q&W.d.S.).N)
-00000b20: 03da 0672 6f75 7465 7372 4800 0000 7242  ...routesrH...rB
-00000b30: 0000 0029 0472 3100 0000 7241 0000 0072  ...).r1...rA...r
-00000b40: 1e00 0000 7240 0000 0072 1800 0000 7218  ....r@...r....r.
-00000b50: 0000 0072 1900 0000 da08 7265 6769 7374  ...r......regist
-00000b60: 6572 5a00 0000 7308 0000 0000 010c 0112  erZ...s.........
-00000b70: 020c 017a 0f52 6f75 7465 722e 7265 6769  ...z.Router.regi
-00000b80: 7374 6572 4e29 0972 1500 0000 7216 0000  sterN).r....r...
-00000b90: 0072 1700 0000 7249 0000 0072 2f00 0000  .r....rI...r/...
-00000ba0: 7236 0000 0072 4200 0000 7248 0000 0072  r6...rB...rH...r
-00000bb0: 4a00 0000 7218 0000 0072 1800 0000 7218  J...r....r....r.
-00000bc0: 0000 0072 1900 0000 7205 0000 0008 0000  ...r....r.......
-00000bd0: 0073 1e00 0000 0803 0202 0201 0602 0603  .s..............
-00000be0: 0202 0201 0201 0201 0602 0a03 0402 081d  ................
-00000bf0: 080b 0813 7205 0000 0029 08da 0774 6f72  ....r....)...tor
-00000c00: 6e61 646f 7202 0000 00da 1274 6f72 6e61  nador......torna
-00000c10: 646f 2e63 6f6e 6375 7272 656e 7472 0300  do.concurrentr..
-00000c20: 0000 da20 6a65 745f 6272 6964 6765 5f62  ... jet_bridge_b
-00000c30: 6173 652e 7574 696c 732e 6173 796e 635f  ase.utils.async_
-00000c40: 6578 6563 7204 0000 00da 066f 626a 6563  execr......objec
-00000c50: 7472 0500 0000 7218 0000 0072 1800 0000  tr....r....r....
-00000c60: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
-00000c70: 756c 653e 0100 0000 7308 0000 0008 010c  ule>....s.......
-00000c80: 010c 020c 03                             .....
+00000000: 420d 0d0a 0000 0000 61aa a062 500b 0000  B.......a..bP...
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 4000 0000 6400 6401 6c00  .@...s@...d.d.l.
+00000030: 5a00 6400 6402 6c00 6d01 5a01 0100 6400  Z.d.d.l.m.Z...d.
+00000040: 6403 6c02 6d03 5a03 0100 6400 6404 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
+00000060: 6506 8303 5a07 6401 5300 2907 e900 0000  e...Z.d.S.).....
+00000070: 004e 2901 da03 6765 6e29 01da 0646 7574  .N)...gen)...Fut
+00000080: 7572 6529 01da 0961 735f 6675 7475 7265  ure)...as_future
+00000090: 6300 0000 0000 0000 0000 0000 0007 0000  c...............
+000000a0: 0040 0000 0073 5800 0000 6500 5a01 6400  .@...sX...e.Z.d.
+000000b0: 5a02 6401 6402 6403 6404 9c02 6405 6406  Z.d.d.d.d...d.d.
+000000c0: 9c03 6407 6408 6409 640a 640b 640c 9c04  ..d.d.d.d.d.d...
+000000d0: 640d 6406 9c03 6702 5a03 6700 5a04 640e  d.d...g.Z.g.Z.d.
+000000e0: 640f 8400 5a05 6410 6411 8400 5a06 6412  d...Z.d.d...Z.d.
+000000f0: 6413 8400 5a07 6414 6415 8400 5a08 6416  d...Z.d.d...Z.d.
+00000100: 5300 2917 da06 526f 7574 6572 da00 da04  S.)...Router....
+00000110: 6c69 7374 da06 6372 6561 7465 2902 da03  list..create)...
+00000120: 6765 74da 0470 6f73 7446 2903 da04 7061  get..postF)...pa
+00000130: 7468 da0e 6d65 7468 6f64 5f6d 6170 7069  th..method_mappi
+00000140: 6e67 da06 6465 7461 696c 7a0e 283f 503c  ng..detailz.(?P<
+00000150: 706b 3e5b 5e2f 5d2b 292f da08 7265 7472  pk>[^/]+)/..retr
+00000160: 6965 7665 da06 7570 6461 7465 da0e 7061  ieve..update..pa
+00000170: 7274 6961 6c5f 7570 6461 7465 da07 6465  rtial_update..de
+00000180: 7374 726f 7929 0472 0900 0000 da03 7075  stroy).r......pu
+00000190: 74da 0570 6174 6368 da06 6465 6c65 7465  t..patch..delete
+000001a0: 5463 0400 0000 0000 0000 0900 0000 0500  Tc..............
+000001b0: 0000 4300 0000 7356 0000 0047 0064 0164  ..C...sV...G.d.d
+000001c0: 0284 0064 027c 0183 037d 0478 307c 03a0  ...d.|...}.x0|..
+000001d0: 00a1 0044 005d 245c 027d 057d 0664 0364  ...D.]$\.}.}.d.d
+000001e0: 0484 007d 077c 077c 0683 017d 0874 017c  ...}.|.|...}.t.|
+000001f0: 047c 057c 0883 0301 0071 1a57 007c 006a  .|.|.....q.W.|.j
+00000200: 02a0 037c 027c 0466 02a1 0101 0064 0053  ...|.|.f.....d.S
+00000210: 0029 054e 6300 0000 0000 0000 0000 0000  .).Nc...........
+00000220: 0001 0000 0040 0000 0073 0c00 0000 6500  .....@...s....e.
+00000230: 5a01 6400 5a02 6401 5300 2902 7a29 526f  Z.d.Z.d.S.).z)Ro
+00000240: 7574 6572 2e61 6464 5f68 616e 646c 6572  uter.add_handler
+00000250: 2e3c 6c6f 6361 6c73 3e2e 4163 7469 6f6e  .<locals>.Action
+00000260: 4861 6e64 6c65 724e 2903 da08 5f5f 6e61  HandlerN)...__na
+00000270: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000280: da0c 5f5f 7175 616c 6e61 6d65 5f5f a900  ..__qualname__..
+00000290: 7218 0000 0072 1800 0000 fa53 2f55 7365  r....r.....S/Use
+000002a0: 7273 2f66 316e 616c 2f44 726f 7062 6f78  rs/f1nal/Dropbox
+000002b0: 2f70 7974 686f 6e2f 6a65 742d 6272 6964  /python/jet-brid
+000002c0: 6765 2f73 7263 2f70 6163 6b61 6765 732f  ge/src/packages/
+000002d0: 6a65 745f 6272 6964 6765 2f6a 6574 5f62  jet_bridge/jet_b
+000002e0: 7269 6467 652f 726f 7574 6572 2e70 79da  ridge/router.py.
+000002f0: 0d41 6374 696f 6e48 616e 646c 6572 2000  .ActionHandler .
+00000300: 0000 7302 0000 0008 0172 1a00 0000 6301  ..s......r....c.
+00000310: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00000320: 0000 0073 1600 0000 7400 6a01 8700 6601  ...s....t.j...f.
+00000330: 6401 6402 8408 8301 7d01 7c01 5300 2903  d.d.....}.|.S.).
+00000340: 4e63 0100 0000 0000 0000 0500 0000 0400  Nc..............
+00000350: 0000 3f00 0000 7334 0000 0087 0387 0087  ..?...s4........
+00000360: 0187 0266 0464 0164 0284 087d 0374 007c  ...f.d.d...}.t.|
+00000370: 0383 0156 007d 0488 01a0 017c 04a1 0156  ...V.}.....|...V
+00000380: 0001 0074 02a0 03a1 0082 0164 0053 0029  ...t.......d.S.)
+00000390: 034e 6300 0000 0000 0000 0002 0000 0003  .Nc.............
+000003a0: 0000 0013 0000 0073 3c00 0000 8802 a000  .......s<.......
+000003b0: a100 7d00 8800 7c00 5f01 8802 a002 7c00  ..}...|._.....|.
+000003c0: a101 0100 8802 6a03 6a04 8800 7c00 6602  ......j.j...|.f.
+000003d0: 8801 9e02 8803 8e01 7d01 8802 a005 7c00  ........}.....|.
+000003e0: a101 0100 7c01 5300 2901 4e29 06da 0b67  ....|.S.).N)...g
+000003f0: 6574 5f72 6571 7565 7374 da06 6163 7469  et_request..acti
+00000400: 6f6e da0f 6265 666f 7265 5f64 6973 7061  on..before_dispa
+00000410: 7463 68da 0476 6965 77da 0864 6973 7061  tch..view..dispa
+00000420: 7463 68da 0e61 6674 6572 5f64 6973 7061  tch..after_dispa
+00000430: 7463 6829 02da 0772 6571 7565 7374 da06  tch)...request..
+00000440: 7265 7375 6c74 2904 721c 0000 00da 0461  result).r......a
+00000450: 7267 73da 0a69 6e6e 6572 5f73 656c 66da  rgs..inner_self.
+00000460: 066b 7761 7267 7372 1800 0000 7219 0000  .kwargsr....r...
+00000470: 00da 0765 7865 6375 7465 2800 0000 730c  ...execute(...s.
+00000480: 0000 0000 0108 0106 010a 0116 010a 017a  ...............z
+00000490: 5852 6f75 7465 722e 6164 645f 6861 6e64  XRouter.add_hand
+000004a0: 6c65 722e 3c6c 6f63 616c 733e 2e63 7265  ler.<locals>.cre
+000004b0: 6174 655f 6163 7469 6f6e 5f6d 6574 686f  ate_action_metho
+000004c0: 642e 3c6c 6f63 616c 733e 2e61 6374 696f  d.<locals>.actio
+000004d0: 6e5f 6d65 7468 6f64 2e3c 6c6f 6361 6c73  n_method.<locals
+000004e0: 3e2e 6578 6563 7574 6529 0472 0400 0000  >.execute).r....
+000004f0: da0e 7772 6974 655f 7265 7370 6f6e 7365  ..write_response
+00000500: 7202 0000 00da 0652 6574 7572 6e29 0572  r......Return).r
+00000510: 2400 0000 7223 0000 0072 2500 0000 7226  $...r#...r%...r&
+00000520: 0000 00da 0872 6573 706f 6e73 6529 0172  .....response).r
+00000530: 1c00 0000 2903 7223 0000 0072 2400 0000  ....).r#...r$...
+00000540: 7225 0000 0072 1900 0000 da0d 6163 7469  r%...r......acti
+00000550: 6f6e 5f6d 6574 686f 6425 0000 0073 0800  on_method%...s..
+00000560: 0000 0003 1208 0a02 0c01 7a47 526f 7574  ..........zGRout
+00000570: 6572 2e61 6464 5f68 616e 646c 6572 2e3c  er.add_handler.<
+00000580: 6c6f 6361 6c73 3e2e 6372 6561 7465 5f61  locals>.create_a
+00000590: 6374 696f 6e5f 6d65 7468 6f64 2e3c 6c6f  ction_method.<lo
+000005a0: 6361 6c73 3e2e 6163 7469 6f6e 5f6d 6574  cals>.action_met
+000005b0: 686f 6429 0272 0200 0000 da09 636f 726f  hod).r......coro
+000005c0: 7574 696e 6529 0272 1c00 0000 722a 0000  utine).r....r*..
+000005d0: 0072 1800 0000 2901 721c 0000 0072 1900  .r....).r....r..
+000005e0: 0000 da14 6372 6561 7465 5f61 6374 696f  ....create_actio
+000005f0: 6e5f 6d65 7468 6f64 2400 0000 7304 0000  n_method$...s...
+00000600: 0000 0112 107a 3052 6f75 7465 722e 6164  .....z0Router.ad
+00000610: 645f 6861 6e64 6c65 722e 3c6c 6f63 616c  d_handler.<local
+00000620: 733e 2e63 7265 6174 655f 6163 7469 6f6e  s>.create_action
+00000630: 5f6d 6574 686f 6429 04da 0569 7465 6d73  _method)...items
+00000640: da07 7365 7461 7474 72da 0475 726c 73da  ..setattr..urls.
+00000650: 0661 7070 656e 6429 09da 0473 656c 6672  .append)...selfr
+00000660: 1e00 0000 da03 7572 6cda 0761 6374 696f  ......url..actio
+00000670: 6e73 721a 0000 00da 066d 6574 686f 645a  nsr......methodZ
+00000680: 0d6d 6574 686f 645f 6163 7469 6f6e 722c  .method_actionr,
+00000690: 0000 00da 0466 756e 6372 1800 0000 7218  .....funcr....r.
+000006a0: 0000 0072 1900 0000 da0b 6164 645f 6861  ...r......add_ha
+000006b0: 6e64 6c65 721f 0000 0073 0c00 0000 0001  ndler....s......
+000006c0: 1003 1201 0813 0801 1002 7a12 526f 7574  ..........z.Rout
+000006d0: 6572 2e61 6464 5f68 616e 646c 6572 6304  er.add_handlerc.
+000006e0: 0000 0000 0000 0006 0000 0005 0000 0003  ................
+000006f0: 0000 0073 5a00 0000 7c01 6a00 8900 7c02  ...sZ...|.j...|.
+00000700: 6401 1900 7d04 7401 7402 8700 6601 6402  d...}.t.t...f.d.
+00000710: 6403 8408 7c04 a003 a100 8302 8301 7d04  d...|.........}.
+00000720: 7404 7c04 8301 6404 6b02 7238 6400 5300  t.|...d.k.r8d.S.
+00000730: 6405 a005 7c03 7c02 6406 1900 a102 7d05  d...|.|.d.....}.
+00000740: 7c00 a006 7c01 7c05 7c04 a103 0100 6400  |...|.|.|.....d.
+00000750: 5300 2907 4e72 0c00 0000 6301 0000 0000  S.).Nr....c.....
+00000760: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
+00000770: 0e00 0000 7400 8800 7c00 6401 1900 8302  ....t...|.d.....
+00000780: 5300 2902 4ee9 0100 0000 2901 da07 6861  S.).N.....)...ha
+00000790: 7361 7474 7229 01da 0178 2901 da07 7669  sattr)...x)...vi
+000007a0: 6577 7365 7472 1800 0000 7219 0000 00da  ewsetr....r.....
+000007b0: 083c 6c61 6d62 6461 3e3f 0000 00f3 0000  .<lambda>?......
+000007c0: 0000 7a2a 526f 7574 6572 2e61 6464 5f72  ..z*Router.add_r
+000007d0: 6f75 7465 5f61 6374 696f 6e73 2e3c 6c6f  oute_actions.<lo
+000007e0: 6361 6c73 3e2e 3c6c 616d 6264 613e 7201  cals>.<lambda>r.
+000007f0: 0000 007a 047b 7d7b 7d72 0b00 0000 2907  ...z.{}{}r....).
+00000800: 721e 0000 00da 0464 6963 74da 0666 696c  r......dict..fil
+00000810: 7465 7272 2d00 0000 da03 6c65 6eda 0666  terr-.....len..f
+00000820: 6f72 6d61 7472 3600 0000 2906 7231 0000  ormatr6...).r1..
+00000830: 0072 1e00 0000 da05 726f 7574 65da 0670  .r......route..p
+00000840: 7265 6669 7872 3300 0000 7232 0000 0072  refixr3...r2...r
+00000850: 1800 0000 2901 723a 0000 0072 1900 0000  ....).r:...r....
+00000860: da11 6164 645f 726f 7574 655f 6163 7469  ..add_route_acti
+00000870: 6f6e 733c 0000 0073 0e00 0000 0001 0601  ons<...s........
+00000880: 0801 1a02 0c01 0402 1001 7a18 526f 7574  ..........z.Rout
+00000890: 6572 2e61 6464 5f72 6f75 7465 5f61 6374  er.add_route_act
+000008a0: 696f 6e73 6304 0000 0000 0000 000a 0000  ionsc...........
+000008b0: 0006 0000 0003 0000 0073 8c00 0000 7c01  .........s....|.
+000008c0: 6a00 7d04 7880 7401 7c04 8301 4400 5d74  j.}.x.t.|...D.]t
+000008d0: 8900 7402 7c04 8800 8302 7d05 7402 7c05  ..t.|.....}.t.|.
+000008e0: 6401 6400 8303 7d06 7c06 6400 6b08 7234  d.d...}.|.d.k.r4
+000008f0: 7110 7402 7c05 6402 6400 8303 7d07 7c07  q.t.|.d.d...}.|.
+00000900: 7c02 6402 1900 6b03 724e 7110 7403 7404  |.d...k.rNq.t.t.
+00000910: 8700 6601 6403 6404 8408 7c06 8302 8301  ..f.d.d...|.....
+00000920: 7d08 6405 a005 7c03 7c02 6406 1900 8800  }.d...|.|.d.....
+00000930: a103 7d09 7c00 a006 7c01 7c09 7c08 a103  ..}.|...|.|.|...
+00000940: 0100 7110 5700 6400 5300 2907 4eda 0f62  ..q.W.d.S.).N..b
+00000950: 696e 645f 746f 5f6d 6574 686f 6473 720d  ind_to_methodsr.
+00000960: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
+00000970: 0200 0000 1300 0000 7308 0000 007c 0088  ........s....|..
+00000980: 0066 0253 0029 014e 7218 0000 0029 0172  .f.S.).Nr....).r
+00000990: 3900 0000 2901 da04 6174 7472 7218 0000  9...)...attrr...
+000009a0: 0072 1900 0000 723b 0000 0055 0000 0072  .r....r;...U...r
+000009b0: 3c00 0000 7a30 526f 7574 6572 2e61 6464  <...z0Router.add
+000009c0: 5f72 6f75 7465 5f65 7874 7261 5f61 6374  _route_extra_act
+000009d0: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 3c6c  ions.<locals>.<l
+000009e0: 616d 6264 613e 7a07 7b7d 7b7d 7b7d 2f72  ambda>z.{}{}{}/r
+000009f0: 0b00 0000 2907 721e 0000 00da 0364 6972  ....).r......dir
+00000a00: da07 6765 7461 7474 7272 3d00 0000 da03  ..getattrr=.....
+00000a10: 6d61 7072 4000 0000 7236 0000 0029 0a72  mapr@...r6...).r
+00000a20: 3100 0000 721e 0000 0072 4100 0000 7242  1...r....rA...rB
+00000a30: 0000 0072 3a00 0000 7234 0000 0072 4400  ...r:...r4...rD.
+00000a40: 0000 720d 0000 005a 0d65 7874 7261 5f61  ..r....Z.extra_a
+00000a50: 6374 696f 6e73 7232 0000 0072 1800 0000  ctionsr2...r....
+00000a60: 2901 7245 0000 0072 1900 0000 da17 6164  ).rE...r......ad
+00000a70: 645f 726f 7574 655f 6578 7472 615f 6163  d_route_extra_ac
+00000a80: 7469 6f6e 7347 0000 0073 1800 0000 0001  tionsG...s......
+00000a90: 0601 0e01 0a01 0c02 0801 0202 0c02 0c01  ................
+00000aa0: 0202 1602 1201 7a1e 526f 7574 6572 2e61  ......z.Router.a
+00000ab0: 6464 5f72 6f75 7465 5f65 7874 7261 5f61  dd_route_extra_a
+00000ac0: 6374 696f 6e73 6303 0000 0000 0000 0004  ctionsc.........
+00000ad0: 0000 0006 0000 0043 0000 0073 4000 0000  .......C...s@...
+00000ae0: 781c 7c00 6a00 4400 5d12 7d03 7c00 a001  x.|.j.D.].}.|...
+00000af0: 7c02 7c03 7c01 a103 0100 7108 5700 781c  |.|.|.....q.W.x.
+00000b00: 7c00 6a00 4400 5d12 7d03 7c00 a002 7c02  |.j.D.].}.|...|.
+00000b10: 7c03 7c01 a103 0100 7126 5700 6400 5300  |.|.....q&W.d.S.
+00000b20: 2901 4e29 03da 0672 6f75 7465 7372 4900  ).N)...routesrI.
+00000b30: 0000 7243 0000 0029 0472 3100 0000 7242  ..rC...).r1...rB
+00000b40: 0000 0072 1e00 0000 7241 0000 0072 1800  ...r....rA...r..
+00000b50: 0000 7218 0000 0072 1900 0000 da08 7265  ..r....r......re
+00000b60: 6769 7374 6572 5a00 0000 7308 0000 0000  gisterZ...s.....
+00000b70: 010c 0112 020c 017a 0f52 6f75 7465 722e  .......z.Router.
+00000b80: 7265 6769 7374 6572 4e29 0972 1500 0000  registerN).r....
+00000b90: 7216 0000 0072 1700 0000 724a 0000 0072  r....r....rJ...r
+00000ba0: 2f00 0000 7236 0000 0072 4300 0000 7249  /...r6...rC...rI
+00000bb0: 0000 0072 4b00 0000 7218 0000 0072 1800  ...rK...r....r..
+00000bc0: 0000 7218 0000 0072 1900 0000 7205 0000  ..r....r....r...
+00000bd0: 0008 0000 0073 1e00 0000 0803 0202 0201  .....s..........
+00000be0: 0602 0603 0202 0201 0201 0201 0602 0a03  ................
+00000bf0: 0402 081d 080b 0813 7205 0000 0029 08da  ........r....)..
+00000c00: 0774 6f72 6e61 646f 7202 0000 00da 1274  .tornador......t
+00000c10: 6f72 6e61 646f 2e63 6f6e 6375 7272 656e  ornado.concurren
+00000c20: 7472 0300 0000 da20 6a65 745f 6272 6964  tr..... jet_brid
+00000c30: 6765 5f62 6173 652e 7574 696c 732e 6173  ge_base.utils.as
+00000c40: 796e 635f 6578 6563 7204 0000 00da 066f  ync_execr......o
+00000c50: 626a 6563 7472 0500 0000 7218 0000 0072  bjectr....r....r
+00000c60: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
+00000c70: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000c80: 0008 010c 010c 020c 03                   .........
```

### Comparing `jet-bridge-1.7.9/jet_bridge/__pycache__/settings.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/__pycache__/settings.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,321 +1,329 @@
-00000000: 330d 0d0a 76b0 eb63 dd18 0000 e300 0000  3...v..c........
-00000010: 0000 0000 0000 0000 001e 0000 0040 0000  .............@..
-00000020: 0073 8e05 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 6d04 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 0100 6501  d.l.m.Z.m.Z...e.
-00000070: 6a0c 6a0d 6501 6a0c 6a0e 650f 8301 8301  j.j.e.j.j.e.....
-00000080: 5a10 6501 6a0c 6a11 6406 8301 5a12 6407  Z.e.j.j.d...Z.d.
-00000090: 5a13 6408 5a14 6503 6409 640a 640b 640c  Z.d.Z.e.d.d.d.d.
-000000a0: 8d03 0100 6503 640d 640e 640f 6515 6410  ....e.d.d.d.e.d.
-000000b0: 8d04 0100 6503 6411 6412 6413 6515 6410  ....e.d.d.d.e.d.
-000000c0: 8d04 0100 6503 6414 6512 6415 640c 8d03  ....e.d.e.d.d...
-000000d0: 0100 6503 6416 6417 6418 640c 8d03 0100  ..e.d.d.d.d.....
-000000e0: 6503 6419 641a 641b 6516 6410 8d04 0100  e.d.d.d.e.d.....
-000000f0: 6503 641c 641a 641d 6516 6410 8d04 0100  e.d.d.d.e.d.....
-00000100: 6503 641e 6401 641e 6515 6410 8d04 0100  e.d.d.d.e.d.....
-00000110: 6503 641f 6420 6421 6515 6410 8d04 0100  e.d.d d!e.d.....
-00000120: 6503 6422 6423 6424 6516 6410 8d04 0100  e.d"d#d$e.d.....
-00000130: 6503 6425 6425 6517 6426 8d03 0100 6503  e.d%d%e.d&....e.
-00000140: 6427 6427 6517 6426 8d03 0100 6503 6428  d'd'e.d&....e.d(
-00000150: 6428 6517 6426 8d03 0100 6503 6429 6423  d(e.d&....e.d)d#
-00000160: 642a 6516 6410 8d04 0100 6503 642b 642c  d*e.d.....e.d+d,
-00000170: 6517 6426 8d03 0100 6503 642d 642e 6517  e.d&....e.d-d.e.
-00000180: 6401 642f 8d04 0100 6503 6430 6431 6517  d.d/....e.d0d1e.
-00000190: 6401 642f 8d04 0100 6503 6432 6433 6517  d.d/....e.d2d3e.
-000001a0: 6401 642f 8d04 0100 6503 6434 6513 6435  d.d/....e.d4e.d5
-000001b0: 640c 8d03 0100 6503 6436 6514 6437 640c  d.....e.d6e.d7d.
-000001c0: 8d03 0100 6503 6438 6508 6a18 6439 640c  ....e.d8e.j.d9d.
-000001d0: 8d03 0100 6503 643a 643b 643c 640c 8d03  ....e.d:d;d<d...
-000001e0: 0100 6503 643d 6401 643e 640c 8d03 0100  ..e.d=d.d>d.....
-000001f0: 6503 643f 6440 6441 8d02 0100 6503 6442  e.d?d@dA....e.dB
-00000200: 6443 6441 8d02 0100 6503 6444 6445 6441  dCdA....e.dDdEdA
-00000210: 8d02 0100 6503 6446 6447 6441 8d02 0100  ....e.dFdGdA....
-00000220: 6503 6448 6449 6441 8d02 0100 6503 644a  e.dHdIdA....e.dJ
-00000230: 644b 6441 8d02 0100 6503 644c 6401 644d  dKdA....e.dLd.dM
-00000240: 640c 8d03 0100 6503 644e 6401 6517 644f  d.....e.dNd.e.dO
-00000250: 8d03 0100 6503 6450 6401 6517 644f 8d03  ....e.dPd.e.dO..
-00000260: 0100 6503 6451 6401 6517 644f 8d03 0100  ..e.dQd.e.dO....
-00000270: 6503 6452 6401 6517 644f 8d03 0100 6503  e.dRd.e.dO....e.
-00000280: 6453 6401 6515 644f 8d03 0100 6503 6454  dSd.e.dO....e.dT
-00000290: 6401 6517 644f 8d03 0100 6503 6455 6401  d.e.dO....e.dUd.
-000002a0: 6517 644f 8d03 0100 6503 6456 6457 6517  e.dO....e.dVdWe.
-000002b0: 644f 8d03 0100 6503 6458 6423 6516 644f  dO....e.dXd#e.dO
-000002c0: 8d03 0100 6503 6459 6401 6517 644f 8d03  ....e.dYd.e.dO..
-000002d0: 0100 6503 645a 641a 6516 644f 8d03 0100  ..e.dZd.e.dO....
-000002e0: 6503 645b 645c 6517 644f 8d03 0100 6503  e.d[d\e.dO....e.
-000002f0: 645d 645e 6517 644f 8d03 0100 6503 645f  d]d^e.dO....e.d_
-00000300: 6460 6461 8d02 0100 6503 6462 6417 6461  d`da....e.dbd.da
-00000310: 8d02 0100 6503 6463 6417 6461 8d02 0100  ....e.dcd.da....
-00000320: 6503 6464 6417 6461 8d02 0100 6503 6465  e.ddd.da....e.de
-00000330: 6417 6461 8d02 0100 6503 6466 6417 6461  d.da....e.dfd.da
-00000340: 8d02 0100 6503 6467 6417 6461 8d02 0100  ....e.dgd.da....
-00000350: 6504 6a19 641a 6468 8d01 0100 6504 6a1a  e.j.d.dh....e.j.
-00000360: 9003 7290 7916 650b 6504 6504 6a1a 6469  ..r.y.e.e.e.j.di
-00000370: 641a 6468 8d04 0100 5700 6e3a 0400 651b  d.dh....W.n:..e.
-00000380: 6b0a 9003 728e 0100 5a1c 0100 7a1c 6504  k...r...Z...z.e.
-00000390: 6a1a 6512 6b03 9003 727e 6506 6a1d 651c  j.e.k...r~e.j.e.
-000003a0: 8301 0100 5700 5900 6401 6401 5a1c 5b1c  ....W.Y.d.d.Z.[.
-000003b0: 5800 6e02 5800 650a 6504 6423 6468 8d02  X.n.X.e.e.d#dh..
-000003c0: 0100 6409 640d 6425 6427 643f 6705 5a1e  ..d.d.d%d'd?g.Z.
-000003d0: 643f 6701 5a1f 6504 6a20 646a 6b03 9003  d?g.Z.e.j djk...
-000003e0: 72d0 651e 6a21 644a 8301 0100 651f 6a21  r.e.j!dJ....e.j!
-000003f0: 644a 8301 0100 6522 6523 646b 646c 8400  dJ....e"e#dkdl..
-00000400: 651e 8302 8301 5a24 6504 6a25 5a26 6504  e.....Z$e.j%Z&e.
-00000410: 6a27 5a28 6504 6a29 5a2a 6504 6a2b 5a2c  j'Z(e.j)Z*e.j+Z,
-00000420: 6504 6a2d 5a2e 6504 6a2f 5a30 6504 6a31  e.j-Z.e.j/Z0e.j1
-00000430: 5a32 6504 6a33 5a34 6504 6a1a 5a35 6504  Z2e.j3Z4e.j.Z5e.
-00000440: 6a36 6a37 8300 6a38 646d 8301 5a39 6504  j6j7..j8dm..Z9e.
-00000450: 6a3a 5a3b 6504 6a3c 5a3d 6504 6a3e 5a3f  j:Z;e.j<Z=e.j>Z?
-00000460: 6504 6a40 5a41 6504 6a42 5a43 6504 6a44  e.j@ZAe.jBZCe.jD
-00000470: 5a45 6504 6a46 5a47 6504 6a48 5a49 6504  ZEe.jFZGe.jHZIe.
-00000480: 6a4a 5a4b 6504 6a4c 5a4d 6504 6a4e 5a4f  jJZKe.jLZMe.jNZO
-00000490: 6504 6a50 5a51 6504 6a52 5a53 6504 6a20  e.jPZQe.jRZSe.j 
-000004a0: 5a54 6504 6a55 5a56 6504 6a57 5a58 6504  ZTe.jUZVe.jWZXe.
-000004b0: 6a59 5a5a 6504 6a5b 5a5c 6504 6a5d 5a5e  jYZZe.j[Z\e.j]Z^
-000004c0: 6504 6a5f 5a60 6504 6a61 9004 72b4 6504  e.j_Z`e.ja..r.e.
-000004d0: 6a61 6a38 646d 8301 6e02 6401 5a62 6504  jaj8dm..n.d.Zbe.
-000004e0: 6a63 9004 72cc 6504 6a63 6a38 646d 8301  jc..r.e.jcj8dm..
-000004f0: 6e02 6401 5a64 6504 6a65 5a66 6504 6a67  n.d.Zde.jeZfe.jg
-00000500: 5a68 6504 6a69 5a6a 6504 6a6b 5a6c 6504  Zhe.jiZje.jkZle.
-00000510: 6a6d 5a6e 6504 6a6f 5a70 6504 6a71 5a72  jmZne.joZpe.jqZr
-00000520: 6504 6a73 5a74 6504 6a75 5a76 6504 6a77  e.jsZte.juZve.jw
-00000530: 5a78 7910 6500 6a79 6504 6a7a 8301 5a7b  Zxy.e.jye.jz..Z{
-00000540: 5700 6e36 0400 657c 6b0a 9005 7252 0100  W.n6..e|k...rR..
-00000550: 5a1c 0100 7a18 6506 6a7d 646e 651c 646f  Z...z.e.j}dne.do
-00000560: 8d02 0100 6900 5a7b 5700 5900 6401 6401  ....i.Z{W.Y.d.d.
-00000570: 5a1c 5b1c 5800 6e02 5800 6504 6a7e 5a7f  Z.[.X.n.X.e.j~Z.
-00000580: 6504 6a80 5a81 6504 6a82 5a83 6504 6a84  e.j.Z.e.j.Z.e.j.
-00000590: 5a85 6504 6a86 5a87 6504 6a88 5a89 6504  Z.e.j.Z.e.j.Z.e.
-000005a0: 6a8a 5a8b 6501 6a8c 6a8d 6470 8301 5a8e  j.Z.e.j.j.dp..Z.
-000005b0: 6401 5300 2971 e900 0000 004e 2902 da06  d.S.)q.....N)...
-000005c0: 6465 6669 6e65 da07 6f70 7469 6f6e 7329  define..options)
-000005d0: 01da 066c 6f67 6765 7229 01da 056d 6564  ...logger)...med
-000005e0: 6961 2902 da11 7061 7273 655f 656e 7669  ia)...parse_envi
-000005f0: 726f 6e6d 656e 74da 1170 6172 7365 5f63  ronment..parse_c
-00000600: 6f6e 6669 675f 6669 6c65 7a08 6a65 742e  onfig_filez.jet.
-00000610: 636f 6e66 7a17 6874 7470 733a 2f2f 6170  confz.https://ap
-00000620: 702e 6a65 7461 646d 696e 2e69 6f7a 1b68  p.jetadmin.ioz.h
-00000630: 7474 7073 3a2f 2f61 7069 2e6a 6574 6164  ttps://api.jetad
-00000640: 6d69 6e2e 696f 2f61 7069 da07 6164 6472  min.io/api..addr
-00000650: 6573 737a 0730 2e30 2e30 2e30 7a0e 7365  essz.0.0.0.0z.se
-00000660: 7276 6572 2061 6464 7265 7373 2902 da07  rver address)...
-00000670: 6465 6661 756c 74da 0468 656c 70da 0470  default..help..p
-00000680: 6f72 7469 b822 0000 7a0b 7365 7276 6572  orti."..z.server
-00000690: 2070 6f72 7429 0372 0900 0000 720a 0000   port).r....r...
-000006a0: 00da 0474 7970 65da 0777 6f72 6b65 7273  ...type..workers
-000006b0: e901 0000 007a 116e 756d 6265 7220 6f66  .....z.number of
-000006c0: 2077 6f72 6b65 7273 da06 636f 6e66 6967   workers..config
-000006d0: 7a10 636f 6e66 6967 2066 696c 6520 7061  z.config file pa
-000006e0: 7468 da12 7573 655f 6465 6661 756c 745f  th..use_default_
-000006f0: 636f 6e66 6967 da00 7a19 7573 6520 6465  config..z.use de
-00000700: 6661 756c 7420 636f 6e66 6967 2076 616c  fault config val
-00000710: 7565 73da 0564 6562 7567 467a 0a64 6562  ues..debugFz.deb
-00000720: 7567 206d 6f64 65da 0972 6561 645f 6f6e  ug mode..read_on
-00000730: 6c79 7a09 7265 6164 206f 6e6c 79da 0774  lyz.read only..t
-00000740: 6872 6561 6473 da0b 636f 6e6e 6563 7469  hreads..connecti
-00000750: 6f6e 73e9 3200 0000 5a08 636f 6e6e 6563  ons.2...Z.connec
-00000760: 7473 da12 6175 746f 5f6f 7065 6e5f 7265  ts..auto_open_re
-00000770: 6769 7374 6572 547a 216f 7065 6e20 746f  gisterTz!open to
-00000780: 6b65 6e20 7265 6769 7374 6572 2061 7574  ken register aut
-00000790: 6f6d 6174 6963 616c 6c79 da07 7072 6f6a  omatically..proj
-000007a0: 6563 7429 0272 0a00 0000 720c 0000 00da  ect).r....r.....
-000007b0: 0574 6f6b 656e da0b 656e 7669 726f 6e6d  .token..environm
-000007c0: 656e 74da 0c63 6f72 735f 6865 6164 6572  ent..cors_header
-000007d0: 737a 1061 6464 2043 4f52 5320 6865 6164  sz.add CORS head
-000007e0: 6572 73da 0862 6173 655f 7572 6c7a 0862  ers..base_urlz.b
-000007f0: 6173 6520 5552 4cda 0e6a 7774 5f76 6572  ase URL..jwt_ver
-00000800: 6966 795f 6b65 797a 0e4a 5754 2076 6572  ify_keyz.JWT ver
-00000810: 6966 7920 6b65 7929 0372 0a00 0000 720c  ify key).r....r.
-00000820: 0000 0072 0900 0000 da0f 6265 6172 6572  ...r......bearer
-00000830: 5f61 7574 685f 6b65 797a 0f42 6561 7265  _auth_keyz.Beare
-00000840: 7220 6175 7468 206b 6579 da10 656e 7669  r auth key..envi
-00000850: 726f 6e6d 656e 745f 7479 7065 7a10 656e  ronment_typez.en
-00000860: 7669 726f 6e6d 656e 7420 7479 7065 da0c  vironment type..
-00000870: 7765 625f 6261 7365 5f75 726c 7a27 4a65  web_base_urlz'Je
-00000880: 7420 4164 6d69 6e20 6672 6f6e 7465 6e64  t Admin frontend
-00000890: 2061 7070 6c69 6361 7469 6f6e 2062 6173   application bas
-000008a0: 6520 5552 4cda 0c61 7069 5f62 6173 655f  e URL..api_base_
-000008b0: 7572 6c7a 164a 6574 2041 646d 696e 2041  urlz.Jet Admin A
-000008c0: 5049 2062 6173 6520 5552 4cda 0d6d 6564  PI base URL..med
-000008d0: 6961 5f73 746f 7261 6765 7a12 6d65 6469  ia_storagez.medi
-000008e0: 6120 7374 6f72 6167 6520 7479 7065 da0a  a storage type..
-000008f0: 6d65 6469 615f 726f 6f74 7205 0000 007a  media_rootr....z
-00000900: 0a6d 6564 6961 2072 6f6f 74da 0e6d 6564  .media root..med
-00000910: 6961 5f62 6173 655f 7572 6c7a 0e6d 6564  ia_base_urlz.med
-00000920: 6961 2062 6173 6520 5552 4cda 0f64 6174  ia base URL..dat
-00000930: 6162 6173 655f 656e 6769 6e65 7a56 6461  abase_enginezVda
-00000940: 7461 6261 7365 2065 6e67 696e 6520 2870  tabase engine (p
-00000950: 6f73 7467 7265 7371 6c2c 206d 7973 716c  ostgresql, mysql
-00000960: 2c20 6f72 6163 6c65 2c20 6d73 7371 6c2b  , oracle, mssql+
-00000970: 7079 6f64 6263 2c20 6269 6771 7565 7279  pyodbc, bigquery
-00000980: 2c20 736e 6f77 666c 616b 652c 2073 716c  , snowflake, sql
-00000990: 6974 6529 2901 720a 0000 00da 0d64 6174  ite)).r......dat
-000009a0: 6162 6173 655f 686f 7374 7a0d 6461 7461  abase_hostz.data
-000009b0: 6261 7365 2068 6f73 74da 0d64 6174 6162  base host..datab
-000009c0: 6173 655f 706f 7274 7a0d 6461 7461 6261  ase_portz.databa
-000009d0: 7365 2070 6f72 74da 0d64 6174 6162 6173  se port..databas
-000009e0: 655f 7573 6572 7a0d 6461 7461 6261 7365  e_userz.database
-000009f0: 2075 7365 72da 1164 6174 6162 6173 655f   user..database_
-00000a00: 7061 7373 776f 7264 7a11 6461 7461 6261  passwordz.databa
-00000a10: 7365 2070 6173 7377 6f72 64da 0d64 6174  se password..dat
-00000a20: 6162 6173 655f 6e61 6d65 7a15 6461 7461  abase_namez.data
-00000a30: 6261 7365 206e 616d 6520 6f72 2070 6174  base name or pat
-00000a40: 68da 0e64 6174 6162 6173 655f 6578 7472  h..database_extr
-00000a50: 617a 1964 6174 6162 6173 6520 6578 7472  az.database extr
-00000a60: 6120 7061 7261 6d65 7465 7273 da0d 6461  a parameters..da
-00000a70: 7461 6261 7365 5f6f 6e6c 7929 0272 0900  tabase_only).r..
-00000a80: 0000 720c 0000 00da 0f64 6174 6162 6173  ..r......databas
-00000a90: 655f 6578 6365 7074 da0f 6461 7461 6261  e_except..databa
-00000aa0: 7365 5f73 6368 656d 61da 1164 6174 6162  se_schema..datab
-00000ab0: 6173 655f 7373 685f 686f 7374 da11 6461  ase_ssh_host..da
-00000ac0: 7461 6261 7365 5f73 7368 5f70 6f72 74da  tabase_ssh_port.
-00000ad0: 1164 6174 6162 6173 655f 7373 685f 7573  .database_ssh_us
-00000ae0: 6572 da18 6461 7461 6261 7365 5f73 7368  er..database_ssh
-00000af0: 5f70 7269 7661 7465 5f6b 6579 da0f 636f  _private_key..co
-00000b00: 6f6b 6965 5f73 616d 6573 6974 65da 044e  okie_samesite..N
-00000b10: 6f6e 65da 0d63 6f6f 6b69 655f 7365 6375  one..cookie_secu
-00000b20: 7265 da0d 636f 6f6b 6965 5f64 6f6d 6169  re..cookie_domai
-00000b30: 6eda 0f63 6f6f 6b69 655f 636f 6d70 7265  n..cookie_compre
-00000b40: 7373 da0a 7374 6f72 655f 7061 7468 7a18  ss..store_pathz.
-00000b50: 6a65 745f 6272 6964 6765 5f73 746f 7265  jet_bridge_store
-00000b60: 2e73 716c 6974 6533 da10 7373 6f5f 6170  .sqlite3..sso_ap
-00000b70: 706c 6963 6174 696f 6e73 7a02 7b7d da0c  plicationsz.{}..
-00000b80: 616c 6c6f 775f 6f72 6967 696e da01 2a29  allow_origin..*)
-00000b90: 0172 0900 0000 da0f 7472 6163 6b5f 6461  .r......track_da
-00000ba0: 7461 6261 7365 73da 1874 7261 636b 5f64  tabases..track_d
-00000bb0: 6174 6162 6173 6573 5f65 6e64 706f 696e  atabases_endpoin
-00000bc0: 74da 1474 7261 636b 5f64 6174 6162 6173  t..track_databas
-00000bd0: 6573 5f61 7574 68da 1574 7261 636b 5f6d  es_auth..track_m
-00000be0: 6f64 656c 735f 656e 6470 6f69 6e74 da11  odels_endpoint..
-00000bf0: 7472 6163 6b5f 6d6f 6465 6c73 5f61 7574  track_models_aut
-00000c00: 68da 0a73 656e 7472 795f 6473 6e29 01da  h..sentry_dsn)..
-00000c10: 0566 696e 616c 5a03 4a45 54da 046e 6f6e  .finalZ.JET..non
-00000c20: 6563 0100 0000 0000 0000 0100 0000 0200  ec..............
-00000c30: 0000 4300 0000 7314 0000 007c 0074 006b  ..C...s....|.t.k
-00000c40: 0770 1274 007c 0019 0064 006b 0853 0029  .p.t.|...d.k.S.)
-00000c50: 014e 2901 7203 0000 0029 01da 0178 a900  .N).r....)...x..
-00000c60: 7245 0000 00fa 552f 5573 6572 732f 6631  rE....U/Users/f1
-00000c70: 6e61 6c2f 4472 6f70 626f 782f 7079 7468  nal/Dropbox/pyth
-00000c80: 6f6e 2f6a 6574 2d62 7269 6467 652f 7372  on/jet-bridge/sr
-00000c90: 632f 7061 636b 6167 6573 2f6a 6574 5f62  c/packages/jet_b
-00000ca0: 7269 6467 652f 6a65 745f 6272 6964 6765  ridge/jet_bridge
-00000cb0: 2f73 6574 7469 6e67 732e 7079 da08 3c6c  /settings.py..<l
-00000cc0: 616d 6264 613e 7100 0000 7300 0000 0072  ambda>q...s....r
-00000cd0: 4700 0000 fa01 2c7a 1f53 534f 5f41 5050  G.....,z.SSO_APP
-00000ce0: 4c49 4341 5449 4f4e 5320 7061 7273 696e  LICATIONS parsin
-00000cf0: 6720 6661 696c 6564 2901 da08 6578 635f  g failed)...exc_
-00000d00: 696e 666f da0d 504f 5353 4942 4c45 5f48  info..POSSIBLE_H
-00000d10: 4f53 5429 8fda 046a 736f 6eda 026f 73da  OST)...json..os.
-00000d20: 0f74 6f72 6e61 646f 2e6f 7074 696f 6e73  .tornado.options
-00000d30: 7202 0000 0072 0300 0000 da16 6a65 745f  r....r......jet_
-00000d40: 6272 6964 6765 5f62 6173 652e 6c6f 6767  bridge_base.logg
-00000d50: 6572 7204 0000 00da 0a6a 6574 5f62 7269  err......jet_bri
-00000d60: 6467 6572 0500 0000 5a19 6a65 745f 6272  dger....Z.jet_br
-00000d70: 6964 6765 2e75 7469 6c73 2e73 6574 7469  idge.utils.setti
-00000d80: 6e67 7372 0600 0000 7207 0000 00da 0470  ngsr....r......p
-00000d90: 6174 68da 0764 6972 6e61 6d65 da07 6162  ath..dirname..ab
-00000da0: 7370 6174 68da 085f 5f66 696c 655f 5fda  spath..__file__.
-00000db0: 0842 4153 455f 4449 52da 046a 6f69 6e5a  .BASE_DIR..joinZ
-00000dc0: 1344 4546 4155 4c54 5f43 4f4e 4649 475f  .DEFAULT_CONFIG_
-00000dd0: 5041 5448 5a14 4445 4641 554c 545f 5745  PATHZ.DEFAULT_WE
-00000de0: 425f 4241 5345 5f55 524c 5a14 4445 4641  B_BASE_URLZ.DEFA
-00000df0: 554c 545f 4150 495f 4241 5345 5f55 524c  ULT_API_BASE_URL
-00000e00: da03 696e 74da 0462 6f6f 6cda 0373 7472  ..int..bool..str
-00000e10: 5a12 4d45 4449 415f 5354 4f52 4147 455f  Z.MEDIA_STORAGE_
-00000e20: 4649 4c45 5a12 7061 7273 655f 636f 6d6d  FILEZ.parse_comm
-00000e30: 616e 645f 6c69 6e65 720f 0000 00da 0749  and_liner......I
-00000e40: 4f45 7272 6f72 da01 65da 0777 6172 6e69  OError..e..warni
-00000e50: 6e67 5a10 7265 7175 6972 6564 5f6f 7074  ngZ.required_opt
-00000e60: 696f 6e73 da20 7265 7175 6972 6564 5f6f  ions. required_o
-00000e70: 7074 696f 6e73 5f77 6974 686f 7574 5f64  ptions_without_d
-00000e80: 6566 6175 6c74 7225 0000 00da 0661 7070  efaultr%.....app
-00000e90: 656e 64da 046c 6973 74da 0666 696c 7465  end..list..filte
-00000ea0: 72da 0f6d 6973 7369 6e67 5f6f 7074 696f  r..missing_optio
-00000eb0: 6e73 7208 0000 00da 0741 4444 5245 5353  nsr......ADDRESS
-00000ec0: 720b 0000 00da 0450 4f52 5472 0d00 0000  r......PORTr....
-00000ed0: da07 574f 524b 4552 5372 1200 0000 da05  ..WORKERSr......
-00000ee0: 4445 4255 4772 1300 0000 da09 5245 4144  DEBUGr......READ
-00000ef0: 5f4f 4e4c 5972 1400 0000 5a07 5448 5245  _ONLYr....Z.THRE
-00000f00: 4144 5372 1500 0000 da0b 434f 4e4e 4543  ADSr......CONNEC
-00000f10: 5449 4f4e 5372 1700 0000 da12 4155 544f  TIONSr......AUTO
-00000f20: 5f4f 5045 4e5f 5245 4749 5354 4552 5a06  _OPEN_REGISTERZ.
-00000f30: 434f 4e46 4947 7210 0000 00da 056c 6f77  CONFIGr......low
-00000f40: 6572 da05 7370 6c69 745a 1255 5345 5f44  er..splitZ.USE_D
-00000f50: 4546 4155 4c54 5f43 4f4e 4649 4772 1800  EFAULT_CONFIGr..
-00000f60: 0000 da07 5052 4f4a 4543 5472 1900 0000  ....PROJECTr....
-00000f70: da05 544f 4b45 4e72 1a00 0000 da0b 454e  ..TOKENr......EN
-00000f80: 5649 524f 4e4d 454e 5472 1b00 0000 da0c  VIRONMENTr......
-00000f90: 434f 5253 5f48 4541 4445 5253 721c 0000  CORS_HEADERSr...
-00000fa0: 00da 0842 4153 455f 5552 4c72 1d00 0000  ...BASE_URLr....
-00000fb0: da0e 4a57 545f 5645 5249 4659 5f4b 4559  ..JWT_VERIFY_KEY
-00000fc0: 721e 0000 00da 0f42 4541 5245 525f 4155  r......BEARER_AU
-00000fd0: 5448 5f4b 4559 721f 0000 00da 1045 4e56  TH_KEYr......ENV
-00000fe0: 4952 4f4e 4d45 4e54 5f54 5950 4572 2000  IRONMENT_TYPEr .
-00000ff0: 0000 da0c 5745 425f 4241 5345 5f55 524c  ....WEB_BASE_URL
-00001000: 7221 0000 00da 0c41 5049 5f42 4153 455f  r!.....API_BASE_
-00001010: 5552 4c72 2200 0000 5a0d 4d45 4449 415f  URLr"...Z.MEDIA_
-00001020: 5354 4f52 4147 4572 2300 0000 da0a 4d45  STORAGEr#.....ME
-00001030: 4449 415f 524f 4f54 7224 0000 00da 0e4d  DIA_ROOTr$.....M
-00001040: 4544 4941 5f42 4153 455f 5552 4cda 0f44  EDIA_BASE_URL..D
-00001050: 4154 4142 4153 455f 454e 4749 4e45 7226  ATABASE_ENGINEr&
-00001060: 0000 00da 0d44 4154 4142 4153 455f 484f  .....DATABASE_HO
-00001070: 5354 7227 0000 00da 0d44 4154 4142 4153  STr'.....DATABAS
-00001080: 455f 504f 5254 7228 0000 00da 0d44 4154  E_PORTr(.....DAT
-00001090: 4142 4153 455f 5553 4552 7229 0000 00da  ABASE_USERr)....
-000010a0: 1144 4154 4142 4153 455f 5041 5353 574f  .DATABASE_PASSWO
-000010b0: 5244 722a 0000 00da 0d44 4154 4142 4153  RDr*.....DATABAS
-000010c0: 455f 4e41 4d45 722b 0000 00da 0e44 4154  E_NAMEr+.....DAT
-000010d0: 4142 4153 455f 4558 5452 4172 2c00 0000  ABASE_EXTRAr,...
-000010e0: da0d 4441 5441 4241 5345 5f4f 4e4c 5972  ..DATABASE_ONLYr
-000010f0: 2d00 0000 da0f 4441 5441 4241 5345 5f45  -.....DATABASE_E
-00001100: 5843 4550 5472 2e00 0000 da0f 4441 5441  XCEPTr......DATA
-00001110: 4241 5345 5f53 4348 454d 4172 2f00 0000  BASE_SCHEMAr/...
-00001120: da11 4441 5441 4241 5345 5f53 5348 5f48  ..DATABASE_SSH_H
-00001130: 4f53 5472 3000 0000 da11 4441 5441 4241  OSTr0.....DATABA
-00001140: 5345 5f53 5348 5f50 4f52 5472 3100 0000  SE_SSH_PORTr1...
-00001150: da11 4441 5441 4241 5345 5f53 5348 5f55  ..DATABASE_SSH_U
-00001160: 5345 5272 3200 0000 da18 4441 5441 4241  SERr2.....DATABA
-00001170: 5345 5f53 5348 5f50 5249 5641 5445 5f4b  SE_SSH_PRIVATE_K
-00001180: 4559 7233 0000 00da 0f43 4f4f 4b49 455f  EYr3.....COOKIE_
-00001190: 5341 4d45 5349 5445 7235 0000 00da 0d43  SAMESITEr5.....C
-000011a0: 4f4f 4b49 455f 5345 4355 5245 7236 0000  OOKIE_SECUREr6..
-000011b0: 00da 0d43 4f4f 4b49 455f 444f 4d41 494e  ...COOKIE_DOMAIN
-000011c0: 7237 0000 00da 0f43 4f4f 4b49 455f 434f  r7.....COOKIE_CO
-000011d0: 4d50 5245 5353 7238 0000 00da 0a53 544f  MPRESSr8.....STO
-000011e0: 5245 5f50 4154 48da 056c 6f61 6473 7239  RE_PATH..loadsr9
-000011f0: 0000 00da 1053 534f 5f41 5050 4c49 4341  .....SSO_APPLICA
-00001200: 5449 4f4e 53da 0945 7863 6570 7469 6f6e  TIONS..Exception
-00001210: da05 6572 726f 7272 3a00 0000 da0c 414c  ..errorr:.....AL
-00001220: 4c4f 575f 4f52 4947 494e 723c 0000 00da  LOW_ORIGINr<....
-00001230: 0f54 5241 434b 5f44 4154 4142 4153 4553  .TRACK_DATABASES
-00001240: 723d 0000 00da 1854 5241 434b 5f44 4154  r=.....TRACK_DAT
-00001250: 4142 4153 4553 5f45 4e44 504f 494e 5472  ABASES_ENDPOINTr
-00001260: 3e00 0000 da14 5452 4143 4b5f 4441 5441  >.....TRACK_DATA
-00001270: 4241 5345 535f 4155 5448 723f 0000 00da  BASES_AUTHr?....
-00001280: 1554 5241 434b 5f4d 4f44 454c 535f 454e  .TRACK_MODELS_EN
-00001290: 4450 4f49 4e54 7240 0000 00da 1154 5241  DPOINTr@.....TRA
-000012a0: 434b 5f4d 4f44 454c 535f 4155 5448 7241  CK_MODELS_AUTHrA
-000012b0: 0000 005a 0a53 454e 5452 595f 4453 4eda  ...Z.SENTRY_DSN.
-000012c0: 0765 6e76 6972 6f6e da03 6765 7472 4a00  .environ..getrJ.
-000012d0: 0000 7245 0000 0072 4500 0000 7245 0000  ..rE...rE...rE..
-000012e0: 0072 4600 0000 da08 3c6d 6f64 756c 653e  .rF.....<module>
-000012f0: 0100 0000 7308 0100 0008 0108 0210 020c  ....s...........
-00001300: 020c 0110 0414 010c 0404 0104 020e 0110  ................
-00001310: 0110 010e 010e 0110 0110 0110 0110 0110  ................
-00001320: 010e 010e 010e 0110 010e 0110 0110 0110  ................
-00001330: 020e 010e 0210 010e 010e 020c 010c 010c  ................
-00001340: 010c 010c 010c 010e 010e 010e 010e 020e  ................
-00001350: 010e 010e 010e 020e 010e 010e 010e 020e  ................
-00001360: 020e 010c 020c 010c 010c 020c 010c 020c  ................
-00001370: 040c 0208 0102 0116 0112 010c 011c 020c  ................
-00001380: 0302 0102 0102 0102 0106 0606 030c 010a  ................
-00001390: 010a 0212 0406 0106 0106 0106 0106 0106  ................
-000013a0: 0106 0106 0106 0110 0106 0106 0106 0106  ................
-000013b0: 0106 0106 0106 0106 0206 0106 0206 0106  ................
-000013c0: 0106 0206 0106 0106 0106 0106 0106 0106  ................
-000013d0: 0118 0118 0106 0206 0106 0106 0106 0206  ................
-000013e0: 0106 0106 0106 0206 0202 0110 0112 010e  ................
-000013f0: 0116 0206 0206 0106 0106 0206 0106 0206  ................
-00001400: 02                                       .
+00000000: 420d 0d0a 0000 0000 9e18 3964 9c19 0000  B.........9d....
+00000010: e300 0000 0000 0000 0000 0000 000a 0000  ................
+00000020: 0040 0000 0073 b605 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 5a00 6400 6401 6c01 5a01 6400 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
+00000070: 0100 6501 6a0c a00d 6501 6a0c a00e 650f  ..e.j...e.j...e.
+00000080: a101 a101 5a10 6501 6a0c a011 6406 a101  ....Z.e.j...d...
+00000090: 5a12 6407 5a13 6408 5a14 6503 6409 640a  Z.d.Z.d.Z.e.d.d.
+000000a0: 640b 640c 8d03 0100 6503 640d 640e 640f  d.d.....e.d.d.d.
+000000b0: 6515 6410 8d04 0100 6503 6411 6412 6413  e.d.....e.d.d.d.
+000000c0: 6515 6410 8d04 0100 6503 6414 6512 6415  e.d.....e.d.e.d.
+000000d0: 640c 8d03 0100 6503 6416 6417 6418 640c  d.....e.d.d.d.d.
+000000e0: 8d03 0100 6503 6419 641a 641b 6516 6410  ....e.d.d.d.e.d.
+000000f0: 8d04 0100 6503 641c 641a 641d 6516 6410  ....e.d.d.d.e.d.
+00000100: 8d04 0100 6503 641e 6401 641e 6515 6410  ....e.d.d.d.e.d.
+00000110: 8d04 0100 6503 641f 6420 6421 6515 6410  ....e.d.d d!e.d.
+00000120: 8d04 0100 6503 6422 6423 6424 6516 6410  ....e.d"d#d$e.d.
+00000130: 8d04 0100 6503 6425 6425 6517 6426 8d03  ....e.d%d%e.d&..
+00000140: 0100 6503 6427 6427 6517 6426 8d03 0100  ..e.d'd'e.d&....
+00000150: 6503 6428 6428 6517 6426 8d03 0100 6503  e.d(d(e.d&....e.
+00000160: 6429 6423 642a 6516 6410 8d04 0100 6503  d)d#d*e.d.....e.
+00000170: 642b 642c 6517 6426 8d03 0100 6503 642d  d+d,e.d&....e.d-
+00000180: 642e 6517 6401 642f 8d04 0100 6503 6430  d.e.d.d/....e.d0
+00000190: 6431 6517 6401 642f 8d04 0100 6503 6432  d1e.d.d/....e.d2
+000001a0: 6433 6517 6401 642f 8d04 0100 6503 6434  d3e.d.d/....e.d4
+000001b0: 6513 6435 640c 8d03 0100 6503 6436 6514  e.d5d.....e.d6e.
+000001c0: 6437 640c 8d03 0100 6503 6438 6508 6a18  d7d.....e.d8e.j.
+000001d0: 6439 640c 8d03 0100 6503 643a 643b 643c  d9d.....e.d:d;d<
+000001e0: 640c 8d03 0100 6503 643d 6401 643e 640c  d.....e.d=d.d>d.
+000001f0: 8d03 0100 6503 643f 6440 6441 8d02 0100  ....e.d?d@dA....
+00000200: 6503 6442 6443 6441 8d02 0100 6503 6444  e.dBdCdA....e.dD
+00000210: 6445 6441 8d02 0100 6503 6446 6447 6441  dEdA....e.dFdGdA
+00000220: 8d02 0100 6503 6448 6449 6441 8d02 0100  ....e.dHdIdA....
+00000230: 6503 644a 644b 6441 8d02 0100 6503 644c  e.dJdKdA....e.dL
+00000240: 6401 644d 640c 8d03 0100 6503 644e 6401  d.dMd.....e.dNd.
+00000250: 6517 644f 8d03 0100 6503 6450 6401 6517  e.dO....e.dPd.e.
+00000260: 644f 8d03 0100 6503 6451 6401 6515 644f  dO....e.dQd.e.dO
+00000270: 8d03 0100 6503 6452 6401 6517 644f 8d03  ....e.dRd.e.dO..
+00000280: 0100 6503 6453 6401 6517 644f 8d03 0100  ..e.dSd.e.dO....
+00000290: 6503 6454 6401 6515 644f 8d03 0100 6503  e.dTd.e.dO....e.
+000002a0: 6455 6401 6517 644f 8d03 0100 6503 6456  dUd.e.dO....e.dV
+000002b0: 6401 6517 644f 8d03 0100 6503 6457 6458  d.e.dO....e.dWdX
+000002c0: 6517 644f 8d03 0100 6503 6459 6423 6516  e.dO....e.dYd#e.
+000002d0: 644f 8d03 0100 6503 645a 6401 6517 644f  dO....e.dZd.e.dO
+000002e0: 8d03 0100 6503 645b 641a 6516 644f 8d03  ....e.d[d.e.dO..
+000002f0: 0100 6503 645c 645d 6517 644f 8d03 0100  ..e.d\d]e.dO....
+00000300: 6503 645e 645f 6517 644f 8d03 0100 6503  e.d^d_e.dO....e.
+00000310: 6460 6461 6462 8d02 0100 6503 6463 6417  d`dadb....e.dcd.
+00000320: 6462 8d02 0100 6503 6464 6417 6462 8d02  db....e.ddd.db..
+00000330: 0100 6503 6465 6417 6462 8d02 0100 6503  ..e.ded.db....e.
+00000340: 6466 6417 6462 8d02 0100 6503 6467 6417  dfd.db....e.dgd.
+00000350: 6462 8d02 0100 6503 6468 641a 6516 644f  db....e.dhd.e.dO
+00000360: 8d03 0100 6503 6469 6417 6462 8d02 0100  ....e.did.db....
+00000370: 6504 6a19 641a 646a 8d01 0100 6504 6a1a  e.j.d.dj....e.j.
+00000380: 9003 72ac 7916 650b 6504 6504 6a1a 646b  ..r.y.e.e.e.j.dk
+00000390: 641a 646a 8d04 0100 5700 6e3a 0400 651b  d.dj....W.n:..e.
+000003a0: 6b0a 9003 72aa 0100 5a1c 0100 7a1a 6504  k...r...Z...z.e.
+000003b0: 6a1a 6512 6b03 9003 729a 6506 a01d 651c  j.e.k...r.e...e.
+000003c0: a101 0100 5700 6401 6401 5a1c 5b1c 5800  ....W.d.d.Z.[.X.
+000003d0: 5900 6e02 5800 650a 6504 6423 646a 8d02  Y.n.X.e.e.d#dj..
+000003e0: 0100 6409 640d 6425 6427 643f 6705 5a1e  ..d.d.d%d'd?g.Z.
+000003f0: 643f 6701 5a1f 6504 6a20 646c 6b03 9003  d?g.Z.e.j dlk...
+00000400: 72ec 651e a021 644a a101 0100 651f a021  r.e..!dJ....e..!
+00000410: 644a a101 0100 6522 6523 646d 646e 8400  dJ....e"e#dmdn..
+00000420: 651e 8302 8301 5a24 6504 6a25 5a26 6504  e.....Z$e.j%Z&e.
+00000430: 6a27 5a28 6504 6a29 5a2a 6504 6a2b 5a2c  j'Z(e.j)Z*e.j+Z,
+00000440: 6504 6a2d 5a2e 6504 6a2f 5a30 6504 6a31  e.j-Z.e.j/Z0e.j1
+00000450: 5a32 6504 6a33 5a34 6504 6a1a 5a35 6504  Z2e.j3Z4e.j.Z5e.
+00000460: 6a36 a037 a100 a038 646f a101 5a39 6504  j6.7...8do..Z9e.
+00000470: 6a3a 5a3b 6504 6a3c 5a3d 6504 6a3e 5a3f  j:Z;e.j<Z=e.j>Z?
+00000480: 6504 6a40 5a41 6504 6a42 5a43 6504 6a44  e.j@ZAe.jBZCe.jD
+00000490: 5a45 6504 6a46 5a47 6504 6a48 5a49 6504  ZEe.jFZGe.jHZIe.
+000004a0: 6a4a 5a4b 6504 6a4c 5a4d 6504 6a4e 5a4f  jJZKe.jLZMe.jNZO
+000004b0: 6504 6a50 5a51 6504 6a52 5a53 6504 6a20  e.jPZQe.jRZSe.j 
+000004c0: 5a54 6504 6a55 5a56 6504 6a57 5a58 6504  ZTe.jUZVe.jWZXe.
+000004d0: 6a59 5a5a 6504 6a5b 5a5c 6504 6a5d 5a5e  jYZZe.j[Z\e.j]Z^
+000004e0: 6504 6a5f 5a60 6504 6a61 9004 72d0 6504  e.j_Z`e.ja..r.e.
+000004f0: 6a61 a038 646f a101 6e02 6401 5a62 6504  ja.8do..n.d.Zbe.
+00000500: 6a63 9004 72e8 6504 6a63 a038 646f a101  jc..r.e.jc.8do..
+00000510: 6e02 6401 5a64 6504 6a65 5a66 6504 6a67  n.d.Zde.jeZfe.jg
+00000520: 5a68 6504 6a69 5a6a 6504 6a6b 5a6c 6504  Zhe.jiZje.jkZle.
+00000530: 6a6d 5a6e 6504 6a6f 5a70 6504 6a71 5a72  jmZne.joZpe.jqZr
+00000540: 6504 6a73 5a74 6504 6a75 5a76 6504 6a77  e.jsZte.juZve.jw
+00000550: 5a78 6504 6a79 5a7a 7910 6500 a07b 6504  Zxe.jyZzy.e..{e.
+00000560: 6a7c a101 5a7d 5700 6e36 0400 657e 6b0a  j|..Z}W.n6..e~k.
+00000570: 9005 7274 0100 5a1c 0100 7a16 6506 6a7f  ..rt..Z...z.e.j.
+00000580: 6470 651c 6471 8d02 0100 6900 5a7d 5700  dpe.dq....i.Z}W.
+00000590: 6401 6401 5a1c 5b1c 5800 5900 6e02 5800  d.d.Z.[.X.Y.n.X.
+000005a0: 6504 6a80 5a81 6504 6a82 5a83 6504 6a84  e.j.Z.e.j.Z.e.j.
+000005b0: 5a85 6504 6a86 5a87 6504 6a88 5a89 6504  Z.e.j.Z.e.j.Z.e.
+000005c0: 6a8a 5a8b 6504 6a8c 5a8d 6504 6a8e 5a8f  j.Z.e.j.Z.e.j.Z.
+000005d0: 6501 6a90 a091 6472 a101 5a92 6401 5300  e.j...dr..Z.d.S.
+000005e0: 2973 e900 0000 004e 2902 da06 6465 6669  )s.....N)...defi
+000005f0: 6e65 da07 6f70 7469 6f6e 7329 01da 066c  ne..options)...l
+00000600: 6f67 6765 7229 01da 056d 6564 6961 2902  ogger)...media).
+00000610: da11 7061 7273 655f 656e 7669 726f 6e6d  ..parse_environm
+00000620: 656e 74da 1170 6172 7365 5f63 6f6e 6669  ent..parse_confi
+00000630: 675f 6669 6c65 7a08 6a65 742e 636f 6e66  g_filez.jet.conf
+00000640: 7a17 6874 7470 733a 2f2f 6170 702e 6a65  z.https://app.je
+00000650: 7461 646d 696e 2e69 6f7a 1b68 7474 7073  tadmin.ioz.https
+00000660: 3a2f 2f61 7069 2e6a 6574 6164 6d69 6e2e  ://api.jetadmin.
+00000670: 696f 2f61 7069 da07 6164 6472 6573 737a  io/api..addressz
+00000680: 0730 2e30 2e30 2e30 7a0e 7365 7276 6572  .0.0.0.0z.server
+00000690: 2061 6464 7265 7373 2902 da07 6465 6661   address)...defa
+000006a0: 756c 74da 0468 656c 70da 0470 6f72 7469  ult..help..porti
+000006b0: b822 0000 7a0b 7365 7276 6572 2070 6f72  ."..z.server por
+000006c0: 7429 0372 0900 0000 720a 0000 00da 0474  t).r....r......t
+000006d0: 7970 65da 0777 6f72 6b65 7273 e901 0000  ype..workers....
+000006e0: 007a 116e 756d 6265 7220 6f66 2077 6f72  .z.number of wor
+000006f0: 6b65 7273 da06 636f 6e66 6967 7a10 636f  kers..configz.co
+00000700: 6e66 6967 2066 696c 6520 7061 7468 da12  nfig file path..
+00000710: 7573 655f 6465 6661 756c 745f 636f 6e66  use_default_conf
+00000720: 6967 da00 7a19 7573 6520 6465 6661 756c  ig..z.use defaul
+00000730: 7420 636f 6e66 6967 2076 616c 7565 73da  t config values.
+00000740: 0564 6562 7567 467a 0a64 6562 7567 206d  .debugFz.debug m
+00000750: 6f64 65da 0972 6561 645f 6f6e 6c79 7a09  ode..read_onlyz.
+00000760: 7265 6164 206f 6e6c 79da 0774 6872 6561  read only..threa
+00000770: 6473 da0b 636f 6e6e 6563 7469 6f6e 73e9  ds..connections.
+00000780: 3200 0000 5a08 636f 6e6e 6563 7473 da12  2...Z.connects..
+00000790: 6175 746f 5f6f 7065 6e5f 7265 6769 7374  auto_open_regist
+000007a0: 6572 547a 216f 7065 6e20 746f 6b65 6e20  erTz!open token 
+000007b0: 7265 6769 7374 6572 2061 7574 6f6d 6174  register automat
+000007c0: 6963 616c 6c79 da07 7072 6f6a 6563 7429  ically..project)
+000007d0: 0272 0a00 0000 720c 0000 00da 0574 6f6b  .r....r......tok
+000007e0: 656e da0b 656e 7669 726f 6e6d 656e 74da  en..environment.
+000007f0: 0c63 6f72 735f 6865 6164 6572 737a 1061  .cors_headersz.a
+00000800: 6464 2043 4f52 5320 6865 6164 6572 73da  dd CORS headers.
+00000810: 0862 6173 655f 7572 6c7a 0862 6173 6520  .base_urlz.base 
+00000820: 5552 4cda 0e6a 7774 5f76 6572 6966 795f  URL..jwt_verify_
+00000830: 6b65 797a 0e4a 5754 2076 6572 6966 7920  keyz.JWT verify 
+00000840: 6b65 7929 0372 0a00 0000 720c 0000 0072  key).r....r....r
+00000850: 0900 0000 da0f 6265 6172 6572 5f61 7574  ......bearer_aut
+00000860: 685f 6b65 797a 0f42 6561 7265 7220 6175  h_keyz.Bearer au
+00000870: 7468 206b 6579 da10 656e 7669 726f 6e6d  th key..environm
+00000880: 656e 745f 7479 7065 7a10 656e 7669 726f  ent_typez.enviro
+00000890: 6e6d 656e 7420 7479 7065 da0c 7765 625f  nment type..web_
+000008a0: 6261 7365 5f75 726c 7a27 4a65 7420 4164  base_urlz'Jet Ad
+000008b0: 6d69 6e20 6672 6f6e 7465 6e64 2061 7070  min frontend app
+000008c0: 6c69 6361 7469 6f6e 2062 6173 6520 5552  lication base UR
+000008d0: 4cda 0c61 7069 5f62 6173 655f 7572 6c7a  L..api_base_urlz
+000008e0: 164a 6574 2041 646d 696e 2041 5049 2062  .Jet Admin API b
+000008f0: 6173 6520 5552 4cda 0d6d 6564 6961 5f73  ase URL..media_s
+00000900: 746f 7261 6765 7a12 6d65 6469 6120 7374  toragez.media st
+00000910: 6f72 6167 6520 7479 7065 da0a 6d65 6469  orage type..medi
+00000920: 615f 726f 6f74 7205 0000 007a 0a6d 6564  a_rootr....z.med
+00000930: 6961 2072 6f6f 74da 0e6d 6564 6961 5f62  ia root..media_b
+00000940: 6173 655f 7572 6c7a 0e6d 6564 6961 2062  ase_urlz.media b
+00000950: 6173 6520 5552 4cda 0f64 6174 6162 6173  ase URL..databas
+00000960: 655f 656e 6769 6e65 7a56 6461 7461 6261  e_enginezVdataba
+00000970: 7365 2065 6e67 696e 6520 2870 6f73 7467  se engine (postg
+00000980: 7265 7371 6c2c 206d 7973 716c 2c20 6f72  resql, mysql, or
+00000990: 6163 6c65 2c20 6d73 7371 6c2b 7079 6f64  acle, mssql+pyod
+000009a0: 6263 2c20 6269 6771 7565 7279 2c20 736e  bc, bigquery, sn
+000009b0: 6f77 666c 616b 652c 2073 716c 6974 6529  owflake, sqlite)
+000009c0: 2901 720a 0000 00da 0d64 6174 6162 6173  ).r......databas
+000009d0: 655f 686f 7374 7a0d 6461 7461 6261 7365  e_hostz.database
+000009e0: 2068 6f73 74da 0d64 6174 6162 6173 655f   host..database_
+000009f0: 706f 7274 7a0d 6461 7461 6261 7365 2070  portz.database p
+00000a00: 6f72 74da 0d64 6174 6162 6173 655f 7573  ort..database_us
+00000a10: 6572 7a0d 6461 7461 6261 7365 2075 7365  erz.database use
+00000a20: 72da 1164 6174 6162 6173 655f 7061 7373  r..database_pass
+00000a30: 776f 7264 7a11 6461 7461 6261 7365 2070  wordz.database p
+00000a40: 6173 7377 6f72 64da 0d64 6174 6162 6173  assword..databas
+00000a50: 655f 6e61 6d65 7a15 6461 7461 6261 7365  e_namez.database
+00000a60: 206e 616d 6520 6f72 2070 6174 68da 0e64   name or path..d
+00000a70: 6174 6162 6173 655f 6578 7472 617a 1964  atabase_extraz.d
+00000a80: 6174 6162 6173 6520 6578 7472 6120 7061  atabase extra pa
+00000a90: 7261 6d65 7465 7273 da0d 6461 7461 6261  rameters..databa
+00000aa0: 7365 5f6f 6e6c 7929 0272 0900 0000 720c  se_only).r....r.
+00000ab0: 0000 00da 0f64 6174 6162 6173 655f 6578  .....database_ex
+00000ac0: 6365 7074 da13 6461 7461 6261 7365 5f6d  cept..database_m
+00000ad0: 6178 5f74 6162 6c65 73da 0f64 6174 6162  ax_tables..datab
+00000ae0: 6173 655f 7363 6865 6d61 da11 6461 7461  ase_schema..data
+00000af0: 6261 7365 5f73 7368 5f68 6f73 74da 1164  base_ssh_host..d
+00000b00: 6174 6162 6173 655f 7373 685f 706f 7274  atabase_ssh_port
+00000b10: da11 6461 7461 6261 7365 5f73 7368 5f75  ..database_ssh_u
+00000b20: 7365 72da 1864 6174 6162 6173 655f 7373  ser..database_ss
+00000b30: 685f 7072 6976 6174 655f 6b65 79da 0f63  h_private_key..c
+00000b40: 6f6f 6b69 655f 7361 6d65 7369 7465 da04  ookie_samesite..
+00000b50: 4e6f 6e65 da0d 636f 6f6b 6965 5f73 6563  None..cookie_sec
+00000b60: 7572 65da 0d63 6f6f 6b69 655f 646f 6d61  ure..cookie_doma
+00000b70: 696e da0f 636f 6f6b 6965 5f63 6f6d 7072  in..cookie_compr
+00000b80: 6573 73da 0a73 746f 7265 5f70 6174 687a  ess..store_pathz
+00000b90: 186a 6574 5f62 7269 6467 655f 7374 6f72  .jet_bridge_stor
+00000ba0: 652e 7371 6c69 7465 33da 1073 736f 5f61  e.sqlite3..sso_a
+00000bb0: 7070 6c69 6361 7469 6f6e 737a 027b 7dda  pplicationsz.{}.
+00000bc0: 0c61 6c6c 6f77 5f6f 7269 6769 6eda 012a  .allow_origin..*
+00000bd0: 2901 7209 0000 00da 0f74 7261 636b 5f64  ).r......track_d
+00000be0: 6174 6162 6173 6573 da18 7472 6163 6b5f  atabases..track_
+00000bf0: 6461 7461 6261 7365 735f 656e 6470 6f69  databases_endpoi
+00000c00: 6e74 da14 7472 6163 6b5f 6461 7461 6261  nt..track_databa
+00000c10: 7365 735f 6175 7468 da15 7472 6163 6b5f  ses_auth..track_
+00000c20: 6d6f 6465 6c73 5f65 6e64 706f 696e 74da  models_endpoint.
+00000c30: 1174 7261 636b 5f6d 6f64 656c 735f 6175  .track_models_au
+00000c40: 7468 da0c 6469 7361 626c 655f 6175 7468  th..disable_auth
+00000c50: da0a 7365 6e74 7279 5f64 736e 2901 da05  ..sentry_dsn)...
+00000c60: 6669 6e61 6c5a 034a 4554 da04 6e6f 6e65  finalZ.JET..none
+00000c70: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
+00000c80: 0043 0000 0073 1400 0000 7c00 7400 6b07  .C...s....|.t.k.
+00000c90: 7012 7400 7c00 1900 6400 6b08 5300 2901  p.t.|...d.k.S.).
+00000ca0: 4e29 0172 0300 0000 2901 da01 78a9 0072  N).r....)...x..r
+00000cb0: 4700 0000 fa55 2f55 7365 7273 2f66 316e  G....U/Users/f1n
+00000cc0: 616c 2f44 726f 7062 6f78 2f70 7974 686f  al/Dropbox/pytho
+00000cd0: 6e2f 6a65 742d 6272 6964 6765 2f73 7263  n/jet-bridge/src
+00000ce0: 2f70 6163 6b61 6765 732f 6a65 745f 6272  /packages/jet_br
+00000cf0: 6964 6765 2f6a 6574 5f62 7269 6467 652f  idge/jet_bridge/
+00000d00: 7365 7474 696e 6773 2e70 79da 083c 6c61  settings.py..<la
+00000d10: 6d62 6461 3e74 0000 00f3 0000 0000 7249  mbda>t........rI
+00000d20: 0000 00fa 012c 7a1f 5353 4f5f 4150 504c  .....,z.SSO_APPL
+00000d30: 4943 4154 494f 4e53 2070 6172 7369 6e67  ICATIONS parsing
+00000d40: 2066 6169 6c65 6429 01da 0865 7863 5f69   failed)...exc_i
+00000d50: 6e66 6fda 0d50 4f53 5349 424c 455f 484f  nfo..POSSIBLE_HO
+00000d60: 5354 2993 da04 6a73 6f6e da02 6f73 da0f  ST)...json..os..
+00000d70: 746f 726e 6164 6f2e 6f70 7469 6f6e 7372  tornado.optionsr
+00000d80: 0200 0000 7203 0000 00da 166a 6574 5f62  ....r......jet_b
+00000d90: 7269 6467 655f 6261 7365 2e6c 6f67 6765  ridge_base.logge
+00000da0: 7272 0400 0000 da0a 6a65 745f 6272 6964  rr......jet_brid
+00000db0: 6765 7205 0000 005a 196a 6574 5f62 7269  ger....Z.jet_bri
+00000dc0: 6467 652e 7574 696c 732e 7365 7474 696e  dge.utils.settin
+00000dd0: 6773 7206 0000 0072 0700 0000 da04 7061  gsr....r......pa
+00000de0: 7468 da07 6469 726e 616d 65da 0761 6273  th..dirname..abs
+00000df0: 7061 7468 da08 5f5f 6669 6c65 5f5f da08  path..__file__..
+00000e00: 4241 5345 5f44 4952 da04 6a6f 696e 5a13  BASE_DIR..joinZ.
+00000e10: 4445 4641 554c 545f 434f 4e46 4947 5f50  DEFAULT_CONFIG_P
+00000e20: 4154 485a 1444 4546 4155 4c54 5f57 4542  ATHZ.DEFAULT_WEB
+00000e30: 5f42 4153 455f 5552 4c5a 1444 4546 4155  _BASE_URLZ.DEFAU
+00000e40: 4c54 5f41 5049 5f42 4153 455f 5552 4cda  LT_API_BASE_URL.
+00000e50: 0369 6e74 da04 626f 6f6c da03 7374 725a  .int..bool..strZ
+00000e60: 124d 4544 4941 5f53 544f 5241 4745 5f46  .MEDIA_STORAGE_F
+00000e70: 494c 455a 1270 6172 7365 5f63 6f6d 6d61  ILEZ.parse_comma
+00000e80: 6e64 5f6c 696e 6572 0f00 0000 da07 494f  nd_liner......IO
+00000e90: 4572 726f 72da 0165 da07 7761 726e 696e  Error..e..warnin
+00000ea0: 675a 1072 6571 7569 7265 645f 6f70 7469  gZ.required_opti
+00000eb0: 6f6e 73da 2072 6571 7569 7265 645f 6f70  ons. required_op
+00000ec0: 7469 6f6e 735f 7769 7468 6f75 745f 6465  tions_without_de
+00000ed0: 6661 756c 7472 2500 0000 da06 6170 7065  faultr%.....appe
+00000ee0: 6e64 da04 6c69 7374 da06 6669 6c74 6572  nd..list..filter
+00000ef0: da0f 6d69 7373 696e 675f 6f70 7469 6f6e  ..missing_option
+00000f00: 7372 0800 0000 da07 4144 4452 4553 5372  sr......ADDRESSr
+00000f10: 0b00 0000 da04 504f 5254 720d 0000 00da  ......PORTr.....
+00000f20: 0757 4f52 4b45 5253 7212 0000 00da 0544  .WORKERSr......D
+00000f30: 4542 5547 7213 0000 00da 0952 4541 445f  EBUGr......READ_
+00000f40: 4f4e 4c59 7214 0000 005a 0754 4852 4541  ONLYr....Z.THREA
+00000f50: 4453 7215 0000 00da 0b43 4f4e 4e45 4354  DSr......CONNECT
+00000f60: 494f 4e53 7217 0000 00da 1241 5554 4f5f  IONSr......AUTO_
+00000f70: 4f50 454e 5f52 4547 4953 5445 525a 0643  OPEN_REGISTERZ.C
+00000f80: 4f4e 4649 4772 1000 0000 da05 6c6f 7765  ONFIGr......lowe
+00000f90: 72da 0573 706c 6974 5a12 5553 455f 4445  r..splitZ.USE_DE
+00000fa0: 4641 554c 545f 434f 4e46 4947 7218 0000  FAULT_CONFIGr...
+00000fb0: 00da 0750 524f 4a45 4354 7219 0000 00da  ...PROJECTr.....
+00000fc0: 0554 4f4b 454e 721a 0000 00da 0b45 4e56  .TOKENr......ENV
+00000fd0: 4952 4f4e 4d45 4e54 721b 0000 00da 0c43  IRONMENTr......C
+00000fe0: 4f52 535f 4845 4144 4552 5372 1c00 0000  ORS_HEADERSr....
+00000ff0: da08 4241 5345 5f55 524c 721d 0000 00da  ..BASE_URLr.....
+00001000: 0e4a 5754 5f56 4552 4946 595f 4b45 5972  .JWT_VERIFY_KEYr
+00001010: 1e00 0000 da0f 4245 4152 4552 5f41 5554  ......BEARER_AUT
+00001020: 485f 4b45 5972 1f00 0000 da10 454e 5649  H_KEYr......ENVI
+00001030: 524f 4e4d 454e 545f 5459 5045 7220 0000  RONMENT_TYPEr ..
+00001040: 00da 0c57 4542 5f42 4153 455f 5552 4c72  ...WEB_BASE_URLr
+00001050: 2100 0000 da0c 4150 495f 4241 5345 5f55  !.....API_BASE_U
+00001060: 524c 7222 0000 005a 0d4d 4544 4941 5f53  RLr"...Z.MEDIA_S
+00001070: 544f 5241 4745 7223 0000 00da 0a4d 4544  TORAGEr#.....MED
+00001080: 4941 5f52 4f4f 5472 2400 0000 da0e 4d45  IA_ROOTr$.....ME
+00001090: 4449 415f 4241 5345 5f55 524c da0f 4441  DIA_BASE_URL..DA
+000010a0: 5441 4241 5345 5f45 4e47 494e 4572 2600  TABASE_ENGINEr&.
+000010b0: 0000 da0d 4441 5441 4241 5345 5f48 4f53  ....DATABASE_HOS
+000010c0: 5472 2700 0000 da0d 4441 5441 4241 5345  Tr'.....DATABASE
+000010d0: 5f50 4f52 5472 2800 0000 da0d 4441 5441  _PORTr(.....DATA
+000010e0: 4241 5345 5f55 5345 5272 2900 0000 da11  BASE_USERr).....
+000010f0: 4441 5441 4241 5345 5f50 4153 5357 4f52  DATABASE_PASSWOR
+00001100: 4472 2a00 0000 da0d 4441 5441 4241 5345  Dr*.....DATABASE
+00001110: 5f4e 414d 4572 2b00 0000 da0e 4441 5441  _NAMEr+.....DATA
+00001120: 4241 5345 5f45 5854 5241 722c 0000 00da  BASE_EXTRAr,....
+00001130: 0d44 4154 4142 4153 455f 4f4e 4c59 722d  .DATABASE_ONLYr-
+00001140: 0000 00da 0f44 4154 4142 4153 455f 4558  .....DATABASE_EX
+00001150: 4345 5054 722e 0000 00da 1344 4154 4142  CEPTr......DATAB
+00001160: 4153 455f 4d41 585f 5441 424c 4553 722f  ASE_MAX_TABLESr/
+00001170: 0000 00da 0f44 4154 4142 4153 455f 5343  .....DATABASE_SC
+00001180: 4845 4d41 7230 0000 00da 1144 4154 4142  HEMAr0.....DATAB
+00001190: 4153 455f 5353 485f 484f 5354 7231 0000  ASE_SSH_HOSTr1..
+000011a0: 00da 1144 4154 4142 4153 455f 5353 485f  ...DATABASE_SSH_
+000011b0: 504f 5254 7232 0000 00da 1144 4154 4142  PORTr2.....DATAB
+000011c0: 4153 455f 5353 485f 5553 4552 7233 0000  ASE_SSH_USERr3..
+000011d0: 00da 1844 4154 4142 4153 455f 5353 485f  ...DATABASE_SSH_
+000011e0: 5052 4956 4154 455f 4b45 5972 3400 0000  PRIVATE_KEYr4...
+000011f0: da0f 434f 4f4b 4945 5f53 414d 4553 4954  ..COOKIE_SAMESIT
+00001200: 4572 3600 0000 da0d 434f 4f4b 4945 5f53  Er6.....COOKIE_S
+00001210: 4543 5552 4572 3700 0000 da0d 434f 4f4b  ECUREr7.....COOK
+00001220: 4945 5f44 4f4d 4149 4e72 3800 0000 da0f  IE_DOMAINr8.....
+00001230: 434f 4f4b 4945 5f43 4f4d 5052 4553 5372  COOKIE_COMPRESSr
+00001240: 3900 0000 da0a 5354 4f52 455f 5041 5448  9.....STORE_PATH
+00001250: da05 6c6f 6164 7372 3a00 0000 da10 5353  ..loadsr:.....SS
+00001260: 4f5f 4150 504c 4943 4154 494f 4e53 da09  O_APPLICATIONS..
+00001270: 4578 6365 7074 696f 6eda 0565 7272 6f72  Exception..error
+00001280: 723b 0000 00da 0c41 4c4c 4f57 5f4f 5249  r;.....ALLOW_ORI
+00001290: 4749 4e72 3d00 0000 da0f 5452 4143 4b5f  GINr=.....TRACK_
+000012a0: 4441 5441 4241 5345 5372 3e00 0000 da18  DATABASESr>.....
+000012b0: 5452 4143 4b5f 4441 5441 4241 5345 535f  TRACK_DATABASES_
+000012c0: 454e 4450 4f49 4e54 723f 0000 00da 1454  ENDPOINTr?.....T
+000012d0: 5241 434b 5f44 4154 4142 4153 4553 5f41  RACK_DATABASES_A
+000012e0: 5554 4872 4000 0000 da15 5452 4143 4b5f  UTHr@.....TRACK_
+000012f0: 4d4f 4445 4c53 5f45 4e44 504f 494e 5472  MODELS_ENDPOINTr
+00001300: 4100 0000 da11 5452 4143 4b5f 4d4f 4445  A.....TRACK_MODE
+00001310: 4c53 5f41 5554 4872 4200 0000 da0c 4449  LS_AUTHrB.....DI
+00001320: 5341 424c 455f 4155 5448 7243 0000 005a  SABLE_AUTHrC...Z
+00001330: 0a53 454e 5452 595f 4453 4eda 0765 6e76  .SENTRY_DSN..env
+00001340: 6972 6f6e da03 6765 7472 4d00 0000 7247  iron..getrM...rG
+00001350: 0000 0072 4700 0000 7247 0000 0072 4800  ...rG...rG...rH.
+00001360: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001370: 7310 0100 0008 0108 0210 020c 020c 0110  s...............
+00001380: 0414 010c 0404 0104 020e 0110 0110 010e  ................
+00001390: 010e 0110 0110 0110 0110 0110 010e 010e  ................
+000013a0: 010e 0110 010e 0110 0110 0110 020e 010e  ................
+000013b0: 0210 010e 010e 020c 010c 010c 010c 010c  ................
+000013c0: 010c 010e 010e 010e 010e 010e 020e 010e  ................
+000013d0: 010e 010e 020e 010e 010e 010e 020e 020e  ................
+000013e0: 010c 020c 010c 010c 020c 010c 020e 020c  ................
+000013f0: 040c 0208 0102 0116 0112 010c 011c 020c  ................
+00001400: 0302 0102 0102 0102 0106 0606 030c 010a  ................
+00001410: 010a 0212 0406 0106 0106 0106 0106 0106  ................
+00001420: 0106 0106 0106 0110 0106 0106 0106 0106  ................
+00001430: 0106 0106 0106 0106 0206 0106 0206 0106  ................
+00001440: 0106 0206 0106 0106 0106 0106 0106 0106  ................
+00001450: 0118 0118 0106 0106 0206 0106 0106 0106  ................
+00001460: 0206 0106 0106 0106 0206 0202 0110 0112  ................
+00001470: 010e 0116 0206 0206 0106 0106 0206 0106  ................
+00001480: 0206 0206 02                             .....
```

### Comparing `jet-bridge-1.7.9/jet_bridge/__pycache__/configuration.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/__pycache__/configuration.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 76b0 eb63 e716 0000 e300 0000  3...v..c........
+00000000: 330d 0d0a aaa6 c264 0c18 0000 e300 0000  3......d........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6200 0000 6400 6401 6c00 5a00 6400  .sb...d.d.l.Z.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 650a 6406 8301 6509 6a0b 650a 6407  ..e.d...e.j.e.d.
 00000070: 8301 3c00 4700 6408 6409 8400 6409 6502  ..<.G.d.d...d.e.
@@ -42,295 +42,304 @@
 00000290: 0400 0000 7400 5300 2901 4e29 0172 0500  ....t.S.).N).r..
 000002a0: 0000 2901 720b 0000 0072 0a00 0000 720a  ..).r....r....r.
 000002b0: 0000 0072 0c00 0000 da0b 6765 745f 7665  ...r......get_ve
 000002c0: 7273 696f 6e12 0000 0073 0200 0000 0001  rsion....s......
 000002d0: 7a22 4a65 7442 7269 6467 6543 6f6e 6669  z"JetBridgeConfi
 000002e0: 6775 7261 7469 6f6e 2e67 6574 5f76 6572  guration.get_ver
 000002f0: 7369 6f6e 6301 0000 0000 0000 0001 0000  sionc...........
-00000300: 0029 0000 0043 0000 0073 ac00 0000 7400  .)...C...s....t.
+00000300: 002e 0000 0043 0000 0073 c000 0000 7400  .....C...s....t.
 00000310: 6a01 7400 6a02 7400 6a03 7400 6a04 7400  j.t.j.t.j.t.j.t.
 00000320: 6a05 7400 6a06 7400 6a07 7400 6a08 7400  j.t.j.t.j.t.j.t.
 00000330: 6a09 7400 6a0a 7400 6a0b 7400 6a0c 7400  j.t.j.t.j.t.j.t.
 00000340: 6a0d 7400 6a0e 7400 6a0f 7400 6a10 7400  j.t.j.t.j.t.j.t.
 00000350: 6a11 7400 6a12 7400 6a13 7400 6a14 7400  j.t.j.t.j.t.j.t.
 00000360: 6a15 7400 6a16 7400 6a17 7400 6a18 7400  j.t.j.t.j.t.j.t.
 00000370: 6a19 7400 6a1a 7400 6a1b 7400 6a1c 7400  j.t.j.t.j.t.j.t.
 00000380: 6a1d 7400 6a1e 7400 6a1f 7400 6a20 7400  j.t.j.t.j.t.j t.
-00000390: 6a21 7c00 6a22 7400 6a23 8301 7400 6a24  j!|.j"t.j#..t.j$
-000003a0: 7400 6a25 7400 6a26 7400 6a27 7400 6a28  t.j%t.j&t.j't.j(
-000003b0: 7400 6a29 6401 9c28 5300 2902 4e29 28da  t.j)d..(S.).N)(.
-000003c0: 0544 4542 5547 da09 5245 4144 5f4f 4e4c  .DEBUG..READ_ONL
-000003d0: 59da 1241 5554 4f5f 4f50 454e 5f52 4547  Y..AUTO_OPEN_REG
-000003e0: 4953 5445 52da 0c57 4542 5f42 4153 455f  ISTER..WEB_BASE_
-000003f0: 5552 4cda 0c41 5049 5f42 4153 455f 5552  URL..API_BASE_UR
-00000400: 4cda 0750 524f 4a45 4354 da05 544f 4b45  L..PROJECT..TOKE
-00000410: 4eda 0b45 4e56 4952 4f4e 4d45 4e54 da0c  N..ENVIRONMENT..
-00000420: 434f 5253 5f48 4541 4445 5253 da08 4241  CORS_HEADERS..BA
-00000430: 5345 5f55 524c da0e 4a57 545f 5645 5249  SE_URL..JWT_VERI
-00000440: 4659 5f4b 4559 da0f 4245 4152 4552 5f41  FY_KEY..BEARER_A
-00000450: 5554 485f 4b45 59da 1045 4e56 4952 4f4e  UTH_KEY..ENVIRON
-00000460: 4d45 4e54 5f54 5950 45da 0f44 4154 4142  MENT_TYPE..DATAB
-00000470: 4153 455f 454e 4749 4e45 da0d 4441 5441  ASE_ENGINE..DATA
-00000480: 4241 5345 5f48 4f53 54da 0d44 4154 4142  BASE_HOST..DATAB
-00000490: 4153 455f 504f 5254 da0d 4441 5441 4241  ASE_PORT..DATABA
-000004a0: 5345 5f55 5345 52da 1144 4154 4142 4153  SE_USER..DATABAS
-000004b0: 455f 5041 5353 574f 5244 da0d 4441 5441  E_PASSWORD..DATA
-000004c0: 4241 5345 5f4e 414d 45da 0e44 4154 4142  BASE_NAME..DATAB
-000004d0: 4153 455f 4558 5452 41da 1444 4154 4142  ASE_EXTRA..DATAB
-000004e0: 4153 455f 434f 4e4e 4543 5449 4f4e 53da  ASE_CONNECTIONS.
-000004f0: 0d44 4154 4142 4153 455f 4f4e 4c59 da0f  .DATABASE_ONLY..
-00000500: 4441 5441 4241 5345 5f45 5843 4550 54da  DATABASE_EXCEPT.
-00000510: 0f44 4154 4142 4153 455f 5343 4845 4d41  .DATABASE_SCHEMA
-00000520: da11 4441 5441 4241 5345 5f53 5348 5f48  ..DATABASE_SSH_H
-00000530: 4f53 54da 1144 4154 4142 4153 455f 5353  OST..DATABASE_SS
-00000540: 485f 504f 5254 da11 4441 5441 4241 5345  H_PORT..DATABASE
-00000550: 5f53 5348 5f55 5345 52da 1844 4154 4142  _SSH_USER..DATAB
-00000560: 4153 455f 5353 485f 5052 4956 4154 455f  ASE_SSH_PRIVATE_
-00000570: 4b45 59da 0f43 4f4f 4b49 455f 5341 4d45  KEY..COOKIE_SAME
-00000580: 5349 5445 da0d 434f 4f4b 4945 5f53 4543  SITE..COOKIE_SEC
-00000590: 5552 45da 0d43 4f4f 4b49 455f 444f 4d41  URE..COOKIE_DOMA
-000005a0: 494e da0f 434f 4f4b 4945 5f43 4f4d 5052  IN..COOKIE_COMPR
-000005b0: 4553 53da 0a53 544f 5245 5f50 4154 48da  ESS..STORE_PATH.
-000005c0: 1053 534f 5f41 5050 4c49 4341 5449 4f4e  .SSO_APPLICATION
-000005d0: 53da 0c41 4c4c 4f57 5f4f 5249 4749 4eda  S..ALLOW_ORIGIN.
-000005e0: 0f54 5241 434b 5f44 4154 4142 4153 4553  .TRACK_DATABASES
-000005f0: da18 5452 4143 4b5f 4441 5441 4241 5345  ..TRACK_DATABASE
-00000600: 535f 454e 4450 4f49 4e54 da14 5452 4143  S_ENDPOINT..TRAC
-00000610: 4b5f 4441 5441 4241 5345 535f 4155 5448  K_DATABASES_AUTH
-00000620: da15 5452 4143 4b5f 4d4f 4445 4c53 5f45  ..TRACK_MODELS_E
-00000630: 4e44 504f 494e 54da 1154 5241 434b 5f4d  NDPOINT..TRACK_M
-00000640: 4f44 454c 535f 4155 5448 292a 7204 0000  ODELS_AUTH)*r...
-00000650: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000660: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000670: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00000680: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00000690: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000006a0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000006b0: 7222 0000 005a 0b43 4f4e 4e45 4354 494f  r"...Z.CONNECTIO
-000006c0: 4e53 7224 0000 0072 2500 0000 7226 0000  NSr$...r%...r&..
-000006d0: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
-000006e0: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
-000006f0: 2d00 0000 722e 0000 0072 2f00 0000 da16  -...r....r/.....
-00000700: 636c 6561 6e5f 7373 6f5f 6170 706c 6963  clean_sso_applic
-00000710: 6174 696f 6e73 7230 0000 0072 3100 0000  ationsr0...r1...
-00000720: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
-00000730: 3500 0000 7236 0000 0029 0172 0b00 0000  5...r6...).r....
-00000740: 720a 0000 0072 0a00 0000 720c 0000 00da  r....r....r.....
-00000750: 0c67 6574 5f73 6574 7469 6e67 7315 0000  .get_settings...
-00000760: 0073 5000 0000 0002 0401 0401 0401 0401  .sP.............
-00000770: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-00000780: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-00000790: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-000007a0: 0401 0401 0401 0401 0401 0a01 0401 0401  ................
-000007b0: 0401 0401 0401 7a23 4a65 7442 7269 6467  ......z#JetBridg
-000007c0: 6543 6f6e 6669 6775 7261 7469 6f6e 2e67  eConfiguration.g
-000007d0: 6574 5f73 6574 7469 6e67 7363 0200 0000  et_settingsc....
-000007e0: 0000 0000 0600 0000 0600 0000 4300 0000  ............C...
-000007f0: 735e 0000 0074 006a 016a 027c 0183 015c  s^...t.j.j.|...\
-00000800: 027d 027d 0374 006a 016a 037c 0383 015c  .}.}.t.j.j.|...\
-00000810: 027d 047d 0578 3874 006a 016a 0474 006a  .}.}.x8t.j.j.t.j
-00000820: 016a 0574 066a 077c 0183 0283 0172 5874  .j.t.j.|.....rXt
-00000830: 006a 016a 057c 0264 017c 0474 0864 0283  .j.j.|.d.|.t.d..
-00000840: 017c 0566 0316 0083 027d 0171 2257 007c  .|.f.....}.q"W.|
-00000850: 0153 0029 034e 7a07 2573 5f25 7325 73e9  .S.).Nz.%s_%s%s.
-00000860: 0700 0000 2909 da02 6f73 da04 7061 7468  ....)...os..path
-00000870: da05 7370 6c69 74da 0873 706c 6974 6578  ..split..splitex
-00000880: 74da 0665 7869 7374 73da 046a 6f69 6e72  t..exists..joinr
-00000890: 0400 0000 da0a 4d45 4449 415f 524f 4f54  ......MEDIA_ROOT
-000008a0: 7203 0000 0029 0672 0b00 0000 723b 0000  r....).r....r;..
-000008b0: 005a 0864 6972 5f6e 616d 65da 0966 696c  .Z.dir_name..fil
-000008c0: 655f 6e61 6d65 5a09 6669 6c65 5f72 6f6f  e_nameZ.file_roo
-000008d0: 745a 0866 696c 655f 6578 7472 0a00 0000  tZ.file_extr....
-000008e0: 720a 0000 0072 0c00 0000 da18 6d65 6469  r....r......medi
-000008f0: 615f 6765 745f 6176 6169 6c61 626c 655f  a_get_available_
-00000900: 6e61 6d65 4100 0000 730a 0000 0000 0110  nameA...s.......
-00000910: 0110 021a 0120 027a 2f4a 6574 4272 6964  ..... .z/JetBrid
-00000920: 6765 436f 6e66 6967 7572 6174 696f 6e2e  geConfiguration.
-00000930: 6d65 6469 615f 6765 745f 6176 6169 6c61  media_get_availa
-00000940: 626c 655f 6e61 6d65 6302 0000 0000 0000  ble_namec.......
-00000950: 0003 0000 0003 0000 0043 0000 0073 1c00  .........C...s..
-00000960: 0000 7400 6a01 6a02 7403 6a04 7c01 8302  ..t.j.j.t.j.|...
-00000970: 7d02 7400 6a01 6a05 7c02 8301 5300 2901  }.t.j.j.|...S.).
-00000980: 4e29 0672 3a00 0000 723b 0000 0072 3f00  N).r:...r;...r?.
-00000990: 0000 7204 0000 0072 4000 0000 723e 0000  ..r....r@...r>..
-000009a0: 0029 0372 0b00 0000 723b 0000 00da 0d61  .).r....r;.....a
-000009b0: 6273 6f6c 7574 655f 7061 7468 720a 0000  bsolute_pathr...
-000009c0: 0072 0a00 0000 720c 0000 00da 0c6d 6564  .r....r......med
-000009d0: 6961 5f65 7869 7374 734a 0000 0073 0400  ia_existsJ...s..
-000009e0: 0000 0001 1001 7a23 4a65 7442 7269 6467  ......z#JetBridg
-000009f0: 6543 6f6e 6669 6775 7261 7469 6f6e 2e6d  eConfiguration.m
-00000a00: 6564 6961 5f65 7869 7374 7363 0200 0000  edia_existsc....
-00000a10: 0000 0000 0800 0000 0400 0000 4300 0000  ............C...
-00000a20: 734e 0000 0074 006a 016a 0274 036a 047c  sN...t.j.j.t.j.|
-00000a30: 0183 027d 0267 007d 0367 007d 0478 2c74  ...}.g.}.g.}.x,t
-00000a40: 006a 057c 0283 0144 005d 1e5c 037d 057d  .j.|...D.].\.}.}
-00000a50: 067d 077c 036a 067c 0683 0101 007c 046a  .}.|.j.|.....|.j
-00000a60: 067c 0783 0101 0071 2457 007c 037c 0466  .|.....q$W.|.|.f
-00000a70: 0253 0029 014e 2907 723a 0000 0072 3b00  .S.).N).r:...r;.
-00000a80: 0000 723f 0000 0072 0400 0000 7240 0000  ..r?...r....r@..
-00000a90: 00da 0477 616c 6bda 0665 7874 656e 6429  ...walk..extend)
-00000aa0: 0872 0b00 0000 723b 0000 0072 4300 0000  .r....r;...rC...
-00000ab0: 5a0b 6469 7265 6374 6f72 6965 73da 0566  Z.directories..f
-00000ac0: 696c 6573 da07 6469 7270 6174 68da 0864  iles..dirpath..d
-00000ad0: 6972 6e61 6d65 73da 0966 696c 656e 616d  irnames..filenam
-00000ae0: 6573 720a 0000 0072 0a00 0000 720c 0000  esr....r....r...
-00000af0: 00da 0d6d 6564 6961 5f6c 6973 7464 6972  ...media_listdir
-00000b00: 4e00 0000 730e 0000 0000 0110 0104 0104  N...s...........
-00000b10: 0216 010a 010e 027a 244a 6574 4272 6964  .......z$JetBrid
-00000b20: 6765 436f 6e66 6967 7572 6174 696f 6e2e  geConfiguration.
-00000b30: 6d65 6469 615f 6c69 7374 6469 7263 0200  media_listdirc..
-00000b40: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00000b50: 0000 731c 0000 0074 006a 016a 0274 036a  ..s....t.j.j.t.j
-00000b60: 047c 0183 027d 0274 006a 016a 057c 0283  .|...}.t.j.j.|..
-00000b70: 0153 0029 014e 2906 723a 0000 0072 3b00  .S.).N).r:...r;.
-00000b80: 0000 723f 0000 0072 0400 0000 7240 0000  ..r?...r....r@..
-00000b90: 00da 0867 6574 6d74 696d 6529 0372 0b00  ...getmtime).r..
-00000ba0: 0000 723b 0000 0072 4300 0000 720a 0000  ..r;...rC...r...
-00000bb0: 0072 0a00 0000 720c 0000 00da 176d 6564  .r....r......med
-00000bc0: 6961 5f67 6574 5f6d 6f64 6966 6965 645f  ia_get_modified_
-00000bd0: 7469 6d65 5900 0000 7304 0000 0000 0110  timeY...s.......
-00000be0: 017a 2e4a 6574 4272 6964 6765 436f 6e66  .z.JetBridgeConf
-00000bf0: 6967 7572 6174 696f 6e2e 6d65 6469 615f  iguration.media_
-00000c00: 6765 745f 6d6f 6469 6669 6564 5f74 696d  get_modified_tim
-00000c10: 6563 0200 0000 0000 0000 0300 0000 0300  ec..............
-00000c20: 0000 4300 0000 731c 0000 0074 006a 016a  ..C...s....t.j.j
-00000c30: 0274 036a 047c 0183 027d 0274 006a 016a  .t.j.|...}.t.j.j
-00000c40: 057c 0283 0153 0029 014e 2906 723a 0000  .|...S.).N).r:..
-00000c50: 0072 3b00 0000 723f 0000 0072 0400 0000  .r;...r?...r....
-00000c60: 7240 0000 00da 0767 6574 7369 7a65 2903  r@.....getsize).
-00000c70: 720b 0000 0072 3b00 0000 7243 0000 0072  r....r;...rC...r
-00000c80: 0a00 0000 720a 0000 0072 0c00 0000 da0a  ....r....r......
-00000c90: 6d65 6469 615f 7369 7a65 5d00 0000 7304  media_size]...s.
-00000ca0: 0000 0000 0110 017a 214a 6574 4272 6964  .......z!JetBrid
-00000cb0: 6765 436f 6e66 6967 7572 6174 696f 6e2e  geConfiguration.
-00000cc0: 6d65 6469 615f 7369 7a65 da02 7262 6303  media_size..rbc.
-00000cd0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-00000ce0: 0000 0073 0a00 0000 7400 7c01 7c02 8302  ...s....t.|.|...
-00000cf0: 5300 2901 4e29 01da 046f 7065 6e29 0372  S.).N)...open).r
-00000d00: 0b00 0000 723b 0000 00da 046d 6f64 6572  ....r;.....moder
+00000390: 6a21 7400 6a22 7400 6a23 7400 6a24 7400  j!t.j"t.j#t.j$t.
+000003a0: 6a25 7c00 6a26 7400 6a27 8301 7400 6a28  j%|.j&t.j'..t.j(
+000003b0: 7400 6a29 7400 6a2a 7400 6a2b 7400 6a2c  t.j)t.j*t.j+t.j,
+000003c0: 7400 6a2d 7400 6a2e 6401 9c2d 5300 2902  t.j-t.j.d..-S.).
+000003d0: 4e29 2dda 0544 4542 5547 da09 5245 4144  N)-..DEBUG..READ
+000003e0: 5f4f 4e4c 59da 1241 5554 4f5f 4f50 454e  _ONLY..AUTO_OPEN
+000003f0: 5f52 4547 4953 5445 52da 0c57 4542 5f42  _REGISTER..WEB_B
+00000400: 4153 455f 5552 4cda 0c41 5049 5f42 4153  ASE_URL..API_BAS
+00000410: 455f 5552 4cda 0750 524f 4a45 4354 da05  E_URL..PROJECT..
+00000420: 544f 4b45 4eda 0b45 4e56 4952 4f4e 4d45  TOKEN..ENVIRONME
+00000430: 4e54 da0c 434f 5253 5f48 4541 4445 5253  NT..CORS_HEADERS
+00000440: da08 4241 5345 5f55 524c da0e 4a57 545f  ..BASE_URL..JWT_
+00000450: 5645 5249 4659 5f4b 4559 da0f 4245 4152  VERIFY_KEY..BEAR
+00000460: 4552 5f41 5554 485f 4b45 59da 1045 4e56  ER_AUTH_KEY..ENV
+00000470: 4952 4f4e 4d45 4e54 5f54 5950 45da 0f44  IRONMENT_TYPE..D
+00000480: 4154 4142 4153 455f 454e 4749 4e45 da0d  ATABASE_ENGINE..
+00000490: 4441 5441 4241 5345 5f48 4f53 54da 0d44  DATABASE_HOST..D
+000004a0: 4154 4142 4153 455f 504f 5254 da0d 4441  ATABASE_PORT..DA
+000004b0: 5441 4241 5345 5f55 5345 52da 1144 4154  TABASE_USER..DAT
+000004c0: 4142 4153 455f 5041 5353 574f 5244 da0d  ABASE_PASSWORD..
+000004d0: 4441 5441 4241 5345 5f4e 414d 45da 0e44  DATABASE_NAME..D
+000004e0: 4154 4142 4153 455f 4558 5452 41da 1444  ATABASE_EXTRA..D
+000004f0: 4154 4142 4153 455f 434f 4e4e 4543 5449  ATABASE_CONNECTI
+00000500: 4f4e 53da 0d44 4154 4142 4153 455f 4f4e  ONS..DATABASE_ON
+00000510: 4c59 da0f 4441 5441 4241 5345 5f45 5843  LY..DATABASE_EXC
+00000520: 4550 54da 1344 4154 4142 4153 455f 4d41  EPT..DATABASE_MA
+00000530: 585f 5441 424c 4553 da0f 4441 5441 4241  X_TABLES..DATABA
+00000540: 5345 5f53 4348 454d 41da 0f44 4154 4142  SE_SCHEMA..DATAB
+00000550: 4153 455f 5353 4c5f 4341 da11 4441 5441  ASE_SSL_CA..DATA
+00000560: 4241 5345 5f53 534c 5f43 4552 54da 1044  BASE_SSL_CERT..D
+00000570: 4154 4142 4153 455f 5353 4c5f 4b45 59da  ATABASE_SSL_KEY.
+00000580: 1144 4154 4142 4153 455f 5353 485f 484f  .DATABASE_SSH_HO
+00000590: 5354 da11 4441 5441 4241 5345 5f53 5348  ST..DATABASE_SSH
+000005a0: 5f50 4f52 54da 1144 4154 4142 4153 455f  _PORT..DATABASE_
+000005b0: 5353 485f 5553 4552 da18 4441 5441 4241  SSH_USER..DATABA
+000005c0: 5345 5f53 5348 5f50 5249 5641 5445 5f4b  SE_SSH_PRIVATE_K
+000005d0: 4559 da0f 434f 4f4b 4945 5f53 414d 4553  EY..COOKIE_SAMES
+000005e0: 4954 45da 0d43 4f4f 4b49 455f 5345 4355  ITE..COOKIE_SECU
+000005f0: 5245 da0d 434f 4f4b 4945 5f44 4f4d 4149  RE..COOKIE_DOMAI
+00000600: 4eda 0f43 4f4f 4b49 455f 434f 4d50 5245  N..COOKIE_COMPRE
+00000610: 5353 da0a 5354 4f52 455f 5041 5448 da10  SS..STORE_PATH..
+00000620: 5353 4f5f 4150 504c 4943 4154 494f 4e53  SSO_APPLICATIONS
+00000630: da0c 414c 4c4f 575f 4f52 4947 494e da0f  ..ALLOW_ORIGIN..
+00000640: 5452 4143 4b5f 4441 5441 4241 5345 53da  TRACK_DATABASES.
+00000650: 1854 5241 434b 5f44 4154 4142 4153 4553  .TRACK_DATABASES
+00000660: 5f45 4e44 504f 494e 54da 1454 5241 434b  _ENDPOINT..TRACK
+00000670: 5f44 4154 4142 4153 4553 5f41 5554 48da  _DATABASES_AUTH.
+00000680: 1554 5241 434b 5f4d 4f44 454c 535f 454e  .TRACK_MODELS_EN
+00000690: 4450 4f49 4e54 da11 5452 4143 4b5f 4d4f  DPOINT..TRACK_MO
+000006a0: 4445 4c53 5f41 5554 48da 0c44 4953 4142  DELS_AUTH..DISAB
+000006b0: 4c45 5f41 5554 4829 2f72 0400 0000 720f  LE_AUTH)/r....r.
+000006c0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+000006d0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
+000006e0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+000006f0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000700: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
+00000710: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00000720: 0000 5a0b 434f 4e4e 4543 5449 4f4e 5372  ..Z.CONNECTIONSr
+00000730: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+00000740: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00000750: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00000760: 0072 2e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+00000770: 7231 0000 0072 3200 0000 7233 0000 00da  r1...r2...r3....
+00000780: 1663 6c65 616e 5f73 736f 5f61 7070 6c69  .clean_sso_appli
+00000790: 6361 7469 6f6e 7372 3400 0000 7235 0000  cationsr4...r5..
+000007a0: 0072 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
+000007b0: 7239 0000 0072 3a00 0000 723b 0000 0029  r9...r:...r;...)
+000007c0: 0172 0b00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+000007d0: 720c 0000 00da 0c67 6574 5f73 6574 7469  r......get_setti
+000007e0: 6e67 7315 0000 0073 5a00 0000 0002 0401  ngs....sZ.......
+000007f0: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000800: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000810: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000820: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000830: 0401 0401 0401 0401 0a01 0401 0401 0401  ................
+00000840: 0401 0401 0401 7a23 4a65 7442 7269 6467  ......z#JetBridg
+00000850: 6543 6f6e 6669 6775 7261 7469 6f6e 2e67  eConfiguration.g
+00000860: 6574 5f73 6574 7469 6e67 7363 0200 0000  et_settingsc....
+00000870: 0000 0000 0600 0000 0600 0000 4300 0000  ............C...
+00000880: 735e 0000 0074 006a 016a 027c 0183 015c  s^...t.j.j.|...\
+00000890: 027d 027d 0374 006a 016a 037c 0383 015c  .}.}.t.j.j.|...\
+000008a0: 027d 047d 0578 3874 006a 016a 0474 006a  .}.}.x8t.j.j.t.j
+000008b0: 016a 0574 066a 077c 0183 0283 0172 5874  .j.t.j.|.....rXt
+000008c0: 006a 016a 057c 0264 017c 0474 0864 0283  .j.j.|.d.|.t.d..
+000008d0: 017c 0566 0316 0083 027d 0171 2257 007c  .|.f.....}.q"W.|
+000008e0: 0153 0029 034e 7a07 2573 5f25 7325 73e9  .S.).Nz.%s_%s%s.
+000008f0: 0700 0000 2909 da02 6f73 da04 7061 7468  ....)...os..path
+00000900: da05 7370 6c69 74da 0873 706c 6974 6578  ..split..splitex
+00000910: 74da 0665 7869 7374 73da 046a 6f69 6e72  t..exists..joinr
+00000920: 0400 0000 da0a 4d45 4449 415f 524f 4f54  ......MEDIA_ROOT
+00000930: 7203 0000 0029 0672 0b00 0000 7240 0000  r....).r....r@..
+00000940: 005a 0864 6972 5f6e 616d 65da 0966 696c  .Z.dir_name..fil
+00000950: 655f 6e61 6d65 5a09 6669 6c65 5f72 6f6f  e_nameZ.file_roo
+00000960: 745a 0866 696c 655f 6578 7472 0a00 0000  tZ.file_extr....
+00000970: 720a 0000 0072 0c00 0000 da18 6d65 6469  r....r......medi
+00000980: 615f 6765 745f 6176 6169 6c61 626c 655f  a_get_available_
+00000990: 6e61 6d65 4600 0000 730a 0000 0000 0110  nameF...s.......
+000009a0: 0110 021a 0120 027a 2f4a 6574 4272 6964  ..... .z/JetBrid
+000009b0: 6765 436f 6e66 6967 7572 6174 696f 6e2e  geConfiguration.
+000009c0: 6d65 6469 615f 6765 745f 6176 6169 6c61  media_get_availa
+000009d0: 626c 655f 6e61 6d65 6302 0000 0000 0000  ble_namec.......
+000009e0: 0003 0000 0003 0000 0043 0000 0073 1c00  .........C...s..
+000009f0: 0000 7400 6a01 6a02 7403 6a04 7c01 8302  ..t.j.j.t.j.|...
+00000a00: 7d02 7400 6a01 6a05 7c02 8301 5300 2901  }.t.j.j.|...S.).
+00000a10: 4e29 0672 3f00 0000 7240 0000 0072 4400  N).r?...r@...rD.
+00000a20: 0000 7204 0000 0072 4500 0000 7243 0000  ..r....rE...rC..
+00000a30: 0029 0372 0b00 0000 7240 0000 00da 0d61  .).r....r@.....a
+00000a40: 6273 6f6c 7574 655f 7061 7468 720a 0000  bsolute_pathr...
+00000a50: 0072 0a00 0000 720c 0000 00da 0c6d 6564  .r....r......med
+00000a60: 6961 5f65 7869 7374 734f 0000 0073 0400  ia_existsO...s..
+00000a70: 0000 0001 1001 7a23 4a65 7442 7269 6467  ......z#JetBridg
+00000a80: 6543 6f6e 6669 6775 7261 7469 6f6e 2e6d  eConfiguration.m
+00000a90: 6564 6961 5f65 7869 7374 7363 0200 0000  edia_existsc....
+00000aa0: 0000 0000 0800 0000 0400 0000 4300 0000  ............C...
+00000ab0: 734e 0000 0074 006a 016a 0274 036a 047c  sN...t.j.j.t.j.|
+00000ac0: 0183 027d 0267 007d 0367 007d 0478 2c74  ...}.g.}.g.}.x,t
+00000ad0: 006a 057c 0283 0144 005d 1e5c 037d 057d  .j.|...D.].\.}.}
+00000ae0: 067d 077c 036a 067c 0683 0101 007c 046a  .}.|.j.|.....|.j
+00000af0: 067c 0783 0101 0071 2457 007c 037c 0466  .|.....q$W.|.|.f
+00000b00: 0253 0029 014e 2907 723f 0000 0072 4000  .S.).N).r?...r@.
+00000b10: 0000 7244 0000 0072 0400 0000 7245 0000  ..rD...r....rE..
+00000b20: 00da 0477 616c 6bda 0665 7874 656e 6429  ...walk..extend)
+00000b30: 0872 0b00 0000 7240 0000 0072 4800 0000  .r....r@...rH...
+00000b40: 5a0b 6469 7265 6374 6f72 6965 73da 0566  Z.directories..f
+00000b50: 696c 6573 da07 6469 7270 6174 68da 0864  iles..dirpath..d
+00000b60: 6972 6e61 6d65 73da 0966 696c 656e 616d  irnames..filenam
+00000b70: 6573 720a 0000 0072 0a00 0000 720c 0000  esr....r....r...
+00000b80: 00da 0d6d 6564 6961 5f6c 6973 7464 6972  ...media_listdir
+00000b90: 5300 0000 730e 0000 0000 0110 0104 0104  S...s...........
+00000ba0: 0216 010a 010e 027a 244a 6574 4272 6964  .......z$JetBrid
+00000bb0: 6765 436f 6e66 6967 7572 6174 696f 6e2e  geConfiguration.
+00000bc0: 6d65 6469 615f 6c69 7374 6469 7263 0200  media_listdirc..
+00000bd0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00000be0: 0000 731c 0000 0074 006a 016a 0274 036a  ..s....t.j.j.t.j
+00000bf0: 047c 0183 027d 0274 006a 016a 057c 0283  .|...}.t.j.j.|..
+00000c00: 0153 0029 014e 2906 723f 0000 0072 4000  .S.).N).r?...r@.
+00000c10: 0000 7244 0000 0072 0400 0000 7245 0000  ..rD...r....rE..
+00000c20: 00da 0867 6574 6d74 696d 6529 0372 0b00  ...getmtime).r..
+00000c30: 0000 7240 0000 0072 4800 0000 720a 0000  ..r@...rH...r...
+00000c40: 0072 0a00 0000 720c 0000 00da 176d 6564  .r....r......med
+00000c50: 6961 5f67 6574 5f6d 6f64 6966 6965 645f  ia_get_modified_
+00000c60: 7469 6d65 5e00 0000 7304 0000 0000 0110  time^...s.......
+00000c70: 017a 2e4a 6574 4272 6964 6765 436f 6e66  .z.JetBridgeConf
+00000c80: 6967 7572 6174 696f 6e2e 6d65 6469 615f  iguration.media_
+00000c90: 6765 745f 6d6f 6469 6669 6564 5f74 696d  get_modified_tim
+00000ca0: 6563 0200 0000 0000 0000 0300 0000 0300  ec..............
+00000cb0: 0000 4300 0000 731c 0000 0074 006a 016a  ..C...s....t.j.j
+00000cc0: 0274 036a 047c 0183 027d 0274 006a 016a  .t.j.|...}.t.j.j
+00000cd0: 057c 0283 0153 0029 014e 2906 723f 0000  .|...S.).N).r?..
+00000ce0: 0072 4000 0000 7244 0000 0072 0400 0000  .r@...rD...r....
+00000cf0: 7245 0000 00da 0767 6574 7369 7a65 2903  rE.....getsize).
+00000d00: 720b 0000 0072 4000 0000 7248 0000 0072  r....r@...rH...r
 00000d10: 0a00 0000 720a 0000 0072 0c00 0000 da0a  ....r....r......
-00000d20: 6d65 6469 615f 6f70 656e 6100 0000 7302  media_opena...s.
-00000d30: 0000 0000 017a 214a 6574 4272 6964 6765  .....z!JetBridge
-00000d40: 436f 6e66 6967 7572 6174 696f 6e2e 6d65  Configuration.me
-00000d50: 6469 615f 6f70 656e 6303 0000 0000 0000  dia_openc.......
-00000d60: 0005 0000 0011 0000 0043 0000 0073 7400  .........C...st.
-00000d70: 0000 7400 6a01 6a02 7403 6a04 7c01 8302  ..t.j.j.t.j.|...
-00000d80: 7d03 7400 6a01 6a05 7400 6a01 6a06 7c03  }.t.j.j.t.j.j.|.
-00000d90: 8301 8301 7350 7916 7400 6a07 7400 6a01  ....sPy.t.j.t.j.
-00000da0: 6a06 7c03 8301 8301 0100 5700 6e14 0400  j.|.......W.n...
-00000db0: 7408 6b0a 724e 0100 0100 0100 5900 6e02  t.k.rN......Y.n.
-00000dc0: 5800 7409 7c03 6401 8302 8f10 7d04 7c04  X.t.|.d.....}.|.
-00000dd0: 6a0a 7c02 8301 0100 5700 6400 5100 5200  j.|.....W.d.Q.R.
-00000de0: 5800 7c01 5300 2902 4eda 0277 6229 0b72  X.|.S.).N..wb).r
-00000df0: 3a00 0000 723b 0000 0072 3f00 0000 7204  :...r;...r?...r.
-00000e00: 0000 0072 4000 0000 723e 0000 00da 0764  ...r@...r>.....d
-00000e10: 6972 6e61 6d65 da08 6d61 6b65 6469 7273  irname..makedirs
-00000e20: da07 4f53 4572 726f 7272 5100 0000 da05  ..OSErrorrQ.....
-00000e30: 7772 6974 6529 0572 0b00 0000 723b 0000  write).r....r;..
-00000e40: 00da 0763 6f6e 7465 6e74 7243 0000 00da  ...contentrC....
-00000e50: 0166 720a 0000 0072 0a00 0000 720c 0000  .fr....r....r...
-00000e60: 00da 0a6d 6564 6961 5f73 6176 6564 0000  ...media_saved..
-00000e70: 0073 1200 0000 0001 1002 1401 0201 1601  .s..............
-00000e80: 0e01 0602 0c01 1402 7a21 4a65 7442 7269  ........z!JetBri
-00000e90: 6467 6543 6f6e 6669 6775 7261 7469 6f6e  dgeConfiguration
-00000ea0: 2e6d 6564 6961 5f73 6176 6563 0200 0000  .media_savec....
-00000eb0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00000ec0: 731e 0000 0074 006a 016a 0274 036a 047c  s....t.j.j.t.j.|
-00000ed0: 0183 027d 0274 006a 057c 0283 0101 0064  ...}.t.j.|.....d
-00000ee0: 0053 0029 014e 2906 723a 0000 0072 3b00  .S.).N).r:...r;.
-00000ef0: 0000 723f 0000 0072 0400 0000 7240 0000  ..r?...r....r@..
-00000f00: 00da 0672 656d 6f76 6529 0372 0b00 0000  ...remove).r....
-00000f10: 723b 0000 0072 4300 0000 720a 0000 0072  r;...rC...r....r
-00000f20: 0a00 0000 720c 0000 00da 0c6d 6564 6961  ....r......media
-00000f30: 5f64 656c 6574 6572 0000 0073 0400 0000  _deleter...s....
-00000f40: 0001 1001 7a23 4a65 7442 7269 6467 6543  ....z#JetBridgeC
-00000f50: 6f6e 6669 6775 7261 7469 6f6e 2e6d 6564  onfiguration.med
-00000f60: 6961 5f64 656c 6574 6563 0300 0000 0000  ia_deletec......
-00000f70: 0000 0400 0000 0300 0000 4300 0000 7332  ..........C...s2
-00000f80: 0000 0074 006a 0172 1664 016a 0274 006a  ...t.j.r.d.j.t.j
-00000f90: 017c 0183 027d 036e 187c 026a 0364 0217  .|...}.n.|.j.d..
-00000fa0: 007c 026a 0417 0064 0317 007c 0117 007d  .|.j...d...|...}
-00000fb0: 037c 0353 0029 044e 7a04 7b7d 7b7d 7a03  .|.S.).Nz.{}{}z.
-00000fc0: 3a2f 2f7a 072f 6d65 6469 612f 2905 7204  ://z./media/).r.
-00000fd0: 0000 005a 0e4d 4544 4941 5f42 4153 455f  ...Z.MEDIA_BASE_
-00000fe0: 5552 4cda 0666 6f72 6d61 74da 0870 726f  URL..format..pro
-00000ff0: 746f 636f 6cda 0468 6f73 7429 0472 0b00  tocol..host).r..
-00001000: 0000 723b 0000 00da 0772 6571 7565 7374  ..r;.....request
-00001010: da03 7572 6c72 0a00 0000 720a 0000 0072  ..urlr....r....r
-00001020: 0c00 0000 da09 6d65 6469 615f 7572 6c76  ......media_urlv
-00001030: 0000 0073 0800 0000 0001 0601 1002 1802  ...s............
-00001040: 7a20 4a65 7442 7269 6467 6543 6f6e 6669  z JetBridgeConfi
-00001050: 6775 7261 7469 6f6e 2e6d 6564 6961 5f75  guration.media_u
-00001060: 726c 4e54 6306 0000 0000 0000 0007 0000  rlNTc...........
-00001070: 0002 0000 0043 0000 0073 4200 0000 7c05  .....C...sB...|.
-00001080: 7212 7c01 6a00 6a01 7c02 8301 7d06 6e0c  r.|.j.j.|...}.n.
-00001090: 7c01 6a00 6a02 7c02 8301 7d06 7c06 6400  |.j.j.|...}.|.d.
-000010a0: 6b08 722a 7c03 5300 7c04 723a 7c05 723a  k.r*|.S.|.r:|.r:
-000010b0: 7c06 6a03 8300 5300 7c06 5300 6400 5300  |.j...S.|.S.d.S.
-000010c0: 2901 4e29 04da 106f 7269 6769 6e61 6c5f  ).N)...original_
-000010d0: 6861 6e64 6c65 725a 1167 6574 5f73 6563  handlerZ.get_sec
-000010e0: 7572 655f 636f 6f6b 6965 5a0a 6765 745f  ure_cookieZ.get_
-000010f0: 636f 6f6b 6965 da06 6465 636f 6465 2907  cookie..decode).
-00001100: 720b 0000 0072 6100 0000 da04 6e61 6d65  r....ra.....name
-00001110: da07 6465 6661 756c 7472 6500 0000 da06  ..defaultre.....
-00001120: 7365 6375 7265 da05 7661 6c75 6572 0a00  secure..valuer..
-00001130: 0000 720a 0000 0072 0c00 0000 da0b 7365  ..r....r......se
-00001140: 7373 696f 6e5f 6765 747e 0000 0073 1000  ssion_get~...s..
-00001150: 0000 0001 0401 0e02 0c02 0801 0401 0801  ................
-00001160: 0802 7a22 4a65 7442 7269 6467 6543 6f6e  ..z"JetBridgeCon
-00001170: 6669 6775 7261 7469 6f6e 2e73 6573 7369  figuration.sessi
-00001180: 6f6e 5f67 6574 6305 0000 0000 0000 0005  on_getc.........
-00001190: 0000 0007 0000 0043 0000 0073 5800 0000  .......C...sX...
-000011a0: 7c03 6400 6b08 7216 7c00 6a00 7c01 7c02  |.d.k.r.|.j.|.|.
-000011b0: 8302 0100 6e3e 7c04 7238 7c01 6a01 6a02  ....n>|.r8|.j.j.
-000011c0: 7c02 7c03 7403 6a04 7403 6a05 7403 6a06  |.|.t.j.t.j.t.j.
-000011d0: 6401 8d05 0100 6e1c 7c01 6a01 6a07 7c02  d.....n.|.j.j.|.
-000011e0: 7c03 7403 6a04 7403 6a05 7403 6a06 6401  |.t.j.t.j.t.j.d.
-000011f0: 8d05 0100 6400 5300 2902 4e29 0372 0700  ....d.S.).N).r..
-00001200: 0000 7268 0000 00da 0664 6f6d 6169 6e29  ..rh.....domain)
-00001210: 08da 0d73 6573 7369 6f6e 5f63 6c65 6172  ...session_clear
-00001220: 7264 0000 005a 1173 6574 5f73 6563 7572  rd...Z.set_secur
-00001230: 655f 636f 6f6b 6965 7204 0000 0072 2b00  e_cookier....r+.
-00001240: 0000 722c 0000 0072 2d00 0000 5a0a 7365  ..r,...r-...Z.se
-00001250: 745f 636f 6f6b 6965 2905 720b 0000 0072  t_cookie).r....r
-00001260: 6100 0000 7266 0000 0072 6900 0000 7268  a...rf...ri...rh
-00001270: 0000 0072 0a00 0000 720a 0000 0072 0c00  ...r....r....r..
-00001280: 0000 da0b 7365 7373 696f 6e5f 7365 748b  ....session_set.
-00001290: 0000 0073 1e00 0000 0001 0801 0e01 0401  ...s............
-000012a0: 0601 0201 0201 0401 0401 0c03 0601 0201  ................
-000012b0: 0201 0401 0401 7a22 4a65 7442 7269 6467  ......z"JetBridg
-000012c0: 6543 6f6e 6669 6775 7261 7469 6f6e 2e73  eConfiguration.s
-000012d0: 6573 7369 6f6e 5f73 6574 6303 0000 0000  ession_setc.....
-000012e0: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
-000012f0: 1000 0000 7c01 6a00 6a01 7c02 8301 0100  ....|.j.j.|.....
-00001300: 6400 5300 2901 4e29 0272 6400 0000 5a0c  d.S.).N).rd...Z.
-00001310: 636c 6561 725f 636f 6f6b 6965 2903 720b  clear_cookie).r.
-00001320: 0000 0072 6100 0000 7266 0000 0072 0a00  ...ra...rf...r..
-00001330: 0000 720a 0000 0072 0c00 0000 726c 0000  ..r....r....rl..
-00001340: 009f 0000 0073 0200 0000 0001 7a24 4a65  .....s......z$Je
-00001350: 7442 7269 6467 6543 6f6e 6669 6775 7261  tBridgeConfigura
-00001360: 7469 6f6e 2e73 6573 7369 6f6e 5f63 6c65  tion.session_cle
-00001370: 6172 2901 7250 0000 0029 034e 5454 2901  ar).rP...).NTT).
-00001380: 5429 12da 085f 5f6e 616d 655f 5fda 0a5f  T)...__name__.._
-00001390: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000013a0: 6c6e 616d 655f 5f72 0d00 0000 720e 0000  lname__r....r...
-000013b0: 0072 3800 0000 7242 0000 0072 4400 0000  .r8...rB...rD...
-000013c0: 724b 0000 0072 4d00 0000 724f 0000 0072  rK...rM...rO...r
-000013d0: 5300 0000 725b 0000 0072 5d00 0000 7263  S...r[...r]...rc
-000013e0: 0000 0072 6a00 0000 726d 0000 0072 6c00  ...rj...rm...rl.
-000013f0: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00001400: 0072 0c00 0000 7208 0000 000d 0000 0073  .r....r........s
-00001410: 1e00 0000 0802 0803 0803 082c 0809 0804  ...........,....
-00001420: 080b 0804 0804 0a03 080e 0804 0808 0a0d  ................
-00001430: 0a14 7208 0000 0029 0d72 3a00 0000 5a1d  ..r....).r:...Z.
-00001440: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00001450: 636f 6e66 6967 7572 6174 696f 6e72 0200  configurationr..
-00001460: 0000 5a1c 6a65 745f 6272 6964 6765 5f62  ..Z.jet_bridge_b
-00001470: 6173 652e 7574 696c 732e 636f 6d6d 6f6e  ase.utils.common
-00001480: 7203 0000 0072 0900 0000 7204 0000 0072  r....r....r....r
-00001490: 0500 0000 5a16 7369 782e 6d6f 7665 732e  ....Z.six.moves.
-000014a0: 6874 7470 5f63 6f6f 6b69 6573 7206 0000  http_cookiesr...
-000014b0: 00da 0373 7472 da09 5f72 6573 6572 7665  ...str.._reserve
-000014c0: 6472 0800 0000 720a 0000 0072 0a00 0000  dr....r....r....
-000014d0: 720a 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
-000014e0: 756c 653e 0100 0000 730c 0000 0008 020c  ule>....s.......
-000014f0: 010c 0210 020c 0212 03                   .........
+00000d20: 6d65 6469 615f 7369 7a65 6200 0000 7304  media_sizeb...s.
+00000d30: 0000 0000 0110 017a 214a 6574 4272 6964  .......z!JetBrid
+00000d40: 6765 436f 6e66 6967 7572 6174 696f 6e2e  geConfiguration.
+00000d50: 6d65 6469 615f 7369 7a65 da02 7262 6303  media_size..rbc.
+00000d60: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+00000d70: 0000 0073 0a00 0000 7400 7c01 7c02 8302  ...s....t.|.|...
+00000d80: 5300 2901 4e29 01da 046f 7065 6e29 0372  S.).N)...open).r
+00000d90: 0b00 0000 7240 0000 00da 046d 6f64 6572  ....r@.....moder
+00000da0: 0a00 0000 720a 0000 0072 0c00 0000 da0a  ....r....r......
+00000db0: 6d65 6469 615f 6f70 656e 6600 0000 7302  media_openf...s.
+00000dc0: 0000 0000 017a 214a 6574 4272 6964 6765  .....z!JetBridge
+00000dd0: 436f 6e66 6967 7572 6174 696f 6e2e 6d65  Configuration.me
+00000de0: 6469 615f 6f70 656e 6303 0000 0000 0000  dia_openc.......
+00000df0: 0005 0000 0011 0000 0043 0000 0073 7400  .........C...st.
+00000e00: 0000 7400 6a01 6a02 7403 6a04 7c01 8302  ..t.j.j.t.j.|...
+00000e10: 7d03 7400 6a01 6a05 7400 6a01 6a06 7c03  }.t.j.j.t.j.j.|.
+00000e20: 8301 8301 7350 7916 7400 6a07 7400 6a01  ....sPy.t.j.t.j.
+00000e30: 6a06 7c03 8301 8301 0100 5700 6e14 0400  j.|.......W.n...
+00000e40: 7408 6b0a 724e 0100 0100 0100 5900 6e02  t.k.rN......Y.n.
+00000e50: 5800 7409 7c03 6401 8302 8f10 7d04 7c04  X.t.|.d.....}.|.
+00000e60: 6a0a 7c02 8301 0100 5700 6400 5100 5200  j.|.....W.d.Q.R.
+00000e70: 5800 7c01 5300 2902 4eda 0277 6229 0b72  X.|.S.).N..wb).r
+00000e80: 3f00 0000 7240 0000 0072 4400 0000 7204  ?...r@...rD...r.
+00000e90: 0000 0072 4500 0000 7243 0000 00da 0764  ...rE...rC.....d
+00000ea0: 6972 6e61 6d65 da08 6d61 6b65 6469 7273  irname..makedirs
+00000eb0: da07 4f53 4572 726f 7272 5600 0000 da05  ..OSErrorrV.....
+00000ec0: 7772 6974 6529 0572 0b00 0000 7240 0000  write).r....r@..
+00000ed0: 00da 0763 6f6e 7465 6e74 7248 0000 00da  ...contentrH....
+00000ee0: 0166 720a 0000 0072 0a00 0000 720c 0000  .fr....r....r...
+00000ef0: 00da 0a6d 6564 6961 5f73 6176 6569 0000  ...media_savei..
+00000f00: 0073 1200 0000 0001 1002 1401 0201 1601  .s..............
+00000f10: 0e01 0602 0c01 1402 7a21 4a65 7442 7269  ........z!JetBri
+00000f20: 6467 6543 6f6e 6669 6775 7261 7469 6f6e  dgeConfiguration
+00000f30: 2e6d 6564 6961 5f73 6176 6563 0200 0000  .media_savec....
+00000f40: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+00000f50: 731e 0000 0074 006a 016a 0274 036a 047c  s....t.j.j.t.j.|
+00000f60: 0183 027d 0274 006a 057c 0283 0101 0064  ...}.t.j.|.....d
+00000f70: 0053 0029 014e 2906 723f 0000 0072 4000  .S.).N).r?...r@.
+00000f80: 0000 7244 0000 0072 0400 0000 7245 0000  ..rD...r....rE..
+00000f90: 00da 0672 656d 6f76 6529 0372 0b00 0000  ...remove).r....
+00000fa0: 7240 0000 0072 4800 0000 720a 0000 0072  r@...rH...r....r
+00000fb0: 0a00 0000 720c 0000 00da 0c6d 6564 6961  ....r......media
+00000fc0: 5f64 656c 6574 6577 0000 0073 0400 0000  _deletew...s....
+00000fd0: 0001 1001 7a23 4a65 7442 7269 6467 6543  ....z#JetBridgeC
+00000fe0: 6f6e 6669 6775 7261 7469 6f6e 2e6d 6564  onfiguration.med
+00000ff0: 6961 5f64 656c 6574 6563 0300 0000 0000  ia_deletec......
+00001000: 0000 0400 0000 0300 0000 4300 0000 7332  ..........C...s2
+00001010: 0000 0074 006a 0172 1664 016a 0274 006a  ...t.j.r.d.j.t.j
+00001020: 017c 0183 027d 036e 187c 026a 0364 0217  .|...}.n.|.j.d..
+00001030: 007c 026a 0417 0064 0317 007c 0117 007d  .|.j...d...|...}
+00001040: 037c 0353 0029 044e 7a04 7b7d 7b7d 7a03  .|.S.).Nz.{}{}z.
+00001050: 3a2f 2f7a 072f 6d65 6469 612f 2905 7204  ://z./media/).r.
+00001060: 0000 005a 0e4d 4544 4941 5f42 4153 455f  ...Z.MEDIA_BASE_
+00001070: 5552 4cda 0666 6f72 6d61 74da 0870 726f  URL..format..pro
+00001080: 746f 636f 6cda 0468 6f73 7429 0472 0b00  tocol..host).r..
+00001090: 0000 7240 0000 00da 0772 6571 7565 7374  ..r@.....request
+000010a0: da03 7572 6c72 0a00 0000 720a 0000 0072  ..urlr....r....r
+000010b0: 0c00 0000 da09 6d65 6469 615f 7572 6c7b  ......media_url{
+000010c0: 0000 0073 0800 0000 0001 0601 1002 1802  ...s............
+000010d0: 7a20 4a65 7442 7269 6467 6543 6f6e 6669  z JetBridgeConfi
+000010e0: 6775 7261 7469 6f6e 2e6d 6564 6961 5f75  guration.media_u
+000010f0: 726c 4e54 6306 0000 0000 0000 0007 0000  rlNTc...........
+00001100: 0002 0000 0043 0000 0073 4200 0000 7c05  .....C...sB...|.
+00001110: 7212 7c01 6a00 6a01 7c02 8301 7d06 6e0c  r.|.j.j.|...}.n.
+00001120: 7c01 6a00 6a02 7c02 8301 7d06 7c06 6400  |.j.j.|...}.|.d.
+00001130: 6b08 722a 7c03 5300 7c04 723a 7c05 723a  k.r*|.S.|.r:|.r:
+00001140: 7c06 6a03 8300 5300 7c06 5300 6400 5300  |.j...S.|.S.d.S.
+00001150: 2901 4e29 04da 106f 7269 6769 6e61 6c5f  ).N)...original_
+00001160: 6861 6e64 6c65 725a 1167 6574 5f73 6563  handlerZ.get_sec
+00001170: 7572 655f 636f 6f6b 6965 5a0a 6765 745f  ure_cookieZ.get_
+00001180: 636f 6f6b 6965 da06 6465 636f 6465 2907  cookie..decode).
+00001190: 720b 0000 0072 6600 0000 da04 6e61 6d65  r....rf.....name
+000011a0: da07 6465 6661 756c 7472 6a00 0000 da06  ..defaultrj.....
+000011b0: 7365 6375 7265 da05 7661 6c75 6572 0a00  secure..valuer..
+000011c0: 0000 720a 0000 0072 0c00 0000 da0b 7365  ..r....r......se
+000011d0: 7373 696f 6e5f 6765 7483 0000 0073 1000  ssion_get....s..
+000011e0: 0000 0001 0401 0e02 0c02 0801 0401 0801  ................
+000011f0: 0802 7a22 4a65 7442 7269 6467 6543 6f6e  ..z"JetBridgeCon
+00001200: 6669 6775 7261 7469 6f6e 2e73 6573 7369  figuration.sessi
+00001210: 6f6e 5f67 6574 6305 0000 0000 0000 0005  on_getc.........
+00001220: 0000 0007 0000 0043 0000 0073 5800 0000  .......C...sX...
+00001230: 7c03 6400 6b08 7216 7c00 6a00 7c01 7c02  |.d.k.r.|.j.|.|.
+00001240: 8302 0100 6e3e 7c04 7238 7c01 6a01 6a02  ....n>|.r8|.j.j.
+00001250: 7c02 7c03 7403 6a04 7403 6a05 7403 6a06  |.|.t.j.t.j.t.j.
+00001260: 6401 8d05 0100 6e1c 7c01 6a01 6a07 7c02  d.....n.|.j.j.|.
+00001270: 7c03 7403 6a04 7403 6a05 7403 6a06 6401  |.t.j.t.j.t.j.d.
+00001280: 8d05 0100 6400 5300 2902 4e29 0372 0700  ....d.S.).N).r..
+00001290: 0000 726d 0000 00da 0664 6f6d 6169 6e29  ..rm.....domain)
+000012a0: 08da 0d73 6573 7369 6f6e 5f63 6c65 6172  ...session_clear
+000012b0: 7269 0000 005a 1173 6574 5f73 6563 7572  ri...Z.set_secur
+000012c0: 655f 636f 6f6b 6965 7204 0000 0072 2f00  e_cookier....r/.
+000012d0: 0000 7230 0000 0072 3100 0000 5a0a 7365  ..r0...r1...Z.se
+000012e0: 745f 636f 6f6b 6965 2905 720b 0000 0072  t_cookie).r....r
+000012f0: 6600 0000 726b 0000 0072 6e00 0000 726d  f...rk...rn...rm
+00001300: 0000 0072 0a00 0000 720a 0000 0072 0c00  ...r....r....r..
+00001310: 0000 da0b 7365 7373 696f 6e5f 7365 7490  ....session_set.
+00001320: 0000 0073 1e00 0000 0001 0801 0e01 0401  ...s............
+00001330: 0601 0201 0201 0401 0401 0c03 0601 0201  ................
+00001340: 0201 0401 0401 7a22 4a65 7442 7269 6467  ......z"JetBridg
+00001350: 6543 6f6e 6669 6775 7261 7469 6f6e 2e73  eConfiguration.s
+00001360: 6573 7369 6f6e 5f73 6574 6303 0000 0000  ession_setc.....
+00001370: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
+00001380: 1000 0000 7c01 6a00 6a01 7c02 8301 0100  ....|.j.j.|.....
+00001390: 6400 5300 2901 4e29 0272 6900 0000 5a0c  d.S.).N).ri...Z.
+000013a0: 636c 6561 725f 636f 6f6b 6965 2903 720b  clear_cookie).r.
+000013b0: 0000 0072 6600 0000 726b 0000 0072 0a00  ...rf...rk...r..
+000013c0: 0000 720a 0000 0072 0c00 0000 7271 0000  ..r....r....rq..
+000013d0: 00a4 0000 0073 0200 0000 0001 7a24 4a65  .....s......z$Je
+000013e0: 7442 7269 6467 6543 6f6e 6669 6775 7261  tBridgeConfigura
+000013f0: 7469 6f6e 2e73 6573 7369 6f6e 5f63 6c65  tion.session_cle
+00001400: 6172 2901 7255 0000 0029 034e 5454 2901  ar).rU...).NTT).
+00001410: 5429 12da 085f 5f6e 616d 655f 5fda 0a5f  T)...__name__.._
+00001420: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001430: 6c6e 616d 655f 5f72 0d00 0000 720e 0000  lname__r....r...
+00001440: 0072 3d00 0000 7247 0000 0072 4900 0000  .r=...rG...rI...
+00001450: 7250 0000 0072 5200 0000 7254 0000 0072  rP...rR...rT...r
+00001460: 5800 0000 7260 0000 0072 6200 0000 7268  X...r`...rb...rh
+00001470: 0000 0072 6f00 0000 7272 0000 0072 7100  ...ro...rr...rq.
+00001480: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00001490: 0072 0c00 0000 7208 0000 000d 0000 0073  .r....r........s
+000014a0: 1e00 0000 0802 0803 0803 0831 0809 0804  ...........1....
+000014b0: 080b 0804 0804 0a03 080e 0804 0808 0a0d  ................
+000014c0: 0a14 7208 0000 0029 0d72 3f00 0000 5a1d  ..r....).r?...Z.
+000014d0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+000014e0: 636f 6e66 6967 7572 6174 696f 6e72 0200  configurationr..
+000014f0: 0000 5a1c 6a65 745f 6272 6964 6765 5f62  ..Z.jet_bridge_b
+00001500: 6173 652e 7574 696c 732e 636f 6d6d 6f6e  ase.utils.common
+00001510: 7203 0000 0072 0900 0000 7204 0000 0072  r....r....r....r
+00001520: 0500 0000 5a16 7369 782e 6d6f 7665 732e  ....Z.six.moves.
+00001530: 6874 7470 5f63 6f6f 6b69 6573 7206 0000  http_cookiesr...
+00001540: 00da 0373 7472 da09 5f72 6573 6572 7665  ...str.._reserve
+00001550: 6472 0800 0000 720a 0000 0072 0a00 0000  dr....r....r....
+00001560: 720a 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+00001570: 756c 653e 0100 0000 730c 0000 0008 020c  ule>....s.......
+00001580: 010c 0210 020c 0212 03                   .........
```

### Comparing `jet-bridge-1.7.9/jet_bridge/settings.py` & `jet-bridge-1.8.2/jet_bridge/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # Options
 
 DEFAULT_WEB_BASE_URL = 'https://app.jetadmin.io'
 DEFAULT_API_BASE_URL = 'https://api.jetadmin.io/api'
 
 define('address', default='0.0.0.0', help='server address')
 define('port', default=8888, help='server port', type=int)
+define('ssl_cert', help='SSL certificate file path', type=str, default=None)
+define('ssl_key', help='SSL private key file path', type=str, default=None)
 define('workers', default=1, help='number of workers', type=int)
 define('config', default=DEFAULT_CONFIG_PATH, help='config file path')
 define('use_default_config', default='', help='use default config values')
 define('debug', default=False, help='debug mode', type=bool)
 define('read_only', default=False, help='read only', type=bool)
 define('threads', default=None, help='threads', type=int)
 define('connections', default=50, help='connects', type=int)
@@ -49,16 +51,21 @@
 define('database_port', help='database port')
 define('database_user', help='database user')
 define('database_password', help='database password')
 define('database_name', help='database name or path')
 define('database_extra', default=None, help='database extra parameters')
 define('database_only', default=None, type=str)
 define('database_except', default=None, type=str)
+define('database_max_tables', default=None, type=int)
 define('database_schema', default=None, type=str)
 
+define('database_ssl_ca', default=None, type=str, help='Path to "CA Certificate" file')
+define('database_ssl_cert', default=None, type=str, help='Path to "Client Certificate" file')
+define('database_ssl_key', default=None, type=str, help='Path to "Client Key" file')
+
 define('database_ssh_host', default=None, type=str)
 define('database_ssh_port', default=None, type=int)
 define('database_ssh_user', default=None, type=str)
 define('database_ssh_private_key', default=None, type=str)
 
 define('cookie_samesite', default='None', type=str)
 define('cookie_secure', default=True, type=bool)
@@ -73,14 +80,16 @@
 define('track_databases', default='')
 define('track_databases_endpoint', default='')
 define('track_databases_auth', default='')
 
 define('track_models_endpoint', default='')
 define('track_models_auth', default='')
 
+define('disable_auth', default=False, type=bool)
+
 define('sentry_dsn', default='')
 
 # Parse
 
 options.parse_command_line(final=False)
 
 if options.config:
@@ -112,14 +121,16 @@
 
 missing_options = list(filter(lambda x: x not in options or options[x] is None, required_options))
 
 # Settings
 
 ADDRESS = options.address
 PORT = options.port
+SSL_CERT = options.ssl_cert
+SSL_KEY = options.ssl_key
 WORKERS = options.workers
 DEBUG = options.debug
 READ_ONLY = options.read_only
 THREADS = options.threads
 CONNECTIONS = options.connections
 AUTO_OPEN_REGISTER = options.auto_open_register
 CONFIG = options.config
@@ -145,16 +156,21 @@
 DATABASE_PORT = options.database_port
 DATABASE_USER = options.database_user
 DATABASE_PASSWORD = options.database_password
 DATABASE_NAME = options.database_name
 DATABASE_EXTRA = options.database_extra
 DATABASE_ONLY = options.database_only.split(',') if options.database_only else None
 DATABASE_EXCEPT = options.database_except.split(',') if options.database_except else None
+DATABASE_MAX_TABLES = options.database_max_tables
 DATABASE_SCHEMA = options.database_schema
 
+DATABASE_SSL_CA = options.database_ssl_ca
+DATABASE_SSL_CERT = options.database_ssl_cert
+DATABASE_SSL_KEY = options.database_ssl_key
+
 DATABASE_SSH_HOST = options.database_ssh_host
 DATABASE_SSH_PORT = options.database_ssh_port
 DATABASE_SSH_USER = options.database_ssh_user
 DATABASE_SSH_PRIVATE_KEY = options.database_ssh_private_key
 
 COOKIE_SAMESITE = options.cookie_samesite
 COOKIE_SECURE = options.cookie_secure
@@ -174,10 +190,12 @@
 TRACK_DATABASES = options.track_databases
 TRACK_DATABASES_ENDPOINT = options.track_databases_endpoint
 TRACK_DATABASES_AUTH = options.track_databases_auth
 
 TRACK_MODELS_ENDPOINT = options.track_models_endpoint
 TRACK_MODELS_AUTH = options.track_models_auth
 
+DISABLE_AUTH = options.disable_auth
+
 SENTRY_DSN = options.sentry_dsn
 
 POSSIBLE_HOST = os.environ.get('POSSIBLE_HOST')
```

### Comparing `jet-bridge-1.7.9/jet_bridge/app.py` & `jet-bridge-1.8.2/jet_bridge/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import tornado.web
 
 from jet_bridge.handlers.temporary_redirect import TemporaryRedirectHandler
 from jet_bridge_base.sentry import sentry_controller
 from jet_bridge_base.utils.async_exec import set_max_workers
 from jet_bridge_base import settings as base_settings
 from jet_bridge_base.views.api import ApiView
+from jet_bridge_base.views.discover_connection import DiscoverConnectionView
+from jet_bridge_base.views.discover_table import DiscoverTableView
 from jet_bridge_base.views.external_auth.complete import ExternalAuthCompleteView
 from jet_bridge_base.views.external_auth.login import ExternalAuthLoginView
 from jet_bridge_base.views.graphql import GraphQLView
 from jet_bridge_base.views.image_resize import ImageResizeView
 from jet_bridge_base.views.file_upload import FileUploadView
 from jet_bridge_base.views.message import MessageView
 from jet_bridge_base.views.model import ModelViewSet
@@ -49,14 +51,16 @@
         (r'/api/model_descriptions/', view_handler(ModelDescriptionView)),
         (r'/api/sql/', view_handler(SqlView)),
         (r'/api/messages/', view_handler(MessageView)),
         (r'/api/file_upload/', view_handler(FileUploadView)),
         (r'/api/image_resize/', view_handler(ImageResizeView)),
         (r'/api/reload/', view_handler(ReloadView)),
         (r'/api/proxy_request/', view_handler(ProxyRequestView)),
+        (r'/api/discover/connection/', view_handler(DiscoverConnectionView)),
+        (r'/api/discover/tables/', view_handler(DiscoverTableView)),
         (r'/media/(.*)', tornado.web.StaticFileHandler, {'path': settings.MEDIA_ROOT}),
         (r'/api/external_auth/login/(?P<app>[^/]+)/', view_handler(ExternalAuthLoginView)),
         (r'/api/external_auth/complete/(?P<app>[^/]+)/', view_handler(ExternalAuthCompleteView)),
         (r'/api/status/', view_handler(StatusView)),
         (r'/api/trigger_exception/', view_handler(TriggerExceptionView)),
     ]
     urls += router.urls
```

### Comparing `jet-bridge-1.7.9/jet_bridge/router.py` & `jet-bridge-1.8.2/jet_bridge/router.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+
 import tornado
 from tornado import gen
 from tornado.concurrent import Future
 
 from jet_bridge_base.utils.async_exec import as_future
 
 
@@ -32,27 +34,32 @@
         class ActionHandler(view):
             pass
 
         for method, method_action in actions.items():
             def create_action_method(action):
                 @gen.coroutine
                 def action_method(inner_self, *args, **kwargs):
+                    request = inner_self.get_request()
+                    request.action = action
 
                     def execute():
-                        request = inner_self.get_request()
-                        request.action = action
                         inner_self.before_dispatch(request)
                         result = inner_self.view.dispatch(action, request, *args, **kwargs)
                         inner_self.after_dispatch(request)
                         return result
 
-                    response = yield as_future(execute)
-
-                    yield inner_self.write_response(response)
-                    raise gen.Return()
+                    try:
+                        response = yield as_future(execute)
+                        yield inner_self.write_response(response)
+                    except Exception:
+                        exc_type, exc, traceback = sys.exc_info()
+                        response = inner_self.view.error_response(request, exc_type, exc, traceback)
+                        yield inner_self.write_response(response)
+                    finally:
+                        raise gen.Return()
 
                 return action_method
 
             func = create_action_method(method_action)
             setattr(ActionHandler, method, func)
 
         self.urls.append((url, ActionHandler))
```

### Comparing `jet-bridge-1.7.9/jet_bridge/__main__.py` & `jet-bridge-1.8.2/jet_bridge/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,30 +32,38 @@
         from jet_bridge.utils.create_config import create_config
         create_config(missing_options == required_options_without_default)
         return
     elif missing_options and len(missing_options) < len(required_options_without_default):
         logger.info('Required options are not specified: {}'.format(', '.join(missing_options)))
         return
 
+    ssl = settings.SSL_CERT or settings.SSL_KEY
+
     address = 'localhost' if settings.ADDRESS == '0.0.0.0' else settings.ADDRESS
-    url = 'http://{}:{}/'.format(address, settings.PORT)
+    protocol = 'https' if ssl else 'http'
+    url = '{}://{}:{}/'.format(protocol, address, settings.PORT)
     api_url = '{}api/'.format(url)
 
     if len(args) >= 1:
         if args[0] == 'check_token':
             check_token_command(api_url)
             return
 
     connect_database_from_settings()
 
     from jet_bridge.app import make_app
 
     app = make_app()
     workers = settings.WORKERS if not settings.DEBUG else 1
-    server = HTTPServer(app)
+
+    ssl_options = {
+        'certfile': settings.SSL_CERT,
+        'keyfile': settings.SSL_KEY
+    } if ssl else None
+    server = HTTPServer(app, ssl_options=ssl_options)
     server.bind(settings.PORT, settings.ADDRESS)
     server.start(workers)
 
     if settings.WORKERS > 1 and settings.DEBUG:
         logger.warning('Multiple workers are not supported in DEBUG mode')
 
     logger.info('Starting server at {} (WORKERS: {})'.format(url, workers))
```

### Comparing `jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/view.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/view.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,357 +1,366 @@
-00000000: 330d 0d0a 76b0 eb63 2412 0000 e300 0000  3...v..c$.......
+00000000: 330d 0d0a 916f c364 2d13 0000 e300 0000  3....o.d-.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 ac00 0000 6400 6401 6c00 5a01 6400  .s....d.d.l.Z.d.
-00000030: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000040: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6405 6c01 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6406 6c09 6d0a 5a0a 0100 6400 6407 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6400 6408 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6409 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
-00000090: 640a 6c11 6d12 5a12 0100 6400 640b 6c13  d.l.m.Z...d.d.l.
-000000a0: 6d14 5a14 0100 6400 640c 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
-000000b0: 0100 4700 640d 640e 8400 640e 6501 6a17  ..G.d.d...d.e.j.
-000000c0: 6a18 8303 5a19 640f 6410 8400 5a1a 6401  j...Z.d.d...Z.d.
-000000d0: 5300 2911 e900 0000 004e 2901 da0e 6765  S.)......N)...ge
-000000e0: 745f 636f 6e6e 6563 7469 6f6e 2901 da0c  t_connection)...
-000000f0: 5265 7175 6573 7445 7272 6f72 2901 da11  RequestError)...
-00000100: 7365 6e74 7279 5f63 6f6e 7472 6f6c 6c65  sentry_controlle
-00000110: 7229 01da 0367 656e 2901 da08 7061 7273  r)...gen)...pars
-00000120: 655f 7173 2901 da07 5265 7175 6573 7429  e_qs)...Request)
-00000130: 01da 1052 6564 6972 6563 7452 6573 706f  ...RedirectRespo
-00000140: 6e73 6529 01da 1054 656d 706c 6174 6552  nse)...TemplateR
-00000150: 6573 706f 6e73 6529 01da 1348 5454 505f  esponse)...HTTP_
-00000160: 3230 345f 4e4f 5f43 4f4e 5445 4e54 2901  204_NO_CONTENT).
-00000170: da09 6173 5f66 7574 7572 6529 01da 1153  ..as_future)...S
-00000180: 7472 6561 6d43 6c6f 7365 6445 7272 6f72  treamClosedError
-00000190: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-000001a0: 0040 0000 0073 a200 0000 6500 5a01 6400  .@...s....e.Z.d.
-000001b0: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
-000001c0: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
-000001d0: 6409 8400 5a07 640a 640b 8400 5a08 640c  d...Z.d.d...Z.d.
-000001e0: 640d 8400 5a09 640e 640f 8400 5a0a 650b  d...Z.d.d...Z.e.
-000001f0: 6a0c 6410 6411 8400 8301 5a0d 650b 6a0c  j.d.d.....Z.e.j.
-00000200: 6412 6413 8400 8301 5a0e 6414 6415 8400  d.d.....Z.d.d...
-00000210: 5a0f 650b 6a0c 6416 6417 8400 8301 5a10  Z.e.j.d.d.....Z.
-00000220: 6418 6419 8400 5a11 641a 641b 8400 5a12  d.d...Z.d.d...Z.
-00000230: 641c 641d 8400 5a13 641e 641f 8400 5a14  d.d...Z.d.d...Z.
-00000240: 6420 6421 8400 5a15 6401 5300 2922 da0f  d d!..Z.d.S.)"..
-00000250: 4261 7365 5669 6577 4861 6e64 6c65 724e  BaseViewHandlerN
-00000260: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-00000270: 0043 0000 0073 1600 0000 6401 6402 8400  .C...s....d.d...
-00000280: 7c00 6a00 6a01 6a02 8300 4400 8301 5300  |.j.j.j...D...S.
-00000290: 2903 4e63 0100 0000 0000 0000 0300 0000  ).Nc............
-000002a0: 0600 0000 5300 0000 7322 0000 0069 007c  ....S...s"...i.|
-000002b0: 005d 1a5c 027d 017d 027c 027c 016a 0083  .].\.}.}.|.|.j..
-000002c0: 006a 0164 0064 0183 0293 0271 0453 0029  .j.d.d.....q.S.)
-000002d0: 02fa 012d da01 5f29 02da 0575 7070 6572  ...-.._)...upper
-000002e0: da07 7265 706c 6163 6529 03da 022e 30da  ..replace)....0.
-000002f0: 016b da01 76a9 0072 1500 0000 fa5a 2f55  .k..v..r.....Z/U
-00000300: 7365 7273 2f66 316e 616c 2f44 726f 7062  sers/f1nal/Dropb
-00000310: 6f78 2f70 7974 686f 6e2f 6a65 742d 6272  ox/python/jet-br
-00000320: 6964 6765 2f73 7263 2f70 6163 6b61 6765  idge/src/package
-00000330: 732f 6a65 745f 6272 6964 6765 2f6a 6574  s/jet_bridge/jet
-00000340: 5f62 7269 6467 652f 6861 6e64 6c65 7273  _bridge/handlers
-00000350: 2f76 6965 772e 7079 fa0a 3c64 6963 7463  /view.py..<dictc
-00000360: 6f6d 703e 1400 0000 7302 0000 0006 007a  omp>....s......z
-00000370: 3342 6173 6556 6965 7748 616e 646c 6572  3BaseViewHandler
-00000380: 2e72 6571 7565 7374 5f68 6561 6465 7273  .request_headers
-00000390: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-000003a0: 6f6d 703e 2903 da07 7265 7175 6573 74da  omp>)...request.
-000003b0: 0768 6561 6465 7273 da05 6974 656d 7329  .headers..items)
-000003c0: 01da 0473 656c 6672 1500 0000 7215 0000  ...selfr....r...
-000003d0: 0072 1600 0000 da0f 7265 7175 6573 745f  .r......request_
-000003e0: 6865 6164 6572 7313 0000 0073 0200 0000  headers....s....
-000003f0: 0001 7a1f 4261 7365 5669 6577 4861 6e64  ..z.BaseViewHand
-00000400: 6c65 722e 7265 7175 6573 745f 6865 6164  ler.request_head
-00000410: 6572 7363 0100 0000 0000 0000 0200 0000  ersc............
-00000420: 0400 0000 4300 0000 731e 0000 0064 0164  ....C...s....d.d
-00000430: 0284 007d 0174 0074 017c 017c 006a 026a  ...}.t.t.|.|.j.j
-00000440: 036a 0483 0083 0283 0153 0029 034e 6301  .j.......S.).Nc.
-00000450: 0000 0000 0000 0004 0000 0003 0000 0053  ...............S
-00000460: 0000 0073 2000 0000 7c00 5c02 7d01 7d02  ...s ...|.\.}.}.
-00000470: 7c02 6401 1900 7d03 7c01 7c03 6a00 7c03  |.d...}.|.|.j.|.
-00000480: 6a01 6602 6602 5300 2902 4e72 0100 0000  j.f.f.S.).Nr....
-00000490: 2902 da08 6669 6c65 6e61 6d65 da04 626f  )...filename..bo
-000004a0: 6479 2904 da03 6172 67da 036b 6579 da05  dy)...arg..key..
-000004b0: 6669 6c65 73da 0466 696c 6572 1500 0000  files..filer....
-000004c0: 7215 0000 0072 1600 0000 da08 6d61 705f  r....r......map_
-000004d0: 6669 6c65 1700 0000 7306 0000 0000 0108  file....s.......
-000004e0: 0108 017a 2f42 6173 6556 6965 7748 616e  ...z/BaseViewHan
-000004f0: 646c 6572 2e72 6571 7565 7374 5f66 696c  dler.request_fil
-00000500: 6573 2e3c 6c6f 6361 6c73 3e2e 6d61 705f  es.<locals>.map_
-00000510: 6669 6c65 2905 da04 6469 6374 da03 6d61  file)...dict..ma
-00000520: 7072 1800 0000 7221 0000 0072 1a00 0000  pr....r!...r....
-00000530: 2902 721b 0000 0072 2300 0000 7215 0000  ).r....r#...r...
-00000540: 0072 1500 0000 7216 0000 00da 0d72 6571  .r....r......req
-00000550: 7565 7374 5f66 696c 6573 1600 0000 7304  uest_files....s.
-00000560: 0000 0000 0108 057a 1d42 6173 6556 6965  .......z.BaseVie
-00000570: 7748 616e 646c 6572 2e72 6571 7565 7374  wHandler.request
-00000580: 5f66 696c 6573 6301 0000 0000 0000 0002  _filesc.........
-00000590: 0000 000e 0000 0043 0000 0073 5c00 0000  .......C...s\...
-000005a0: 7400 7c00 6a01 6a02 6401 6402 8d02 7d01  t.|.j.j.d.d...}.
-000005b0: 7403 7c00 6a01 6a04 6a05 8300 7c00 6a01  t.|.j.j.j...|.j.
-000005c0: 6a06 7c00 6a01 6a07 7c00 6a01 6a08 7c00  j.|.j.j.|.j.j.|.
-000005d0: 6a09 7c00 6a01 6a0a 7c01 7c00 6a0b 8300  j.|.j.j.|.|.j...
-000005e0: 7c00 6a01 6a0c 7c00 6a01 6a0d 7c00 6a0e  |.j.j.|.j.j.|.j.
-000005f0: 8300 7c00 6a01 7c00 830d 5300 2903 4e54  ..|.j.|...S.).NT
-00000600: 2901 da11 6b65 6570 5f62 6c61 6e6b 5f76  )...keep_blank_v
-00000610: 616c 7565 7329 0f72 0600 0000 7218 0000  alues).r....r...
-00000620: 00da 0571 7565 7279 7207 0000 00da 066d  ...queryr......m
-00000630: 6574 686f 6472 1000 0000 da08 7072 6f74  ethodr......prot
-00000640: 6f63 6f6c da04 686f 7374 da04 7061 7468  ocol..host..path
-00000650: da0b 7061 7468 5f6b 7761 7267 73da 0375  ..path_kwargs..u
-00000660: 7269 721c 0000 0072 1e00 0000 da0e 626f  rir....r......bo
-00000670: 6479 5f61 7267 756d 656e 7473 7226 0000  dy_argumentsr&..
-00000680: 0029 0272 1b00 0000 da0f 7175 6572 795f  .).r......query_
-00000690: 6172 6775 6d65 6e74 7372 1500 0000 7215  argumentsr....r.
-000006a0: 0000 0072 1600 0000 da0b 6765 745f 7265  ...r......get_re
-000006b0: 7175 6573 741e 0000 0073 1e00 0000 0001  quest....s......
-000006c0: 1001 0201 0a01 0601 0601 0601 0401 0601  ................
-000006d0: 0201 0601 0601 0601 0601 0401 7a1b 4261  ............z.Ba
-000006e0: 7365 5669 6577 4861 6e64 6c65 722e 6765  seViewHandler.ge
-000006f0: 745f 7265 7175 6573 7463 0200 0000 0000  t_requestc......
-00000700: 0000 0200 0000 0200 0000 4300 0000 7310  ..........C...s.
-00000710: 0000 007c 006a 006a 017c 0183 0101 0064  ...|.j.j.|.....d
-00000720: 0053 0029 014e 2902 da04 7669 6577 da0f  .S.).N)...view..
-00000730: 6265 666f 7265 5f64 6973 7061 7463 6829  before_dispatch)
-00000740: 0272 1b00 0000 7218 0000 0072 1500 0000  .r....r....r....
-00000750: 7215 0000 0072 1600 0000 7233 0000 0030  r....r....r3...0
-00000760: 0000 0073 0200 0000 0001 7a1f 4261 7365  ...s......z.Base
-00000770: 5669 6577 4861 6e64 6c65 722e 6265 666f  ViewHandler.befo
-00000780: 7265 5f64 6973 7061 7463 6863 0200 0000  re_dispatchc....
-00000790: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-000007a0: 7310 0000 007c 006a 006a 017c 0183 0101  s....|.j.j.|....
-000007b0: 0064 0053 0029 014e 2902 7232 0000 00da  .d.S.).N).r2....
-000007c0: 0e61 6674 6572 5f64 6973 7061 7463 6829  .after_dispatch)
-000007d0: 0272 1b00 0000 7218 0000 0072 1500 0000  .r....r....r....
-000007e0: 7215 0000 0072 1600 0000 7234 0000 0033  r....r....r4...3
-000007f0: 0000 0073 0200 0000 0001 7a1e 4261 7365  ...s......z.Base
-00000800: 5669 6577 4861 6e64 6c65 722e 6166 7465  ViewHandler.afte
-00000810: 725f 6469 7370 6174 6368 6301 0000 0000  r_dispatchc.....
-00000820: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00000830: 0e00 0000 7c00 6a00 6a01 8300 0100 6400  ....|.j.j.....d.
-00000840: 5300 2901 4e29 0272 3200 0000 da09 6f6e  S.).N).r2.....on
-00000850: 5f66 696e 6973 6829 0172 1b00 0000 7215  _finish).r....r.
-00000860: 0000 0072 1500 0000 7216 0000 0072 3500  ...r....r....r5.
-00000870: 0000 3600 0000 7302 0000 0000 017a 1942  ..6...s......z.B
-00000880: 6173 6556 6965 7748 616e 646c 6572 2e6f  aseViewHandler.o
-00000890: 6e5f 6669 6e69 7368 6301 0000 0000 0000  n_finishc.......
-000008a0: 0003 0000 0004 0000 0043 0000 0073 2c00  .........C...s,.
-000008b0: 0000 7826 7c00 6a00 6a01 8300 6a02 8300  ..x&|.j.j...j...
-000008c0: 4400 5d14 5c02 7d01 7d02 7c00 6a03 7c01  D.].\.}.}.|.j.|.
-000008d0: 7c02 8302 0100 7110 5700 6400 5300 2901  |.....q.W.d.S.).
-000008e0: 4e29 0472 3200 0000 da0f 6465 6661 756c  N).r2.....defaul
-000008f0: 745f 6865 6164 6572 7372 1a00 0000 da0a  t_headersr......
-00000900: 7365 745f 6865 6164 6572 2903 721b 0000  set_header).r...
-00000910: 00da 046e 616d 65da 0576 616c 7565 7215  ...name..valuer.
-00000920: 0000 0072 1500 0000 7216 0000 00da 1373  ...r....r......s
-00000930: 6574 5f64 6566 6175 6c74 5f68 6561 6465  et_default_heade
-00000940: 7273 3900 0000 7304 0000 0000 0118 017a  rs9...s........z
-00000950: 2342 6173 6556 6965 7748 616e 646c 6572  #BaseViewHandler
-00000960: 2e73 6574 5f64 6566 6175 6c74 5f68 6561  .set_default_hea
-00000970: 6465 7273 6302 0000 0000 0000 0004 0000  dersc...........
-00000980: 000b 0000 0063 0000 0073 b600 0000 7994  .....c...s....y.
-00000990: 7400 7c01 7401 8302 7226 7c00 6a02 7c01  t.|.t...r&|.j.|.
-000009a0: 6a03 7c01 6a04 6401 8d02 0100 7405 6a06  j.|.j.d.....t.j.
-000009b0: 8300 8201 7820 7c01 6a07 8300 4400 5d14  ....x |.j...D.].
-000009c0: 5c02 7d02 7d03 7c00 6a08 7c02 7c03 8302  \.}.}.|.j.|.|...
-000009d0: 0100 7130 5700 7c01 6a04 6400 6b09 725e  ..q0W.|.j.d.k.r^
-000009e0: 7c00 6a09 7c01 6a04 8301 0100 7400 7c01  |.j.|.j.....t.|.
-000009f0: 740a 8302 7282 7c00 6a0b 7c01 6a0c 6601  t...r.|.j.|.j.f.
-00000a00: 7c01 6a0d 707a 6900 8e01 5600 0100 6e10  |.j.pzi...V...n.
-00000a10: 7c00 6a0e 7c01 6a0b 8300 8301 5600 0100  |.j.|.j.....V...
-00000a20: 5700 6e14 0400 740f 6b0a 72a8 0100 0100  W.n...t.k.r.....
-00000a30: 0100 5900 6e02 5800 7405 6a06 8300 8201  ..Y.n.X.t.j.....
-00000a40: 6400 5300 2902 4e29 01da 0673 7461 7475  d.S.).N)...statu
-00000a50: 7329 10da 0a69 7369 6e73 7461 6e63 6572  s)...isinstancer
-00000a60: 0800 0000 da08 7265 6469 7265 6374 da03  ......redirect..
-00000a70: 7572 6c72 3b00 0000 7205 0000 00da 0652  urlr;...r......R
-00000a80: 6574 7572 6eda 0c68 6561 6465 725f 6974  eturn..header_it
-00000a90: 656d 7372 3700 0000 da0a 7365 745f 7374  emsr7.....set_st
-00000aa0: 6174 7573 7209 0000 00da 0672 656e 6465  atusr......rende
-00000ab0: 72da 0874 656d 706c 6174 65da 0464 6174  r..template..dat
-00000ac0: 61da 0666 696e 6973 6872 0c00 0000 2904  a..finishr....).
-00000ad0: 721b 0000 00da 0872 6573 706f 6e73 6572  r......responser
-00000ae0: 3800 0000 7239 0000 0072 1500 0000 7215  8...r9...r....r.
-00000af0: 0000 0072 1600 0000 da0e 7772 6974 655f  ...r......write_
-00000b00: 7265 7370 6f6e 7365 3d00 0000 731c 0000  response=...s...
-00000b10: 0000 0202 010a 0112 0108 0212 0110 020a  ................
-00000b20: 010c 020a 011a 0214 010e 0106 027a 1e42  .............z.B
-00000b30: 6173 6556 6965 7748 616e 646c 6572 2e77  aseViewHandler.w
-00000b40: 7269 7465 5f72 6573 706f 6e73 6563 0200  rite_responsec..
-00000b50: 0000 0000 0000 0900 0000 1300 0000 6b00  ..............k.
-00000b60: 0000 738c 0000 0064 0004 007d 0304 007d  ..s....d...}...}
-00000b70: 047d 057c 026a 0064 0183 0172 267c 0264  .}.|.j.d...r&|.d
-00000b80: 0119 005c 037d 037d 047d 056e 0674 0183  ...\.}.}.}.n.t..
-00000b90: 007d 0479 0c7c 006a 0283 007d 0657 006e  .}.y.|.j...}.W.n
-00000ba0: 2804 0074 036b 0a72 6001 007d 0701 007a  (..t.k.r`..}...z
-00000bb0: 0c7c 076a 047d 0657 0059 0064 0064 007d  .|.j.}.W.Y.d.d.}
-00000bc0: 077e 0758 006e 0258 007c 006a 056a 067c  .~.X.n.X.|.j.j.|
-00000bd0: 067c 037c 047c 0583 047d 087c 006a 077c  .|.|.|...}.|.j.|
-00000be0: 0883 0156 0001 0074 086a 0983 0082 0164  ...V...t.j.....d
-00000bf0: 0053 0029 024e da08 6578 635f 696e 666f  .S.).N..exc_info
-00000c00: 290a da03 6765 74da 0945 7863 6570 7469  )...get..Excepti
-00000c10: 6f6e 7231 0000 0072 0300 0000 7218 0000  onr1...r....r...
-00000c20: 0072 3200 0000 da0e 6572 726f 725f 7265  .r2.....error_re
-00000c30: 7370 6f6e 7365 7247 0000 0072 0500 0000  sponserG...r....
-00000c40: 723f 0000 0029 0972 1b00 0000 da0b 7374  r?...).r......st
-00000c50: 6174 7573 5f63 6f64 65da 066b 7761 7267  atus_code..kwarg
-00000c60: 73da 0865 7863 5f74 7970 65da 0365 7863  s..exc_type..exc
-00000c70: da09 7472 6163 6562 6163 6b72 1800 0000  ..tracebackr....
-00000c80: da01 6572 4600 0000 7215 0000 0072 1500  ..erF...r....r..
-00000c90: 0000 7216 0000 00da 0b77 7269 7465 5f65  ..r......write_e
-00000ca0: 7272 6f72 5300 0000 7316 0000 0000 020c  rrorS...s.......
-00000cb0: 020a 0110 0206 0202 010c 0110 0118 0212  ................
-00000cc0: 010c 017a 1b42 6173 6556 6965 7748 616e  ...z.BaseViewHan
-00000cd0: 646c 6572 2e77 7269 7465 5f65 7272 6f72  dler.write_error
-00000ce0: 6301 0000 0000 0000 0003 0000 0002 0000  c...............
-00000cf0: 004f 0000 0073 1600 0000 7c00 6a00 7401  .O...s....|.j.t.
-00000d00: 8301 0100 7c00 6a02 8300 0100 6400 5300  ....|.j.....d.S.
-00000d10: 2901 4e29 0372 4100 0000 720a 0000 0072  ).N).rA...r....r
-00000d20: 4500 0000 2903 721b 0000 00da 0461 7267  E...).r......arg
-00000d30: 7372 4d00 0000 7215 0000 0072 1500 0000  srM...r....r....
-00000d40: 7216 0000 00da 076f 7074 696f 6e73 6500  r......optionse.
-00000d50: 0000 7304 0000 0000 010a 017a 1742 6173  ..s........z.Bas
-00000d60: 6556 6965 7748 616e 646c 6572 2e6f 7074  eViewHandler.opt
-00000d70: 696f 6e73 6302 0000 0000 0000 0007 0000  ionsc...........
-00000d80: 0006 0000 002f 0000 0073 7e00 0000 8804  ...../...s~.....
-00000d90: 6a00 8300 8903 7401 8803 8301 7d04 7c04  j.....t.....}.|.
-00000da0: 723c 7402 6a03 6401 7c04 6a04 6402 8301  r<t.j.d.|.j.d...
-00000db0: 7c04 6a04 6403 8301 7c04 6a04 6404 8301  |.j.d...|.j.d...
-00000dc0: 6405 9c03 8302 0100 6e0c 7402 6a03 6401  d.......n.t.j.d.
-00000dd0: 6900 8302 0100 8700 8701 8702 8703 8704  i...............
-00000de0: 6605 6406 6407 8408 7d05 7405 7c05 8301  f.d.d...}.t.|...
-00000df0: 5600 7d06 8804 6a06 7c06 8301 5600 0100  V.}...j.|...V...
-00000e00: 7407 6a08 8300 8201 6400 5300 2908 4e7a  t.j.....d.S.).Nz
-00000e10: 1344 6174 6162 6173 6520 636f 6e6e 6563  .Database connec
-00000e20: 7469 6f6e 7238 0000 00da 0770 726f 6a65  tionr8.....proje
-00000e30: 6374 da05 746f 6b65 6e29 0372 3800 0000  ct..token).r8...
-00000e40: 7255 0000 0072 5600 0000 6300 0000 0000  rU...rV...c.....
-00000e50: 0000 0001 0000 0003 0000 0013 0000 0073  ...............s
-00000e60: 2e00 0000 8804 6a00 8803 8301 0100 8804  ......j.........
-00000e70: 6a01 6a02 8800 8803 6602 8801 9e02 8802  j.j.....f.......
-00000e80: 8e01 7d00 8804 6a03 8803 8301 0100 7c00  ..}...j.......|.
-00000e90: 5300 2901 4e29 0472 3300 0000 7232 0000  S.).N).r3...r2..
-00000ea0: 00da 0864 6973 7061 7463 6872 3400 0000  ...dispatchr4...
-00000eb0: 2901 da06 7265 7375 6c74 2905 da06 6163  )...result)...ac
-00000ec0: 7469 6f6e 7253 0000 0072 4d00 0000 7218  tionrS...rM...r.
-00000ed0: 0000 0072 1b00 0000 7215 0000 0072 1600  ...r....r....r..
-00000ee0: 0000 da07 6578 6563 7574 6577 0000 0073  ....executew...s
-00000ef0: 0800 0000 0001 0a01 1601 0a01 7a29 4261  ............z)Ba
-00000f00: 7365 5669 6577 4861 6e64 6c65 722e 6469  seViewHandler.di
-00000f10: 7370 6174 6368 2e3c 6c6f 6361 6c73 3e2e  spatch.<locals>.
-00000f20: 6578 6563 7574 6529 0972 3100 0000 7202  execute).r1...r.
-00000f30: 0000 0072 0400 0000 da0b 7365 745f 636f  ...r......set_co
-00000f40: 6e74 6578 7472 4900 0000 720b 0000 0072  ntextrI...r....r
-00000f50: 4700 0000 7205 0000 0072 3f00 0000 2907  G...r....r?...).
-00000f60: 721b 0000 0072 5900 0000 7253 0000 0072  r....rY...rS...r
-00000f70: 4d00 0000 da0a 636f 6e6e 6563 7469 6f6e  M.....connection
-00000f80: 725a 0000 0072 4600 0000 7215 0000 0029  rZ...rF...r....)
-00000f90: 0572 5900 0000 7253 0000 0072 4d00 0000  .rY...rS...rM...
-00000fa0: 7218 0000 0072 1b00 0000 7216 0000 0072  r....r....r....r
-00000fb0: 5700 0000 6900 0000 7318 0000 0000 0208  W...i...s.......
-00000fc0: 0208 0104 0106 0108 0108 0112 030c 0214  ................
-00000fd0: 060a 010c 017a 1842 6173 6556 6965 7748  .....z.BaseViewH
-00000fe0: 616e 646c 6572 2e64 6973 7061 7463 6863  andler.dispatchc
-00000ff0: 0100 0000 0000 0000 0300 0000 0300 0000  ................
-00001000: 4f00 0000 7310 0000 007c 006a 0064 027c  O...s....|.j.d.|
-00001010: 019e 027c 028e 0153 0029 034e 7249 0000  ...|...S.).NrI..
-00001020: 0029 0172 4900 0000 2901 7257 0000 0029  .).rI...).rW...)
-00001030: 0372 1b00 0000 7253 0000 0072 4d00 0000  .r....rS...rM...
-00001040: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001050: 4900 0000 8100 0000 7302 0000 0000 017a  I.......s......z
-00001060: 1342 6173 6556 6965 7748 616e 646c 6572  .BaseViewHandler
-00001070: 2e67 6574 6301 0000 0000 0000 0003 0000  .getc...........
-00001080: 0003 0000 004f 0000 0073 1000 0000 7c00  .....O...s....|.
-00001090: 6a00 6402 7c01 9e02 7c02 8e01 5300 2903  j.d.|...|...S.).
-000010a0: 4eda 0470 6f73 7429 0172 5d00 0000 2901  N..post).r]...).
-000010b0: 7257 0000 0029 0372 1b00 0000 7253 0000  rW...).r....rS..
-000010c0: 0072 4d00 0000 7215 0000 0072 1500 0000  .rM...r....r....
-000010d0: 7216 0000 0072 5d00 0000 8400 0000 7302  r....r].......s.
-000010e0: 0000 0000 017a 1442 6173 6556 6965 7748  .....z.BaseViewH
-000010f0: 616e 646c 6572 2e70 6f73 7463 0100 0000  andler.postc....
-00001100: 0000 0000 0300 0000 0300 0000 4f00 0000  ............O...
-00001110: 7310 0000 007c 006a 0064 027c 019e 027c  s....|.j.d.|...|
-00001120: 028e 0153 0029 034e da03 7075 7429 0172  ...S.).N..put).r
-00001130: 5e00 0000 2901 7257 0000 0029 0372 1b00  ^...).rW...).r..
-00001140: 0000 7253 0000 0072 4d00 0000 7215 0000  ..rS...rM...r...
-00001150: 0072 1500 0000 7216 0000 0072 5e00 0000  .r....r....r^...
-00001160: 8700 0000 7302 0000 0000 017a 1342 6173  ....s......z.Bas
-00001170: 6556 6965 7748 616e 646c 6572 2e70 7574  eViewHandler.put
-00001180: 6301 0000 0000 0000 0003 0000 0003 0000  c...............
-00001190: 004f 0000 0073 1000 0000 7c00 6a00 6402  .O...s....|.j.d.
-000011a0: 7c01 9e02 7c02 8e01 5300 2903 4eda 0570  |...|...S.).N..p
-000011b0: 6174 6368 2901 725f 0000 0029 0172 5700  atch).r_...).rW.
-000011c0: 0000 2903 721b 0000 0072 5300 0000 724d  ..).r....rS...rM
-000011d0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000011e0: 0000 725f 0000 008a 0000 0073 0200 0000  ..r_.......s....
-000011f0: 0001 7a15 4261 7365 5669 6577 4861 6e64  ..z.BaseViewHand
-00001200: 6c65 722e 7061 7463 6863 0100 0000 0000  ler.patchc......
-00001210: 0000 0300 0000 0300 0000 4f00 0000 7310  ..........O...s.
-00001220: 0000 007c 006a 0064 027c 019e 027c 028e  ...|.j.d.|...|..
-00001230: 0153 0029 034e da06 6465 6c65 7465 2901  .S.).N..delete).
-00001240: 7260 0000 0029 0172 5700 0000 2903 721b  r`...).rW...).r.
-00001250: 0000 0072 5300 0000 724d 0000 0072 1500  ...rS...rM...r..
-00001260: 0000 7215 0000 0072 1600 0000 7260 0000  ..r....r....r`..
-00001270: 008d 0000 0073 0200 0000 0001 7a16 4261  .....s......z.Ba
-00001280: 7365 5669 6577 4861 6e64 6c65 722e 6465  seViewHandler.de
-00001290: 6c65 7465 2916 da08 5f5f 6e61 6d65 5f5f  lete)...__name__
-000012a0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000012b0: 7175 616c 6e61 6d65 5f5f 7232 0000 0072  qualname__r2...r
-000012c0: 1c00 0000 7226 0000 0072 3100 0000 7233  ....r&...r1...r3
-000012d0: 0000 0072 3400 0000 7235 0000 0072 3a00  ...r4...r5...r:.
-000012e0: 0000 7205 0000 00da 0963 6f72 6f75 7469  ..r......corouti
-000012f0: 6e65 7247 0000 0072 5200 0000 7254 0000  nerG...rR...rT..
-00001300: 0072 5700 0000 7249 0000 0072 5d00 0000  .rW...rI...r]...
-00001310: 725e 0000 0072 5f00 0000 7260 0000 0072  r^...r_...r`...r
-00001320: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00001330: 0000 0072 0d00 0000 1000 0000 7322 0000  ...r........s"..
-00001340: 0008 0104 0208 0308 0808 1208 0308 0308  ................
-00001350: 0308 040e 160e 1208 040e 1808 0308 0308  ................
-00001360: 0308 0372 0d00 0000 6301 0000 0000 0000  ...r....c.......
-00001370: 0002 0000 0004 0000 0003 0000 0073 1800  .............s..
-00001380: 0000 4700 8700 6601 6401 6402 8408 6402  ..G...f.d.d...d.
-00001390: 7400 8303 7d01 7c01 5300 2903 4e63 0000  t...}.|.S.).Nc..
-000013a0: 0000 0000 0000 0000 0000 0100 0000 0000  ................
-000013b0: 0000 7312 0000 0065 005a 0164 005a 0294  ..s....e.Z.d.Z..
-000013c0: 0083 005a 0364 0153 0029 027a 2176 6965  ...Z.d.S.).z!vie
-000013d0: 775f 6861 6e64 6c65 722e 3c6c 6f63 616c  w_handler.<local
-000013e0: 733e 2e56 6965 7748 616e 646c 6572 4e29  s>.ViewHandlerN)
-000013f0: 0472 6100 0000 7262 0000 0072 6300 0000  .ra...rb...rc...
-00001400: 7232 0000 0072 1500 0000 2901 da03 636c  r2...r....)...cl
-00001410: 7372 1500 0000 7216 0000 00da 0b56 6965  sr....r......Vie
-00001420: 7748 616e 646c 6572 9200 0000 7302 0000  wHandler....s...
-00001430: 0008 0172 6600 0000 2901 720d 0000 0029  ...rf...).r....)
-00001440: 0272 6500 0000 7266 0000 0072 1500 0000  .re...rf...r....
-00001450: 2901 7265 0000 0072 1600 0000 da0c 7669  ).re...r......vi
-00001460: 6577 5f68 616e 646c 6572 9100 0000 7304  ew_handler....s.
-00001470: 0000 0000 0114 0372 6700 0000 291b da0b  .......rg...)...
-00001480: 746f 726e 6164 6f2e 7765 62da 0774 6f72  tornado.web..tor
-00001490: 6e61 646f da12 6a65 745f 6272 6964 6765  nado..jet_bridge
-000014a0: 5f62 6173 652e 6462 7202 0000 005a 286a  _base.dbr....Z(j
-000014b0: 6574 5f62 7269 6467 655f 6261 7365 2e65  et_bridge_base.e
-000014c0: 7863 6570 7469 6f6e 732e 7265 7175 6573  xceptions.reques
-000014d0: 745f 6572 726f 7272 0300 0000 da16 6a65  t_errorr......je
-000014e0: 745f 6272 6964 6765 5f62 6173 652e 7365  t_bridge_base.se
-000014f0: 6e74 7279 7204 0000 0072 0500 0000 da16  ntryr....r......
-00001500: 7369 782e 6d6f 7665 732e 7572 6c6c 6962  six.moves.urllib
-00001510: 5f70 6172 7365 7206 0000 005a 176a 6574  _parser....Z.jet
-00001520: 5f62 7269 6467 655f 6261 7365 2e72 6571  _bridge_base.req
-00001530: 7565 7374 7207 0000 00da 226a 6574 5f62  uestr....."jet_b
-00001540: 7269 6467 655f 6261 7365 2e72 6573 706f  ridge_base.respo
-00001550: 6e73 6573 2e72 6564 6972 6563 7472 0800  nses.redirectr..
-00001560: 0000 da22 6a65 745f 6272 6964 6765 5f62  ..."jet_bridge_b
-00001570: 6173 652e 7265 7370 6f6e 7365 732e 7465  ase.responses.te
-00001580: 6d70 6c61 7465 7209 0000 005a 166a 6574  mplater....Z.jet
-00001590: 5f62 7269 6467 655f 6261 7365 2e73 7461  _bridge_base.sta
-000015a0: 7475 7372 0a00 0000 da20 6a65 745f 6272  tusr..... jet_br
-000015b0: 6964 6765 5f62 6173 652e 7574 696c 732e  idge_base.utils.
-000015c0: 6173 796e 635f 6578 6563 720b 0000 005a  async_execr....Z
-000015d0: 1074 6f72 6e61 646f 2e69 6f73 7472 6561  .tornado.iostrea
-000015e0: 6d72 0c00 0000 da03 7765 62da 0e52 6571  mr......web..Req
-000015f0: 7565 7374 4861 6e64 6c65 7272 0d00 0000  uestHandlerr....
-00001600: 7267 0000 0072 1500 0000 7215 0000 0072  rg...r....r....r
-00001610: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-00001620: 6c65 3e01 0000 0073 1c00 0000 0801 0c01  le>....s........
-00001630: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c01  ................
-00001640: 0c01 0c03 147f 0002                      ........
+00000020: 0073 b400 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
+00000030: 6401 6c01 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c07 6d08 5a08 0100 6400 6405 6c02  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6408 6c0e 6d0f 5a0f 0100 6400 6409 6c10  d.l.m.Z...d.d.l.
+00000090: 6d11 5a11 0100 6400 640a 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 640b 6c14 6d15 5a15 0100 6400  ..d.d.l.m.Z...d.
+000000b0: 640c 6c16 6d17 5a17 0100 4700 640d 640e  d.l.m.Z...G.d.d.
+000000c0: 8400 640e 6502 6a18 6a19 8303 5a1a 640f  ..d.e.j.j...Z.d.
+000000d0: 6410 8400 5a1b 6401 5300 2911 e900 0000  d...Z.d.S.).....
+000000e0: 004e 2901 da0e 6765 745f 636f 6e6e 6563  .N)...get_connec
+000000f0: 7469 6f6e 2901 da0c 5265 7175 6573 7445  tion)...RequestE
+00000100: 7272 6f72 2901 da11 7365 6e74 7279 5f63  rror)...sentry_c
+00000110: 6f6e 7472 6f6c 6c65 7229 01da 0367 656e  ontroller)...gen
+00000120: 2901 da08 7061 7273 655f 7173 2901 da07  )...parse_qs)...
+00000130: 5265 7175 6573 7429 01da 1052 6564 6972  Request)...Redir
+00000140: 6563 7452 6573 706f 6e73 6529 01da 1054  ectResponse)...T
+00000150: 656d 706c 6174 6552 6573 706f 6e73 6529  emplateResponse)
+00000160: 01da 1348 5454 505f 3230 345f 4e4f 5f43  ...HTTP_204_NO_C
+00000170: 4f4e 5445 4e54 2901 da09 6173 5f66 7574  ONTENT)...as_fut
+00000180: 7572 6529 01da 1153 7472 6561 6d43 6c6f  ure)...StreamClo
+00000190: 7365 6445 7272 6f72 6300 0000 0000 0000  sedErrorc.......
+000001a0: 0000 0000 0003 0000 0040 0000 0073 a200  .........@...s..
+000001b0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000001c0: 6403 8400 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
+000001d0: 6407 8400 5a06 6408 6409 8400 5a07 640a  d...Z.d.d...Z.d.
+000001e0: 640b 8400 5a08 640c 640d 8400 5a09 640e  d...Z.d.d...Z.d.
+000001f0: 640f 8400 5a0a 650b 6a0c 6410 6411 8400  d...Z.e.j.d.d...
+00000200: 8301 5a0d 650b 6a0c 6412 6413 8400 8301  ..Z.e.j.d.d.....
+00000210: 5a0e 6414 6415 8400 5a0f 650b 6a0c 6416  Z.d.d...Z.e.j.d.
+00000220: 6417 8400 8301 5a10 6418 6419 8400 5a11  d.....Z.d.d...Z.
+00000230: 641a 641b 8400 5a12 641c 641d 8400 5a13  d.d...Z.d.d...Z.
+00000240: 641e 641f 8400 5a14 6420 6421 8400 5a15  d.d...Z.d d!..Z.
+00000250: 6401 5300 2922 da0f 4261 7365 5669 6577  d.S.)"..BaseView
+00000260: 4861 6e64 6c65 724e 6301 0000 0000 0000  HandlerNc.......
+00000270: 0001 0000 0002 0000 0043 0000 0073 1600  .........C...s..
+00000280: 0000 6401 6402 8400 7c00 6a00 6a01 6a02  ..d.d...|.j.j.j.
+00000290: 8300 4400 8301 5300 2903 4e63 0100 0000  ..D...S.).Nc....
+000002a0: 0000 0000 0300 0000 0600 0000 5300 0000  ............S...
+000002b0: 7322 0000 0069 007c 005d 1a5c 027d 017d  s"...i.|.].\.}.}
+000002c0: 027c 027c 016a 0083 006a 0164 0064 0183  .|.|.j...j.d.d..
+000002d0: 0293 0271 0453 0029 02fa 012d da01 5f29  ...q.S.)...-.._)
+000002e0: 02da 0575 7070 6572 da07 7265 706c 6163  ...upper..replac
+000002f0: 6529 03da 022e 30da 016b da01 76a9 0072  e)....0..k..v..r
+00000300: 1500 0000 fa5a 2f55 7365 7273 2f66 316e  .....Z/Users/f1n
+00000310: 616c 2f44 726f 7062 6f78 2f70 7974 686f  al/Dropbox/pytho
+00000320: 6e2f 6a65 742d 6272 6964 6765 2f73 7263  n/jet-bridge/src
+00000330: 2f70 6163 6b61 6765 732f 6a65 745f 6272  /packages/jet_br
+00000340: 6964 6765 2f6a 6574 5f62 7269 6467 652f  idge/jet_bridge/
+00000350: 6861 6e64 6c65 7273 2f76 6965 772e 7079  handlers/view.py
+00000360: fa0a 3c64 6963 7463 6f6d 703e 1600 0000  ..<dictcomp>....
+00000370: 7302 0000 0006 007a 3342 6173 6556 6965  s......z3BaseVie
+00000380: 7748 616e 646c 6572 2e72 6571 7565 7374  wHandler.request
+00000390: 5f68 6561 6465 7273 2e3c 6c6f 6361 6c73  _headers.<locals
+000003a0: 3e2e 3c64 6963 7463 6f6d 703e 2903 da07  >.<dictcomp>)...
+000003b0: 7265 7175 6573 74da 0768 6561 6465 7273  request..headers
+000003c0: da05 6974 656d 7329 01da 0473 656c 6672  ..items)...selfr
+000003d0: 1500 0000 7215 0000 0072 1600 0000 da0f  ....r....r......
+000003e0: 7265 7175 6573 745f 6865 6164 6572 7315  request_headers.
+000003f0: 0000 0073 0200 0000 0001 7a1f 4261 7365  ...s......z.Base
+00000400: 5669 6577 4861 6e64 6c65 722e 7265 7175  ViewHandler.requ
+00000410: 6573 745f 6865 6164 6572 7363 0100 0000  est_headersc....
+00000420: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000430: 731e 0000 0064 0164 0284 007d 0174 0074  s....d.d...}.t.t
+00000440: 017c 017c 006a 026a 036a 0483 0083 0283  .|.|.j.j.j......
+00000450: 0153 0029 034e 6301 0000 0000 0000 0004  .S.).Nc.........
+00000460: 0000 0003 0000 0053 0000 0073 2000 0000  .......S...s ...
+00000470: 7c00 5c02 7d01 7d02 7c02 6401 1900 7d03  |.\.}.}.|.d...}.
+00000480: 7c01 7c03 6a00 7c03 6a01 6602 6602 5300  |.|.j.|.j.f.f.S.
+00000490: 2902 4e72 0100 0000 2902 da08 6669 6c65  ).Nr....)...file
+000004a0: 6e61 6d65 da04 626f 6479 2904 da03 6172  name..body)...ar
+000004b0: 67da 036b 6579 da05 6669 6c65 73da 0466  g..key..files..f
+000004c0: 696c 6572 1500 0000 7215 0000 0072 1600  iler....r....r..
+000004d0: 0000 da08 6d61 705f 6669 6c65 1900 0000  ....map_file....
+000004e0: 7306 0000 0000 0108 0108 017a 2f42 6173  s..........z/Bas
+000004f0: 6556 6965 7748 616e 646c 6572 2e72 6571  eViewHandler.req
+00000500: 7565 7374 5f66 696c 6573 2e3c 6c6f 6361  uest_files.<loca
+00000510: 6c73 3e2e 6d61 705f 6669 6c65 2905 da04  ls>.map_file)...
+00000520: 6469 6374 da03 6d61 7072 1800 0000 7221  dict..mapr....r!
+00000530: 0000 0072 1a00 0000 2902 721b 0000 0072  ...r....).r....r
+00000540: 2300 0000 7215 0000 0072 1500 0000 7216  #...r....r....r.
+00000550: 0000 00da 0d72 6571 7565 7374 5f66 696c  .....request_fil
+00000560: 6573 1800 0000 7304 0000 0000 0108 057a  es....s........z
+00000570: 1d42 6173 6556 6965 7748 616e 646c 6572  .BaseViewHandler
+00000580: 2e72 6571 7565 7374 5f66 696c 6573 6301  .request_filesc.
+00000590: 0000 0000 0000 0002 0000 000e 0000 0043  ...............C
+000005a0: 0000 0073 5c00 0000 7400 7c00 6a01 6a02  ...s\...t.|.j.j.
+000005b0: 6401 6402 8d02 7d01 7403 7c00 6a01 6a04  d.d...}.t.|.j.j.
+000005c0: 6a05 8300 7c00 6a01 6a06 7c00 6a01 6a07  j...|.j.j.|.j.j.
+000005d0: 7c00 6a01 6a08 7c00 6a09 7c00 6a01 6a0a  |.j.j.|.j.|.j.j.
+000005e0: 7c01 7c00 6a0b 8300 7c00 6a01 6a0c 7c00  |.|.j...|.j.j.|.
+000005f0: 6a01 6a0d 7c00 6a0e 8300 7c00 6a01 7c00  j.j.|.j...|.j.|.
+00000600: 830d 5300 2903 4e54 2901 da11 6b65 6570  ..S.).NT)...keep
+00000610: 5f62 6c61 6e6b 5f76 616c 7565 7329 0f72  _blank_values).r
+00000620: 0600 0000 7218 0000 00da 0571 7565 7279  ....r......query
+00000630: 7207 0000 00da 066d 6574 686f 6472 1000  r......methodr..
+00000640: 0000 da08 7072 6f74 6f63 6f6c da04 686f  ....protocol..ho
+00000650: 7374 da04 7061 7468 da0b 7061 7468 5f6b  st..path..path_k
+00000660: 7761 7267 73da 0375 7269 721c 0000 0072  wargs..urir....r
+00000670: 1e00 0000 da0e 626f 6479 5f61 7267 756d  ......body_argum
+00000680: 656e 7473 7226 0000 0029 0272 1b00 0000  entsr&...).r....
+00000690: da0f 7175 6572 795f 6172 6775 6d65 6e74  ..query_argument
+000006a0: 7372 1500 0000 7215 0000 0072 1600 0000  sr....r....r....
+000006b0: da0b 6765 745f 7265 7175 6573 7420 0000  ..get_request ..
+000006c0: 0073 1e00 0000 0001 1001 0201 0a01 0601  .s..............
+000006d0: 0601 0601 0401 0601 0201 0601 0601 0601  ................
+000006e0: 0601 0401 7a1b 4261 7365 5669 6577 4861  ....z.BaseViewHa
+000006f0: 6e64 6c65 722e 6765 745f 7265 7175 6573  ndler.get_reques
+00000700: 7463 0200 0000 0000 0000 0200 0000 0200  tc..............
+00000710: 0000 4300 0000 7310 0000 007c 006a 006a  ..C...s....|.j.j
+00000720: 017c 0183 0101 0064 0053 0029 014e 2902  .|.....d.S.).N).
+00000730: da04 7669 6577 da0f 6265 666f 7265 5f64  ..view..before_d
+00000740: 6973 7061 7463 6829 0272 1b00 0000 7218  ispatch).r....r.
+00000750: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000760: 0000 7233 0000 0032 0000 0073 0200 0000  ..r3...2...s....
+00000770: 0001 7a1f 4261 7365 5669 6577 4861 6e64  ..z.BaseViewHand
+00000780: 6c65 722e 6265 666f 7265 5f64 6973 7061  ler.before_dispa
+00000790: 7463 6863 0200 0000 0000 0000 0200 0000  tchc............
+000007a0: 0200 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
+000007b0: 006a 017c 0183 0101 0064 0053 0029 014e  .j.|.....d.S.).N
+000007c0: 2902 7232 0000 00da 0e61 6674 6572 5f64  ).r2.....after_d
+000007d0: 6973 7061 7463 6829 0272 1b00 0000 7218  ispatch).r....r.
+000007e0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000007f0: 0000 7234 0000 0035 0000 0073 0200 0000  ..r4...5...s....
+00000800: 0001 7a1e 4261 7365 5669 6577 4861 6e64  ..z.BaseViewHand
+00000810: 6c65 722e 6166 7465 725f 6469 7370 6174  ler.after_dispat
+00000820: 6368 6301 0000 0000 0000 0001 0000 0001  chc.............
+00000830: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
+00000840: 6a01 8300 0100 6400 5300 2901 4e29 0272  j.....d.S.).N).r
+00000850: 3200 0000 da09 6f6e 5f66 696e 6973 6829  2.....on_finish)
+00000860: 0172 1b00 0000 7215 0000 0072 1500 0000  .r....r....r....
+00000870: 7216 0000 0072 3500 0000 3800 0000 7302  r....r5...8...s.
+00000880: 0000 0000 017a 1942 6173 6556 6965 7748  .....z.BaseViewH
+00000890: 616e 646c 6572 2e6f 6e5f 6669 6e69 7368  andler.on_finish
+000008a0: 6301 0000 0000 0000 0003 0000 0004 0000  c...............
+000008b0: 0043 0000 0073 2c00 0000 7826 7c00 6a00  .C...s,...x&|.j.
+000008c0: 6a01 8300 6a02 8300 4400 5d14 5c02 7d01  j...j...D.].\.}.
+000008d0: 7d02 7c00 6a03 7c01 7c02 8302 0100 7110  }.|.j.|.|.....q.
+000008e0: 5700 6400 5300 2901 4e29 0472 3200 0000  W.d.S.).N).r2...
+000008f0: da0f 6465 6661 756c 745f 6865 6164 6572  ..default_header
+00000900: 7372 1a00 0000 da0a 7365 745f 6865 6164  sr......set_head
+00000910: 6572 2903 721b 0000 00da 046e 616d 65da  er).r......name.
+00000920: 0576 616c 7565 7215 0000 0072 1500 0000  .valuer....r....
+00000930: 7216 0000 00da 1373 6574 5f64 6566 6175  r......set_defau
+00000940: 6c74 5f68 6561 6465 7273 3b00 0000 7304  lt_headers;...s.
+00000950: 0000 0000 0118 017a 2342 6173 6556 6965  .......z#BaseVie
+00000960: 7748 616e 646c 6572 2e73 6574 5f64 6566  wHandler.set_def
+00000970: 6175 6c74 5f68 6561 6465 7273 6302 0000  ault_headersc...
+00000980: 0000 0000 0004 0000 000b 0000 0063 0000  .............c..
+00000990: 0073 b600 0000 7994 7400 7c01 7401 8302  .s....y.t.|.t...
+000009a0: 7226 7c00 6a02 7c01 6a03 7c01 6a04 6401  r&|.j.|.j.|.j.d.
+000009b0: 8d02 0100 7405 6a06 8300 8201 7820 7c01  ....t.j.....x |.
+000009c0: 6a07 8300 4400 5d14 5c02 7d02 7d03 7c00  j...D.].\.}.}.|.
+000009d0: 6a08 7c02 7c03 8302 0100 7130 5700 7c01  j.|.|.....q0W.|.
+000009e0: 6a04 6400 6b09 725e 7c00 6a09 7c01 6a04  j.d.k.r^|.j.|.j.
+000009f0: 8301 0100 7400 7c01 740a 8302 7282 7c00  ....t.|.t...r.|.
+00000a00: 6a0b 7c01 6a0c 6601 7c01 6a0d 707a 6900  j.|.j.f.|.j.pzi.
+00000a10: 8e01 5600 0100 6e10 7c00 6a0e 7c01 6a0b  ..V...n.|.j.|.j.
+00000a20: 8300 8301 5600 0100 5700 6e14 0400 740f  ....V...W.n...t.
+00000a30: 6b0a 72a8 0100 0100 0100 5900 6e02 5800  k.r.......Y.n.X.
+00000a40: 7405 6a06 8300 8201 6400 5300 2902 4e29  t.j.....d.S.).N)
+00000a50: 01da 0673 7461 7475 7329 10da 0a69 7369  ...status)...isi
+00000a60: 6e73 7461 6e63 6572 0800 0000 da08 7265  nstancer......re
+00000a70: 6469 7265 6374 da03 7572 6c72 3b00 0000  direct..urlr;...
+00000a80: 7205 0000 00da 0652 6574 7572 6eda 0c68  r......Return..h
+00000a90: 6561 6465 725f 6974 656d 7372 3700 0000  eader_itemsr7...
+00000aa0: da0a 7365 745f 7374 6174 7573 7209 0000  ..set_statusr...
+00000ab0: 00da 0672 656e 6465 72da 0874 656d 706c  ...render..templ
+00000ac0: 6174 65da 0464 6174 61da 0666 696e 6973  ate..data..finis
+00000ad0: 6872 0c00 0000 2904 721b 0000 00da 0872  hr....).r......r
+00000ae0: 6573 706f 6e73 6572 3800 0000 7239 0000  esponser8...r9..
+00000af0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000b00: da0e 7772 6974 655f 7265 7370 6f6e 7365  ..write_response
+00000b10: 3f00 0000 731c 0000 0000 0202 010a 0112  ?...s...........
+00000b20: 0108 0212 0110 020a 010c 020a 011a 0214  ................
+00000b30: 010e 0106 027a 1e42 6173 6556 6965 7748  .....z.BaseViewH
+00000b40: 616e 646c 6572 2e77 7269 7465 5f72 6573  andler.write_res
+00000b50: 706f 6e73 6563 0200 0000 0000 0000 0900  ponsec..........
+00000b60: 0000 1300 0000 6b00 0000 738c 0000 0064  ......k...s....d
+00000b70: 0004 007d 0304 007d 047d 057c 026a 0064  ...}...}.}.|.j.d
+00000b80: 0183 0172 267c 0264 0119 005c 037d 037d  ...r&|.d...\.}.}
+00000b90: 047d 056e 0674 0183 007d 0479 0c7c 006a  .}.n.t...}.y.|.j
+00000ba0: 0283 007d 0657 006e 2804 0074 036b 0a72  ...}.W.n(..t.k.r
+00000bb0: 6001 007d 0701 007a 0c7c 076a 047d 0657  `..}...z.|.j.}.W
+00000bc0: 0059 0064 0064 007d 077e 0758 006e 0258  .Y.d.d.}.~.X.n.X
+00000bd0: 007c 006a 056a 067c 067c 037c 047c 0583  .|.j.j.|.|.|.|..
+00000be0: 047d 087c 006a 077c 0883 0156 0001 0074  .}.|.j.|...V...t
+00000bf0: 086a 0983 0082 0164 0053 0029 024e da08  .j.....d.S.).N..
+00000c00: 6578 635f 696e 666f 290a da03 6765 74da  exc_info)...get.
+00000c10: 0945 7863 6570 7469 6f6e 7231 0000 0072  .Exceptionr1...r
+00000c20: 0300 0000 7218 0000 0072 3200 0000 da0e  ....r....r2.....
+00000c30: 6572 726f 725f 7265 7370 6f6e 7365 7247  error_responserG
+00000c40: 0000 0072 0500 0000 723f 0000 0029 0972  ...r....r?...).r
+00000c50: 1b00 0000 da0b 7374 6174 7573 5f63 6f64  ......status_cod
+00000c60: 65da 066b 7761 7267 73da 0865 7863 5f74  e..kwargs..exc_t
+00000c70: 7970 65da 0365 7863 da09 7472 6163 6562  ype..exc..traceb
+00000c80: 6163 6b72 1800 0000 da01 6572 4600 0000  ackr......erF...
+00000c90: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000ca0: 0b77 7269 7465 5f65 7272 6f72 5500 0000  .write_errorU...
+00000cb0: 7316 0000 0000 020c 020a 0110 0206 0202  s...............
+00000cc0: 010c 0110 0118 0212 010c 017a 1b42 6173  ...........z.Bas
+00000cd0: 6556 6965 7748 616e 646c 6572 2e77 7269  eViewHandler.wri
+00000ce0: 7465 5f65 7272 6f72 6301 0000 0000 0000  te_errorc.......
+00000cf0: 0003 0000 0002 0000 004f 0000 0073 1600  .........O...s..
+00000d00: 0000 7c00 6a00 7401 8301 0100 7c00 6a02  ..|.j.t.....|.j.
+00000d10: 8300 0100 6400 5300 2901 4e29 0372 4100  ....d.S.).N).rA.
+00000d20: 0000 720a 0000 0072 4500 0000 2903 721b  ..r....rE...).r.
+00000d30: 0000 00da 0461 7267 7372 4d00 0000 7215  .....argsrM...r.
+00000d40: 0000 0072 1500 0000 7216 0000 00da 076f  ...r....r......o
+00000d50: 7074 696f 6e73 6700 0000 7304 0000 0000  ptionsg...s.....
+00000d60: 010a 017a 1742 6173 6556 6965 7748 616e  ...z.BaseViewHan
+00000d70: 646c 6572 2e6f 7074 696f 6e73 6302 0000  dler.optionsc...
+00000d80: 0000 0000 000a 0000 0011 0000 002f 0000  ............./..
+00000d90: 0073 cc00 0000 8804 6a00 8300 8903 7401  .s......j.....t.
+00000da0: 8803 8301 7d04 7c04 723c 7402 6a03 6401  ....}.|.r<t.j.d.
+00000db0: 7c04 6a04 6402 8301 7c04 6a04 6403 8301  |.j.d...|.j.d...
+00000dc0: 7c04 6a04 6404 8301 6405 9c03 8302 0100  |.j.d...d.......
+00000dd0: 6e0c 7402 6a03 6401 6900 8302 0100 8700  n.t.j.d.i.......
+00000de0: 8701 8702 8703 8704 6605 6406 6407 8408  ........f.d.d...
+00000df0: 7d05 7a60 791a 7405 7c05 8301 5600 7d06  }.z`y.t.|...V.}.
+00000e00: 8804 6a06 7c06 8301 5600 0100 5700 6e40  ..j.|...V...W.n@
+00000e10: 0400 7407 6b0a 72b8 0100 0100 0100 7408  ..t.k.r.......t.
+00000e20: 6a09 8300 5c03 7d07 7d08 7d09 8804 6a0a  j...\.}.}.}...j.
+00000e30: 6a0b 8803 7c07 7c08 7c09 8304 7d06 8804  j...|.|.|...}...
+00000e40: 6a06 7c06 8301 5600 0100 5900 6e02 5800  j.|...V...Y.n.X.
+00000e50: 5700 6400 740c 6a0d 8300 8201 5800 6400  W.d.t.j.....X.d.
+00000e60: 5300 2908 4e7a 1344 6174 6162 6173 6520  S.).Nz.Database 
+00000e70: 636f 6e6e 6563 7469 6f6e 7238 0000 00da  connectionr8....
+00000e80: 0770 726f 6a65 6374 da05 746f 6b65 6e29  .project..token)
+00000e90: 0372 3800 0000 7255 0000 0072 5600 0000  .r8...rU...rV...
+00000ea0: 6300 0000 0000 0000 0001 0000 0003 0000  c...............
+00000eb0: 0013 0000 0073 2e00 0000 8804 6a00 8803  .....s......j...
+00000ec0: 8301 0100 8804 6a01 6a02 8800 8803 6602  ......j.j.....f.
+00000ed0: 8801 9e02 8802 8e01 7d00 8804 6a03 8803  ........}...j...
+00000ee0: 8301 0100 7c00 5300 2901 4e29 0472 3300  ....|.S.).N).r3.
+00000ef0: 0000 7232 0000 00da 0864 6973 7061 7463  ..r2.....dispatc
+00000f00: 6872 3400 0000 2901 da06 7265 7375 6c74  hr4...)...result
+00000f10: 2905 da06 6163 7469 6f6e 7253 0000 0072  )...actionrS...r
+00000f20: 4d00 0000 7218 0000 0072 1b00 0000 7215  M...r....r....r.
+00000f30: 0000 0072 1600 0000 da07 6578 6563 7574  ...r......execut
+00000f40: 6579 0000 0073 0800 0000 0001 0a01 1601  ey...s..........
+00000f50: 0a01 7a29 4261 7365 5669 6577 4861 6e64  ..z)BaseViewHand
+00000f60: 6c65 722e 6469 7370 6174 6368 2e3c 6c6f  ler.dispatch.<lo
+00000f70: 6361 6c73 3e2e 6578 6563 7574 6529 0e72  cals>.execute).r
+00000f80: 3100 0000 7202 0000 0072 0400 0000 da0b  1...r....r......
+00000f90: 7365 745f 636f 6e74 6578 7472 4900 0000  set_contextrI...
+00000fa0: 720b 0000 0072 4700 0000 724a 0000 00da  r....rG...rJ....
+00000fb0: 0373 7973 7248 0000 0072 3200 0000 724b  .sysrH...r2...rK
+00000fc0: 0000 0072 0500 0000 723f 0000 0029 0a72  ...r....r?...).r
+00000fd0: 1b00 0000 7259 0000 0072 5300 0000 724d  ....rY...rS...rM
+00000fe0: 0000 00da 0a63 6f6e 6e65 6374 696f 6e72  .....connectionr
+00000ff0: 5a00 0000 7246 0000 0072 4e00 0000 724f  Z...rF...rN...rO
+00001000: 0000 0072 5000 0000 7215 0000 0029 0572  ...rP...r....).r
+00001010: 5900 0000 7253 0000 0072 4d00 0000 7218  Y...rS...rM...r.
+00001020: 0000 0072 1b00 0000 7216 0000 0072 5700  ...r....r....rW.
+00001030: 0000 6b00 0000 7322 0000 0000 0208 0208  ..k...s"........
+00001040: 0104 0106 0108 0108 0112 030c 0214 0604  ................
+00001050: 010a 0110 010e 010e 0112 0116 027a 1842  .............z.B
+00001060: 6173 6556 6965 7748 616e 646c 6572 2e64  aseViewHandler.d
+00001070: 6973 7061 7463 6863 0100 0000 0000 0000  ispatchc........
+00001080: 0300 0000 0300 0000 4f00 0000 7310 0000  ........O...s...
+00001090: 007c 006a 0064 027c 019e 027c 028e 0153  .|.j.d.|...|...S
+000010a0: 0029 034e 7249 0000 0029 0172 4900 0000  .).NrI...).rI...
+000010b0: 2901 7257 0000 0029 0372 1b00 0000 7253  ).rW...).r....rS
+000010c0: 0000 0072 4d00 0000 7215 0000 0072 1500  ...rM...r....r..
+000010d0: 0000 7216 0000 0072 4900 0000 8900 0000  ..r....rI.......
+000010e0: 7302 0000 0000 017a 1342 6173 6556 6965  s......z.BaseVie
+000010f0: 7748 616e 646c 6572 2e67 6574 6301 0000  wHandler.getc...
+00001100: 0000 0000 0003 0000 0003 0000 004f 0000  .............O..
+00001110: 0073 1000 0000 7c00 6a00 6402 7c01 9e02  .s....|.j.d.|...
+00001120: 7c02 8e01 5300 2903 4eda 0470 6f73 7429  |...S.).N..post)
+00001130: 0172 5e00 0000 2901 7257 0000 0029 0372  .r^...).rW...).r
+00001140: 1b00 0000 7253 0000 0072 4d00 0000 7215  ....rS...rM...r.
+00001150: 0000 0072 1500 0000 7216 0000 0072 5e00  ...r....r....r^.
+00001160: 0000 8c00 0000 7302 0000 0000 017a 1442  ......s......z.B
+00001170: 6173 6556 6965 7748 616e 646c 6572 2e70  aseViewHandler.p
+00001180: 6f73 7463 0100 0000 0000 0000 0300 0000  ostc............
+00001190: 0300 0000 4f00 0000 7310 0000 007c 006a  ....O...s....|.j
+000011a0: 0064 027c 019e 027c 028e 0153 0029 034e  .d.|...|...S.).N
+000011b0: da03 7075 7429 0172 5f00 0000 2901 7257  ..put).r_...).rW
+000011c0: 0000 0029 0372 1b00 0000 7253 0000 0072  ...).r....rS...r
+000011d0: 4d00 0000 7215 0000 0072 1500 0000 7216  M...r....r....r.
+000011e0: 0000 0072 5f00 0000 8f00 0000 7302 0000  ...r_.......s...
+000011f0: 0000 017a 1342 6173 6556 6965 7748 616e  ...z.BaseViewHan
+00001200: 646c 6572 2e70 7574 6301 0000 0000 0000  dler.putc.......
+00001210: 0003 0000 0003 0000 004f 0000 0073 1000  .........O...s..
+00001220: 0000 7c00 6a00 6402 7c01 9e02 7c02 8e01  ..|.j.d.|...|...
+00001230: 5300 2903 4eda 0570 6174 6368 2901 7260  S.).N..patch).r`
+00001240: 0000 0029 0172 5700 0000 2903 721b 0000  ...).rW...).r...
+00001250: 0072 5300 0000 724d 0000 0072 1500 0000  .rS...rM...r....
+00001260: 7215 0000 0072 1600 0000 7260 0000 0092  r....r....r`....
+00001270: 0000 0073 0200 0000 0001 7a15 4261 7365  ...s......z.Base
+00001280: 5669 6577 4861 6e64 6c65 722e 7061 7463  ViewHandler.patc
+00001290: 6863 0100 0000 0000 0000 0300 0000 0300  hc..............
+000012a0: 0000 4f00 0000 7310 0000 007c 006a 0064  ..O...s....|.j.d
+000012b0: 027c 019e 027c 028e 0153 0029 034e da06  .|...|...S.).N..
+000012c0: 6465 6c65 7465 2901 7261 0000 0029 0172  delete).ra...).r
+000012d0: 5700 0000 2903 721b 0000 0072 5300 0000  W...).r....rS...
+000012e0: 724d 0000 0072 1500 0000 7215 0000 0072  rM...r....r....r
+000012f0: 1600 0000 7261 0000 0095 0000 0073 0200  ....ra.......s..
+00001300: 0000 0001 7a16 4261 7365 5669 6577 4861  ....z.BaseViewHa
+00001310: 6e64 6c65 722e 6465 6c65 7465 2916 da08  ndler.delete)...
+00001320: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00001330: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00001340: 5f5f 7232 0000 0072 1c00 0000 7226 0000  __r2...r....r&..
+00001350: 0072 3100 0000 7233 0000 0072 3400 0000  .r1...r3...r4...
+00001360: 7235 0000 0072 3a00 0000 7205 0000 00da  r5...r:...r.....
+00001370: 0963 6f72 6f75 7469 6e65 7247 0000 0072  .coroutinerG...r
+00001380: 5200 0000 7254 0000 0072 5700 0000 7249  R...rT...rW...rI
+00001390: 0000 0072 5e00 0000 725f 0000 0072 6000  ...r^...r_...r`.
+000013a0: 0000 7261 0000 0072 1500 0000 7215 0000  ..ra...r....r...
+000013b0: 0072 1500 0000 7216 0000 0072 0d00 0000  .r....r....r....
+000013c0: 1200 0000 7322 0000 0008 0104 0208 0308  ....s"..........
+000013d0: 0808 1208 0308 0308 0308 040e 160e 1208  ................
+000013e0: 040e 1e08 0308 0308 0308 0372 0d00 0000  ...........r....
+000013f0: 6301 0000 0000 0000 0002 0000 0004 0000  c...............
+00001400: 0003 0000 0073 1800 0000 4700 8700 6601  .....s....G...f.
+00001410: 6401 6402 8408 6402 7400 8303 7d01 7c01  d.d...d.t...}.|.
+00001420: 5300 2903 4e63 0000 0000 0000 0000 0000  S.).Nc..........
+00001430: 0000 0100 0000 0000 0000 7312 0000 0065  ..........s....e
+00001440: 005a 0164 005a 0294 0083 005a 0364 0153  .Z.d.Z.....Z.d.S
+00001450: 0029 027a 2176 6965 775f 6861 6e64 6c65  .).z!view_handle
+00001460: 722e 3c6c 6f63 616c 733e 2e56 6965 7748  r.<locals>.ViewH
+00001470: 616e 646c 6572 4e29 0472 6200 0000 7263  andlerN).rb...rc
+00001480: 0000 0072 6400 0000 7232 0000 0072 1500  ...rd...r2...r..
+00001490: 0000 2901 da03 636c 7372 1500 0000 7216  ..)...clsr....r.
+000014a0: 0000 00da 0b56 6965 7748 616e 646c 6572  .....ViewHandler
+000014b0: 9a00 0000 7302 0000 0008 0172 6700 0000  ....s......rg...
+000014c0: 2901 720d 0000 0029 0272 6600 0000 7267  ).r....).rf...rg
+000014d0: 0000 0072 1500 0000 2901 7266 0000 0072  ...r....).rf...r
+000014e0: 1600 0000 da0c 7669 6577 5f68 616e 646c  ......view_handl
+000014f0: 6572 9900 0000 7304 0000 0000 0114 0372  er....s........r
+00001500: 6800 0000 291c 725c 0000 00da 0b74 6f72  h...).r\.....tor
+00001510: 6e61 646f 2e77 6562 da07 746f 726e 6164  nado.web..tornad
+00001520: 6fda 126a 6574 5f62 7269 6467 655f 6261  o..jet_bridge_ba
+00001530: 7365 2e64 6272 0200 0000 5a28 6a65 745f  se.dbr....Z(jet_
+00001540: 6272 6964 6765 5f62 6173 652e 6578 6365  bridge_base.exce
+00001550: 7074 696f 6e73 2e72 6571 7565 7374 5f65  ptions.request_e
+00001560: 7272 6f72 7203 0000 00da 166a 6574 5f62  rrorr......jet_b
+00001570: 7269 6467 655f 6261 7365 2e73 656e 7472  ridge_base.sentr
+00001580: 7972 0400 0000 7205 0000 00da 1673 6978  yr....r......six
+00001590: 2e6d 6f76 6573 2e75 726c 6c69 625f 7061  .moves.urllib_pa
+000015a0: 7273 6572 0600 0000 5a17 6a65 745f 6272  rser....Z.jet_br
+000015b0: 6964 6765 5f62 6173 652e 7265 7175 6573  idge_base.reques
+000015c0: 7472 0700 0000 da22 6a65 745f 6272 6964  tr....."jet_brid
+000015d0: 6765 5f62 6173 652e 7265 7370 6f6e 7365  ge_base.response
+000015e0: 732e 7265 6469 7265 6374 7208 0000 00da  s.redirectr.....
+000015f0: 226a 6574 5f62 7269 6467 655f 6261 7365  "jet_bridge_base
+00001600: 2e72 6573 706f 6e73 6573 2e74 656d 706c  .responses.templ
+00001610: 6174 6572 0900 0000 5a16 6a65 745f 6272  ater....Z.jet_br
+00001620: 6964 6765 5f62 6173 652e 7374 6174 7573  idge_base.status
+00001630: 720a 0000 00da 206a 6574 5f62 7269 6467  r..... jet_bridg
+00001640: 655f 6261 7365 2e75 7469 6c73 2e61 7379  e_base.utils.asy
+00001650: 6e63 5f65 7865 6372 0b00 0000 5a10 746f  nc_execr....Z.to
+00001660: 726e 6164 6f2e 696f 7374 7265 616d 720c  rnado.iostreamr.
+00001670: 0000 00da 0377 6562 da0e 5265 7175 6573  .....web..Reques
+00001680: 7448 616e 646c 6572 720d 0000 0072 6800  tHandlerr....rh.
+00001690: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
+000016a0: 0072 1600 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000016b0: 0100 0000 731e 0000 0008 0208 010c 010c  ....s...........
+000016c0: 010c 010c 010c 020c 010c 010c 010c 010c  ................
+000016d0: 010c 0314 7f00 08                        .......
```

### Comparing `jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc` & `jet-bridge-1.8.2/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/jet_bridge/handlers/view.py` & `jet-bridge-1.8.2/jet_bridge/handlers/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+
 import tornado.web
 from jet_bridge_base.db import get_connection
 from jet_bridge_base.exceptions.request_error import RequestError
 from jet_bridge_base.sentry import sentry_controller
 from tornado import gen
 from six.moves.urllib_parse import parse_qs
 
@@ -118,17 +120,23 @@
 
         def execute():
             self.before_dispatch(request)
             result = self.view.dispatch(action, request, *args, **kwargs)
             self.after_dispatch(request)
             return result
 
-        response = yield as_future(execute)
-        yield self.write_response(response)
-        raise gen.Return()
+        try:
+            response = yield as_future(execute)
+            yield self.write_response(response)
+        except Exception:
+            exc_type, exc, traceback = sys.exc_info()
+            response = self.view.error_response(request, exc_type, exc, traceback)
+            yield self.write_response(response)
+        finally:
+            raise gen.Return()
 
     def get(self, *args, **kwargs):
         return self.dispatch('get', *args, **kwargs)
 
     def post(self, *args, **kwargs):
         return self.dispatch('post', *args, **kwargs)
```

### Comparing `jet-bridge-1.7.9/jet_bridge/jet_bridge_store.sqlite3` & `jet-bridge-1.8.2/jet_bridge/jet_bridge_store.sqlite3`

 * *Files 14% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -112,9 +112,16 @@
 INSERT INTO model_relation_override VALUES(125,'b94dba766915db55d04e43a38ad492ba1ab70f05799b0e45fb01cb4df76fba05','survicate_survicate_report_survey_export_daa9c072d06d651b',1,'email__to__repl_users_user__email','MANYTOONE','email','repl_users_user','email');
 INSERT INTO model_relation_override VALUES(126,'b94dba766915db55d04e43a38ad492ba1ab70f05799b0e45fb01cb4df76fba05','jet_notion_ticket',1,'reporter_email_text__to__repl_users_user__email','MANYTOONE','reporter_email_text','repl_users_user','email');
 INSERT INTO model_relation_override VALUES(127,'b94dba766915db55d04e43a38ad492ba1ab70f05799b0e45fb01cb4df76fba05','repl_projects_automation',1,'environment_id__to__repl_projects_environment__id','MANYTOONE','environment_id','repl_projects_environment','id');
 INSERT INTO model_relation_override VALUES(128,'b94dba766915db55d04e43a38ad492ba1ab70f05799b0e45fb01cb4df76fba05','repl_projects_automation',1,'project_id__to__repl_projects_project__id','MANYTOONE','project_id','repl_projects_project','id');
 INSERT INTO model_relation_override VALUES(129,'32414af7d38202c26acf22ccd6e0416cb348cf991a7a6e815522c493a40a4992','dev_LOCATIONS',1,'company__to__dev_COMPANY____jet_pk__','MANYTOONE','company','dev_COMPANY','__jet_pk__');
 INSERT INTO model_relation_override VALUES(130,'32414af7d38202c26acf22ccd6e0416cb348cf991a7a6e815522c493a40a4992','dev_COMPANY',1,'dev_LOCATIONS__company__to____jet_pk__','ONETOMANY','__jet_pk__','dev_LOCATIONS','company');
 INSERT INTO model_relation_override VALUES(131,'502f0a1cbef3e38fac78a2913cc11a7567d7ac9db529794cc2f341664063fdae','user',1,'groupId__to__test.group__id','MANYTOONE','groupId','test.group','id');
+INSERT INTO model_relation_override VALUES(132,'b12968d400623aebb96751b11372056fd3a5c63ffafd659b3d775461e0d8a7e6','posts',1,'creator_user_id__to__auth.users__id','MANYTOONE','creator_user_id','auth.users','id');
+INSERT INTO model_relation_override VALUES(133,'b12968d400623aebb96751b11372056fd3a5c63ffafd659b3d775461e0d8a7e6','auth.users',1,'posts__creator_user_id__to__id','ONETOMANY','id','posts','creator_user_id');
+INSERT INTO model_relation_override VALUES(134,'b12968d400623aebb96751b11372056fd3a5c63ffafd659b3d775461e0d8a7e6','playlists',1,'user_id__to__auth.users__id','MANYTOONE','user_id','auth.users','id');
+INSERT INTO model_relation_override VALUES(135,'200adbaaad949a9db266df353e124cb8998d6b84fe61b580b03102eee939227c','awards_comments',1,'__parent____to__awards____jet_item_pk__','MANYTOONE','__parent__','awards','__jet_item_pk__');
+INSERT INTO model_relation_override VALUES(136,'200adbaaad949a9db266df353e124cb8998d6b84fe61b580b03102eee939227c','awards',1,'awards_comments____parent____to____jet_item_pk__','ONETOMANY','__jet_item_pk__','awards_comments','__parent__');
+INSERT INTO model_relation_override VALUES(137,'200adbaaad949a9db266df353e124cb8998d6b84fe61b580b03102eee939227c','persons',1,'persons_comments____parent____to____jet_item_pk__','ONETOMANY','__jet_item_pk__','persons_comments','__parent__');
+INSERT INTO model_relation_override VALUES(138,'200adbaaad949a9db266df353e124cb8998d6b84fe61b580b03102eee939227c','persons_comments',1,'__parent____to__persons____jet_item_pk__','MANYTOONE','__parent__','persons','__jet_item_pk__');
 CREATE INDEX model_draft ON model_relation_override (connection_id, model, draft);
 COMMIT;
```

### Comparing `jet-bridge-1.7.9/README.md` & `jet-bridge-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.9/setup.py` & `jet-bridge-1.8.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return file.read()
 
 
 def get_install_requires():
     install_requires = [
         'tornado==5.1.1',
         'six',
-        'jet-bridge-base==1.7.9',
+        'jet-bridge-base==1.8.2',
         'paramiko==2.8.1',
         'sshtunnel',
     ]
 
     return install_requires
 
 setup(
```

