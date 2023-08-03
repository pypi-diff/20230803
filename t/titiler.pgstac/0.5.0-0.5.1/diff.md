# Comparing `tmp/titiler.pgstac-0.5.0.tar.gz` & `tmp/titiler.pgstac-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.pgstac-0.5.0.tar", last modified: Thu Jul 20 10:46:30 2023, max compression
+gzip compressed data, was "titiler.pgstac-0.5.1.tar", last modified: Thu Aug  3 14:33:51 2023, max compression
```

## Comparing `titiler.pgstac-0.5.0.tar` & `titiler.pgstac-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1097 2023-07-20 10:45:45.444031 titiler.pgstac-0.5.0/LICENSE
--rw-r--r--   0        0        0     4459 2023-07-20 10:45:45.444031 titiler.pgstac-0.5.0/README.md
--rw-r--r--   0        0        0     2558 2023-07-20 10:45:45.552033 titiler.pgstac-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/__init__.py
--rw-r--r--   0        0        0      874 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/db.py
--rw-r--r--   0        0        0     5129 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/dependencies.py
--rw-r--r--   0        0        0    37947 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/factory.py
--rw-r--r--   0        0        0       91 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/logger.py
--rw-r--r--   0        0        0     7780 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/main.py
--rw-r--r--   0        0        0     5913 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/model.py
--rw-r--r--   0        0        0    13737 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/mosaic.py
--rw-r--r--   0        0        0     3037 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/reader.py
--rw-r--r--   0        0        0     3542 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/settings.py
--rw-r--r--   0        0        0    10268 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/templates/index.html
--rw-r--r--   0        0        0      834 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/utils.py
--rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 titiler.pgstac-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-08-03 14:33:18.331355 titiler.pgstac-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4459 2023-08-03 14:33:18.331355 titiler.pgstac-0.5.1/README.md
+-rw-r--r--   0        0        0     2579 2023-08-03 14:33:18.455352 titiler.pgstac-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/__init__.py
+-rw-r--r--   0        0        0      874 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/db.py
+-rw-r--r--   0        0        0     5129 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/dependencies.py
+-rw-r--r--   0        0        0    37947 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/factory.py
+-rw-r--r--   0        0        0       91 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/logger.py
+-rw-r--r--   0        0        0     7780 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/main.py
+-rw-r--r--   0        0        0     5913 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/model.py
+-rw-r--r--   0        0        0    13737 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/mosaic.py
+-rw-r--r--   0        0        0     3037 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/reader.py
+-rw-r--r--   0        0        0     3542 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/settings.py
+-rw-r--r--   0        0        0    10268 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/templates/index.html
+-rw-r--r--   0        0        0      834 2023-08-03 14:33:18.459352 titiler.pgstac-0.5.1/titiler/pgstac/utils.py
+-rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 titiler.pgstac-0.5.1/PKG-INFO
```

### Comparing `titiler.pgstac-0.5.0/LICENSE` & `titiler.pgstac-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/README.md` & `titiler.pgstac-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/pyproject.toml` & `titiler.pgstac-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,18 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
     "titiler.core>=0.12.0,<0.13",
     "titiler.mosaic>=0.12.0,<0.13",
     "geojson-pydantic~=0.6",
     "pydantic~=1.0",
+    "python-dotenv",
 ]
 dynamic = []
-version = "0.5.0"
+version = "0.5.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 psycopg = [
     "psycopg[pool]",
```

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/db.py` & `titiler.pgstac-0.5.1/titiler/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/dependencies.py` & `titiler.pgstac-0.5.1/titiler/pgstac/dependencies.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/factory.py` & `titiler.pgstac-0.5.1/titiler/pgstac/factory.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/main.py` & `titiler.pgstac-0.5.1/titiler/pgstac/main.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/model.py` & `titiler.pgstac-0.5.1/titiler/pgstac/model.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/mosaic.py` & `titiler.pgstac-0.5.1/titiler/pgstac/mosaic.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/reader.py` & `titiler.pgstac-0.5.1/titiler/pgstac/reader.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/settings.py` & `titiler.pgstac-0.5.1/titiler/pgstac/settings.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/templates/index.html` & `titiler.pgstac-0.5.1/titiler/pgstac/templates/index.html`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/titiler/pgstac/utils.py` & `titiler.pgstac-0.5.1/titiler/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.5.0/PKG-INFO` & `titiler.pgstac-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 0.5.0
+Version: 0.5.1
 Summary: Connect PgSTAC and TiTiler.
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,pgSTAC
 Author-email: Vincent Sarago <vincent@developmentseed.com>,David Bitner <david@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.5.0 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.5.1 Summary: Connect
 PgSTAC and TiTiler. Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile
 server,pgSTAC Author-email: Vincent Sarago
 developmentseed.com>,David Bitner
 developmentseed.com> Requires-Python: >=3.8 Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

