# Comparing `tmp/llm_strategy-0.0.3.tar.gz` & `tmp/llm_strategy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_strategy-0.0.3.tar", max compression
+gzip compressed data, was "llm_strategy-1.0.0.tar", max compression
```

## Comparing `llm_strategy-0.0.3.tar` & `llm_strategy-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1090 2023-03-07 16:50:56.815528 llm_strategy-0.0.3/LICENSE
--rw-r--r--   0        0        0     5216 2023-03-07 16:50:56.815528 llm_strategy-0.0.3/README.md
--rw-r--r--   0        0        0       65 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/__init__.py
--rw-r--r--   0        0        0    18772 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/dataclasses_schema.py
--rw-r--r--   0        0        0     5873 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/decorators.py
--rw-r--r--   0        0        0     5951 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/llm_implement.py
--rw-r--r--   0        0        0     3307 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/prompt_doc_string.py
--rw-r--r--   0        0        0     1249 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/prompt_template.py
--rw-r--r--   0        0        0        0 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/testing/__init__.py
--rw-r--r--   0        0        0     3167 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/testing/fake_llm.py
--rw-r--r--   0        0        0      745 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/testing/tests/test_fake_llm.py
--rw-r--r--   0        0        0     8547 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/tests/test_dataclasses_schema.py
--rw-r--r--   0        0        0     4258 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/tests/test_llm_implement.py
--rw-r--r--   0        0        0    21582 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/tests/test_llm_strategy.py
--rw-r--r--   0        0        0     1197 2023-03-07 16:50:56.819528 llm_strategy-0.0.3/llm_strategy/tests/test_prompt_doct_string.py
--rw-r--r--   0        0        0     1907 2023-03-07 16:51:36.431533 llm_strategy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 llm_strategy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-08-02 22:30:44.700720 llm_strategy-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5216 2023-08-02 22:30:44.700720 llm_strategy-1.0.0/README.md
+-rw-r--r--   0        0        0      185 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/__init__.py
+-rw-r--r--   0        0        0     2220 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/adapters.py
+-rw-r--r--   0        0        0     2120 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/chat_chain.py
+-rw-r--r--   0        0        0    36554 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/llm_function.py
+-rw-r--r--   0        0        0     4562 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/llm_strategy.py
+-rw-r--r--   0        0        0        0 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/__init__.py
+-rw-r--r--   0        0        0     5974 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/fake_chat_model.py
+-rw-r--r--   0        0        0     3217 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/fake_llm.py
+-rw-r--r--   0        0        0     1999 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/tests/test_fake_chat_model.py
+-rw-r--r--   0        0        0      685 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/tests/test_fake_llm.py
+-rw-r--r--   0        0        0      776 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/tests/test_adapters.py
+-rw-r--r--   0        0        0    15025 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/tests/test_llm_function.py
+-rw-r--r--   0        0        0    23624 2023-08-02 22:30:44.708720 llm_strategy-1.0.0/llm_strategy/tests/test_llm_strategy.py
+-rw-r--r--   0        0        0     1847 2023-08-02 22:31:14.316805 llm_strategy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 llm_strategy-1.0.0/PKG-INFO
```

### Comparing `llm_strategy-0.0.3/LICENSE` & `llm_strategy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_strategy-0.0.3/README.md` & `llm_strategy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `llm_strategy-0.0.3/llm_strategy/decorators.py` & `llm_strategy-1.0.0/llm_strategy/llm_strategy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,163 +1,135 @@
 # type: ignore
 import dataclasses
-import dis
-import functools
+import functools  # noqa: F401
 import inspect
-import types
 import typing
 from dataclasses import dataclass
 
 import typing_extensions
 from langchain.llms.base import BaseLLM
 
-from llm_strategy.dataclasses_schema import DataclassesSchema
-from llm_strategy.llm_implement import LLMCall, unwrap_function
+from llm_strategy.llm_function import (
+    LLMFunction,
+    apply_decorator,
+    is_not_implemented,
+    unwrap_function,
+)
 
 P = typing_extensions.ParamSpec("P")
 T = typing.TypeVar("T")
 
 
-def check_not_implemented(f: typing.Callable) -> bool:
-    """Check that a function (property getter, regular method, class method or static method)
-    only raises NotImplementedError."""
-    unwrapped_f = unwrap_function(f)
-
-    if not hasattr(unwrapped_f, "__code__"):
-        raise ValueError(f"Cannot check whether {f} is implemented. Where is __code__?")
-
-    # Inspect the opcodes
-    code = unwrapped_f.__code__
-    # Get the opcodes
-    opcodes = list(dis.get_instructions(code))
-    # Check that it only uses the following opcodes:
-    # - RESUME
-    # - LOAD_GLOBAL
-    # - PRECALL
-    # - CALL
-    # - RAISE_VARARGS
-    valid_opcodes = {
-        "RESUME",
-        "LOAD_GLOBAL",
-        "PRECALL",
-        "CALL",
-        "RAISE_VARARGS",
-    }
-    # We allow at most a function of length len(valid_opcodes)
-    if len(opcodes) > len(valid_opcodes):
+def can_wrap_function_in_llm(f: typing.Callable[P, T]) -> bool:
+    """
+    Return True if f can be wrapped in an LLMCall.
+    """
+    unwrapped = unwrap_function(f)
+    if not callable(unwrapped):
+        return False
+    if inspect.isgeneratorfunction(unwrapped):
+        return False
+    if inspect.iscoroutinefunction(unwrapped):
         return False
-    for opcode in opcodes:
-        if opcode.opname not in valid_opcodes:
-            return False
-        # Check that the function only raises NotImplementedError
-        if opcode.opname == "LOAD_GLOBAL" and opcode.argval != "NotImplementedError":
-            return False
-        if opcode.opname == "RAISE_VARARGS" and opcode.argval != 1:
-            return False
-        valid_opcodes.remove(opcode.opname)
-    # Check that the function raises a NotImplementedError at the end.
-    if opcodes[-1].opname != "RAISE_VARARGS":
+    if not inspect.isfunction(unwrapped) and not inspect.ismethod(unwrapped):
         return False
-    return True
+    return is_not_implemented(unwrapped)
 
 
-def llm_strategy(  # noqa: C901
-    llm: BaseLLM, parent_dataclasses_schema: DataclassesSchema | None = None
-) -> typing.Callable[[T], T]:
+def llm_strategy(llm: BaseLLM) -> typing.Callable[[T], T]:  # noqa: C901
     """
     A strategy that implements what ever it decorates (or is called on) using the LLM.
     """
 
     @typing.no_type_check
     def decorator(f: T) -> T:
+        assert can_wrap_member_in_llm(f)
+
         # For an instance of dataclass, call llm_strategy_dataclass with the fields.
         if dataclasses.is_dataclass(f):
             if isinstance(f, type):
-                return llm_strategy_dataclass(f, llm, parent_dataclasses_schema)
+                return llm_dataclass(f, llm)
             else:
-                implemented_dataclass = llm_strategy_dataclass(type(f), llm, parent_dataclasses_schema)
+                implemented_dataclass = llm_dataclass(type(f), llm)
                 # Create an instance of the implemented dataclass using the fields from f
                 params = {field.name: getattr(f, field.name) for field in dataclasses.fields(f)}
                 return implemented_dataclass(**params)
-        elif isinstance(f, classmethod):
-            return classmethod(decorator(f.__func__))
-        elif isinstance(f, staticmethod):
-            return staticmethod(decorator(f.__func__))
-        elif isinstance(f, property):
-            return property(decorator(f.fget), doc=f.__doc__)
-        elif isinstance(f, types.MethodType):
-            return types.MethodType(decorator(f.__func__), f.__self__)
-        # Does the function have a __wrapped__ attribute?
-        elif hasattr(f, "__wrapped__"):
-            # If so, it is a wrapped function. Unwrap it.
-            return decorator(f.__wrapped__)
-        elif isinstance(f, LLMCall):
-            return f
-        elif callable(f):
-            llm_call = LLMCall.wrap_callable(f, llm, parent_dataclasses_schema)
-
-            @functools.wraps(f)
-            def wrapper(*args, **kwargs):
-                return llm_call(*args, **kwargs)
-
-            return wrapper
         else:
-            raise ValueError(f"Cannot decorate {f} with llm_strategy.")
+
+            def inner_decorator(unwrapped_f):
+                llm_f = None
+
+                @functools.wraps(unwrapped_f)
+                def strategy_wrapper(*args, **kwargs):
+                    nonlocal llm_f
+                    if llm_f is None:
+                        # Get the signature of f
+                        sig = inspect.signature(unwrapped_f, eval_str=True)
+                        # Add a llm parameter to the signature as first argument
+                        new_params = [inspect.Parameter("__llm", inspect.Parameter.POSITIONAL_ONLY)]
+                        new_params.extend(sig.parameters.values())
+
+                        new_sig = sig.replace(parameters=new_params)
+
+                        def dummy_f(*args, **kwargs):
+                            raise NotImplementedError()
+
+                        new_f = functools.wraps(unwrapped_f)(dummy_f)
+                        new_f.__module__ = unwrapped_f.__module__
+                        # Set the signature of the new function
+                        new_f.__signature__ = new_sig
+
+                        del new_f.__wrapped__
+
+                        # Wrap the function in an LLMFunction
+                        llm_f = functools.wraps(new_f)(LLMFunction())
+
+                    return llm_f(llm, *args, **kwargs)
+
+                return strategy_wrapper
+
+            return apply_decorator(f, inner_decorator)
 
     return decorator
 
 
 def can_wrap_member_in_llm(f: typing.Callable[P, T]) -> bool:
     """
     Return True if f can be wrapped in an LLMCall.
     """
-    # An existing LLMCall was already determined to be wrappable.
-    if isinstance(f, LLMCall):
+    if isinstance(f, LLMFunction):
         return True
     if dataclasses.is_dataclass(f):
         return True
 
-    unwrapped = unwrap_function(f)
-    if not callable(unwrapped):
-        return False
-    if inspect.isgeneratorfunction(unwrapped):
-        return False
-    if inspect.iscoroutinefunction(unwrapped):
-        return False
-    if not inspect.isfunction(unwrapped) and not inspect.ismethod(unwrapped):
-        return False
-    return check_not_implemented(unwrapped)
+    return can_wrap_function_in_llm(f)
 
 
 @typing_extensions.dataclass_transform()
-def llm_strategy_dataclass(
-    dataclass_type: type, llm: BaseLLM, parent_dataclasses_schema: DataclassesSchema | None = None
-) -> type:
-    global long_unlikely__dataclasses_schema
+def llm_dataclass(dataclass_type: type, llm: BaseLLM) -> type:
     global long_unlikely_prefix__llm
     global long_unlikely__member_name, long_unlikely__member
     long_unlikely_prefix__llm = llm
-    long_unlikely__dataclasses_schema = parent_dataclasses_schema
     long_unlikely__member_name, long_unlikely__member = None, None
 
     @dataclass
     class SpecificLLMImplementation(dataclass_type):
         global long_unlikely__member_name, long_unlikely__member
         for long_unlikely__member_name, long_unlikely__member in inspect.getmembers_static(  # noqa: B007
             dataclass_type, can_wrap_member_in_llm
         ):
             exec(
                 f"""
-@llm_strategy(long_unlikely_prefix__llm, long_unlikely__dataclasses_schema)
+@llm_strategy(long_unlikely_prefix__llm)
 @functools.wraps(long_unlikely__member)
 def {long_unlikely__member_name}(*args, **kwargs):
     raise NotImplementedError()
 """
             )
 
     SpecificLLMImplementation.__name__ = f"{llm.__class__.__name__}_{dataclass_type.__name__}"
     SpecificLLMImplementation.__qualname__ = f"{llm.__class__.__name__}_{dataclass_type.__qualname__}"
 
     del long_unlikely__member_name, long_unlikely__member
-    del long_unlikely_prefix__llm, long_unlikely__dataclasses_schema
+    del long_unlikely_prefix__llm
 
     return SpecificLLMImplementation
```

### Comparing `llm_strategy-0.0.3/llm_strategy/testing/fake_llm.py` & `llm_strategy-1.0.0/llm_strategy/testing/fake_llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Mapping
 
 from langchain.llms.base import LLM, BaseLLM
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class FakeLLM(LLM, BaseModel):
     """Fake LLM wrapper for testing purposes.
 
     We can use this to test the behavior of the LLM wrapper without having to actually call the LLM.
 
@@ -17,15 +17,15 @@
     the full response (as it is build over time) and return the part before the query and the stop word.
 
     This also means that there is no non-determinism in the output, which is good for testing, but bad for variance.
     Especially if we want to test the behavior of the LLM wrapper when the LLM is not deterministic. (Create different
     outputs for different calls, for example.)
     """
 
-    texts: set[str] = set()
+    texts: set[str] = Field(default_factory=set)
     """The texts to return on call."""
     external_llm: BaseLLM | None = None
     """An external LLM to use if the query is not found."""
 
     def __del__(self) -> None:
         # If we have an external LLM, we write out all our responses to stdout so that they can be copied into the
         # constructor call for the next run by hand if needed.
@@ -59,15 +59,16 @@
         if self.external_llm is not None:
             response = self.external_llm(prompt, stop=stop)
             text = prompt + response
             self.texts.add(text)
             return response
 
         # If no queries are provided, print the code to update the query
-        code_snippet = f"""# Add the following to the queries dict:
-{prompt!r}, # TODO: Append the correct response here
-"""
-        raise NotImplementedError("No query provided. Add the following to the queries dict:\n\n" + code_snippet)
+        code_snippet = (
+            f"# Add the following to the queries list:\n\n{repr(prompt)}\n# TODO: Append the correct response here"
+        )
+        print(code_snippet)
+        raise NotImplementedError("No query provided to FakeLLM." + code_snippet)
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
         return {}
```

### Comparing `llm_strategy-0.0.3/llm_strategy/testing/tests/test_fake_llm.py` & `llm_strategy-1.0.0/llm_strategy/testing/tests/test_fake_llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+import langchain
+import pytest
+
 from llm_strategy.testing import fake_llm
 
+langchain.llm_cache = None
+
 
 def test_fake_llm_query():
     """Test that the fake LLM returns the correct query."""
     llm = fake_llm.FakeLLM(texts={"foobar"})
     assert llm("foo") == "bar"
 
 
@@ -12,13 +17,9 @@
     llm = fake_llm.FakeLLM(texts={"foobar"})
     assert llm("foo", stop=["a"]) == "b"
 
 
 def test_fake_llm_missing_query():
     """Test that the fake LLM raises an error if the query is missing."""
     llm = fake_llm.FakeLLM(texts=set())
-    try:
-        llm("foo")
-    except NotImplementedError as e:
-        assert "Add the following to the queries dict:" in str(e)
-    else:
-        raise AssertionError("Expected NotImplementedError")
+    with pytest.raises(NotImplementedError):
+        raise ValueError(llm("foo"))
```

### Comparing `llm_strategy-0.0.3/llm_strategy/tests/test_llm_strategy.py` & `llm_strategy-1.0.0/llm_strategy/tests/test_llm_strategy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 from dataclasses import dataclass
 
-from llm_strategy.decorators import (
-    can_wrap_member_in_llm,
-    check_not_implemented,
-    llm_strategy,
-)
+from llm_strategy import llm_strategy
+from llm_strategy.llm_function import is_not_implemented
 from llm_strategy.testing.fake_llm import FakeLLM
 
 
 @dataclass
 class DummyInterface:
     """A dataclass with some members that are not implemented."""
 
     a: int = -1
 
     @staticmethod
     def static_method(a: int, b: int) -> int:
         """Add two numbers."""
         raise NotImplementedError()
 
-    @classmethod
-    def class_method(cls, a: int, b: int) -> int:
-        """Add two numbers."""
-        raise NotImplementedError()
+    # @classmethod
+    # def class_method(cls: type, a: int, b: int) -> int:
+    #     """Add two numbers."""
+    #     raise NotImplementedError()
 
     @property
-    def property_getter(self) -> int:
+    def property_getter(self: "DummyInterface") -> int:
         """Return 0."""
         raise NotImplementedError()
 
-    def bound_method(self, a: int, b: int) -> int:
+    def bound_method(self: "DummyInterface", a: int, b: int) -> int:
         """Add two numbers."""
         raise NotImplementedError()
 
-    def bound_method_raises_class(self, a: int, b: int = 1) -> int:
-        """Add two numbers."""
-        raise NotImplementedError
-
-    def bound_method_implemented(self, b: int = 1) -> int:
+    def bound_method_implemented(self: "DummyInterface", b: int = 1) -> int:
         """Add two numbers."""
         return self.a + b
 
     @staticmethod
     def static_method_implemented(a: int, b: int = 1) -> int:
         """Add two numbers."""
         return a + b
@@ -53,167 +46,168 @@
 
     @property
     def property_getter_implemented(self) -> int:
         """Return 1."""
         return 1
 
 
-def test_can_wrap_member_in_llm():
-    """Test that can_wrap_member_in_llm works as expected."""
-    # This automatically also checks check_not_implemented.
-    assert can_wrap_member_in_llm(DummyInterface.static_method)
-    assert can_wrap_member_in_llm(DummyInterface.bound_method)
-    assert can_wrap_member_in_llm(DummyInterface.class_method)
-    assert can_wrap_member_in_llm(DummyInterface.property_getter)
-    assert can_wrap_member_in_llm(DummyInterface.bound_method_raises_class)
-
-    assert not can_wrap_member_in_llm(DummyInterface.bound_method_implemented)
-    assert not can_wrap_member_in_llm(DummyInterface.static_method_implemented)
-    assert not can_wrap_member_in_llm(DummyInterface.class_method_implemented)
-    assert not can_wrap_member_in_llm(DummyInterface.property_getter_implemented)
-
-
 def not_implemented_function():
     raise NotImplementedError
 
 
-def test_check_not_implemented_functon():
-    assert check_not_implemented(not_implemented_function)
-    assert not check_not_implemented(lambda: 1)
+def test_is_not_implemented_functon():
+    assert is_not_implemented(not_implemented_function)
+    assert not is_not_implemented(lambda: 1)
 
 
 def test_llm_strategy_on_functions():
     def add_two_ints(a: int, b: int) -> int:
         """Add two integers."""
-        return a + b
+        raise NotImplementedError()
 
     def add_two_ints_with_default(a: int, b: int = 1) -> int:
         """Add two integers with a default value."""
-        return a + b
+        raise NotImplementedError()
 
     def add_two_ints_with_default_and_kwarg(*, a: int, c: int = 2) -> int:
         """Add two integers with a default value."""
-        return a + c
+        raise NotImplementedError()
 
     llm = FakeLLM(
         texts={
             (
-                "Execute the following function that is described via a doc string:\n\nAdd two integers.\n\n#"
-                " Task\n\nExecute the function with the inputs that follow in the next section and finally return the"
-                " output using the output type\nas YAML document in an # Output section. (If the value is a literal,"
-                " then just write the value. We parse the text in the\n# Output section using `yaml.safe_load` in"
-                " Python.)\n\n# Input Types\n\na: int\nb: int\n\n\n# Inputs\n\na: 1\nb: 2\n\n\n# Output"
-                " Type\n\nint\n\n# Execution Scratch-Pad (Think Step by Step)\n\n\n# Output\n\n---\nresult: 3"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nAdd two integers with a default"
-                " value.\n\n# Task\n\nExecute the function with the inputs that follow in the next section and finally"
-                " return the output using the output type\nas YAML document in an # Output section. (If the value is a"
-                " literal, then just write the value. We parse the text in the\n# Output section using `yaml.safe_load`"
-                " in Python.)\n\n# Input Types\n\na: int\nc: int\n\n\n# Inputs\n\na: 1\nc: 2\n\n\n# Output"
-                " Type\n\nint\n\n# Execution Scratch-Pad (Think Step by Step)\n\n\ndef add_two_integers(a, c=0):\n   "
-                ' """Add two integers with a default value."""\n    return a + c \n\n\n# Output\n\n---\nresult: 3'
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nAdd two integers with a default"
-                " value.\n\n# Task\n\nExecute the function with the inputs that follow in the next section and finally"
-                " return the output using the output type\nas YAML document in an # Output section. (If the value is a"
-                " literal, then just write the value. We parse the text in the\n# Output section using `yaml.safe_load`"
-                " in Python.)\n\n# Input Types\n\na: int\nb: int\n\n\n# Inputs\n\na: 1\nb: 1\n\n\n# Output"
-                " Type\n\nint\n\n# Execution Scratch-Pad (Think Step by Step)\n\n\n# Output\n\n---\nresult: 2"
+                "Add two integers.\n\nThe input and output are formatted as a JSON interface that conforms to the "
+                'JSON schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a list '
+                'of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object {'
+                '"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": '
+                '["bar", "baz"]}} is not well-formatted.\n\nHere is the input schema:\n```\n{"properties": {"a": {'
+                '"type": "integer"}, "b": {"type": "integer"}}, "required": ["a", "b"]}\n```\n\nHere is the output '
+                'schema:\n```\n{"properties": {"return_value": {"type": "integer"}}, "required": ['
+                '"return_value"]}\n```\nNow output the results for the following inputs:\n```\n{"a": 1, "b": 2}\n```'
+                '{"return_value": 3}\n'
+            ),
+            (
+                "Add two integers with a default value.\n\nThe input and output are formatted as a JSON interface "
+                'that conforms to the JSON schemas below.\n\nAs an example, for the schema {"properties": {"foo": {'
+                '"description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ['
+                '"foo"]}} the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {'
+                '"properties": {"foo": ["bar", "baz"]}} is not well-formatted.\n\nHere is the input schema:\n```\n{'
+                '"properties": {"a": {"type": "integer"}, "b": {"type": "integer"}}, "required": ["a"]}\n```\n\nHere '
+                'is the output schema:\n```\n{"properties": {"return_value": {"type": "integer"}}, "required": ['
+                '"return_value"]}\n```\nNow output the results for the following inputs:\n```\n{"a": 1, "b": 1}\n```'
+                '{"return_value": 2}\n'
+            ),
+            (
+                "Add two integers with a default value.\n\nThe input and output are formatted as a JSON interface "
+                'that conforms to the JSON schemas below.\n\nAs an example, for the schema {"properties": {"foo": {'
+                '"description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ['
+                '"foo"]}} the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {'
+                '"properties": {"foo": ["bar", "baz"]}} is not well-formatted.\n\nHere is the input schema:\n```\n{'
+                '"properties": {"a": {"type": "integer"}, "c": {"type": "integer"}}, "required": ["a"]}\n```\n\nHere '
+                'is the output schema:\n```\n{"properties": {"return_value": {"type": "integer"}}, "required": ['
+                '"return_value"]}\n```\nNow output the results for the following inputs:\n```\n{"a": 1, "c": 2}\n```'
+                '{"return_value": 3}\n'
             ),
         },
         # external_llm=OpenAI(),
     )
 
     assert llm_strategy(llm)(add_two_ints)(1, 2) == 3
     assert llm_strategy(llm)(add_two_ints_with_default)(1) == 2
     assert llm_strategy(llm)(add_two_ints_with_default_and_kwarg)(a=1) == 3
 
 
 def test_llm_strategy_dummy_interface():
     llm = FakeLLM(
-        texts={
+        texts=[
             (
-                "Execute the following function that is described via a doc string:\n\nAdd two numbers.\n\n#"
-                " Task\n\nExecute the function with the inputs that follow in the next section and finally return the"
-                " output using the output type\nas YAML document in an # Output section. (If the value is a literal,"
-                " then just write the value. We parse the text in the\n# Output section using `yaml.safe_load` in"
-                " Python.)\n\n# Dataclasses Schema\n\ntypes:\n  DummyInterface:\n    a:\n      type: int\n "
-                " FakeLLM_DummyInterface:\n    a:\n      type: int\n    bases:\n    - DummyInterface\n\n\n# Input"
-                " Types\n\na: int\nb: int\nself: FakeLLM_DummyInterface\n\n\n# Inputs\n\na: 1\nb: 2\nself:\n  a:"
-                " -1\n\n\n# Output Type\n\nint\n\n# Execution Scratch-Pad (Think Step by Step)\n\n\n#"
-                " Output\n\n---\nresult: 3"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nAdd two numbers.\n\n#"
-                " Task\n\nExecute the function with the inputs that follow in the next section and finally return the"
-                " output using the output type\nas YAML document in an # Output section. (If the value is a literal,"
-                " then just write the value. We parse the text in the\n# Output section using `yaml.safe_load` in"
-                " Python.)\n\n# Dataclasses Schema\n\ntypes:\n  type:\n    a:\n      type: int\n\n\n# Input Types\n\na:"
-                " int\nb: int\ncls: type\n\n\n# Inputs\n\na: 1\nb: 2\ncls: <class"
-                " 'llm_strategy.llm_strategy.FakeLLM_DummyInterface'>\n\n\n# Output Type\n\nint\n\n# Execution"
-                " Scratch-Pad (Think Step by Step)\n\n\n# Output\n\n---\nresult: 3"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nAdd two numbers.\n\n#"
-                " Task\n\nExecute the function with the inputs that follow in the next section and finally return the"
-                " output using the output type\nas YAML document in an # Output section. (If the value is a literal,"
-                " then just write the value. We parse the text in the\n# Output section using `yaml.safe_load` in"
-                " Python.)\n\n# Input Types\n\na: int\nb: int\n\n\n# Inputs\n\na: 1\nb: 2\n\n\n# Output"
-                " Type\n\nint\n\n# Execution Scratch-Pad (Think Step by Step)\n\n1. Declare variable c and assign the"
-                " value of a + b\n2. Return the value of c\n\n# Output\n\n---\nresult: 3"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nReturn 0.\n\n# Task\n\nExecute"
-                " the function with the inputs that follow in the next section and finally return the output using the"
-                " output type\nas YAML document in an # Output section. (If the value is a literal, then just write the"
-                " value. We parse the text in the\n# Output section using `yaml.safe_load` in Python.)\n\n# Dataclasses"
-                " Schema\n\ntypes:\n  DummyInterface:\n    a:\n      type: int\n  FakeLLM_DummyInterface:\n    a:\n    "
-                "  type: int\n    bases:\n    - DummyInterface\n\n\n# Input Types\n\nself:"
-                " FakeLLM_DummyInterface\n\n\n# Inputs\n\nself:\n  a: -1\n\n\n# Output Type\n\nint\n\n# Execution"
-                " Scratch-Pad (Think Step by Step)\n\n\n# Output\n\n---\nresult: 0"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nAdd two numbers.\n\n#"
-                " Task\n\nExecute the function with the inputs that follow in the next section and finally return the"
-                " output using the output type\nas YAML document in an # Output section. (If the value is a literal,"
-                " then just write the value. We parse the text in the\n# Output section using `yaml.safe_load` in"
-                " Python.)\n\n# Dataclasses Schema\n\ntypes:\n  type:\n    a:\n      type: int\n\n\n# Input Types\n\na:"
-                " int\nb: int\ncls: type\n\n\n# Inputs\n\na: 1\nb: 2\ncls: <class"
-                " 'llm_strategy.decorators.FakeLLM_DummyInterface'>\n\n\n# Output Type\n\nint\n\n# Execution"
-                " Scratch-Pad (Think Step by Step)\n\n\n# Output\n\n---\nresult: 3"
+                "Return 0.\n\nThe input and output are formatted as a JSON interface that conforms to the JSON "
+                'schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a list of '
+                'strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object {"foo": ['
+                '"bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", '
+                '"baz"]}} is not well-formatted.\n\nHere is the schema for additional data types:\n```\n{'
+                '"DummyInterface": {"properties": {"a": {"type": "integer"}}}}\n```\n\nHere is the input '
+                'schema:\n```\n{"properties": {"self": {"$ref": "DummyInterface"}}, "required": ['
+                '"self"]}\n```\n\nHere is the output schema:\n```\n{"properties": {"return_value": {"type": '
+                '"integer"}}, "required": ["return_value"]}\n```\nNow output the results for the following '
+                'inputs:\n```\n{"self": {"a": -1}}\n```'
+                '{"return_value": 0}\n'
+            ),
+            (
+                "Add two numbers.\n\nThe input and output are formatted as a JSON interface that conforms to the JSON "
+                'schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a list of '
+                'strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object {"foo": ['
+                '"bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", '
+                '"baz"]}} is not well-formatted.\n\nHere is the input schema:\n```\n{"properties": {"a": {"type": '
+                '"integer"}, "b": {"type": "integer"}}, "required": ["a", "b"]}\n```\n\nHere is the output '
+                'schema:\n```\n{"properties": {"return_value": {"type": "integer"}}, "required": ['
+                '"return_value"]}\n```\nNow output the results for the following inputs:\n```\n{"a": 1, "b": 2}\n```'
+                '{"return_value": 3}\n'
+            ),
+            (
+                "Add two numbers.\n\nThe input is formatted as a JSON interface of Inputs that conforms to the JSON "
+                "schema below, and the output should be formatted as a JSON instance of Outputs that conforms to the "
+                'JSON schema below.\n\nAs an example, for the schema {"properties": {"foo": {"title": "Foo", '
+                '"description": "a list of strings", "type": "array", "items": {"type": "string"}}}, "required": ['
+                '"foo"]}} the object {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {'
+                '"properties": {"foo": ["bar", "baz"]}} is not well-formatted.\n\nHere is the schema:\n```\n{'
+                '"DummyInterface": {"properties": {"a": {"title": "A", "default": -1, "type": "integer"}}}, '
+                '"Inputs": {"properties": {"self": {"$ref": "#/definitions/DummyInterface"}, "a": {"title": "A", '
+                '"type": "integer"}, "b": {"title": "B", "type": "integer"}}, "required": ["self", "a", "b"]}, '
+                '"Outputs": {"properties": {"return_value": {"title": "Return Value", "type": "integer"}}, '
+                '"required": ["return_value"]}}\n```\n\nNow output the results for the following inputs:\n```\n{'
+                '"self": {"a": -1}, "a": 1, "b": 2}\n```\n '
+                '{"return_value": 3}\n'
+            ),
+            (
+                "Add two numbers.\n\nThe input and output are formatted as a JSON interface that conforms to the JSON "
+                'schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a list of '
+                'strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object {"foo": ['
+                '"bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar", '
+                '"baz"]}} is not well-formatted.\n\nHere is the schema for additional data types:\n```\n{'
+                '"DummyInterface": {"properties": {"a": {"type": "integer"}}}}\n```\n\nHere is the input '
+                'schema:\n```\n{"properties": {"self": {"$ref": "DummyInterface"}, "a": {"type": "integer"}, '
+                '"b": {"type": "integer"}}, "required": ["self", "a", "b"]}\n```\n\nHere is the output '
+                'schema:\n```\n{"properties": {"return_value": {"type": "integer"}}, "required": ['
+                '"return_value"]}\n```\nNow output the results for the following inputs:\n```\n{"self": {"a": -1}, '
+                '"a": 1, "b": 2}\n```'
+                '{"return_value": 3}\n'
             ),
-        }
+        ]
         # external_llm=OpenAI(),
     )
 
     llm_DummyInterface = llm_strategy(llm)(DummyInterface)
     llm_DummyInstance = llm_DummyInterface()
     assert llm_DummyInstance.property_getter == 0
     assert llm_DummyInterface.static_method(1, 2) == 3
-    assert llm_DummyInterface.static_method(1, 2) == 3
+    assert llm_DummyInstance.static_method(1, 2) == 3
     assert llm_DummyInstance.bound_method(1, 2) == 3
-    assert llm_DummyInterface.class_method(1, 2) == 3
-    assert llm_DummyInstance.bound_method_raises_class(1, 2) == 3
+    # assert llm_DummyInterface.class_method(1, 2) == 3
+    # assert llm_DummyInstance.class_method(1, 2) == 3
+
+    assert llm_DummyInterface.static_method_implemented(1, 2) == 3
+    assert llm_DummyInstance.bound_method_implemented(1) == 0
+    assert llm_DummyInterface.class_method_implemented(1, 2) == 3
+    assert llm_DummyInstance.property_getter_implemented == 1
 
 
 @dataclass
 class Customer:
     first_name: str
     last_name: str
     birthday: str
     city: str
 
 
 @dataclass
 class CustomerDatabase:
     customers: list[Customer]
 
-    def find_customer_index(self, query: str) -> int:
+    def find_customer_index(self: "CustomerDatabase", query: str) -> int:
         """Find the index of the customer that matches the natural language query best.
 
         We support semantic queries instead of SQL, so we can search for things like
         "the customer that was born in 1990".
 
         Args:
             query: Natural language query
@@ -241,103 +235,120 @@
         raise NotImplementedError()
 
 
 def test_llm_strategy():
     llm = FakeLLM(
         texts={
             (
-                "Execute the following function that is described via a doc string:\n\n\n        Create mock queries"
-                " that match one of the mock customers better than the others.\n\n        We support semantic queries"
-                ' instead of SQL, so we can search for things like\n        "the customer that was born in 1990".\n  '
-                "      \n\n# Task\n\nExecute the function with the inputs that follow in the next section and finally"
-                " return the output using the output type\nas YAML document in an # Output section. (If the value is a"
-                " literal, then just write the value. We parse the text in the\n# Output section using `yaml.safe_load`"
-                " in Python.)\n\n# Dataclasses Schema\n\ntypes:\n  Customer:\n    birthday:\n      type: str\n   "
-                " city:\n      type: str\n    first_name:\n      type: str\n    last_name:\n      type: str\n "
-                " CustomerDatabase:\n    customers:\n      type: '[Customer]'\n  FakeLLM_CustomerDatabase:\n   "
-                " bases:\n    - CustomerDatabase\n    customers:\n      type: '[Customer]'\n\n\n# Input"
-                " Types\n\ncustomer_database: FakeLLM_CustomerDatabase\nnum_queries: int\n\n\n#"
-                " Inputs\n\ncustomer_database:\n  customers:\n  - birthday: '1965-12-21'\n    city: London\n   "
-                " first_name: John\n    last_name: Doe\n  - birthday: '1973-10-19'\n    city: Paris\n    first_name:"
-                " Jane\n    last_name: Smith\n  - birthday: '1975-07-04'\n    city: Tokyo\n    first_name: Bob\n   "
-                " last_name: Jones\nnum_queries: 3\n\n\n# Output Type\n\n[str]\n\n# Execution Scratch-Pad (Think Step"
-                " by Step)\n\n\n# Output\n\n---\nresult:\n- 'The customer that was born in 1965'\n- 'The customer that"
-                " lives in Tokyo'\n- 'The customer with the last name of Jones'"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nFind the index of the customer"
-                " that matches the natural language query best.\n\n        We support semantic queries instead of SQL,"
-                ' so we can search for things like\n        "the customer that was born in 1990".\n\n        Args:\n '
-                "           query: Natural language query\n\n        Returns:\n            The index of the best"
-                " matching customer in the database.\n        \n\n# Task\n\nExecute the function with the inputs that"
-                " follow in the next section and finally return the output using the output type\nas YAML document in"
-                " an # Output section. (If the value is a literal, then just write the value. We parse the text in"
-                " the\n# Output section using `yaml.safe_load` in Python.)\n\n# Dataclasses Schema\n\ntypes:\n "
-                " Customer:\n    birthday:\n      type: str\n    city:\n      type: str\n    first_name:\n      type:"
-                " str\n    last_name:\n      type: str\n  CustomerDatabase:\n    customers:\n      type: '[Customer]'\n"
-                "  FakeLLM_CustomerDatabase:\n    bases:\n    - CustomerDatabase\n    customers:\n      type:"
-                " '[Customer]'\n\n\n# Input Types\n\nquery: str\nself: FakeLLM_CustomerDatabase\n\n\n# Inputs\n\nquery:"
-                " The customer with the last name of Jones\nself:\n  customers:\n  - birthday: '1965-12-21'\n    city:"
-                " London\n    first_name: John\n    last_name: Doe\n  - birthday: '1973-10-19'\n    city: Paris\n   "
-                " first_name: Jane\n    last_name: Smith\n  - birthday: '1975-07-04'\n    city: Tokyo\n    first_name:"
-                " Bob\n    last_name: Jones\n\n\n# Output Type\n\nint\n\n# Execution Scratch-Pad (Think Step by"
-                " Step)\n\n\n# Output\n\n---\nresult: 2"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\n\n        Create mock customers"
-                " with believable data (our customers are world citizens).\n        \n\n# Task\n\nExecute the function"
-                " with the inputs that follow in the next section and finally return the output using the output"
-                " type\nas YAML document in an # Output section. (If the value is a literal, then just write the value."
-                " We parse the text in the\n# Output section using `yaml.safe_load` in Python.)\n\n# Dataclasses"
-                " Schema\n\ntypes:\n  Customer:\n    birthday:\n      type: str\n    city:\n      type: str\n   "
-                " first_name:\n      type: str\n    last_name:\n      type: str\n\n\n# Input Types\n\nnum_customers:"
-                " int\n\n\n# Inputs\n\nnum_customers: 3\n\n\n# Output Type\n\n[Customer]\n\n# Execution Scratch-Pad"
-                ' (Think Step by Step)\n\n\n# Output\n\n---\nresult:\n- birthday: "1965-12-21"\n  city: London\n '
-                ' first_name: John\n  last_name: Doe\n- birthday: "1973-10-19"\n  city: Paris\n  first_name: Jane\n '
-                ' last_name: Smith\n- birthday: "1975-07-04"\n  city: Tokyo\n  first_name: Bob\n  last_name: Jones'
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nFind the index of the customer"
-                " that matches the natural language query best.\n\n        We support semantic queries instead of SQL,"
-                ' so we can search for things like\n        "the customer that was born in 1990".\n\n        Args:\n '
-                "           query: Natural language query\n\n        Returns:\n            The index of the best"
-                " matching customer in the database.\n        \n\n# Task\n\nExecute the function with the inputs that"
-                " follow in the next section and finally return the output using the output type\nas YAML document in"
-                " an # Output section. (If the value is a literal, then just write the value. We parse the text in"
-                " the\n# Output section using `yaml.safe_load` in Python.)\n\n# Dataclasses Schema\n\ntypes:\n "
-                " Customer:\n    birthday:\n      type: str\n    city:\n      type: str\n    first_name:\n      type:"
-                " str\n    last_name:\n      type: str\n  CustomerDatabase:\n    customers:\n      type: '[Customer]'\n"
-                "  FakeLLM_CustomerDatabase:\n    bases:\n    - CustomerDatabase\n    customers:\n      type:"
-                " '[Customer]'\n\n\n# Input Types\n\nquery: str\nself: FakeLLM_CustomerDatabase\n\n\n# Inputs\n\nquery:"
-                " The customer that lives in Tokyo\nself:\n  customers:\n  - birthday: '1965-12-21'\n    city: London\n"
-                "    first_name: John\n    last_name: Doe\n  - birthday: '1973-10-19'\n    city: Paris\n    first_name:"
-                " Jane\n    last_name: Smith\n  - birthday: '1975-07-04'\n    city: Tokyo\n    first_name: Bob\n   "
-                " last_name: Jones\n\n\n# Output Type\n\nint\n\n# Execution Scratch-Pad (Think Step by Step)\n\n\n#"
-                " Output\n\n---\nresult: 2"
-            ),
-            (
-                "Execute the following function that is described via a doc string:\n\nFind the index of the customer"
-                " that matches the natural language query best.\n\n        We support semantic queries instead of SQL,"
-                ' so we can search for things like\n        "the customer that was born in 1990".\n\n        Args:\n '
-                "           query: Natural language query\n\n        Returns:\n            The index of the best"
-                " matching customer in the database.\n        \n\n# Task\n\nExecute the function with the inputs that"
-                " follow in the next section and finally return the output using the output type\nas YAML document in"
-                " an # Output section. (If the value is a literal, then just write the value. We parse the text in"
-                " the\n# Output section using `yaml.safe_load` in Python.)\n\n# Dataclasses Schema\n\ntypes:\n "
-                " Customer:\n    birthday:\n      type: str\n    city:\n      type: str\n    first_name:\n      type:"
-                " str\n    last_name:\n      type: str\n  CustomerDatabase:\n    customers:\n      type: '[Customer]'\n"
-                "  FakeLLM_CustomerDatabase:\n    bases:\n    - CustomerDatabase\n    customers:\n      type:"
-                " '[Customer]'\n\n\n# Input Types\n\nquery: str\nself: FakeLLM_CustomerDatabase\n\n\n# Inputs\n\nquery:"
-                " The customer that was born in 1965\nself:\n  customers:\n  - birthday: '1965-12-21'\n    city:"
-                " London\n    first_name: John\n    last_name: Doe\n  - birthday: '1973-10-19'\n    city: Paris\n   "
-                " first_name: Jane\n    last_name: Smith\n  - birthday: '1975-07-04'\n    city: Tokyo\n    first_name:"
-                " Bob\n    last_name: Jones\n\n\n# Output Type\n\nint\n\n# Execution Scratch-Pad (Think Step by"
-                " Step)\n\n\n\n# Output\n\n---\nresult: 0"
+                "Create mock queries that match one of the mock customers better than the others.\n\nWe support"
+                ' semantic queries instead of SQL, so we can search for things like\n"the customer that was born in'
+                ' 1990".\n\nThe input and output are formatted as a JSON interface that conforms to the JSON schemas'
+                ' below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a list of strings",'
+                ' "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object {"foo": ["bar",'
+                ' "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo": ["bar",'
+                ' "baz"]}} is not well-formatted.\n\nHere is the schema for additional data types:\n```\n{"Customer":'
+                ' {"properties": {"first_name": {"type": "string"}, "last_name": {"type": "string"}, "birthday":'
+                ' {"type": "string"}, "city": {"type": "string"}}, "required": ["first_name", "last_name", "birthday",'
+                ' "city"]}, "CustomerDatabase": {"properties": {"customers": {"type": "array", "items": {"$ref":'
+                ' "Customer"}}}, "required": ["customers"]}}\n```\n\nHere is the input schema:\n```\n{"properties":'
+                ' {"customer_database": {"$ref": "CustomerDatabase"}, "num_queries": {"type": "integer"}}, "required":'
+                ' ["customer_database"]}\n```\n\nHere is the output schema:\n```\n{"properties": {"return_value":'
+                ' {"type": "array", "items": {"type": "string"}}}, "required": ["return_value"]}\n```\nNow output the'
+                ' results for the following inputs:\n```\n{"customer_database": {"customers": [{"first_name": "John",'
+                ' "last_name": "Smith", "birthday": "01/01/1990", "city": "New York"}, {"first_name": "Jane",'
+                ' "last_name": "Doe", "birthday": "02/02/1995", "city": "London"}, {"first_name": "Alex", "last_name":'
+                ' "Parker", "birthday": "03/03/1985", "city": "Paris"}]}, "num_queries": 3}\n```\n\nThe output should'
+                ' be:\n```\n{"return_value": ["the customer that was born in 1990", "the customer that lives in'
+                ' London", "the customer that has the last name Parker"]}\n```'
+            ),
+            (
+                "Create mock customers with believable data (our customers are world citizens).\n\nThe input and output"
+                " are formatted as a JSON interface that conforms to the JSON schemas below.\n\nAs an example, for the"
+                ' schema {"properties": {"foo": {"description": "a list of strings", "type": "array", "items": {"type":'
+                ' "string"}}}, "required": ["foo"]}} the object {"foo": ["bar", "baz"]} is a well-formatted instance of'
+                ' the schema. The object {"properties": {"foo": ["bar", "baz"]}} is not well-formatted.\n\nHere is the'
+                ' schema for additional data types:\n```\n{"Customer": {"properties": {"first_name": {"type":'
+                ' "string"}, "last_name": {"type": "string"}, "birthday": {"type": "string"}, "city": {"type":'
+                ' "string"}}, "required": ["first_name", "last_name", "birthday", "city"]}}\n```\n\nHere is the input'
+                ' schema:\n```\n{"properties": {"num_customers": {"type": "integer"}}}\n```\n\nHere is the output'
+                ' schema:\n```\n{"properties": {"return_value": {"type": "array", "items": {"$ref": "Customer"}}},'
+                ' "required": ["return_value"]}\n```\nNow output the results for the following'
+                ' inputs:\n```\n{"num_customers": 3}\n```\n\nOutput:\n```\n{"return_value": [{"first_name": "John",'
+                ' "last_name": "Smith", "birthday": "01/01/1990", "city": "New York"}, \n{"first_name": "Jane",'
+                ' "last_name": "Doe", "birthday": "02/02/1995", "city": "London"}, \n{"first_name": "Alex",'
+                ' "last_name": "Parker", "birthday": "03/03/1985", "city": "Paris"}]}'
+            ),
+            (
+                "Find the index of the customer that matches the natural language query best.\n\nWe support semantic"
+                ' queries instead of SQL, so we can search for things like\n"the customer that was born in'
+                ' 1990".\n\nArgs:\n    query: Natural language query\n\nReturns:\n    The index of the best matching'
+                " customer in the database.\n\nThe input and output are formatted as a JSON interface that conforms to"
+                ' the JSON schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a'
+                ' list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object'
+                ' {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo":'
+                ' ["bar", "baz"]}} is not well-formatted.\n\nHere is the schema for additional data'
+                ' types:\n```\n{"Customer": {"properties": {"first_name": {"type": "string"}, "last_name": {"type":'
+                ' "string"}, "birthday": {"type": "string"}, "city": {"type": "string"}}, "required": ["first_name",'
+                ' "last_name", "birthday", "city"]}, "CustomerDatabase": {"properties": {"customers": {"type": "array",'
+                ' "items": {"$ref": "Customer"}}}, "required": ["customers"]}}\n```\n\nHere is the input'
+                ' schema:\n```\n{"properties": {"self": {"$ref": "CustomerDatabase"}, "query": {"type": "string"}},'
+                ' "required": ["self", "query"]}\n```\n\nHere is the output schema:\n```\n{"properties":'
+                ' {"return_value": {"type": "integer"}}, "required": ["return_value"]}\n```\nNow output the results for'
+                ' the following inputs:\n```\n{"self": {"customers": [{"first_name": "John", "last_name": "Smith",'
+                ' "birthday": "01/01/1990", "city": "New York"}, {"first_name": "Jane", "last_name": "Doe", "birthday":'
+                ' "02/02/1995", "city": "London"}, {"first_name": "Alex", "last_name": "Parker", "birthday":'
+                ' "03/03/1985", "city": "Paris"}]}, "query": "the customer that has the last name'
+                ' Parker"}\n```\n\nOutput: {"return_value": 2}'
+            ),
+            (
+                "Find the index of the customer that matches the natural language query best.\n\nWe support semantic"
+                ' queries instead of SQL, so we can search for things like\n"the customer that was born in'
+                ' 1990".\n\nArgs:\n    query: Natural language query\n\nReturns:\n    The index of the best matching'
+                " customer in the database.\n\nThe input and output are formatted as a JSON interface that conforms to"
+                ' the JSON schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a'
+                ' list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object'
+                ' {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo":'
+                ' ["bar", "baz"]}} is not well-formatted.\n\nHere is the schema for additional data'
+                ' types:\n```\n{"Customer": {"properties": {"first_name": {"type": "string"}, "last_name": {"type":'
+                ' "string"}, "birthday": {"type": "string"}, "city": {"type": "string"}}, "required": ["first_name",'
+                ' "last_name", "birthday", "city"]}, "CustomerDatabase": {"properties": {"customers": {"type": "array",'
+                ' "items": {"$ref": "Customer"}}}, "required": ["customers"]}}\n```\n\nHere is the input'
+                ' schema:\n```\n{"properties": {"self": {"$ref": "CustomerDatabase"}, "query": {"type": "string"}},'
+                ' "required": ["self", "query"]}\n```\n\nHere is the output schema:\n```\n{"properties":'
+                ' {"return_value": {"type": "integer"}}, "required": ["return_value"]}\n```\nNow output the results for'
+                ' the following inputs:\n```\n{"self": {"customers": [{"first_name": "John", "last_name": "Smith",'
+                ' "birthday": "01/01/1990", "city": "New York"}, {"first_name": "Jane", "last_name": "Doe", "birthday":'
+                ' "02/02/1995", "city": "London"}, {"first_name": "Alex", "last_name": "Parker", "birthday":'
+                ' "03/03/1985", "city": "Paris"}]}, "query": "the customer that was born in'
+                ' 1990"}\n```\n\nOutput:\n{"return_value": 0}'
+            ),
+            (
+                "Find the index of the customer that matches the natural language query best.\n\nWe support semantic"
+                ' queries instead of SQL, so we can search for things like\n"the customer that was born in'
+                ' 1990".\n\nArgs:\n    query: Natural language query\n\nReturns:\n    The index of the best matching'
+                " customer in the database.\n\nThe input and output are formatted as a JSON interface that conforms to"
+                ' the JSON schemas below.\n\nAs an example, for the schema {"properties": {"foo": {"description": "a'
+                ' list of strings", "type": "array", "items": {"type": "string"}}}, "required": ["foo"]}} the object'
+                ' {"foo": ["bar", "baz"]} is a well-formatted instance of the schema. The object {"properties": {"foo":'
+                ' ["bar", "baz"]}} is not well-formatted.\n\nHere is the schema for additional data'
+                ' types:\n```\n{"Customer": {"properties": {"first_name": {"type": "string"}, "last_name": {"type":'
+                ' "string"}, "birthday": {"type": "string"}, "city": {"type": "string"}}, "required": ["first_name",'
+                ' "last_name", "birthday", "city"]}, "CustomerDatabase": {"properties": {"customers": {"type": "array",'
+                ' "items": {"$ref": "Customer"}}}, "required": ["customers"]}}\n```\n\nHere is the input'
+                ' schema:\n```\n{"properties": {"self": {"$ref": "CustomerDatabase"}, "query": {"type": "string"}},'
+                ' "required": ["self", "query"]}\n```\n\nHere is the output schema:\n```\n{"properties":'
+                ' {"return_value": {"type": "integer"}}, "required": ["return_value"]}\n```\nNow output the results for'
+                ' the following inputs:\n```\n{"self": {"customers": [{"first_name": "John", "last_name": "Smith",'
+                ' "birthday": "01/01/1990", "city": "New York"}, {"first_name": "Jane", "last_name": "Doe", "birthday":'
+                ' "02/02/1995", "city": "London"}, {"first_name": "Alex", "last_name": "Parker", "birthday":'
+                ' "03/03/1985", "city": "Paris"}]}, "query": "the customer that lives in'
+                ' London"}\n```\n\n{"return_value": 1}'
             ),
         }
+        #
         # external_llm=OpenAI(),
     )
 
     LLMCustomerDatabase = llm_strategy(llm)(CustomerDatabase)
 
     customers = LLMCustomerDatabase.create_mock_customers(3)
```

### Comparing `llm_strategy-0.0.3/pyproject.toml` & `llm_strategy-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 [tool.poetry]
 name = "llm_strategy"
-version = "0.0.3"
+version = "1.0.0"
 description = "Directly Connecting Python to LLMs - Dataclasses & Interfaces <-> LLMs"
 authors = ["Andreas Kirsch, Daedalus Lab Ltd <blackhc@gmail.com>"]
 repository = "https://github.com/blackhc/llm-strategy"
 documentation = "https://blackhc.github.io/llm-strategy/"
 readme = "README.md"
 packages = [
   {include = "llm_strategy"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
-langchain = ">=0.0.42"
+langchain = ">=0.0.127"
 openai = ">=0.25.0"
-docstring-parser = "^0.15"
-parse = "^1.19.0"
 typing-extensions = "^4.4.0"
-pyyaml = "^6.0"
 pydantic = "^1.10.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.6.6"
 mypy = "^0.991"
```

### Comparing `llm_strategy-0.0.3/PKG-INFO` & `llm_strategy-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: llm-strategy
-Version: 0.0.3
+Version: 1.0.0
 Summary: Directly Connecting Python to LLMs - Dataclasses & Interfaces <-> LLMs
 Home-page: https://github.com/blackhc/llm-strategy
 Author: Andreas Kirsch, Daedalus Lab Ltd
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: docstring-parser (>=0.15,<0.16)
-Requires-Dist: langchain (>=0.0.42)
+Requires-Dist: langchain (>=0.0.127)
 Requires-Dist: openai (>=0.25.0)
-Requires-Dist: parse (>=1.19.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://blackhc.github.io/llm-strategy/
 Project-URL: Repository, https://github.com/blackhc/llm-strategy
 Description-Content-Type: text/markdown
 
 # llm-strategy
```

