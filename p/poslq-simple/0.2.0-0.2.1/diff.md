# Comparing `tmp/poslq_simple-0.2.0.tar.gz` & `tmp/poslq_simple-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poslq_simple-0.2.0.tar", last modified: Tue Aug  1 19:17:11 2023, max compression
+gzip compressed data, was "poslq_simple-0.2.1.tar", last modified: Thu Aug  3 01:01:56 2023, max compression
```

## Comparing `poslq_simple-0.2.0.tar` & `poslq_simple-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-08-01 16:11:42.000000 poslq_simple-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3436 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2912 2023-08-01 19:12:02.000000 poslq_simple-0.2.0/README.md
--rw-rw-rw-   0        0        0      611 2023-08-01 19:13:26.000000 poslq_simple-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.061864 poslq_simple-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.086370 poslq_simple-0.2.0/src/poslq_simple.egg-info/
--rw-rw-rw-   0        0        0     3436 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/src/posql_simple/
--rw-rw-rw-   0        0        0        0 2023-08-01 16:11:42.000000 poslq_simple-0.2.0/src/posql_simple/__init__.py
--rw-rw-rw-   0        0        0     5738 2023-08-01 19:10:49.000000 poslq_simple-0.2.0/src/posql_simple/w_out_sql.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:01:56.075601 poslq_simple-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3394 2023-08-03 01:01:56.075601 poslq_simple-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2023-07-16 19:45:03.000000 poslq_simple-0.2.1/README.md
+-rw-rw-rw-   0        0        0      611 2023-08-03 01:01:34.000000 poslq_simple-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 01:01:56.075601 poslq_simple-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 01:01:56.051716 poslq_simple-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 01:01:56.071771 poslq_simple-0.2.1/src/poslq_simple.egg-info/
+-rw-rw-rw-   0        0        0     3394 2023-08-03 01:01:56.000000 poslq_simple-0.2.1/src/poslq_simple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-08-03 01:01:56.000000 poslq_simple-0.2.1/src/poslq_simple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 01:01:56.000000 poslq_simple-0.2.1/src/poslq_simple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 01:01:56.000000 poslq_simple-0.2.1/src/poslq_simple.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 01:01:56.074769 poslq_simple-0.2.1/src/posql_simple/
+-rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.2.1/src/posql_simple/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-08-03 00:49:47.000000 poslq_simple-0.2.1/src/posql_simple/test.py
+-rw-rw-rw-   0        0        0     5739 2023-08-03 00:49:47.000000 poslq_simple-0.2.1/src/posql_simple/w_out_sql.py
```

### Comparing `poslq_simple-0.2.0/LICENSE` & `poslq_simple-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.2.0/PKG-INFO` & `poslq_simple-0.2.1/src/poslq_simple.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: poslq_simple
-Version: 0.2.0
+Name: poslq-simple
+Version: 0.2.1
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
 if the transaction is OK, and false if it's not ok ).
 Each object is **padded** with the "_id" entry ( uuid generated string ).
-You can add your own custom "_id" entry ( or _id is a fully generated new uuid4 ).
+You can add your own custom "_id" entry.
 
 ``delete_by_id`` method takes one positional param which is the id ( making a linear search ). Like the ``add_record`` method, it returns a boolean.
 
 ``find_by_id`` same as ``delete_by_id`` ; returning **deep copy** of the dict ( avoid mutability ) or else None.
 
 ``update_obj`` : takes two positional args : new_obj ( the obj to persist, must contain an "_id" entry , or else throwing an error ),
 returning a bool.
```

### Comparing `poslq_simple-0.2.0/README.md` & `poslq_simple-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
 if the transaction is OK, and false if it's not ok ).
 Each object is **padded** with the "_id" entry ( uuid generated string ).
-You can add your own custom "_id" entry ( or _id is a fully generated new uuid4 ).
+You can add your own custom "_id" entry.
 
 ``delete_by_id`` method takes one positional param which is the id ( making a linear search ). Like the ``add_record`` method, it returns a boolean.
 
 ``find_by_id`` same as ``delete_by_id`` ; returning **deep copy** of the dict ( avoid mutability ) or else None.
 
 ``update_obj`` : takes two positional args : new_obj ( the obj to persist, must contain an "_id" entry , or else throwing an error ),
 returning a bool.
```

### Comparing `poslq_simple-0.2.0/pyproject.toml` & `poslq_simple-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "poslq_simple"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="enyos", email="lebedevhh@outlook.fr" },
 ]
 description = "A simple nosql json storage for small projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `poslq_simple-0.2.0/src/poslq_simple.egg-info/PKG-INFO` & `poslq_simple-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: poslq-simple
-Version: 0.2.0
+Name: poslq_simple
+Version: 0.2.1
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
 if the transaction is OK, and false if it's not ok ).
 Each object is **padded** with the "_id" entry ( uuid generated string ).
-You can add your own custom "_id" entry ( or _id is a fully generated new uuid4 ).
+You can add your own custom "_id" entry.
 
 ``delete_by_id`` method takes one positional param which is the id ( making a linear search ). Like the ``add_record`` method, it returns a boolean.
 
 ``find_by_id`` same as ``delete_by_id`` ; returning **deep copy** of the dict ( avoid mutability ) or else None.
 
 ``update_obj`` : takes two positional args : new_obj ( the obj to persist, must contain an "_id" entry , or else throwing an error ),
 returning a bool.
```

### Comparing `poslq_simple-0.2.0/src/posql_simple/w_out_sql.py` & `poslq_simple-0.2.1/src/posql_simple/w_out_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return "path : {path_name}, collections : {coll}".format( path_name = self.path, coll = self.__data )
 
     def bind_new_collection(self, collection ):
         self.__data[collection.collect_name] = collection.get_all_slot()
         self.save()
 
     def get_collection(self, coll_name : str ):
-        if ( col_name in list(self.__data.keys())):
+        if ( coll_name in list(self.__data.keys())):
             return Collection( coll_name, self.__data[coll_name])
         else :
             print ( "[INFO] this is collection doesn't exist")
             print ( "[INFO] created new collection into {db_name}, with name {coll_name}".format(db_name = self.path, coll_name = coll_name))
             result = Collection( coll_name )
             self.bind_new_collection( result )
             return result
```

