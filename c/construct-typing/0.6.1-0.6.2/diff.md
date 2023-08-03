# Comparing `tmp/construct-typing-0.6.1.tar.gz` & `tmp/construct-typing-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-typing-0.6.1.tar", last modified: Mon Jul 24 09:57:12 2023, max compression
+gzip compressed data, was "construct-typing-0.6.2.tar", last modified: Thu Aug  3 07:31:03 2023, max compression
```

## Comparing `construct-typing-0.6.1.tar` & `construct-typing-0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:57:12.940410 construct-typing-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 09:57:02.000000 construct-typing-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-24 09:57:12.940410 construct-typing-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-24 09:57:02.000000 construct-typing-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:57:12.936410 construct-typing-0.6.1/construct-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/expr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:57:12.936410 construct-typing-0.6.1/construct-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/lib/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/lib/bitstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/lib/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/lib/hex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/lib/py3compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:57:12.940410 construct-typing-0.6.1/construct_typed/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct_typed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct_typed/dataclass_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct_typed/generic_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct_typed/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct_typed/tenum.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 09:57:02.000000 construct-typing-0.6.1/construct_typed/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:57:12.940410 construct-typing-0.6.1/construct_typing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-24 09:57:12.000000 construct-typing-0.6.1/construct_typing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 09:57:12.000000 construct-typing-0.6.1/construct_typing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:57:12.000000 construct-typing-0.6.1/construct_typing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 09:57:12.000000 construct-typing-0.6.1/construct_typing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 09:57:12.000000 construct-typing-0.6.1/construct_typing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:57:12.940410 construct-typing-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-24 09:57:02.000000 construct-typing-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:03.479564 construct-typing-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 07:30:46.000000 construct-typing-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-08-03 07:31:03.479564 construct-typing-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-03 07:30:46.000000 construct-typing-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:03.475564 construct-typing-0.6.2/construct-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/expr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:03.479564 construct-typing-0.6.2/construct-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/lib/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/lib/bitstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/lib/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/lib/hex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/lib/py3compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:03.479564 construct-typing-0.6.2/construct_typed/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct_typed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct_typed/dataclass_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct_typed/generic_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct_typed/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct_typed/tenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 07:30:46.000000 construct-typing-0.6.2/construct_typed/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:03.479564 construct-typing-0.6.2/construct_typing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-08-03 07:31:03.000000 construct-typing-0.6.2/construct_typing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-03 07:31:03.000000 construct-typing-0.6.2/construct_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:31:03.000000 construct-typing-0.6.2/construct_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 07:31:03.000000 construct-typing-0.6.2/construct_typing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 07:31:03.000000 construct-typing-0.6.2/construct_typing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:31:03.479564 construct-typing-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-03 07:30:46.000000 construct-typing-0.6.2/setup.py
```

### Comparing `construct-typing-0.6.1/LICENSE` & `construct-typing-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/PKG-INFO` & `construct-typing-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-typing
-Version: 0.6.1
+Version: 0.6.2
 Summary: Extension for the python package 'construct' that adds typing features
 Home-page: https://github.com/timrid/construct-typing
 Author: Tim Riddermann
 License: MIT
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,annotation,type hint,typing,typed,bitstruct,PEP 561
 Platform: POSIX
 Platform: Windows
```

### Comparing `construct-typing-0.6.1/README.md` & `construct-typing-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/__init__.pyi` & `construct-typing-0.6.2/construct-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/core.pyi` & `construct-typing-0.6.2/construct-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/expr.pyi` & `construct-typing-0.6.2/construct-stubs/expr.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/lib/__init__.pyi` & `construct-typing-0.6.2/construct-stubs/lib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/lib/binary.pyi` & `construct-typing-0.6.2/construct-stubs/lib/binary.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/lib/bitstream.pyi` & `construct-typing-0.6.2/construct-stubs/lib/bitstream.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/lib/containers.pyi` & `construct-typing-0.6.2/construct-stubs/lib/containers.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct-stubs/lib/py3compat.pyi` & `construct-typing-0.6.2/construct-stubs/lib/py3compat.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct_typed/__init__.py` & `construct-typing-0.6.2/construct_typed/__init__.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct_typed/dataclass_struct.py` & `construct-typing-0.6.2/construct_typed/dataclass_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,23 +149,14 @@
         ...     pixels: bytes = csfield(Bytes(this.height * this.width))
         >>> d = DataclassStruct(Image)
         >>> d.parse(b"\x01\x0212")
         Image(width=1, height=2, pixels=b'12')
     """
 
     subcon: "cs.Struct"
-    if t.TYPE_CHECKING:
-
-        def __new__(
-            cls,
-            dc_type: t.Type[DataclassType],
-            reverse: bool = False,
-        ) -> "DataclassStruct[DataclassType]":
-            ...
-
     def __init__(
         self,
         dc_type: t.Type[DataclassType],
         reverse: bool = False,
     ) -> None:
         if not issubclass(dc_type, DataclassMixin):
             raise TypeError(f"'{repr(dc_type)}' has to be a '{repr(DataclassMixin)}'")
```

### Comparing `construct-typing-0.6.1/construct_typed/generic_wrapper.py` & `construct-typing-0.6.2/construct_typed/generic_wrapper.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/construct_typed/tenum.py` & `construct-typing-0.6.2/construct_typed/tenum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import enum
 import typing as t
 
+from typing_extensions import Self
+
 from .generic_wrapper import *
 
 
 # ## TEnum ############################################################################################################
 class EnumValue:
     """
     This is a helper class for adding documentation to an enum value.
@@ -41,15 +43,15 @@
         >>> State(3)  # missing value
         <State.3: 3>
 
         >>> State.Running.__doc__  # documentation
         'This is the running state.'
     """
 
-    def __new__(cls, val: t.Union[EnumValue, int]) -> "EnumBase":
+    def __new__(cls, val: t.Union[EnumValue, int]) -> "Self":
         if isinstance(val, EnumValue):
             obj = int.__new__(cls, val.value)
             obj._value_ = val.value
             obj.__doc__ = val.__doc__
         else:
             obj = int.__new__(cls, val)
             obj._value_ = val
@@ -85,22 +87,14 @@
 EnumType = t.TypeVar("EnumType", bound=EnumBase)
 
 
 class TEnum(Adapter[int, int, EnumType, EnumType]):
     """
     Typed enum.
     """
-
-    if t.TYPE_CHECKING:
-
-        def __new__(
-            cls, subcon: Construct[int, int], enum_type: t.Type[EnumType]
-        ) -> "TEnum[EnumType]":
-            ...
-
     def __init__(self, subcon: Construct[int, int], enum_type: t.Type[EnumType]):
         if not issubclass(enum_type, EnumBase):
             raise TypeError(
                 "'{}' has to be a '{}'".format(repr(enum_type), repr(EnumBase))
             )
 
         # save enum type
@@ -154,15 +148,15 @@
         >>> Option(4)
         <Option.4: 4>
 
         >>> Option.OptTwo.__doc__  # documentation
         'This is option two.'
     """
 
-    def __new__(cls, val: t.Union[EnumValue, int]) -> "FlagsEnumBase":
+    def __new__(cls, val: t.Union[EnumValue, int]) -> "Self":
         if isinstance(val, EnumValue):
             obj = int.__new__(cls, val.value)
             obj._value_ = val.value
             obj.__doc__ = val.__doc__
         else:
             obj = int.__new__(cls, val)
             obj._value_ = val
@@ -189,22 +183,14 @@
 FlagsEnumType = t.TypeVar("FlagsEnumType", bound=FlagsEnumBase)
 
 
 class TFlagsEnum(Adapter[int, int, FlagsEnumType, FlagsEnumType]):
     """
     Typed enum.
     """
-
-    if t.TYPE_CHECKING:
-
-        def __new__(
-            cls, subcon: Construct[int, int], enum_type: t.Type[FlagsEnumType]
-        ) -> "TFlagsEnum[FlagsEnumType]":
-            ...
-
     def __init__(self, subcon: Construct[int, int], enum_type: t.Type[FlagsEnumType]):
         if not issubclass(enum_type, FlagsEnumBase):
             raise TypeError(
                 "'{}' has to be a '{}'".format(repr(enum_type), repr(FlagsEnumBase))
             )
 
         # save enum type
```

### Comparing `construct-typing-0.6.1/construct_typing.egg-info/PKG-INFO` & `construct-typing-0.6.2/construct_typing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-typing
-Version: 0.6.1
+Version: 0.6.2
 Summary: Extension for the python package 'construct' that adds typing features
 Home-page: https://github.com/timrid/construct-typing
 Author: Tim Riddermann
 License: MIT
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,annotation,type hint,typing,typed,bitstruct,PEP 561
 Platform: POSIX
 Platform: Windows
```

### Comparing `construct-typing-0.6.1/construct_typing.egg-info/SOURCES.txt` & `construct-typing-0.6.2/construct_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `construct-typing-0.6.1/setup.py` & `construct-typing-0.6.2/setup.py`

 * *Files identical despite different names*

