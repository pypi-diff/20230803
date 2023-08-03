# Comparing `tmp/envguardian-1.0.0.tar.gz` & `tmp/envguardian-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envguardian-1.0.0.tar", max compression
+gzip compressed data, was "envguardian-1.1.0.tar", max compression
```

## Comparing `envguardian-1.0.0.tar` & `envguardian-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2023-08-03 13:49:23.759431 envguardian-1.0.0/README.md
--rw-r--r--   0        0        0       21 2023-08-03 12:41:41.990789 envguardian-1.0.0/envguardian/__init__.py
--rw-r--r--   0        0        0      291 2023-08-03 13:03:17.998126 envguardian-1.0.0/envguardian/_coercers.py
--rw-r--r--   0        0        0     1092 2023-08-03 13:07:28.415875 envguardian-1.0.0/envguardian/_utils.py
--rw-r--r--   0        0        0      731 2023-08-03 12:38:45.768498 envguardian-1.0.0/envguardian/_validators.py
--rw-r--r--   0        0        0     2848 2023-08-03 13:26:34.598092 envguardian-1.0.0/envguardian/env.py
--rw-r--r--   0        0        0      329 2023-08-03 14:02:52.868698 envguardian-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 envguardian-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2112 2023-08-03 16:26:14.871232 envguardian-1.1.0/README.md
+-rw-r--r--   0        0        0       20 2023-08-03 18:57:55.312794 envguardian-1.1.0/envguardian/__init__.py
+-rw-r--r--   0        0        0      295 2023-08-03 16:12:41.304408 envguardian-1.1.0/envguardian/_coercers.py
+-rw-r--r--   0        0        0     3048 2023-08-03 19:42:03.622927 envguardian-1.1.0/envguardian/_env.py
+-rw-r--r--   0        0        0      966 2023-08-03 19:11:48.536077 envguardian-1.1.0/envguardian/_utils.py
+-rw-r--r--   0        0        0      735 2023-08-03 16:12:41.281373 envguardian-1.1.0/envguardian/_validators.py
+-rw-r--r--   0        0        0      328 2023-08-03 21:08:35.982300 envguardian-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2710 1970-01-01 00:00:00.000000 envguardian-1.1.0/PKG-INFO
```

### Comparing `envguardian-1.0.0/envguardian/_utils.py` & `envguardian-1.1.0/envguardian/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from typing import Dict, Any, Callable
 
 
-def get_schema_key_value_pair_from_environment_variables(validation_schema, values_dict) -> Dict[str, Any]:
+def get_schema_key_value_pair_from_environment_variables(validation_schema, values_dict):
     """
     This function gets the key-value pair of the defined keys in the validation schema from another dictionary
     :param validation_schema:
     :param values_dict:
     :return: Dict[str, Any]
     """
     schema_keys = list(validation_schema)
 
-    schema_values: Dict[str, Any] = {}
+    schema_values = {}
 
     for schema_key in schema_keys:
         schema_values[schema_key] = values_dict.get(schema_key, None)
 
     return schema_values
 
 
-def validate_dictionary_against_validation_schema(validation_schema: Dict[str, Callable],
-                                                  candidate_dict: Dict[str, Any]) -> [bool | str]:
+def validate_dictionary_against_validation_schema(validation_schema,
+                                                  candidate_dict):
     """
     This function validates a candidate dict against a validation_schema
 
     :param validation_schema: Dict[str, Any]
     :param candidate_dict: Dict[str, Any]
     :return: [bool | str]
     """
```

### Comparing `envguardian-1.0.0/envguardian/_validators.py` & `envguardian-1.1.0/envguardian/_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     return type(candidate).__name__ == 'str' or f"`{candidate}` is not a string"
 
 
 def enum_validator(candidate, choices):
     return candidate in choices or f"`{candidate}` is not one of: {choices}"
 
 
-def int_validator(candidate):
+def integer_validator(candidate):
     try:
         int(candidate)
         return True
     except:
         return f"`{candidate}` is not an integer"
```

### Comparing `envguardian-1.0.0/envguardian/env.py` & `envguardian-1.1.0/envguardian/_env.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import functools
 import importlib
 import os
-from typing import List
 
-from envguardian._coercers import *
-from envguardian._utils import *
-from envguardian._validators import *
+from ._coercers import string_coercer, float_coercer, boolean_coercer, enum_coercer, integer_coercer
+from ._utils import get_schema_key_value_pair_from_environment_variables, \
+    validate_dictionary_against_validation_schema
+from ._validators import string_validator, float_validator, enum_validator, integer_validator, \
+    boolean_validator
 
 
 def get_schema():
     return getattr(importlib.import_module('Env'), 'env_schema', None)
 
 
 class Env:
 
-    def __init__(self, validation_schema: Dict[str, Callable]):
+    def __init__(self, validation_schema):
         self.schema = validation_schema
 
     @staticmethod
     def string():
         """
         String Schema definition. Returns the string validator and coercer
         :return:
         """
         return string_validator, string_coercer
 
     @staticmethod
-    def int():
+    def integer():
         """
         Integer Schema definition. Returns the int validator and coercer
         :return:
         """
-        return int_validator, int_coercer
+        return integer_validator, integer_coercer
 
     @staticmethod
     def float():
         """
         Float schema definition. Returns the float validator and coercer
         :return:
         """
         return float_validator, float_coercer
 
     @staticmethod
-    def enum(choices: List[Any]):
+    def enum(choices):
         """
         Enum schema definition. Returns the enum validator and coercer. Coercer casts to string
         :return:
         """
         return functools.partial(enum_validator, choices=choices), enum_coercer
 
     @staticmethod
@@ -67,41 +68,44 @@
         imported_schema = get_schema()
 
         if not imported_schema and not validation_schema:
             print('Invalid Validation Schema')
 
             return
 
-        schema = imported_schema or validation_schema
+        schema = validation_schema or imported_schema
 
         candidate_dict = get_schema_key_value_pair_from_environment_variables(schema, dict(os.environ))
 
         validation_results = validate_dictionary_against_validation_schema(schema, candidate_dict)
 
-        failed_validations: Dict[str, str] = {}
+        failed_validations = {}
 
         for index, candidate in enumerate(candidate_dict):
-            if validation_results[index] == True:
+            if validation_results[index] is True:
                 continue
 
             failed_validations[candidate] = validation_results[index]
 
         if len(failed_validations):
-            raise Exception(str(failed_validations))
+            raise ValueError(str(failed_validations))
 
     @staticmethod
     def get(environment_variable, validation_schema=None):
         imported_schema = get_schema()
 
         if not imported_schema and not validation_schema:
             print('Invalid Validation Schema')
 
             return
 
-        schema = imported_schema or validation_schema
+        schema = validation_schema or imported_schema
 
         val = os.environ.get(environment_variable, None)
 
         if not val:
             return None
 
         return schema.get(environment_variable)[1](val)
+
+
+__all__ = ['Env']
```

