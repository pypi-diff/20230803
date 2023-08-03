# Comparing `tmp/apisql-0.3.2.tar.gz` & `tmp/apisql-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apisql-0.3.2.tar", last modified: Mon Jul 31 11:24:21 2023, max compression
+gzip compressed data, was "apisql-0.3.3.tar", last modified: Thu Aug  3 09:51:48 2023, max compression
```

## Comparing `apisql-0.3.2.tar` & `apisql-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:24:21.797768 apisql-0.3.2/
--rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.3.2/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.3.2/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.3.2/Makefile
--rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:24:21.797946 apisql-0.3.2/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.3.2/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:24:21.791808 apisql-0.3.2/apisql/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-31 11:23:53.000000 apisql-0.3.2/apisql/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.3.2/apisql/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     5421 2023-07-31 11:04:14.000000 apisql-0.3.2/apisql/blueprint.py
--rw-r--r--   0 adam       (501) staff       (20)     4893 2023-07-31 11:23:48.000000 apisql-0.3.2/apisql/controllers.py
--rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.3.2/apisql/logger.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:24:21.796978 apisql-0.3.2/apisql/utils/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.3.2/apisql/utils/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.3.2/apisql/utils/file_maker.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:24:21.795997 apisql-0.3.2/apisql.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:24:21.000000 apisql-0.3.2/apisql.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      380 2023-07-31 11:24:21.000000 apisql-0.3.2/apisql.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-31 11:24:21.000000 apisql-0.3.2/apisql.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.3.2/apisql.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)      156 2023-07-31 11:24:21.000000 apisql-0.3.2/apisql.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-31 11:24:21.000000 apisql-0.3.2/apisql.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-07-31 11:24:21.798609 apisql-0.3.2/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1815 2023-07-31 11:11:42.000000 apisql-0.3.2/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-03 09:51:48.011676 apisql-0.3.3/
+-rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.3.3/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.3.3/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.3.3/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-08-03 09:51:48.011842 apisql-0.3.3/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.3.3/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-03 09:51:48.006278 apisql-0.3.3/apisql/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-08-03 09:51:24.000000 apisql-0.3.3/apisql/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.3.3/apisql/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     5421 2023-07-31 11:04:14.000000 apisql-0.3.3/apisql/blueprint.py
+-rw-r--r--   0 adam       (501) staff       (20)     4899 2023-08-03 09:51:04.000000 apisql-0.3.3/apisql/controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.3.3/apisql/logger.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-03 09:51:48.010902 apisql-0.3.3/apisql/utils/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.3.3/apisql/utils/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.3.3/apisql/utils/file_maker.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-03 09:51:48.009624 apisql-0.3.3/apisql.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-08-03 09:51:47.000000 apisql-0.3.3/apisql.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      380 2023-08-03 09:51:47.000000 apisql-0.3.3/apisql.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-08-03 09:51:47.000000 apisql-0.3.3/apisql.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.3.3/apisql.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)      156 2023-08-03 09:51:47.000000 apisql-0.3.3/apisql.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-08-03 09:51:47.000000 apisql-0.3.3/apisql.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-08-03 09:51:48.012501 apisql-0.3.3/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1815 2023-07-31 11:11:42.000000 apisql-0.3.3/setup.py
```

### Comparing `apisql-0.3.2/LICENSE` & `apisql-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apisql-0.3.2/PKG-INFO` & `apisql-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.3.2
+Version: 0.3.3
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apisql-0.3.2/README.md` & `apisql-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `apisql-0.3.2/apisql/blueprint.py` & `apisql-0.3.3/apisql/blueprint.py`

 * *Files identical despite different names*

### Comparing `apisql-0.3.2/apisql/controllers.py` & `apisql-0.3.3/apisql/controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def query_db_streaming(self, query_str, formatters):
         try:
             headers, formatters = self.parse_formatters(formatters)
 
             with self.engine.connect() as connection:
                 logger.debug('executing %r', query_str)
                 result = connection.execution_options(stream_results=True)\
-                    .execute(query_str)
+                    .execute(text(query_str))
                 yield headers
                 yield from (
                     [f(row) for f in formatters]
                     for row in map(self.jsonable, map(dict, result))
                 )
         except Exception:
             logger.exception('EXC')
```

### Comparing `apisql-0.3.2/apisql/utils/file_maker.py` & `apisql-0.3.3/apisql/utils/file_maker.py`

 * *Files identical despite different names*

### Comparing `apisql-0.3.2/apisql.egg-info/PKG-INFO` & `apisql-0.3.3/apisql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.3.2
+Version: 0.3.3
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apisql-0.3.2/setup.py` & `apisql-0.3.3/setup.py`

 * *Files identical despite different names*

