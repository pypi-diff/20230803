# Comparing `tmp/triplets-0.0.3.tar.gz` & `tmp/triplets-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/triplets-0.0.3.tar", last modified: Thu Mar 23 05:40:23 2023, max compression
+gzip compressed data, was "dist/triplets-0.0.4.tar", last modified: Thu Aug  3 12:49:14 2023, max compression
```

## Comparing `triplets-0.0.3.tar` & `triplets-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:40:23.000000 triplets-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-23 05:40:10.000000 triplets-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-23 05:40:23.000000 triplets-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-23 05:40:10.000000 triplets-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-23 05:40:23.000000 triplets-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-23 05:40:10.000000 triplets-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-23 05:40:10.000000 triplets-0.0.3/triplets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-03-23 05:40:10.000000 triplets-0.0.3/triplets/cgmes_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-03-23 05:40:10.000000 triplets-0.0.3/triplets/rdf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-03-23 05:40:10.000000 triplets-0.0.3/triplets/rdfs_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 05:40:23.000000 triplets-0.0.3/triplets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-23 05:40:10.000000 triplets-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:49:14.000000 triplets-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 12:49:00.000000 triplets-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-03 12:49:14.000000 triplets-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 12:49:00.000000 triplets-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-03 12:49:14.000000 triplets-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 12:49:00.000000 triplets-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 12:49:01.000000 triplets-0.0.4/triplets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-08-03 12:49:01.000000 triplets-0.0.4/triplets/cgmes_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37936 2023-08-03 12:49:01.000000 triplets-0.0.4/triplets/rdf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-08-03 12:49:01.000000 triplets-0.0.4/triplets/rdfs_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 12:49:14.000000 triplets-0.0.4/triplets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-03 12:49:01.000000 triplets-0.0.4/versioneer.py
```

### Comparing `triplets-0.0.3/PKG-INFO` & `triplets-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplets
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple RDF tools to load/modify/export RDF data using Pandas DataFrames
 Home-page: https://github.com/Haigutus/rdf_tools
 Author: Kristjan Vilgo
 Author-email: kristjan.vilgo@gmail.com
 License: MIT
 Description: # RDF parser:
```

### Comparing `triplets-0.0.3/README.md` & `triplets-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `triplets-0.0.3/setup.py` & `triplets-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `triplets-0.0.3/triplets/cgmes_tools.py` & `triplets-0.0.4/triplets/cgmes_tools.py`

 * *Files identical despite different names*

### Comparing `triplets-0.0.3/triplets/rdf_parser.py` & `triplets-0.0.4/triplets/rdf_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 #
 # Author:      kristjan.vilgo
 #
 # Created:     13.12.2018
 # Copyright:   (c) kristjan.vilgo 2018
 # Licence:     GPLv2
 # -------------------------------------------------------------------------------
-
 from io import BytesIO
 import os
 
 from lxml import etree
 from lxml.builder import ElementMaker
 from lxml.etree import QName
 
 import pandas
-#import dask as pandas
 import datetime
 import zipfile
 import uuid
-import json
 
 from collections import OrderedDict
 
 # from collections import deque
 
 # from multiprocessing import Pool - TODO add parallel loading for import ALL DASK, SPARK, MODIN, VAEX
 
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 # pandas.set_option("display.height", 1000)
 pandas.set_option("display.max_rows", 18)
 pandas.set_option("display.max_columns", 8)
 pandas.set_option("display.width", 1000)
 
 
@@ -44,15 +45,15 @@
 def print_duration(text, start_time):
     """Print duration between now and start time
     Input: text, start_time
     Output: duration (in seconds), end_time"""
 
     end_time = datetime.datetime.now()
     duration = end_time - start_time
-    print(text, duration)
+    logger.debug(f"{text}  {duration}")
 
     return duration, end_time
 
 
 def remove_prefix(original_string, prefix_string):
     """Removes prefix from a string"""
 
@@ -109,30 +110,33 @@
     """Returns list of XML file objects and/or paths in ZIP file"""
 
     xml_files_list = []
     zip_files_list = []  # TODO - add support random folders as well
 
     for item in list_of_paths_to_zip_globalzip_xml:
 
-        item_lower = item.lower()
+        if type(item) == str:
+            item = open(item, "rb")
+
+        item_lower = item.name.lower()
 
         if ".xml" in item_lower or ".rdf" in item_lower:
             xml_files_list.append(item)
 
             if debug:
-                print("Added: {}".format(item))
+                logger.debug("Added: {}".format(item))
 
         elif ".zip" in item_lower:
             zip_files_list.append(item)
 
             if debug:
-                print("Added for further processing: {}".format(item))
+                logger.debug("Added for further processing: {}".format(item))
 
         else:
-            print("WARNING 1 - Not supported file: {}".format(item))
+            logger.warning("Not supported file: {}".format(item))
 
     for zip_file_path in zip_files_list:
 
         zip_container = zipfile.ZipFile(zip_file_path)
         zipped_files = zip_container.namelist()
 
         for zipped_file in zipped_files:
@@ -141,42 +145,43 @@
 
             if ".xml" in zipped_file_lower or ".rdf" in zipped_file_lower:
                 file_object = BytesIO(zip_container.read(zipped_file))
                 file_object.name = zipped_file
                 xml_files_list.append(file_object)
 
                 if debug:
-                    print("INFO - Added: {}".format(zipped_file))
+                    logger.debug("Added: {}".format(zipped_file))
 
             elif ".zip" in zipped_file_lower:
                 zip_files_list.append(BytesIO(zip_container.read(zipped_file)))
 
                 if debug:
-                    print("INFO - Added for further processing: {}".format(zipped_file))
+                    logger.debug("Added for further processing: {}".format(zipped_file))
 
             else:
-                print("WARNING - Not supported file: {}".format(zipped_file))
+                logger.warning("Not supported file: {}".format(zipped_file))
 
     return xml_files_list
 
 
 def load_RDF_to_list(path_or_fileobject, debug=False, keep_ns=False):
     """Parse single file to triplestore list"""
 
     file_name = path_or_fileobject
 
     if type(path_or_fileobject) != str:
         file_name = path_or_fileobject.name
 
-    print("INFO - Loading {}".format(file_name))
+    logger.info("Loading {}".format(file_name))
 
     RDF_objects, INSTANCE_ID = load_RDF_objects_from_XML(path_or_fileobject, debug)
 
     if debug:
         start_time = datetime.datetime.now()
+        start_time = datetime.datetime.now()
 
     # Lets generate list for RDF data and store the original filename under rdf:label in dcat:Distribution object
     ID = str(uuid.uuid4())
     data_list = [
                     (ID, "Type", "Distribution", INSTANCE_ID),
                     (ID, "label", file_name, INSTANCE_ID)
                 ]
@@ -256,15 +261,15 @@
         start_time = datetime.datetime.now()
 
     data = pandas.DataFrame(data_list, columns=["ID", "KEY", "VALUE", "INSTANCE_ID"])
 
     if debug:
         print_duration("Data list loaded to DataFrame", start_time)
         print_duration("All loaded in ", process_start)
-        # print(data.info())
+        # logger.debug(data.info())
 
     return data
 
 
 # Extend this functionality to pandas DataFrame
 pandas.read_RDF = load_all_to_dataframe
 
@@ -272,34 +277,60 @@
 def type_tableview(data, type_name, string_to_number=True):
     """Creates a table view of all objects of same type, with their parameters in columns"""
 
     # Get all ID-s of rows where Type == type_name
     type_id = data.query("VALUE == '{}' & KEY == 'Type'".format(type_name))
 
     if type_id.empty:
-        print('WARNING - No data available for {}'.format(type_name))
+        logger.warning('No data available for {}'.format(type_name))
         return None
 
     # Filter original data by found type_id data
-    type_data = pandas.merge(type_id[["ID"]], data, right_on="ID", left_on="ID").drop_duplicates(["ID",
-                                                                                                  "KEY"])  # There can't be duplicate ID and KEY pairs for pivot, but this will lose data on full model DependantOn and other info, solution would be to use pivot table function.
+    # There can't be duplicate ID and KEY pairs for pivot, but this will lose data on full model DependantOn and other info, solution would be to use pivot table function.
+    type_data = pandas.merge(type_id[["ID"]], data, right_on="ID", left_on="ID").drop_duplicates(["ID", "KEY"])
 
     # Convert form triplets to a table view all objects of same type
     data_view = type_data.pivot(index="ID", columns="KEY")["VALUE"]
 
     if string_to_number:
         # Convert to data type to numeric in columns that contain only numbers (for easier data usage later on)
         data_view = data_view.apply(pandas.to_numeric, errors='ignore')
 
     return data_view
 
-
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.type_tableview = type_tableview
 
+def key_tableview(data, key_name, string_to_number=True):
+    """Creates a table view of all objects of same type, with their parameters in columns"""
+
+    # Get all ID-s of rows where KEY == key_name
+    type_id = data.query("KEY == @key_name")
+
+    if type_id.empty:
+        logger.warning('No data available for {}'.format(key_name))
+        return None
+
+    # Filter original data by found type_id data
+    # There can't be duplicate ID and KEY pairs for pivot, but this will lose data on full model DependantOn and other info, solution would be to use pivot table function.
+    type_data = pandas.merge(type_id[["ID"]], data, right_on="ID", left_on="ID").drop_duplicates(["ID", "KEY"])
+
+    # Convert form triplets to a table view all objects of same type
+    data_view = type_data.pivot(index="ID", columns="KEY")["VALUE"]
+
+    if string_to_number:
+        # Convert to data type to numeric in columns that contain only numbers (for easier data usage later on)
+        data_view = data_view.apply(pandas.to_numeric, errors='ignore')
+
+    return data_view
+
+
+# Extend this functionality to pandas DataFrame
+pandas.DataFrame.key_tableview = key_tableview
+
 
 def references_to_simple(data, reference, columns=["Type"]):
     """Creates a table view of all elements that specified element refers to,
     by default returns two columns ID and Type, but this can be extended"""
 
     reference_data = data.references_to(reference, levels=1).drop_duplicates(["ID_FROM", "KEY"])
 
@@ -313,30 +344,29 @@
 pandas.DataFrame.references_to_simple = references_to_simple
 
 
 def references_to(data, reference, levels=1):
     """Return all object pointing towards reference object"""
 
     # TODO - add the key on which connection was made
+    level = 0
 
     # Get the object itself
-    object_data = data.query("ID == '{}'".format(reference)).copy()
-    object_data["level"] = 0
-    object_data["ID_FROM"] = reference
-
-    # Dataframe where to keep the results
-    objects_data = pandas.DataFrame()
-    objects_data = objects_data.append(object_data)
+    object_data = data.query(f"ID == '{reference}'").copy()
+    object_data["level"] = level
+    # object_data["ID_TO"] = reference
+    # object_data["ID_FROM"] = reference
 
     # Add object to processing list
     objects_list = [object_data]
-    level = 1
 
     for object_data in objects_list:
 
+        level += 1
+
         # End loop if we have reached desired level
         if level > levels:
             break
 
         # Get column where possible reference to other objects reside
         reference_column = object_data[["ID"]]
 
@@ -347,26 +377,21 @@
                                       suffixes=("_TO", "_FROM"))[["ID_TO", "ID_FROM"]].drop_duplicates("ID_FROM")
 
         if not reference_data.empty:
             referring_objects = pandas.merge(reference_data, data,
                                              left_on="ID_FROM",
                                              right_on="ID")  # .drop(columns=["ID_FROM"])
 
-            # Add data for future processing
-            objects_list.append(referring_objects.copy())
-
             # Set object level
             referring_objects["level"] = level
 
-            # Add objects to general objects data frame
-            objects_data = objects_data.append(referring_objects)
-
-        level += 1
+            # Add data for future processing
+            objects_list.append(referring_objects)
 
-    return objects_data
+    return pandas.concat(objects_list)
 
 
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.references_to = references_to
 
 
 def references_from_simple(data, reference, columns=["Type"]):
@@ -385,56 +410,51 @@
 pandas.DataFrame.references_from_simple = references_from_simple
 
 
 def references_from(data, reference, levels=1):
     """Return all triplets that reference object points to"""
 
     # TODO - add the key on which connection was made
+    level = 0
 
-    # Get all values of reference object VALUE columns
-
-    objects_data = pandas.DataFrame()
-
-    object_data = data.query("ID == '{}'".format(reference)).copy()
-    # object_data["ID_FROM"] = object_data["ID"]
+    # Get the object itself
+    object_data = data.query(f"ID == '{reference}'").copy()
+    object_data["level"] = level
+    #object_data["ID_TO"] = reference
+    #object_data["ID_FROM"] = reference
 
+    # Add object to processing list
     objects_list = [object_data]
-    level = 0
 
     for object_data in objects_list:
 
-        # print("{}/{}".format(level, levels))
+        level += 1
 
         # End loop if we have reached desired level
         if level > levels:
             break
 
-        # Set object level
-        object_data["level"] = level
-
-        # Add objects to general objects data frame
-        objects_data = objects_data.append(object_data)
-
         # Get column where possible reference to other objects reside
         reference_column = object_data[["ID", "VALUE"]]
 
         # Filter original data ID-s by values form reference object
         reference_data = pandas.merge(reference_column, data,
                                       left_on="VALUE",
                                       right_on="ID",
-                                      suffixes=("_FROM", ""))
+                                      suffixes=("_FROM", "")).rename(columns={"VALUE_FROM": "ID_TO"})
 
         if not reference_data.empty:
-            objects_list.append(reference_data.copy())
 
-        level += 1
+            # Set object level
+            reference_data["level"] = level
 
-        objects_data["ID_TO"] = objects_data["ID"]
+            # Add data for future processing
+            objects_list.append(reference_data)
 
-    return objects_data
+    return pandas.concat(objects_list)
 
 
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.references_from = references_from
 
 
 def references_all(data):
@@ -446,19 +466,40 @@
 
     return data[["ID", "KEY", "VALUE"]].drop_duplicates().merge(data[["ID"]].drop_duplicates(), left_on="VALUE", right_on="ID", suffixes=("_FROM", "_TO"))[["ID_FROM", "KEY", "ID_TO"]]
 
 
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.references_all = references_all
 
+def references_simple(data, reference, columns=None, levels=1):
+    """Creates a table view of all elements that specified element refers to,
+    by default returns two columns ID and Type, but this can be extended"""
+
+
+    reference_data = data.references(reference, levels=levels).drop_duplicates(["ID", "KEY"])
+
+    # Convert form triplets to a table view with columns - ID, Type by default
+    data_view = reference_data[["ID", "KEY", "VALUE"]].pivot(index="ID", columns="KEY")["VALUE"]
+
+    if not columns:
+        columns = []
+        available_columns = data_view.columns
+        if "Type" in available_columns:
+            columns.append("Type")
+
+        if "IdentifiedObject.name" in available_columns:
+            columns.append("IdentifiedObject.name")
+
+    return data_view[columns].merge(reference_data[["ID", "level", "ID_FROM", "ID_TO"]], on="ID", how="left").drop_duplicates("ID").sort_values("level")
+pandas.DataFrame.references_simple = references_simple
 
 def references(data, ID, levels=1):
     FROM = data.references_from(ID, levels)
     TO = data.references_to(ID, levels)
-    return pandas.concat([FROM, TO])
+    return pandas.concat([FROM, TO]).drop_duplicates(["ID", "KEY", "VALUE", "INSTANCE_ID"])
 pandas.DataFrame.references = references
 
 # def references(data, ID, levels=1):
 #     all_references = data.references_all()
 #     refrences_list = []
 #
 #     references = all_references.query("ID_FROM == @ID or ID_TO==@ID").copy()
@@ -502,35 +543,34 @@
     data.loc[data[data.KEY == key].index, "VALUE"] = value  # TODO add changes to change DataFrame
 
 
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.set_VALUE_at_KEY = set_VALUE_at_KEY
 
 
-def export_to_excel(data, path=None, file_name=None):
+def export_to_excel(data, path=None):
     """Exports to excel all data with same INSTACE_ID and if label element exists for it. Each Type is put to a sheet"""
     # TODO set some nice properties - https://xlsxwriter.readthedocs.io/workbook.html#workbook-set-properties
 
-    labels = data.merge(data.query("KEY == 'Type' and VALUE == 'Distribution'").ID).query("KEY == 'label'").iterrows()
+    labels = data.query("KEY == 'label'").iterrows()
     # TODO dont use iterrows
     # TODO instead of label use Distribution
     for _, label in labels:
         instance_data = data[data.INSTANCE_ID == label.INSTANCE_ID]
 
         types = instance_data.types_dict()
 
-        if file_name is None:
-            file_name = '{}.xlsx'.format(label.VALUE.split(".")[0])
+        file_name = '{}.xlsx'.format(label.VALUE.split(".")[0])
 
         if path is None:
             path = os.getcwd()
 
         file_path = os.path.join(path, file_name)
 
-        print("INFO - Exporting excel: {}".format(file_name))
+        logger.info("Exporting excel: {}".format(file_path))
         writer = pandas.ExcelWriter(file_path)
 
         for class_type in types:
             class_data = instance_data.type_tableview(class_type)
             class_data.to_excel(writer, class_type)
 
             # Get sheet to do some formatting
@@ -548,40 +588,27 @@
         writer.save()
 
 
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.export_to_excel = export_to_excel
 
 
-def export_to_cimxml(data,
-                     rdf_map=None,
-                     namespace_map=None,
+def export_to_cimxml(data, rdf_map=None, namespace_map={"rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#"},
                      class_KEY="Type",
                      export_undefined=True,
                      export_type="xml_per_instance_zip_per_xml",
                      global_zip_filename="Export.zip",
-                     filename_class="Distribution",
-                     filename_tag="label",
-                     default_id_attribute="{http://www.w3.org/1999/02/22-rdf-syntax-ns#}about",
-                     default_id_prefix="urn:uuid:",
-                     default_namespace=None,
-                     debug=False):
+                     debug=False,
+                     export_to_memory=False):
     if debug:
         start_time = datetime.datetime.now()
         init_time = start_time
 
-    if not namespace_map:
-        namespace_map = {
-            "xml": "http://www.w3.org/XML/1998/namespace",
-            "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
-            "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
-        }
-
     # File names are kept under rdfs:lable
-    labels = data.merge(data.query(f"KEY == '{class_KEY}' and VALUE == '{filename_class}'").ID).query(f"KEY == '{filename_tag}'").itertuples()
+    labels = data.query("KEY == 'label'").itertuples()
 
     # Keep all file names and data to be exported
     export_files = []
 
     # Create element builder
     E = ElementMaker(nsmap=namespace_map)
 
@@ -590,24 +617,25 @@
 
     for label in labels:
 
         instance_data = data[data.INSTANCE_ID == label.INSTANCE_ID]
 
         instance_type = None
 
+        # TODO remove dependace on this header field, wich might not be present
         if len(instance_data.query("KEY == 'Model.messageType'")):
-            instance_type = instance_data.query("KEY == 'Model.messageType'").VALUE.item()
+            instance_type = instance_data.query("KEY == 'Model.messageType'").iloc[0].VALUE
 
         # If there is sub structure available in schema get it, otherwise use root definitions
         instance_rdf_map = rdf_map.get(instance_type, rdf_map)  # TODO - needs revision, add support both for md:FullModel, dcat:DataSet and without profile definiton
 
         if instance_rdf_map is None:
-            print("WARNING - No rdf mapping available for {}".format(instance_type))
+            logger.warning("No rdf mapping available for {}".format(instance_type))
             if not export_undefined:
-                print("INFO - File not created for {}".format(label.VALUE))
+                logger.warning("File not created for {}".format(label.VALUE))
                 continue
 
         # Create xml root element
         RDF = E(QName(namespace_map["rdf"], "RDF"))
 
         # Store created xml rdf class elements
         objects = OrderedDict()
@@ -626,37 +654,31 @@
             class_def = instance_rdf_map.get(class_name, None)
 
             if class_def is not None:
 
                 class_namespace = class_def["namespace"]
                 id_name = class_def["attrib"]["attribute"]
                 id_value_prefix = class_def["attrib"]["value_prefix"]
-                language = class_def.get("language", None)
 
             else:
-                print("WARNING - Definition missing for class: {} with {}: ".format(class_name, ID))
+                logger.debug("Definition missing for class: {} with {}: ".format(class_name, ID))
 
                 if export_undefined:
-                    class_namespace = default_namespace
-                    id_name = default_id_attribute
-                    id_value_prefix = default_id_prefix
-                    language = None
+                    class_namespace = None
+                    id_name = "{http://www.w3.org/1999/02/22-rdf-syntax-ns#}about"
+                    id_value_prefix = "urn:uuid:"
                 else:
-                    print("INFO - Not Exported")
+                    logger.debug(f" {class_name} not Exported")
                     continue
 
             # Create class element
-            # print(class_namespace, class_name) # DEBUG
+            # logger.debug(class_namespace, class_name) # DEBUG
             rdf_object = E(QName(class_namespace, class_name))
             # Add ID attribute
             rdf_object.attrib[QName(id_name)] = f"{id_value_prefix}{ID}"
-
-            if language:
-                rdf_object.attrib["{http://www.w3.org/XML/1998/namespace}lang"] = language
-
             # Add object to RDF
             RDF.append(rdf_object)
             # Add object with it's ID to dict (later we use it to add attributes to that class)
             objects[ID] = rdf_object
 
         if debug:
             _, start_time = print_duration("Objects added", start_time)
@@ -676,96 +698,103 @@
 
                     tag_def = instance_rdf_map.get(KEY, None)
 
                     if tag_def is not None:
                         tag = E(QName(tag_def["namespace"], KEY))
                         attrib = tag_def.get("attrib", None)
                         text_prefix = tag_def.get("text", "")
-                        language = tag_def.get("language", None)
 
                         if attrib:
                             tag.attrib[QName(attrib["attribute"])] = f"{attrib['value_prefix']}{VALUE}"
                         else:
                             tag.text = f"{text_prefix}{VALUE}"
 
-                        if language:
-                            tag.attrib["{http://www.w3.org/XML/1998/namespace}lang"] = language
-
                         _object.append(tag)
 
                     else:
-                        print("Definition missing for tag: " + KEY)
+                        logger.debug("Definition missing for tag: " + KEY)
 
                         if export_undefined:
-                            tag = E(QName(default_namespace, KEY))
+                            tag = E(KEY)
                             tag.text = str(VALUE)
 
                             _object.append(tag)
 
+
                 else:
-                    print("Attribute VALUE is None, thus not exported: ID: {} KEY: {}".format(ID, KEY))
+                    logger.debug("Attribute VALUE is None, thus not exported: ID: {} KEY: {}".format(ID, KEY))
                     pass
 
             else:
-                print("No Object with ID: {}".format(ID))
+                logger.debug("No Object with ID: {}".format(ID))
                 pass
 
         if debug:
             _, start_time = print_duration("Attributes added", start_time)
 
         # etree.tostring(RDF, pretty_print=True, xml_declaration=True, encoding='UTF-8')
-        # print(etree.tostring(RDF, pretty_print=True).decode())
+        # logger.debug(etree.tostring(RDF, pretty_print=True).decode())
 
         # Convert to XML
         xml = etree.tostring(RDF, pretty_print=True, xml_declaration=True, encoding='UTF-8')
         # TODO - clean namespaces
 
-        print("INFO - Exporting RDF to {}".format(label.VALUE))
+        logger.info("Exporting RDF to {}".format(label.VALUE))
 
         export_files.append({"filename": label.VALUE, "file": xml})
 
         if debug:
             _, start_time = print_duration("XML created", start_time)
 
     # Export XML
     if export_type == "xml_per_instance":
         for export_file in export_files:
             # Write to file
-            with open(export_file["filename"], 'w', encoding="utf-8") as file:
+            with open(export_file["filename"], 'w') as file:
                 file.write(export_file["file"].decode())
-                print('INFO - Saved {}'.format(export_file["filename"]))
+                logger.info('Saved {}'.format(export_file["filename"]))
 
     # Export ZIP containing all xml
     elif export_type == "xml_per_instance_zip_per_all":
         from zipfile import ZipFile, ZIP_DEFLATED
 
-        with ZipFile(global_zip_filename, mode='w', compression=ZIP_DEFLATED) as zip_file:
+        gloabl_zip_fileobject = BytesIO()
+        with ZipFile(gloabl_zip_fileobject, "a", ZIP_DEFLATED, False) as zip_file:
+
             for export_file in export_files:
                 zip_file.writestr(export_file["filename"], export_file["file"])
 
-        print('INFO - Saved {}'.format(global_zip_filename))
+        if export_to_memory:
+            gloabl_zip_fileobject.name = global_zip_filename
+            return gloabl_zip_fileobject
+
+        else:
+            with open(global_zip_filename, "wb") as file_oject:
+                gloabl_zip_fileobject.seek(0)
+                file_oject.write(gloabl_zip_fileobject.read())
+                logger.info('Saved {}'.format(global_zip_filename))
 
     # Export each xml in separate zip
     elif export_type == "xml_per_instance_zip_per_xml":
         from zipfile import ZipFile, ZIP_DEFLATED
 
         for export_file in export_files:
             zip_filename = export_file["filename"].replace('.xml', '.zip')
             with ZipFile(zip_filename, mode='w', compression=ZIP_DEFLATED) as zip_file:
                 zip_file.writestr(export_file["filename"], export_file["file"])
 
-                print('INFO - Saved {}'.format(zip_filename))
+                logger.info('Saved {}'.format(zip_filename))
 
     else:
-        print("Not supported option")
-        print("Supported options are: xml_per_instance, xml_per_instance_zip_per_all, xml_per_instance_zip_per_xml")
+        logger.info("Not supported option")
+        logger.info("Supported options are: xml_per_instance, xml_per_instance_zip_per_all, xml_per_instance_zip_per_xml")
 
     if debug:
-        print_duration("DEBUG - Files saved in", start_time)
-        print_duration("DEBUG - Whole Export done in", init_time)
+        print_duration("Files saved in", start_time)
+        print_duration("Whole Export done in", init_time)
 
 
 # Extend this functionality to pandas DataFrame
 pandas.DataFrame.export_to_cimxml = export_to_cimxml
 
 
 def get_object_data(data, object_UUID):
@@ -782,52 +811,43 @@
 
 
 pandas.DataFrame.tableview_to_triplet = tableview_to_triplet
 
 # Let's add empty dataframe to keep changes
 pandas.DataFrame.changes = pandas.DataFrame()
 
-
 def update_triplet_from_triplet(data, update_data, update=True, add=True):
     """Update or add data to current triplet from another one
     VALUE at ID and KEY is updated and KEY ID pair does not exist it is added together with VALUE
     you can control if data is added or updated with parameters update and add, by default both are True"""
     # TODO add changes dataframe, where to keep all changes done by this function
     # TODO create function to do also ID and KEY changes
 
-    report_columns = ["ID", "KEY", "VALUE", "VALUE_OLD", "INSTANCE_ID"]
     write_columns = ["ID", "KEY", "VALUE", "INSTANCE_ID"]
 
-    # Make merge to see what updated data already exists in old and what needs to be added
-    test_merge = data.merge(update_data, on=["ID", "KEY"], how='right', indicator=True, suffixes=("_OLD", ""), sort=False)
-
-    if update:
-
-        # Get unique data to be updated (if drop duplicates is not used, the update by index fill corrupt data)
-        data_to_update = test_merge.query("_merge == 'both'").drop_duplicates(subset=write_columns)
+    # Choose what columns to use for final merge
+    merge_columns = ["ID", "KEY"]
+    if "INSTANCE_ID" in update_data.columns:
+        merge_columns = ["ID", "KEY", "INSTANCE_ID"]
 
-        # Store changes
-        data.changes = data.changes.append(data_to_update[report_columns], ignore_index=True)
+    # First reset index to be sure that data does not have duplicated keys
+    data = data.reset_index(drop=True)
 
-        # Get original index for update to work # TODO could be simplified by keeping index at test merge
-        old_index_new_value = data.merge(data_to_update[write_columns], on=["ID", "KEY"], how='left', suffixes=("_OLD", ""), sort=False).dropna()[["VALUE"]]
+    # Make merge to see what updated data already exists in old and what needs to be added
+    changes = data.reset_index(names="original_index").merge(update_data, on=merge_columns, how='right', indicator=True, suffixes=("_OLD", ""), sort=False)
 
-        # Update data by original index (if data anomalies are present it is due to above merge extending initial data set with new rows and indexes)
-        data.update(old_index_new_value)
-        # TODO compare performance of append + drop vs update
+    if update:
+        # Filter data that needs to be updated
+        data_to_update = changes.query("_merge == 'both'").drop_duplicates(subset="original_index")
+        data.iloc[data_to_update["original_index"].astype(int)] = data_to_update[write_columns]
 
     if add:
-
-        data_to_add = test_merge.query("_merge == 'right_only'").drop_duplicates(subset=write_columns)
-
-        # Store changes
-        data.changes = data.changes.append(data_to_add[report_columns], ignore_index=True)
-
-        # Add data
-        data = data.append(data_to_add[write_columns], ignore_index=True)
+        # Filter data that needs to be added
+        data_to_add = changes.query("_merge == 'right_only'")[write_columns]
+        data = pandas.concat([data, data_to_add]).drop_duplicates(keep='last', ignore_index=True)
 
     return data
 
 
 pandas.DataFrame.update_triplet_from_triplet = update_triplet_from_triplet
 
 
@@ -851,49 +871,89 @@
     """Retuns from_triplet - what_triplet"""
     return from_triplet.drop(from_triplet.reset_index().merge(what_triplet[columns], on=columns, how="inner")["index"], axis=0)
 
 
 def filter_triplet_by_type(triplet, type):
     """Filter out all objects data by rdf:type"""
     return triplet.merge(triplet.query("KEY == 'Type' and VALUE == @type").ID)
-pandas.DataFrame.filter_by_type = filter_triplet_by_type
-
 
-def triplet_diff(left_data, right_data):
 
-    return left_data.merge(right_data, on=["ID", "KEY", "VALUE"], how='outer', indicator=True, suffixes=("_OLD", "_NEW"), sort=False).query("_merge != 'both'")
+def triplet_diff(old_data, new_data):
 
+    return old_data.merge(new_data, on=["ID", "KEY", "VALUE"], how='outer', indicator=True, suffixes=("_OLD", "_NEW"), sort=False).query("_merge != 'both'")
 
-def print_triplet_diff(left_data, right_data, file_id_object="Distribution", file_id_key="label", exclude_objects=[]):
 
-    diff = triplet_diff(left_data, right_data)
+def print_triplet_diff(old_data, new_data, file_id_object="Distribution", file_id_key="label", exclude_objects=None):
 
-    changes = diff.replace({'_merge': {"left_only": "-", "right_only": "+"}}).sort_values(by=['ID', 'KEY'])
+    # Get diff between datasets
+    diff = triplet_diff(old_data, new_data)
+    diff = diff.replace({'_merge': {"left_only": "-", "right_only": "+"}}).sort_values(by=['ID', 'KEY'])
 
-    file_id_data = filter_triplet_by_type(changes, file_id_object)
-    changes = remove_triplet_from_triplet(changes, file_id_data)
-    print(f"INFO - removed {file_id_object} from diff")
+    # Extract internal structures keeping file name information
+    file_id_data = filter_triplet_by_type(diff, file_id_object)
+    diff = remove_triplet_from_triplet(diff, file_id_data)
+    logger.info(f"INFO - removed {file_id_object} from diff")
 
+    # Exclude defined types form export
     if exclude_objects:
         for object_name in exclude_objects:
-            excluded_data = filter_triplet_by_type(changes, object_name)
-            changes = remove_triplet_from_triplet(changes, excluded_data)
+            excluded_data = filter_triplet_by_type(diff, object_name)
+            diff = remove_triplet_from_triplet(diff, excluded_data)
             print(f"INFO - removed {object_name} from diff")
 
-    for _, file_id in file_id_data.query("KEY == @file_id_key and _merge == '-'").VALUE.iteritems():
+    # Extract types on left and right to get changed/modified types
+    removed_added_modified_types = pandas.concat([
+        old_data.merge(diff["ID"]).query("KEY == 'Type'").drop_duplicates(),
+        new_data.merge(diff["ID"]).query("KEY == 'Type'").drop_duplicates()
+        ])[["ID", "KEY", "VALUE"]].drop_duplicates()
+
+    # Print old file name
+    for _, file_id in file_id_data.query(f"KEY == '{file_id_key}' and _merge == '-'").VALUE.items():
         print(f"--- {file_id}")# from-file-modification-time")
 
-    for _, file_id in file_id_data.query("KEY == @file_id_key and _merge == '+'").VALUE.iteritems():
+    # Print new file name
+    for _, file_id in file_id_data.query(f"KEY == '{file_id_key}' and _merge == '+'").VALUE.items():
         print(f"+++ {file_id}")# to-file-modification-time")
 
-    changes_on_left = len(changes.query("_merge == '-'"))
-    changes_on_right = len(changes.query("_merge == '+'"))
-    print(f"@@ -1,{changes_on_left} +1,{changes_on_right} @@")
-    for _, change in (changes._merge + changes.ID + " " + changes.KEY + " " + changes.VALUE).iteritems():
-        print(change)
+    # Print changes
+
+    print("")
+    print(f"@@ -1,0 +1,0 @@ Removed:")
+
+    for key, value in diff.query("KEY == 'Type' and _merge == '-'").VALUE.value_counts().items():
+        print(" ", key, value)
+
+    print("")
+    print(f"@@ -1,0 +1,0 @@ Added:")
+    for key, value in diff.query("KEY == 'Type' and _merge == '+'").VALUE.value_counts().items():
+        print(" ", key, value)
+
+    print("")
+    print(f"@@ -1,0 +1,0 @@ Changed:")
+    for key, value in pandas.concat([removed_added_modified_types, diff.query("KEY == 'Type'")])[["ID", "KEY", "VALUE"]].drop_duplicates(keep=False).VALUE.value_counts().items():
+        print(" ", key, value)
+
+    # Types changed
+    # TODO add name field to be used with Type for better reporting
+
+    for group_name, group in removed_added_modified_types.groupby("VALUE"):
+        #print(f"Types - {group_name}")
+        for objec_type in group.itertuples():
+
+            current_diff = diff.query("ID == @objec_type.ID")
+
+            changes_on_left = len(current_diff.query("_merge == '-'"))
+            changes_on_right = len(current_diff.query("_merge == '+'"))
+            print("")
+            print(f"@@ -1,{changes_on_left} +1,{changes_on_right} @@ {objec_type.VALUE} {objec_type.ID}")
+
+            for _, change in (current_diff._merge.astype(str) + current_diff.KEY.astype(str) + " -> " + current_diff.VALUE.astype(str)).items():
+                print(change)
+
+    # Nice diff viewer https://diffy.org/
 
 # changes = changes.replace({'_merge': {"left_only": "-", "right_only": "+"}})
 
 def export_to_networkx(data):
     """Converts triplet to networkx graph"""
     import networkx
 
@@ -908,59 +968,30 @@
     graph.add_nodes_from([(ID, {"Type": VALUE}) for ID, VALUE in nodes.values])
     graph.add_edges_from([(FROM, TO, {"Type": KEY}) for FROM, KEY, TO in edges.values])
 
     return graph
 
 pandas.DataFrame.to_networkx = export_to_networkx
 
-
-def load_export_conf(list_of_conf_paths):
-    """Loads export configuration form json files"""
-    conf = {}
-    for export_format in list_of_conf_paths:
-        print(f"Loading {export_format}")
-        conf.update(json.load(open(export_format)))
-
-    return conf
-
-
-def rename_and_append_key(data, original_key, new_key, original_value=None, new_value=None):
-
-    if original_value:
-        description = pandas.DataFrame(data.query(f"KEY == '{original_key}' and VALUE =='{original_value}'"))
-        description["VALUE"] = new_value
-    else:
-        description = pandas.DataFrame(data.query(f"KEY == '{original_key}'"))
-
-    description["KEY"] = new_key
-    data = data.append(description, ignore_index=True)
-    return data
-
-def add_key_and_value(data, type, key, value, id=None):
-
-    if id:
-        filter = data.query("ID == @id and KEY == 'Type' and VALUE == @type")
-
-    else:
-        filter = data.query("KEY == 'Type' and VALUE == @type")
-
-    filter["KEY"] = key
-    filter["VALUE"] = value
-
-    data = data.append(filter, ignore_index=True)
-    return data
-
 # END OF FUNCTIONS
 
 
 # TEST AND EXAMPLES
 if __name__ == '__main__':
-    path = "../test_models/TestConfigurations_packageCASv2.0/RealGrid/CGMES_v2.4.15_RealGridTestConfiguration_v2.zip"
 
-    data = pandas.read_RDF([path], debug=True)  # Last took 0:00:03.514987
+    import sys
+    logging.basicConfig(stream=sys.stdout,
+                        format='%(levelname) -10s %(asctime)s %(name) -30s %(funcName) -35s %(lineno) -5d: %(message)s',
+                        level=logging.DEBUG)
+
+    path = "../test_data/TestConfigurations_packageCASv2.0/RealGrid/CGMES_v2.4.15_RealGridTestConfiguration_v2.zip"
+
+    data = pandas.read_RDF([path], debug=True)
+    # Last took 0:00:07.919968 on python 3.7  and pandas 1.3.5
+    # Last took 0:00:04.312218 on python 3.11 abd pandas 2.0.2
 
     print("Loaded types")
     print(data.query("KEY == 'Type'")["VALUE"].value_counts())
 
     print("Example how to get table view of all objects of specified type")
     print(data.type_tableview("ACLineSegment"))
 
@@ -983,8 +1014,15 @@
     # data.query("ID == '#Resistance'")
     #
     # data_types = data.query("KEY == 'dataType'")["VALUE"].drop_duplicates()
 
     # for quick export of data use data[data.VALUE == "PowerTransformer"].to_csv(export.csv) or data[data.VALUE == "PowerTransformer"].to_clipboard() and  paste to excel, for other method refer to pandas manual
 
 
-
+    # SvPowerFlow = data.type_tableview("SvPowerFlow").reset_index()
+    # TieFlow = data.type_tableview('TieFlow').reset_index()
+    # tieflow_data = TieFlow.merge(SvPowerFlow, right_on='SvPowerFlow.Terminal', left_on="TieFlow.Terminal", how="left", suffixes=("", "_SvPowerFlow"))
+    #
+    # print(f"""
+    # NP (tieflow):   {tieflow_data["SvPowerFlow.p"].sum()} MW
+    # NP (CA.nI)  :   {data.type_tableview("ControlArea").iloc[0]["ControlArea.netInterchange"]} MW
+    # """)
```

### Comparing `triplets-0.0.3/triplets/rdfs_tools.py` & `triplets-0.0.4/triplets/rdfs_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                     },
                     "Model.version": {
                         "namespace": "http://iec.ch/TC57/61970-552/ModelDescription/1#"
                     }}
 
 if __name__ == '__main__':
 
-    path = r"rdfs\CGMES_2_4_15_09May2019_RDFS\UNIQUE_RDFSAugmented-v2_4_15-09May2019.zip"
+    path = r"..\profiles\ENTSOE\2019-05-09_RDFS_CGMES_2_4_15\EquipmentProfileCoreOperationShortCircuitRDFSAugmented-v2_4_15-09May2019.rdf"
 
     data = load_all_to_dataframe([path])
 
     print(validation_view(data, "#ACLineSegment"))
     print(validation_view(data, "#PowerTransformerEnd"))
```

### Comparing `triplets-0.0.3/triplets.egg-info/PKG-INFO` & `triplets-0.0.4/triplets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplets
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple RDF tools to load/modify/export RDF data using Pandas DataFrames
 Home-page: https://github.com/Haigutus/rdf_tools
 Author: Kristjan Vilgo
 Author-email: kristjan.vilgo@gmail.com
 License: MIT
 Description: # RDF parser:
```

### Comparing `triplets-0.0.3/versioneer.py` & `triplets-0.0.4/versioneer.py`

 * *Files identical despite different names*

