# Comparing `tmp/psyqlepg-0.0.6.tar.gz` & `tmp/psyqlepg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyqlepg-0.0.6.tar", last modified: Tue Jul 25 13:49:13 2023, max compression
+gzip compressed data, was "psyqlepg-0.0.7.tar", last modified: Thu Aug  3 05:45:57 2023, max compression
```

## Comparing `psyqlepg-0.0.6.tar` & `psyqlepg-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.712839 psyqlepg-0.0.6/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.6/LICENSE
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-25 13:49:13.711839 psyqlepg-0.0.6/PKG-INFO
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      219 2023-07-19 09:40:34.000000 psyqlepg-0.0.6/README.md
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-07-25 13:48:58.000000 psyqlepg-0.0.6/pyproject.toml
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-07-25 13:49:13.712839 psyqlepg-0.0.6/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.709839 psyqlepg-0.0.6/src/
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.710839 psyqlepg-0.0.6/src/psyqlepg/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     4593 2023-07-25 13:48:36.000000 psyqlepg-0.0.6/src/psyqlepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.711839 psyqlepg-0.0.6/src/psyqlepg.egg-info/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-08-03 05:45:57.560615 psyqlepg-0.0.7/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.7/LICENSE
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-08-03 05:45:57.559615 psyqlepg-0.0.7/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      219 2023-07-19 09:40:34.000000 psyqlepg-0.0.7/README.md
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-08-03 05:35:07.000000 psyqlepg-0.0.7/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-08-03 05:45:57.560615 psyqlepg-0.0.7/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-08-03 05:45:57.557615 psyqlepg-0.0.7/src/
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-08-03 05:45:57.558615 psyqlepg-0.0.7/src/psyqlepg/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     5268 2023-08-03 05:45:26.000000 psyqlepg-0.0.7/src/psyqlepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-08-03 05:45:57.559615 psyqlepg-0.0.7/src/psyqlepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-08-03 05:45:57.000000 psyqlepg-0.0.7/src/psyqlepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-08-03 05:45:57.000000 psyqlepg-0.0.7/src/psyqlepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-08-03 05:45:57.000000 psyqlepg-0.0.7/src/psyqlepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-08-03 05:45:57.000000 psyqlepg-0.0.7/src/psyqlepg.egg-info/top_level.txt
```

### Comparing `psyqlepg-0.0.6/LICENSE` & `psyqlepg-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psyqlepg-0.0.6/PKG-INFO` & `psyqlepg-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyqlepg
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple SQL library for psycopg3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/psyqlepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/psyqlepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `psyqlepg-0.0.6/src/psyqlepg/__init__.py` & `psyqlepg-0.0.7/src/psyqlepg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 class Where:
     def __init__(self, name=None, value=None):
         self.params = []
         self.args = []
         if (name):
             self.append(name, value)
 
-
     def append(self, name, value=None):
         if isinstance(name, sql.Composable):
             self.params.append(name)
         else:
             self.params.append(sql.SQL('{} = %s').format(sql.Identifier(name)))
             self.args.append(value)
         return self
@@ -21,14 +20,39 @@
     def clause(self):
         if not self.params:
             return sql.SQL('true').format()
 
         return sql.SQL('{params}').format(
             params=sql.SQL(' and ').join(self.params))
 
+    def as_string(self, context):
+        return self.clause().as_string(context)
+
+
+class List:
+    def __init__(self, value=None):
+        self.params = []
+        self.args = []
+        if (value):
+            self.append(value)
+
+    def append(self, value):
+        if isinstance(value, sql.Composable):
+            self.params.append(value)
+        elif isinstance(value, list):
+            for v in value:
+                self.append(v)
+        else:
+            self.params.append(sql.SQL('%s'))
+            self.args.append(value)
+        return self
+
+    def clause(self):
+        return sql.SQL('{params}').format(
+            params=sql.SQL(', ').join(self.params))
 
     def as_string(self, context):
         return self.clause().as_string(context)
 
 
 def selectone(conn, table, primary_key, identifier):
     query = sql.SQL('''
```

### Comparing `psyqlepg-0.0.6/src/psyqlepg.egg-info/PKG-INFO` & `psyqlepg-0.0.7/src/psyqlepg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyqlepg
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple SQL library for psycopg3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/psyqlepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/psyqlepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

