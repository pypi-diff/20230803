# Comparing `tmp/rfit-0.3.20230712.tar.gz` & `tmp/rfit-0.3.20230803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfit-0.3.20230712.tar", last modified: Tue Jul 11 14:31:30 2023, max compression
+gzip compressed data, was "rfit-0.3.20230803.tar", last modified: Thu Aug  3 20:37:18 2023, max compression
```

## Comparing `rfit-0.3.20230712.tar` & `rfit-0.3.20230803.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.338324 rfit-0.3.20230712/
--rw-r--r--   0 elo        (503) staff       (20)     1065 2023-07-11 14:19:49.000000 rfit-0.3.20230712/LICENSE
--rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 14:31:30.338467 rfit-0.3.20230712/PKG-INFO
--rw-r--r--   0 elo        (503) staff       (20)      346 2023-07-11 14:30:33.000000 rfit-0.3.20230712/README.md
--rw-r--r--   0 elo        (503) staff       (20)       84 2023-07-11 14:19:49.000000 rfit-0.3.20230712/pyproject.toml
--rw-r--r--   0 elo        (503) staff       (20)      697 2023-07-11 14:31:30.339106 rfit-0.3.20230712/setup.cfg
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.331164 rfit-0.3.20230712/src/
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.334062 rfit-0.3.20230712/src/rfit/
--rw-r--r--   0 elo        (503) staff       (20)      363 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/__init__.py
--rw-r--r--   0 elo        (503) staff       (20)     2225 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/api.py
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.337710 rfit-0.3.20230712/src/rfit/learn/
--rw-r--r--   0 elo        (503) staff       (20)      304 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/learn/__init__.py
--rwxr-xr-x   0 elo        (503) staff       (20)     4749 2023-07-11 14:19:49.000000 rfit-0.3.20230712/src/rfit/learn/boundary_plots.py
--rwxr-xr-x   0 elo        (503) staff       (20)     1432 2023-07-11 14:29:18.000000 rfit-0.3.20230712/src/rfit/learn/helper.py
-drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-07-11 14:31:30.336462 rfit-0.3.20230712/src/rfit.egg-info/
--rw-r--r--   0 elo        (503) staff       (20)      861 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/PKG-INFO
--rw-r--r--   0 elo        (503) staff       (20)      323 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/SOURCES.txt
--rw-r--r--   0 elo        (503) staff       (20)        1 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/dependency_links.txt
--rw-r--r--   0 elo        (503) staff       (20)       33 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/requires.txt
--rw-r--r--   0 elo        (503) staff       (20)        5 2023-07-11 14:31:30.000000 rfit-0.3.20230712/src/rfit.egg-info/top_level.txt
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-08-03 20:37:18.396706 rfit-0.3.20230803/
+-rw-r--r--   0 elo        (503) staff       (20)     1065 2023-07-11 14:39:42.000000 rfit-0.3.20230803/LICENSE
+-rw-r--r--   0 elo        (503) staff       (20)      861 2023-08-03 20:37:18.396932 rfit-0.3.20230803/PKG-INFO
+-rw-r--r--   0 elo        (503) staff       (20)      346 2023-08-03 20:33:48.000000 rfit-0.3.20230803/README.md
+-rw-r--r--   0 elo        (503) staff       (20)       84 2023-07-11 14:39:42.000000 rfit-0.3.20230803/pyproject.toml
+-rw-r--r--   0 elo        (503) staff       (20)      714 2023-08-03 20:37:18.398106 rfit-0.3.20230803/setup.cfg
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-08-03 20:37:18.387096 rfit-0.3.20230803/src/
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-08-03 20:37:18.391281 rfit-0.3.20230803/src/rfit/
+-rw-r--r--   0 elo        (503) staff       (20)      363 2023-07-11 14:39:42.000000 rfit-0.3.20230803/src/rfit/__init__.py
+-rw-r--r--   0 elo        (503) staff       (20)     2225 2023-07-11 14:39:42.000000 rfit-0.3.20230803/src/rfit/api.py
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-08-03 20:37:18.395882 rfit-0.3.20230803/src/rfit/learn/
+-rw-r--r--   0 elo        (503) staff       (20)      304 2023-07-11 14:39:42.000000 rfit-0.3.20230803/src/rfit/learn/__init__.py
+-rwxr-xr-x   0 elo        (503) staff       (20)     4749 2023-07-11 14:39:42.000000 rfit-0.3.20230803/src/rfit/learn/boundary_plots.py
+-rwxr-xr-x   0 elo        (503) staff       (20)     1432 2023-07-11 14:39:42.000000 rfit-0.3.20230803/src/rfit/learn/helper.py
+drwxr-xr-x   0 elo        (503) staff       (20)        0 2023-08-03 20:37:18.393872 rfit-0.3.20230803/src/rfit.egg-info/
+-rw-r--r--   0 elo        (503) staff       (20)      861 2023-08-03 20:37:18.000000 rfit-0.3.20230803/src/rfit.egg-info/PKG-INFO
+-rw-r--r--   0 elo        (503) staff       (20)      323 2023-08-03 20:37:18.000000 rfit-0.3.20230803/src/rfit.egg-info/SOURCES.txt
+-rw-r--r--   0 elo        (503) staff       (20)        1 2023-08-03 20:37:18.000000 rfit-0.3.20230803/src/rfit.egg-info/dependency_links.txt
+-rw-r--r--   0 elo        (503) staff       (20)       49 2023-08-03 20:37:18.000000 rfit-0.3.20230803/src/rfit.egg-info/requires.txt
+-rw-r--r--   0 elo        (503) staff       (20)        5 2023-08-03 20:37:18.000000 rfit-0.3.20230803/src/rfit.egg-info/top_level.txt
```

### Comparing `rfit-0.3.20230712/LICENSE` & `rfit-0.3.20230803/LICENSE`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230712/PKG-INFO` & `rfit-0.3.20230803/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rfit
-Version: 0.3.20230712
+Version: 0.3.20230803
 Summary: GWU Data Science python class helper functions
 Home-page: https://github.com/physicsland/rfitapi
 Author: Edwin Lo
 Author-email: elo@regression.fit
 Project-URL: Bug Tracker, https://github.com/physicsland/rfitapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Regression.fit api
 
-Last updated: 2023-07-12
+Last updated: 2023-08-03
 
 This package (rfit - regression.fit) is for use at The George Washington University Data Science program. There are some useful and convenient functions we use in our python classes. 
 
 One of them is dfapi, which connects to the api.regression.fit endpoint, to load dataframes used in our classes.
```

### Comparing `rfit-0.3.20230712/setup.cfg` & `rfit-0.3.20230803/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rfit
-version = 0.3.20230712
+version = 0.3.20230803
 author = Edwin Lo
 author_email = elo@regression.fit
 description = GWU Data Science python class helper functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/physicsland/rfitapi
 project_urls = 
@@ -20,14 +20,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
 	matplotlib
 	pandas
 	requests
+	mysql.connector
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rfit-0.3.20230712/src/rfit/api.py` & `rfit-0.3.20230803/src/rfit/api.py`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230712/src/rfit/learn/boundary_plots.py` & `rfit-0.3.20230803/src/rfit/learn/boundary_plots.py`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230712/src/rfit/learn/helper.py` & `rfit-0.3.20230803/src/rfit/learn/helper.py`

 * *Files identical despite different names*

### Comparing `rfit-0.3.20230712/src/rfit.egg-info/PKG-INFO` & `rfit-0.3.20230803/src/rfit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rfit
-Version: 0.3.20230712
+Version: 0.3.20230803
 Summary: GWU Data Science python class helper functions
 Home-page: https://github.com/physicsland/rfitapi
 Author: Edwin Lo
 Author-email: elo@regression.fit
 Project-URL: Bug Tracker, https://github.com/physicsland/rfitapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Regression.fit api
 
-Last updated: 2023-07-12
+Last updated: 2023-08-03
 
 This package (rfit - regression.fit) is for use at The George Washington University Data Science program. There are some useful and convenient functions we use in our python classes. 
 
 One of them is dfapi, which connects to the api.regression.fit endpoint, to load dataframes used in our classes.
```

