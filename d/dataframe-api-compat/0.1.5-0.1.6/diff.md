# Comparing `tmp/dataframe_api_compat-0.1.5.tar.gz` & `tmp/dataframe_api_compat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_api_compat-0.1.5.tar", last modified: Wed Aug  2 19:22:09 2023, max compression
+gzip compressed data, was "dataframe_api_compat-0.1.6.tar", last modified: Wed Aug  2 19:24:42 2023, max compression
```

## Comparing `dataframe_api_compat-0.1.5.tar` & `dataframe_api_compat-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.5/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.5/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.048094 dataframe_api_compat-0.1.5/dataframe_api_compat/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      184 2023-08-02 18:57:06.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/__init__.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4298 2023-08-02 15:50:33.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28860 2023-08-02 15:50:34.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/pandas_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3740 2023-08-02 15:47:51.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25380 2023-08-02 16:45:27.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/polars_standard.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:14:05.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/py.typed
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      500 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.5/pyproject.toml
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      947 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.5/setup.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.6/LICENSE
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.6/README.md
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/dataframe_api_compat/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      184 2023-08-02 18:57:06.000000 dataframe_api_compat-0.1.6/dataframe_api_compat/__init__.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/dataframe_api_compat/pandas_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4298 2023-08-02 15:50:33.000000 dataframe_api_compat-0.1.6/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28860 2023-08-02 15:50:34.000000 dataframe_api_compat-0.1.6/dataframe_api_compat/pandas_standard/pandas_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/dataframe_api_compat/polars_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3755 2023-08-02 19:23:24.000000 dataframe_api_compat-0.1.6/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25380 2023-08-02 16:45:27.000000 dataframe_api_compat-0.1.6/dataframe_api_compat/polars_standard/polars_standard.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:14:05.000000 dataframe_api_compat-0.1.6/dataframe_api_compat/py.typed
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/dataframe_api_compat.egg-info/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:24:42.000000 dataframe_api_compat-0.1.6/dataframe_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      500 2023-08-02 19:24:42.000000 dataframe_api_compat-0.1.6/dataframe_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 19:24:42.000000 dataframe_api_compat-0.1.6/dataframe_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 19:24:42.000000 dataframe_api_compat-0.1.6/dataframe_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.6/pyproject.toml
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      947 2023-08-02 19:24:42.958097 dataframe_api_compat-0.1.6/setup.cfg
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.6/setup.py
```

### Comparing `dataframe_api_compat-0.1.5/LICENSE` & `dataframe_api_compat-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.5/PKG-INFO` & `dataframe_api_compat-0.1.6/dataframe_api_compat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dataframe_api_compat
-Version: 0.1.5
+Name: dataframe-api-compat
+Version: 0.1.6
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dataframe_api_compat-0.1.5/README.md` & `dataframe_api_compat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/__init__.py` & `dataframe_api_compat-0.1.6/dataframe_api_compat/pandas_standard/__init__.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/pandas_standard.py` & `dataframe_api_compat-0.1.6/dataframe_api_compat/pandas_standard/pandas_standard.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/__init__.py` & `dataframe_api_compat-0.1.6/dataframe_api_compat/polars_standard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 ) -> PolarsColumn[Any]:
     return PolarsColumn(
         pl.Series(values=sequence, dtype=_map_standard_to_polars_dtypes(dtype), name=name)
     )
 
 
 def convert_to_standard_compliant_dataframe(
-    df: pl.DataFrame, api_version: str | None = None
+    df: pl.DataFrame | pl.LazyFrame, api_version: str | None = None
 ) -> PolarsDataFrame:
     if api_version is None:
         api_version = "2023.08"
     if api_version != "2023.08":  # pragma: no cover
         raise ValueError(
             f"Unknown api_version: {api_version}. Expected: '2023.08', or None"
         )
```

### Comparing `dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/polars_standard.py` & `dataframe_api_compat-0.1.6/dataframe_api_compat/polars_standard/polars_standard.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/PKG-INFO` & `dataframe_api_compat-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dataframe-api-compat
-Version: 0.1.5
+Name: dataframe_api_compat
+Version: 0.1.6
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dataframe_api_compat-0.1.5/setup.cfg` & `dataframe_api_compat-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dataframe_api_compat
-version = 0.1.5
+version = 0.1.6
 description = Implementation of the DataFrame Standard for pandas and polars
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/data-apis/dataframe-api-compat
 author = Marco Gorelli
 license = MIT
 license_files = LICENSE
```

