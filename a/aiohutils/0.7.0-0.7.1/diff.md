# Comparing `tmp/aiohutils-0.7.0.tar.gz` & `tmp/aiohutils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohutils-0.7.0.tar", last modified: Thu Aug  3 07:41:48 2023, max compression
+gzip compressed data, was "aiohutils-0.7.1.tar", last modified: Thu Aug  3 07:50:35 2023, max compression
```

## Comparing `aiohutils-0.7.0.tar` & `aiohutils-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:41:48.345554 aiohutils-0.7.0/
--rw-rw-rw-   0        0        0      503 2023-08-03 07:41:48.344552 aiohutils-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-08-03 06:55:23.000000 aiohutils-0.7.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-03 07:41:48.329594 aiohutils-0.7.0/aiohutils/
--rw-rw-rw-   0        0        0       22 2023-08-03 07:41:45.000000 aiohutils-0.7.0/aiohutils/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-08-03 07:39:47.000000 aiohutils-0.7.0/aiohutils/session.py
--rw-rw-rw-   0        0        0     2956 2023-08-03 07:04:03.000000 aiohutils-0.7.0/aiohutils/tests.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:41:48.343557 aiohutils-0.7.0/aiohutils.egg-info/
--rw-rw-rw-   0        0        0      503 2023-08-03 07:41:48.000000 aiohutils-0.7.0/aiohutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 07:41:48.000000 aiohutils-0.7.0/aiohutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:41:48.000000 aiohutils-0.7.0/aiohutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-08-03 07:41:48.000000 aiohutils-0.7.0/aiohutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 07:41:48.000000 aiohutils-0.7.0/aiohutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.7.0/aiohutils.egg-info/zip-safe
--rw-rw-rw-   0        0        0      967 2023-08-03 07:01:19.000000 aiohutils-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 07:41:48.345554 aiohutils-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 07:50:35.333392 aiohutils-0.7.1/
+-rw-rw-rw-   0        0        0      503 2023-08-03 07:50:35.332394 aiohutils-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-08-03 06:55:23.000000 aiohutils-0.7.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-03 07:50:35.312448 aiohutils-0.7.1/aiohutils/
+-rw-rw-rw-   0        0        0       22 2023-08-03 07:50:32.000000 aiohutils-0.7.1/aiohutils/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-08-03 07:39:47.000000 aiohutils-0.7.1/aiohutils/session.py
+-rw-rw-rw-   0        0        0     2946 2023-08-03 07:49:19.000000 aiohutils-0.7.1/aiohutils/tests.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:50:35.331397 aiohutils-0.7.1/aiohutils.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.7.1/aiohutils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      967 2023-08-03 07:01:19.000000 aiohutils-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:50:35.333392 aiohutils-0.7.1/setup.cfg
```

### Comparing `aiohutils-0.7.0/aiohutils/session.py` & `aiohutils-0.7.1/aiohutils/session.py`

 * *Files identical despite different names*

### Comparing `aiohutils-0.7.0/aiohutils/tests.py` & `aiohutils-0.7.1/aiohutils/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             with open(FakeResponse().file, 'wb') as f:
                 f.write(content)
             return resp
 
         sm.get = recording_get
 
     yield
-    await sm.close()
+    return
 
 
 @fixture(scope='session')
 def event_loop():
     loop = new_event_loop()
     yield loop
     loop.close()
```

### Comparing `aiohutils-0.7.0/pyproject.toml` & `aiohutils-0.7.1/pyproject.toml`

 * *Files identical despite different names*

