# Comparing `tmp/mtsql-1.4.202308011012-py3-none-any.whl.zip` & `tmp/mtsql-1.5.202308031654-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19218 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       44 b- defN 23-Mar-28 14:19 mt/sql/__init__.py
--rw-rw-r--  2.0 unx     9994 b- defN 23-May-07 05:12 mt/sql/base.py
--rw-rw-r--  2.0 unx     4894 b- defN 23-Mar-28 14:19 mt/sql/mysql.py
--rw-rw-r--  2.0 unx    65229 b- defN 23-Aug-01 10:12 mt/sql/psql.py
--rw-rw-r--  2.0 unx     8678 b- defN 23-Mar-28 14:19 mt/sql/sqlite.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Aug-01 10:12 mt/sql/version.py
--rw-rw-r--  2.0 unx     1070 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/LICENSE
--rw-rw-r--  2.0 unx      597 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/RECORD
-11 files, 91860 bytes uncompressed, 17764 bytes compressed:  80.7%
+Zip file size: 19266 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
+-rw-r--r--  2.0 unx     9994 b- defN 23-May-11 07:16 mt/sql/base.py
+-rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
+-rw-r--r--  2.0 unx    65391 b- defN 23-Aug-03 16:53 mt/sql/psql.py
+-rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Aug-03 16:54 mt/sql/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Aug-03 16:54 mtsql-1.5.202308031654.dist-info/LICENSE
+-rw-r--r--  2.0 unx      597 b- defN 23-Aug-03 16:54 mtsql-1.5.202308031654.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 16:54 mtsql-1.5.202308031654.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Aug-03 16:54 mtsql-1.5.202308031654.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-Aug-03 16:54 mtsql-1.5.202308031654.dist-info/RECORD
+11 files, 92022 bytes uncompressed, 17812 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.4.202308011012.dist-info/LICENSE
+Filename: mtsql-1.5.202308031654.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.4.202308011012.dist-info/METADATA
+Filename: mtsql-1.5.202308031654.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.4.202308011012.dist-info/WHEEL
+Filename: mtsql-1.5.202308031654.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.4.202308011012.dist-info/top_level.txt
+Filename: mtsql-1.5.202308031654.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.4.202308011012.dist-info/RECORD
+Filename: mtsql-1.5.202308031654.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/psql.py

```diff
@@ -710,40 +710,45 @@
     )
 
 
 def vacuum_table(
     table_name,
     engine,
     schema: tp.Optional[str] = None,
+    full: bool = False,
     nb_trials: int = 3,
     logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Vacuums a table of a schema.
 
     Parameters
     ----------
     table_name: str
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
+    full : bool
+        whether or not to do a full vacuuming
     nb_trials: int
         number of query trials
     logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns
     """
     frame_sql_str = frame_sql(table_name, schema=schema)
     engine2 = engine.execution_options(isolation_level="AUTOCOMMIT")
-    return exec_sql(
-        f"VACUUM {frame_sql_str};", engine2, nb_trials=nb_trials, logger=logger
-    )
+    if full:
+        stmt = f"VACUUM FULL {frame_sql_str};"
+    else:
+        stmt = f"VACUUM {frame_sql_str};"
+    return exec_sql(stmt, engine2, nb_trials=nb_trials, logger=logger)
 
 
 def drop_table(
     table_name,
     engine,
     schema: tp.Optional[str] = None,
     restrict=True,
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('08')
-VERSION_DAY = int('01')
-VERSION_HOUR = int('10')
-VERSION_MINUTE = int('12')
+VERSION_DAY = int('03')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('54')
 MAJOR_VERSION = 1
-MINOR_VERSION = 4
-PATCH_VERSION = 202308011012
-version_date = '2023/08/01 10:12'
+MINOR_VERSION = 5
+PATCH_VERSION = 202308031654
+version_date = '2023/08/03 16:54'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.4.202308011012.dist-info/LICENSE` & `mtsql-1.5.202308031654.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.4.202308011012.dist-info/METADATA` & `mtsql-1.5.202308031654.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.4.202308011012
+Version: 1.5.202308031654
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

## Comparing `mtsql-1.4.202308011012.dist-info/RECORD` & `mtsql-1.5.202308031654.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mt/sql/__init__.py,sha256=b7zO50apZxt9Hg2eOkJhRLrXgACR8eS5b-Rphdn5qNQ,44
 mt/sql/base.py,sha256=sFr7O_Odfsf2AHr9kq3DXGCAFInCKgHSgLJaen507_I,9994
 mt/sql/mysql.py,sha256=n2ENDctdUqZuSaDAcrqZYtPtawq3Wx4dOPCRsCB5Q4w,4894
-mt/sql/psql.py,sha256=xzxYkgqmtM081cOKRfczbk5bW9Osp4d3S2zq7g-_2n0,65229
+mt/sql/psql.py,sha256=xD-Kg0pTFl3KoMRnTf6xOvjd2rFYsPbV10jCrS-rFeY,65391
 mt/sql/sqlite.py,sha256=T2ak_hhNi_zRfpg_gp8JhNHn7D2kl4i-Ey6-9ANMtz0,8678
-mt/sql/version.py,sha256=1zg-L-U2I2GzgDToL-mg_6LpqsQdAxue2MRfPsujyq0,396
-mtsql-1.4.202308011012.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtsql-1.4.202308011012.dist-info/METADATA,sha256=lCQD-yX7uV5PTUAaaarM-Es4J35FiqZf37xem_0zRIg,597
-mtsql-1.4.202308011012.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtsql-1.4.202308011012.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtsql-1.4.202308011012.dist-info/RECORD,,
+mt/sql/version.py,sha256=-npfHWfbYul3yt2vQJDJ8WwhNYxEw9uSGJkqOIlRUTQ,396
+mtsql-1.5.202308031654.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtsql-1.5.202308031654.dist-info/METADATA,sha256=wk53uyZWUiqxtv9lbyjk6KXmO2qjLaEKFsRxsGG8Efo,597
+mtsql-1.5.202308031654.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtsql-1.5.202308031654.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtsql-1.5.202308031654.dist-info/RECORD,,
```

