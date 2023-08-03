# Comparing `tmp/dbhydra-1.2.3.tar.gz` & `tmp/dbhydra-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.2.3.tar", last modified: Wed Aug  2 14:54:40 2023, max compression
+gzip compressed data, was "dbhydra-1.2.4.tar", last modified: Thu Aug  3 14:33:35 2023, max compression
```

## Comparing `dbhydra-1.2.3.tar` & `dbhydra-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.680045 dbhydra-1.2.3/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-08-02 14:54:40.680045 dbhydra-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.647133 dbhydra-1.2.3/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.3/dbhydra/__init__.py
--rw-rw-rw-   0        0        0    69488 2023-08-02 14:51:30.000000 dbhydra-1.2.3/dbhydra/dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.679048 dbhydra-1.2.3/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.3/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:54:40.662099 dbhydra-1.2.3/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 14:54:40.000000 dbhydra-1.2.3/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 14:54:40.680045 dbhydra-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-08-02 14:54:37.000000 dbhydra-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:33:35.410869 dbhydra-1.2.4/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-08-03 14:33:35.409871 dbhydra-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 14:33:35.361961 dbhydra-1.2.4/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.4/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0    71688 2023-08-02 18:51:21.000000 dbhydra-1.2.4/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:33:35.409871 dbhydra-1.2.4/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.4/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.4/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.4/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.4/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:33:35.381953 dbhydra-1.2.4/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-08-03 14:33:34.000000 dbhydra-1.2.4/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-08-03 14:33:35.000000 dbhydra-1.2.4/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 14:33:34.000000 dbhydra-1.2.4/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-08-03 14:33:34.000000 dbhydra-1.2.4/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 14:33:35.000000 dbhydra-1.2.4/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 14:33:35.410869 dbhydra-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-08-03 14:33:31.000000 dbhydra-1.2.4/setup.py
```

### Comparing `dbhydra-1.2.3/LICENSE` & `dbhydra-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.3/PKG-INFO` & `dbhydra-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.2.3
+Version: 1.2.4
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.2.3/README.md` & `dbhydra-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.3/dbhydra/dbhydra_core.py` & `dbhydra-1.2.4/dbhydra/dbhydra_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import ast
 import json
 import math
 import sys
 import threading
 from contextlib import contextmanager
 from sys import platform
+import os
 
 import numpy as np
 import pandas as pd
 import pymongo
 import pymysql as MySQLdb
 from google.cloud import bigquery
 from google.oauth2 import service_account
@@ -763,17 +764,22 @@
         """id_column_name -> name of predefined column with autoincrement + PK"""
         super().__init__(db1, name, columns)
         self.types = types
         self.id_column_name = id_column_name
 
     # Temporary disabled, please make sure this is implemented where needed, don't introduce breaking changes please
     # @abc.abstractmethod
-    def init_from_column_type_dict(db1, name, column_type_dict, init_from_column_type_dict="id"):
-        pass
-
+    @classmethod
+    def init_from_column_type_dict(cls, db1, name, column_type_dict, id_column_name="id"):
+        column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
+        columns = list(column_converted_type_dict.keys())
+        types = list(column_converted_type_dict.values())
+        return cls(db1, name, columns, types, id_column_name=id_column_name)
+    
+    
     def drop(self):
         query = "DROP TABLE " + self.name
         print(query)
         self.db1.execute(query)
 
     def update(self, variable_assign, where=None):
         if where is None:
@@ -1398,20 +1404,21 @@
 
 class MysqlTable(MysqlSelectable, AbstractTable):
     def __init__(self, db1, name, columns=None, types=None, id_column_name = "id"):
         super().__init__(db1, name, columns)
         self.types = types
         self.id_column_name = id_column_name
 
-    @classmethod
-    def init_from_column_type_dict(cls, db1, name, column_type_dict, id_column_name="id"):
-        column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
-        columns = list(column_converted_type_dict.keys())
-        types = list(column_converted_type_dict.values())
-        return cls(db1, name, columns, types, id_column_name=id_column_name)
+    #Disabled because it is inherited
+    # @classmethod
+    # def init_from_column_type_dict(cls, db1, name, column_type_dict, id_column_name="id"):
+    #     column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
+    #     columns = list(column_converted_type_dict.keys())
+    #     types = list(column_converted_type_dict.values())
+    #     return cls(db1, name, columns, types, id_column_name=id_column_name)
 
     def initialize_columns(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
         query = f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND  TABLE_NAME  = '" + self.name + "';"
         columns = information_schema_table.select(query)
         self.columns = columns
 
@@ -1657,17 +1664,32 @@
             self.db1.execute(command)
             index = self.columns.index(column_name)
             self.types[index] = new_column_type
         except:
             print("Cant modify column to table.")
 
 
-class XlsxDB:
-    def __init__(self, name="new_db", config_file="config.ini"):
-        self.name = name
+class XlsxDB(AbstractDB):
+    def __init__(self, config_file="config.ini", db_details=None):
+        if db_details is None:
+            self.name="new_db"
+        else:
+            self.name = db_details.get("DB_DATABASE")
+        self.lock = threading.Lock()
+        
+        self.python_database_type_mapping = {
+        'int': "int",
+        'float': "double",
+        'str': "str",
+        'list': "str",
+        'dict': "str",
+        'bool': "bool",
+        'datetime': "datetime"
+        }
+
 
         """
         db_details=read_connection_details(config_file)
         locally=True
         if db_details["LOCALLY"]=="False":
             locally=False
 
@@ -1680,38 +1702,71 @@
         else:
             self.DB_SERVER = db_details["DB_SERVER"]
             self.DB_DATABASE = db_details["DB_DATABASE"]
             self.DB_USERNAME = db_details["DB_USERNAME"]
             self.DB_PASSWORD = db_details["DB_PASSWORD"]
             self.connect_remotely()
         """
+        
+        class DummyXlsxConnection: #compatibility with MySQL connection
+            def begin(*args):
+                pass
+            def commit(*args):
+                pass
+            def rollback(*args):
+                pass
+            
+        class DummyXlsxCursor: #compatibility with MySQL connection
+            def execute(*args):    
+                pass
+            
+            def fetchall(*args):
+                pass
+            
+        self.cursor=DummyXlsxCursor()
+        self.connection=DummyXlsxConnection()
+        self.create_database()
+        
+    def connect_locally(self):
+        pass #no real connection
+        
+    def connect_remotely(self):
+        pass #no real connection
 
     def execute(self, query):
         pass
         # self.cursor.execute(query)
         # self.cursor.commit()
 
     def close_connection(self):
         pass
         # self.connection.close()
         # print("DB connection closed")
 
     def create_database(self):
-        import os
         try:
             os.mkdir(self.name)
             print("Database created")
-        except:
+        except FileExistsError:
             print("Database is already created")
 
 
 class XlsxTable(AbstractTable):
-    def __init__(self, db1, name, columns=None, types=None):
+    def __init__(self, db1, name, columns=None, types=None, id_column_name = "id"):
         super().__init__(db1, name, columns)
         self.types = types
+        self.id_column_name=id_column_name
+        
+        
+    def create(self):
+        df=pd.DataFrame(columns=self.columns)
+        df.to_excel(self.db1.name + "\\" + self.name + ".xlsx",index=False)
+    
+    def drop(self):
+        pass
 
     def select_to_df(self):
         try:
             df = pd.read_excel(self.db1.name + "//" + self.name + ".xlsx")
             # cols=df.columns
             # print(cols)
             # df.set_index(cols[0],inplace=True)
@@ -1723,41 +1778,47 @@
         return (df)
 
     def insert_from_df(self, df, batch=1, try_mode=False, debug_mode=False):
         assert len(df.columns) + 1 == len(self.columns)  # +1 because of id column
 
         original_df = self.select_to_df()
 
+        original_df.index=original_df[self.id_column_name]
         try:
             original_df = original_df.drop(original_df.columns[0], axis=1)
         except:
             print("First column could not be dropped")
 
-        df.columns = original_df.columns
         # handling nan values -> change to NULL TODO
         for column in list(df.columns):
             df.loc[pd.isna(df[column]), column] = "NULL"
 
         def concat_with_reset_index_in_second_df(original_df, df):
             """Subsitute of reset_index method because we need to maintain the ids of original df"""
-            maximal_index = max(original_df.index)
+            if len(original_df.index)>0:
+                maximal_index = max(original_df.index)
+            else:
+                maximal_index=0
             df.index = df.index + maximal_index + 1
+            df.reindex(columns=original_df.columns.tolist()) #to ensure that columns get correctly inserted
             original_df = original_df.append(df)
             # df=pd.concat([original_df,df])
             return (original_df)
 
-        if len(original_df) > 0:
-            df = concat_with_reset_index_in_second_df(original_df, df)
-
-        df.to_excel(self.db1.name + "\\" + self.name + ".xlsx")
+        df = concat_with_reset_index_in_second_df(original_df, df)
+        df["uid"]=df.index
+        df.reindex(columns=["uid"]+df.columns[:-1].tolist()) #uid as a first column
+        df.reset_index(drop=True,inplace=True)
+        print("INSERTED",df)
+        df.to_excel(self.db1.name + "\\" + self.name + ".xlsx",index=False)
 
     def replace_from_df(self, df):
         assert len(df.columns) == len(self.columns)  # +1 because of id column
-        df.drop(df.columns[0], axis=1, inplace=True)
-        df.to_excel(self.db1.name + "\\" + self.name + ".xlsx")
+        #df.drop(df.columns[0], axis=1, inplace=True)
+        df.to_excel(self.db1.name + "\\" + self.name + ".xlsx",index=False)
 
     def update(self, variable_assign, where=None):
         def split_assign(variable_assign):
             variable = variable_assign.split("=")[0]
             value = variable_assign.split("=")[1]
             try:
                 value = int(value)  # integers
@@ -1770,15 +1831,15 @@
         print(where)
         print(variable, value)
         if where is None:
             df[variable] = value
             print(df)
         else:
             where_variable, where_value = split_assign(where)
-            df[variable] = df[where_variable].apply(lambda x: value if x == where_value else x)
+            df[variable] = df[where_variable].apply(lambda x: value if str(x) == str(where_value) else x) #
         self.replace_from_df(df)
 
     def delete(self, where=None):
         def split_assign(variable_assign):
             variable = variable_assign.split("=")[0]
             value = variable_assign.split("=")[1]
             try:
```

### Comparing `dbhydra-1.2.3/dbhydra/tests/test_mongo.py` & `dbhydra-1.2.4/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.3/dbhydra/tests/test_sql.py` & `dbhydra-1.2.4/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.3/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.2.4/dbhydra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.2.3
+Version: 1.2.4
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.2.3/setup.py` & `dbhydra-1.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.2.3',
+    version='1.2.4',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

