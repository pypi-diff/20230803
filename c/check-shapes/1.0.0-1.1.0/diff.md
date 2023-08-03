# Comparing `tmp/check_shapes-1.0.0.tar.gz` & `tmp/check_shapes-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_shapes-1.0.0.tar", max compression
+gzip compressed data, was "check_shapes-1.1.0.tar", max compression
```

## Comparing `check_shapes-1.0.0.tar` & `check_shapes-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    11357 2022-10-13 11:01:34.869189 check_shapes-1.0.0/LICENSE
--rw-r--r--   0        0        0     1147 2022-10-13 11:01:34.869189 check_shapes-1.0.0/README.md
--rw-r--r--   0        0        0     2348 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/__init__.py
--rw-r--r--   0        0        0     1756 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/accessors.py
--rw-r--r--   0        0        0     6712 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/argument_ref.py
--rw-r--r--   0        0        0     1106 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/base_types.py
--rw-r--r--   0        0        0     4213 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/bool_specs.py
--rw-r--r--   0        0        0     2908 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/check_shapes.lark
--rw-r--r--   0        0        0    22255 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/checker.py
--rw-r--r--   0        0        0     2775 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/checker_context.py
--rw-r--r--   0        0        0     5493 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/config.py
--rw-r--r--   0        0        0     7750 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/decorator.py
--rw-r--r--   0        0        0     1617 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/docstring.lark
--rw-r--r--   0        0        0    19129 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/error_contexts.py
--rw-r--r--   0        0        0     2624 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/exceptions.py
--rw-r--r--   0        0        0     2561 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/inheritance.py
--rw-r--r--   0        0        0        0 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/integration/__init__.py
--rw-r--r--   0        0        0     3046 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/integration/tf.py
--rw-r--r--   0        0        0     2297 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/integration/tfp.py
--rw-r--r--   0        0        0     1317 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/integration/torch.py
--rw-r--r--   0        0        0    25108 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/parser.py
--rw-r--r--   0        0        0        0 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/py.typed
--rw-r--r--   0        0        0     3374 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/shapes.py
--rw-r--r--   0        0        0     3226 2022-10-13 11:01:34.869189 check_shapes-1.0.0/check_shapes/specs.py
--rw-r--r--   0        0        0     4324 2022-10-13 11:01:34.877189 check_shapes-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 check_shapes-1.0.0/setup.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 check_shapes-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 14:20:56.824118 check_shapes-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1147 2023-08-03 14:20:56.824118 check_shapes-1.1.0/README.md
+-rw-r--r--   0        0        0     2436 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/__init__.py
+-rw-r--r--   0        0        0     1756 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/accessors.py
+-rw-r--r--   0        0        0     6712 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/argument_ref.py
+-rw-r--r--   0        0        0     1106 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/base_types.py
+-rw-r--r--   0        0        0     4213 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/bool_specs.py
+-rw-r--r--   0        0        0     2908 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/check_shapes.lark
+-rw-r--r--   0        0        0    22338 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/checker.py
+-rw-r--r--   0        0        0     2775 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/checker_context.py
+-rw-r--r--   0        0        0     5981 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/config.py
+-rw-r--r--   0        0        0     8043 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/decorator.py
+-rw-r--r--   0        0        0     1617 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/docstring.lark
+-rw-r--r--   0        0        0    19158 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/error_contexts.py
+-rw-r--r--   0        0        0     2624 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/exceptions.py
+-rw-r--r--   0        0        0     2561 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/inheritance.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/__init__.py
+-rw-r--r--   0        0        0     3046 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/tf.py
+-rw-r--r--   0        0        0     2297 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/tfp.py
+-rw-r--r--   0        0        0     1317 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/torch.py
+-rw-r--r--   0        0        0    25108 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/parser.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/py.typed
+-rw-r--r--   0        0        0     3374 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/shapes.py
+-rw-r--r--   0        0        0     3226 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/specs.py
+-rw-r--r--   0        0        0     4390 2023-08-03 14:20:56.828118 check_shapes-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 check_shapes-1.1.0/PKG-INFO
```

### Comparing `check_shapes-1.0.0/LICENSE` & `check_shapes-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/README.md` & `check_shapes-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/__init__.py` & `check_shapes-1.1.0/check_shapes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 from .base_types import Dimension, Shape
 from .checker import ShapeChecker
 from .checker_context import check_shape, get_shape_checker
 from .config import (
     DocstringFormat,
     ShapeCheckingState,
     disable_check_shapes,
+    get_drop_frames,
     get_enable_check_shapes,
     get_enable_function_call_precompute,
     get_rewrite_docstrings,
+    set_drop_frames,
     set_enable_check_shapes,
     set_enable_function_call_precompute,
     set_rewrite_docstrings,
 )
 from .decorator import check_shapes
 from .error_contexts import ErrorContext
 from .inheritance import inherit_check_shapes
@@ -37,15 +39,15 @@
 from .integration.torch import install_torch_integration
 from .shapes import get_shape, register_get_shape
 
 install_tf_integration()
 install_tfp_integration()
 install_torch_integration()
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 __all__ = [
     "Dimension",
     "DocstringFormat",
     "ErrorContext",
     "Shape",
     "ShapeChecker",
@@ -60,22 +62,24 @@
     "checker_context",
     "config",
     "decorator",
     "disable_check_shapes",
     "error_contexts",
     "exceptions",
     "get_check_shapes",
+    "get_drop_frames",
     "get_enable_check_shapes",
     "get_enable_function_call_precompute",
     "get_rewrite_docstrings",
     "get_shape",
     "get_shape_checker",
     "inherit_check_shapes",
     "inheritance",
     "parser",
     "register_get_shape",
+    "set_drop_frames",
     "set_enable_check_shapes",
     "set_enable_function_call_precompute",
     "set_rewrite_docstrings",
     "shapes",
     "specs",
 ]
```

### Comparing `check_shapes-1.0.0/check_shapes/accessors.py` & `check_shapes-1.1.0/check_shapes/accessors.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/argument_ref.py` & `check_shapes-1.1.0/check_shapes/argument_ref.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/base_types.py` & `check_shapes-1.1.0/check_shapes/base_types.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/bool_specs.py` & `check_shapes-1.1.0/check_shapes/bool_specs.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/check_shapes.lark` & `check_shapes-1.1.0/check_shapes/check_shapes.lark`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/checker.py` & `check_shapes-1.1.0/check_shapes/checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,17 @@
         n_unknown = len(unknown_len_variables)
 
         if n_unknown == 0:
             self._assert(unallocated_len == 0)
         else:
             self._assert(unallocated_len >= 0)
             if n_unknown == 1:
-                (expected_name,) = unknown_len_variables
+                (  # pylint: disable=unbalanced-dict-unpacking
+                    expected_name,
+                ) = unknown_len_variables
                 if expected_name is not None:
                     broadcastable = unknown_len_variables[expected_name]
                     if n_allocated_none <= 1 or (not broadcastable):
                         self._assert(unallocated_len % n_allocated_none == 0)
                         unknown_len = unallocated_len // n_allocated_none
                         allocated_sizes = [unknown_len if s is None else s for s in allocated_sizes]
```

### Comparing `check_shapes-1.0.0/check_shapes/checker_context.py` & `check_shapes-1.1.0/check_shapes/checker_context.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/config.py` & `check_shapes-1.1.0/check_shapes/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Code for configuring check_shapes."
 """
 from contextlib import contextmanager
 from enum import Enum
-from typing import Callable, Iterator, List, Union
+from typing import Callable, ContextManager, Iterator, List, Union
 
-IsCompiledMode = Callable[[], bool]
-
-
-_is_compiled_mode: List[IsCompiledMode] = []
-
-
-def add_is_compiled_mode(is_compiled_mode: IsCompiledMode) -> None:
-    """
-    Add a function for determining whether we are currently executing "compiled mode".
+from dropstackframe import get_enable_drop_stack_frame, set_enable_drop_stack_frame
 
-    Used when func:`set_enable_check_shapes` is set to ``EAGER_MODE_ONLY``.
-    """
-    _is_compiled_mode.append(is_compiled_mode)
+IsCompiledMode = Callable[[], bool]
 
 
 class ShapeCheckingState(Enum):
     """
     Different states of whether to actually check shapes.
     """
 
@@ -63,17 +53,14 @@
             # pylint: disable=no-member
             return not any(is_compiled_mode() for is_compiled_mode in _is_compiled_mode)
         else:
             assert self is ShapeCheckingState.DISABLED, self
             return False
 
 
-_enabled = ShapeCheckingState.EAGER_MODE_ONLY
-
-
 class DocstringFormat(Enum):
     """
     Enumeration of supported formats of docstrings.
     """
 
     SPHINX = "sphinx"
     """
@@ -82,19 +69,29 @@
 
     NONE = "none"
     """
     Do not rewrite docstrings.
     """
 
 
+_is_compiled_mode: List[IsCompiledMode] = []
+_enabled = ShapeCheckingState.EAGER_MODE_ONLY
 _docstring_format = DocstringFormat.SPHINX
-
 _function_call_precompute_enabled = False
 
 
+def add_is_compiled_mode(is_compiled_mode: IsCompiledMode) -> None:
+    """
+    Add a function for determining whether we are currently executing "compiled mode".
+
+    Used when func:`set_enable_check_shapes` is set to ``EAGER_MODE_ONLY``.
+    """
+    _is_compiled_mode.append(is_compiled_mode)
+
+
 def set_enable_check_shapes(enabled: Union[ShapeCheckingState, str, bool]) -> None:
     """
     Set whether to enable :mod:`check_shapes`.
 
     Check shapes has a non-zero impact on performance. If this is unacceptable to you, you can
     use this function to disable it.
 
@@ -188,7 +185,21 @@
 
 
 def get_enable_function_call_precompute() -> bool:
     """
     Get whether to precompute function call path and line numbers for debugging.
     """
     return _function_call_precompute_enabled
+
+
+def set_drop_frames(drop_frames: bool) -> ContextManager[None]:
+    """
+    Set whether :mod:`check_shapes` should hide itself from exception stack traces.
+    """
+    return set_enable_drop_stack_frame(drop_frames)
+
+
+def get_drop_frames() -> bool:
+    """
+    Get whether :mod:`check_shapes` should hide itself from exception stack traces.
+    """
+    return get_enable_drop_stack_frame()
```

### Comparing `check_shapes-1.0.0/check_shapes/decorator.py` & `check_shapes-1.1.0/check_shapes/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 Decorator for checking the shapes of function using tf Tensors.
 """
 import inspect
 from abc import ABC, abstractmethod
 from functools import update_wrapper
 from typing import Any, Callable, Sequence, cast
 
+from dropstackframe import drop_stack_frame
+
 from .accessors import set_check_shapes
 from .argument_ref import RESULT_TOKEN
 from .base_types import C
 from .checker import ShapeChecker
 from .checker_context import set_shape_checker
 from .config import get_enable_check_shapes
 from .error_contexts import (
@@ -113,15 +115,19 @@
 
     def _check_shapes(func: C) -> C:
         bound_error_context = FunctionDefinitionContext(func)
         signature = inspect.signature(func)
 
         def wrapped_function(*args: Any, **kwargs: Any) -> Any:
             if not get_enable_check_shapes():
-                return func(*args, **kwargs)
+                try:
+                    return func(*args, **kwargs)
+                except Exception:
+                    drop_stack_frame()
+                    raise
 
             try:
                 bound_arguments = signature.bind(*args, **kwargs)
             except TypeError as e:
                 # TypeError is raised if *args and **kwargs don't actually match the arguments of
                 # `func`. In that case we just call `func` normally, which will also result in an
                 # error, but an error with the error message the user is used to.
@@ -178,15 +184,19 @@
                         processed_specs.append((arg_value, arg_spec.tensor, arg_context))
 
                 checker.check_shapes(processed_specs)
 
             _check_specs(pre_specs)
 
             with set_shape_checker(checker):
-                result = func(*args, **kwargs)
+                try:
+                    result = func(*args, **kwargs)
+                except Exception:
+                    drop_stack_frame()
+                    raise
             arg_map[RESULT_TOKEN] = result
 
             _check_specs(post_specs)
 
             return result
 
         wrapped = wrapped_function
```

### Comparing `check_shapes-1.0.0/check_shapes/docstring.lark` & `check_shapes-1.1.0/check_shapes/docstring.lark`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/error_contexts.py` & `check_shapes-1.1.0/check_shapes/error_contexts.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     """
     An error occured in the context of a function definition.
     """
 
     func: Callable[..., Any]
 
     def print(self, builder: MessageBuilder) -> None:
-        name = self.func.__qualname__
+        name = getattr(self.func, "__qualname__", repr(self.func))
         try:
             path = inspect.getsourcefile(self.func)
         except Exception:  # pragma: no cover
             path = _UNKNOWN_FILE
         try:
             _, line_int = inspect.getsourcelines(self.func)
             line = str(line_int)
```

### Comparing `check_shapes-1.0.0/check_shapes/exceptions.py` & `check_shapes-1.1.0/check_shapes/exceptions.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/inheritance.py` & `check_shapes-1.1.0/check_shapes/inheritance.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/integration/tf.py` & `check_shapes-1.1.0/check_shapes/integration/tf.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/integration/tfp.py` & `check_shapes-1.1.0/check_shapes/integration/tfp.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/integration/torch.py` & `check_shapes-1.1.0/check_shapes/integration/torch.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/parser.py` & `check_shapes-1.1.0/check_shapes/parser.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/shapes.py` & `check_shapes-1.1.0/check_shapes/shapes.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/check_shapes/specs.py` & `check_shapes-1.1.0/check_shapes/specs.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.0.0/pyproject.toml` & `check_shapes-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "check_shapes"
-version = "1.0.0"
+version = "1.1.0"
 description = "A library for annotating and checking the shapes of tensors."
 authors = [
     "Jesper Nielsen <jespernielsen1982+check_shapes@gmail.com>",
     "The GPflow Contributors",
 ]
 license = "Apache-2.0"
 
@@ -20,28 +20,30 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Debuggers",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 lark = "^1.1.0"
-python = ">=3.7,<3.11"
+python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^5.2.2"
 black = "20.8b1"  # Pinned for backwards compatibility with the old stuff.
 click = "<8.1.0"  # Required by `black = "20.8b1"`.
+dropstackframe = ">=0.1.0"
 isort = "^5.10.0"
 matplotlib = "^3.0.0"
 mypy = ">0.920,!=0.982"
 numpy = "<1.22.0"  # MyPy is unhappy about Python 3.7 and newer versions of NumPy.
 # Pandas constrained to reduce Poetry search-time. Feel free to loosen this when we no longer need
 # to support Python 3.7:
 pandas = ">=1.1.0,<1.4.0"
```

### Comparing `check_shapes-1.0.0/PKG-INFO` & `check_shapes-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: check-shapes
-Version: 1.0.0
+Version: 1.1.0
 Summary: A library for annotating and checking the shapes of tensors.
 Home-page: https://gpflow.github.io/check_shapes
 License: Apache-2.0
 Author: Jesper Nielsen
 Author-email: jespernielsen1982+check_shapes@gmail.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Typing :: Typed
 Requires-Dist: lark (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://gpflow.github.io/check_shapes
 Project-URL: Repository, https://github.com/GPflow/check_shapes
```

