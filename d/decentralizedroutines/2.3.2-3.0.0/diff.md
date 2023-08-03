# Comparing `tmp/decentralizedroutines-2.3.2.tar.gz` & `tmp/decentralizedroutines-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.3.2.tar", last modified: Wed Aug  2 09:49:45 2023, max compression
+gzip compressed data, was "decentralizedroutines-3.0.0.tar", last modified: Thu Aug  3 11:13:10 2023, max compression
```

## Comparing `decentralizedroutines-2.3.2.tar` & `decentralizedroutines-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:49:45.039029 decentralizedroutines-2.3.2/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.3.2/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-08-02 09:49:45.039029 decentralizedroutines-2.3.2/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.3.2/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.3.2/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-08-02 09:49:45.039029 decentralizedroutines-2.3.2/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:49:45.039029 decentralizedroutines-2.3.2/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:49:45.039029 decentralizedroutines-2.3.2/src/decentralizedroutines/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/__init__.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      699 2023-07-31 11:46:47.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/master.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/runroutines.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:43:01.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/update_version_requirements.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/worker.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.3.2/src/decentralizedroutines/worker_lib.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:49:45.039029 decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-08-02 09:49:45.000000 decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-08-02 09:49:45.000000 decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 09:49:45.000000 decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-08-02 09:49:45.000000 decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-08-02 09:49:45.000000 decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:13:10.638285 decentralizedroutines-3.0.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-3.0.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-08-03 11:13:10.638285 decentralizedroutines-3.0.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-3.0.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-3.0.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-08-03 11:13:10.638285 decentralizedroutines-3.0.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:13:10.638285 decentralizedroutines-3.0.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:13:10.638285 decentralizedroutines-3.0.0/src/decentralizedroutines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      699 2023-07-31 11:46:47.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/master.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/runroutines.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:43:01.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-3.0.0/src/decentralizedroutines/worker_lib.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:13:10.638285 decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-08-03 11:13:10.000000 decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-08-03 11:13:10.000000 decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-03 11:13:10.000000 decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-08-03 11:13:10.000000 decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-08-03 11:13:10.000000 decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.3.2/LICENSE` & `decentralizedroutines-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/PKG-INFO` & `decentralizedroutines-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.3.2
+Version: 3.0.0
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.3.2/setup.cfg` & `decentralizedroutines-3.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = decentralizedroutines
-version = 2.3.2
+version = 3.0.0
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Master/Worker implementation of decentralized git published routines and kinesis worker pool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/DecentralizedRoutines
 project_urls = 
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	shareddata==2.3.2
+	shareddata==3.0.0
 	psutil==5.9.5
 	tzlocal==4.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/RoutineScheduler.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/defaults.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/defaults.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/master.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/master.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/runroutines.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/update_version_requirements.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/update_version_requirements.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/worker.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/worker.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-3.0.0/src/decentralizedroutines/worker_lib.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.3.2
+Version: 3.0.0
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.3.2/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-3.0.0/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

