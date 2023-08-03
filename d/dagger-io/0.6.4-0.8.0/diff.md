# Comparing `tmp/dagger_io-0.6.4.tar.gz` & `tmp/dagger_io-0.8.0.tar.gz`

## Comparing `dagger_io-0.6.4.tar` & `dagger_io-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,59 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/__main__.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/cli.py
--rw-r--r--   0        0        0    28643 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/codegen.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/config.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/connection.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/context.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/exceptions.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/py.typed
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/session.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/api/__init__.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/api/base.py
--rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/api/gen.py
--rw-r--r--   0        0        0    97080 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/api/gen_sync.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/engine/_version.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/engine/cli.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/engine/conn.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/engine/download.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/__main__.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/_commands.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/_context.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/_converter.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/_exceptions.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/_server.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/_util.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/server/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 dagger_io-0.6.4/dagger/transport/httpx.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.6.4/.gitignore
--rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.6.4/LICENSE
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 dagger_io-0.6.4/README.md
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 dagger_io-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 dagger_io-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dagger_io-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/client.rst
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/connection.rst
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/exceptions.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/_ext/dagger_ext.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_config.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_connection.py
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_exceptions.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_managers.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_codegen/__init__.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_codegen/cli.py
+-rw-r--r--   0        0        0    28844 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_codegen/generator.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/_version.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/conn.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/download.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/progress.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/session.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/__init__.py
+-rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_core.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_guards.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_session.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/conn.py
+-rw-r--r--   0        0        0    92472 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/gen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_transport/__init__.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_transport/httpx.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/__main__.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_commands.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_context.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_converter.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_exceptions.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_server.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_util.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_codegen.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_connection_errors.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_execute_errors.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_inputs.py
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_integration.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_response.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/engine/test_cli.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/engine/test_download.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.8.0/.gitignore
+-rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 dagger_io-0.8.0/README.md
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 dagger_io-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 dagger_io-0.8.0/PKG-INFO
```

### Comparing `dagger_io-0.6.4/dagger/codegen.py` & `dagger_io-0.8.0/src/dagger/_codegen/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,14 @@
             return t.name
 
 
 @dataclass
 class Context:
     """Shared state during execution."""
 
-    sync: bool
-    """Sync or async client."""
-
     id_map: IDMap
     """Map to convert ids (custom scalars) to corresponding types."""
 
     id_query_map: IDQueryMap
     """Map to convert types to ids."""
 
     simple_objects_map: SimpleObjectsMap
@@ -174,40 +171,38 @@
     @joiner
     def render_body(self, t: _H) -> Iterator[str]:
         if t.description:
             yield from wrap(doc(t.description))
 
 
 @joiner
-def generate(
-    schema: GraphQLSchema,
-    sync: bool = False,  # noqa: FBT001, FBT002
-) -> Iterator[str]:
+def generate(schema: GraphQLSchema) -> Iterator[str]:
     """Code generation main function."""
     yield textwrap.dedent(
         """\
         # Code generated by dagger. DO NOT EDIT.
 
-        import warnings
+        import warnings  # noqa: F401
         from collections.abc import Callable, Sequence
         from dataclasses import dataclass
         from typing import Optional
 
-        from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
+        from ._core import Arg, Root
+        from ._guards import typecheck
+        from .base import Enum, Input, Scalar, Type
         """,
     )
 
     # Pre-create handy maps to make handler code simpler.
     id_map = create_id_map(schema.type_map)
     id_query_map = create_id_query_map(id_map, schema.type_map)
     simple_objects_map = create_simple_objects_map(schema.type_map)
 
     # shared state between all handler instances
     ctx = Context(
-        sync=sync,
         id_map=id_map,
         id_query_map=id_query_map,
         simple_objects_map=simple_objects_map,
     )
 
     handlers: tuple[Handler, ...] = (
         Scalar(ctx),
@@ -503,16 +498,15 @@
         self.graphql = graphql
 
         self.name = format_name(name)
         self.named_type = get_named_type(graphql.type)
 
         # On object type fields, don't replace ID scalar with object
         # only if field name is `id` and the corresponding type is different
-        # from the output type (e.g., `file(id: FileID) -> File`, but also
-        # `with_rootfs(id: Directory) -> Container`).
+        # from the output type (e.g., `file(id: FileID) -> File`).
         id_map = ctx.id_map
         if (
             name == "id"
             and is_custom_scalar_type(graphql.type)
             and self.named_type.name in id_map
             and parent
             and get_named_type(parent.graphql.type).name == id_map[self.named_type.name]
@@ -576,18 +570,21 @@
     ) -> None:
         self.ctx = ctx
         self.graphql_name = name
         self.graphql = field
 
         self.name = format_name(name)
         self.named_type = get_named_type(field.type)
-        self.args = sorted(
-            (_InputField(ctx, *args, parent=self) for args in field.args.items()),
-            key=attrgetter("has_default"),
-        )
+
+        self.required_args = []
+        self.default_args = []
+        for args in field.args.items():
+            arg = _InputField(ctx, *args, parent=self)
+            (self.default_args if arg.has_default else self.required_args).append(arg)
+        self.args = self.required_args + self.default_args
         self.description = field.description
 
         self.is_custom_scalar = is_custom_scalar_type(field.type)
         self.is_leaf = is_output_leaf_type(field.type)
         self.is_exec = self.is_leaf
         self.type = format_output_type(field.type).replace("Query", "Client")
         self.parent_name = get_named_type(parent).name
@@ -632,15 +629,15 @@
             "@typecheck",
             self.func_signature(),
             indent(self.func_body()),
         )
 
         # convenience to await any object that has a sync method
         # without having to call it explicitly
-        if not self.ctx.sync and self.is_leaf and self.name == "sync":
+        if self.is_leaf and self.name == "sync":
             yield from (
                 "",
                 "def __await__(self):",
                 indent("return self.sync().__await__()"),
             )
 
         if self.name == "id":
@@ -655,20 +652,27 @@
                     "",
                     "@classmethod",
                     "def _from_id_query_field(cls):",
                     indent(f'return "{self.id_query_field}"'),
                 )
 
     def func_signature(self) -> str:
-        params = ", ".join(chain(("self",), (a.as_param() for a in self.args)))
+        params = ", ".join(
+            chain(
+                ("self",),
+                (a.as_param() for a in self.required_args),
+                ("*",) if self.default_args else (),
+                (a.as_param() for a in self.default_args),
+            )
+        )
         # arbitrary heuristic to force trailing comma in long signatures
         if len(params) > 40:  # noqa: PLR2004
             params = f"{params},"
         sig = f"def {self.name}({params}) -> {self.type}:"
-        if self.is_exec and not self.ctx.sync:
+        if self.is_exec:
             sig = f"async {sig}"
         # Add quotes around types that haven't been defined yet (forward references).
         if self.ctx.remaining:
             sig = re.sub(rf"\b({'|'.join(self.ctx.remaining)})\b", r'"\1"', sig)
         return sig
 
     @joiner
@@ -698,29 +702,31 @@
             yield "_args = ["
             yield from (indent(arg.as_arg()) for arg in self.args)
             yield "]"
 
         yield f'_ctx = self._select("{self.graphql_name}", _args)'
 
         if self.is_exec:
-            exec_ = "_ctx.execute_sync" if self.ctx.sync else "await _ctx.execute"
             if self.convert_id:
                 if _field := self.id_query_field:
-                    yield f"_id = {exec_}({self.named_type.name})"
-                    yield f'_ctx = self._root_select("{_field}", [Arg("id", _id)])'
+                    yield f"_id = await _ctx.execute({self.named_type.name})"
+                    yield (
+                        f'_ctx = Client.from_context(_ctx)._select("{_field}",'
+                        ' [Arg("id", _id)])'
+                    )
                     yield f"return {self.type}(_ctx)"
                 else:
-                    yield f"{exec_}()"
+                    yield "await _ctx.execute()"
                     yield "return self"
             else:
                 if slots := self.sub_select_slots:
                     target = self.named_type.name
                     kwargs = ", ".join(s.as_kwarg() for s in slots)
                     yield f"_ctx = {target}(_ctx)._select_multiple({kwargs},)"
-                yield f"return {exec_}({self.type})"
+                yield f"return await _ctx.execute({self.type})"
         else:
             yield f"return {self.type}(_ctx)"
 
     def func_doc(self) -> str:
         def _out():
             if self.description:
                 yield (textwrap.fill(line) for line in self.description.splitlines())
```

### Comparing `dagger_io-0.6.4/dagger/config.py` & `dagger_io-0.8.0/src/dagger/_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 from dataclasses import dataclass, field
 from os import PathLike
 
-import httpx
+from rich.console import Console
 
 
-@dataclass
+@dataclass(slots=True, kw_only=True)
 class Config:
     """Options for connecting to the Dagger engine.
 
     Parameters
     ----------
     workdir:
         The host workdir loaded into dagger.
@@ -26,23 +26,14 @@
     """
 
     workdir: PathLike[str] | str = ""
     config_path: PathLike[str] | str = ""
     log_output: typing.TextIO | None = None
     timeout: int = 10
     execute_timeout: int | float | None = None
-
-
-@dataclass(kw_only=True)
-class ConnectParams:
-    """Options for making a session connection. For internal use only."""
-
-    port: int
-    session_token: str
-    url: httpx.URL = field(init=False)
+    console: Console = field(init=False)
 
     def __post_init__(self):
-        self.port = int(self.port)
-        if self.port < 1:
-            msg = f"Invalid port value: {self.port}"
-            raise ValueError(msg)
-        self.url = httpx.URL(f"http://127.0.0.1:{self.port}/query")
+        self.console = Console(
+            file=self.log_output,
+            stderr=True,
+        )
```

### Comparing `dagger_io-0.6.4/dagger/connection.py` & `dagger_io-0.8.0/src/dagger/_connection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+import logging
 import warnings
 
-from dagger import Client, Config, SyncClient
+from gql.client import AsyncClientSession
 
-from .context import ResourceManager, SyncResourceManager
-from .engine import Engine
-from .session import Session
+from dagger import Client, Config, QueryError, VersionMismatch
 
+from ._engine._version import CLI_VERSION
+from ._engine.conn import Engine
+from ._engine.progress import Progress
+from ._managers import ResourceManager
+from .client._session import Session
 
-class Connection(ResourceManager, SyncResourceManager):
-    """
-    Connect to a Dagger Engine.
+logger = logging.getLogger(__name__)
+
+
+class Connection(ResourceManager):
+    """Connect to a Dagger Engine.
 
     Example::
 
         async def main():
             async with dagger.Connection() as client:
                 ctr = client.container().from_("alpine")
 
+
     You can stream the logs from the engine to see progress::
 
         import sys
         import anyio
         import dagger
 
         async def main():
@@ -35,26 +42,41 @@
 
         anyio.run(main)
     """
 
     def __init__(self, config: Config | None = None) -> None:
         super().__init__()
         self.cfg = config or Config()
+        self._progress = Progress(self.cfg.console)
+        self._engine = Engine(self.cfg, self._progress)
 
-    async def __aenter__(self) -> Client:
+    async def start(self) -> AsyncClientSession:
         async with self.get_stack() as stack:
-            conn = await stack.enter_async_context(Engine(self.cfg))
+            progress = await stack.enter_async_context(self._progress)
+            conn = await stack.enter_async_context(self._engine)
+
+            progress.update("Establishing connection to Engine")
             session = await stack.enter_async_context(Session(conn, self.cfg))
-        return Client.from_session(session)
 
-    def __enter__(self) -> SyncClient:
-        warnings.warn(
-            "The synchronous API is deprecated and will be removed in a future"
-            " release. See https://github.com/dagger/dagger/issues/5192"
-            " for more information.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        with self.get_sync_stack() as stack:
-            conn = stack.enter_context(Engine(self.cfg))
-            session = stack.enter_context(Session(conn, self.cfg))
-        return SyncClient.from_session(session)
+            # If log_output is set, we don't need to show any more progress.
+            if self.cfg.log_output:
+                progress.stop()
+            else:
+                progress.update("Running pipelines")
+
+            return session
+
+    async def aclose(self) -> None:
+        await self.stack.aclose()
+
+    async def __aenter__(self):
+        client = Client.from_session(await self.start())
+
+        try:
+            if not await client.check_version_compatibility(CLI_VERSION) and (
+                msg := self._engine.version_mismatch_msg
+            ):
+                warnings.warn(msg, VersionMismatch, stacklevel=2)
+        except QueryError as e:
+            logger.warning("Failed to check Dagger engine version compatibility: %s", e)
+
+        return client
```

### Comparing `dagger_io-0.6.4/dagger/context.py` & `dagger_io-0.8.0/src/dagger/_managers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# TODO: Rename this file managers.py
 import contextlib
 import typing
 
 from typing_extensions import Self
 
 
 class ResourceManager(contextlib.AbstractAsyncContextManager):
```

### Comparing `dagger_io-0.6.4/dagger/exceptions.py` & `dagger_io-0.8.0/src/dagger/_exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from typing import Any
 
 import cattrs
 import graphql
 from gql.transport.exceptions import TransportQueryError
 
 
+class VersionMismatch(Warning):
+    """Dagger CLI version doesn't match required version."""
+
+
 class DaggerError(Exception):
     """Base exception for all Dagger exceptions."""
 
 
 class ProvisionError(DaggerError):
     """Error while provisioning the Dagger engine."""
 
@@ -60,19 +64,19 @@
 
     line: int
     column: int
 
 
 @dataclass
 class QueryErrorValue:
-    """Error value returned by the API."""
+    """An error value returned by the API."""
 
     message: str
-    locations: list[QueryErrorLocation]
-    path: list[str]
+    locations: list[QueryErrorLocation] | None
+    path: list[str] | None
     extensions: dict[str, Any] = field(default_factory=dict)
 
     def __str__(self) -> str:
         return self.message
 
 
 class QueryError(ClientError):
@@ -93,55 +97,100 @@
         return super().__new__(new_type)
 
     def __init__(self, errors: list[QueryErrorValue], query: graphql.DocumentNode):
         if not errors:
             msg = "Errors list is empty"
             raise ValueError(msg)
         super().__init__(errors[0])
-        self.errors = errors
+        self.errors: list[QueryErrorValue] = errors
         self.query = query
 
-    @classmethod
-    def from_transport(cls, exc: TransportQueryError, query: graphql.DocumentNode):
-        """Create instance from a gql exception."""
-        try:
-            errors = cattrs.structure(exc.errors, list[QueryErrorValue])
-        except (TypeError, KeyError, ValueError):
-            return None
-        return QueryError(errors, query) if errors else None
-
     def debug_query(self):
-        """Return GraphQL query for debugging purposes."""
+        """Return GraphQL query for debugging purposes.
+
+        Example::
+
+            try:
+                await ctr
+            except dagger.QueryError as e:
+                print(e.debug_query())
+        """
         lines = graphql.print_ast(self.query).splitlines()
         # count number of digits from line count
         pad = len(str(len(lines)))
         locations = {loc.line: loc.column for loc in self.errors[0].locations}
         res = []
         for nr, line in enumerate(lines, start=1):
             # prepend line number
             res.append(f"{{:{pad}d}}: {{}}".format(nr, line))
             if nr in locations:
                 # add caret below line, pointing to start of error
                 res.append(" " * (pad + 1 + locations[nr]) + "^")
         return "\n".join(res)
 
 
+def _query_error_from_transport(exc: TransportQueryError, query: graphql.DocumentNode):
+    """Create instance from a gql exception."""
+    try:
+        errors = cattrs.structure(exc.errors, list[QueryErrorValue])
+    except (TypeError, KeyError, ValueError):
+        return None
+    return QueryError(errors, query) if errors else None
+
+
 class ExecError(QueryError):
-    """API error from an exec operation."""
+    """API error from an exec operation.
+
+    Attributes
+    ----------
+    command:
+        The command that was executed.
+    message:
+        The error message.
+    exit_code:
+        The exit code of the command.
+    stdout:
+        The stdout of the command.
+    stderr:
+        The stderr of the command.
+    """
 
     _type = "EXEC_ERROR"
 
+    command: list[str]
+    message: str
+    exit_code: int
+    stdout: str
+    stderr: str
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         error: QueryErrorValue = self.args[0]
         ext = error.extensions
-        self.command: list[str] = ext["cmd"]
+        self.command = ext["cmd"]
         self.message = error.message
-        self.exit_code: int = ext["exitCode"]
-        self.stdout: str = ext["stdout"]
-        self.stderr: str = ext["stderr"]
+        self.exit_code = ext["exitCode"]
+        self.stdout = ext["stdout"]
+        self.stderr = ext["stderr"]
 
     def __str__(self):
+        """Prints the error message with stdout and stderr."""
         # As a default when just printing the error, include the stdout
         # and stderr for visibility
         return f"{self.message}\nStdout:\n{self.stdout}\nStderr:\n{self.stderr}"
+
+
+__all__ = [
+    "VersionMismatch",
+    "DaggerError",
+    "ProvisionError",
+    "DownloadError",
+    "SessionError",
+    "ClientError",
+    "ClientConnectionError",
+    "TransportError",
+    "ExecuteTimeoutError",
+    "InvalidQueryError",
+    "QueryError",
+    "ExecError",
+]
```

### Comparing `dagger_io-0.6.4/dagger/log.py` & `dagger_io-0.8.0/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.4/dagger/session.py` & `dagger_io-0.8.0/src/dagger/client/_session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,80 @@
-import contextlib
 import logging
-from typing import TypeAlias, TypeVar
+from dataclasses import dataclass, field
 
 import httpx
-from gql.client import AsyncClientSession, SyncClientSession
+from gql.client import AsyncClientSession
 from gql.client import Client as GraphQLClient
-from gql.transport import AsyncTransport, Transport
 from gql.transport.exceptions import (
     TransportProtocolError,
     TransportQueryError,
     TransportServerError,
 )
 
-from dagger.exceptions import ClientConnectionError
+import dagger
+from dagger._managers import ResourceManager
 
-from .config import Config, ConnectParams
-from .context import ResourceManager, SyncResourceManager
-from .transport.httpx import HTTPXAsyncTransport, HTTPXTransport
+from ._transport.httpx import HTTPXAsyncTransport
 
 logger = logging.getLogger(__name__)
 
 
-_T = TypeVar("_T")
+@dataclass(slots=True, kw_only=True)
+class ConnectParams:
+    """Options for making a session connection. For internal use only."""
+
+    port: int
+    session_token: str
+    url: httpx.URL = field(init=False)
+
+    def __post_init__(self):
+        self.port = int(self.port)
+        if self.port < 1:
+            msg = f"Invalid port value: {self.port}"
+            raise ValueError(msg)
+        self.url = httpx.URL(f"http://127.0.0.1:{self.port}/query")
 
 
-ClientSession: TypeAlias = AsyncClientSession | SyncClientSession
-
-
-class Session(ResourceManager, SyncResourceManager):
+class Session(ResourceManager):
     """Establish a GraphQL client connection to the engine."""
 
-    def __init__(self, conn: ConnectParams, cfg: Config):
+    def __init__(self, conn: ConnectParams, cfg: dagger.Config):
         super().__init__()
         self.conn = conn
         self.cfg = cfg
 
-    def make_transport(self) -> AsyncTransport:
-        return self._make_transport(HTTPXAsyncTransport)
-
-    def make_sync_transport(self) -> Transport:
-        return self._make_transport(HTTPXTransport)
-
-    def _make_transport(self, cls: type[_T]) -> _T:
-        return cls(
+    async def __aenter__(self) -> AsyncClientSession:
+        transport = HTTPXAsyncTransport(
             self.conn.url,
             timeout=self.cfg.execute_timeout,
             auth=(self.conn.session_token, ""),
         )
-
-    def make_graphql_client(
-        self,
-        transport: AsyncTransport | Transport,
-    ) -> GraphQLClient:
-        return GraphQLClient(
+        client = GraphQLClient(
             transport=transport,
             fetch_schema_from_transport=True,
             # Don't timeout with the event loop. This setting is only for AsyncTransport
             # and uses `asyncio.wait_for` which is not compatible with other event loops
             # (e.g., Trio). Catching the TimeoutError would also be more complicated,
             # unless *gql* adopts AnyIO in the future, but still only on *async*.
             # Since we're using *httpx* as the transport for both *async* and *sync*, we
             # can use that project's Timeout instead for both environments.
             execute_timeout=None,
         )
-
-    async def __aenter__(self) -> AsyncClientSession:
-        transport = self.make_transport()
-        client = self.make_graphql_client(transport)
-
         async with self.get_stack() as stack:
-            # TODO: handle cancellation, retries and timeout (self.cfg.timeout)
-            with self._handle_connection():
+            try:
                 session = await stack.enter_async_context(client)
-
-        return session
-
-    def __enter__(self) -> SyncClientSession:
-        transport = self.make_sync_transport()
-        client = self.make_graphql_client(transport)
-
-        with self.get_sync_stack() as stack, self._handle_connection():
-            # TODO: handle cancellation, retries and timeout (self.cfg.timeout)
-            session = stack.enter_context(client)
-
-        return session
-
-    @contextlib.contextmanager
-    def _handle_connection(self):
-        # Reduces duplication when handling errors, between sync and async.
-        try:
-            yield
-        except httpx.RequestError as e:
-            msg = f"Could not make request: {e}"
-            raise ClientConnectionError(msg) from e
-        except (TransportProtocolError, TransportServerError) as e:
-            msg = f"Got unexpected response from engine: {e}"
-            raise ClientConnectionError(msg) from e
-        except TransportQueryError as e:
-            # Only query during connection is the introspection query
-            # for building the schema.
-            msg = str(e)
-            # Extract only the error message.
-            if e.errors and "message" in e.errors[0]:
-                msg = e.errors[0]["message"].strip()
-            msg = f"Failed to build schema from introspection query: {msg}"
-            raise ClientConnectionError(msg) from e
+            except httpx.RequestError as e:
+                msg = f"Could not make request: {e}"
+                raise dagger.ClientConnectionError(msg) from e
+            except (TransportProtocolError, TransportServerError) as e:
+                msg = f"Got unexpected response from engine: {e}"
+                raise dagger.ClientConnectionError(msg) from e
+            except TransportQueryError as e:
+                # Only query during connection is the introspection query
+                # for building the schema.
+                msg = str(e)
+                # Extract only the error message.
+                if e.errors and "message" in e.errors[0]:
+                    msg = e.errors[0]["message"].strip()
+                msg = f"Failed to build schema from introspection query: {msg}"
+                raise dagger.ClientConnectionError(msg) from e
+            return session
```

### Comparing `dagger_io-0.6.4/dagger/api/gen.py` & `dagger_io-0.8.0/src/dagger/client/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Code generated by dagger. DO NOT EDIT.
 
-import warnings
+import warnings  # noqa: F401
 from collections.abc import Callable, Sequence
 from dataclasses import dataclass
 from typing import Optional
 
-from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
+from ._core import Arg, Root
+from ._guards import typecheck
+from .base import Enum, Input, Scalar, Type
 
 
 class CacheID(Scalar):
     """A global cache volume identifier."""
 
 
 class ContainerID(Scalar):
@@ -147,14 +149,15 @@
 class Container(Type):
     """An OCI-compatible container, also known as a docker container."""
 
     @typecheck
     def build(
         self,
         context: "Directory",
+        *,
         dockerfile: Optional[str] = None,
         build_args: Optional[Sequence[BuildArg]] = None,
         target: Optional[str] = None,
         secrets: Optional[Sequence["Secret"]] = None,
     ) -> "Container":
         """Initializes this container from a Dockerfile build.
 
@@ -221,14 +224,15 @@
         ]
         _ctx = self._select("directory", _args)
         return Directory(_ctx)
 
     @typecheck
     async def endpoint(
         self,
+        *,
         port: Optional[int] = None,
         scheme: Optional[str] = None,
     ) -> str:
         """Retrieves an endpoint that clients can use to reach this container.
 
         If no port is specified, the first exposed port is used. If none exist
         an error is returned.
@@ -326,101 +330,18 @@
         _ctx = EnvVariable(_ctx)._select_multiple(
             _name="name",
             _value="value",
         )
         return await _ctx.execute(list[EnvVariable])
 
     @typecheck
-    def exec(
-        self,
-        args: Optional[Sequence[str]] = None,
-        stdin: Optional[str] = None,
-        redirect_stdout: Optional[str] = None,
-        redirect_stderr: Optional[str] = None,
-        experimental_privileged_nesting: Optional[bool] = None,
-    ) -> "Container":
-        """Retrieves this container after executing the specified command inside
-        it.
-
-        .. deprecated::
-            Replaced by :py:meth:`with_exec`.
-
-        Parameters
-        ----------
-        args:
-            Command to run instead of the container's default command (e.g.,
-            ["run", "main.go"]).
-        stdin:
-            Content to write to the command's standard input before closing
-            (e.g., "Hello world").
-        redirect_stdout:
-            Redirect the command's standard output to a file in the container
-            (e.g., "/tmp/stdout").
-        redirect_stderr:
-            Redirect the command's standard error to a file in the container
-            (e.g., "/tmp/stderr").
-        experimental_privileged_nesting:
-            Provide dagger access to the executed command.
-            Do not use this option unless you trust the command being
-            executed.
-            The command being executed WILL BE GRANTED FULL ACCESS TO YOUR
-            HOST FILESYSTEM.
-        """
-        warnings.warn(
-            'Method "exec" is deprecated: Replaced by "with_exec".',
-            DeprecationWarning,
-            stacklevel=4,
-        )
-        _args = [
-            Arg("args", args, None),
-            Arg("stdin", stdin, None),
-            Arg("redirectStdout", redirect_stdout, None),
-            Arg("redirectStderr", redirect_stderr, None),
-            Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
-        ]
-        _ctx = self._select("exec", _args)
-        return Container(_ctx)
-
-    @typecheck
-    async def exit_code(self) -> int:
-        """Exit code of the last executed command. Zero means success.
-
-        Will execute default command if none is set, or error if there's no
-        default.
-
-        .. deprecated::
-            Use :py:meth:`sync` instead.
-
-        Returns
-        -------
-        int
-            The `Int` scalar type represents non-fractional signed whole
-            numeric values. Int can represent values between -(2^31) and 2^31
-            - 1.
-
-        Raises
-        ------
-        ExecuteTimeoutError
-            If the time to execute the query exceeds the configured timeout.
-        QueryError
-            If the API returns an error.
-        """
-        warnings.warn(
-            'Method "exit_code" is deprecated: Use "sync" instead.',
-            DeprecationWarning,
-            stacklevel=4,
-        )
-        _args: list[Arg] = []
-        _ctx = self._select("exitCode", _args)
-        return await _ctx.execute(int)
-
-    @typecheck
     async def export(
         self,
         path: str,
+        *,
         platform_variants: Optional[Sequence["Container"]] = None,
         forced_compression: Optional[ImageLayerCompression] = None,
         media_types: Optional[ImageMediaTypes] = None,
     ) -> bool:
         """Writes the container as an OCI tarball to the destination file path on
         the host for the specified platform variants.
 
@@ -523,30 +444,14 @@
         _args = [
             Arg("address", address),
         ]
         _ctx = self._select("from", _args)
         return Container(_ctx)
 
     @typecheck
-    def fs(self) -> "Directory":
-        """Retrieves this container's root filesystem. Mounts are not included.
-
-        .. deprecated::
-            Replaced by :py:meth:`rootfs`.
-        """
-        warnings.warn(
-            'Method "fs" is deprecated: Replaced by "rootfs".',
-            DeprecationWarning,
-            stacklevel=4,
-        )
-        _args: list[Arg] = []
-        _ctx = self._select("fs", _args)
-        return Directory(_ctx)
-
-    @typecheck
     async def hostname(self) -> str:
         """Retrieves a hostname which can be used by clients to reach this
         container.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
 
@@ -624,14 +529,15 @@
         _ctx = self._select("imageRef", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
     def import_(
         self,
         source: "File",
+        *,
         tag: Optional[str] = None,
     ) -> "Container":
         """Reads the container from an OCI tarball.
 
         NOTE: this involves unpacking the tarball to an OCI store on the host
         at
         $XDG_CACHE_DIR/dagger/oci. This directory can be removed whenever you
@@ -710,14 +616,15 @@
         _ctx = self._select("mounts", _args)
         return await _ctx.execute(list[str])
 
     @typecheck
     def pipeline(
         self,
         name: str,
+        *,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Container":
         """Creates a named sub-pipeline
 
         Parameters
         ----------
@@ -758,14 +665,15 @@
         _ctx = self._select("platform", _args)
         return await _ctx.execute(Platform)
 
     @typecheck
     async def publish(
         self,
         address: str,
+        *,
         platform_variants: Optional[Sequence["Container"]] = None,
         forced_compression: Optional[ImageLayerCompression] = None,
         media_types: Optional[ImageMediaTypes] = None,
     ) -> str:
         """Publishes this container as a new image to the specified address.
 
         Publish returns a fully qualified ref.
@@ -889,15 +797,15 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sync", _args)
         _id = await _ctx.execute(ContainerID)
-        _ctx = self._root_select("container", [Arg("id", _id)])
+        _ctx = Client.from_context(_ctx)._select("container", [Arg("id", _id)])
         return Container(_ctx)
 
     def __await__(self):
         return self.sync().__await__()
 
     @typecheck
     async def user(self) -> Optional[str]:
@@ -920,14 +828,15 @@
         _args: list[Arg] = []
         _ctx = self._select("user", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
     def with_default_args(
         self,
+        *,
         args: Optional[Sequence[str]] = None,
     ) -> "Container":
         """Configures default arguments for future commands.
 
         Parameters
         ----------
         args:
@@ -941,14 +850,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_directory(
         self,
         path: str,
         directory: "Directory",
+        *,
         exclude: Optional[Sequence[str]] = None,
         include: Optional[Sequence[str]] = None,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a directory written at the given path.
 
         Parameters
@@ -995,14 +905,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_env_variable(
         self,
         name: str,
         value: str,
+        *,
         expand: Optional[bool] = None,
     ) -> "Container":
         """Retrieves this container plus the given environment variable.
 
         Parameters
         ----------
         name:
@@ -1022,14 +933,15 @@
         _ctx = self._select("withEnvVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_exec(
         self,
         args: Sequence[str],
+        *,
         skip_entrypoint: Optional[bool] = None,
         stdin: Optional[str] = None,
         redirect_stdout: Optional[str] = None,
         redirect_stderr: Optional[str] = None,
         experimental_privileged_nesting: Optional[bool] = None,
         insecure_root_capabilities: Optional[bool] = None,
     ) -> "Container":
@@ -1081,14 +993,15 @@
         _ctx = self._select("withExec", _args)
         return Container(_ctx)
 
     @typecheck
     def with_exposed_port(
         self,
         port: int,
+        *,
         protocol: Optional[NetworkProtocol] = None,
         description: Optional[str] = None,
     ) -> "Container":
         """Expose a network port.
 
         Exposed ports serve two purposes:
           - For health checks and introspection, when running services
@@ -1111,36 +1024,19 @@
             Arg("protocol", protocol, None),
             Arg("description", description, None),
         ]
         _ctx = self._select("withExposedPort", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_fs(self, id: "Directory") -> "Container":
-        """Initializes this container from this DirectoryID.
-
-        .. deprecated::
-            Replaced by :py:meth:`with_rootfs`.
-        """
-        warnings.warn(
-            'Method "with_fs" is deprecated: Replaced by "with_rootfs".',
-            DeprecationWarning,
-            stacklevel=4,
-        )
-        _args = [
-            Arg("id", id),
-        ]
-        _ctx = self._select("withFS", _args)
-        return Container(_ctx)
-
-    @typecheck
     def with_file(
         self,
         path: str,
         source: "File",
+        *,
         permissions: Optional[int] = None,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus the contents of the given file copied to
         the given path.
 
         Parameters
@@ -1197,14 +1093,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_mounted_cache(
         self,
         path: str,
         cache: CacheVolume,
+        *,
         source: Optional["Directory"] = None,
         sharing: Optional[CacheSharingMode] = None,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a cache volume mounted at the given
         path.
 
@@ -1240,14 +1137,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_mounted_directory(
         self,
         path: str,
         source: "Directory",
+        *,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a directory mounted at the given path.
 
         Parameters
         ----------
         path:
@@ -1269,14 +1167,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_mounted_file(
         self,
         path: str,
         source: "File",
+        *,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a file mounted at the given path.
 
         Parameters
         ----------
         path:
@@ -1298,14 +1197,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_mounted_secret(
         self,
         path: str,
         source: "Secret",
+        *,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a secret mounted into a file at the
         given path.
 
         Parameters
         ----------
@@ -1343,14 +1243,15 @@
         _ctx = self._select("withMountedTemp", _args)
         return Container(_ctx)
 
     @typecheck
     def with_new_file(
         self,
         path: str,
+        *,
         contents: Optional[str] = None,
         permissions: Optional[int] = None,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a new file written at the given path.
 
         Parameters
@@ -1403,18 +1304,18 @@
             Arg("username", username),
             Arg("secret", secret),
         ]
         _ctx = self._select("withRegistryAuth", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_rootfs(self, id: "Directory") -> "Container":
+    def with_rootfs(self, directory: "Directory") -> "Container":
         """Initializes this container from this DirectoryID."""
         _args = [
-            Arg("id", id),
+            Arg("directory", directory),
         ]
         _ctx = self._select("withRootfs", _args)
         return Container(_ctx)
 
     @typecheck
     def with_secret_variable(self, name: str, secret: "Secret") -> "Container":
         """Retrieves this container plus an env variable containing the given
@@ -1466,14 +1367,15 @@
         return Container(_ctx)
 
     @typecheck
     def with_unix_socket(
         self,
         path: str,
         source: "Socket",
+        *,
         owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a socket forwarded to the given Unix
         socket path.
 
         Parameters
         ----------
@@ -1540,14 +1442,15 @@
         _ctx = self._select("withoutEnvVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def without_exposed_port(
         self,
         port: int,
+        *,
         protocol: Optional[NetworkProtocol] = None,
     ) -> "Container":
         """Unexpose a previously exposed port.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
 
@@ -1704,14 +1607,15 @@
         ]
         _ctx = self._select("directory", _args)
         return Directory(_ctx)
 
     @typecheck
     def docker_build(
         self,
+        *,
         dockerfile: Optional[str] = None,
         platform: Optional[Platform] = None,
         build_args: Optional[Sequence[BuildArg]] = None,
         target: Optional[str] = None,
         secrets: Optional[Sequence["Secret"]] = None,
     ) -> Container:
         """Builds a new Docker container from this directory.
@@ -1738,15 +1642,15 @@
             Arg("target", target, None),
             Arg("secrets", secrets, None),
         ]
         _ctx = self._select("dockerBuild", _args)
         return Container(_ctx)
 
     @typecheck
-    async def entries(self, path: Optional[str] = None) -> list[str]:
+    async def entries(self, *, path: Optional[str] = None) -> list[str]:
         """Returns a list of files and directories at the given path.
 
         Parameters
         ----------
         path:
             Location of the directory to look at (e.g., "/src").
 
@@ -1844,14 +1748,15 @@
     def _from_id_query_field(cls):
         return "directory"
 
     @typecheck
     def pipeline(
         self,
         name: str,
+        *,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Directory":
         """Creates a named sub-pipeline
 
         Parameters
         ----------
@@ -1880,25 +1785,26 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sync", _args)
         _id = await _ctx.execute(DirectoryID)
-        _ctx = self._root_select("directory", [Arg("id", _id)])
+        _ctx = Client.from_context(_ctx)._select("directory", [Arg("id", _id)])
         return Directory(_ctx)
 
     def __await__(self):
         return self.sync().__await__()
 
     @typecheck
     def with_directory(
         self,
         path: str,
         directory: "Directory",
+        *,
         exclude: Optional[Sequence[str]] = None,
         include: Optional[Sequence[str]] = None,
     ) -> "Directory":
         """Retrieves this directory plus a directory written at the given path.
 
         Parameters
         ----------
@@ -1923,14 +1829,15 @@
         return Directory(_ctx)
 
     @typecheck
     def with_file(
         self,
         path: str,
         source: "File",
+        *,
         permissions: Optional[int] = None,
     ) -> "Directory":
         """Retrieves this directory plus the contents of the given file copied to
         the given path.
 
         Parameters
         ----------
@@ -1950,14 +1857,15 @@
         _ctx = self._select("withFile", _args)
         return Directory(_ctx)
 
     @typecheck
     def with_new_directory(
         self,
         path: str,
+        *,
         permissions: Optional[int] = None,
     ) -> "Directory":
         """Retrieves this directory plus a new directory created at the given
         path.
 
         Parameters
         ----------
@@ -1975,14 +1883,15 @@
         return Directory(_ctx)
 
     @typecheck
     def with_new_file(
         self,
         path: str,
         contents: str,
+        *,
         permissions: Optional[int] = None,
     ) -> "Directory":
         """Retrieves this directory plus a new file written at the given path.
 
         Parameters
         ----------
         path:
@@ -2142,14 +2051,15 @@
         _ctx = self._select("contents", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def export(
         self,
         path: str,
+        *,
         allow_parent_dir_path: Optional[bool] = None,
     ) -> bool:
         """Writes the file to a file path on the host.
 
         Parameters
         ----------
         path:
@@ -2207,32 +2117,14 @@
         return FileID
 
     @classmethod
     def _from_id_query_field(cls):
         return "file"
 
     @typecheck
-    def secret(self) -> "Secret":
-        """Retrieves a secret referencing the contents of this file.
-
-        .. deprecated::
-            insecure, leaves secret in cache. Superseded by
-            :py:meth:`set_secret`
-        """
-        warnings.warn(
-            'Method "secret" is deprecated: insecure, leaves secret in cache.'
-            ' Superseded by "set_secret"',
-            DeprecationWarning,
-            stacklevel=4,
-        )
-        _args: list[Arg] = []
-        _ctx = self._select("secret", _args)
-        return Secret(_ctx)
-
-    @typecheck
     async def size(self) -> int:
         """Gets the size of the file, in bytes.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
@@ -2260,15 +2152,15 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sync", _args)
         _id = await _ctx.execute(FileID)
-        _ctx = self._root_select("file", [Arg("id", _id)])
+        _ctx = Client.from_context(_ctx)._select("file", [Arg("id", _id)])
         return File(_ctx)
 
     def __await__(self):
         return self.sync().__await__()
 
     @typecheck
     def with_timestamps(self, timestamp: int) -> "File":
@@ -2297,14 +2189,15 @@
 
 class GitRef(Type):
     """A git ref (tag, branch or commit)."""
 
     @typecheck
     def tree(
         self,
+        *,
         ssh_known_hosts: Optional[str] = None,
         ssh_auth_socket: Optional["Socket"] = None,
     ) -> Directory:
         """The filesystem tree at this ref."""
         _args = [
             Arg("sshKnownHosts", ssh_known_hosts, None),
             Arg("sshAuthSocket", ssh_auth_socket, None),
@@ -2366,14 +2259,15 @@
 class Host(Type):
     """Information about the host execution environment."""
 
     @typecheck
     def directory(
         self,
         path: str,
+        *,
         exclude: Optional[Sequence[str]] = None,
         include: Optional[Sequence[str]] = None,
     ) -> Directory:
         """Accesses a directory on the host.
 
         Parameters
         ----------
@@ -2391,29 +2285,14 @@
             Arg("exclude", exclude, None),
             Arg("include", include, None),
         ]
         _ctx = self._select("directory", _args)
         return Directory(_ctx)
 
     @typecheck
-    def env_variable(self, name: str) -> "HostVariable":
-        """Accesses an environment variable on the host.
-
-        Parameters
-        ----------
-        name:
-            Name of the environment variable (e.g., "PATH").
-        """
-        _args = [
-            Arg("name", name),
-        ]
-        _ctx = self._select("envVariable", _args)
-        return HostVariable(_ctx)
-
-    @typecheck
     def file(self, path: str) -> File:
         """Accesses a file on the host.
 
         Parameters
         ----------
         path:
             Location of the file to retrieve (e.g., "README.md").
@@ -2421,102 +2300,47 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("file", _args)
         return File(_ctx)
 
     @typecheck
-    def unix_socket(self, path: str) -> "Socket":
-        """Accesses a Unix socket on the host.
+    def set_secret_file(self, name: str, path: str) -> "Secret":
+        """Sets a secret given a user-defined name and the file path on the host,
+        and returns the secret.
+        The file is limited to a size of 512000 bytes.
 
         Parameters
         ----------
+        name:
+            The user defined name for this secret.
         path:
-            Location of the Unix socket (e.g., "/var/run/docker.sock").
+            Location of the file to set as a secret.
         """
         _args = [
+            Arg("name", name),
             Arg("path", path),
         ]
-        _ctx = self._select("unixSocket", _args)
-        return Socket(_ctx)
+        _ctx = self._select("setSecretFile", _args)
+        return Secret(_ctx)
 
     @typecheck
-    def workdir(
-        self,
-        exclude: Optional[Sequence[str]] = None,
-        include: Optional[Sequence[str]] = None,
-    ) -> Directory:
-        """Retrieves the current working directory on the host.
-
-        .. deprecated::
-            Use :py:meth:`directory` with path set to '.' instead.
+    def unix_socket(self, path: str) -> "Socket":
+        """Accesses a Unix socket on the host.
 
         Parameters
         ----------
-        exclude:
-            Exclude artifacts that match the given pattern (e.g.,
-            ["node_modules/", ".git*"]).
-        include:
-            Include only artifacts that match the given pattern (e.g.,
-            ["app/", "package.*"]).
+        path:
+            Location of the Unix socket (e.g., "/var/run/docker.sock").
         """
-        warnings.warn(
-            'Method "workdir" is deprecated: Use "directory" with path set to \'.\''
-            " instead.",
-            DeprecationWarning,
-            stacklevel=4,
-        )
         _args = [
-            Arg("exclude", exclude, None),
-            Arg("include", include, None),
+            Arg("path", path),
         ]
-        _ctx = self._select("workdir", _args)
-        return Directory(_ctx)
-
-
-class HostVariable(Type):
-    """An environment variable on the host environment."""
-
-    @typecheck
-    def secret(self) -> "Secret":
-        """A secret referencing the value of this variable.
-
-        .. deprecated::
-            been superseded by :py:meth:`set_secret`
-        """
-        warnings.warn(
-            'Method "secret" is deprecated: been superseded by "set_secret"',
-            DeprecationWarning,
-            stacklevel=4,
-        )
-        _args: list[Arg] = []
-        _ctx = self._select("secret", _args)
-        return Secret(_ctx)
-
-    @typecheck
-    async def value(self) -> str:
-        """The value of this variable.
-
-        Returns
-        -------
-        str
-            The `String` scalar type represents textual data, represented as
-            UTF-8 character sequences. The String type is most often used by
-            GraphQL to represent free-form human-readable text.
-
-        Raises
-        ------
-        ExecuteTimeoutError
-            If the time to execute the query exceeds the configured timeout.
-        QueryError
-            If the API returns an error.
-        """
-        _args: list[Arg] = []
-        _ctx = self._select("value", _args)
-        return await _ctx.execute(str)
+        _ctx = self._select("unixSocket", _args)
+        return Socket(_ctx)
 
 
 class Label(Type):
     """A simple key value object that represents a label."""
 
     __slots__ = (
         "_name",
@@ -2966,16 +2790,45 @@
         _args = [
             Arg("key", key),
         ]
         _ctx = self._select("cacheVolume", _args)
         return CacheVolume(_ctx)
 
     @typecheck
+    async def check_version_compatibility(self, version: str) -> bool:
+        """Checks if the current Dagger Engine is compatible with an SDK's
+        required version.
+
+        Parameters
+        ----------
+        version:
+            The SDK's required version.
+
+        Returns
+        -------
+        bool
+            The `Boolean` scalar type represents `true` or `false`.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args = [
+            Arg("version", version),
+        ]
+        _ctx = self._select("checkVersionCompatibility", _args)
+        return await _ctx.execute(bool)
+
+    @typecheck
     def container(
         self,
+        *,
         id: Optional[ContainerID] = None,
         platform: Optional[Platform] = None,
     ) -> Container:
         """Loads a container from ID.
 
         Null ID returns an empty container (scratch).
         Optional platform argument initializes new containers to execute and
@@ -3008,15 +2861,19 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("defaultPlatform", _args)
         return await _ctx.execute(Platform)
 
     @typecheck
-    def directory(self, id: Optional[DirectoryID] = None) -> Directory:
+    def directory(
+        self,
+        *,
+        id: Optional[DirectoryID] = None,
+    ) -> Directory:
         """Load a directory by ID. No argument produces an empty directory."""
         _args = [
             Arg("id", id, None),
         ]
         _ctx = self._select("directory", _args)
         return Directory(_ctx)
 
@@ -3029,14 +2886,15 @@
         _ctx = self._select("file", _args)
         return File(_ctx)
 
     @typecheck
     def git(
         self,
         url: str,
+        *,
         keep_git_dir: Optional[bool] = None,
         experimental_service_host: Optional[Container] = None,
     ) -> GitRepository:
         """Queries a git repository.
 
         Parameters
         ----------
@@ -3065,14 +2923,15 @@
         _ctx = self._select("host", _args)
         return Host(_ctx)
 
     @typecheck
     def http(
         self,
         url: str,
+        *,
         experimental_service_host: Optional[Container] = None,
     ) -> File:
         """Returns a file containing an http remote url content.
 
         Parameters
         ----------
         url:
@@ -3087,14 +2946,15 @@
         _ctx = self._select("http", _args)
         return File(_ctx)
 
     @typecheck
     def pipeline(
         self,
         name: str,
+        *,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Client":
         """Creates a named sub-pipeline.
 
         Parameters
         ----------
@@ -3110,25 +2970,26 @@
             Arg("description", description, None),
             Arg("labels", labels, None),
         ]
         _ctx = self._select("pipeline", _args)
         return Client(_ctx)
 
     @typecheck
-    def project(self, id: Optional[ProjectID] = None) -> Project:
+    def project(self, *, id: Optional[ProjectID] = None) -> Project:
         """Load a project from ID."""
         _args = [
             Arg("id", id, None),
         ]
         _ctx = self._select("project", _args)
         return Project(_ctx)
 
     @typecheck
     def project_command(
         self,
+        *,
         id: Optional[ProjectCommandID] = None,
     ) -> ProjectCommand:
         """Load a project command from ID."""
         _args = [
             Arg("id", id, None),
         ]
         _ctx = self._select("projectCommand", _args)
@@ -3160,15 +3021,15 @@
             Arg("name", name),
             Arg("plaintext", plaintext),
         ]
         _ctx = self._select("setSecret", _args)
         return Secret(_ctx)
 
     @typecheck
-    def socket(self, id: Optional[SocketID] = None) -> "Socket":
+    def socket(self, *, id: Optional[SocketID] = None) -> "Socket":
         """Loads a socket by its ID."""
         _args = [
             Arg("id", id, None),
         ]
         _ctx = self._select("socket", _args)
         return Socket(_ctx)
 
@@ -3285,15 +3146,14 @@
     "DirectoryID",
     "EnvVariable",
     "File",
     "FileID",
     "GitRef",
     "GitRepository",
     "Host",
-    "HostVariable",
     "ImageLayerCompression",
     "ImageMediaTypes",
     "Label",
     "NetworkProtocol",
     "PipelineLabel",
     "Platform",
     "Port",
```

### Comparing `dagger_io-0.6.4/dagger/engine/cli.py` & `dagger_io-0.8.0/src/dagger/_engine/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 import subprocess
 import time
 from importlib import metadata
 from pathlib import Path
 
 import dagger
-from dagger.config import ConnectParams
-from dagger.context import SyncResourceManager
-from dagger.exceptions import SessionError
+from dagger._managers import SyncResourceManager
+
+from .conn import ConnectParams
 
 logger = logging.getLogger(__name__)
 
 
 OS_ETXTBSY = 26
 
 
@@ -26,37 +26,33 @@
 class CLISession(SyncResourceManager):
     """Start an engine session with a provided CLI path."""
 
     def __init__(self, cfg: dagger.Config, path: str) -> None:
         super().__init__()
         self.cfg = cfg
         self.path = path
-        # no constructor param intentional
-        self.is_async = True
 
     def __enter__(self) -> ConnectParams:
         with self.get_sync_stack() as stack:
             try:
                 proc = self._start()
             except (OSError, ValueError, TypeError) as e:
-                raise SessionError(e) from e
+                raise dagger.SessionError(e) from e
             stack.push(proc)
             conn = self._get_conn(proc)
         return conn
 
     def _start(self) -> subprocess.Popen:
         args = [
             self.path,
             "session",
             "--label",
             "dagger.io/sdk.name:python",
             "--label",
             f"dagger.io/sdk.version:{get_sdk_version()}",
-            "--label",
-            f"dagger.io/sdk.async:{str(self.is_async).lower()}",
         ]
         if self.cfg.workdir:
             args.extend(["--workdir", str(Path(self.cfg.workdir).absolute())])
         if self.cfg.config_path:
             args.extend(["--project", str(Path(self.cfg.config_path).absolute())])
 
         # Retry starting if "text file busy" error is hit. That error can happen
@@ -82,15 +78,15 @@
                     raise
                 logger.warning("file busy, retrying in 0.1 seconds...")
                 time.sleep(0.1)
             else:
                 return proc
 
         msg = "CLI busy"
-        raise SessionError(msg)
+        raise dagger.SessionError(msg)
 
     def _get_conn(self, proc: subprocess.Popen) -> ConnectParams:
         # TODO: implement engine session timeout (self.cfg.engine_timeout?)
         assert proc.stdout
         conn = proc.stdout.readline()
 
         # Check if subprocess exited with an error
@@ -103,18 +99,18 @@
 
             msg = str(exc)
             detail = err or out
             if detail and detail.strip():
                 # `msg` ends in a period, just append
                 msg = f"{msg} {detail.strip()}"
 
-            raise SessionError(msg)
+            raise dagger.SessionError(msg)
 
         if not conn:
             msg = "No connection params"
-            raise SessionError(msg)
+            raise dagger.SessionError(msg)
 
         try:
             return ConnectParams(**json.loads(conn))
         except (ValueError, TypeError) as e:
             msg = f"Invalid connection params: {conn}"
-            raise SessionError(msg) from e
+            raise dagger.SessionError(msg) from e
```

### Comparing `dagger_io-0.6.4/dagger/engine/conn.py` & `dagger_io-0.8.0/src/dagger/_engine/conn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 import logging
 import os
 
 import anyio
 
-from dagger.config import Config, ConnectParams
-from dagger.context import SyncResourceManager
-from dagger.exceptions import ProvisionError
+import dagger
+from dagger._managers import SyncResourceManager
+from dagger.client._session import ConnectParams
 
-from .cli import CLISession
+from ._version import CLI_VERSION
 from .download import Downloader
+from .progress import Progress
+from .session import CLISession
 
 logger = logging.getLogger(__name__)
 
 
 class Engine(SyncResourceManager):
     """Start engine, provisioning if needed."""
 
-    def __init__(self, cfg: Config) -> None:
+    def __init__(self, cfg: dagger.Config, progress: Progress) -> None:
         super().__init__()
         self.cfg = cfg
-        self.is_async = True
+        self.progress = progress
+        self.version_mismatch_msg = ""
 
     def from_env(self) -> ConnectParams | None:
         if not (port := os.environ.get("DAGGER_SESSION_PORT")):
             return None
         if not (token := os.environ.get("DAGGER_SESSION_TOKEN")):
             msg = "DAGGER_SESSION_TOKEN must be set when using DAGGER_SESSION_PORT"
-            raise ProvisionError(msg)
+            raise dagger.ProvisionError(msg)
         try:
             return ConnectParams(port=int(port), session_token=token)
         except ValueError as e:
             # only port is validated
             msg = f"Invalid DAGGER_SESSION_PORT: {port}"
-            raise ProvisionError(msg) from e
+            raise dagger.ProvisionError(msg) from e
 
     def from_cli(self) -> ConnectParams:
-        cli_bin = os.environ.get("_EXPERIMENTAL_DAGGER_CLI_BIN") or Downloader().get()
-        cli_session = CLISession(self.cfg, cli_bin)
-        cli_session.is_async = self.is_async
+        # Only start progress if we are provisioning, not on active sessions
+        # like `dagger run`.
+        self.progress.start("Provisioning engine")
+
+        if cli_bin := os.environ.get("_EXPERIMENTAL_DAGGER_CLI_BIN"):
+            # Warn if engine version is incompatible only if an explicit
+            # binary is provided. It's already done by the API when
+            # using the TUI, and using the Downloader ensures the correct
+            # version is used.
+            self.version_mismatch_msg = (
+                f'Dagger CLI version mismatch (required {CLI_VERSION}): "{cli_bin}"'
+            )
+        else:
+            cli_bin = Downloader().get(self.progress)
+
+        self.progress.update("Creating new Engine session")
         with self.get_sync_stack() as stack:
-            return stack.enter_context(cli_session)
+            return stack.enter_context(CLISession(self.cfg, cli_bin))
 
     def start(self) -> ConnectParams:
         return self.from_env() or self.from_cli()
 
-    def __enter__(self) -> ConnectParams:
-        self.is_async = False
-        return self.start()
-
     async def __aenter__(self) -> ConnectParams:
-        self.is_async = True
-        # TODO: Create proper async provisioning later.
-        # This is just to support sync faster.
+        # TODO: Create proper async provisioning.
         return await anyio.to_thread.run_sync(self.start)
 
     async def __aexit__(self, *exc_details) -> None:
-        # TODO: Create proper async provisioning later.
-        # This is just to support sync faster.
+        # TODO: Create proper async provisioning.
         await anyio.to_thread.run_sync(self.__exit__, *exc_details)
```

### Comparing `dagger_io-0.6.4/dagger/engine/download.py` & `dagger_io-0.8.0/src/dagger/_engine/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from collections.abc import Iterator
 from pathlib import Path, PurePath
 from typing import IO
 
 import httpx
 import platformdirs
 
-from dagger.context import SyncResourceManager
-from dagger.exceptions import DownloadError
+import dagger
+from dagger._engine.progress import Progress
+from dagger._managers import SyncResourceManager
 
 from ._version import CLI_VERSION
 
 DEFAULT_CLI_HOST = "dl.dagger.io"
 
 logger = logging.getLogger(__name__)
 
@@ -143,66 +144,67 @@
         # See https://github.com/dagger/dagger/issues/3963
         env = os.environ.get("XDG_CACHE_HOME", "").strip()
         path = Path(env).expanduser() if env else platformdirs.user_cache_path()
         cache_dir = path / "dagger"
         cache_dir.mkdir(mode=0o700, parents=True, exist_ok=True)
         return cache_dir
 
-    def get(self) -> str:
+    def get(self, progress: Progress) -> str:
         """Download CLI to cache and return its path."""
         cli_bin_path = self.cache_dir / f"{self.CLI_BIN_PREFIX}{self.version}"
 
         if self.platform.os == "windows":
             cli_bin_path = cli_bin_path.with_suffix(".exe")
 
         if not cli_bin_path.exists():
+            progress.update("Downloading dagger CLI")
             cli_bin_path = self._download(cli_bin_path)
 
         # garbage collection of old binaries
         for file in self.cache_dir.glob(f"{self.CLI_BIN_PREFIX}*"):
             if file != cli_bin_path:
                 file.unlink()
 
         return str(cli_bin_path.absolute())
 
     def _download(self, path: Path) -> Path:
         try:
             expected_hash = self.expected_checksum()
         except httpx.HTTPError as e:
             msg = f"Failed to download checksums from {self.checksum_url}: {e}"
-            raise DownloadError(msg) from e
+            raise dagger.DownloadError(msg) from e
 
         with TempFile(f"temp-{self.CLI_BIN_PREFIX}", self.cache_dir) as tmp_bin:
             try:
                 actual_hash = self.extract_cli_archive(tmp_bin)
             except httpx.HTTPError as e:
                 msg = f"Failed to download archive from {self.archive_url}: {e}"
-                raise DownloadError(msg) from e
+                raise dagger.DownloadError(msg) from e
 
             if actual_hash != expected_hash:
                 msg = (
                     f"Downloaded CLI binary checksum ({actual_hash}) "
                     f"does not match expected checksum ({expected_hash})"
                 )
-                raise DownloadError(msg)
+                raise dagger.DownloadError(msg)
 
         tmp_bin_path = Path(tmp_bin.name)
         tmp_bin_path.chmod(0o700)
         return tmp_bin_path.rename(path)
 
     def expected_checksum(self) -> str:
         archive_name = self.archive_name
         with httpx.stream("GET", self.checksum_url, follow_redirects=True) as r:
             r.raise_for_status()
             for line in r.iter_lines():
                 checksum, filename = line.split()
                 if filename == archive_name:
                     return checksum
         msg = "Could not find checksum for archive"
-        raise DownloadError(msg)
+        raise dagger.DownloadError(msg)
 
     def extract_cli_archive(self, dest: IO[bytes]) -> str:
         """
         Download the CLI archive and extract the binary into the provided dest.
 
         Returns
         -------
@@ -232,19 +234,19 @@
                 if member.name == "dagger" and (file := tar.extractfile(member)):
                     yield file
                     # ensure the entire body is read into the hash
                     reader.readall()
                     break
             else:
                 msg = "There is no item named 'dagger' in the archive"
-                raise DownloadError(msg)
+                raise dagger.DownloadError(msg)
 
     @contextlib.contextmanager
     def _extract_from_zip(self, reader: StreamReader) -> Iterator[IO[bytes]]:
         # TODO: extract from stream instead of loading archive into memory
         with zipfile.ZipFile(reader.getbuffer()) as zar:
             try:
                 with zar.open("dagger.exe") as file:
                     yield file
             except KeyError as e:
                 msg = "There is no item named 'dagger.exe' in the archive"
-                raise DownloadError(msg) from e
+                raise dagger.DownloadError(msg) from e
```

### Comparing `dagger_io-0.6.4/dagger/server/_commands.py` & `dagger_io-0.8.0/src/dagger/server/_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import strawberry
 from strawberry.extensions import FieldExtension
 from strawberry.extensions.field_extension import AsyncExtensionResolver
 from strawberry.field import StrawberryField
 from strawberry.types import Info
 from strawberry.utils.await_maybe import await_maybe
 
-from dagger.api.base import Type as DaggerType
-from dagger.api.gen import Client
+from dagger.client.base import Type as DaggerType
+from dagger.client.gen import Client
 
 from ._exceptions import BadParameterError, SchemaValidationError
 from ._util import has_resolver
 
 _dummy_types = {}
```

### Comparing `dagger_io-0.6.4/dagger/server/_converter.py` & `dagger_io-0.8.0/src/dagger/server/_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 import anyio
 from cattrs import Converter
 from cattrs.gen import make_dict_structure_fn, make_dict_unstructure_fn, override
 from cattrs.preconf.json import make_converter
 from strawberry.type import has_object_definition
 
-from dagger.api.base import (
-    Type as BaseType,
-)
-from dagger.api.base import (
+from dagger.client._guards import (
     is_id_type_subclass,
 )
+from dagger.client.base import (
+    Type as BaseType,
+)
 
 from ._context import Context
 from ._util import has_resolver
 
 T = TypeVar("T")
 Type = TypeVar("Type", bound=BaseType)
```

### Comparing `dagger_io-0.6.4/dagger/server/_server.py` & `dagger_io-0.8.0/src/dagger/server/_server.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.4/dagger/server/cli.py` & `dagger_io-0.8.0/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.4/dagger/transport/httpx.py` & `dagger_io-0.8.0/src/dagger/client/_transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.4/LICENSE` & `dagger_io-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.4/README.md` & `dagger_io-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -101,17 +101,17 @@
 
 This library is maintained with [Hatch](https://hatch.pypa.io/).
 
 The following commands are available:
 - `hatch run test`: Run tests.
 - `hatch run fmt`: Re-format code following common styling conventions.
 - `hatch run lint`: Check for linting violations.
-- `hatch run generate`: Regenerate API client after changes to the codegen.
 - `hatch run typing:check`: Run the type checker.
-- `hatch run docs:build`: Build reference docs locally (check with `(cd docs/_build && python -m http.server)`).
+- `hatch run docs:build`: Build reference docs locally
+- `hatch run docs:preview`: Build and serve reference docs (defaults to localhost:8000)
 
 ### Engine changes
 
 Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet.
 
 The simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :
```

### Comparing `dagger_io-0.6.4/pyproject.toml` & `dagger_io-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,20 +33,18 @@
     # TODO: replace next two lines with the following when gql version 3.5.0 is released
     # "gql[httpx]>=3.5.0",
     "gql>=3.4.0",
     "httpx>=0.23.1",
     "beartype>=0.11.0",
     "platformdirs>=2.6.2",
     "typing_extensions>=4.4.0",
+    "rich>=10.11.0",
 ]
 
 [project.optional-dependencies]
-cli = [
-    "typer[all]>=0.6.1",
-]
 server = [
     "typer[all]>=0.6.1",
     "strawberry-graphql>=0.187.0",
 ]
 
 [project.urls]
 "Homepage" = "https://dagger.io"
@@ -57,35 +55,38 @@
 "Community" = "https://discord.gg/ufnyBtc8uY"
 "Twitter" = "https://twitter.com/dagger_io"
 
 [tool.hatch.version]
 source = "vcs"
 fallback-version = "0.0.0"
 
-[tool.hatch.build]
+[tool.hatch.build.targets.sdist]
+only-include = [
+    "src",
+    "tests",
+    "docs",
+    "CHANGELOG.md",
+]
+
+[tool.hatch.build.targets.wheel]
 packages = ["src/dagger"]
 
 [tool.hatch.envs.default]
-features = ["cli", "server"]
+features = ["server"]
 dependencies = [
     "black>=22.3.0",
     "ruff>=0.0.218",
     "pytest>=7.2.0",
     "pytest-mock>=3.10.0",
     "pytest-subprocess>=1.4.2",
     "pytest-lazy-fixture>=0.6.3",
     "pytest-httpx>=0.21.3",
 ]
 
 [tool.hatch.envs.default.scripts]
-generate = [
-    "python -m dagger generate --output src/dagger/api/gen.py",
-    "python -m dagger generate --output src/dagger/api/gen_sync.py --sync",
-    "black --preview src/dagger/api/gen*.py",
-]
 fmt = [
     "ruff --fix-only -e {args:. ../../docs/current}",
     "black --preview {args:. ../../docs/current}",
 ]
 lint = [
     "ruff check {args:. ../../docs/current}",
     "black --preview --check {args:. ../../docs/current}",
@@ -195,16 +196,17 @@
 [tool.ruff.isort]
 known-first-party = ["dagger"]
 
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = ["typer.Option"]
 
 [tool.ruff.per-file-ignores]
-"./examples/*" = ["T201"]
-"./src/dagger/api/gen*.py" = [
+"./docs/*" = ["D1"]
+"./experimental/*" = ["D1", "T201"]
+"./src/dagger/client/gen.py" = [
     # Not much control over field names and docs coming from the API.
     # Note: We could detect built-in shadowing like the reserved
     # keywords but these built-ins aren't being used in the generated
     # code so no need to bother.
     "A",
     "D",
     # Too hard to properly wrap long lines in codegen.
@@ -214,23 +216,25 @@
     # Too many arguments to function call.
     "PLR0913",
     # `Optional` is preferred over `| None` because of how
     # beartype handles forward references.
     "UP007",
 ]
 # Ignore built-in shadowing in test mocks.
-"./tests/api/test_inputs.py" = ["A", "ERA001"]
+"./tests/client/test_inputs.py" = ["A", "ERA001"]
 "./tests/*.py" = [
     # Ignore security issues in tests.
     "S",
     # Magic value comparison doesn't apply to tests.
     "PLR2004",
     # Allow more than one statement in pytest.raises.
     "PT012",
+    # No public interfaces.
+    "D1",
 ]
 # Allow some patterns to redefine imports in __init__.
-"__init__.py" = ["F401", "F403", "PLC0414"]
+"__init__.py" = ["I001", "F401", "F403", "PLC0414"]
 # Typer uses boolean parameters for the CLI. Let it.
 "./src/**/cli.py" = ["FBT"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
```

### Comparing `dagger_io-0.6.4/PKG-INFO` & `dagger_io-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.6.4
+Version: 0.8.0
 Summary: A client package for running Dagger pipelines in Python.
 Project-URL: Homepage, https://dagger.io
 Project-URL: Documentation, https://docs.dagger.io/sdk/python
 Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
 Project-URL: Tracker, https://github.com/dagger/dagger/issues
 Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
 Project-URL: Community, https://discord.gg/ufnyBtc8uY
@@ -28,17 +28,16 @@
 Requires-Dist: anyio>=3.6.2
 Requires-Dist: beartype>=0.11.0
 Requires-Dist: cattrs>=22.2.0
 Requires-Dist: gql>=3.4.0
 Requires-Dist: graphql-core>=3.2.3
 Requires-Dist: httpx>=0.23.1
 Requires-Dist: platformdirs>=2.6.2
+Requires-Dist: rich>=10.11.0
 Requires-Dist: typing-extensions>=4.4.0
-Provides-Extra: cli
-Requires-Dist: typer[all]>=0.6.1; extra == 'cli'
 Provides-Extra: server
 Requires-Dist: strawberry-graphql>=0.187.0; extra == 'server'
 Requires-Dist: typer[all]>=0.6.1; extra == 'server'
 Description-Content-Type: text/markdown
 
 # Dagger Python SDK
 
@@ -143,17 +142,17 @@
 
 This library is maintained with [Hatch](https://hatch.pypa.io/).
 
 The following commands are available:
 - `hatch run test`: Run tests.
 - `hatch run fmt`: Re-format code following common styling conventions.
 - `hatch run lint`: Check for linting violations.
-- `hatch run generate`: Regenerate API client after changes to the codegen.
 - `hatch run typing:check`: Run the type checker.
-- `hatch run docs:build`: Build reference docs locally (check with `(cd docs/_build && python -m http.server)`).
+- `hatch run docs:build`: Build reference docs locally
+- `hatch run docs:preview`: Build and serve reference docs (defaults to localhost:8000)
 
 ### Engine changes
 
 Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet.
 
 The simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :
```

