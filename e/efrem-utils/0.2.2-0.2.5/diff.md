# Comparing `tmp/efrem_utils-0.2.2.tar.gz` & `tmp/efrem_utils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.2.2.tar", max compression
+gzip compressed data, was "efrem_utils-0.2.5.tar", max compression
```

## Comparing `efrem_utils-0.2.2.tar` & `efrem_utils-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11573 2023-08-02 15:41:28.245768 efrem_utils-0.2.2/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.2.2/LICENSE
--rw-r--r--   0        0        0      361 2023-08-02 15:41:26.866041 efrem_utils-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.2.2/README.md
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    12856 2023-08-02 18:33:59.735966 efrem_utils-0.2.5/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.2.5/LICENSE
+-rw-r--r--   0        0        0      361 2023-08-02 18:34:14.279734 efrem_utils-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.2.5/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.2.5/PKG-INFO
```

### Comparing `efrem_utils-0.2.2/efrem_utils.py` & `efrem_utils-0.2.5/efrem_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 # --- # 
 
 class Case:
     class _Mode(Enum):
         match = 0 # pass same args, see if output matches
         validate = 1 # pass same args to both, see if kwargs.get("validator") passes
 
-    def __init__(self, function, *_, **kwargs):
+    def __init__(self, function = (lambda *args, **kwargs: ((args), kwargs) if kwargs else args), *_, **kwargs):
         if len(kwargs) == 0: self.mode = Case._Mode.match
         elif len(kwargs) == 1 and ("validator" in kwargs): self.mode = Case._Mode.validate; self.validator = kwargs["validator"]
         else: raise ValueError("Currently a not supported case")
         self.function = function
 
     def __repr__(self) -> str:
         return f"Case(function = {self.function.__name__}, mode = {self.mode})"
@@ -222,9 +222,40 @@
 
         test_cases()
 
         return function
     
     return parametrized_decorator
 
-def parametrized_wrap(inputs: list[Any] | tuple[Any], outputs: list[Any] | tuple[Any]):
-    return parametrized(expected_io=[([arg], ans) for arg, ans in zip(inputs, outputs)])
+def parametrized_wrap(
+    inputs: list[Any] | tuple[Any], outputs: list[Any] | tuple[Any],
+    function = lambda arg, ans: ([arg], ans)
+) -> Callable[[Callable], Callable]:
+    return parametrized(expected_io=[function(arg, ans) for arg, ans in zip(inputs, outputs)])
+
+# --- #
+
+def parametrized_kwrap(
+    inputs: list[Any] | tuple[Any] = None, 
+    kw_inputs: list[dict[str, Any]] = None, 
+    outputs: list[Any] | tuple[Any] = None,
+    
+    function = None
+) -> Callable[[Callable], Callable]:
+    
+    if inputs and kw_inputs:
+        if function == None: function = lambda arg, ans, **kwargs: ([arg], kwargs, ans)
+        assert len(inputs) == len(kw_inputs) == len(outputs)
+        return parametrized(expected_io=[function(arg, ans, **kwargs) for arg, ans, kwargs in zip(inputs, outputs, kw_inputs)])
+    
+    elif inputs and not kw_inputs:
+        if function == None: function = lambda arg, ans: ([arg], ans)
+        assert len(inputs) == len(outputs)
+        return parametrized(expected_io=[function(arg, ans) for arg, ans in zip(inputs, outputs)])
+    
+    elif not inputs and kw_inputs:
+        if function == None: function = lambda ans, **kwargs: ([], kwargs, ans)
+        assert len(kw_inputs) == len(outputs)
+        return parametrized(expected_io=[function(ans, **kwargs) for ans, kwargs in zip(outputs, kw_inputs)])
+    
+    else:
+        ...
```

### Comparing `efrem_utils-0.2.2/LICENSE` & `efrem_utils-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.2.2/README.md` & `efrem_utils-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.2.2/PKG-INFO` & `efrem_utils-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.2.2
+Version: 0.2.5
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

