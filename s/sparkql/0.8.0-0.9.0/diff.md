# Comparing `tmp/sparkql-0.8.0.tar.gz` & `tmp/sparkql-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkql-0.8.0.tar", max compression
+gzip compressed data, was "sparkql-0.9.0.tar", max compression
```

## Comparing `sparkql-0.8.0.tar` & `sparkql-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1087 2023-07-30 22:43:49.078621 sparkql-0.8.0/LICENSE
--rw-r--r--   0        0        0    15308 2023-07-30 22:43:49.078621 sparkql-0.8.0/README.md
--rw-r--r--   0        0        0     1443 2023-07-30 22:44:41.414889 sparkql-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      952 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/__init__.py
--rw-r--r--   0        0        0     1218 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/accessors.py
--rw-r--r--   0        0        0     2387 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/exceptions.py
--rw-r--r--   0        0        0      491 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/__init__.py
--rw-r--r--   0        0        0     6065 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/array.py
--rw-r--r--   0        0        0     4165 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/atomic.py
--rw-r--r--   0        0        0    13748 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/base.py
--rw-r--r--   0        0        0    26487 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/struct.py
--rw-r--r--   0        0        0     3692 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/formatters.py
--rw-r--r--   0        0        0      351 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/schema_builder.py
--rw-r--r--   0        0        0     6566 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/schema_merger.py
--rw-r--r--   0        0        0    17131 1970-01-01 00:00:00.000000 sparkql-0.8.0/setup.py
--rw-r--r--   0        0        0    16026 1970-01-01 00:00:00.000000 sparkql-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-08-02 23:47:25.151180 sparkql-0.9.0/LICENSE
+-rw-r--r--   0        0        0    15308 2023-08-02 23:47:25.151180 sparkql-0.9.0/README.md
+-rw-r--r--   0        0        0     1505 2023-08-02 23:48:12.831408 sparkql-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-08-02 23:47:25.151180 sparkql-0.9.0/sparkql/__init__.py
+-rw-r--r--   0        0        0     1239 2023-08-02 23:47:25.151180 sparkql-0.9.0/sparkql/accessors.py
+-rw-r--r--   0        0        0     2387 2023-08-02 23:47:25.151180 sparkql-0.9.0/sparkql/exceptions.py
+-rw-r--r--   0        0        0      491 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/fields/__init__.py
+-rw-r--r--   0        0        0     6120 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/fields/array.py
+-rw-r--r--   0        0        0     4176 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/fields/atomic.py
+-rw-r--r--   0        0        0    13528 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/fields/base.py
+-rw-r--r--   0        0        0    27111 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/fields/struct.py
+-rw-r--r--   0        0        0     3692 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/formatters.py
+-rw-r--r--   0        0        0        0 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/py.typed
+-rw-r--r--   0        0        0      394 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/schema_builder.py
+-rw-r--r--   0        0        0     7287 2023-08-02 23:47:25.155180 sparkql-0.9.0/sparkql/schema_merger.py
+-rw-r--r--   0        0        0    17131 1970-01-01 00:00:00.000000 sparkql-0.9.0/setup.py
+-rw-r--r--   0        0        0    16026 1970-01-01 00:00:00.000000 sparkql-0.9.0/PKG-INFO
```

### Comparing `sparkql-0.8.0/LICENSE` & `sparkql-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkql-0.8.0/README.md` & `sparkql-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sparkql-0.8.0/pyproject.toml` & `sparkql-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkql"
-version = "0.8.0"  # do not edit manually. kept in sync with `tool.commitizen` config via automation
+version = "0.9.0"  # do not edit manually. kept in sync with `tool.commitizen` config via automation
 description = "sparkql: Apache Spark SQL DataFrame schema management for sensible humans"
 authors = ["Matt J Williams <mattjw@mattjw.net>"]
 repository = "https://github.com/mattjw/sparkql"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -13,15 +13,15 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "~7.2"
 invoke = "~2.0"
 black = "~23.1"
 pycodestyle = "~2.10"
 pydocstyle = "~6.3"
-pytype = "2023.2.17"
+mypy = "~1.4.1"
 pylint = "~2.16"
 pytest-spark = "~0.6"
 termcolor = "~2.2.0"
 commitizen = "~2.42.1"
 tomlkit = "~0.11.6"
 pytest-only = "~=2.0.0"
 coverage = {extras = ["toml"], version = "~7.2.1"}
@@ -39,16 +39,21 @@
 debug-auto-git-tag = "tasks:debug_auto_git_tag"
 
 [tool.black]
 line-length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.0"  # do not edit manually. kept in sync with `tool.poetry` config via automation
+version = "0.9.0"  # do not edit manually. kept in sync with `tool.poetry` config via automation
 tag_format = "v$version"
 
 [tool.coverage.run]
 branch = true
 
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:"
+]
+
 [build-system]
 requires = ["poetry>=1.3"]
 build-backend = "poetry.masonry.api"
```

### Comparing `sparkql-0.8.0/sparkql/__init__.py` & `sparkql-0.9.0/sparkql/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.8.0/sparkql/accessors.py` & `sparkql-0.9.0/sparkql/accessors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Accessor functions in order to access field paths, field names, and related field attributes."""
 
-from typing import Sequence
+from typing import Sequence, Dict, Any
 
 from pyspark.sql import Column
 from pyspark.sql.types import StructField
 
 from sparkql.fields.base import BaseField
 
 
@@ -24,15 +24,15 @@
 
 
 def name(field: BaseField) -> str:
     """Return field name of field `field`; an alias of `BaseField.NAME`."""
     return field.NAME
 
 
-def metadata(field: BaseField) -> dict:
+def metadata(field: BaseField) -> Dict[str, Any]:
     """Return field metadata of field `field`; an alias of `BaseField.METADATA`."""
     return field.METADATA
 
 
 def struct_field(field: BaseField) -> StructField:
     """Return the equivalent PySpark StructField of field `field`."""
     return field._spark_struct_field  # pylint: disable=protected-access
```

### Comparing `sparkql-0.8.0/sparkql/exceptions.py` & `sparkql-0.9.0/sparkql/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.8.0/sparkql/fields/array.py` & `sparkql-0.9.0/sparkql/fields/array.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Array field."""
 
 import copy
 from collections.abc import Sequence
-from typing import Optional, Generic, TypeVar, Any, Dict
+from typing import Optional, Generic, TypeVar, Any, Dict, Type, cast, TYPE_CHECKING
 
 from pyspark.sql.types import ArrayType, StructField
 
 from sparkql.exceptions import FieldValueValidationError
 from sparkql.fields.base import BaseField
 
+if TYPE_CHECKING:
+    from sparkql import Struct
+
 
 ArrayElementType = TypeVar("ArrayElementType", bound=BaseField)  # pylint: disable=invalid-name
 
 
 class Array(Generic[ArrayElementType], BaseField):
     """
     Array field; shadows ArrayType in the Spark API.
@@ -20,20 +23,22 @@
     A spark schema generated with this array field will behave as follows:
     - Nullability of the `StructField` is given by `Array.nullable`, as per normal.
     - `containsNull` of the `ArrayType` is given by the nullability of the element contained
       within this field. In other words, `ArrayType.containsNull` is given by
       `Array.element.nullable`.
 
     Attributes:
-        etype: Data type info for the element of this array. Should be an instance of a `BaseField`.
+        e:
+            Data type info for the element of this array. Should be an instance of a `BaseField`.
+            Received in constructor as "element".
     """
 
     __hash__ = BaseField.__hash__
 
-    e: ArrayElementType  # pytype: disable=not-supported-yet  # pylint: disable=invalid-name
+    e: ArrayElementType  # pylint: disable=invalid-name
 
     def __init__(
         self,
         element: ArrayElementType,
         nullable: bool = True,
         name: Optional[str] = None,
         metadata: Optional[Dict[str, Any]] = None,
@@ -49,41 +54,39 @@
             raise ValueError(
                 "When using a field as the element field of an array, the field should not have a name. "
                 f"The field's name resolved to: {element._resolve_field_name()}"
             )
 
         # hand down this array's explicit name to its child element
         # this is to ensure correct naming in path chaining (see `self._replace_parent` and `path_seq`)
-        element = element._replace_explicit_name(name=self._explicit_name)
+        element = cast(ArrayElementType, element._replace_explicit_name(name=self._explicit_name))
         self.e = element  # pylint: disable=invalid-name
 
     #
     # Field path chaining
 
-    def _replace_parent(  # pytype: disable=name-error
-        self, parent: Optional["Struct"] = None  # pytype: disable=invalid-annotation,name-error
-    ) -> "Struct":  # pytype: disable=invalid-annotation,name-error
+    def _replace_parent(self, parent: Optional["Struct"] = None) -> "Array[ArrayElementType]":
         """Return a copy of this array with the parent attribute set."""
         self_copy = copy.copy(self)
         self_copy._parent_struct = parent  # pylint: disable=protected-access
-        self_copy.e = self.e._replace_parent(parent=parent)  # pylint: disable=protected-access
+        self_copy.e = cast(ArrayElementType, self.e._replace_parent(parent=parent))  # pylint: disable=protected-access
         return self_copy
 
     #
     # Field name management
 
-    def _set_contextual_name(self, value: str):
+    def _set_contextual_name(self, value: str) -> None:
         super()._set_contextual_name(value)
         # set child to same name as parent; i.e., propagate contextual name downwards:
         self.e._set_contextual_name(value)  # pylint: disable=protected-access
 
     #
     # Pass through to the element, for users who don't want to use the `.e` field
 
-    def __getattribute__(self, attr_name: str):
+    def __getattribute__(self, attr_name: str) -> Any:
         """Custom get attirubte behaviour."""
         if attr_name.startswith("_"):
             return super().__getattribute__(attr_name)
 
         try:
             attr_value = super().__getattribute__(attr_name)
         except AttributeError:
@@ -94,15 +97,15 @@
 
         return getattr(super().__getattribute__("e"), attr_name)
 
     #
     # Spark type management
 
     @property
-    def _spark_type_class(self):
+    def _spark_type_class(self) -> Type[ArrayType]:
         return ArrayType
 
     @property
     def _spark_struct_field(self) -> StructField:
         """The Spark StructField for this field."""
         # containsNull => is used to indicate if elements in a ArrayType value can have null values
         return StructField(
```

### Comparing `sparkql-0.8.0/sparkql/fields/atomic.py` & `sparkql-0.9.0/sparkql/fields/atomic.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,53 +12,52 @@
     DoubleType,
     FloatType,
     StringType,
     BinaryType,
     BooleanType,
     DateType,
     TimestampType,
-    DataType,
 )
 
 from sparkql.fields.base import AtomicField, IntegralField, FractionalField, _validate_value_type_for_field
 
 
 #
 # DataType -> AtomicType -> NumericType -> IntegralType
 
 
 class Byte(IntegralField):
     """Field for Spark's ByteType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[ByteType]:
         return ByteType
 
 
 class Integer(IntegralField):
     """Field for Spark's IntegerType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[IntegerType]:
         return IntegerType
 
 
 class Long(IntegralField):
     """Field for Spark's LongType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[LongType]:
         return LongType
 
 
 class Short(IntegralField):
     """Field for Spark's ShortType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[ShortType]:
         return ShortType
 
 
 #
 # DataType -> AtomicType -> NumericType -> FractionalType
 
 
@@ -70,43 +69,43 @@
 
     def __init__(self, precision: int = 10, scale: int = 0, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.__precision = precision
         self.__scale = scale
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[DecimalType]:
         return DecimalType
 
     @property
-    def _spark_data_type(self) -> DataType:
+    def _spark_data_type(self) -> DecimalType:
         return DecimalType(self.__precision, self.__scale)
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((decimal.Decimal,), value)
 
 
 class Double(FractionalField):
     """Field for Spark's DoubleType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[DoubleType]:
         return DoubleType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((float,), value)
 
 
 class Float(FractionalField):
     """Field for Spark's FloatType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[FloatType]:
         return FloatType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((float,), value)
 
 
@@ -114,61 +113,61 @@
 # DataType -> AtomicType -> non-numeric types
 
 
 class String(AtomicField):
     """Field for Spark's StringType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[StringType]:
         return StringType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((str,), value)
 
 
 class Binary(AtomicField):
     """Field for Spark's BinaryType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[BinaryType]:
         return BinaryType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((bytearray,), value)
 
 
 class Boolean(AtomicField):
     """Field for Spark's BooleanType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[BooleanType]:
         return BooleanType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((bool,), value)
 
 
 class Date(AtomicField):
     """Field for Spark's DateType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[DateType]:
         return DateType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((date, datetime), value)
 
 
 class Timestamp(AtomicField):
     """Field for Spark's TimestampType."""
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
+    def _spark_type_class(self) -> Type[TimestampType]:
         return TimestampType
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((datetime,), value)
```

### Comparing `sparkql-0.8.0/sparkql/fields/base.py` & `sparkql-0.9.0/sparkql/fields/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Base field and abstract fields."""
 
 from abc import ABC, abstractmethod
-from typing import Optional, Type, Any, Tuple, Sequence, Dict
+from typing import Optional, Type, Any, Tuple, Sequence, Dict, TYPE_CHECKING, cast
 import copy
 
 from pyspark.sql import types as sql_type, Column
 from pyspark.sql import functions as sql_funcs
 from pyspark.sql.types import StructField, DataType
-
 from sparkql.exceptions import FieldNameError, FieldParentError, FieldValueValidationError
 
-
-# pytype: disable=invalid-annotation
+if TYPE_CHECKING:
+    from sparkql import Struct
 
 
-def _validate_value_type_for_field(accepted_types: Tuple[Type, ...], value: Any):
+def _validate_value_type_for_field(accepted_types: Tuple[Type[Any], ...], value: Any) -> None:
     """Raise error if `value` is not compatible with types; None values are always permitted."""
     if value is not None and not isinstance(value, accepted_types):
         pretty_types = " ,".join("'" + accepted_type.__name__ + "'" for accepted_type in accepted_types)
         raise FieldValueValidationError(
             f"Value '{value}' has invalid type '{value.__class__.__name__}'. Allowed types are: {pretty_types}"
         )
 
@@ -37,15 +36,15 @@
     # for convenience only; these will be overwritten.)
     __nullable: bool = True
     __name_explicit: Optional[str] = None
     __name_contextual: Optional[str] = None
     __metadata: Dict[str, Any] = {}  # must be overwritten in constructor
 
     # Placeholder for "protected" style variables. (Again, represented only for convenience.)
-    _parent_struct: Optional["Struct"] = None  # pytype: disable=name-error
+    _parent_struct: Optional["Struct"] = None
 
     def __init__(self, nullable: bool = True, name: Optional[str] = None, metadata: Optional[Dict[str, Any]] = None):
         """
         Constructor for a base field.
 
         Args:
             nullable: Is this field nullable.
@@ -63,26 +62,26 @@
 
     @property
     def _is_nullable(self) -> bool:
         """The nullability status of this field."""
         return self.__nullable
 
     @property
-    def _metadata(self) -> Optional[Dict[str, Any]]:
+    def _metadata(self) -> Dict[str, Any]:
         """The metadata of this field."""
         return self.__metadata
 
     #
     # Field path chaining
 
     @property
-    def _parent(self) -> Optional["Struct"]:  # pytype: disable=name-error
+    def _parent(self) -> Optional["Struct"]:
         return self._parent_struct
 
-    def _replace_parent(self, parent: Optional["Struct"] = None) -> "BaseField":  # pytype: disable=name-error
+    def _replace_parent(self, parent: Optional["Struct"] = None) -> "BaseField":
         """Return a copy of this Field with the parent attribute set."""
         field = copy.copy(self)
         if self._parent_struct is not None:
             raise FieldParentError("Attempted to set parent field that has already been set")
         field._parent_struct = parent  # pylint: disable=protected-access
         return field
 
@@ -106,15 +105,15 @@
     def _explicit_name(self) -> Optional[str]:
         return self.__name_explicit
 
     @property
     def _contextual_name(self) -> Optional[str]:
         return self.__name_contextual
 
-    def _set_contextual_name(self, value: str):
+    def _set_contextual_name(self, value: str) -> None:
         # Intentionally not using an implicit setter here
         if self.__name_contextual is not None:
             raise FieldNameError(
                 "Attempted to override a name that has already been set: "
                 f"'{value}' replacing '{self.__name_contextual}'"
             )
         self.__name_contextual = value
@@ -128,15 +127,15 @@
             raise FieldNameError(
                 "No field name found among: explicit name = {}, inferred name = {}".format(
                     self.__name_explicit, self.__name_contextual
                 )
             )
         return name
 
-    def _resolve_field_name(self, default=None) -> Optional[str]:
+    def _resolve_field_name(self, default: Optional[str] = None) -> Optional[str]:
         """
         Resolve name for this field, or None if no concrete name set.
 
         Should only be used by this class and its subclasses.
         """
         if self.__name_explicit is not None:
             return self.__name_explicit
@@ -151,18 +150,18 @@
     def SEQ(self) -> Sequence[str]:
         """
         The sequence of items that constitute the path to this field.
 
         The result is context-specific and depends on the path to this field through nested structs (if any).
         """
         fields = [self]
-        parent = fields[0]._parent  # pylint: disable=protected-access
+        parent = self._parent  # pylint: disable=protected-access
         while parent is not None:  # pylint: disable=protected-access
-            fields.insert(0, fields[0]._parent)  # pylint: disable=protected-access
-            parent = fields[0]._parent  # pytype: disable=attribute-error  # pylint: disable=protected-access
+            fields.insert(0, parent)
+            parent = parent._parent  # pylint: disable=protected-access
 
         assert all(
             field._resolve_field_name() is not None for field in fields  # pylint: disable=protected-access
         ), f"Encountered an unset name while traversing path. Path is: {_pretty_path(fields)}"
 
         return [f._field_name for f in fields]  # pylint: disable=protected-access
 
@@ -214,17 +213,14 @@
     @abstractmethod
     def _validate_on_value(self, value: Any) -> None:
         """
         Raises an error if `value` is not compatible with this field.
 
         Incompatibility may be due to incorrect nullability or incorrect type.
         """
-        # for acceptable type declarations according to pytype, see pytype source code:
-        #   types.py:1183
-        #   _acceptable_types = {...}
         if not self._is_nullable and value is None:
             msg = "Non-nullable field cannot have None value"
             if self._resolve_field_name() is not None:
                 msg += f" (field name = '{self._resolve_field_name()}')"
             raise FieldValueValidationError(msg)
 
     #
@@ -238,51 +234,51 @@
             isinstance(other, BaseField)
             and self._is_nullable == other._is_nullable
             and self._resolve_field_name() == other._resolve_field_name()  # may be None == None
             and self._spark_type_class == other._spark_type_class
             and self._metadata == other._metadata  # may be None == None
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Returns the name of this field."""
         # stringifying a field as its field adds some convenience for cases where we need the field
         # name
-        return self._resolve_field_name("")
+        return cast(str, self._resolve_field_name(""))
 
-    def _info(self):
+    def _info(self) -> str:
         """String formatted object with a more complete summary of this field, primarily for debugging."""
         return (
             f"<{self.__class__.__name__}\n"
             f"  spark type = {self._spark_type_class.__name__}\n"
             f"  nullable = {self._is_nullable}\n"
             f"  name = {self._resolve_field_name()} <- {[self.__name_explicit, self.__name_contextual]}\n"
             f"  parent = {self._parent}\n"
             f"  metadata = {self._metadata}\n"
             ">"
         )
 
-    def _short_info(self):
+    def _short_info(self) -> str:
         """Short info string for use in error messages."""
         nullable = "Nullable " if self._is_nullable else ""
 
         # Good candidate for python pattern matching once <3.10 support no longer required
         num_metadata_items = len(self.__metadata)
         if num_metadata_items == 0:
             metadata = ""
         elif num_metadata_items == 1:
             metadata = f" [with {num_metadata_items} metadata item]"
         else:
             metadata = f" [with {num_metadata_items} metadata items]"
 
         return f"<{nullable}{self.__class__.__name__}{metadata}: {self._resolve_field_name()}>"
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((self._is_nullable, self._resolve_field_name(""), self._spark_type_class))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self._short_info()
 
 
 class AtomicField(BaseField):
     """
     Atomic field type.
 
@@ -398,11 +394,11 @@
         """The class of the Spark type corresponding to this field."""
 
     @abstractmethod
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
 
 
-def _pretty_path(path: Sequence[BaseField]):
+def _pretty_path(path: Sequence[BaseField]) -> str:
     """Build pretty string of path, for debug and/or error purposes."""
     # pylint: disable=protected-access
     return "< " + " -> ".join(f"'{field._resolve_field_name()}' ({type(field).__name__})" for field in path) + " >"
```

### Comparing `sparkql-0.8.0/sparkql/fields/struct.py` & `sparkql-0.9.0/sparkql/fields/struct.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import dataclasses
 from collections import OrderedDict
 from dataclasses import dataclass
 from difflib import ndiff
 from inspect import isclass
 from typing import ClassVar, Optional, Mapping, Type, Any, Generator, Tuple, MutableMapping, Dict, List
 
-from pyspark.sql import types as sql_types, DataFrame
-from pyspark.sql.types import DataType, StructField, Row
+from pyspark.sql import DataFrame
+from pyspark.sql.types import StructType, StructField, Row
 
 from sparkql.formatters import pretty_schema
 from sparkql.schema_builder import schema as schematise
 from sparkql.exceptions import (
     InvalidStructError,
     StructImplementationError,
     InvalidDataFrameError,
@@ -36,15 +36,15 @@
     """
 
     is_valid: bool
     pretty_struct: str
     pretty_data_frame: str
     report: str = ""
 
-    def raise_on_invalid(self):
+    def raise_on_invalid(self) -> None:
         """
         If the DataFrame did not adhere to the schema, raises an appropriate error.
 
         Raises:
             InvalidDataFrameError if the DataFrame does not pass validation.
         """
         if not self.is_valid:
@@ -54,14 +54,31 @@
 class Struct(BaseField):
     """A struct; shadows StructType in the Spark API."""
 
     __hash__ = BaseField.__hash__
     _struct_metadata: ClassVar[Optional["_StructInnerMetadata"]] = None
 
     @classmethod
+    def _valid_struct_metadata(cls) -> "_StructInnerMetadata":
+        """
+        A wrapper for the `_struct_metadata` class variable, which ensures a non-None return, failing if None.
+
+        Raises:
+            ValueError:
+                If the class's `_struct_metadata` is None, which means its inner metadata has not been set. The
+                noneness of `_struct_metadata` is managed by sparkql under-the-hood. In normal use of sparkql,
+                this should never occur.
+        """
+        # using this method instead of `_struct_metadata` (in appropriate contexts) simplifies type hinting by ensuring
+        # other functions are always dealing with a non-null `_struct_metadata`
+        if cls._struct_metadata is None:
+            raise ValueError(f"Struct class {cls.__name__} has not had its inner metadata extracted")
+        return cls._struct_metadata
+
+    @classmethod
     def validate_data_frame(cls, dframe: DataFrame) -> ValidationResult:
         """
         Validate that the DataFrame `dframe` adheres to the schema of this struct.
 
         Args:
             dframe: DataFrame to be validated.
 
@@ -87,38 +104,38 @@
         )
         return ValidationResult(is_valid, pretty_struct=pretty_struct, pretty_data_frame=pretty_dframe, report=report)
 
     #
     # Handle type management and Spark representations for a Struct object
 
     @property
-    def _spark_type_class(self) -> Type[DataType]:
-        return sql_types.StructType
+    def _spark_type_class(self) -> Type[StructType]:
+        return StructType
 
     @property
     def _spark_struct_field(self) -> StructField:
         """The Spark StructField for this field."""
         return StructField(
             name=self._field_name,
-            dataType=self._struct_metadata.spark_struct,
+            dataType=self._valid_struct_metadata().spark_struct,
             nullable=self._is_nullable,
             metadata=self._metadata,
         )
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         if value is None:
             # super() will have already validate none vs nullability. if None, then it's safe to be none
             return
         if not isinstance(value, Mapping):
             raise FieldValueValidationError(f"Value for a struct must be a mapping, not '{type(value).__name__}'")
 
         dic: Mapping[str, Any] = value
 
-        fields = list(self._struct_metadata.fields.values())
+        fields = list(self._valid_struct_metadata().fields.values())
         field_names = [field._field_name for field in fields]  # pylint: disable=protected-access
         if len(fields) != len(dic):
             raise FieldValueValidationError(
                 f"Dict has incorrect number of fields. \n"
                 f"Struct requires {len(fields)} fields: {', '.join(field_names)} \n"
                 f"Dict has {len(dic)} fields: {', '.join(dic.keys())}"
             )
@@ -133,17 +150,17 @@
         for field in fields:
             field._validate_on_value(dic[field._field_name])  # pylint: disable=protected-access
 
     #
     # Hook in to sub-class creation. Ensure fields are pre-processed when a sub-class is declared
 
     @classmethod
-    def __init_subclass__(cls, **options):  # pylint: disable=unused-argument
+    def __init_subclass__(cls, **options: Any) -> None:  # pylint: disable=unused-argument
         """Hook in to the subclassing of this base class; process fields when sub-classing occurs."""
-        super().__init_subclass__(**options)  # pytype: disable=attribute-error
+        super().__init_subclass__(**options)
 
         # Ensure a subclass does not break any base class functionality
         for child_prop, child_val in cls.__dict__.items():
             if (child_prop in Struct.__dict__) and (isinstance(child_val, BaseField)):
                 raise InvalidStructError(
                     f"Field should not override inherited or reserved class properties: {child_prop}"
                 )
@@ -153,38 +170,38 @@
 
         # Validate the "implements" (if any)
         _Validator(cls).validate()
 
     #
     # Handle dot chaining for full path ref to nested fields
 
-    def __getattribute__(self, attr_name):
+    def __getattribute__(self, attr_name: str) -> Any:
         """
         Customise how field attributes are handled.
 
         Augment the attribute reference chain to ensure that a field's parent is set.
         """
-        attr_value = super().__getattribute__(attr_name)  # pytype: disable=attribute-error
+        attr_value = super().__getattribute__(attr_name)
 
-        if attr_name == "_struct_metadata":
+        if attr_name in {"_struct_metadata", "_valid_struct_metadata"}:
             return attr_value
 
-        resolved_field = self._struct_metadata.resolve_field(
+        resolved_field = self._valid_struct_metadata().resolve_field(
             struct_object=self, attr_name=attr_name, attr_value=attr_value
         )
         if resolved_field is not None:
             return resolved_field
 
         return attr_value
 
     #
     # Makers
 
     @classmethod
-    def make_dict(cls, *args, **kwargs) -> Dict[str, Any]:
+    def make_dict(cls, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """
         Create a data instance of this Struct schema, as a dictionary.
 
         Specify the values for the fields of this struct using args and keyword args, in the same way you would
         specify values in a constructor. Use the struct's property names are keyword arguments. Omitted fields default
         to null.
 
@@ -222,54 +239,54 @@
 
         Returns:
             An instance of this struct, as a dictioniary.
         """
         return _DictMaker(struct_class=cls, positional_args=args, keyword_args=kwargs).make_dict()
 
     @classmethod
-    def make_row(cls, *args, **kwargs) -> Row:
+    def make_row(cls, *args: Any, **kwargs: Any) -> Row:
         """Reserved."""
         # pylint: disable=broad-exception-raised
         raise Exception("Function name reserved.")
 
     #
     # Other methods
 
     def __eq__(self, other: Any) -> bool:
         """True if `self` equals `other`."""
         return (
             super().__eq__(other)
             and isinstance(other, Struct)
-            and self._struct_metadata.fields == other._struct_metadata.fields
-            and list(self._struct_metadata.fields.keys()) == list(other._struct_metadata.fields.keys())
+            and self._valid_struct_metadata().fields == other._valid_struct_metadata().fields
+            and list(self._valid_struct_metadata().fields.keys()) == list(other._valid_struct_metadata().fields.keys())
         )
 
 
 @dataclass(frozen=True)
 class _StructInnerMetadata:
     """Inner metadata object for Struct classes; hides complexity of field handling."""
 
     fields: Mapping[str, BaseField]
     # ^ All fields for the Struct, including both native fields and imported from includes
 
     @staticmethod
-    def from_struct_class(struct_class: Type["Struct"]) -> "_StructInnerMetadata":
+    def from_struct_class(struct_class: Type[Struct]) -> "_StructInnerMetadata":
         """Build instance from a struct class."""
         return _StructInnerMetadata(fields=_FieldsExtractor(struct_class).extract())
 
     @property
-    def spark_struct(self) -> sql_types.StructType:
+    def spark_struct(self) -> StructType:
         """Complete Spark StructType for the sparkql Struct."""
-        return sql_types.StructType(
+        return StructType(
             [field._spark_struct_field for field in self.fields.values()]  # pylint: disable=protected-access
         )
 
     # Resolving of class attributes
     @staticmethod
-    def resolve_field(struct_object: "Struct", attr_name: str, attr_value: Any) -> Optional[BaseField]:
+    def resolve_field(struct_object: Struct, attr_name: str, attr_value: Any) -> Optional[BaseField]:
         """
         Attempt to resolve a `getattribute` call on the Struct, returning a BaseField if applicable.
 
         This should be used to hook into the Struct's `getattribute` behaviour to customise resolution of
         fields. Will also check if the `getattribute` call is attempting to resolve a field. If not, returns None.
 
         Args:
@@ -308,37 +325,37 @@
     - Includes fields: Fields pulled in from `Meta.includes`.
     """
 
     INCLUDES_FIELD_NAME: ClassVar[str] = "includes"
 
     struct_class: Type[Struct]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """Validate input instance variables."""
         _validate_struct_class(self.struct_class)
 
     def extract(self) -> Mapping[str, BaseField]:
         """Extract the fields."""
         # pylint: disable=attribute-defined-outside-init
 
         # Extract and hand native fields
         # native field name -> field
         self._native_fields = OrderedDict(self._yield_native_fields())
         for field_name, field in self._native_fields.items():
             field._set_contextual_name(field_name)  # pylint: disable=protected-access
 
         # Start with super class fields, if any
-        self._fields = OrderedDict(self._get_super_class_fields())
+        self._fields: MutableMapping[str, BaseField] = OrderedDict(self._get_super_class_fields())
 
         # Add native fields
         self._fields = self._safe_combine_fields(self._fields, self._native_fields)
 
         # Add includes fields (if any)
         for included_struct in self._yield_included_structs():
-            incl_fields = included_struct._struct_metadata.fields  # pylint: disable=protected-access
+            incl_fields = included_struct._valid_struct_metadata().fields  # pylint: disable=protected-access
             for incl_field_name, incl_field in incl_fields.items():
                 if incl_field_name not in self._fields:
                     self._fields[incl_field_name] = incl_field  # populate `_fields`
                     # Modify the root struct so that includes fields are available:
                     setattr(self.struct_class, incl_field_name, incl_field)
                 elif self._fields[incl_field_name] != incl_field:
                     raise InvalidStructError(
@@ -347,15 +364,15 @@
                     )
 
         return self._fields
 
     #
     # Extraction and processing of the Struct class
 
-    def _yield_native_fields(self) -> Generator[Tuple[str, Struct], None, None]:
+    def _yield_native_fields(self) -> Generator[Tuple[str, BaseField], None, None]:
         """
         Get the native fields specified for this Struct class, if any.
 
         Yields:
             A `(str, BaseField)` pair for each field found in this class. Each pair consists of the attribute name and
             the field.
         """
@@ -374,24 +391,22 @@
 
         A class specified in `Meta.includes` is converted to an instance of the class before returning.
 
         Yields:
             A Struct object. Note that this is an instance of the Struct, not the class.
             If `Meta` or `Meta.includes` are not provided, no yield.
         """
-        for struct in _yield_structs_from_meta(
-            self.struct_class, self.INCLUDES_FIELD_NAME  # pytype: disable=wrong-arg-types
-        ):
+        for struct in _yield_structs_from_meta(self.struct_class, self.INCLUDES_FIELD_NAME):
             yield struct
 
     #
     # Handle inheritance from super class
 
-    def _get_super_class(self) -> Type:
-        """Obtain super class."""
+    def _get_super_class(self) -> Type[Struct]:
+        """Obtain super class; this will be the Struct class, or a class that is a subclass (/descendant) of Struct."""
         root_class = self.struct_class
 
         assert len(root_class.__mro__) >= 2
         # by definition, the `_FieldsExtractor` will only be invoked when the `root_class` is subclassing Struct, and
         # thus the MRO for the `root_class` will always have at least two elems
 
         return root_class.__mro__[1]
@@ -448,63 +463,57 @@
     Assumes that the inner metadata of the class has been extracted.
     """
 
     IMPLEMENTS_FIELD_NAME: ClassVar[str] = "implements"
 
     struct_class: Type[Struct]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """Validate input instance variables."""
         _validate_struct_class(self.struct_class)
 
-    def validate(self):
+    def validate(self) -> None:
         """
         Validate that the meets "implements" requirements, if specified.
 
         Raises:
             StructImplementationError:
                 If class does not correctly implement any required structs.
         """
         root_struct_metadata: _StructInnerMetadata = (
-            self.struct_class._struct_metadata  # pylint: disable=protected-access
+            self.struct_class._valid_struct_metadata()  # pylint: disable=protected-access
         )
-        if root_struct_metadata is None:
-            raise ValueError(f"Struct class {self.struct_class} has not had its inner metadata extracted")
 
         for required_struct in self._yield_implements_structs():
-            req_fields = (
-                required_struct._struct_metadata.fields  # pylint: disable=protected-access  # pytype: disable=attribute-error
-            )
+            req_fields = required_struct._valid_struct_metadata().fields  # pylint: disable=protected-access
             for req_field_name, req_field in req_fields.items():
-                if req_field_name not in root_struct_metadata.fields:  # pytype: disable=attribute-error
+                if req_field_name not in root_struct_metadata.fields:
                     raise StructImplementationError(
                         f"Struct '{self.struct_class.__name__}' does not implement field '{req_field_name}' "
                         f"required by struct '{type(required_struct).__name__}'"
                     )
-                if req_field != root_struct_metadata.fields[req_field_name]:  # pytype: disable=attribute-error
+                if req_field != root_struct_metadata.fields[req_field_name]:
                     # pylint: disable=protected-access
                     raise StructImplementationError(
-                        f"Struct '{self.struct_class.__name__}' "  # pytype: disable=attribute-error
+                        f"Struct '{self.struct_class.__name__}' "
                         f"implements field '{req_field_name}' "
                         f"(required by struct '{type(required_struct).__name__}') but field is not compatible. "
                         f"Required {req_field._short_info()} "
                         f"but found {root_struct_metadata.fields[req_field_name]._short_info()}"
                     )
 
     def _yield_implements_structs(self) -> Generator[Struct, None, None]:
         """Get the Structs specified in the `Meta.implements`, if any."""
-        for struct in _yield_structs_from_meta(
-            self.struct_class, self.IMPLEMENTS_FIELD_NAME  # pytype: disable=wrong-arg-types
-        ):
+        for struct in _yield_structs_from_meta(self.struct_class, self.IMPLEMENTS_FIELD_NAME):
             yield struct
 
 
-def _get_inner_meta_class(struct_class: Type[Struct]) -> Optional[Type]:
+def _get_inner_meta_class(struct_class: Type[Struct]) -> Optional[Type[Any]]:
     """Retrieve the `Meta` inner class of a Struct class, or None if none is provided."""
-    if not hasattr(struct_class, _META_INNER_CLASS_NAME):  # pytype: disable=wrong-arg-types
+    if not hasattr(struct_class, _META_INNER_CLASS_NAME):
         return None
     inner_meta_class = getattr(struct_class, _META_INNER_CLASS_NAME)
 
     if not isinstance(inner_meta_class, type):
         raise InvalidStructError(
             f"The '{_META_INNER_CLASS_NAME}' "
             "property of a Struct must only be used as an "
@@ -544,60 +553,60 @@
                 "Encountered item in 'includes' list of 'Meta' inner class that is not a Struct or Struct "
                 f"subclass. Item at index {index} is {struct_class}"
             )
 
         yield struct_instance
 
 
-def _validate_struct_class(struct_class: Type):
+def _validate_struct_class(struct_class: Type[Struct]) -> None:
     if not issubclass(struct_class, Struct):
         raise ValueError("'struct_class' must inherit from Struct")
     if struct_class is Struct:
         raise ValueError("'struct_class' must not be Struct")
 
 
 @dataclass
 class _DictMaker:
     """Construct an instance of a Struct, as a dictionary."""
 
     struct_class: Type[Struct]
-    positional_args: Tuple[Any]
+    positional_args: Tuple[Any, ...]
     keyword_args: Dict[str, Any]
 
     # internal state
-    _struct_property_to_field: Dict[str, BaseField] = dataclasses.field(init=False)
+    _struct_property_to_field: Mapping[str, BaseField] = dataclasses.field(init=False)
 
-    _property_to_value: "OrderedDict[str, List[Any]]" = dataclasses.field(init=False)
+    _property_to_value: OrderedDict[str, List[Any]] = dataclasses.field(init=False)
     # ^ store extracted values while we process them. maps property name (i.e., attrib name) to a value.
     #   we'll track if there are any surplus values for the same field
 
     _surplus_positional_values: List[Any] = dataclasses.field(default_factory=list, init=False)
     _surplus_keyword_args: Dict[str, Any] = dataclasses.field(default_factory=dict, init=False)
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         # extract `_struct_metadata.fields` for convenience
-        inner_meta = self.struct_class._struct_metadata  # pylint: disable=protected-access
-        self._struct_property_to_field = inner_meta.fields  # pytype: disable=attribute-error,annotation-type-mismatch
+        inner_meta = self.struct_class._valid_struct_metadata()  # pylint: disable=protected-access
+        self._struct_property_to_field = inner_meta.fields
         self._property_to_value = OrderedDict((property_name, []) for property_name in self._struct_property_to_field)
 
-    def _process_positional_args(self):
+    def _process_positional_args(self) -> None:
         property_to_field = OrderedDict(self._struct_property_to_field)
         args = list(self.positional_args)
         while args:
             arg_value = args.pop(0)
             # determine what field this value is for
             if not property_to_field:
                 # we've run out of struct fields. we have surplus positional args
                 self._surplus_positional_values.append(arg_value)
             else:
                 property_name = next(iter(property_to_field.keys()))
                 property_to_field.pop(property_name)
                 self._property_to_value[property_name].append(arg_value)
 
-    def _process_keyword_args(self):
+    def _process_keyword_args(self) -> None:
         property_to_field = OrderedDict(self._struct_property_to_field)
         kwargs = dict(self.keyword_args)
         while kwargs:
             arg_property_name = next(iter(kwargs.keys()))
             arg_value = kwargs.pop(arg_property_name)
 
             if arg_property_name not in property_to_field:
```

### Comparing `sparkql-0.8.0/sparkql/formatters.py` & `sparkql-0.9.0/sparkql/formatters.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.8.0/sparkql/schema_merger.py` & `sparkql-0.9.0/sparkql/schema_merger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Support for combining Spark schemas."""
 
 from collections import OrderedDict
 from copy import copy
-from typing import Dict, Union, Optional, overload
-
-
-from pyspark.sql.types import StructType, StructField, ArrayType, AtomicType
+from typing import Dict, Union, Optional, overload, get_args, cast
 
+from pyspark.sql.types import StructType, StructField, ArrayType, AtomicType, DataType
 
 MergeableSparkDataType = Union[StructType, ArrayType, AtomicType]
 
 
 @overload
 def merge_schemas(type_a: StructType, type_b: StructType) -> StructType:  # noqa: D103 (pydocstyle missing docstring)
     ...  # pragma: no cover
@@ -50,14 +48,24 @@
     """
     Merge two schemas.
 
     See `merge_schemas` for detailed behaviour description.
     """
 
     @classmethod
+    def __validate_mergeable(cls, data_type: DataType) -> MergeableSparkDataType:
+        if not isinstance(data_type, get_args(MergeableSparkDataType)):
+            raise ValueError(
+                "Data type is not mergeable, expected one of: "
+                f"{[t.__name__ for t in get_args(MergeableSparkDataType)]} "
+                f"but got '{type(data_type).__name__}'"
+            )
+        return cast(MergeableSparkDataType, data_type)
+
+    @classmethod
     def append_to_fields(cls, fields: Dict[str, StructField], field: StructField) -> None:
         """
         Add `field` to `fields`; modifies `fields` as a side-effect.
 
         Args:
             fields: Mapping of field name to field.
             field: Field to be added.
@@ -91,15 +99,19 @@
                         f"metadata of field B is {field_b.metadata}. ",
                         parent_field_name=field_a.name,
                     )
                 )
 
         return StructField(
             name=field_a.name,
-            dataType=cls.merge_types(field_a.dataType, field_b.dataType, parent_field_name=field_a.name),
+            dataType=cls.merge_types(
+                cls.__validate_mergeable(field_a.dataType),
+                cls.__validate_mergeable(field_b.dataType),
+                parent_field_name=field_a.name,
+            ),
             nullable=field_a.nullable,
             metadata={**(field_a.metadata or {}), **(field_b.metadata or {})},
         )
 
     #
     # Merge by type
 
@@ -141,30 +153,34 @@
             cls.append_to_fields(fields, field)
         for field in struct_type_b.fields:
             cls.append_to_fields(fields, field)
 
         return StructType(list(fields.values()))
 
     @classmethod
-    def merge_array_types(cls, array_type_a: ArrayType, array_type_b: ArrayType, parent_field_name) -> ArrayType:
+    def merge_array_types(
+        cls, array_type_a: ArrayType, array_type_b: ArrayType, parent_field_name: Optional[str]
+    ) -> ArrayType:
         assert all(isinstance(obj, ArrayType) for obj in [array_type_a, array_type_b])
 
         if array_type_a.containsNull != array_type_b.containsNull:
             raise ValueError(
                 _validation_error_message(
                     "Arrays must have matching containsNull constraints. "
                     f"containsNull of array A is {array_type_a.containsNull}. "
                     f"containsNull of array B is {array_type_b.containsNull}",
                     parent_field_name=parent_field_name,
                 )
             )
 
         return ArrayType(
             elementType=cls.merge_types(
-                array_type_a.elementType, array_type_b.elementType, parent_field_name=parent_field_name
+                cls.__validate_mergeable(array_type_a.elementType),
+                cls.__validate_mergeable(array_type_b.elementType),
+                parent_field_name=parent_field_name,
             ),
             containsNull=array_type_a.containsNull,
         )
 
 
 def _validation_error_message(message: str, parent_field_name: Optional[str]) -> str:
     if parent_field_name is not None:
```

### Comparing `sparkql-0.8.0/setup.py` & `sparkql-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                      'reformat = tasks:reformat',
                      'test = tasks:test',
                      'typecheck = tasks:typecheck',
                      'verify-all = tasks:verify_all']}
 
 setup_kwargs = {
     'name': 'sparkql',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'sparkql: Apache Spark SQL DataFrame schema management for sensible humans',
     'long_description': '# sparkql ✨\n\n[![PyPI version](https://badge.fury.io/py/sparkql.svg)](https://badge.fury.io/py/sparkql)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/mattjw/sparkql/workflows/CI/badge.svg)](https://github.com/mattjw/sparkql/actions)\n[![codecov](https://codecov.io/gh/mattjw/sparkql/branch/master/graph/badge.svg)](https://codecov.io/gh/mattjw/sparkql)\n\nPython Spark SQL DataFrame schema management for sensible humans.\n\n> _Don\'t sweat it... sparkql it ✨_\n\n## Why use sparkql\n\n`sparkql` takes the pain out of working with DataFrame schemas in PySpark.\nIt makes schema definition more Pythonic. And it\'s\nparticularly useful you\'re dealing with structured data.\n\nIn plain old PySpark, you might find that you write schemas\n[like this](https://github.com/mattjw/sparkql/tree/master/examples/conferences_comparison/plain_schema.py):\n\n```python\nCITY_SCHEMA = StructType()\nCITY_NAME_FIELD = "name"\nCITY_SCHEMA.add(StructField(CITY_NAME_FIELD, StringType(), False))\nCITY_LAT_FIELD = "latitude"\nCITY_SCHEMA.add(StructField(CITY_LAT_FIELD, FloatType()))\nCITY_LONG_FIELD = "longitude"\nCITY_SCHEMA.add(StructField(CITY_LONG_FIELD, FloatType()))\n\nCONFERENCE_SCHEMA = StructType()\nCONF_NAME_FIELD = "name"\nCONFERENCE_SCHEMA.add(StructField(CONF_NAME_FIELD, StringType(), False))\nCONF_CITY_FIELD = "city"\nCONFERENCE_SCHEMA.add(StructField(CONF_CITY_FIELD, CITY_SCHEMA))\n```\n\nAnd then plain old PySpark makes you deal with nested fields like this:\n\n```python\ndframe.withColumn("city_name", df[CONF_CITY_FIELD][CITY_NAME_FIELD])\n```\n\nInstead, with `sparkql`, schemas become a lot\n[more literate](https://github.com/mattjw/sparkql/tree/master/examples/conferences_comparison/sparkql_schema.py):\n\n```python\nclass City(Struct):\n    name = String(nullable=False)\n    latitude = Float()\n    longitude = Float()\n\nclass Conference(Struct):\n    name = String(nullable=False)\n    city = City()\n```\n\nAs does dealing with nested fields:\n\n```python\ndframe.withColumn("city_name", Conference.city.name.COL)\n```\n\nHere\'s a summary of `sparkql`\'s features.\n\n- ORM-like class-based Spark schema definitions.\n- Automated field naming: The attribute name of a field as it appears\n  in its `Struct` is (by default) used as its field name. This name can\n  be optionally overridden.\n- Programatically reference nested fields in your structs with the\n  `PATH` and `COL` special properties. Avoid hand-constructing strings\n  (or `Column`s) to reference your nested fields.\n- Validate that a DataFrame matches a `sparkql` schema.\n- Reuse and build composite schemas with `inheritance`, `includes`, and\n  `implements`.\n- Get a human-readable Spark schema representation with `pretty_schema`.\n- Create an instance of a schema as a dictionary, with validation of\n  the input values.\n\nRead on for documentation on these features.\n\n## Defining a schema\n\nEach Spark atomic type has a counterpart `sparkql` field:\n\n| PySpark type | `sparkql` field |\n|---|---|\n| `ByteType` | `Byte` |\n| `IntegerType` | `Integer` |\n| `LongType` | `Long` |\n| `ShortType` | `Short` |\n| `DecimalType` | `Decimal` |\n| `DoubleType` | `Double` |\n| `FloatType` | `Float` |\n| `StringType` | `String` |\n| `BinaryType` | `Binary` |\n| `BooleanType` | `Boolean` |\n| `DateType` | `Date` |\n| `TimestampType` | `Timestamp` |\n\n`Array` (counterpart to `ArrayType` in PySpark) allows the definition\nof arrays of objects. By creating a subclass of `Struct`, we can\ndefine a custom class that will be converted to a `StructType`.\n\nFor\n[example](https://github.com/mattjw/sparkql/tree/master/examples/arrays/arrays.py),\ngiven the `sparkql` schema definition:\n\n```python\nfrom sparkql import Struct, String, Array\n\nclass Article(Struct):\n    title = String(nullable=False)\n    tags = Array(String(), nullable=False)\n    comments = Array(String(nullable=False))\n```\n\nThen we can build the equivalent PySpark schema (a `StructType`)\nwith:\n\n```python\nfrom sparkql import schema\n\npyspark_struct = schema(Article)\n```\n\nPretty printing the schema with the expression\n`sparkql.pretty_schema(pyspark_struct)` will give the following:\n\n```text\nStructType([\n    StructField(\'title\', StringType(), False),\n    StructField(\'tags\',\n        ArrayType(StringType(), True),\n        False),\n    StructField(\'comments\',\n        ArrayType(StringType(), False),\n        True)])\n```\n\n## Features\n\nMany examples of how to use `sparkql` can be found in\n[`examples`](https://github.com/mattjw/sparkql/tree/master/examples).\n\n### Automated field naming\n\nBy default, field names are inferred from the attribute name in the\nstruct they are declared.\n\nFor example, given the struct\n\n```python\nclass Geolocation(Struct):\n    latitude = Float()\n    longitude = Float()\n```\n\nthe concrete name of the `Geolocation.latitude` field is `latitude`.\n\nNames also be overridden by explicitly specifying the field name as an\nargument to the field\n\n```python\nclass Geolocation(Struct):\n    latitude = Float(name="lat")\n    longitude = Float(name="lon")\n```\n\nwhich would mean the concrete name of the `Geolocation.latitude` field\nis `lat`.\n\n### Field paths and nested objects\n\nReferencing fields in nested data can be a chore. `sparkql` simplifies this\nwith path referencing.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/nested_objects/sparkql_example.py), if we have a\nschema with nested objects:\n\n```python\nclass Address(Struct):\n    post_code = String()\n    city = String()\n\n\nclass User(Struct):\n    username = String(nullable=False)\n    address = Address()\n\n\nclass Comment(Struct):\n    message = String()\n    author = User(nullable=False)\n\n\nclass Article(Struct):\n    title = String(nullable=False)\n    author = User(nullable=False)\n    comments = Array(Comment())\n```\n\nWe can use the special `PATH` property to turn a path into a\nSpark-understandable string:\n\n```python\nauthor_city_str = Article.author.address.city.PATH\n"author.address.city"\n```\n\n`COL` is a counterpart to `PATH` that returns a Spark `Column`\nobject for the path, allowing it to be used in all places where Spark\nrequires a column.\n\nFunction equivalents `path_str`, `path_col`, and `name` are also available.\nThis table demonstrates the equivalence of the property styles and the function\nstyles:\n\n| Property style | Function style | Result (both styles are equivalent) |\n| --- | --- | --- |\n| `Article.author.address.city.PATH` | `sparkql.path_str(Article.author.address.city)` | `"author.address.city"` |\n| `Article.author.address.city.COL` | `sparkql.path_col(Article.author.address.city)` | `Column` pointing to `author.address.city` |\n| `Article.author.address.city.NAME` | `sparkql.name(Article.author.address.city)` | `"city"` |\n\nFor paths that include an array, two approaches are provided:\n\n```python\ncomment_usernames_str = Article.comments.e.author.username.PATH\n"comments.author.username"\n\ncomment_usernames_str = Article.comments.author.username.PATH\n"comments.author.username"\n```\n\nBoth give the same result. However, the former (`e`) is more\ntype-oriented. The `e` attribute corresponds to the array\'s element\nfield. Although this looks strange at first, it has the advantage of\nbeing inspectable by IDEs and other tools, allowing goodness such as\nIDE auto-completion, automated refactoring, and identifying errors\nbefore runtime.\n\n### Field metadata\n\nField [metadata](https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.types.StructField.html) can be specified with the `metadata` argument to a field, which accepts a dictionary\nof key-value pairs.\n\n```python\nclass Article(Struct):\n    title = String(nullable=False,\n                   metadata={"description": "The title of the article", "max_length": 100})\n```\n\nThe metadata can be accessed with the `METADATA` property of the field:\n\n```python\nArticle.title.METADATA\n{"description": "The title of the article", "max_length": 100}\n```\n\n### DataFrame validation\n\nStruct method `validate_data_frame` will verify if a given DataFrame\'s\nschema matches the Struct.\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/validation/test_validation.py),\nif we have our `Article`\nstruct and a DataFrame we want to ensure adheres to the `Article`\nschema:\n\n```python\ndframe = spark_session.createDataFrame([{"title": "abc"}])\n\nclass Article(Struct):\n    title = String()\n    body = String()\n```\n\nThen we can can validate with:\n\n```python\nvalidation_result = Article.validate_data_frame(dframe)\n```\n\n`validation_result.is_valid` indicates whether the DataFrame is valid\n(`False` in this case), and `validation_result.report` is a\nhuman-readable string describing the differences:\n\n```text\nStruct schema...\n\nStructType([\n    StructField(\'title\', StringType(), True),\n    StructField(\'body\', StringType(), True)])\n\nDataFrame schema...\n\nStructType([\n    StructField(\'title\', StringType(), True)])\n\nDiff of struct -> data frame...\n\n  StructType([\n-     StructField(\'title\', StringType(), True)])\n+     StructField(\'title\', StringType(), True),\n+     StructField(\'body\', StringType(), True)])\n```\n\nFor convenience,\n\n```python\nArticle.validate_data_frame(dframe).raise_on_invalid()\n```\n\nwill raise a `InvalidDataFrameError` (see `sparkql.exceptions`) if the  \nDataFrame is not valid.\n\n### Creating an instance of a schema\n\n`sparkql` simplifies the process of creating an instance of a struct.\nYou might need to do this, for example, when creating test data, or\nwhen creating an object (a dict or a row) to return from a UDF.\n\nUse `Struct.make_dict(...)` to instantiate a struct as a dictionary.\nThis has the advantage that the input values will be correctly\nvalidated, and it will convert schema property names into their\nunderlying field names.\n\nFor\n[example](https://github.com/mattjw/sparkql/tree/master/examples/struct_instantiation/instantiate_as_dict.py),\ngiven some simple Structs:\n\n```python\nclass User(Struct):\n    id = Integer(name="user_id", nullable=False)\n    username = String()\n\nclass Article(Struct):\n    id = Integer(name="article_id", nullable=False)\n    title = String()\n    author = User()\n    text = String(name="body")\n```\n\nHere are a few examples of creating dicts from `Article`:\n\n```python\nArticle.make_dict(\n    id=1001,\n    title="The article title",\n    author=User.make_dict(\n        id=440,\n        username="user"\n    ),\n    text="Lorem ipsum article text lorem ipsum."\n)\n\n# generates...\n{\n    "article_id": 1001,\n    "author": {\n        "user_id": 440,\n        "username": "user"},\n    "body": "Lorem ipsum article text lorem ipsum.",\n    "title": "The article title"\n}\n```\n\n```python\nArticle.make_dict(\n    id=1002\n)\n\n# generates...\n{\n    "article_id": 1002,\n    "author": None,\n    "body": None,\n    "title": None\n}\n```\n\nSee\n[this example](https://github.com/mattjw/sparkql/tree/master/examples/conferences_extended/conferences.py)\nfor an extended example of using `make_dict`.\n\n### Composite schemas\n\nIt is sometimes useful to be able to re-use the fields of one struct\nin another struct. `sparkql` provides a few features to enable this:\n\n- _inheritance_: A subclass inherits the fields of a base struct class.\n- _includes_: Incorporate fields from another struct.\n- _implements_: Enforce that a struct must implement the fields of\n  another struct.\n\nSee the following examples for a better explanation.\n\n#### Using inheritance\n\nFor [example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/inheritance.py), the following:\n\n```python\nclass BaseEvent(Struct):\n    correlation_id = String(nullable=False)\n    event_time = Timestamp(nullable=False)\n\nclass RegistrationEvent(BaseEvent):\n    user_id = String(nullable=False)\n```\n\nwill produce the following `RegistrationEvent` schema:\n\n```text\nStructType([\n    StructField(\'correlation_id\', StringType(), False),\n    StructField(\'event_time\', TimestampType(), False),\n    StructField(\'user_id\', StringType(), False)])\n```\n\n#### Using an `includes` declaration\n\nFor [example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/includes.py), the following:\n\n```python\nclass EventMetadata(Struct):\n    correlation_id = String(nullable=False)\n    event_time = Timestamp(nullable=False)\n\nclass RegistrationEvent(Struct):\n    class Meta:\n        includes = [EventMetadata]\n    user_id = String(nullable=False)\n```\n\nwill produce the `RegistrationEvent` schema:\n\n```text\nStructType(List(\n    StructField(\'user_id\', StringType(), False),\n    StructField(\'correlation_id\', StringType(), False),\n    StructField(\'event_time\', TimestampType(), False)))\n```\n\n#### Using an `implements` declaration\n\n`implements` is similar to `includes`, but does not automatically\nincorporate the fields of specified structs. Instead, it is up to\nthe implementor to ensure that the required fields are declared in\nthe struct.\n\nFailing to implement a field from an `implements` struct will result in\na `StructImplementationError` error.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/implements.py):\n\n```\nclass LogEntryMetadata(Struct):\n    logged_at = Timestamp(nullable=False)\n\nclass PageViewLogEntry(Struct):\n    class Meta:\n        implements = [LogEntryMetadata]\n    page_id = String(nullable=False)\n\n# the above class declaration will fail with the following StructImplementationError error:\n#   Struct \'PageViewLogEntry\' does not implement field \'logged_at\' required by struct \'LogEntryMetadata\'\n```\n\n\n### Prettified Spark schema strings\n\nSpark\'s stringified schema representation isn\'t very user-friendly, particularly for large schemas:\n\n\n```text\nStructType([StructField(\'name\', StringType(), False), StructField(\'city\', StructType([StructField(\'name\', StringType(), False), StructField(\'latitude\', FloatType(), True), StructField(\'longitude\', FloatType(), True)]), True)])\n```\n\nThe function `pretty_schema` will return something more useful:\n\n```text\nStructType([\n    StructField(\'name\', StringType(), False),\n    StructField(\'city\',\n        StructType([\n            StructField(\'name\', StringType(), False),\n            StructField(\'latitude\', FloatType(), True),\n            StructField(\'longitude\', FloatType(), True)]),\n        True)])\n```\n\n### Merge two Spark `StructType` types\n\nIt can be useful to build a composite schema from two `StructType`s. sparkql provides a\n`merge_schemas` function to do this.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/merge_struct_types/merge_struct_types.py):\n\n```python\nschema_a = StructType([\n    StructField("message", StringType()),\n    StructField("author", ArrayType(\n        StructType([\n            StructField("name", StringType())\n        ])\n    ))\n])\n\nschema_b = StructType([\n    StructField("author", ArrayType(\n        StructType([\n            StructField("address", StringType())\n        ])\n    ))\n])\n\nmerged_schema = merge_schemas(schema_a, schema_b) \n```\n\nresults in a `merged_schema` that looks like:\n\n```text\nStructType([\n    StructField(\'message\', StringType(), True),\n    StructField(\'author\',\n        ArrayType(StructType([\n            StructField(\'name\', StringType(), True),\n            StructField(\'address\', StringType(), True)]), True),\n        True)])\n```\n\n## Contributing\n\nContributions are very welcome. Developers who\'d like to contribute to\nthis project should refer to [CONTRIBUTING.md](./CONTRIBUTING.md).\n',
     'author': 'Matt J Williams',
     'author_email': 'mattjw@mattjw.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mattjw/sparkql',
```

### Comparing `sparkql-0.8.0/PKG-INFO` & `sparkql-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkql
-Version: 0.8.0
+Version: 0.9.0
 Summary: sparkql: Apache Spark SQL DataFrame schema management for sensible humans
 Home-page: https://github.com/mattjw/sparkql
 License: MIT
 Author: Matt J Williams
 Author-email: mattjw@mattjw.net
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

