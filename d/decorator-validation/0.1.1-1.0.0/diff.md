# Comparing `tmp/decorator_validation-0.1.1.tar.gz` & `tmp/decorator_validation-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_validation-0.1.1.tar", max compression
+gzip compressed data, was "decorator_validation-1.0.0.tar", max compression
```

## Comparing `decorator_validation-0.1.1.tar` & `decorator_validation-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       38 2023-08-03 14:40:11.351648 decorator_validation-0.1.1/decorator_validation/__init__.py
--rw-r--r--   0        0        0     2642 2023-08-03 14:13:48.790369 decorator_validation-0.1.1/decorator_validation/decorators.py
--rw-r--r--   0        0        0      518 2023-08-03 14:42:12.010260 decorator_validation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1072 2023-08-03 14:10:47.510415 decorator_validation-0.1.1/README.md
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 decorator_validation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-08-03 14:40:11.351648 decorator_validation-1.0.0/decorator_validation/__init__.py
+-rw-r--r--   0        0        0     2642 2023-08-03 14:13:48.790369 decorator_validation-1.0.0/decorator_validation/decorators.py
+-rw-r--r--   0        0        0      518 2023-08-03 14:45:33.376432 decorator_validation-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1310 2023-08-03 14:45:15.137378 decorator_validation-1.0.0/README.md
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 decorator_validation-1.0.0/PKG-INFO
```

### Comparing `decorator_validation-0.1.1/decorator_validation/decorators.py` & `decorator_validation-1.0.0/decorator_validation/decorators.py`

 * *Files identical despite different names*

### Comparing `decorator_validation-0.1.1/pyproject.toml` & `decorator_validation-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decorator_validation"
-version = "0.1.1"
+version = "1.0.0"
 description = ""
     authors = ["FailedRobot <sry@nomail.com>"]
 readme = "README.md"
 packages = [{include = "decorator_validation"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `decorator_validation-0.1.1/README.md` & `decorator_validation-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -18,22 +18,32 @@
         raise TypeError(...)
     if not isinstance(some_additional_info, dict):
         raise TypeError(...)
     # now begin to code...
 
 # now
 @validate_types(bar=(int,), message=(str,), some_additional_info=(dict,))
-def foo(bar: int, message: str):
+def foo(bar: int, message: str, , some_additional_info: dict):
+    # begin to code
+```
+
+If of course also supports multiple types:
+
+```python
+from pathlib import Path
+
+@validate_types(path=(str, Path), message=(str,))
+def foo(path: str | Path, message: str):
     # begin to code
 ```
 
 Do you want to convert your input-types fast and without clutter?
 
 ```python
 def from_dict(dict_: dict):
     return (dict_.get('bar'), dict_.get('message'), dict_.get('some_additional_info')), {}
 
 @convert_with(from_dict)
 def foo(bar: int, message:str, some_additional_info: dict):
     ...
 
-```
+```
```

### Comparing `decorator_validation-0.1.1/PKG-INFO` & `decorator_validation-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-validation
-Version: 0.1.1
+Version: 1.0.0
 Summary: 
 Author: FailedRobot
 Author-email: sry@nomail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,22 +31,33 @@
         raise TypeError(...)
     if not isinstance(some_additional_info, dict):
         raise TypeError(...)
     # now begin to code...
 
 # now
 @validate_types(bar=(int,), message=(str,), some_additional_info=(dict,))
-def foo(bar: int, message: str):
+def foo(bar: int, message: str, , some_additional_info: dict):
+    # begin to code
+```
+
+If of course also supports multiple types:
+
+```python
+from pathlib import Path
+
+@validate_types(path=(str, Path), message=(str,))
+def foo(path: str | Path, message: str):
     # begin to code
 ```
 
 Do you want to convert your input-types fast and without clutter?
 
 ```python
 def from_dict(dict_: dict):
     return (dict_.get('bar'), dict_.get('message'), dict_.get('some_additional_info')), {}
 
 @convert_with(from_dict)
 def foo(bar: int, message:str, some_additional_info: dict):
     ...
 
 ```
+
```

