# Comparing `tmp/motorhead-0.2308.0.tar.gz` & `tmp/motorhead-0.2308.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motorhead-0.2308.0.tar", max compression
+gzip compressed data, was "motorhead-0.2308.1.tar", max compression
```

## Comparing `motorhead-0.2308.0.tar` & `motorhead-0.2308.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.0/LICENSE
--rw-r--r--   0        0        0     2100 2023-07-29 23:37:28.841882 motorhead-0.2308.0/README.md
--rw-r--r--   0        0        0     2038 2023-08-03 18:52:22.265079 motorhead-0.2308.0/motorhead/__init__.py
--rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.0/motorhead/bound_method_wrapper.py
--rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.0/motorhead/delete_rule.py
--rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.0/motorhead/model/__init__.py
--rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.0/motorhead/model/deleteresultmodel.py
--rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.0/motorhead/model/document.py
--rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.0/motorhead/model/objectid.py
--rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.0/motorhead/model/utcdatetime.py
--rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.0/motorhead/operator.py
--rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.0/motorhead/py.typed
--rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.0/motorhead/query.py
--rw-r--r--   0        0        0    28508 2023-08-03 18:51:22.611747 motorhead-0.2308.0/motorhead/service.py
--rw-r--r--   0        0        0     6022 2023-08-03 18:52:05.408756 motorhead-0.2308.0/motorhead/typing.py
--rw-r--r--   0        0        0     1678 2023-08-03 18:51:37.484136 motorhead-0.2308.0/motorhead/validator.py
--rw-r--r--   0        0        0     2824 2023-08-03 21:01:58.639960 motorhead-0.2308.0/pyproject.toml
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 motorhead-0.2308.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.1/LICENSE
+-rw-r--r--   0        0        0     2348 2023-08-03 21:23:41.370318 motorhead-0.2308.1/README.md
+-rw-r--r--   0        0        0     2038 2023-08-03 18:52:22.265079 motorhead-0.2308.1/motorhead/__init__.py
+-rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.1/motorhead/bound_method_wrapper.py
+-rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.1/motorhead/delete_rule.py
+-rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.1/motorhead/model/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.1/motorhead/model/deleteresultmodel.py
+-rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.1/motorhead/model/document.py
+-rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.1/motorhead/model/objectid.py
+-rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.1/motorhead/model/utcdatetime.py
+-rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.1/motorhead/operator.py
+-rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.1/motorhead/py.typed
+-rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.1/motorhead/query.py
+-rw-r--r--   0        0        0    28508 2023-08-03 18:51:22.611747 motorhead-0.2308.1/motorhead/service.py
+-rw-r--r--   0        0        0     6022 2023-08-03 18:52:05.408756 motorhead-0.2308.1/motorhead/typing.py
+-rw-r--r--   0        0        0     1678 2023-08-03 18:51:37.484136 motorhead-0.2308.1/motorhead/validator.py
+-rw-r--r--   0        0        0     2824 2023-08-03 21:24:25.476920 motorhead-0.2308.1/pyproject.toml
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 motorhead-0.2308.1/PKG-INFO
```

### Comparing `motorhead-0.2308.0/LICENSE` & `motorhead-0.2308.1/LICENSE`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/README.md` & `motorhead-0.2308.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Motorhead
 
-Async MongoDB with Pydantic v2+ - made easy.
+Async MongoDB with vanilla Pydantic v2+ - made easy.
 
 Key features:
 
-- Database **model** and API design with `Pydantic` v2+.
+- Database **model** and API design with vanilla `Pydantic` v2+.
 - Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.
+- ODM-like query builder for convenient, typed, and Pythonic query construction.
 - Declarative **index** specification.
 - Typed **utilities** for convenient model and API creation.
 - Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
+- Simplicity: by not being a classic ODM, the codebase is very simple and easy to understand (even contribute to) even for relative beginners.
 
-By providing a convenient, declarative middle layer between MongoDB and your API, `motorhead` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver). What's missing is the built-in ODM performance and memory overhead, whose benefits are rarely felt when working with document databases.
+By providing a convenient, declarative middle layer between MongoDB and your API, `motorhead` is halfway between an object document mapper (based on vanilla `Pydantic`) and a database driver (by wrapping the official, async `motor` driver). What's missing is the built-in ODM performance and memory overhead, whose benefits are rarely felt when working with document databases.
 
 See the [full documentation here](https://volfpeter.github.io/motorhead/).
 
 ## Installation
 
 The library is available on PyPI and can be installed with:
```

### Comparing `motorhead-0.2308.0/motorhead/__init__.py` & `motorhead-0.2308.1/motorhead/__init__.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/bound_method_wrapper.py` & `motorhead-0.2308.1/motorhead/bound_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/delete_rule.py` & `motorhead-0.2308.1/motorhead/delete_rule.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/model/document.py` & `motorhead-0.2308.1/motorhead/model/document.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/model/objectid.py` & `motorhead-0.2308.1/motorhead/model/objectid.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/model/utcdatetime.py` & `motorhead-0.2308.1/motorhead/model/utcdatetime.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/operator.py` & `motorhead-0.2308.1/motorhead/operator.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/query.py` & `motorhead-0.2308.1/motorhead/query.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/service.py` & `motorhead-0.2308.1/motorhead/service.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/typing.py` & `motorhead-0.2308.1/motorhead/typing.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/motorhead/validator.py` & `motorhead-0.2308.1/motorhead/validator.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.0/pyproject.toml` & `motorhead-0.2308.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/motorhead"
 Documentation = "https://volfpeter.github.io/motorhead"
 
 [tool.poetry]
 name = "motorhead"
-version = "0.2308.0"
+version = "0.2308.1"
 description = "Async MongoDB with Pydantic - made easy."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "motorhead"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `motorhead-0.2308.0/PKG-INFO` & `motorhead-0.2308.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: motorhead
-Version: 0.2308.0
+Version: 0.2308.1
 Summary: Async MongoDB with Pydantic - made easy.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: motor (>=3.1.0,<4.0.0)
 Requires-Dist: pydantic (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Motorhead
 
-Async MongoDB with Pydantic v2+ - made easy.
+Async MongoDB with vanilla Pydantic v2+ - made easy.
 
 Key features:
 
-- Database **model** and API design with `Pydantic` v2+.
+- Database **model** and API design with vanilla `Pydantic` v2+.
 - Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.
+- ODM-like query builder for convenient, typed, and Pythonic query construction.
 - Declarative **index** specification.
 - Typed **utilities** for convenient model and API creation.
 - Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
+- Simplicity: by not being a classic ODM, the codebase is very simple and easy to understand (even contribute to) even for relative beginners.
 
-By providing a convenient, declarative middle layer between MongoDB and your API, `motorhead` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver). What's missing is the built-in ODM performance and memory overhead, whose benefits are rarely felt when working with document databases.
+By providing a convenient, declarative middle layer between MongoDB and your API, `motorhead` is halfway between an object document mapper (based on vanilla `Pydantic`) and a database driver (by wrapping the official, async `motor` driver). What's missing is the built-in ODM performance and memory overhead, whose benefits are rarely felt when working with document databases.
 
 See the [full documentation here](https://volfpeter.github.io/motorhead/).
 
 ## Installation
 
 The library is available on PyPI and can be installed with:
```

