# Comparing `tmp/Peliqan-0.1.3.tar.gz` & `tmp/Peliqan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-0.1.3.tar", last modified: Fri Jul 28 11:35:53 2023, max compression
+gzip compressed data, was "Peliqan-0.1.4.tar", last modified: Thu Aug  3 11:07:50 2023, max compression
```

## Comparing `Peliqan-0.1.3.tar` & `Peliqan-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-28 11:35:53.300680 Peliqan-0.1.3/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-28 11:35:53.300561 Peliqan-0.1.3/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-28 11:35:53.300253 Peliqan-0.1.3/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-07-28 06:15:32.000000 Peliqan-0.1.3/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-28 11:35:53.300358 Peliqan-0.1.3/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    40386 2023-07-28 07:29:22.000000 Peliqan-0.1.3/peliqan/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-28 11:35:53.300723 Peliqan-0.1.3/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-28 06:15:32.000000 Peliqan-0.1.3/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-08-03 11:07:50.893272 Peliqan-0.1.4/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-08-03 11:07:50.893167 Peliqan-0.1.4/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-08-03 11:07:50.892698 Peliqan-0.1.4/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-08-03 11:07:50.000000 Peliqan-0.1.4/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-08-03 11:07:50.000000 Peliqan-0.1.4/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-08-03 11:07:50.000000 Peliqan-0.1.4/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-08-03 11:07:50.000000 Peliqan-0.1.4/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-08-03 11:07:50.000000 Peliqan-0.1.4/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-0.1.4/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-08-03 11:07:50.892792 Peliqan-0.1.4/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    40526 2023-08-03 11:07:45.000000 Peliqan-0.1.4/peliqan/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-08-03 11:07:50.893304 Peliqan-0.1.4/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-08-02 11:35:09.000000 Peliqan-0.1.4/setup.py
```

### Comparing `Peliqan-0.1.3/PKG-INFO` & `Peliqan-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.3/Peliqan.egg-info/PKG-INFO` & `Peliqan-0.1.4/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.3/README.md` & `Peliqan-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-0.1.3/peliqan/__init__.py` & `Peliqan-0.1.4/peliqan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 # import necessary modules
 import logging
 
 import pandas
@@ -109,42 +109,47 @@
         if "detail" in response_dict:
             return response_dict["detail"]
         else:
             return response_dict
 
     def findone(self, object_name, **kwargs):
         if "searchterm" not in kwargs:
-            raise PeliqanClientException(f"Parameter searchterm is required and searchfield is sometimes required for function 'findone'.")
+            raise PeliqanClientException(
+                f"Parameter searchterm is required and searchfield is sometimes required for function 'findone'.")
         response_dict = self.request_endpoint_via_proxy(object_name, 'findone', **kwargs)
         if "detail" in response_dict:
             detail = response_dict["detail"]
-            if not isinstance(detail, dict): # replace empty string response "" (if no record found) with {}
+            if not isinstance(detail, dict):  # replace empty string response "" (if no record found) with {}
                 detail = {}
             return detail
         else:
             return response_dict
 
     def list(self, object_name, **kwargs):
         response_dict = self.request_endpoint_via_proxy(object_name, 'list', **kwargs)
         return response_dict
 
     def add(self, object_name, *args, **kwargs):
-        kwargs = self.args_to_kwargs(args, kwargs) # allow using both keyword arguments or a dict as argument: pq.add("contact", name='John', city='NY') or pq.add("contact", contact_obj)
+        kwargs = self.args_to_kwargs(args,
+                                     kwargs)  # allow using both keyword arguments or a dict as argument: pq.add("contact", name='John', city='NY') or pq.add("contact", contact_obj)
         response_dict = self.request_endpoint_via_proxy(object_name, 'add', **kwargs)
         return response_dict
 
     def update(self, object_name, *args, **kwargs):
-        kwargs = self.args_to_kwargs(args, kwargs) # allow using both keyword arguments or a dict as argument: pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
+        kwargs = self.args_to_kwargs(args,
+                                     kwargs)  # allow using both keyword arguments or a dict as argument: pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
         response_dict = self.request_endpoint_via_proxy(object_name, 'update', **kwargs)
         return response_dict
 
     def upsert(self, object_name, *args, **kwargs):
-        kwargs = self.args_to_kwargs(args, kwargs) # allow using both keyword arguments or a dict as argument: pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
+        kwargs = self.args_to_kwargs(args,
+                                     kwargs)  # allow using both keyword arguments or a dict as argument: pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
         if "searchterm" not in kwargs:
-            raise PeliqanClientException(f"Parameter searchterm is required and searchfield is sometimes required for function 'upsert'.")
+            raise PeliqanClientException(
+                f"Parameter searchterm is required and searchfield is sometimes required for function 'upsert'.")
         if "searchfield" not in kwargs:
             kwargs["searchfield"] = None
         response_dict_findone = self.request_endpoint_via_proxy(object_name, 'findone',
                                                                 searchfield=kwargs["searchfield"],
                                                                 searchterm=kwargs["searchterm"])
         kwargs.pop('searchfield', None)
         kwargs.pop('searchterm', None)
@@ -499,39 +504,39 @@
 
     def _to_dtype(self, column_type, tz):
         if (
             column_type[0:3].lower() == "int" or
             column_type[0:3].lower() == "num" or
             column_type[0:6].lower() == "bigint"
         ):  # todo add more field types
-            type_name = int
+            type_name = pd.Int64Dtype()
 
         elif (
             column_type[0:6].lower() == "double" or
             column_type[0:5].lower() == "float" or
             column_type[0:7].lower() == "decimal"
         ):
-            type_name = float
+            type_name = pd.Float64Dtype()
 
         elif column_type == "date":
             type_name = pd.DatetimeTZDtype(tz=tz)
 
         elif column_type[0:9].lower() == "timestamp" or column_type[0:8].lower() == "datetime":
             type_name = pd.DatetimeTZDtype(tz=tz)
 
         elif column_type[0:4].lower() == "bool":
-            type_name = bool
+            type_name = pd.BooleanDtype()
         else:
-            type_name = str
+            type_name = pd.StringDtype()
 
         return type_name
 
     # todo allow user to set a PK column for the query (or update the guessed PK)
-    def load_table(self, table_name='', query='', table_id=None, fillna_with='', to_dict=False,
-                   enable_python_types=False, tz='UTC'):
+    def load_table(self, table_name='', query='', table_id=None, fillnat_with=None, fillna_with=None, df=False,
+                   enable_python_types=True, tz='UTC'):
         """
         Return the records in a table.
 
         :param table_name: The name of a table.
         :param query: A valid Trino sql query.
         :param table_id: An integer value that uniquely identifies a table.
         :param fillna_with: Replace empty value with a default placeholder.
@@ -571,30 +576,27 @@
         columns = []
         dtypes = []
         for column in column_data:
             dtypes.append((column[0], self._to_dtype(column[1], tz)))
             columns.append(column[0])
 
         # Create dataframe
-        df = pd.DataFrame(records, columns=columns)
+        dataframe = pd.DataFrame(records, columns=columns)
+
+        dataframe.replace({pandas.NaT: fillnat_with, pandas.NA: fillna_with}, inplace=True)
+
         if enable_python_types:
             for dtype in dtypes:
-                df[dtype[0]] = df[dtype[0]].astype(dtype[1])
-
-        if fillna_with is not None:
-            # replace Na/NaN
-            df.fillna(fillna_with, inplace=True)
-            # replace NaT
-            df.replace({pandas.NaT: None}, inplace=True)
+                dataframe[dtype[0]] = dataframe[dtype[0]].astype(dtype[1])
 
-        if to_dict:
-            return df.to_dict('records')
+        if df:
+            return dataframe
 
         else:
-            return df
+            return dataframe.to_dict('records')
 
     # todo: make it easier to find table & field ids in UI
     def update_cell(self, row_pk, value, table_id=None, table_name=None, field_id=None, field_name=None):
         if not row_pk:
             raise PeliqanClientException("row_pk must be provided.")
 
         # BACKEND_URL and JWT are prepended to the generated script,
```

### Comparing `Peliqan-0.1.3/setup.py` & `Peliqan-0.1.4/setup.py`

 * *Files identical despite different names*

