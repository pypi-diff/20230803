# Comparing `tmp/jsno-1.0.5.tar.gz` & `tmp/jsno-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.5.tar", last modified: Tue Aug  1 12:18:00 2023, max compression
+gzip compressed data, was "jsno-1.0.6.tar", last modified: Thu Aug  3 10:41:18 2023, max compression
```

## Comparing `jsno-1.0.5.tar` & `jsno-1.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.653600 jsno-1.0.5/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.5/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)    10756 2023-08-01 12:18:00.653119 jsno-1.0.5/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     9082 2023-08-01 12:15:43.000000 jsno-1.0.5/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.647870 jsno-1.0.5/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1748 2023-08-01 12:17:09.000000 jsno-1.0.5/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2316 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4542 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.0.5/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      630 2023-07-29 19:08:24.000000 jsno-1.0.5/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5243 2023-07-29 19:40:07.000000 jsno-1.0.5/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     3976 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      882 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.649085 jsno-1.0.5/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)    10756 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      568 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      639 2023-08-01 12:17:32.000000 jsno-1.0.5/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-08-01 12:18:00.653705 jsno-1.0.5/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.652546 jsno-1.0.5/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1223 2023-07-29 19:21:09.000000 jsno-1.0.5/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.0.5/tests/test_ast_example.py
--rw-r--r--   0 pekka      (501) staff       (20)     4205 2023-07-29 18:53:29.000000 jsno-1.0.5/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 18:50:18.000000 jsno-1.0.5/tests/test_dates.py
--rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.0.5/tests/test_dumps_and_loads.py
--rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.0.5/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 18:53:15.000000 jsno-1.0.5/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.0.5/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 18:45:56.000000 jsno-1.0.5/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4437 2023-07-29 18:50:19.000000 jsno-1.0.5/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.0.5/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 10:41:18.187160 jsno-1.0.6/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.6/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)    10475 2023-08-03 10:41:18.186825 jsno-1.0.6/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)     8801 2023-08-03 10:41:05.000000 jsno-1.0.6/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 10:41:18.181425 jsno-1.0.6/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1748 2023-08-03 10:40:14.000000 jsno-1.0.6/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2316 2023-07-29 19:39:45.000000 jsno-1.0.6/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4542 2023-07-29 19:39:45.000000 jsno-1.0.6/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.0.6/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      630 2023-07-29 19:08:24.000000 jsno-1.0.6/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5587 2023-08-03 10:38:04.000000 jsno-1.0.6/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3976 2023-07-29 19:39:45.000000 jsno-1.0.6/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      882 2023-07-29 19:39:45.000000 jsno-1.0.6/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.0.6/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 10:41:18.182958 jsno-1.0.6/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)    10475 2023-08-03 10:41:18.000000 jsno-1.0.6/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      568 2023-08-03 10:41:18.000000 jsno-1.0.6/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-08-03 10:41:18.000000 jsno-1.0.6/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-08-03 10:41:18.000000 jsno-1.0.6/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-08-03 10:41:18.000000 jsno-1.0.6/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      639 2023-08-03 10:40:19.000000 jsno-1.0.6/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-08-03 10:41:18.187229 jsno-1.0.6/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 10:41:18.186507 jsno-1.0.6/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     1223 2023-07-29 19:21:09.000000 jsno-1.0.6/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.0.6/tests/test_ast_example.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4205 2023-07-29 18:53:29.000000 jsno-1.0.6/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3220 2023-08-03 10:39:19.000000 jsno-1.0.6/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.0.6/tests/test_dumps_and_loads.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.0.6/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 18:53:15.000000 jsno-1.0.6/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.0.6/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 18:45:56.000000 jsno-1.0.6/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4437 2023-07-29 18:50:19.000000 jsno-1.0.6/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.0.6/tests/test_variant.py
```

### Comparing `jsno-1.0.5/LICENSE` & `jsno-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/PKG-INFO` & `jsno-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.5
+Version: 1.0.6
 Summary: Convert Python data to and from json-compatible data structures
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -255,28 +255,14 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
-## Jsonification as string
-
-For types that can be converted to strings and back, jsno has a convenience
-function _jsonify_as_string_. For example, to provide jsonification for the _furl_
-class of the furl library:
-
-```py
-from furl import furl
-
-jsno.jsnonify_as_string(furl)
-```
-
-
-
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
 defined using a hierarchy of dataclasses:
```

### Comparing `jsno-1.0.5/README.md` & `jsno-1.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -219,28 +219,14 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
-## Jsonification as string
-
-For types that can be converted to strings and back, jsno has a convenience
-function _jsonify_as_string_. For example, to provide jsonification for the _furl_
-class of the furl library:
-
-```py
-from furl import furl
-
-jsno.jsnonify_as_string(furl)
-```
-
-
-
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
 defined using a hierarchy of dataclasses:
```

### Comparing `jsno-1.0.5/jsno/__init__.py` & `jsno-1.0.6/jsno/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from jsno.unjsonify import unjsonify, UnjsonifyError
 from jsno.variant import get_variantfamily, variantfamily, variantlabel, VariantFamily
 
 # import to register jsonifiers
 import jsno.abc  # noqa
 
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 __all__ = [
     "dumps",
     "jsonify",
     "jsonify_as_string",
     "jsonify_with_method",
     "get_variantfamily",
```

### Comparing `jsno-1.0.5/jsno/abc.py` & `jsno-1.0.6/jsno/abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno/jsonify.py` & `jsno-1.0.6/jsno/jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno/jsonize.py` & `jsno-1.0.6/jsno/jsonize.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno/method.py` & `jsno-1.0.6/jsno/method.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno/standard.py` & `jsno-1.0.6/jsno/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,34 @@
         return as_type(int(ys), int(ms), int(ds))
     except ValueError as exc:
         detail = exc.args[0]
 
     raise_error(value, as_type, detail)
 
 
+# datetime.time
+
+
+@jsonify.register(datetime.time)
+def _(value):
+    return str(value)
+
+
+@unjsonify.register(datetime.time)
+def _(value, as_type):
+    typecheck(value, str, as_type)
+
+    try:
+        return datetime.time.fromisoformat(value)
+    except ValueError as exc:
+        detail = exc.args[0]
+
+    raise_error(value, as_type, detail)
+
+
 # datetime.datetime
 
 
 UTC = zoneinfo.ZoneInfo("UTC")
 
 
 def is_utc_datetime(dt) -> bool:
```

### Comparing `jsno-1.0.5/jsno/unjsonify.py` & `jsno-1.0.6/jsno/unjsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno/utils.py` & `jsno-1.0.6/jsno/utils.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno/variant.py` & `jsno-1.0.6/jsno/variant.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/jsno.egg-info/PKG-INFO` & `jsno-1.0.6/jsno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.5
+Version: 1.0.6
 Summary: Convert Python data to and from json-compatible data structures
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -255,28 +255,14 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
-## Jsonification as string
-
-For types that can be converted to strings and back, jsno has a convenience
-function _jsonify_as_string_. For example, to provide jsonification for the _furl_
-class of the furl library:
-
-```py
-from furl import furl
-
-jsno.jsnonify_as_string(furl)
-```
-
-
-
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
 defined using a hierarchy of dataclasses:
```

### Comparing `jsno-1.0.5/jsno.egg-info/SOURCES.txt` & `jsno-1.0.6/jsno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/pyproject.toml` & `jsno-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.5"
+version = "1.0.6"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `jsno-1.0.5/tests/test_abc.py` & `jsno-1.0.6/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_ast_example.py` & `jsno-1.0.6/tests/test_ast_example.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_dataclasses.py` & `jsno-1.0.6/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_dates.py` & `jsno-1.0.6/tests/test_dates.py`

 * *Files 20% similar despite different names*

```diff
@@ -83,7 +83,24 @@
         )
     )
 
 
 def test_unjsonify_datetime_failure():
     with pytest.raises(UnjsonifyError):
         unjsonify[datetime.datetime]('2023-13-13T12:34:56')
+
+
+def test_jsonify_time():
+    assert jsonify(datetime.time(23,59,59)) == "23:59:59"
+
+
+def test_unjsonify_time():
+    assert unjsonify[datetime.time]("23:59:59") == datetime.time(23,59,59)
+
+
+def test_unjsonify_time_failure():
+    with pytest.raises(UnjsonifyError):
+        unjsonify[datetime.time]("24:59:59")
+
+
+
+
```

### Comparing `jsno-1.0.5/tests/test_examples.py` & `jsno-1.0.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_jsonify.py` & `jsno-1.0.6/tests/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_methods.py` & `jsno-1.0.6/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_standard.py` & `jsno-1.0.6/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_unjsonify.py` & `jsno-1.0.6/tests/test_unjsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.5/tests/test_variant.py` & `jsno-1.0.6/tests/test_variant.py`

 * *Files identical despite different names*

