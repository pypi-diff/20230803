# Comparing `tmp/acryl-PyHive-0.6.8.tar.gz` & `tmp/acryl-PyHive-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryl-PyHive-0.6.8.tar", last modified: Tue Jun 29 23:52:20 2021, max compression
+gzip compressed data, was "acryl-PyHive-0.6.9.tar", last modified: Tue Jun 29 23:53:17 2021, max compression
```

## Comparing `acryl-PyHive-0.6.8.tar` & `acryl-PyHive-0.6.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:52:20.968221 acryl-PyHive-0.6.8/
--rw-r--r--   0 hsheth     (502) staff       (20)      558 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/LICENSE
--rw-r--r--   0 hsheth     (502) staff       (20)       16 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/MANIFEST.in
--rw-r--r--   0 hsheth     (502) staff       (20)     6392 2021-06-29 23:52:20.968345 acryl-PyHive-0.6.8/PKG-INFO
--rw-r--r--   0 hsheth     (502) staff       (20)     5812 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/README.rst
-drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:52:20.957382 acryl-PyHive-0.6.8/TCLIService/
--rw-r--r--   0 hsheth     (502) staff       (20)   131364 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/TCLIService/TCLIService.py
--rw-r--r--   0 hsheth     (502) staff       (20)       49 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/TCLIService/__init__.py
--rw-r--r--   0 hsheth     (502) staff       (20)     1087 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/TCLIService/constants.py
--rw-r--r--   0 hsheth     (502) staff       (20)   263044 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/TCLIService/ttypes.py
-drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:52:20.962528 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/
--rw-r--r--   0 hsheth     (502) staff       (20)     6392 2021-06-29 23:52:20.000000 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/PKG-INFO
--rw-r--r--   0 hsheth     (502) staff       (20)      544 2021-06-29 23:52:20.000000 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/SOURCES.txt
--rw-r--r--   0 hsheth     (502) staff       (20)        1 2021-06-29 23:52:20.000000 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/dependency_links.txt
--rw-r--r--   0 hsheth     (502) staff       (20)      262 2021-06-29 23:52:20.000000 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/entry_points.txt
--rw-r--r--   0 hsheth     (502) staff       (20)      200 2021-06-29 23:52:20.000000 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/requires.txt
--rw-r--r--   0 hsheth     (502) staff       (20)       19 2021-06-29 23:52:20.000000 acryl-PyHive-0.6.8/acryl_PyHive.egg-info/top_level.txt
-drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:52:20.967452 acryl-PyHive-0.6.8/pyhive/
--rw-r--r--   0 hsheth     (502) staff       (20)      101 2021-06-29 23:51:46.000000 acryl-PyHive-0.6.8/pyhive/__init__.py
--rw-r--r--   0 hsheth     (502) staff       (20)     9248 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/common.py
--rw-r--r--   0 hsheth     (502) staff       (20)     2196 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/exc.py
--rw-r--r--   0 hsheth     (502) staff       (20)    23739 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/hive.py
--rw-r--r--   0 hsheth     (502) staff       (20)    15262 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/presto.py
--rw-r--r--   0 hsheth     (502) staff       (20)    14465 2021-06-29 23:48:57.000000 acryl-PyHive-0.6.8/pyhive/sqlalchemy_hive.py
--rw-r--r--   0 hsheth     (502) staff       (20)     7388 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/sqlalchemy_presto.py
--rw-r--r--   0 hsheth     (502) staff       (20)     1926 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/sqlalchemy_trino.py
--rw-r--r--   0 hsheth     (502) staff       (20)     4834 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/pyhive/trino.py
--rw-r--r--   0 hsheth     (502) staff       (20)      878 2021-06-29 23:52:20.968940 acryl-PyHive-0.6.8/setup.cfg
--rwxr-xr-x   0 hsheth     (502) staff       (20)     2304 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.8/setup.py
+drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:53:17.006195 acryl-PyHive-0.6.9/
+-rw-r--r--   0 hsheth     (502) staff       (20)      558 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/LICENSE
+-rw-r--r--   0 hsheth     (502) staff       (20)       16 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/MANIFEST.in
+-rw-r--r--   0 hsheth     (502) staff       (20)     6392 2021-06-29 23:53:17.006307 acryl-PyHive-0.6.9/PKG-INFO
+-rw-r--r--   0 hsheth     (502) staff       (20)     5812 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/README.rst
+drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:53:16.999820 acryl-PyHive-0.6.9/TCLIService/
+-rw-r--r--   0 hsheth     (502) staff       (20)   131364 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/TCLIService/TCLIService.py
+-rw-r--r--   0 hsheth     (502) staff       (20)       49 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/TCLIService/__init__.py
+-rw-r--r--   0 hsheth     (502) staff       (20)     1087 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/TCLIService/constants.py
+-rw-r--r--   0 hsheth     (502) staff       (20)   263044 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/TCLIService/ttypes.py
+drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:53:17.002509 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/
+-rw-r--r--   0 hsheth     (502) staff       (20)     6392 2021-06-29 23:53:16.000000 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/PKG-INFO
+-rw-r--r--   0 hsheth     (502) staff       (20)      544 2021-06-29 23:53:16.000000 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/SOURCES.txt
+-rw-r--r--   0 hsheth     (502) staff       (20)        1 2021-06-29 23:53:16.000000 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/dependency_links.txt
+-rw-r--r--   0 hsheth     (502) staff       (20)      262 2021-06-29 23:53:16.000000 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/entry_points.txt
+-rw-r--r--   0 hsheth     (502) staff       (20)      200 2021-06-29 23:53:16.000000 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/requires.txt
+-rw-r--r--   0 hsheth     (502) staff       (20)       19 2021-06-29 23:53:16.000000 acryl-PyHive-0.6.9/acryl_PyHive.egg-info/top_level.txt
+drwxr-xr-x   0 hsheth     (502) staff       (20)        0 2021-06-29 23:53:17.005674 acryl-PyHive-0.6.9/pyhive/
+-rw-r--r--   0 hsheth     (502) staff       (20)      101 2021-06-29 23:53:03.000000 acryl-PyHive-0.6.9/pyhive/__init__.py
+-rw-r--r--   0 hsheth     (502) staff       (20)     9248 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/common.py
+-rw-r--r--   0 hsheth     (502) staff       (20)     2196 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/exc.py
+-rw-r--r--   0 hsheth     (502) staff       (20)    23739 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/hive.py
+-rw-r--r--   0 hsheth     (502) staff       (20)    15262 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/presto.py
+-rw-r--r--   0 hsheth     (502) staff       (20)    14444 2021-06-29 23:52:49.000000 acryl-PyHive-0.6.9/pyhive/sqlalchemy_hive.py
+-rw-r--r--   0 hsheth     (502) staff       (20)     7388 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/sqlalchemy_presto.py
+-rw-r--r--   0 hsheth     (502) staff       (20)     1926 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/sqlalchemy_trino.py
+-rw-r--r--   0 hsheth     (502) staff       (20)     4834 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/pyhive/trino.py
+-rw-r--r--   0 hsheth     (502) staff       (20)      878 2021-06-29 23:53:17.006816 acryl-PyHive-0.6.9/setup.cfg
+-rwxr-xr-x   0 hsheth     (502) staff       (20)     2304 2021-06-29 23:03:57.000000 acryl-PyHive-0.6.9/setup.py
```

### Comparing `acryl-PyHive-0.6.8/LICENSE` & `acryl-PyHive-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/PKG-INFO` & `acryl-PyHive-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-PyHive
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python interface to Hive
 Home-page: https://github.com/hsheth2/PyHive
 Author: Jing Wang
 Author-email: jing@dropbox.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `acryl-PyHive-0.6.8/README.rst` & `acryl-PyHive-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/TCLIService/TCLIService.py` & `acryl-PyHive-0.6.9/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/TCLIService/constants.py` & `acryl-PyHive-0.6.9/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/TCLIService/ttypes.py` & `acryl-PyHive-0.6.9/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/acryl_PyHive.egg-info/PKG-INFO` & `acryl-PyHive-0.6.9/acryl_PyHive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-PyHive
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python interface to Hive
 Home-page: https://github.com/hsheth2/PyHive
 Author: Jing Wang
 Author-email: jing@dropbox.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `acryl-PyHive-0.6.8/acryl_PyHive.egg-info/SOURCES.txt` & `acryl-PyHive-0.6.9/acryl_PyHive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/common.py` & `acryl-PyHive-0.6.9/pyhive/common.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/exc.py` & `acryl-PyHive-0.6.9/pyhive/exc.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/hive.py` & `acryl-PyHive-0.6.9/pyhive/hive.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/presto.py` & `acryl-PyHive-0.6.9/pyhive/presto.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/sqlalchemy_hive.py` & `acryl-PyHive-0.6.9/pyhive/sqlalchemy_hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,15 +389,14 @@
             elif col_name != "" and data_type is not None:
                 properties[col_name] = data_type.strip()
             else:
                 # col_name == "", data_type is not None
                 prop_name = "{} {}".format(active_heading, data_type.rstrip())
                 properties[prop_name] = value.rstrip()
         
-        breakpoint()
         return {'text': properties.get('Table Parameters: comment', None), 'properties': properties}
 
     def do_rollback(self, dbapi_connection):
         # No transactions for Hive
         pass
 
     def _check_unicode_returns(self, connection, additional_tests=None):
```

### Comparing `acryl-PyHive-0.6.8/pyhive/sqlalchemy_presto.py` & `acryl-PyHive-0.6.9/pyhive/sqlalchemy_presto.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/sqlalchemy_trino.py` & `acryl-PyHive-0.6.9/pyhive/sqlalchemy_trino.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/pyhive/trino.py` & `acryl-PyHive-0.6.9/pyhive/trino.py`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/setup.cfg` & `acryl-PyHive-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `acryl-PyHive-0.6.8/setup.py` & `acryl-PyHive-0.6.9/setup.py`

 * *Files identical despite different names*

