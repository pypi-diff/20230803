# Comparing `tmp/consumableai-1.0.2.tar.gz` & `tmp/consumableai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consumableai-1.0.2.tar", last modified: Wed Jun 28 11:01:16 2023, max compression
+gzip compressed data, was "consumableai-1.0.3.tar", last modified: Thu Aug  3 13:02:52 2023, max compression
```

## Comparing `consumableai-1.0.2.tar` & `consumableai-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sandeep    (501) staff       (20)        0 2023-06-28 11:01:16.968261 consumableai-1.0.2/
--rw-r--r--   0 sandeep    (501) staff       (20)     1070 2023-06-01 16:21:54.000000 consumableai-1.0.2/LICENSE
--rw-r--r--   0 sandeep    (501) staff       (20)     1817 2023-06-28 11:01:16.967975 consumableai-1.0.2/PKG-INFO
--rw-r--r--   0 sandeep    (501) staff       (20)     1625 2023-06-02 08:23:20.000000 consumableai-1.0.2/README.md
-drwxr-xr-x   0 sandeep    (501) staff       (20)        0 2023-06-28 11:01:16.966414 consumableai-1.0.2/consumableai/
--rw-r--r--   0 sandeep    (501) staff       (20)        0 2023-05-29 10:28:08.000000 consumableai-1.0.2/consumableai/__init__.py
--rw-r--r--   0 sandeep    (501) staff       (20)     6215 2023-06-06 08:45:52.000000 consumableai-1.0.2/consumableai/cli.py
-drwxr-xr-x   0 sandeep    (501) staff       (20)        0 2023-06-28 11:01:16.967622 consumableai-1.0.2/consumableai.egg-info/
--rw-r--r--   0 sandeep    (501) staff       (20)     1817 2023-06-28 11:01:16.000000 consumableai-1.0.2/consumableai.egg-info/PKG-INFO
--rw-r--r--   0 sandeep    (501) staff       (20)      289 2023-06-28 11:01:16.000000 consumableai-1.0.2/consumableai.egg-info/SOURCES.txt
--rw-r--r--   0 sandeep    (501) staff       (20)        1 2023-06-28 11:01:16.000000 consumableai-1.0.2/consumableai.egg-info/dependency_links.txt
--rw-r--r--   0 sandeep    (501) staff       (20)       56 2023-06-28 11:01:16.000000 consumableai-1.0.2/consumableai.egg-info/entry_points.txt
--rw-r--r--   0 sandeep    (501) staff       (20)       53 2023-06-28 11:01:16.000000 consumableai-1.0.2/consumableai.egg-info/requires.txt
--rw-r--r--   0 sandeep    (501) staff       (20)       13 2023-06-28 11:01:16.000000 consumableai-1.0.2/consumableai.egg-info/top_level.txt
--rw-r--r--   0 sandeep    (501) staff       (20)       38 2023-06-28 11:01:16.968331 consumableai-1.0.2/setup.cfg
--rw-r--r--   0 sandeep    (501) staff       (20)      633 2023-06-28 08:58:50.000000 consumableai-1.0.2/setup.py
+drwxr-xr-x   0 sandeep    (501) staff       (20)        0 2023-08-03 13:02:52.475793 consumableai-1.0.3/
+-rw-r--r--   0 sandeep    (501) staff       (20)     1070 2023-06-01 16:21:54.000000 consumableai-1.0.3/LICENSE
+-rw-r--r--   0 sandeep    (501) staff       (20)     1817 2023-08-03 13:02:52.475624 consumableai-1.0.3/PKG-INFO
+-rw-r--r--   0 sandeep    (501) staff       (20)     1625 2023-06-02 08:23:20.000000 consumableai-1.0.3/README.md
+drwxr-xr-x   0 sandeep    (501) staff       (20)        0 2023-08-03 13:02:52.474563 consumableai-1.0.3/consumableai/
+-rw-r--r--   0 sandeep    (501) staff       (20)        0 2023-05-29 10:28:08.000000 consumableai-1.0.3/consumableai/__init__.py
+-rw-r--r--   0 sandeep    (501) staff       (20)     6955 2023-08-03 12:59:29.000000 consumableai-1.0.3/consumableai/cli.py
+drwxr-xr-x   0 sandeep    (501) staff       (20)        0 2023-08-03 13:02:52.475430 consumableai-1.0.3/consumableai.egg-info/
+-rw-r--r--   0 sandeep    (501) staff       (20)     1817 2023-08-03 13:02:52.000000 consumableai-1.0.3/consumableai.egg-info/PKG-INFO
+-rw-r--r--   0 sandeep    (501) staff       (20)      289 2023-08-03 13:02:52.000000 consumableai-1.0.3/consumableai.egg-info/SOURCES.txt
+-rw-r--r--   0 sandeep    (501) staff       (20)        1 2023-08-03 13:02:52.000000 consumableai-1.0.3/consumableai.egg-info/dependency_links.txt
+-rw-r--r--   0 sandeep    (501) staff       (20)       56 2023-08-03 13:02:52.000000 consumableai-1.0.3/consumableai.egg-info/entry_points.txt
+-rw-r--r--   0 sandeep    (501) staff       (20)       53 2023-08-03 13:02:52.000000 consumableai-1.0.3/consumableai.egg-info/requires.txt
+-rw-r--r--   0 sandeep    (501) staff       (20)       13 2023-08-03 13:02:52.000000 consumableai-1.0.3/consumableai.egg-info/top_level.txt
+-rw-r--r--   0 sandeep    (501) staff       (20)       38 2023-08-03 13:02:52.475841 consumableai-1.0.3/setup.cfg
+-rw-r--r--   0 sandeep    (501) staff       (20)      633 2023-08-03 12:59:59.000000 consumableai-1.0.3/setup.py
```

### Comparing `consumableai-1.0.2/LICENSE` & `consumableai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `consumableai-1.0.2/PKG-INFO` & `consumableai-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consumableai
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `consumableai-1.0.2/README.md` & `consumableai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `consumableai-1.0.2/consumableai/cli.py` & `consumableai-1.0.3/consumableai/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,24 +91,38 @@
             port=port,
             database=database,
             user=username,
             password=password
         )
 
         if not all_schemas and all_tables:
-            query = '''SELECT table_schema as schema, table_name as table, column_name as "column name", data_type as "data type", is_nullable as constraint
+            if len(all_tables) == 1:
+                query = '''SELECT table_schema as schema, table_name as table, column_name as "column name", data_type as "data type", is_nullable as constraint
+                    FROM information_schema.columns
+                    where 1=1
+                    and table_name = %s
+                    '''
+            else:    
+                query = '''SELECT table_schema as schema, table_name as table, column_name as "column name", data_type as "data type", is_nullable as constraint
                     FROM information_schema.columns
                     where 1=1
                     and table_name in %s
                     '''
             df = pd.read_sql(query, conn, index_col=None, params=(
                 tuple(all_tables)))
 
         if all_schemas and not all_tables:
-            query = '''SELECT table_schema as schema, table_name as table, column_name as "column name", data_type as "data type", is_nullable as constraint
+            if len(all_schemas) == 1:
+                query = '''SELECT table_schema as schema, table_name as table, column_name as "column name", data_type as "data type", is_nullable as constraint
+                    FROM information_schema.columns
+                    where 1=1
+                    and table_schema = %s
+                    '''
+            else: 
+                query = '''SELECT table_schema as schema, table_name as table, column_name as "column name", data_type as "data type", is_nullable as constraint
                     FROM information_schema.columns
                     where 1=1
                     and table_schema in %s
                     '''
             df = pd.read_sql(query, conn, index_col=None, params=(
                 tuple(all_schemas)))
```

### Comparing `consumableai-1.0.2/consumableai.egg-info/PKG-INFO` & `consumableai-1.0.3/consumableai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consumableai
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `consumableai-1.0.2/setup.py` & `consumableai-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='consumableai',
-    version='1.0.2',
+    version='1.0.3',
     packages=['consumableai'],
     entry_points={
         'console_scripts': [
             'consumableai=consumableai.cli:main',
         ],
     },
     scripts=['consumableai/cli.py'],
```

