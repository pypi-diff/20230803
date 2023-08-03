# Comparing `tmp/qtgql-0.131.0.tar.gz` & `tmp/qtgql-0.132.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.131.0.tar", max compression
+gzip compressed data, was "qtgql-0.132.0.tar", max compression
```

## Comparing `qtgql-0.131.0.tar` & `qtgql-0.132.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-07-31 06:39:39.488650 qtgql-0.131.0/LICENSE
--rw-r--r--   0        0        0     1116 2023-07-31 06:39:39.488650 qtgql-0.131.0/README.md
--rw-r--r--   0        0        0     4337 2023-07-31 06:40:14.224894 qtgql-0.131.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-07-31 06:40:15.164901 qtgql-0.131.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     2116 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3393 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1216 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3855 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3877 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    16149 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0     4441 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/selections_injection.py
--rw-r--r--   0        0        0      864 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0     2208 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/utils.py
--rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4600 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0     2019 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3629 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2985 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1137 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4791 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4164 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5052 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     6471 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18386 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1579 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.131.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 09:01:23.572032 qtgql-0.132.0/LICENSE
+-rw-r--r--   0        0        0     1116 2023-08-02 09:01:23.572032 qtgql-0.132.0/README.md
+-rw-r--r--   0        0        0     4337 2023-08-02 09:01:50.788511 qtgql-0.132.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-08-02 09:01:51.568527 qtgql-0.132.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     2116 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1708 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3454 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1216 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3855 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-08-02 09:01:23.580032 qtgql-0.132.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16161 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4441 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2208 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     5521 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0     2019 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4247 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     3013 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1137 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     5565 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4207 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5264 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     6471 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18970 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1753 2023-08-02 09:01:23.584032 qtgql-0.132.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.132.0/PKG-INFO
```

### Comparing `qtgql-0.131.0/LICENSE` & `qtgql-0.132.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/README.md` & `qtgql-0.132.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/pyproject.toml` & `qtgql-0.132.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.131.0"
+version = "0.132.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/cli.py` & `qtgql-0.132.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/config.py` & `qtgql-0.132.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.132.0/qtgqlcodegen/core/cppref.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,10 +60,10 @@
 
 
 def QtGqlBasesNs() -> CppAttribute:
     return QtGqlNs().ns_add("bases")
 
 
 class QtGqlTypes:
-    QGraphQLList = QtGqlBasesNs().ns_add("ListModelABC")
+    ListModelABC = QtGqlBasesNs().ns_add("ListModelABC")
     NodeInterfaceABC = QtGqlBasesNs().ns_add("NodeInterfaceABC")
     ObjectTypeABC = QtGqlBasesNs().ns_add("ObjectTypeABC")
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.132.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 is_inline_fragment = ast_identifier_factory(gql_lang.InlineFragmentNode)
 is_fragment_spread_node = ast_identifier_factory(gql_lang.FragmentSpreadNode)
 is_fragment_definition_node = ast_identifier_factory(gql_def.FragmentDefinitionNode)
 is_operation_def_node = ast_identifier_factory(gql_def.OperationDefinitionNode)
 is_field_node = ast_identifier_factory(gql_def.FieldNode)
 is_nonnull_node = ast_identifier_factory(gql_lang.NonNullTypeNode)
 is_named_type_node = ast_identifier_factory(gql_lang.NamedTypeNode)
+is_list_node = ast_identifier_factory(gql_lang.ListTypeNode)
 
 
 T_Definition = TypeVar("T_Definition", bound=gql_def.GraphQLType)
 
 
 def definition_identifier_factory(
     expected: type[T_Definition],
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/core/template.py` & `qtgql-0.132.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/generator.py` & `qtgql-0.132.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.132.0/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.132.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from graphql.language import visitor
 
 from qtgqlcodegen.core.graphql_ref import (
     SelectionsSet,
     is_field_node,
     is_fragment_definition_node,
     is_inline_fragment,
+    is_list_node,
     is_named_type_node,
     is_nonnull_node,
     is_operation_def_node,
 )
 from qtgqlcodegen.operation.definitions import (
     OperationTypeInfo,
     QtGqlOperationDefinition,
@@ -24,15 +25,14 @@
 from qtgqlcodegen.operation.selections_injection import inject_required_selections
 from qtgqlcodegen.operation.utils import unwrap_frag_spreads
 from qtgqlcodegen.schema.definitions import (
     QtGqlFieldDefinition,
     QtGqlVariableDefinition,
     SchemaTypeInfo,
 )
-from qtgqlcodegen.schema.evaluation import evaluate_graphql_type
 from qtgqlcodegen.types import (
     QtGqlInterface,
     QtGqlList,
     QtGqlOptional,
     QtGqlQueriedInterface,
     QtGqlQueriedObjectType,
     QtGqlQueriedUnion,
@@ -69,27 +69,34 @@
     return sorted(ret, key=lambda v: v.argument[0])
 
 
 def _evaluate_variable_node_type(
     type_info: SchemaTypeInfo,
     node: graphql.TypeNode,
 ) -> QtGqlTypeABC:
-    if nonnull := is_nonnull_node(node):
-        return evaluate_graphql_type(
-            type_info,
-            graphql.type.GraphQLNonNull(
-                type_info.schema_definition.get_type(nonnull.type.name.value),  # type: ignore
-            ),
+    ret: QtGqlTypeABC | None = None
+    is_optional: bool = True
+    if non_null := is_nonnull_node(node):
+        node = non_null.type
+        is_optional = False
+
+    if list_node := is_list_node(node):
+        ret = QtGqlList(
+            of_type=_evaluate_variable_node_type(type_info, list_node.type),
         )
 
-    if named_type := is_named_type_node(node):
-        gql_concrete = type_info.schema_definition.get_type(named_type.name.value)
-        assert gql_concrete
-        return evaluate_graphql_type(type_info, gql_concrete)
-    raise NotImplementedError(node, "Type is not supported as a variable ATM")
+    elif named_type := is_named_type_node(node):
+        ret = type_info.get_type(named_type.name.value)
+
+    if not ret:  # pragma: no cover
+        raise NotImplementedError(node, "Type is not supported as a variable ATM")
+
+    if is_optional:
+        return QtGqlOptional(of_type=ret)
+    return ret
 
 
 def _evaluate_variable(
     type_info: SchemaTypeInfo,
     var: gql_lang.VariableDefinitionNode,
 ) -> QtGqlVariableDefinition:
     return QtGqlVariableDefinition(
@@ -101,24 +108,15 @@
 def _evaluate_selection_set_type(
     type_info: OperationTypeInfo,
     concrete_type: QtGqlTypeABC,
     selection_set_node: SelectionsSet | None,
     path: str,
 ) -> QtGqlTypeABC:
     ret: QtGqlTypeABC | None = None
-    if not selection_set_node:
-        # these types have no selections
-        assert (
-            concrete_type.is_builtin_scalar
-            or concrete_type.is_custom_scalar
-            or concrete_type.is_enum
-        )
-        ret = concrete_type  # currently there is no need for a "proxied" type.
-
-    elif obj_type := concrete_type.is_object_type:
+    if obj_type := concrete_type.is_object_type:
         ret = _evaluate_object_type(
             type_info=type_info,
             concrete=obj_type,
             selection_set=selection_set_node,
             path=path,
         )
     elif lst := concrete_type.is_model:
@@ -138,14 +136,24 @@
     elif is_union := concrete_type.is_union:
         ret = _evaluate_union(
             type_info=type_info,
             concrete=is_union,
             selection_set=selection_set_node,
             path=path,
         )
+
+    elif not selection_set_node:
+        # these types have no selections
+        assert (
+            concrete_type.is_builtin_scalar
+            or concrete_type.is_custom_scalar
+            or concrete_type.is_enum
+        )
+        ret = concrete_type  # currently there is no need for a "proxied" type.
+
     if not ret:  # pragma: no cover
         raise NotImplementedError(f"type {concrete_type} not supported yet")
 
     if concrete_type.is_optional:
         return QtGqlOptional(of_type=ret)
     return ret
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/operation/selections_injection.py` & `qtgql-0.132.0/qtgqlcodegen/operation/selections_injection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/operation/template.py` & `qtgql-0.132.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/operation/utils.py` & `qtgql-0.132.0/qtgqlcodegen/operation/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.132.0/qtgqlcodegen/schema/definitions.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 from attr import Factory, define
 from graphql import OperationType
 
-from qtgqlcodegen.utils import require
+from qtgqlcodegen.types import BuiltinScalars
+from qtgqlcodegen.utils import cached_method, require
 
 if TYPE_CHECKING:
     from graphql.type import definition as gql_def
     from typing_extensions import TypeAlias
 
     from qtgqlcodegen.types import (
         CustomScalarDefinition,
@@ -125,14 +126,38 @@
 
     def get_object_type(self, name: str) -> QtGqlObjectType | None:
         return self.object_types.get(name, None)
 
     def get_object_or_interface(self, name: str) -> QtGqlInterface | QtGqlObjectType:
         return require(self.get_object_type(name) or self.get_interface(name))
 
+    def get_enum(self, name: str) -> QtGqlEnumDefinition | None:
+        return self.enums.get(name, None)
+
+    def get_input_type(self, name: str) -> QtGqlInputObjectTypeDefinition | None:
+        return self.input_objects.get(name, None)
+
+    def get_custom_scalar(self, name: str) -> CustomScalarDefinition | None:
+        return self.custom_scalars.get(name, None)
+
+    @cached_method()
+    def get_type(self, name: str) -> QtGqlTypeABC:
+        """
+        :param name: Any type name
+        :return: Scalar / Input / Object / Interface based on that name
+        """
+        return require(
+            BuiltinScalars.by_graphql_name(name)
+            or self.get_object_type(name)
+            or self.get_interface(name)
+            or self.get_enum(name)
+            or self.get_input_type(name)
+            or self.get_custom_scalar(name),
+        )
+
     def add_objecttype(self, objecttype: QtGqlObjectType) -> None:
         self.object_types[objecttype.name] = objecttype
 
     @cached_property
     def root_types(self) -> list[gql_def.GraphQLObjectType | None]:
         return [
             self.schema_definition.get_root_type(OperationType.QUERY),
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.132.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/schema/template.py` & `qtgql-0.132.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake` & `qtgql-0.132.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -18,33 +18,41 @@
 {% for choice in proxy_field.type.choices -%}
 {% set do_on_meets -%}
 👉 setter_name 👈(👉choice.deserializer_name👈(👉proxy_field.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
 {% elif proxy_field.type.is_model -%}
-    👉proxy_field.concrete.type.member_type👈 👉proxy_field.name👈_init_list;
+    {% if proxy_field.type.of_type.is_builtin_scalar %}
+    std::vector<👉proxy_field.type.of_type.type_name()👈> 👉proxy_field.name👈_init_vec;
     for (const auto& node: data.value("👉proxy_field.name👈").toArray()){
-    {% if proxy_field.type.is_model.of_type.is_queried_object_type %}
-        👉proxy_field.name👈_init_list.append(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
-    {% elif proxy_field.type.is_model.of_type.is_queried_union or proxy_field.type.is_model.of_type.is_queried_interface %}
-        auto node_data = node.toObject();
-        auto 👉proxy_field.name👈_typename = node_data.value("__typename").toString();
-        {%set type_cond -%}👉proxy_field.name👈_typename{% endset -%}
-        {% for choice in proxy_field.type.of_type.choices -%}
-        {% set do_on_meets -%}
-        👉proxy_field.name👈_init_list.append(👉choice.deserializer_name👈(node_data, 👉operation_pointer👈) 👉 setter_end 👈);
-        {% endset -%}
-        👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
-        {% endfor %}
+        👉proxy_field.name👈_init_vec.push_back(node.👉 proxy_field.type.of_type.from_json_convertor 👈);
+    }
+    👉 setter_name 👈(std::make_shared<👉proxy_field.concrete.type.type_name()👈>(nullptr, 👉proxy_field.name👈_init_vec) 👉 setter_end 👈);
     {% else %}
-    throw qtgql::exceptions::NotImplementedError({"can't deserialize model of 👉proxy_field.type.of_type.__class__👈"});
+        👉proxy_field.concrete.type.member_type👈 👉proxy_field.name👈_init_vec;
+        for (const auto& node: data.value("👉proxy_field.name👈").toArray()){
+        {% if proxy_field.type.is_model.of_type.is_queried_object_type %}
+            👉proxy_field.name👈_init_vec.push_back(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
+        {% elif proxy_field.type.is_model.of_type.is_queried_union or proxy_field.type.is_model.of_type.is_queried_interface %}
+            auto node_data = node.toObject();
+            auto 👉proxy_field.name👈_typename = node_data.value("__typename").toString();
+            {%set type_cond -%}👉proxy_field.name👈_typename{% endset -%}
+            {% for choice in proxy_field.type.of_type.choices -%}
+            {% set do_on_meets -%}
+            👉proxy_field.name👈_init_vec.push_back(👉choice.deserializer_name👈(node_data, 👉operation_pointer👈) 👉 setter_end 👈);
+            {% endset -%}
+            👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
+            {% endfor %}
+        {% else %}
+        throw qtgql::exceptions::NotImplementedError({"can't deserialize model of 👉proxy_field.type.of_type.__class__👈"});
+        {% endif %}
+        };
+        👉 setter_name 👈(👉proxy_field.name👈_init_vec 👉 setter_end 👈);
     {% endif %}
-    };
-    👉 setter_name 👈(👉proxy_field.name👈_init_list👉 setter_end 👈);
 {% elif proxy_field.type.is_builtin_scalar -%}
     {% if proxy_field.type.is_void -%}
     /* deliberately empty */
     {% else -%}
     👉 setter_name 👈(data.value("👉proxy_field.name👈").👉 proxy_field.type.is_builtin_scalar.from_json_convertor 👈 👉 setter_end 👈);
     {% endif %}
     {% elif proxy_field.type.is_custom_scalar -%}
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 {% if field.type.is_queried_object_type  and field.type.is_optional %}
 if (👉 instance_of_concrete 👈){
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
 }
 {% elif field.type.is_queried_object_type %}
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
-{% elif field.type.is_model  %}
+{% elif field.type.is_model and not field.type.of_type.is_builtin_scalar %}
     {% if  field.type.is_model.of_type.is_queried_object_type %}
-    auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
+    auto init_vec_👉 field.name 👈 =  std::vector<👉field.type.of_type.name👈*>();
     for (const auto & node: 👉 instance_of_concrete 👈){
-    init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
+    init_vec_👉 field.name 👈.push_back(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
     }
-    👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
-    {% elif field.type.is_model.of_type.is_queried_union or field.type.is_model.of_type.is_queried_interface %}
-    auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.property_type👈>>();
+    👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.property_type 👈>(this, std::move(init_vec_👉 field.name 👈));
+    {% elif field.type.is_model.of_type.is_queried_union or field.type.is_model.of_type.is_queried_interface%}
+    auto init_vec_👉 field.name 👈 =  std::vector<👉field.type.of_type.property_type👈>();
     for (const auto & node: 👉 instance_of_concrete 👈){
         auto 👉field.name👈_typename = node->__typename();
         {%set type_cond -%}👉field.name👈_typename{% endset -%}
         {% for choice in field.type.of_type.choices -%}
         {% set do_on_meets -%}
-        init_list_👉 field.name 👈->append(qobject_cast<👉 field.type.of_type.property_type 👈>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(node))));
+        init_vec_👉 field.name 👈.push_back(qobject_cast<👉 field.type.of_type.property_type 👈>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(node))));
         {% endset -%}
         👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
         {% endfor %}
     }
-    👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.type_name() 👈>(this, std::move(init_list_👉 field.name 👈));
+    👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.property_type 👈>(this, std::move(init_vec_👉 field.name 👈));
     {% else %}
     not implemented
     {% endif %}
 {% elif field.type.is_queried_interface or  field.type.is_queried_union %}
 auto concrete_👉field.name👈 = 👉 instance_of_concrete 👈;
 auto 👉field.name👈_typename = concrete_👉field.name👈->__typename();
 {%set type_cond -%}👉field.name👈_typename{% endset -%}
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -56,15 +56,34 @@
     else{
     👉 setter_name 👈(👉proxy_field.type.deserializer_name👈(👉f_concrete.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
     }
     {% else %}
     👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
     {% endif %}
 {% elif proxy_field.type.is_model %}
-👉deserialize_concrete_field(proxy_field)👈
+    {% if proxy_field.type.of_type.is_builtin_scalar %}
+    auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toArray();
+    auto new_len = 👉f_concrete.name👈_data.size();
+    auto prev_len = 👉current👈->rowCount();
+    if (new_len < prev_len){
+        👉current👈->removeRows(prev_len - 1, prev_len - new_len);
+    }
+    for (int  i = 0; i < 👉f_concrete.name👈_data.size(); i++){
+        auto node_data = 👉f_concrete.name👈_data.at(i).👉 f_concrete.type.of_type.from_json_convertor 👈;
+        if (i >= prev_len){
+            👉current👈->append(node_data);
+        } else if (node_data != 👉current👈->get(i)){
+            👉current👈->replace(i, node_data);
+        }
+    }
+
+
+{% else %}
+    👉deserialize_concrete_field(proxy_field)👈
+    {% endif %}
 {% elif proxy_field.type.is_enum %}
 auto new_👉f_concrete.name👈= Enums::👉proxy_field.type.is_enum.map_name👈::by_name(data.value("👉proxy_field.name👈").toString());
 if (👉current👈 != new_👉f_concrete.name👈){
 👉 setter_name 👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
 {% elif proxy_field.type.is_queried_interface or proxy_field.type.is_queried_union %}
 auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toObject();
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.132.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 {%- from "macros/iterate_type_condition.jinja.hpp" import  iterate_type_condition -%}
 {% macro update_proxy_field(field, operation) -%}
 {% set new_concrete -%}
 m_inst->👉field.concrete.getter_name👈(👉field.build_variables_tuple_for_field_arguments 👈)
 {%- endset -%}
 auto operation = m_operation;
-{% if field.type.is_model -%}
+{% if field.type.is_model and not field.type.of_type.is_builtin_scalar -%}
     auto new_data = 👉new_concrete👈;
     auto new_len = new_data.size();
     auto prev_len = 👉field.private_name👈->rowCount();
     if (new_len < prev_len){
         👉field.private_name👈->removeRows(prev_len - 1, prev_len - new_len);
     }
     for (int i = 0; i < new_len; i++){
         const auto& concrete = new_data.at(i);
     {% if field.type.of_type.is_queried_object_type -%}
-        if (i > prev_len){
-            👉field.private_name👈->insert(i, new 👉field.type.of_type.name👈(operation, concrete));
+        if (i >= prev_len){
+            👉field.private_name👈->append(new 👉field.type.of_type.name👈(operation, concrete));
         } else {
             auto proxy_to_update = 👉field.private_name👈->get(i);
             if(proxy_to_update){
                 proxy_to_update->qtgql_replace_concrete(concrete);
             }
             else{ {#// handle optionals no need to delete -#}
-                👉field.private_name👈->insert(i, new 👉field.type.of_type.name👈(operation, concrete));
+                👉field.private_name👈->replace(i, new 👉field.type.of_type.name👈(operation, concrete));
             }
         }
 
     {% elif field.type.of_type.is_queried_union or field.type.of_type.is_queried_interface %}
         auto 👉field.name👈_typename = concrete->__typename();
         {%set type_cond -%}👉field.name👈_typename{% endset -%}
         {% for choice in field.type.of_type.choices %}
         {% set do_on_meets -%}
-        if (i > prev_len){
-            👉field.private_name👈->insert(i, new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
+        if (i >= prev_len){
+            👉field.private_name👈->append(new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
         } else{
             auto proxy_to_update = 👉field.private_name👈->get(i);
             if (proxy_to_update && proxy_to_update->__typename() == "👉choice.concrete.name👈"){
                 qobject_cast<👉choice.property_type👈>(proxy_to_update)->qtgql_replace_concrete(std::static_pointer_cast<👉choice.concrete.name👈>(concrete));
             }
             else{
-                👉field.private_name👈->insert(i, new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
+                👉field.private_name👈->replace(i, new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
                 delete proxy_to_update; {# // might have been optional or the type_name changed #}
             }
 
         }
 
         {% endset %}
         👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,18 @@
 };
 
 
 
 // 👉 t.name 👈 Getters
 {%for f in t.fields -%}
 [[nodiscard]] const 👉 f.type.property_type 👈  👉 t.name 👈::👉 f.concrete.getter_name 👈() const {
-{% if f.type.is_queried_object_type or f.type.is_model or f.type.is_queried_interface or f.type.is_queried_union %}
+
+{% if f.type.is_model and f.type.of_type.is_builtin_scalar -%}
+return m_inst->👉 f.concrete.getter_name 👈(👉f.build_variables_tuple_for_field_arguments.replace("operation", "m_operation")👈).get();
+{% elif f.type.is_queried_object_type or f.type.is_queried_interface or f.type.is_queried_union or f.type.is_model  -%}
 return 👉f.private_name👈;
 {% else -%}
 return m_inst->👉 f.concrete.getter_name 👈(👉f.build_variables_tuple_for_field_arguments.replace("operation", "m_operation")👈);
 {%- endif -%}
 };
 {% endfor %}
```

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.132.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.131.0/qtgqlcodegen/types.py` & `qtgql-0.132.0/qtgqlcodegen/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,27 +153,36 @@
 
     @property
     def is_model(self) -> QtGqlList | None:
         return self
 
     @property
     def member_type(self) -> str:
-        return f"QList<{self.of_type.member_type}>"
+        if self.of_type.is_builtin_scalar:
+            # scalars has no underlying fields hence they don't need to be
+            # proxied. So each proxy would get an instance to the model.
+            return f"std::shared_ptr<{self.type_name()}>"
+
+        return f"std::vector<{self.of_type.member_type}>"
 
     def type_name(self) -> str:
+        if bs := self.of_type.is_builtin_scalar:
+            return f"{QtGqlTypes.ListModelABC.name}<{bs.member_type}>"
         raise NotImplementedError(
-            "models have no valid type for schema concretes, call member_type",
+            "complex models have no valid type for schema concretes, call member_type",
         )
 
     @property
     def property_type(self) -> str:
         if self.of_type.is_queried_object_type or self.of_type.is_queried_interface:
-            return f"qtgql::bases::ListModelABC<{self.of_type.type_name()}> *"
+            return f"{QtGqlTypes.ListModelABC.name}<{self.of_type.property_type}> *"
         if self.of_type.is_queried_union:
-            return f"qtgql::bases::ListModelABC<{self.of_type.is_queried_union.type_name()}> *"
+            return f"{QtGqlTypes.ListModelABC.name}<{self.of_type.property_type}> *"
+        if bs := self.of_type.is_builtin_scalar:
+            return f"{QtGqlTypes.ListModelABC.name}<{bs.member_type}> *"
         raise NotImplementedError
 
 
 @define
 class QtGqlUnion(QtGqlTypeABC):
     types: tuple[QtGqlObjectType | QtGqlDeferredType, ...]
 
@@ -216,14 +225,18 @@
     def type_name(self) -> str:
         return self.attr.name
 
     @property
     def is_void(self) -> bool:
         return self is BuiltinScalars.VOID
 
+    @property
+    def property_type(self) -> str:
+        return self.type_name()
+
     def json_repr(self, attr_name: str | None = None) -> str:
         return f"{attr_name}"
 
 
 @define
 class CustomScalarDefinition(QtGqlTypeABC):
     name: str
```

### Comparing `qtgql-0.131.0/PKG-INFO` & `qtgql-0.132.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.131.0
+Version: 0.132.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
```

