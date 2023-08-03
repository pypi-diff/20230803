# Comparing `tmp/packg-0.2.26.tar.gz` & `tmp/packg-0.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.26.tar", last modified: Thu Aug  3 08:05:11 2023, max compression
+gzip compressed data, was "packg-0.2.27.tar", last modified: Thu Aug  3 08:09:41 2023, max compression
```

## Comparing `packg-0.2.26.tar` & `packg-0.2.27.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.132194 packg-0.2.26/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.26/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-08-03 08:05:11.132194 packg-0.2.26/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-08-03 08:03:51.000000 packg-0.2.26/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.26/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-08-03 08:03:51.000000 packg-0.2.26/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-08-03 08:05:11.136195 packg-0.2.26/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.016193 packg-0.2.26/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.072193 packg-0.2.26/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/__main__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3097 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5871 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      544 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     8439 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.116194 packg-0.2.26/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      831 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/compressed.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4034 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/file_indexer.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/gitmatcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6252 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10990 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4027 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4890 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5959 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/misc.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2394 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/packaging.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/paths.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.120194 packg-0.2.26/src/packg/run/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3626 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/run/syncjupytext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.128194 packg-0.2.26/src/packg/strings/
--rw-------   0 gings    (14999) lmb-mit   (1061)      284 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/strings/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4842 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/strings/abbreviations.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1933 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/strings/base64utils.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      623 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/strings/quote_urlparse.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1968 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1407 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-08-03 08:03:51.000000 packg-0.2.26/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:05:11.092194 packg-0.2.26/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-08-03 08:05:10.000000 packg-0.2.26/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      955 2023-08-03 08:05:10.000000 packg-0.2.26/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-08-03 08:05:10.000000 packg-0.2.26/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-08-03 08:05:10.000000 packg-0.2.26/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-08-03 08:05:10.000000 packg-0.2.26/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.26/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:41.040805 packg-0.2.27/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.27/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-08-03 08:09:41.040805 packg-0.2.27/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-08-03 08:08:12.000000 packg-0.2.27/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.27/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-08-03 08:08:12.000000 packg-0.2.27/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-08-03 08:09:41.040805 packg-0.2.27/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:40.924803 packg-0.2.27/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:40.980804 packg-0.2.27/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/__main__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3097 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5871 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      544 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8439 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:41.024804 packg-0.2.27/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      849 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/compressed.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4034 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/file_indexer.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6252 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10990 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4027 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4890 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5959 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/misc.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2394 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/packaging.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/paths.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:41.024804 packg-0.2.27/src/packg/run/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3626 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/run/syncjupytext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:41.036805 packg-0.2.27/src/packg/strings/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      284 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/strings/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4842 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/strings/abbreviations.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1933 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/strings/base64utils.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      623 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/strings/quote_urlparse.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1968 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1407 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-08-03 08:08:12.000000 packg-0.2.27/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 08:09:41.000804 packg-0.2.27/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-08-03 08:09:40.000000 packg-0.2.27/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      955 2023-08-03 08:09:40.000000 packg-0.2.27/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-08-03 08:09:40.000000 packg-0.2.27/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-08-03 08:09:40.000000 packg-0.2.27/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-08-03 08:09:40.000000 packg-0.2.27/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.27/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.26/LICENSE` & `packg-0.2.27/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/PKG-INFO` & `packg-0.2.27/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.26
+Version: 0.2.27
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.26 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.27 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.26/README.md` & `packg-0.2.27/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/pyproject.toml` & `packg-0.2.27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/caching.py` & `packg-0.2.27/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/constclass.py` & `packg-0.2.27/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/debugging.py` & `packg-0.2.27/src/packg/debugging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/import_from_source.py` & `packg-0.2.27/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/iotools/__init__.py` & `packg-0.2.27/src/packg/iotools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,9 @@
     "load_json_xz",
     "dump_json_xz",
     "load_yaml",
     "loads_yaml",
     "dump_yaml",
     "dumps_yaml",
     "make_git_pathspec",
+    "make_index",
 ]
```

### Comparing `packg-0.2.26/src/packg/iotools/file_indexer.py` & `packg-0.2.27/src/packg/iotools/file_indexer.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/iotools/jsonext.py` & `packg-0.2.27/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.27/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/iotools/misc.py` & `packg-0.2.27/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/iotools/yamlext.py` & `packg-0.2.27/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/log.py` & `packg-0.2.27/src/packg/log.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/packaging.py` & `packg-0.2.27/src/packg/packaging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/paths.py` & `packg-0.2.27/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/run/syncjupytext.py` & `packg-0.2.27/src/packg/run/syncjupytext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/strings/abbreviations.py` & `packg-0.2.27/src/packg/strings/abbreviations.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/strings/base64utils.py` & `packg-0.2.27/src/packg/strings/base64utils.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/strings/quote_urlparse.py` & `packg-0.2.27/src/packg/strings/quote_urlparse.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/system.py` & `packg-0.2.27/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/tensors.py` & `packg-0.2.27/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg/typext.py` & `packg-0.2.27/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.26/src/packg.egg-info/PKG-INFO` & `packg-0.2.27/src/packg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.26
+Version: 0.2.27
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.26 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.27 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.26/src/packg.egg-info/SOURCES.txt` & `packg-0.2.27/src/packg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

