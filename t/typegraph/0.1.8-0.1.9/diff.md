# Comparing `tmp/typegraph-0.1.8.tar.gz` & `tmp/typegraph-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph-0.1.8.tar", max compression
+gzip compressed data, was "typegraph-0.1.9.tar", max compression
```

## Comparing `typegraph-0.1.8.tar` & `typegraph-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     5254 2023-05-16 07:53:50.765317 typegraph-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     1446 2023-05-16 07:53:50.765317 typegraph-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      225 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/__init__.py
--rw-r--r--   0        0        0      904 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/effects.py
--rw-r--r--   0        0        0     3323 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/auth/__init__.py
--rw-r--r--   0        0        0      377 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/auth/oauth2.py
--rw-r--r--   0        0        0     1868 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/builder.py
--rw-r--r--   0        0        0     3066 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/models.py
--rw-r--r--   0        0        0     1953 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/nodes.py
--rw-r--r--   0        0        0     5774 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/typegraph.py
--rw-r--r--   0        0        0     9347 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/base/importer.py
--rw-r--r--   0        0        0     3667 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/base/typify.py
--rw-r--r--   0        0        0     7421 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/google_discovery.py
--rw-r--r--   0        0        0     4236 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/graphql.py
--rw-r--r--   0        0        0     8909 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/openapi.py
--rw-r--r--   0        0        0     3904 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/injection.py
--rw-r--r--   0        0        0     4338 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/policies.py
--rw-r--r--   0        0        0     1761 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/aws/runtimes/s3.py
--rw-r--r--   0        0        0    28490 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/relations.py
--rw-r--r--   0        0        0    17565 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/runtimes/prisma.py
--rw-r--r--   0        0        0     6601 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/schema.py
--rw-r--r--   0        0        0    15008 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/type_generator.py
--rw-r--r--   0        0        0     2373 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/utils.py
--rw-r--r--   0        0        0     2185 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/temporal/runtimes/temporal.py
--rw-r--r--   0        0        0     1351 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/base.py
--rw-r--r--   0        0        0     5322 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/deno.py
--rw-r--r--   0        0        0     1494 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/graphql.py
--rw-r--r--   0        0        0     2598 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/http.py
--rw-r--r--   0        0        0     1431 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/python.py
--rw-r--r--   0        0        0     2949 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/random.py
--rw-r--r--   0        0        0     2053 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/typegate.py
--rw-r--r--   0        0        0     1178 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/wasmedge.py
--rw-r--r--   0        0        0    22574 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/types.py
--rw-r--r--   0        0        0      487 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/__init__.py
--rw-r--r--   0        0        0      644 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/attrs.py
--rw-r--r--   0        0        0     1977 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/jsonschema.py
--rw-r--r--   0        0        0     2198 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/loaders.py
--rw-r--r--   0        0        0      185 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/sanitizers.py
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 typegraph-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    15181 2023-05-26 17:50:09.169361 typegraph-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     1460 2023-05-26 17:50:09.169361 typegraph-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-05-26 17:50:09.169361 typegraph-0.1.9/typegraph/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-26 17:50:09.169361 typegraph-0.1.9/typegraph/effects.py
+-rw-r--r--   0        0        0     3349 2023-05-26 17:50:09.169361 typegraph-0.1.9/typegraph/graph/auth/__init__.py
+-rw-r--r--   0        0        0      404 2023-05-26 17:50:09.169361 typegraph-0.1.9/typegraph/graph/auth/oauth2.py
+-rw-r--r--   0        0        0     1895 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/graph/builder.py
+-rw-r--r--   0        0        0     3093 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/graph/models.py
+-rw-r--r--   0        0        0     1980 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/graph/nodes.py
+-rw-r--r--   0        0        0     6041 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/graph/typegraph.py
+-rw-r--r--   0        0        0    10109 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/importers/base/importer.py
+-rw-r--r--   0        0        0     3951 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/importers/base/typify.py
+-rw-r--r--   0        0        0     7665 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/importers/google_discovery.py
+-rw-r--r--   0        0        0     4263 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/importers/graphql.py
+-rw-r--r--   0        0        0    11024 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/importers/openapi.py
+-rw-r--r--   0        0        0     3931 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/injection.py
+-rw-r--r--   0        0        0     4365 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/policies.py
+-rw-r--r--   0        0        0     3634 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/aws/runtimes/s3.py
+-rw-r--r--   0        0        0    28517 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/prisma/relations.py
+-rw-r--r--   0        0        0    17592 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/prisma/runtimes/prisma.py
+-rw-r--r--   0        0        0     6628 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/prisma/schema.py
+-rw-r--r--   0        0        0    15035 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/prisma/type_generator.py
+-rw-r--r--   0        0        0     2400 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/prisma/utils.py
+-rw-r--r--   0        0        0     2497 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/providers/temporal/runtimes/temporal.py
+-rw-r--r--   0        0        0     1378 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/base.py
+-rw-r--r--   0        0        0     5349 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/deno.py
+-rw-r--r--   0        0        0     1521 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/graphql.py
+-rw-r--r--   0        0        0     2625 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/http.py
+-rw-r--r--   0        0        0     1458 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/python.py
+-rw-r--r--   0        0        0     2976 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/random.py
+-rw-r--r--   0        0        0     2080 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/typegate.py
+-rw-r--r--   0        0        0     1204 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/runtimes/wasmedge.py
+-rw-r--r--   0        0        0    23259 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/types.py
+-rw-r--r--   0        0        0      514 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/utils/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/utils/attrs.py
+-rw-r--r--   0        0        0     3438 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/utils/jsonschema.py
+-rw-r--r--   0        0        0     2465 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/utils/loaders.py
+-rw-r--r--   0        0        0      914 2023-05-26 17:50:09.173361 typegraph-0.1.9/typegraph/utils/sanitizers.py
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 typegraph-0.1.9/PKG-INFO
```

### Comparing `typegraph-0.1.8/pyproject.toml` & `typegraph-0.1.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "typegraph"
-version = "0.1.8"
-description = "The low-code API platform for developers. Build modular APIs with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
+version = "0.1.9"
+description = "Open source, low-code backend platform for developers — build modular APIs with zero-trust and serverless deployment, no matter where and how (legacy) systems are."
 authors = ["Metatype Contributors <support@metatype.dev>"]
-license = "ELv2"
+license = "MPL-2.0"
 homepage = "https://metatype.dev"
 repository = "https://github.com/metatypedev/metatype"
 include = ["typegraph/**/*", "LICENSE.md"]
 keywords = ["api", "composition", "typesystem", "graphql", "ecosystem"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typegraph-0.1.8/typegraph/effects.py` & `typegraph-0.1.9/typegraph/effects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from enum import auto
 from typing import Optional
 
 from attrs import frozen
 from strenum import LowercaseStrEnum
```

### Comparing `typegraph-0.1.8/typegraph/graph/auth/__init__.py` & `typegraph-0.1.9/typegraph/graph/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
-
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Dict
 
 from typegraph.graph.auth import oauth2
 from typegraph.graph.models import Auth
```

### Comparing `typegraph-0.1.8/typegraph/graph/builder.py` & `typegraph-0.1.9/typegraph/graph/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Dict, Union
 
 from ordered_set import OrderedSet
 
 from typegraph.graph.nodes import Node, NodeProxy
```

### Comparing `typegraph-0.1.8/typegraph/graph/models.py` & `typegraph-0.1.9/typegraph/graph/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Dict, List, Literal, Optional
 
 from attrs import define, field, frozen
 
 
 @define
```

### Comparing `typegraph-0.1.8/typegraph/graph/nodes.py` & `typegraph-0.1.9/typegraph/graph/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional
 
 if TYPE_CHECKING:
     from typegraph import types as t
     from typegraph.graph.builder import Collector
     from typegraph.graph.typegraph import TypeGraph
```

### Comparing `typegraph-0.1.8/typegraph/graph/typegraph.py` & `typegraph-0.1.9/typegraph/graph/typegraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import inspect
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Set, Union
 
 from typegraph.graph.builder import Collector
 from typegraph.graph.models import Auth, Cors, Rate
 from typegraph.graph.nodes import Node, NodeProxy
 from typegraph.runtimes.deno import DenoRuntime
 
 if TYPE_CHECKING:
     from typegraph import types as t
+    from typegraph.policies import Policy
 
 
 OperationTable = Dict[str, Union["t.func", "t.struct"]]
 
 typegraph_version = "0.0.1"
 
 
@@ -66,32 +68,37 @@
         TypegraphContext.pop()
 
     def __call__(
         self, node: str, after_apply: Callable[["t.typedef"], "t.typdef"] = lambda x: x
     ) -> "NodeProxy":
         return NodeProxy(self, node, after_apply)
 
-    def expose(self, **ops: Union["t.func", "t.struct"]):
+    def expose(
+        self,
+        default_policy: Optional[Union["Policy", List["Policy"]]] = None,
+        **ops: Union["t.func", "t.struct"],
+    ):
         from typegraph import types as t
 
-        default_policy = ops.pop("default_policy", [])
-        if not isinstance(default_policy, list):
-            default_policy = [default_policy]
+        default_policies = default_policy or []
+        if not isinstance(default_policies, list):
+            default_policies = [default_policies]
 
         # allow to expose only functions or structures (namespaces)
         for name, op in ops.items():
             if not isinstance(op, t.func) and not isinstance(op, t.struct):
                 raise Exception(
-                    f"cannot expose type {op.title} under {name}, requires a function or structure (namespace), got a {op.type}"
+                    f"cannot expose type {op.title} under {name}, requires a function"
+                    f" or structure (namespace), got a {op.type}"
                 )
 
             if name in self.exposed:
                 raise Exception(f"operation {name} already exposed")
 
-            self.exposed[name] = op.add_policy(*default_policy)
+            self.exposed[name] = op.add_policy(*default_policies)
 
         return self
 
     def root(self) -> "t.struct":
         from typegraph import types as t
 
         def assert_no_effect_materializers(
@@ -114,15 +121,16 @@
                         )
                     assert_no_effect_materializers(e.out)
 
                 else:
                     assert_no_effect_materializers(e)
 
         with self:
-            root = t.struct(self.exposed).named(self.name)
+            # allow all characters for the root entry-point
+            root = t.struct(self.exposed).named(self.name, validate=False)
 
         root._propagate_runtime(DenoRuntime())
 
         return root
 
     def collect_nodes(self) -> Collector:
         def visit(nodes: List[Node], collector: Collector):
```

### Comparing `typegraph-0.1.8/typegraph/importers/base/importer.py` & `typegraph-0.1.9/typegraph/importers/base/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import inspect
 import itertools
 import re
 import sys
 from ast import literal_eval
 from typing import Dict, List, Optional, Set, Tuple
@@ -11,67 +12,70 @@
 from attrs import define, field, frozen
 from box import Box
 from redbaron import AtomtrailersNode, NameNode, RedBaron
 
 from typegraph import TypeGraph, t
 from typegraph.importers.base.typify import Typify
 from typegraph.types import reserved_types
+from typegraph.utils.sanitizers import as_attr
 
 # TODO: detect indentation size/character from file
 
 
 @define
 class Codegen:
     indent: str = field(default=" " * 4)
     indent_level: int = field(default=1)
     indent_level_pyi: int = field(default=0)
     res: str = field(default="", init=False)
     res_hint: str = field(default="", init=False)
 
-    def line(self, line: str = "", indent_level=0):
+    def line(self, line: str = "", indent_level=0, do=True):
+        if not do:
+            return
         indent = self.indent * (self.indent_level + indent_level)
         if line == "":
             self.res += "\n"
         else:
             self.res += f"{indent}{line}\n"
 
-    def hint_line(self, line: str = "", indent_level=0):
+    def hint_line(self, line: str = "", indent_level=0, do=True):
+        if not do:
+            return
         indent = self.indent * (self.indent_level_pyi + indent_level)
         if line == "":
             self.res_hint += "\n"
         else:
             self.res_hint += f"{indent}{line}\n"
 
 
-# Some Type Name => Some_Type_Name
-def as_attr(name: str):
-    return re.sub(r"\s+", "_", name)
-
-
 class Importer:
     """Base importer class"""
 
     imports: Set[Tuple[str, str]]
     headers: List[str]  # codegen header lines
     name: str
     types: Dict[str, t.typedef]
     exposed: Dict[str, t.func]
     renames: Dict[str, str]
     tg: TypeGraph
+    enable_params: bool
 
     def __init__(
         self, name: str, *, renames: Dict[str, str] = {}, keep_names: List[str] = []
     ):
         """
         Args:
             `name`: name of the importer
             `renames`: a dictionary mapping original (imported) names to exposed names
             `keep_names`: a list of names to keep as the original (imported)
         """
 
+        self.enable_params = False
+
         self.imports = {
             ("typegraph", "t"),
         }
         self.headers = []
 
         valid_name = re.sub("\\W", "_", name)
         if valid_name != name:
@@ -125,45 +129,58 @@
         typify = Typify(self, "t")
 
         for header_line in self.headers:
             cg.line(header_line)
         cg.line()
 
         counter = itertools.count(1)
-        renames = {name: f"_{self.name}_{next(counter)}_{name}" for name in self.types}
+        renames = {
+            as_attr(name): f"_{as_attr(self.name)}_{next(counter)}_{as_attr(name)}"
+            for name in self.types
+        }
         renames.update(self.renames)
 
         cg.line(f"renames = {repr(renames)}")
         cg.line()
 
         cg.line("types = {}")
         cg.hint_line("from typegraph import t")
+        cg.hint_line("from typing import Dict, Union", do=self.enable_params)
         cg.hint_line("class TypeList:")
 
         if len(self.types) > 0:
             for name, tpe in self.types.items():
-                cg.line(f"types[{repr(name)}] = {typify(tpe, name)}")
-                cg.hint_line(f"{as_attr(name)}: t.typedef = ...", 1)
-
+                attr_name = as_attr(name)
+                cg.line(f"types[{repr(attr_name)}] = {typify(tpe, name)}")
+                cg.hint_line(f"{attr_name}: t.typedef = ...", 1)
             cg.line()
 
         cg.line("functions = {}")
         cg.hint_line("class FuncList:")
         for name, fn in self.exposed.items():
-            cg.line(f"functions[{repr(name)}] = {typify(fn)}")
-            cg.hint_line(f"{as_attr(name)}: t.func = ...", 1)
+            attr_name = as_attr(name)
+            cg.line(f"functions[{repr(attr_name)}] = {typify(fn)}")
+            cg.hint_line(f"{attr_name}: t.func = ...", 1)
         cg.line()
 
         cg.hint_line("class Import:")
         cg.hint_line("types: TypeList = ...", 1)
         cg.hint_line("functions: FuncList = ...", 1)
-        cg.hint_line(f"def {self.get_def_name()}() -> Import: ...")
+
+        cg.hint_line(
+            f"def {self.get_def_name()}(params: Union[None, Dict[str, str]]) -> Import: ...",
+            do=self.enable_params,
+        )
+        cg.hint_line(
+            f"def {self.get_def_name()}() -> Import: ...", do=not self.enable_params
+        )
 
         self.imports.add(("box", "Box"))
         self.imports.add(("typegraph.importers.base.importer", "Import"))
+
         cg.line(
             f"return Import(importer={repr(self.name)}, renames=renames, types=Box(types), functions=Box(functions))"
         )
 
         return cg
 
     def get_def_name(self):
@@ -211,27 +228,31 @@
             if comment_node.type != "comment":
                 target_node.insert_before(comment)
             else:
                 comment_node.value = comment
             target_node.value = source.res
         else:
             wth.insert_before(comment)
-            wth.insert_before(f"def {name}():\n{source.res}")
+            if self.enable_params:
+                wth.insert_before(f"def {name}(params = None):\n{source.res}")
+            else:
+                wth.insert_before(f"def {name}():\n{source.res}")
 
         new_code = black.format_str(code.dumps(), mode=black.FileMode())
         new_hint_code = black.format_str(source.res_hint, mode=black.FileMode())
 
         with open(file, "w") as f:
             f.write(new_code)
 
         filename_pyi = re.sub(r"\.py$", ".pyi", file)
         with open(filename_pyi, "w") as f:
             f.write(new_hint_code)
 
         print(f"File updated: {file}", file=sys.stderr)
+        print(f"File updated: {filename_pyi}", file=sys.stderr)
         exit(0)
 
     def find_generate_arg(self, code: RedBaron) -> Optional[NameNode]:
         for node in code.find_all("atomtrailers"):
             found = self.find_generate_arg_in(node)
             if found:
                 return found
```

### Comparing `typegraph-0.1.8/typegraph/importers/base/typify.py` & `typegraph-0.1.9/typegraph/importers/base/typify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import TYPE_CHECKING, Callable, Optional, Union, cast
 
 from attrs import define, field, frozen
 
 from typegraph import effects
 from typegraph import types as t
 from typegraph.effects import Effect
 from typegraph.graph.nodes import NodeProxy
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always
+from typegraph.utils.sanitizers import as_attr
 
 if TYPE_CHECKING:
     from typegraph.importers.base.importer import Importer
 
 
 @frozen
 class TypifyRuntime(Runtime):
@@ -39,25 +41,25 @@
     ns: str = field(default="t")
 
     def __call__(self, typ: t.TypeNode, name: Optional[str] = None) -> str:
         # dispatch
         if isinstance(typ, NodeProxy):
             renames = self.importer.renames
             name = renames[typ.node] if typ.node in renames else typ.node
-            return f"{self.ns}.proxy(renames[{repr(name)}])"
+            return f"{self.ns}.proxy(renames[{repr(as_attr(name))}])"
 
         if hasattr(self, typ.type):
             method = getattr(self, typ.type)
         else:
             if typ.type in simple_types:
                 method = getattr(self, "simple")
             else:
                 raise Exception(f"No handler for type '{typ.type}'")
 
-        suffix = "" if name is None else f".named(renames[{repr(name)}])"
+        suffix = "" if name is None else f".named(renames[{repr(as_attr(name))}])"
         return method(typ) + suffix
 
     def constraints(typ: t.typedef) -> str:
         ret = ""
         if not hasattr(typ, "_constraints"):
             return ret
         for k, v in typ._constraints().items():
@@ -89,15 +91,20 @@
     def array(self, typ: t.typedef) -> str:
         typ = cast(t.array, typ)
         return f"{self.ns}.array({self(typ.of)}){Typify.constraints(typ)}"
 
     def union(self, typ: t.typedef) -> str:
         typ = cast(t.union, typ)
         variants = [self(v) for v in typ.variants]
-        return f"{self.ns}.union({', '.join(variants)})"
+        return f"{self.ns}.union([{', '.join(variants)}])"
+
+    def either(self, typ: t.typedef) -> str:
+        typ = cast(t.union, typ)
+        variants = [self(v) for v in typ.variants]
+        return f"{self.ns}.either([{', '.join(variants)}])"
 
     def function(self, typ: t.typedef) -> str:
         typ = cast(t.func, typ)
         assert isinstance(typ.mat, TypifyMat)
         codegen = typ.mat.codegen
         if callable(codegen):
             return codegen(self(typ.inp), self(typ.out))
```

### Comparing `typegraph-0.1.8/typegraph/importers/google_discovery.py` & `typegraph-0.1.9/typegraph/importers/google_discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typegraph import t
 from typing import Dict, List, Optional
 import json
 import re
 
 import httpx
@@ -54,24 +55,25 @@
     def generate(self):
         assert self.specification.discoveryVersion == "v1"
         assert self.specification.protocol == "rest"
 
         self.specification.revision
         self.specification.version
 
-        self.specification.canonicalName
+        # self.specification.canonicalName
         self.specification.description
         self.specification.documentationLink
         with self:
-            # self.renames["ErrorResponse"] = "error_response"
             self.types["ErrorResponse"] = self.error_struct()
             for schema in self.specification.schemas.values():
-                assert schema.type == "object"
-                # self.renames[f"{schema.id}In"] = f"{camel_to_snake(schema.id)}_in"
-                # self.renames[f"{schema.id}Out"] = f"{camel_to_snake(schema.id)}_out"
+                assert schema.type == "object" or schema.type == "any"
+                if schema.type == "any":
+                    print(f"Warning: schema of type '{schema.type}' not supported")
+                    continue
+
                 self.types[f"{schema.id}In"] = self.gen_type(
                     schema,
                     has_error=False,
                     filter_read_only=False,
                     suffix="In",
                     allow_opt=False,
                 )
@@ -110,14 +112,17 @@
         if "id" in cursor:
             ref = f"{cursor.id}{suffix}"
             # self.renames[ref] = ref
             self.obj_fields_cache[ref] = fields
 
         return ret
 
+    def gen_any(self):
+        return t.struct({"_": t.string().optional()})
+
     def gen_type(
         self, cursor, has_error=False, filter_read_only=False, suffix="", allow_opt=True
     ):
         if (
             allow_opt
             and "description" in cursor
             and not cursor.description.startswith("Required")
@@ -134,15 +139,15 @@
             return t.proxy(f'{cursor["$ref"]}{suffix}')
 
         simple_type = {
             "string": t.string(),
             "boolean": t.boolean(),
             "integer": t.integer(),
             "number": t.float(),
-            "any": t.struct({"_": t.string().optional()}),
+            "any": self.gen_any(),
         }
 
         tpe = simple_type.get(cursor.type)
         if tpe is not None:
             return tpe
 
         if cursor.type == "array":
@@ -156,34 +161,40 @@
 
         raise Exception(f"Unexpect type {cursor}")
 
     def prepare_expose(self, cursor, hierarchy="", url_prefix=""):
         if "methods" in cursor:
             for methodName, method in cursor.methods.items():
                 inp_fields: Dict[str, t.typedef] = {}
-                # query params
-                for parameterName, parameter in method.parameters.items():
-                    if parameterName != "readMask":
-                        inp_fields[parameterName] = self.gen_type(
-                            parameter, suffix="In"
-                        )
+                if "parameters" in method:
+                    # query params
+                    for parameterName, parameter in method.parameters.items():
+                        if parameterName != "readMask":
+                            inp_fields[parameterName] = self.gen_type(
+                                parameter, suffix="In"
+                            )
 
-                # flatten first depth fields
+                # flatten first depth fields and merge
                 if "request" in method and "$ref" in method.request:
                     # resolve first depth
                     ref = f"{method.request.get('$ref')}In"
                     assert self.obj_fields_cache.get(ref) is not None
                     for k, v in self.obj_fields_cache.get(ref).items():
                         inp_fields[k] = v
+
                 # Bearer token
                 inp_fields["auth"] = t.string().optional()
 
                 # In/Out
                 inp = t.struct(inp_fields)
-                out = self.gen_type(method.response, suffix="Out")
+                out = None
+                if "response" not in method:
+                    out = self.gen_any()
+                else:
+                    out = self.gen_type(method.response, suffix="Out")
 
                 # kwargs
                 fparams = {
                     "auth_token_field": repr("auth"),  # Bearer token
                     "content_type": repr("application/json"),
                 }
                 kwargs = ", ".join([f"{k}={v}" for k, v in fparams.items()])
```

### Comparing `typegraph-0.1.8/typegraph/importers/graphql.py` & `typegraph-0.1.9/typegraph/importers/graphql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import json
 from typing import Literal, Optional
 
 import httpx
 from box import Box
 from graphql import get_introspection_query
```

### Comparing `typegraph-0.1.8/typegraph/importers/openapi.py` & `typegraph-0.1.9/typegraph/importers/openapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import json
 import pathlib
 import re
 from sys import stderr
 from typing import Callable, Dict, List, Optional, Tuple
 from urllib.parse import urljoin
@@ -23,20 +24,33 @@
         "urlenc": "application/x-www-form-urlencoded",
         "multipart": "multipart/form-data",
     }
 )
 
 
 def ref_to_name(ref: str) -> str:
-    match = re.match(r"^#/components/schemas/(\w+)$", ref)
+    """
+    Example match:\n
+    `#/components/schemas/financial_connections.account_owner`
+    """
+    match = re.match(r"^#/components/schemas/([\w\-_\.]+)$", ref)
     if not match:
         raise Exception(f"Could not resolve $ref '{ref}'")
     return match.group(1)
 
 
+def create_fn_name(method: str, path: str):
+    """
+    Example:\n
+    `method`=get, `path`=/users/{id} => getUsersId
+    """
+    parts = map(lambda s: s.capitalize(), re.findall(r"([^/{}]+)", path))
+    return f"{method}{''.join(parts)}"
+
+
 class OpenApiImporter(Importer):
     base_url: str
     specification: Box
     additional_types: List[str]
     typedef_from_jsonschema: TypedefFromJsonSchema
 
     def __init__(
@@ -64,15 +78,14 @@
                 r"\.yaml$", url
             ):
                 self.specification = Box(yaml.safe_load(res.text))
             else:  # suppose it is JSON
                 self.specification = Box(res.json())
 
             self.base_url = url
-
         else:
             assert file is not None and base_url is not None
             self.base_url = base_url
 
             path = pathlib.Path(file)
             with open(path) as f:
                 if path.suffix == ".json":
@@ -85,21 +98,30 @@
                     )
 
         self.typedef_from_jsonschema = TypedefFromJsonSchema(
             ref_to_name, lambda ref: self.resolve_ref(ref)
         )
 
         self.imports.add(("typegraph.runtimes.http", "HTTPRuntime"))
+        self.imports.add(("typegraph.utils.sanitizers", "inject_params"))
 
         if "servers" in self.specification:
             server_url = self.specification.servers[0].url
         else:
             server_url = "/"
-        url = urljoin(self.base_url, server_url)
-        self.headers.append(f"{name} = HTTPRuntime({repr(url)})")
+
+        # Enable the function argument `params`
+        self.enable_params = True
+        if server_url.startswith("/"):
+            url = urljoin(self.base_url, server_url)
+        else:
+            url = server_url
+
+        self.headers.append(f"target_url = inject_params({repr(url)}, params)")
+        self.headers.append(f"{name} = HTTPRuntime(target_url)")
 
     def resolve_ref(self, obj: Box):
         if "$ref" not in obj:
             return obj
 
         match = re.match(r"#/components/([^/]+)/([^/]+)$", obj["$ref"])
         if not match:
@@ -111,16 +133,19 @@
         assert ver.major == 3
         assert ver.minor <= 0
 
         self.specification.info
         self.specification.paths
 
         schemas = self.specification.get("components", {}).get("schemas", [])
-        for name, schema in schemas.items():
-            self.add_schema(name, schema)
+
+        # can be a BoxList(list) or a list
+        if hasattr(schemas, "items"):
+            for name, schema in schemas.items():
+                self.add_schema(name, schema)
 
         with self as imp:
             for path in self.specification.paths:
                 for name, fn in self.gen_functions(path).items():
                     imp.expose(name, fn)
 
     def add_schema(self, name: str, schema: Box):
@@ -170,27 +195,30 @@
         self.runtime = importer.name
         self.typedef_from_jsonschema = importer.typedef_from_jsonschema
         self.resolve_ref = lambda ref: importer.resolve_ref(ref)
 
     def generate_functions(self):
         ret = {}
         for method in self.spec:
+            name = None
             if method in METHODS:
                 try:
                     name, fn = self.generate_function(method)
                     ret[name] = fn
                 except Exception as e:
-                    name = self.spec[method].operationId
+                    identifier = name
+                    if identifier is None:
+                        identifier = f"method={method} path={self.path}"
                     print(
-                        f"Warning: Generation of function '{name}' skipped: {e}",
+                        f"Warning: Generation of function {identifier}: {e}",
                         file=stderr,
                     )
             else:
                 print(
-                    f"Warning: Unsupported method {method}: generation skipped",
+                    f"Warning: Unsupported method {method} at path={self.path}: generation skipped",
                     file=stderr,
                 )
         return ret
 
     def generate_function(self, method: str) -> Tuple[str, t.func]:
         spec = self.spec[method]
         inp_type, inp_config = self.gen_input_type(spec)
@@ -213,16 +241,24 @@
             else:
                 out = t.struct()
 
         # TODO what for other 4xx codes
         if "404" in spec.responses:
             out = out.optional()
 
+        # operationId is optional
+        # (method, path) can still uniquely identify a endpoint
+        name = (
+            spec.operationId
+            if hasattr(spec, "operationId")
+            else create_fn_name(method, self.path)
+        )
+
         return (
-            spec.operationId,
+            name,
             t.func(
                 inp_type,
                 out,
                 TypifyMat(
                     lambda inp, out: f"{self.runtime}.{method}('{self.path}', {inp}, {out}, {as_kwargs(inp_config)})"
                 ),
             ),
@@ -243,28 +279,46 @@
 
         if "requestBody" in op_spec:
             body = op_spec.requestBody.content
             types = body.keys()
             if MIME_TYPES.json in types:
                 content_type = MIME_TYPES.json
             elif MIME_TYPES.urlenc in types:
-                content_type = MIME_TYPES.json
+                content_type = MIME_TYPES.urlenc
             elif MIME_TYPES.multipart in types:
                 content_type = MIME_TYPES.multipart
             else:
                 raise Exception(
                     f"No supported content type for request: {', '.join(types)}"
                 )
-
             schema = body[content_type].schema
             schema = self.resolve_ref(schema)
+
             if schema.type != "object":
                 raise Exception(f"Unsupported type for request body: {schema.type}")
 
-            for name, typ in self.typedef_from_jsonschema(schema).props.items():
+            gen_typ = self.typedef_from_jsonschema(schema)
+            if isinstance(gen_typ, t.optional):
+                gen_typ = gen_typ.of
+
+            # print(f"{gen_typ.name} of type {gen_typ.__class__.__name__}")
+            # print(f"  {schema}")
+            if not isinstance(gen_typ, t.struct):
+                """
+                Example:
+                Spec: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.yaml
+                At method=post path=/repos/{owner}/{repo}/pages
+                - It uses `anyOf` with *property names of the *closest schema as variants but not references to object or schemas (against jsonschema spec)
+                https://swagger.io/docs/specification/data-models/oneof-anyof-allof-not/
+                """
+                raise Exception(
+                    f"spec assigned type as 'object' but '{gen_typ.__class__.__name__}' was generated instead"
+                )
+
+            for name, typ in gen_typ.props.items():
                 if name in props:
                     raise Exception(
                         f"Name clash: '{name}' present in both query parameters and request body"
                     )
                 props[name] = typ
 
             kwargs.content_type = repr(content_type)
```

### Comparing `typegraph-0.1.8/typegraph/injection.py` & `typegraph-0.1.9/typegraph/injection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 from attrs import field, frozen
 from typegraph.graph.builder import Collector
 from typegraph.graph.nodes import NodeProxy
 from typegraph.utils.attrs import always
 from typegraph.graph.nodes import Node
```

### Comparing `typegraph-0.1.8/typegraph/policies.py` & `typegraph-0.1.9/typegraph/policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import re
 from typing import List, Optional, Pattern, Union
 
 from attrs import evolve, field, frozen
 
 from typegraph.effects import EffectType
```

### Comparing `typegraph-0.1.8/typegraph/providers/aws/runtimes/s3.py` & `typegraph-0.1.9/typegraph/runtimes/wasmedge.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,53 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
+
+import base64
 
 from attrs import frozen
 
-from typegraph import effects, t
+from typegraph import effects
+from typegraph import types as t
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
-from typegraph.utils.attrs import always
+from typegraph.utils.attrs import always, required
 
 
 @frozen
-class S3Runtime(Runtime):
+class WasmEdgeRuntime(Runtime):
     """
-    [Documentation](https://metatype.dev/docs/reference/runtimes/s3)
+    [Documentation](https://metatype.dev/docs/reference/runtimes/wasmedge)
     """
 
-    host: str
-    region: str
-    access_key_secret: str
-    secret_key_secret: str
-    runtime_name: str = always("s3")
+    runtime_name: str = always("wasmedge")
 
     def data(self, collector):
-        data = super().data(collector)
-        data["data"].update(
-            host=self.host,
-            region=self.region,
-            access_key_secret=self.access_key_secret,
-            secret_key_secret=self.secret_key_secret,
-        )
-        return data
-
-    def sign(self, bucket: str, content_type: str):
-        return t.func(
-            t.struct({"length": t.integer(), "path": t.string()}),
-            t.string(),
-            SignMat(self, bucket, content_type),
-        )
+        return {
+            **super().data(collector),
+        }
+
+    def wasi(
+        self,
+        wasm_file: str,
+        func: str,
+        inp,
+        out,
+        effect: Effect = effects.none(),
+        **kwargs
+    ):
+        with open(wasm_file, "rb") as f:
+            wasm = base64.b64encode(f.read()).decode("utf-8")
 
-    def list(self, bucket: str):
         return t.func(
-            t.struct({"path": t.string()}),
-            t.struct(
-                {
-                    "keys": t.array(t.struct({"key": t.string(), "size": t.integer()})),
-                    "prefix": t.array(t.string()),
-                }
-            ),
-            ListMat(self, bucket),
+            inp,
+            out,
+            WASIMat(self, wasm, func, effect=effect, **kwargs),
         )
 
 
 @frozen
-class SignMat(Materializer):
-    runtime: Runtime
-    bucket: str
-    content_type: str
-    materializer_name: str = always("sign")
-    effect: Effect = always(effects.none())
-
-
-@frozen
-class ListMat(Materializer):
+class WASIMat(Materializer):
     runtime: Runtime
-    bucket: str
-    materializer_name: str = always("list")
-    effect: Effect = always(effects.none())
+    wasm: str
+    func: str
+    effect: Effect = required()
+    materializer_name: str = always("wasi")
```

### Comparing `typegraph-0.1.8/typegraph/providers/prisma/relations.py` & `typegraph-0.1.9/typegraph/providers/prisma/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from collections import defaultdict
 
 from attr import field
 from typegraph import t, TypeGraph
 from attrs import define, frozen
 from typing import Any, Optional, Tuple, List, Dict
```

### Comparing `typegraph-0.1.8/typegraph/providers/prisma/runtimes/prisma.py` & `typegraph-0.1.9/typegraph/providers/prisma/runtimes/prisma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import List, Optional, Union
 
 from attrs import field, frozen
 
 from typegraph import effects
 from typegraph import types as t
```

### Comparing `typegraph-0.1.8/typegraph/providers/prisma/schema.py` & `typegraph-0.1.9/typegraph/providers/prisma/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import List, Optional, Tuple
 
 from attrs import evolve, frozen
 
 from typegraph import types as t
 from typegraph.graph.typegraph import resolve_proxy
```

### Comparing `typegraph-0.1.8/typegraph/providers/prisma/type_generator.py` & `typegraph-0.1.9/typegraph/providers/prisma/type_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Optional, Set, Union
 
 from attrs import frozen
 
 from typegraph import t
 from typegraph.graph.typegraph import find, resolve_proxy
```

### Comparing `typegraph-0.1.8/typegraph/providers/prisma/utils.py` & `typegraph-0.1.9/typegraph/providers/prisma/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typegraph import types as t
 from typegraph.graph.nodes import NodeProxy
 
 
 def resolve_entity_quantifier(tpe: t.typedef):
     if isinstance(tpe, t.array):
```

### Comparing `typegraph-0.1.8/typegraph/providers/temporal/runtimes/temporal.py` & `typegraph-0.1.9/typegraph/providers/temporal/runtimes/temporal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from attrs import frozen
 
+from typegraph import effects
 from typegraph import types as t
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always
 
 
 @frozen
 class TemporalRuntime(Runtime):
     """
     [Documentation](https://metatype.dev/docs/reference/runtimes/temporal)
     """
 
-    host: str
     name: str
+    host: str
     runtime_name: str = always("temporal")
 
     def data(self, collector):
         data = super().data(collector)
         data["data"].update(
             host=self.host,
         )
         return data
 
     def start_workflow(self, workflow_type: str, arg):
         return t.func(
             t.struct({"workflow_id": t.string(), "args": t.array(arg)}),
             t.string(),
-            StartWorkflowMat(self, workflow_type),
+            StartWorkflowMat(
+                runtime=self, effect=effects.create(), workflow_type=workflow_type
+            ),
         )
 
     def signal_workflow(self, signal_name: str, arg):
         return t.func(
             t.struct(
                 {"workflow_id": t.string(), "run_id": t.string(), "args": t.array(arg)}
             ),
             t.string(),
-            SignalWorkflowMat(self, signal_name),
+            SignalWorkflowMat(
+                runtime=self, effect=effects.update(), signal_name=signal_name
+            ),
         )
 
     def query_workflow(self, query_type: str, arg):
         return t.func(
             t.struct(
                 {"workflow_id": t.string(), "run_id": t.string(), "args": t.array(arg)}
             ),
             t.string(),
-            QueryWorkflowMat(self, query_type),
+            QueryWorkflowMat(
+                runtime=self, effect=effects.none(), query_type=query_type
+            ),
         )
 
     def describe_workflow(self):
         return t.func(
             t.struct({"workflow_id": t.string(), "run_id": t.string()}),
             t.string(),
-            DescribeWorkflowMat(self),
+            DescribeWorkflowMat(runtime=self, effect=effects.none()),
         )
 
 
 @frozen
 class StartWorkflowMat(Materializer):
     runtime: Runtime
     workflow_type: str
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/base.py` & `typegraph-0.1.9/typegraph/runtimes/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from attrs import frozen
 
 from typegraph.effects import Effect
 from typegraph.graph.builder import Collector
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/deno.py` & `typegraph-0.1.9/typegraph/runtimes/deno.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import os
 from typing import Any, Dict, List, Optional, Tuple
 
 from attrs import field, frozen
 from frozendict import frozendict
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/graphql.py` & `typegraph-0.1.9/typegraph/runtimes/graphql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Optional, Tuple
 
 from attrs import frozen
 
 from typegraph import effects
 from typegraph import types as t
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/http.py` & `typegraph-0.1.9/typegraph/runtimes/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Dict, Optional, Tuple
 
 from attrs import field, frozen
 from frozendict import frozendict
 
 from typegraph import effects
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/python.py` & `typegraph-0.1.9/typegraph/runtimes/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import ast
 import hashlib
 import inspect
 
 from astunparse import unparse
 from attr import field
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/random.py` & `typegraph-0.1.9/typegraph/runtimes/random.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import Callable, Dict, List, Optional
 
 from attrs import field, frozen
 
 from typegraph import effects, utils
 from typegraph import types as t
```

### Comparing `typegraph-0.1.8/typegraph/runtimes/typegate.py` & `typegraph-0.1.9/typegraph/runtimes/typegate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from attrs import frozen
 
 from typegraph import effects
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always
```

### Comparing `typegraph-0.1.8/typegraph/types.py` & `typegraph-0.1.9/typegraph/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Set,
     Tuple,
     Type,
+    TypeVar,
     Union,
     get_args,
     get_origin,
     overload,
 )
 
 from attrs import evolve, field, frozen
@@ -29,15 +31,16 @@
     context,
     parent,
     secret,
     static,
 )
 from typegraph.policies import Policy, EffectPolicies
 from typegraph.runtimes.base import Materializer, Runtime
-from typegraph.utils.attrs import SKIP, always, asdict
+from typegraph.utils.attrs import SKIP, asdict
+import re
 
 # if os.environ.get("DEBUG"):
 #     import debugpy
 
 #     debugpy.listen(5678)
 #     print("Waiting for debugger attach...")
 #     debugpy.wait_for_client()
@@ -51,30 +54,32 @@
 
 
 def is_optional(tpe: Type):
     # Optional = Union[T, NoneType]
     return get_origin(tpe) is Union and type(None) in get_args(tpe)
 
 
+def validate_name(name: str):
+    invalids = re.findall("[^_A-Za-z0-9]+", name)
+    # print(invalids)
+    if bool(invalids):
+        raise Exception(f'name "{name}" does not match [_A-Za-z0-9]')
+
+
 class Secret(Node):
     secret: str
 
     def __init__(self, secret: str):
         super().__init__(Collector.secrets)
         self.secret = secret
 
     def data(self, collector: "Collector") -> dict:
         return self.secret  # this is a string
 
 
-# Optional keyword-only field
-def optional_field():
-    return field(kw_only=True, default=None)
-
-
 # reserved types are used for internal implementation
 # and cannot be used to define user custom types
 #
 # more information at https://spec.graphql.org/draft/
 reserved_types = [
     # Primitives
     "Int",
@@ -103,27 +108,27 @@
     graph: TypeGraph = field(
         kw_only=True,
         factory=TypegraphContext.get_active,
         init=False,
         metadata={SKIP: True},
     )
     name: str = field(kw_only=True, default="")
-    description: Optional[str] = optional_field()
-    runtime: Optional["Runtime"] = optional_field()
-    injection: InjectionSwitch = optional_field()
+    description: Optional[str] = field(kw_only=True, default=None)
+    runtime: Optional["Runtime"] = field(kw_only=True, default=None)
+    injection: InjectionSwitch = field(kw_only=True, default=None)
     policies: Tuple[Policy, ...] = field(kw_only=True, factory=tuple)
     # runtime_config: Dict[str, Any] = field(
     #     kw_only=True, factory=dict, hash=False, metadata={SKIP: True}
     # )
     runtime_config: Dict[str, Any] = field(
         kw_only=True, factory=frozendict, hash=False, metadata={SKIP: True}
     )
-    _enum: Optional[Tuple[str]] = optional_field()
+    _enum: Optional[Tuple[str]] = field(kw_only=True, default=None)
 
-    collector_target: Optional[str] = always(Collector.types)
+    collector_target: Optional[str] = field(default=Collector.types, init=False)
 
     def __attrs_post_init__(self):
         if self.graph is None:
             raise Exception("No typegraph context")
         if self.name == "":
             object.__setattr__(self, "name", f"{self.type}_{self.graph.next_type_id()}")
 
@@ -168,15 +173,17 @@
         # https://spec.graphql.org/draft/#sel-GAJTBAABABFj6D
         if name.startswith("__"):
             raise Exception(
                 f"type name {name} cannot start with `__`, it's reserved for introspection"
             )
         types[name] = self
 
-    def named(self, name: str) -> "typedef":
+    def named(self, name: str, validate=True) -> "typedef":
+        if validate:
+            validate_name(name)
         ret = self.replace(name=name)
         ret.register_name()
         return ret
 
     def describe(self, description: str) -> "typedef":
         return self.replace(description=description)
 
@@ -310,23 +317,29 @@
 
 #
 # Type constraints
 
 TYPE_CONSTRAINT = "__type_constraint_name"
 
 
-def constraint(name: Optional[str] = None):
+def constraint(name: Optional[str] = None, **kwargs):
     # Additional constraint on type: Validation keyword.
     # Field to be manually set on the serialization.
     return field(
-        kw_only=True, default=None, metadata={SKIP: True, TYPE_CONSTRAINT: name or True}
+        kw_only=True,
+        default=None,
+        metadata={SKIP: True, TYPE_CONSTRAINT: name or True},
+        **kwargs,
     )
 
 
-def with_constraints(cls):
+Cls = TypeVar("Cls", bound=typedef)
+
+
+def with_constraints(cls: Type[Cls]) -> Type[Cls]:
     if not hasattr(cls, "__attrs_attrs__"):
         raise Exception(
             "@with_constraints decorator requires class to have attribute '__attrs_attrs__'"
         )
     if not issubclass(cls, typedef):
         raise Exception("@with_constraints decorator requires a subclass of 'typedef'")
 
@@ -494,14 +507,24 @@
     return string().format("phone")
 
 
 def enum(variants: List[str]) -> string:
     return string().enum(variants)
 
 
+@with_constraints
+@frozen
+class file(typedef):
+    _min: Optional[int] = constraint("minSize")
+    _max: Optional[int] = constraint("maxSize")
+    _allow: Optional[Tuple[str, ...]] = constraint(
+        "mimeTypes", converter=lambda v: v and tuple(v)
+    )
+
+
 def validate_struct_props(instance, attribute, props):
     for tpe in props.values():
         if not isinstance(tpe, typedef) and not isinstance(tpe, NodeProxy):
             raise Exception(
                 f"expected typedef or NodeProxy, got {type(tpe).__name__}: {props}"
             )
 
@@ -766,14 +789,15 @@
 def gen(out: typedef, mat: Materializer, **kwargs) -> func:
     return func(struct(), out, mat, **kwargs)
 
 
 # single instance
 def named(name: str, define: Callable[[], typedef]) -> TypeNode:
     defined = find(name)
+    validate_name(name)
     if defined is not None:
         return defined
     else:
         return define().named(name)
 
 
 def proxy(name: str) -> NodeProxy:
```

### Comparing `typegraph-0.1.8/typegraph/utils/attrs.py` & `typegraph-0.1.9/typegraph/utils/attrs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import attrs
 from attrs import Attribute, field
 
 SKIP = "asdict_skip"
```

### Comparing `typegraph-0.1.8/typegraph/utils/loaders.py` & `typegraph-0.1.9/typegraph/utils/loaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
+# Copyright Metatype OÜ, licensed under the Mozilla Public License Version 2.0.
+# SPDX-License-Identifier: MPL-2.0
 
 import importlib
 import json
 import pkgutil
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import List
 
 import attrs
 from attrs import define
 from frozendict import frozendict
 
+from typegraph import version
 from typegraph.graph.typegraph import TypeGraph
 
 
 # TDM is: typegraph definition module, defining one or more typegraphs
 @define
 class LoadedTdm:
     path: str
@@ -63,20 +65,29 @@
         if isinstance(obj, TypeGraph):
             ret.append(obj)
     return ret
 
 
 def cmd():
     parser = ArgumentParser()
-    parser.add_argument("module")
+    parser.add_argument("module", nargs="?")
     parser.add_argument("--pretty", action="store_true")
+    parser.add_argument("--version", action="store_true")
     # TODO option: output file
 
     args = parser.parse_args()
 
+    if args.version:
+        print(version)
+        return
+
+    if args.module is None:
+        print("No module specified")
+        return
+
     tgs = import_file(args.module)
 
     class JSONEncoder(json.JSONEncoder):
         def default(self, o):
             if attrs.has(o):
                 return attrs.asdict(o)
             if isinstance(o, frozendict):
```

### Comparing `typegraph-0.1.8/PKG-INFO` & `typegraph-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: typegraph
-Version: 0.1.8
-Summary: The low-code API platform for developers. Build modular APIs with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
+Version: 0.1.9
+Summary: Open source, low-code backend platform for developers — build modular APIs with zero-trust and serverless deployment, no matter where and how (legacy) systems are.
 Home-page: https://metatype.dev
-License: ELv2
+License: MPL-2.0
 Keywords: api,composition,typesystem,graphql,ecosystem
 Author: Metatype Contributors
 Author-email: support@metatype.dev
 Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

