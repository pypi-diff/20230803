# Comparing `tmp/predibase-api-2023.7.9.tar.gz` & `tmp/predibase-api-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2023.7.9.tar", last modified: Wed Jul 19 04:40:19 2023, max compression
+gzip compressed data, was "predibase-api-2023.8.1.tar", last modified: Thu Aug  3 01:12:09 2023, max compression
```

## Comparing `predibase-api-2023.7.9.tar` & `predibase-api-2023.8.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:39:48.000000 predibase-api-2023.7.9/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:40:06.000000 predibase-api-2023.7.9/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.479126 predibase-api-2023.8.1/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.483126 predibase-api-2023.8.1/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.483126 predibase-api-2023.8.1/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.483126 predibase-api-2023.8.1/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.483126 predibase-api-2023.8.1/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.483126 predibase-api-2023.8.1/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.483126 predibase-api-2023.8.1/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.479126 predibase-api-2023.8.1/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 01:12:09.000000 predibase-api-2023.8.1/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-03 01:12:09.000000 predibase-api-2023.8.1/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:12:09.000000 predibase-api-2023.8.1/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:11:41.000000 predibase-api-2023.8.1/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 01:12:09.000000 predibase-api-2023.8.1/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 01:12:09.000000 predibase-api-2023.8.1/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:12:09.487126 predibase-api-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-03 01:11:11.000000 predibase-api-2023.8.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 01:12:01.000000 predibase-api-2023.8.1/version.txt
```

### Comparing `predibase-api-2023.7.9/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2023.8.1/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2023.8.1/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2023.8.1/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2023.8.1/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2023.8.1/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2023.8.1/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2023.8.1/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.9/setup.py` & `predibase-api-2023.8.1/setup.py`

 * *Files identical despite different names*

