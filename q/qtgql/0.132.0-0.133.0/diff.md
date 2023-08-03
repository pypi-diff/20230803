# Comparing `tmp/qtgql-0.132.0.tar.gz` & `tmp/qtgql-0.133.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.132.0.tar", max compression
+gzip compressed data, was "qtgql-0.133.0.tar", max compression
```

## Comparing `qtgql-0.132.0.tar` & `qtgql-0.133.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-08-02 09:01:23.572032 qtgql-0.132.0/LICENSE
--rw-r--r--   0        0        0     1116 2023-08-02 09:01:23.572032 qtgql-0.132.0/README.md
--rw-r--r--   0        0        0     4337 2023-08-02 09:01:50.788511 qtgql-0.132.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-08-02 09:01:51.568527 qtgql-0.132.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     2116 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1708 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3454 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1216 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3855 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3877 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    16161 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0     4441 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/selections_injection.py
--rw-r--r--   0        0        0      864 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0     2208 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/utils.py
--rw-r--r--   0        0        0        0 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     5521 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0     2019 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4247 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     3013 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1137 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     5565 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4207 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5264 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     6471 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18970 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1753 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.132.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 07:57:01.286965 qtgql-0.133.0/LICENSE
+-rw-r--r--   0        0        0     1116 2023-08-03 07:57:01.286965 qtgql-0.133.0/README.md
+-rw-r--r--   0        0        0     4337 2023-08-03 07:57:34.277369 qtgql-0.133.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-08-03 07:57:35.169424 qtgql-0.133.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     2116 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1708 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3454 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1216 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3855 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16194 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4441 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2208 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     5521 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8761 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0     2019 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4238 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     3013 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1137 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     5635 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4207 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5264 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     6819 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    19611 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1753 2023-08-03 07:57:01.302965 qtgql-0.133.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.133.0/PKG-INFO
```

### Comparing `qtgql-0.132.0/LICENSE` & `qtgql-0.133.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/README.md` & `qtgql-0.133.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/pyproject.toml` & `qtgql-0.133.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.132.0"
+version = "0.133.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/cli.py` & `qtgql-0.133.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/config.py` & `qtgql-0.133.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.133.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.133.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/core/template.py` & `qtgql-0.133.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/generator.py` & `qtgql-0.133.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.133.0/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.133.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from qtgqlcodegen.operation.utils import unwrap_frag_spreads
 from qtgqlcodegen.schema.definitions import (
     QtGqlFieldDefinition,
     QtGqlVariableDefinition,
     SchemaTypeInfo,
 )
 from qtgqlcodegen.types import (
+    QtGqlInputList,
     QtGqlInterface,
     QtGqlList,
     QtGqlOptional,
     QtGqlQueriedInterface,
     QtGqlQueriedObjectType,
     QtGqlQueriedUnion,
     QtGqlUnion,
@@ -76,15 +77,15 @@
     ret: QtGqlTypeABC | None = None
     is_optional: bool = True
     if non_null := is_nonnull_node(node):
         node = non_null.type
         is_optional = False
 
     if list_node := is_list_node(node):
-        ret = QtGqlList(
+        ret = QtGqlInputList(
             of_type=_evaluate_variable_node_type(type_info, list_node.type),
         )
 
     elif named_type := is_named_type_node(node):
         ret = type_info.get_type(named_type.name.value)
 
     if not ret:  # pragma: no cover
@@ -108,28 +109,38 @@
 def _evaluate_selection_set_type(
     type_info: OperationTypeInfo,
     concrete_type: QtGqlTypeABC,
     selection_set_node: SelectionsSet | None,
     path: str,
 ) -> QtGqlTypeABC:
     ret: QtGqlTypeABC | None = None
-    if obj_type := concrete_type.is_object_type:
-        ret = _evaluate_object_type(
+    if lst := concrete_type.is_model:
+        ret = _evaluate_list(
             type_info=type_info,
-            concrete=obj_type,
+            concrete=lst,
             selection_set=selection_set_node,
             path=path,
         )
-    elif lst := concrete_type.is_model:
-        ret = _evaluate_list(
+    elif not selection_set_node:
+        # these types have no selections
+        assert (
+            concrete_type.is_builtin_scalar
+            or concrete_type.is_custom_scalar
+            or concrete_type.is_enum
+        )
+        ret = concrete_type  # currently there is no need for a "proxied" type.
+
+    elif obj_type := concrete_type.is_object_type:
+        ret = _evaluate_object_type(
             type_info=type_info,
-            concrete=lst,
+            concrete=obj_type,
             selection_set=selection_set_node,
             path=path,
         )
+
     elif interface := concrete_type.is_interface:
         ret = _evaluate_interface(
             type_info=type_info,
             concrete=interface,
             selection_set=selection_set_node,
             path=path,
         )
@@ -137,23 +148,14 @@
         ret = _evaluate_union(
             type_info=type_info,
             concrete=is_union,
             selection_set=selection_set_node,
             path=path,
         )
 
-    elif not selection_set_node:
-        # these types have no selections
-        assert (
-            concrete_type.is_builtin_scalar
-            or concrete_type.is_custom_scalar
-            or concrete_type.is_enum
-        )
-        ret = concrete_type  # currently there is no need for a "proxied" type.
-
     if not ret:  # pragma: no cover
         raise NotImplementedError(f"type {concrete_type} not supported yet")
 
     if concrete_type.is_optional:
         return QtGqlOptional(of_type=ret)
     return ret
 
@@ -180,15 +182,15 @@
         type_info=type_info,
     )
 
 
 def _evaluate_list(
     type_info: OperationTypeInfo,
     concrete: QtGqlList,
-    selection_set: SelectionsSet,
+    selection_set: SelectionsSet | None,
     path: str,
 ) -> QtGqlList:
     return QtGqlList(
         of_type=_evaluate_selection_set_type(
             type_info,
             concrete_type=concrete.of_type,
             selection_set_node=selection_set,
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/operation/selections_injection.py` & `qtgql-0.133.0/qtgqlcodegen/operation/selections_injection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/operation/template.py` & `qtgql-0.133.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/operation/utils.py` & `qtgql-0.133.0/qtgqlcodegen/operation/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.133.0/qtgqlcodegen/schema/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     @cached_property
     def arguments(self) -> tuple[QtGqlArgumentDefinition, ...]:
         return tuple(self.arguments_dict.values())
 
     @cached_property
     def arguments_type(self) -> str:
-        return "std::tuple<" + ",".join([arg.type.type_name() for arg in self.arguments]) + ">"
+        return "std::tuple<" + ",".join([arg.type.member_type for arg in self.arguments]) + ">"
 
     def index_for_argument(self, arg: str) -> int:
         return self.arguments.index(self.arguments_dict[arg])
 
     @cached_property
     def getter_name(self) -> str:
         return f"get_{self.name}"
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.133.0/qtgqlcodegen/schema/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SchemaTypeInfo,
 )
 from qtgqlcodegen.types import (
     BuiltinScalars,
     EnumValue,
     QtGqlDeferredType,
     QtGqlEnumDefinition,
+    QtGqlInputList,
     QtGqlInputObjectTypeDefinition,
     QtGqlInterface,
     QtGqlList,
     QtGqlObjectType,
     QtGqlOptional,
     QtGqlTypeABC,
     QtGqlUnion,
@@ -54,28 +55,34 @@
         type_info.input_objects[ret.name] = ret
     return ret
 
 
 def evaluate_graphql_type(
     type_info: SchemaTypeInfo,
     t: gql_def.GraphQLType,
+    is_input: bool = False,
 ) -> QtGqlTypeABC:
     # even though every type in qtgql has a default constructor,
     # hence there is no "real" non-null values
     # we store it as optional for generating nullable checks only for what's required.
     ret: QtGqlTypeABC | None = None
     is_optional = True
     if non_null := is_non_null_definition(t):
         t = non_null.of_type
         is_optional = False
 
     if list_def := is_list_definition(t):
-        ret = QtGqlList(
-            of_type=evaluate_graphql_type(type_info, list_def.of_type),
-        )
+        if is_input:
+            ret = QtGqlInputList(
+                of_type=evaluate_graphql_type(type_info, list_def.of_type, is_input=True),
+            )
+        else:
+            ret = QtGqlList(
+                of_type=evaluate_graphql_type(type_info, list_def.of_type),
+            )
     elif scalar_def := is_scalar_definition(t):
         if builtin_scalar := BuiltinScalars.by_graphql_name(scalar_def.name):
             ret = builtin_scalar
         else:
             ret = type_info.custom_scalars[scalar_def.name]
 
     elif enum_def := is_enum_definition(t):
@@ -128,15 +135,15 @@
 
 def _evaluate_argument_field(
     type_info: SchemaTypeInfo,
     name: str,
     field: gql_def.GraphQLInputField | gql_def.GraphQLArgument,
 ) -> QtGqlArgumentDefinition:
     return QtGqlArgumentDefinition(
-        type=evaluate_graphql_type(type_info, field.type),
+        type=evaluate_graphql_type(type_info, field.type, is_input=True),
         name=name,
         description=field.description,
     )
 
 
 class InterfaceOrObjectOptions(NamedTuple):
     implements: tuple[QtGqlInterface, ...]
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/schema/template.py` & `qtgql-0.133.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake` & `qtgql-0.133.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         👉proxy_field.name👈_init_vec.push_back(node.👉 proxy_field.type.of_type.from_json_convertor 👈);
     }
     👉 setter_name 👈(std::make_shared<👉proxy_field.concrete.type.type_name()👈>(nullptr, 👉proxy_field.name👈_init_vec) 👉 setter_end 👈);
     {% else %}
         👉proxy_field.concrete.type.member_type👈 👉proxy_field.name👈_init_vec;
         for (const auto& node: data.value("👉proxy_field.name👈").toArray()){
         {% if proxy_field.type.is_model.of_type.is_queried_object_type %}
-            👉proxy_field.name👈_init_vec.push_back(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
+            👉proxy_field.name👈_init_vec.push_back(👉 proxy_field.type.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
         {% elif proxy_field.type.is_model.of_type.is_queried_union or proxy_field.type.is_model.of_type.is_queried_interface %}
             auto node_data = node.toObject();
             auto 👉proxy_field.name👈_typename = node_data.value("__typename").toString();
             {%set type_cond -%}👉proxy_field.name👈_typename{% endset -%}
             {% for choice in proxy_field.type.of_type.choices -%}
             {% set do_on_meets -%}
             👉proxy_field.name👈_init_vec.push_back(👉choice.deserializer_name👈(node_data, 👉operation_pointer👈) 👉 setter_end 👈);
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 {% set setter_end -%}
 {% if proxy_field.variable_uses -%}
 , 👉private_name👈_args
 {% endif -%}
 {%- endset -%}
 {%- set setter_name -%}inst->👉 proxy_field.concrete.setter_name 👈{% endset -%}
 
-{%- if proxy_field.is_root and f_concrete.type.is_object_type or f_concrete.type.is_interface or f_concrete.type.is_union -%}
+{%- if proxy_field.is_root and (f_concrete.type.is_object_type or f_concrete.type.is_interface or f_concrete.type.is_union
+or (f_concrete.type.is_model and f_concrete.type.needs_proxy_model)) -%}
 {#- // root fields that has no default value might not have value even if they are not optional -#}
 {% if proxy_field.variable_uses  -%}
 if (!inst->👉private_name👈.contains(👉private_name👈_args))
 {% else -%}
 if (!👉current👈)
 {% endif %}
 {
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.133.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.133.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -72,15 +72,23 @@
 {% for var in context.operation.variables -%}
 std::optional<👉 var.type.member_type 👈> 👉 var.name 👈 = {};
 {% endfor -%}
     QJsonObject to_json() const{
     QJsonObject __ret;
     {% for var in context.operation.variables -%}
     if (👉 var.name 👈.has_value()){
-    __ret.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
+    {% if var.type.is_input_list -%}
+        QJsonArray 👉 var.name 👈_json;
+        for (const auto& node: 👉 var.name 👈.value()){
+            👉 var.name 👈_json.append(👉 var.type.of_type.json_repr("node") 👈);
+        }
+        __ret.insert("👉 var.name 👈",  👉 var.name 👈_json);
+    {% else -%}
+        __ret.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
+    {% endif -%}
     }
     {% endfor -%}
     return __ret;
     }
 };
 
 class 👉 context.operation.name 👈: public qtgql::bases::OperationHandlerABC{
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.133.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/qtgqlcodegen/types.py` & `qtgql-0.133.0/qtgqlcodegen/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         return None
 
     @property
     def is_model(self) -> QtGqlList | None:
         return None
 
     @property
+    def is_input_list(self) -> QtGqlInputList | None:
+        return None
+
+    @property
     def is_enum(self) -> QtGqlEnumDefinition | None:
         return None
 
     @property
     def is_builtin_scalar(self) -> BuiltinScalar | None:
         return None
 
@@ -152,14 +156,25 @@
     of_type: QtGqlTypeABC
 
     @property
     def is_model(self) -> QtGqlList | None:
         return self
 
     @property
+    def needs_proxy_model(self) -> bool:
+        """Model of scalars / enums.
+
+        have no further selections hence they are shared across the
+        schema.
+        """
+        if self.of_type.is_builtin_scalar or self.of_type.is_enum:
+            return True
+        return False
+
+    @property
     def member_type(self) -> str:
         if self.of_type.is_builtin_scalar:
             # scalars has no underlying fields hence they don't need to be
             # proxied. So each proxy would get an instance to the model.
             return f"std::shared_ptr<{self.type_name()}>"
 
         return f"std::vector<{self.of_type.member_type}>"
@@ -179,14 +194,26 @@
             return f"{QtGqlTypes.ListModelABC.name}<{self.of_type.property_type}> *"
         if bs := self.of_type.is_builtin_scalar:
             return f"{QtGqlTypes.ListModelABC.name}<{bs.member_type}> *"
         raise NotImplementedError
 
 
 @define
+class QtGqlInputList(QtGqlTypeABC):
+    of_type: QtGqlTypeABC
+
+    @property
+    def is_input_list(self) -> QtGqlInputList | None:
+        return self
+
+    def type_name(self) -> str:
+        return f"std::list<{self.of_type.type_name()}>"
+
+
+@define
 class QtGqlUnion(QtGqlTypeABC):
     types: tuple[QtGqlObjectType | QtGqlDeferredType, ...]
 
     @property
     def is_union(self) -> QtGqlUnion | None:
         return self
```

### Comparing `qtgql-0.132.0/qtgqlcodegen/utils.py` & `qtgql-0.133.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.132.0/PKG-INFO` & `qtgql-0.133.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.132.0
+Version: 0.133.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
```

