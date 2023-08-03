# Comparing `tmp/dh_json_logic-1.2.1.tar.gz` & `tmp/dh_json_logic-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh_json_logic-1.2.1.tar", max compression
+gzip compressed data, was "dh_json_logic-1.2.2.tar", max compression
```

## Comparing `dh_json_logic-1.2.1.tar` & `dh_json_logic-1.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/LICENSE
--rw-r--r--   0        0        0     3169 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/README.md
--rw-r--r--   0        0        0    31272 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/dh_json_logic/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 dh_json_logic-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-03 08:42:42.109624 dh_json_logic-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3169 2023-08-03 08:42:42.109624 dh_json_logic-1.2.2/README.md
+-rw-r--r--   0        0        0    31460 2023-08-03 08:42:42.109624 dh_json_logic-1.2.2/dh_json_logic/__init__.py
+-rw-r--r--   0        0        0     1274 2023-08-03 08:42:42.109624 dh_json_logic-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 dh_json_logic-1.2.2/PKG-INFO
```

### Comparing `dh_json_logic-1.2.1/LICENSE` & `dh_json_logic-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.2.1/README.md` & `dh_json_logic-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.2.1/dh_json_logic/__init__.py` & `dh_json_logic-1.2.2/dh_json_logic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,18 +384,18 @@
     - For more then 3 arguments:
         - If the first argument evaluates to True then evaluate and return
           the second argument.
         - If the first argument evaluates to False then jump to the next pair
           (e.g.: from 0,1 to 2,3) and evaluate them.
     """
     for i in range(0, len(args) - 1, 2):
-        if _truthy(jsonLogic(args[i], data)):
-            return jsonLogic(args[i + 1], data)
+        if _truthy(_jsonLogic(args[i], data)):
+            return _jsonLogic(args[i + 1], data)
     if len(args) % 2:
-        return jsonLogic(args[-1], data)
+        return _jsonLogic(args[-1], data)
     else:
         return None
 
 
 def _iif(data, a, b, c):
     """
     Evaluate ternary expression and return corresponding evaluated
@@ -410,15 +410,15 @@
     If all arguments evaluate to True return the last (truthy) one (meaning
     that the whole expression evaluates to True).
     Otherwise return first countered falsy argument (meaning that the whole
     expression evaluates to False).
     """
     current = False
     for current in args:
-        current = jsonLogic(current, data)
+        current = _jsonLogic(current, data)
         if _falsy(current):
             return current  # First falsy argument
     return current  # Last argument
 
 
 def _or(data, *args):
     """
@@ -426,15 +426,15 @@
     If at least one argument evaluates to True - return it
     (meaning that the whole expression evaluates to True).
     Otherwise return the last (falsy) argument (meaning that the whole
     expression evaluates to False).
     """
     current = False
     for current in args:
-        current = jsonLogic(current, data)
+        current = _jsonLogic(current, data)
         if _truthy(current):
             return current  # First truthy argument
     return current  # Last argument
 
 
 _logical_operations = {
     'if': _if,
@@ -471,19 +471,19 @@
         {"%": [{"var": ""}, 2]}
     ]}
     calculates to: [1, 3, 5]
 
     If 'scopedData' argument does not evaluate to an array, an empty array
     is returned.
     """
-    scopedData = jsonLogic(scopedData, data)
+    scopedData = _jsonLogic(scopedData, data)
     if not _is_array(scopedData):
         return []
     return list(filter(
-        lambda datum: _truthy(jsonLogic(scopedLogic, datum)),
+        lambda datum: _truthy(_jsonLogic(scopedLogic, datum)),
         scopedData))
 
 
 def _map(data, scopedData, scopedLogic):
     """
     Apply 'scopedLogic' argument to each 'scopedData' element.
 
@@ -506,19 +506,19 @@
         {"*": [{"var": ""}, 2]}
     ]}
     calculates to: [2, 4, 6, 8, 10]
 
     If 'scopedData' argument does not evaluate to an array, an empty array
     is returned.
     """
-    scopedData = jsonLogic(scopedData, data)
+    scopedData = _jsonLogic(scopedData, data)
     if not _is_array(scopedData):
         return []
     return list(map(
-        lambda datum: jsonLogic(scopedLogic, datum),
+        lambda datum: _jsonLogic(scopedLogic, datum),
         scopedData))
 
 
 def _reduce(data, scopedData, scopedLogic, initial=None):
     """
     Apply 'scopedLogic' cumulatively to the elements in 'scopedData' argument,
     from left to right, so as to reduce the sequence it to a single value.
@@ -549,19 +549,19 @@
         0
     ]}
     calculates as: ((((1+2)+3)+4)+5) = 15
 
     If 'scopedData' argument does not evaluate to an array, the 'initial'
     value is returned.
     """
-    scopedData = jsonLogic(scopedData, data)
+    scopedData = _jsonLogic(scopedData, data)
     if not _is_array(scopedData):
         return initial
     return reduce(
-        lambda accumulator, current: jsonLogic(
+        lambda accumulator, current: _jsonLogic(
             scopedLogic, {'accumulator': accumulator, 'current': current}),
         scopedData, initial)
 
 
 def _all(data, scopedData, scopedLogic):
     """
     Check if 'scopedLogic' evaluates to a truthy value for all
@@ -590,21 +590,21 @@
 
     If 'scopedData' argument does not evaluate to an array or if the array
     is empty, False is returned.
 
     N.B.: According to current core JsonLogic evaluation of 'scopedData'
     elements stops upon encountering first falsy value.
     """
-    scopedData = jsonLogic(scopedData, data)
+    scopedData = _jsonLogic(scopedData, data)
     if not _is_array(scopedData):
         return False
     if len(scopedData) == 0:
         return False  # "all" of an empty set is false
     for datum in scopedData:
-        if _falsy(jsonLogic(scopedLogic, datum)):
+        if _falsy(_jsonLogic(scopedLogic, datum)):
             return False  # First falsy, short circuit
     return True  # All were truthy
 
 
 def _none(data, scopedData, scopedLogic):
     """
     Check if 'scopedLogic' evaluates to a truthy value for none of
@@ -768,24 +768,32 @@
     'missing_some': _missing_some
 }
 
 
 # MAIN LOGIC
 
 def jsonLogic(logic, data=None):
+    try:
+        return _jsonLogic(logic, data)
+    except TypeError as e:
+        logging.error("JsonLogic: %s", e)
+        return None
+
+
+def _jsonLogic(logic, data=None):
     """
     Evaluate provided JsonLogic using given data (if any).
     If a single JsonLogic rule is provided - return a single resulting value.
     If an array of JsonLogic rule is provided - return an array of each rule's
     resulting values.
     """
 
     # Is this an array of JsonLogic rules?
     if _is_array(logic):
-        return list(map(lambda sublogic: jsonLogic(sublogic, data), logic))
+        return list(map(lambda sublogic: _jsonLogic(sublogic, data), logic))
 
     # You've recursed to a primitive, stop!
     if not is_logic(logic):
         return logic
 
     # Get operator
     operator = _get_operator(logic)
@@ -803,15 +811,15 @@
 
     # Next up, try applying scoped operations that manage their own data scopes
     # for each constituent operation
     if operator in _scoped_operations:
         return _scoped_operations[operator](data, *values)
 
     # Recursion!
-    values = [jsonLogic(val, data) for val in values]
+    values = [_jsonLogic(val, data) for val in values]
 
     # Apply data retrieval operations
     if operator in _data_operations:
         return _data_operations[operator](data, *values)
 
     # Apply simple custom operations (if any)
     if operator in _custom_operations:
```

### Comparing `dh_json_logic-1.2.1/pyproject.toml` & `dh_json_logic-1.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = [ "poetry_core>=1.6.1" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dh-json-logic"
-version = "1.2.1"
+version = "1.2.2"
 description = "A fork of https://github.com/YaraslauZhylko/json-logic-py/"
 readme="README.md"
 authors = [ "dearhealth" ]
 homepage = "https://github.com/dearhealth/json-logic-py"
 repository = "https://github.com/dearhealth/json-logic-py"
 
   [tool.poetry.dependencies]
```

### Comparing `dh_json_logic-1.2.1/PKG-INFO` & `dh_json_logic-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dh-json-logic
-Version: 1.2.1
+Version: 1.2.2
 Summary: A fork of https://github.com/YaraslauZhylko/json-logic-py/
 Home-page: https://github.com/dearhealth/json-logic-py
 Author: dearhealth
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

