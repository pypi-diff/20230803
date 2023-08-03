# Comparing `tmp/pysimplebase-0.0.6.tar.gz` & `tmp/pysimplebase-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimplebase-0.0.6.tar", last modified: Wed Aug  2 08:12:23 2023, max compression
+gzip compressed data, was "pysimplebase-0.0.7.tar", last modified: Thu Aug  3 04:06:26 2023, max compression
```

## Comparing `pysimplebase-0.0.6.tar` & `pysimplebase-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:12:23.695044 pysimplebase-0.0.6/
--rw-rw-rw-   0        0        0    35162 2022-12-05 10:38:56.000000 pysimplebase-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3936 2023-08-02 08:12:23.694046 pysimplebase-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3432 2023-08-02 05:48:07.000000 pysimplebase-0.0.6/README.rst
--rw-rw-rw-   0        0        0      663 2023-08-02 08:11:53.000000 pysimplebase-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-02 08:12:23.677116 pysimplebase-0.0.6/pysimplebase/
--rw-rw-rw-   0        0        0      105 2023-08-01 06:46:33.000000 pysimplebase-0.0.6/pysimplebase/__init__.py
--rw-rw-rw-   0        0        0    75061 2023-08-01 08:32:15.000000 pysimplebase-0.0.6/pysimplebase/pysimplebase.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:12:23.693072 pysimplebase-0.0.6/pysimplebase.egg-info/
--rw-rw-rw-   0        0        0     3936 2023-08-02 08:12:23.000000 pysimplebase-0.0.6/pysimplebase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-02 08:12:23.000000 pysimplebase-0.0.6/pysimplebase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:12:23.000000 pysimplebase-0.0.6/pysimplebase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:12:23.000000 pysimplebase-0.0.6/pysimplebase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-02 08:12:23.000000 pysimplebase-0.0.6/pysimplebase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 08:12:23.695044 pysimplebase-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 04:06:26.373576 pysimplebase-0.0.7/
+-rw-rw-rw-   0        0        0    35162 2022-12-05 10:38:56.000000 pysimplebase-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3949 2023-08-03 04:06:26.372578 pysimplebase-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3445 2023-08-03 04:05:55.000000 pysimplebase-0.0.7/README.rst
+-rw-rw-rw-   0        0        0      649 2023-08-03 04:03:37.000000 pysimplebase-0.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-03 04:06:26.353629 pysimplebase-0.0.7/pysimplebase/
+-rw-rw-rw-   0        0        0      105 2023-08-01 06:46:33.000000 pysimplebase-0.0.7/pysimplebase/__init__.py
+-rw-rw-rw-   0        0        0    75061 2023-08-01 08:32:15.000000 pysimplebase-0.0.7/pysimplebase/pysimplebase.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:06:26.371582 pysimplebase-0.0.7/pysimplebase.egg-info/
+-rw-rw-rw-   0        0        0     3949 2023-08-03 04:06:26.000000 pysimplebase-0.0.7/pysimplebase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-03 04:06:26.000000 pysimplebase-0.0.7/pysimplebase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 04:06:26.000000 pysimplebase-0.0.7/pysimplebase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 04:06:26.000000 pysimplebase-0.0.7/pysimplebase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 04:06:26.000000 pysimplebase-0.0.7/pysimplebase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 04:06:26.373576 pysimplebase-0.0.7/setup.cfg
```

### Comparing `pysimplebase-0.0.6/LICENSE` & `pysimplebase-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pysimplebase-0.0.6/PKG-INFO` & `pysimplebase-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: pysimplebase
-Version: 0.0.6
+Version: 0.0.7
 Summary: High performance JSON-oriented database
 Author-email: Dmitry Vorontsov <dv1555@hotmail.com>
 Project-URL: Homepage, https://simplebase.readthedocs.io/en/latest/#
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-SimpleBase is a JSON based serverless database with improved performance on key operations
+SimpleBase is a lightweight JSON based serverless database with improved performance on key operations
 
-The strength of document-oriented NoSQL DBMS is their natural simplicity, but they are usually not very fast (unless they are serious server DBMS like MongoDB). SimpleBase fixes performance issues in critical areas
+The strength of document-oriented NoSQL database is their natural simplicity, but they are usually not very fast (unless they are serious server databases like MongoDB). SimpleBase solves performance issues in critical areas
 
- * **Instant addition** of new records to collections, regardless of the size of the collection due to a special storage architecture
- * Faster work with operations, due to the fact that it is **not required to encode / decode the entire collection** (which can be very large)
- * Collections are always **stored in RAM** with concurrency change tracking: data is re-read from disk only if it has been changed by another process
- * **ACID for multi-user and multi-threading**
- * Two types of indexes for key types of queries - a **hash index** and a **special B-tree** for full-text search
- * Support for **transactions** (sessions)
- * MongoDB-like syntax, incl. 100% similar query language
- * Written in **pure python**, only about 1800 lines
+* **Instant addition** of new records to collections, regardless of the size of the collection due to a special storage architecture
+* Faster work with operations, due to the fact that it is **not required to encode / decode the entire collection** (which can be very large)
+* Collections are always **stored in RAM** with concurrency change tracking: data is re-read from disk only if it has been changed by another process
+* **ACID for multi-user and multi-threading**
+* Two types of indexes for key types of queries - a **hash index** and a **special B-tree** for full-text search
+* Support for **transactions** (sessions)
+* MongoDB-like syntax, incl. 100% similar query language
+* Written in **pure python**, only about 1800 lines
 
 Why SimpleBase?
 ------------------
 
 It was written for situations where you need to organize a local database without a server with a JSON-oriented interface. But at the same time, increased performance requirements: for large collections (1000000+ documents in the collection), fast, almost instantaneous execution of some operations is required:
 
- * Add a new document to the collection with 1000000 documents - 0.007 seconds, with 2000000 documents - also 0.0007 seconds - ie. operation time does not depend on the size of the table
- * Find an element by equality in a collection with 1000000+ entries in 1-2 microseconds
- * Organize real-time search by occurrence of a string across a large collection without friezes
+* Add a new document to the collection with 1000000 documents - 0.007 seconds, with 2000000 documents - also 0.0007 seconds - ie. operation time does not depend on the size of the table
+* Find an element by equality in a collection with 1000000+ entries in 1-2 microseconds
+* Organize real-time search by occurrence of a string across a large collection without friezes
 
 
 .. code-block:: Python
 
-  from simplebase import SimpleBase,DBSession
+  from pysimplebase import SimpleBase,DBSession
   
   #creatig database
   db = SimpleBase("samples_db")
   
   #inserting documents into collection
   id = db['goods'].insert({"name":"coffee", "price":15}) #insert one document
   print(db['goods'].get(id))
```

### Comparing `pysimplebase-0.0.6/README.rst` & `pysimplebase-0.0.7/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-SimpleBase is a JSON based serverless database with improved performance on key operations
+SimpleBase is a lightweight JSON based serverless database with improved performance on key operations
 
-The strength of document-oriented NoSQL DBMS is their natural simplicity, but they are usually not very fast (unless they are serious server DBMS like MongoDB). SimpleBase fixes performance issues in critical areas
+The strength of document-oriented NoSQL database is their natural simplicity, but they are usually not very fast (unless they are serious server databases like MongoDB). SimpleBase solves performance issues in critical areas
 
- * **Instant addition** of new records to collections, regardless of the size of the collection due to a special storage architecture
- * Faster work with operations, due to the fact that it is **not required to encode / decode the entire collection** (which can be very large)
- * Collections are always **stored in RAM** with concurrency change tracking: data is re-read from disk only if it has been changed by another process
- * **ACID for multi-user and multi-threading**
- * Two types of indexes for key types of queries - a **hash index** and a **special B-tree** for full-text search
- * Support for **transactions** (sessions)
- * MongoDB-like syntax, incl. 100% similar query language
- * Written in **pure python**, only about 1800 lines
+* **Instant addition** of new records to collections, regardless of the size of the collection due to a special storage architecture
+* Faster work with operations, due to the fact that it is **not required to encode / decode the entire collection** (which can be very large)
+* Collections are always **stored in RAM** with concurrency change tracking: data is re-read from disk only if it has been changed by another process
+* **ACID for multi-user and multi-threading**
+* Two types of indexes for key types of queries - a **hash index** and a **special B-tree** for full-text search
+* Support for **transactions** (sessions)
+* MongoDB-like syntax, incl. 100% similar query language
+* Written in **pure python**, only about 1800 lines
 
 Why SimpleBase?
 ------------------
 
 It was written for situations where you need to organize a local database without a server with a JSON-oriented interface. But at the same time, increased performance requirements: for large collections (1000000+ documents in the collection), fast, almost instantaneous execution of some operations is required:
 
- * Add a new document to the collection with 1000000 documents - 0.007 seconds, with 2000000 documents - also 0.0007 seconds - ie. operation time does not depend on the size of the table
- * Find an element by equality in a collection with 1000000+ entries in 1-2 microseconds
- * Organize real-time search by occurrence of a string across a large collection without friezes
+* Add a new document to the collection with 1000000 documents - 0.007 seconds, with 2000000 documents - also 0.0007 seconds - ie. operation time does not depend on the size of the table
+* Find an element by equality in a collection with 1000000+ entries in 1-2 microseconds
+* Organize real-time search by occurrence of a string across a large collection without friezes
 
 
 .. code-block:: Python
 
-  from simplebase import SimpleBase,DBSession
+  from pysimplebase import SimpleBase,DBSession
   
   #creatig database
   db = SimpleBase("samples_db")
   
   #inserting documents into collection
   id = db['goods'].insert({"name":"coffee", "price":15}) #insert one document
   print(db['goods'].get(id))
```

### Comparing `pysimplebase-0.0.6/pyproject.toml` & `pysimplebase-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysimplebase"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Dmitry Vorontsov", email="dv1555@hotmail.com" },
 ]
 description = "High performance JSON-oriented database"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "filelock",
-  "hashlib",
   "msgspec"
 ]
 
 
 [project.urls]
 "Homepage" = "https://simplebase.readthedocs.io/en/latest/#"
```

### Comparing `pysimplebase-0.0.6/pysimplebase/pysimplebase.py` & `pysimplebase-0.0.7/pysimplebase/pysimplebase.py`

 * *Files identical despite different names*

### Comparing `pysimplebase-0.0.6/pysimplebase.egg-info/PKG-INFO` & `pysimplebase-0.0.7/pysimplebase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: pysimplebase
-Version: 0.0.6
+Version: 0.0.7
 Summary: High performance JSON-oriented database
 Author-email: Dmitry Vorontsov <dv1555@hotmail.com>
 Project-URL: Homepage, https://simplebase.readthedocs.io/en/latest/#
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-SimpleBase is a JSON based serverless database with improved performance on key operations
+SimpleBase is a lightweight JSON based serverless database with improved performance on key operations
 
-The strength of document-oriented NoSQL DBMS is their natural simplicity, but they are usually not very fast (unless they are serious server DBMS like MongoDB). SimpleBase fixes performance issues in critical areas
+The strength of document-oriented NoSQL database is their natural simplicity, but they are usually not very fast (unless they are serious server databases like MongoDB). SimpleBase solves performance issues in critical areas
 
- * **Instant addition** of new records to collections, regardless of the size of the collection due to a special storage architecture
- * Faster work with operations, due to the fact that it is **not required to encode / decode the entire collection** (which can be very large)
- * Collections are always **stored in RAM** with concurrency change tracking: data is re-read from disk only if it has been changed by another process
- * **ACID for multi-user and multi-threading**
- * Two types of indexes for key types of queries - a **hash index** and a **special B-tree** for full-text search
- * Support for **transactions** (sessions)
- * MongoDB-like syntax, incl. 100% similar query language
- * Written in **pure python**, only about 1800 lines
+* **Instant addition** of new records to collections, regardless of the size of the collection due to a special storage architecture
+* Faster work with operations, due to the fact that it is **not required to encode / decode the entire collection** (which can be very large)
+* Collections are always **stored in RAM** with concurrency change tracking: data is re-read from disk only if it has been changed by another process
+* **ACID for multi-user and multi-threading**
+* Two types of indexes for key types of queries - a **hash index** and a **special B-tree** for full-text search
+* Support for **transactions** (sessions)
+* MongoDB-like syntax, incl. 100% similar query language
+* Written in **pure python**, only about 1800 lines
 
 Why SimpleBase?
 ------------------
 
 It was written for situations where you need to organize a local database without a server with a JSON-oriented interface. But at the same time, increased performance requirements: for large collections (1000000+ documents in the collection), fast, almost instantaneous execution of some operations is required:
 
- * Add a new document to the collection with 1000000 documents - 0.007 seconds, with 2000000 documents - also 0.0007 seconds - ie. operation time does not depend on the size of the table
- * Find an element by equality in a collection with 1000000+ entries in 1-2 microseconds
- * Organize real-time search by occurrence of a string across a large collection without friezes
+* Add a new document to the collection with 1000000 documents - 0.007 seconds, with 2000000 documents - also 0.0007 seconds - ie. operation time does not depend on the size of the table
+* Find an element by equality in a collection with 1000000+ entries in 1-2 microseconds
+* Organize real-time search by occurrence of a string across a large collection without friezes
 
 
 .. code-block:: Python
 
-  from simplebase import SimpleBase,DBSession
+  from pysimplebase import SimpleBase,DBSession
   
   #creatig database
   db = SimpleBase("samples_db")
   
   #inserting documents into collection
   id = db['goods'].insert({"name":"coffee", "price":15}) #insert one document
   print(db['goods'].get(id))
```

