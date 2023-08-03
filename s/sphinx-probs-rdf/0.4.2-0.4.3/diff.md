# Comparing `tmp/sphinx_probs_rdf-0.4.2.tar.gz` & `tmp/sphinx_probs_rdf-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_probs_rdf-0.4.2.tar", last modified: Wed May 10 23:00:33 2023, max compression
+gzip compressed data, was "sphinx_probs_rdf-0.4.3.tar", last modified: Thu Aug  3 20:59:36 2023, max compression
```

## Comparing `sphinx_probs_rdf-0.4.2.tar` & `sphinx_probs_rdf-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.542753 sphinx_probs_rdf-0.4.2/
--rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/LICENSE
--rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/MANIFEST.in
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-10 23:00:33.542877 sphinx_probs_rdf-0.4.2/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/README.rst
--rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-05-10 23:00:33.543872 sphinx_probs_rdf-0.4.2/setup.cfg
--rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/setup.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.415589 sphinx_probs_rdf-0.4.2/src/
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.484474 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/
--rw-r--r--   0 rcl38      (502) staff       (20)     5539 2023-05-08 07:12:14.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/__init__.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.495337 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/_static/
--rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/_static/system-definitions.css
--rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/builder.py
--rw-r--r--   0 rcl38      (502) staff       (20)    30726 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/directives.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/resolve.py
--rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-05-10 22:59:13.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/version.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.490803 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/not-zip-safe
--rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/requires.txt
--rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/top_level.txt
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.542340 sphinx_probs_rdf-0.4.2/tests/
--rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_directive_options.py
--rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_missing_process.py
--rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_basic.py
--rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_myst.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_prefixes.py
--rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_system_directives.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-08-03 20:59:36.762868 sphinx_probs_rdf-0.4.3/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/LICENSE
+-rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/MANIFEST.in
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-08-03 20:59:36.762961 sphinx_probs_rdf-0.4.3/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/README.rst
+-rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-08-03 20:59:36.763609 sphinx_probs_rdf-0.4.3/setup.cfg
+-rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/setup.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-08-03 20:59:36.723728 sphinx_probs_rdf-0.4.3/src/
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-08-03 20:59:36.740630 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/
+-rw-r--r--   0 rcl38      (502) staff       (20)     5539 2023-05-08 07:12:14.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/__init__.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-08-03 20:59:36.746554 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/_static/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/_static/system-definitions.css
+-rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/builder.py
+-rw-r--r--   0 rcl38      (502) staff       (20)    30980 2023-08-01 16:29:28.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/directives.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/resolve.py
+-rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-08-03 20:59:05.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/version.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-08-03 20:59:36.744834 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-08-03 20:59:36.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-08-03 20:59:36.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-08-03 20:59:36.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-08-03 20:59:36.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/requires.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-08-03 20:59:36.000000 sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/top_level.txt
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-08-03 20:59:36.762603 sphinx_probs_rdf-0.4.3/tests/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/tests/test_directive_options.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/tests/test_missing_process.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/tests/test_postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.3/tests/test_probs_rdf_builder_basic.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.3/tests/test_probs_rdf_builder_myst.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.3/tests/test_probs_rdf_builder_prefixes.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.3/tests/test_probs_system_directives.py
```

### Comparing `sphinx_probs_rdf-0.4.2/LICENSE` & `sphinx_probs_rdf-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/PKG-INFO` & `sphinx_probs_rdf-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_probs_rdf
-Version: 0.4.2
+Version: 0.4.3
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.4.2/setup.py` & `sphinx_probs_rdf-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/__init__.py` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/_static/system-definitions.css` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/_static/system-definitions.css`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/builder.py` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/builder.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/directives.py` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/directives.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,14 +580,21 @@
             g.add((uri, PROBS.objectIsTraded, Literal(imp or exp)))
 
         if "equivalent" in self.options:
             for item in self.options["equivalent"]:
                 item_uri = self.parse_uri(item)
                 g.add((uri, PROBS.objectEquivalentTo, item_uri))
 
+        # Define a process which represents the balancing market / control
+        # volume for this object
+        process_uri = URIRef(str(uri) + "_Market")
+        g.add((process_uri, RDF.type, PROBS.Process))
+        g.add((process_uri, PROBS.marketForObject, uri))
+        g.add((process_uri, RDFS.label, Literal(label)))
+
     def parse_uri(self, item):
         """Convert a string to a URIRef.
 
         A blank prefix or bare id refers to the namespace given by the
         `probs_rdf_system_prefix` config variable.
 
         A missing suffix means the same as the object currently being defined.
@@ -631,25 +638,23 @@
         for obj_uri in objects:
             object_processes[obj_uri] = []
 
         # Add in all the places that an object is consumed or produced by a
         # process
         for process_uri, objs in process_recipe.items():
             if process_uri not in processes:
-                logger.error(
-                    "Process %s that %s object %s is not defined",
+                logger.warning(
+                    "Process %s is not defined",
                     process_uri,
-                    direction,
-                    obj_uri,
                     # location=(self.env.docname, self.lineno)
                 )
                 continue
             for obj_uri, direction in objs:
                 if obj_uri not in objects:
-                    logger.error(
+                    logger.warning(
                         "Object %s %s by process %s is not defined",
                         obj_uri,
                         direction[:-1] + "d",
                         process_uri,
                         # location=(self.env.docname, self.lineno)
                     )
                     continue
```

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/postprocess.py` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/resolve.py` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf/resolve.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/PKG-INFO` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-probs-rdf
-Version: 0.4.2
+Version: 0.4.3
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/SOURCES.txt` & `sphinx_probs_rdf-0.4.3/src/sphinx_probs_rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_directive_options.py` & `sphinx_probs_rdf-0.4.3/tests/test_directive_options.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_missing_process.py` & `sphinx_probs_rdf-0.4.3/tests/test_missing_process.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_postprocess.py` & `sphinx_probs_rdf-0.4.3/tests/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_basic.py` & `sphinx_probs_rdf-0.4.3/tests/test_probs_rdf_builder_basic.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_myst.py` & `sphinx_probs_rdf-0.4.3/tests/test_probs_rdf_builder_myst.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_prefixes.py` & `sphinx_probs_rdf-0.4.3/tests/test_probs_rdf_builder_prefixes.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.2/tests/test_probs_system_directives.py` & `sphinx_probs_rdf-0.4.3/tests/test_probs_system_directives.py`

 * *Files identical despite different names*

