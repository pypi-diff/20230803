# Comparing `tmp/dataclasses_struct-0.7.0.tar.gz` & `tmp/dataclasses_struct-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_struct-0.7.0.tar", max compression
+gzip compressed data, was "dataclasses_struct-0.8.0.tar", max compression
```

## Comparing `dataclasses_struct-0.7.0.tar` & `dataclasses_struct-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.7.0/LICENSE
--rw-r--r--   0        0        0     5340 2023-07-28 03:31:38.580475 dataclasses_struct-0.7.0/README.md
--rw-r--r--   0        0        0      706 2023-07-27 21:59:59.471071 dataclasses_struct-0.7.0/dataclasses_struct/__init__.py
--rw-r--r--   0        0        0     8928 2023-07-28 03:31:38.580475 dataclasses_struct-0.7.0/dataclasses_struct/dataclass.py
--rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.7.0/dataclasses_struct/ext/__init__.py
--rw-r--r--   0        0        0     1834 2023-07-28 03:31:38.580475 dataclasses_struct-0.7.0/dataclasses_struct/ext/mypy_plugin.py
--rw-r--r--   0        0        0     4429 2023-07-27 22:31:52.560957 dataclasses_struct-0.7.0/dataclasses_struct/field.py
--rw-r--r--   0        0        0      313 2023-07-27 22:18:30.718550 dataclasses_struct-0.7.0/dataclasses_struct/intsizes.py
--rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.7.0/dataclasses_struct/py.typed
--rw-r--r--   0        0        0     1340 2023-07-27 21:05:55.445954 dataclasses_struct-0.7.0/dataclasses_struct/types.py
--rw-r--r--   0        0        0     1046 2023-07-28 03:32:25.032358 dataclasses_struct-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6171 1970-01-01 00:00:00.000000 dataclasses_struct-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5481 2023-08-03 20:48:52.178708 dataclasses_struct-0.8.0/README.md
+-rw-r--r--   0        0        0      756 2023-08-03 20:48:52.178708 dataclasses_struct-0.8.0/dataclasses_struct/__init__.py
+-rw-r--r--   0        0        0     9432 2023-08-03 20:48:56.654693 dataclasses_struct-0.8.0/dataclasses_struct/dataclass.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.0/dataclasses_struct/ext/__init__.py
+-rw-r--r--   0        0        0     1834 2023-08-03 20:21:38.340118 dataclasses_struct-0.8.0/dataclasses_struct/ext/mypy_plugin.py
+-rw-r--r--   0        0        0     4429 2023-07-27 22:31:52.560957 dataclasses_struct-0.8.0/dataclasses_struct/field.py
+-rw-r--r--   0        0        0      313 2023-07-27 22:18:30.718550 dataclasses_struct-0.8.0/dataclasses_struct/intsizes.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.0/dataclasses_struct/py.typed
+-rw-r--r--   0        0        0     1340 2023-08-03 02:47:39.912029 dataclasses_struct-0.8.0/dataclasses_struct/types.py
+-rw-r--r--   0        0        0     1046 2023-08-03 20:51:53.342123 dataclasses_struct-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6312 1970-01-01 00:00:00.000000 dataclasses_struct-0.8.0/PKG-INFO
```

### Comparing `dataclasses_struct-0.7.0/LICENSE` & `dataclasses_struct-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.7.0/README.md` & `dataclasses_struct-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,17 @@
 [dataclass](https://docs.python.org/3/library/dataclasses.html) with boilerplate
 `__init__`, `__repr__`, `__eq__` etc. auto-generated. Additionally, two methods
 are added to the class: `pack`, a method for packing an instance of the class to
 `bytes`, and `from_packed`, a class method that returns a new instance of the
 class from its packed `bytes` representation.
 
 A class or object can be check to see if it is a dataclass-struct using the
-`is_dataclass_struct` function.
+`is_dataclass_struct` function. The `get_struct_size` function will return
+the size in bytes of the packed representation of a dataclass_struct class
+or an instance of one.
 
 An additional class attribute, `__dataclass_struct__`. The [`struct` format
 string](https://docs.python.org/3/library/struct.html#format-strings), packed
 size, and endianness can be accessed like so:
 
 ```python
 >>> Test.__dataclass_struct__.format
```

### Comparing `dataclasses_struct-0.7.0/dataclasses_struct/__init__.py` & `dataclasses_struct-0.8.0/dataclasses_struct/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from importlib import metadata
 
 __version__ = metadata.version(__package__)
 
 from .dataclass import (
     dataclass,
+    get_struct_size,
     is_dataclass_struct,
+    DataclassStructProtocol,
     ENDIANS,
     NATIVE_ENDIAN_ALIGNED,
     NATIVE_ENDIAN,
     LITTLE_ENDIAN,
     BIG_ENDIAN,
     NETWORK_ENDIAN,
 )
```

### Comparing `dataclasses_struct-0.7.0/dataclasses_struct/dataclass.py` & `dataclasses_struct-0.8.0/dataclasses_struct/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Generator, Iterator
 import dataclasses
-import struct
+from struct import Struct
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Protocol,
@@ -59,15 +59,15 @@
     return pad_before, pad_after, field
 
 
 T = TypeVar('T')
 
 
 class _DataclassStructInternal(Generic[T]):
-    struct: struct.Struct
+    struct: Struct
     cls: Type[T]
     _fieldnames: List[str]
     _fieldtypes: List[type]
 
     @property
     def format(self) -> str:
         return self.struct.format
@@ -83,15 +83,15 @@
     def __init__(
         self,
         fmt: str,
         cls: type,
         fieldnames: List[str],
         fieldtypes: List[type],
     ):
-        self.struct = struct.Struct(fmt)
+        self.struct = Struct(fmt)
         self.cls = cls
         self._fieldnames = fieldnames
         self._fieldtypes = fieldtypes
 
     def _flattened_attrs(self, obj) -> List[Any]:
         """
         Returns a list of all attributes, including those of any nested structs
@@ -109,29 +109,34 @@
         return self.struct.pack(*self._flattened_attrs(obj))
 
     def _arg_generator(self, args: Iterator) -> Generator:
         for fieldtype in self._fieldtypes:
             if is_dataclass_struct(fieldtype):
                 yield fieldtype.__dataclass_struct__._init_from_args(args)
             else:
-                yield next(args)
+                yield fieldtype(next(args))
 
     def _init_from_args(self, args: Iterator) -> T:
         """
         Returns an instance of self.cls, consuming args
         """
         return self.cls(*self._arg_generator(args))
 
     def unpack(self, data: bytes) -> T:
         return self._init_from_args(iter(self.struct.unpack(data)))
 
 
 class DataclassStructProtocol(Protocol):
     __dataclass_struct__: _DataclassStructInternal
 
+    @classmethod
+    def from_packed(cls: Type[T], data: bytes) -> T: ...
+
+    def pack(self) -> bytes: ...
+
 
 @overload
 def is_dataclass_struct(obj: type) -> TypeGuard[Type[DataclassStructProtocol]]:
     ...
 
 
 @overload
@@ -150,14 +155,24 @@
     return (
         dataclasses.is_dataclass(obj)
         and hasattr(obj, '__dataclass_struct__')
         and isinstance(obj.__dataclass_struct__, _DataclassStructInternal)
     )
 
 
+def get_struct_size(cls_or_obj: Any) -> int:
+    """
+    Returns the size of the packed representation of the struct in bytes.
+    Accepts either a class or an instance of a dataclass_struct.
+    """
+    if not is_dataclass_struct(cls_or_obj):
+        raise TypeError(f'{cls_or_obj} is not a dataclass_struct')
+    return cls_or_obj.__dataclass_struct__.size
+
+
 class _NestedField(Field):
     type_: Type[DataclassStructProtocol]
 
     def __init__(self, cls: Type[DataclassStructProtocol]):
         self.type_ = cls
 
     def format(self) -> str:
@@ -271,15 +286,15 @@
     scope: Dict[str, Any] = {'cls_type': cls}
     exec(func, {}, scope)
     return classmethod(scope['from_packed'])
 
 
 def _make_class(
     cls: type, endian: str, allow_native: bool, validate: bool
-) -> type:
+) -> Type[DataclassStructProtocol]:
     cls_annotations = get_type_hints(cls, include_extras=True)
     struct_format = [endian]
     fieldtypes = []
     for name, field in cls_annotations.items():
         fmt, type_ = _validate_and_parse_field(
             cls,
             name,
```

### Comparing `dataclasses_struct-0.7.0/dataclasses_struct/ext/mypy_plugin.py` & `dataclasses_struct-0.8.0/dataclasses_struct/ext/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.7.0/dataclasses_struct/field.py` & `dataclasses_struct-0.8.0/dataclasses_struct/field.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.7.0/dataclasses_struct/types.py` & `dataclasses_struct-0.8.0/dataclasses_struct/types.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.7.0/pyproject.toml` & `dataclasses_struct-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-struct"
-version = "0.7.0"
+version = "0.8.0"
 description = "Converting dataclasses to and from fixed-length binary data using struct"
 authors = ["Harry Mander <harrymander96@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/harrymander/dataclasses-struct"
 repository = "https://github.com/harrymander/dataclasses-struct"
 documentation = "https://github.com/harrymander/dataclasses-struct/blob/main/README.md#usage"
```

### Comparing `dataclasses_struct-0.7.0/PKG-INFO` & `dataclasses_struct-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-struct
-Version: 0.7.0
+Version: 0.8.0
 Summary: Converting dataclasses to and from fixed-length binary data using struct
 Home-page: https://github.com/harrymander/dataclasses-struct
 License: MIT
 Author: Harry Mander
 Author-email: harrymander96@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -150,15 +150,17 @@
 [dataclass](https://docs.python.org/3/library/dataclasses.html) with boilerplate
 `__init__`, `__repr__`, `__eq__` etc. auto-generated. Additionally, two methods
 are added to the class: `pack`, a method for packing an instance of the class to
 `bytes`, and `from_packed`, a class method that returns a new instance of the
 class from its packed `bytes` representation.
 
 A class or object can be check to see if it is a dataclass-struct using the
-`is_dataclass_struct` function.
+`is_dataclass_struct` function. The `get_struct_size` function will return
+the size in bytes of the packed representation of a dataclass_struct class
+or an instance of one.
 
 An additional class attribute, `__dataclass_struct__`. The [`struct` format
 string](https://docs.python.org/3/library/struct.html#format-strings), packed
 size, and endianness can be accessed like so:
 
 ```python
 >>> Test.__dataclass_struct__.format
```

