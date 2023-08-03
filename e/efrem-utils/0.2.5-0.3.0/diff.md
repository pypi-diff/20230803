# Comparing `tmp/efrem_utils-0.2.5.tar.gz` & `tmp/efrem_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.2.5.tar", max compression
+gzip compressed data, was "efrem_utils-0.3.0.tar", max compression
```

## Comparing `efrem_utils-0.2.5.tar` & `efrem_utils-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    12856 2023-08-02 18:33:59.735966 efrem_utils-0.2.5/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.2.5/LICENSE
--rw-r--r--   0        0        0      361 2023-08-02 18:34:14.279734 efrem_utils-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.2.5/README.md
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    19006 2023-08-03 16:16:17.173939 efrem_utils-0.3.0/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0      361 2023-08-03 16:16:18.327714 efrem_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.3.0/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.3.0/PKG-INFO
```

### Comparing `efrem_utils-0.2.5/efrem_utils.py` & `efrem_utils-0.3.0/efrem_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 from enum import Enum
-from typing import Callable, TypeVar, Iterable, Optional, Any
-
+from typing import Callable, TypeVar, Iterable, Optional, Any, ParamSpec, Self
 T = TypeVar("T")
 W = TypeVar("W")
-
 def validated_input(
     msg: str | None = None,
     validators: Iterable[tuple[Callable[[T], bool], str | Callable[[T], str] | None]] | None = None,
     constructor: Callable[[T], W] = str,
     precomp: Callable[[str], T] | None = None,
     precomp_error: str | Callable[[str], str] | None = None
 ) -> Callable[[], W]:
@@ -21,113 +19,73 @@
 
     If an error is raised during the process of validation, it will count as a fail of validation, so 
     you can use this to make easy typechecks by using something like:
     `lambda buffer: float(buffer) or True` as a validator function.
 
     The precomp(utation) function will be applied to the input before validation `and` when it will be passed to a constructor. [ It applies to the value of input() ]
     """
-
-    if msg is None:
-        msg = f"Enter a {constructor}: "
-
-    if validators is None:
-        validators = [
-            (lambda buffer: constructor(buffer) or True, lambda buffer: f"<{buffer}> is not a valid {constructor}")
-        ]
-    
-    if precomp_error is None:
-        precomp_error = "Precomputation failed at input == <{buffer}> :("
-        
+    if msg is None: msg = f"Enter a {constructor}: "
+    if validators is None: validators = [(lambda buffer: constructor(buffer) or True, lambda buffer: f"<{buffer}> is not a valid {constructor}")]
+    if precomp_error is None: precomp_error = "Precomputation failed at input == <{buffer}> :("
     def inner() -> W:
         while True:
-
             buffer: str = input(msg)
-
             if precomp is not None:
-                try:
-                    buffer: T = precomp(buffer)
+                try: buffer: T = precomp(buffer)
                 except:
                     print(precomp_error(buffer) if callable(precomp_error) else precomp_error.format(buffer=buffer))
                     continue
-
             for validator, err_msg in validators:
                 result: bool
-                try:
-                    result = validator(buffer)
-                except:
-                    result = False
-
+                try: result = validator(buffer)
+                except: result = False
                 if not result:
-                    if err_msg is not None:
-                        print(err_msg(buffer) if callable(err_msg) else err_msg.format(buffer=buffer))
+                    if err_msg is not None: print(err_msg(buffer) if callable(err_msg) else err_msg.format(buffer=buffer))
                     break
-
             else: # if no break happens in validation checking - return
-                return constructor(buffer)
-                
+                return constructor(buffer) 
     return inner
-
 # --- # 
-
 class Case:
     class _Mode(Enum):
         match = 0 # pass same args, see if output matches
         validate = 1 # pass same args to both, see if kwargs.get("validator") passes
-
     def __init__(self, function = (lambda *args, **kwargs: ((args), kwargs) if kwargs else args), *_, **kwargs):
         if len(kwargs) == 0: self.mode = Case._Mode.match
         elif len(kwargs) == 1 and ("validator" in kwargs): self.mode = Case._Mode.validate; self.validator = kwargs["validator"]
         else: raise ValueError("Currently a not supported case")
         self.function = function
-
-    def __repr__(self) -> str:
-        return f"Case(function = {self.function.__name__}, mode = {self.mode})"
-
+    def __repr__(self) -> str: return f"Case(function = {self.function.__name__}, mode = {self.mode})"
 def parametrized(
     expected_io: list[
         (tuple[tuple[Any, ...] | list[Any], Any | Case | Exception]) | 
         (tuple[tuple[Any, ...] | list[Any], dict[str, Any], Any | Case | Exception]) |
         (list[tuple[Any, ...] | list[Any], Any | Case | Exception]) | 
         (list[tuple[Any, ...] | list[Any], dict[str, Any], Any | Case | Exception])
     # problem? :trollface: :union_type: :trollge:
 ]) -> Callable[[Callable], Callable]: # returns a decorator
-
-    #
-    # [
-    #   (*args: tuple | list, **kwargs: Optional[dict[str, Any]], expect: Any | Case | Exception),
-    #   ...
-    # ]
-    #
-
     class _TestMode(Enum):
         normal_case: int = 0
         case_test: int = 1
         exception_test: int = 2
-
         @classmethod
         def from_expect(cls: _TestMode, expect: Any | Case | Exception) -> _TestMode:
             # Exception test:
             try:
                 if isinstance(expect(), Exception): return cls.exception_test
             except:
                 if isinstance(expect, Exception): return cls.exception_test
-
             if isinstance(expect, Case): return cls.case_test
-
             else: return cls.normal_case
 
 
     def parametrized_decorator(function):
-
         def parse_case(*, args: Optional[tuple[Any, ...] | list[Any]] = (), kwargs: Optional[dict[str, Any]] = {}, expect: Any | Case | Exception) -> None:
-
             test_mode: _TestMode = _TestMode.from_expect(expect=expect)
-
             info: str = f"{function.__name__}({repr(args)*bool(args)}{(', '*(bool(args) and bool(kwargs)))+repr(kwargs)*bool(kwargs)})"
-
             match test_mode:
                 case _TestMode.normal_case:
                     # in a normal case, we just call the function with the provided arguments, and check if the result matches expectations
                     try:
                         result = function(*args, **kwargs) if kwargs else function(*args)
                         callable_expect = callable(expect)
                         expectation_passed = expect(result) if callable_expect else expect == result
@@ -207,55 +165,113 @@
                     except Exception as exc:
                         if type(exc) == expect:
                             print(f"\x1B[38;5;50mException test passed: {info} -> {repr(exc)}\x1B[0m")
                         else:
                             print(f"\x1B[38;5;196mException test failed: {info} -> {repr(exc)} instead of {repr(expect())}\x1B[0m")
 
         def test_cases() -> None:
-            
             for test_case in expected_io:
                 if len(test_case) == 2:
-                    if isinstance(test_case[0], dict):
-                        parse_case(kwargs=test_case[0], expect=test_case[1])
-                    else:
-                        parse_case(args=test_case[0], expect=test_case[1])
+                    if isinstance(test_case[0], dict): parse_case(kwargs=test_case[0], expect=test_case[1])
+                    else: parse_case(args=test_case[0], expect=test_case[1])
                 elif len(test_case) == 3: parse_case(args=test_case[0], kwargs=test_case[1], expect=test_case[2])
-
         test_cases()
-
         return function
-    
     return parametrized_decorator
-
 def parametrized_wrap(
     inputs: list[Any] | tuple[Any], outputs: list[Any] | tuple[Any],
     function = lambda arg, ans: ([arg], ans)
 ) -> Callable[[Callable], Callable]:
     return parametrized(expected_io=[function(arg, ans) for arg, ans in zip(inputs, outputs)])
-
 # --- #
-
 def parametrized_kwrap(
     inputs: list[Any] | tuple[Any] = None, 
     kw_inputs: list[dict[str, Any]] = None, 
     outputs: list[Any] | tuple[Any] = None,
-    
     function = None
 ) -> Callable[[Callable], Callable]:
-    
     if inputs and kw_inputs:
         if function == None: function = lambda arg, ans, **kwargs: ([arg], kwargs, ans)
         assert len(inputs) == len(kw_inputs) == len(outputs)
         return parametrized(expected_io=[function(arg, ans, **kwargs) for arg, ans, kwargs in zip(inputs, outputs, kw_inputs)])
-    
     elif inputs and not kw_inputs:
         if function == None: function = lambda arg, ans: ([arg], ans)
         assert len(inputs) == len(outputs)
         return parametrized(expected_io=[function(arg, ans) for arg, ans in zip(inputs, outputs)])
-    
     elif not inputs and kw_inputs:
         if function == None: function = lambda ans, **kwargs: ([], kwargs, ans)
         assert len(kw_inputs) == len(outputs)
         return parametrized(expected_io=[function(ans, **kwargs) for ans, kwargs in zip(outputs, kw_inputs)])
-    
-    else:
-        ...
+    else: ...
+# --- #
+ClsVar = TypeVar("ClsVar")
+Param = ParamSpec("Param")
+RetType = TypeVar("RetType")
+class ANSI: reset = "\x1B[0m";passed_0 = "\x1B[38;5;46m";failed_0 = "\x1B[38;5;196m";unexpected_exception_0 = "\x1B[38;5;129m";unexpected_return_0 = "\x1B[38;5;160m"
+class Args:
+    instances: list[Self] = []
+    @classmethod
+    def pop(cls: ClsVar, /, true_pop: bool = False) -> ClsVar:
+        if true_pop: return cls.instances.pop()
+        else: return cls.instances[-1]
+    def __init__(self: Self, /, *args: tuple[Any, ...], **kwargs: dict[str, Any]) -> None: self.args = args; self.kwargs = kwargs; Args.instances.append(self)
+    def __getitem__(self: Self, /, key: slice | Any) -> list | tuple:
+        if isinstance(key, slice): return [self, key.step if key.step else (key.stop if key.stop else (key.start))]
+        else: return self, key
+    def __call__(self: Self, /, function: Callable[Param, RetType]) -> RetType: return function(*self.args, **self.kwargs)
+    def call_string(self: Self, /, function: Callable[Param, RetType]) -> str: return f"{function.__name__}({f'*args = {repr(self.args)}'*bool(self.args)}{(', '*(bool(self.args) and bool(self.kwargs)))+f'**kwargs = {repr(self.kwargs)}'*bool(self.kwargs)})"
+    def __repr__(self: Self) -> str: return f"Args(*args = {repr(self.args)} ; **kwargs = {repr(self.kwargs)})"
+class Case:
+    @classmethod
+    def condition_test(cls: ClsVar, /, args: Args, condition: Callable[Param, bool], name: str = "Meta test") -> ClsVar:
+        def get_response(self: Self, /, function: Callable[Param, RetType]) -> str:
+            call_string = self.args.call_string(function=function)
+            try:
+                result: RetType = args(function=function); condition_string = f"{condition.__name__}({repr(result)})"
+                if condition(result): return f"{ANSI.passed_0}{name} passed: {call_string} -> {repr(result)}, and {condition_string} is truthy{ANSI.reset}" # test pass
+                else: return f"{ANSI.failed_0}{name} failed: {call_string} -> {repr(result)}, and {condition_string} is falsy{ANSI.reset}" # test fail
+            except Exception as exc: return f"{ANSI.unexpected_exception_0}Unexpected exception raised: {call_string} -> {repr(exc)}{ANSI.reset}" # test raised unexpected exception
+        return cls(args=args, get_response=get_response)
+    @classmethod
+    def equal(cls: ClsVar, /, args: Args, expected_result: Any) -> ClsVar:
+        def get_response(self: Self, /, function: Callable[Param, RetType]) -> str:
+            call_string = self.args.call_string(function=function)
+            try:
+                result: RetType = args(function=function)
+                if result == expected_result: return f"{ANSI.passed_0}Equal test passed: {call_string} -> {repr(result)} == {repr(expected_result)}{ANSI.reset}" # test pass
+                else: return f"{ANSI.failed_0}Equal test failed: {call_string} -> {repr(result)} instead of {repr(expected_result)}{ANSI.reset}" # test fail
+            except Exception as exc: return f"{ANSI.unexpected_exception_0}Equal test raised an unexpected exception: {call_string} -> {repr(exc)} instead of {repr(expected_result)}{ANSI.reset}" # test raised unexpected exception
+        return cls(args=args, get_response=get_response)
+    @classmethod
+    def expect(cls: ClsVar, /, args: Args, exception: Exception) -> ClsVar:
+        def get_response(self: Self, /, function: Callable[Param, RetType]) -> str:
+            call_string = self.args.call_string(function)
+            try:
+                result: RetType = self.args(function=function); return f"{ANSI.unexpected_return_0}Exception test didnt raise an exception: {call_string} -> {repr(result)} instead of {repr(exception())}{ANSI.reset}"
+            except Exception as exc:
+                if type(exc) == exception: return f"{ANSI.passed_0}Exception test passed: {call_string} -> {repr(exception())}{ANSI.reset}"
+                else: return f"{ANSI.failed_0}Exception test failed: {call_string} -> {repr(exc)} instead of {repr(exception())}{ANSI.reset}"
+        return cls(args=args, get_response=get_response)
+    def __init__(self: Self, /, args: Args, get_response: Callable[[Self, Callable[Param, RetType]], str]) -> None: self.args = args; self.get_response = get_response
+    @classmethod
+    def copycat(cls: ClsVar, /, args: Args, copycat_function: Callable[Param, RetType]) -> ClsVar:
+        def get_response(self: Self, /, function: Callable[Param, RetType]) -> str:
+            call_string_0: str = self.args.call_string(function); call_string_1: str = self.args.call_string(copycat_function); res_0: Any | None = None; res_1: Any | None = None; exc_0: Exception | None = None; exc_1: Exception | None = None
+            try: res_0 = args(function)
+            except Exception as buf_exc_0: exc_0 = buf_exc_0
+            try: res_1 = args(copycat_function)
+            except Exception as buf_exc_1: exc_1 = buf_exc_1
+            if exc_0 or exc_1:
+                if exc_0 and exc_1: return f"{ANSI.unexpected_exception_0}Copycat test raised an unexpected exception: {call_string_0} -> {repr(exc_0)} || {call_string_1} -> {repr(exc_1)}{ANSI.reset}"
+                elif exc_0 and not exc_1: return f"{ANSI.unexpected_exception_0}Copycat test raised an unexpected exception: {call_string_0} -> {repr(exc_0)} || {call_string_1} -> {repr(res_1)}{ANSI.reset}"
+                elif not exc_0 and exc_1: return f"{ANSI.unexpected_exception_0}Copycat test raised an unexpected exception: {call_string_0} -> {repr(res_0)} || {call_string_1} -> {repr(exc_1)}{ANSI.reset}"
+            else:
+                if res_0 == res_1: return f"{ANSI.passed_0}Copycat test passed: {call_string_0} -> {repr(res_0)} == {call_string_1} (which is {repr(res_1)}){ANSI.reset}"
+                else: return f"{ANSI.failed_0}Copycat test failed: {call_string_0} -> {repr(res_0)} buf {call_string_1} -> {repr(res_1)}{ANSI.reset}"
+        return cls(args=args, get_response=get_response) 
+    def __call__(self: Self, /, function: Callable[Param, RetType]) -> str: return self.get_response(function)
+    def __repr__(self: Self) -> str: return f"Case({self.args}, {self.get_response.__name__})"
+def test(cases: Iterable[Case]) -> Callable[[Callable[Param, RetType]], Callable[Param, RetType]]: # returns a decorator [parametrized decorator implementation]
+    def test_decorator(function: Callable[Param, RetType]) -> Callable[Param, RetType]:
+        for case in cases: print(case.get_response(case, function=function))
+        return function
+    return test_decorator
```

### Comparing `efrem_utils-0.2.5/LICENSE` & `efrem_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.2.5/README.md` & `efrem_utils-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.2.5/PKG-INFO` & `efrem_utils-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.2.5
+Version: 0.3.0
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

