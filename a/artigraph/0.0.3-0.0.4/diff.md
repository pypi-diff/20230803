# Comparing `tmp/artigraph-0.0.3.tar.gz` & `tmp/artigraph-0.0.4.tar.gz`

## Comparing `artigraph-0.0.3.tar` & `artigraph-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,49 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/__init__.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/db.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/artifact.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/artifact_group.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/node.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/artifact.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/base.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/node.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/run.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/run_parameter.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/__init__.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/_core.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/numpy.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/pandas.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/polars.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/storage/__init__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/storage/_core.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/storage/aws.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 artigraph-0.0.3/README.md
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 artigraph-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 artigraph-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 artigraph-0.0.4/Untitled.ipynb
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/__init__.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/db.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/py.typed
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/__init__.py
+-rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/artifact.py
+-rw-r--r--   0        0        0    12490 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/artifact_model.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/node.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/__init__.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/artifact.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/base.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/node.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/run.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/__init__.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/core.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/datetime.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/json.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/numpy.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/pandas.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/polars.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/pyarrow.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/__init__.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/aws.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/core.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/file.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_db.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_storage.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_artifact.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_artifact_model.py
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_node.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_core.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_json.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_numpy.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_pandas.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_polars.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_pyarrow.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 artigraph-0.0.4/README.md
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 artigraph-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 artigraph-0.0.4/PKG-INFO
```

### Comparing `artigraph-0.0.3/src/artigraph/db.py` & `artigraph-0.0.4/src/artigraph/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,82 @@
 from contextlib import asynccontextmanager, contextmanager
 from contextvars import ContextVar
-from typing import (
-    AsyncContextManager,
-    AsyncIterator,
-    Callable,
-    ContextManager,
-    Iterator,
-    Literal,
-    overload,
-)
-
-from sqlalchemy import Engine
-from sqlalchemy.ext.asyncio import (
-    AsyncEngine,
-    AsyncSession,
-)
-from sqlalchemy.orm import Session
-
-_CURRENT_SYNC_ENGINE: ContextVar[Engine] = ContextVar("CURRENT_SYNC_ENGINE")
-_CURRENT_ASYNC_ENGINE: ContextVar[AsyncEngine] = ContextVar("CURRENT_ASYNC_ENGINE")
-_CURRENT_SYNC_SESSION: ContextVar[Session] = ContextVar("CURRENT_SYNC_SESSION")
-_CURRENT_ASYNC_SESSION: ContextVar[AsyncSession] = ContextVar("CURRENT_ASYNC_SESSION")
+from typing import Any, AsyncIterator, Callable, Iterator, TypeVar
+
+from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, async_sessionmaker
+
+E = TypeVar("E", bound=AsyncEngine)
+
+_CURRENT_ENGINE: ContextVar[AsyncEngine] = ContextVar("CURRENT_ASYNC_ENGINE")
+_CURRENT_SESSION: ContextVar[AsyncSession] = ContextVar("CURRENT_ASYNC_SESSION")
 
 
 @contextmanager
-def engine_context(engine: Engine | AsyncEngine) -> Iterator[None]:
+def engine_context(engine: E) -> Iterator[E]:
     """Define which engine to use in the context."""
     reset = set_engine(engine)
     try:
-        yield
+        yield engine
     finally:
         reset()
 
 
-def set_engine(engine: Engine | AsyncEngine) -> Callable[[], None]:
-    """Set the current engine."""
-    if isinstance(engine, Engine):
-        var = _CURRENT_SYNC_ENGINE
-    elif isinstance(engine, AsyncEngine):
-        var = _CURRENT_ASYNC_ENGINE
-    else:
-        msg = f"Unsupported engine type: {type(engine)}"
-        raise TypeError(msg)
-    token = var.set(engine)
-    return lambda: var.reset(token)
-
-
-@overload
-def enter_session(*, sync: Literal[True]) -> ContextManager[Session]:
-    ...
-
-
-@overload
-def enter_session(*, sync: Literal[False] = ...) -> AsyncContextManager[AsyncSession]:
-    ...
-
-
-def enter_session(
-    *, sync: bool = False
-) -> ContextManager[Session] | AsyncContextManager[AsyncSession]:
-    """A context manager for a database session."""
-    if sync:
-        return _sync_session_context()
-    else:
-        return _async_session_context()
+@asynccontextmanager
+async def session_context(**kwargs: Any) -> AsyncIterator[AsyncSession]:
+    """Define which session to use in the context."""
+    async with async_sessionmaker(get_engine(), **kwargs)() as session:
+        reset = set_session(session)
+        try:
+            yield session
+        finally:
+            reset()
 
 
-@contextmanager
-def _sync_session_context() -> Iterator[Session]:
-    """A context manager for a synchronous database session."""
+@asynccontextmanager
+async def current_session() -> AsyncIterator[AsyncSession]:
+    """A context manager for an asynchronous database session."""
     try:
-        session = _CURRENT_SYNC_SESSION.get()
+        session = get_session()
     except LookupError:
         pass
     else:
         yield session
         return
 
-    try:
-        engine = _CURRENT_SYNC_ENGINE.get()
-    except LookupError:
-        msg = "No current synchronous engine"
-        raise LookupError(msg) from None
-
-    with Session(engine) as session:
+    async with AsyncSession(get_engine()) as session:
         try:
             yield session
         except Exception:
-            session.rollback()
+            await session.rollback()
             raise
-        finally:
-            session.close()
 
 
-@asynccontextmanager
-async def _async_session_context() -> AsyncIterator[AsyncSession]:
-    """A context manager for an asynchronous database session."""
-    try:
-        session = _CURRENT_ASYNC_SESSION.get()
-    except LookupError:
-        pass
-    else:
-        yield session
-        return
+def set_engine(engine: AsyncEngine) -> Callable[[], None]:
+    """Set the current engine."""
+    var = _CURRENT_ENGINE
+    token = var.set(engine)
+    return lambda: var.reset(token)
+
 
+def get_engine() -> AsyncEngine:
+    """Get the current engine."""
     try:
-        engine = _CURRENT_ASYNC_ENGINE.get()
-    except LookupError:
+        return _CURRENT_ENGINE.get()
+    except LookupError:  # nocov
         msg = "No current asynchronous engine"
         raise LookupError(msg) from None
 
-    async with AsyncSession(engine) as session:
-        try:
-            yield session
-        except Exception:
-            await session.rollback()
-            raise
-        finally:
-            await session.close()
+
+def set_session(session: AsyncSession) -> Callable[[], None]:
+    """Set the current session."""
+    var = _CURRENT_SESSION
+    token = var.set(session)
+    return lambda: var.reset(token)
+
+
+def get_session() -> AsyncSession:
+    """Get the current session."""
+    try:
+        return _CURRENT_SESSION.get()
+    except LookupError:  # nocov
+        msg = "No current asynchronous session"
+        raise LookupError(msg) from None
```

### Comparing `artigraph-0.0.3/src/artigraph/serializer/_core.py` & `artigraph-0.0.4/src/artigraph/serializer/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,42 @@
 import logging
-import warnings
-from typing import Any, Protocol, TypedDict, TypeVar, runtime_checkable
+from abc import ABC, abstractmethod
+from inspect import isclass
+from typing import Any, Generic, Sequence, TypedDict, TypeVar
+
+from typing_extensions import Self
 
 T = TypeVar("T")
 S = TypeVar("S", bound="Serializer[Any]")
 
 WRAPPER_VERSION = 1
 SERIALIZERS_BY_TYPE: dict[type[Any], "Serializer[Any]"] = {}
 SERIALIZERS_BY_NAME: dict[str, "Serializer[Any]"] = {}
 
 logger = logging.getLogger(__name__)
 
 
 def get_serialize_by_name(name: str) -> "Serializer[Any]":
     """Get a serializer by name."""
-    if name not in SERIALIZERS_BY_NAME:
+    if name not in SERIALIZERS_BY_NAME:  # nocov
         msg = f"No serializer named {name!r}"
         raise ValueError(msg)
     return SERIALIZERS_BY_NAME[name]
 
 
 def get_serializer_by_type(value: type[T] | T) -> "Serializer[T]":
     """Get a serializer for a value."""
-    for cls in (value if isinstance(value, type) else value).mro():
+    for cls in (value if isclass(value) else type(value)).mro():
         if cls in SERIALIZERS_BY_TYPE:
             return SERIALIZERS_BY_TYPE[cls]
-    msg = f"No serializer exists for {value!r}"
-    raise ValueError(msg)
-
-
-def register_serializer(serializer: "Serializer") -> None:
-    """Register a serializer.
-
-    It's recommended that each serializer be defined and registerd in a separate module
-    so that users can select which serializers they want to use by importing the module.
-    Thus if a user does not import a serializer if will not be registered. This is
-    important for two reasons:
-
-    1. It allows users to avoid importing dependencies they don't need.
-    2. Serializers that supprt the same type will override each other - only the last one
-       registered will be used unless the user explicitly selects one.
-    """
-    if not isinstance(serializer, Serializer):
-        msg = f"{serializer} is not of Serializer"
-        raise ValueError(msg)
+    msg = f"No serializer exists for {value!r}"  # nocov
+    raise ValueError(msg)  # nocov
 
-    if type(serializer).__module__ in serializer.name:
-        warnings.warn(
-            "Serializer name contains 'module.__name__' which may change between "
-            "versions. Consider avoiding dynamic names",
-            UserWarning,
-            stacklevel=2,
-        )
 
-    if serializer.name in SERIALIZERS_BY_NAME:
-        msg = f"Serializer named {serializer.name!r} already registered."
-        raise ValueError(msg)
-    SERIALIZERS_BY_NAME[serializer.name] = serializer
-
-    for st in serializer.types if isinstance(serializer.types, tuple) else (serializer.types,):
-        if st in SERIALIZERS_BY_TYPE:
-            logger.debug("Overriding serializer for type %s with %s", st, serializer)
-        SERIALIZERS_BY_TYPE[st] = serializer
-
-
-@runtime_checkable
-class Serializer(Protocol[T]):
+class Serializer(ABC, Generic[T]):
     """A type of artifact that can be serialized to a string or bytes."""
 
     name: str
     """A globally unique name for this serializer.
 
     This will typically be of the form "library_name.SerializerName". You should avoid
     using dynamic values like `__name__` or `__qualname__` as these may change between
@@ -77,27 +44,88 @@
 
     The serializer name will be used to recover this class from a when deserializing
     artifacts so it must not change between versions of the library. If you need to
     change the name, you should create and register a subclass with the new name and
     deprecate the old one.
     """
 
-    types: type[T] | tuple[type[T], ...]
+    types: Sequence[type[T]]
     """The type or types of values that can be serialized."""
 
-    def __init__(self) -> None:
-        """Initialize the serializer."""
+    def register(self) -> Self:
+        """Register a serializer.
+
+        It's recommended that each serializer be defined and registerd in a separate module
+        so that users can select which serializers they want to use by importing the module.
+        Thus if a user does not import a serializer if will not be registered. This is
+        important for two reasons:
+
+        1. It allows users to avoid importing dependencies they don't need.
+        2. Serializers that supprt the same type will override each other - only the last one
+        registered will be used unless the user explicitly selects one.
+        """
+        if not isinstance(self, Serializer):  # nocov
+            msg = f"{self} is not of Serializer"
+            raise ValueError(msg)
+
+        if self.name in SERIALIZERS_BY_NAME:
+            msg = f"Serializer named {self.name!r} already registered."
+            raise ValueError(msg)
+        SERIALIZERS_BY_NAME[self.name] = self
+
+        for serializable_type in self.types:
+            if serializable_type not in SERIALIZERS_BY_TYPE:
+                SERIALIZERS_BY_TYPE[serializable_type] = self
+            else:
+                logger.debug(
+                    "Did not register %s for %s - %s already exists",
+                    self,
+                    serializable_type,
+                    SERIALIZERS_BY_TYPE[serializable_type],
+                )
+
+        return self
 
+    @abstractmethod
     def serialize(self, value: T, /) -> bytes:
         """Serialize a value to a string or bytes."""
+        raise NotImplementedError()  # nocov
 
+    @abstractmethod
     def deserialize(self, value: bytes, /) -> T:
         """Deserialize a string or bytes to a value."""
+        raise NotImplementedError()  # nocov
 
 
 class DataWrapper(TypedDict):
     """A wrapper for serialized data."""
 
     wrapper_version: int
     serializer_name: int
     data_encoding: str
     data: str
+
+
+class StringSerializer(Serializer[str]):
+    """A serializer for JSON."""
+
+    types = (str,)
+    name = "artigraph-string"
+
+    serialize = staticmethod(str.encode)  # type: ignore
+    deserialize = staticmethod(bytes.decode)  # type: ignore
+
+
+StringSerializer().register()
+
+
+class BytesSerializer(Serializer[bytes]):
+    """A serializer for JSON."""
+
+    types = (bytes,)
+    name = "artigraph-bytes"
+
+    serialize = staticmethod(lambda b: b)  # type: ignore
+    deserialize = staticmethod(lambda b: b)  # type: ignore
+
+
+BytesSerializer().register()
```

### Comparing `artigraph-0.0.3/src/artigraph/serializer/numpy.py` & `artigraph-0.0.4/src/artigraph/serializer/numpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 import numpy as np
 import pandas as pd
 
-from artigraph.serializer._core import register_serializer
-from artigraph.serializer.pandas import pandas_serializer
+from artigraph.serializer.core import Serializer
+from artigraph.serializer.pandas import dataframe_serializer
 
 NP_1D_SHAPE_LEN = 1
 NP_2D_SHAPE_LEN = 2
 
 
-class NumpySerializer:
+class ArraySerializer(Serializer[np.ndarray]):
     """A serializer for numpy arrays."""
 
-    types = np.ndarray
-    name = "artigraph.numpy"
+    types = (np.ndarray,)
+    name = "artigraph-numpy"
 
     @staticmethod
     def serialize(value: np.ndarray) -> bytes:
         """Serialize a numpy array."""
         if len(value.shape) == NP_1D_SHAPE_LEN:
-            pd_value = pd.Series(value)
+            pd_value = pd.DataFrame({"1darray": value})
         elif len(value.shape) == NP_2D_SHAPE_LEN:
             pd_value = pd.DataFrame(dict(enumerate(value.T)))
         else:
             msg = f"Can only serialize 1D or 2D arrays, not {value.shape}."
             raise ValueError(msg)
-        return pandas_serializer.serialize(pd_value)
+        return dataframe_serializer.serialize(pd_value)
 
     @staticmethod
     def deserialize(value: bytes) -> np.ndarray:
         """Deserialize a numpy array."""
-        pd_value = pandas_serializer.deserialize(value)
-        if isinstance(pd_value, pd.Series):
-            return pd_value.to_numpy()
-        elif isinstance(pd_value, pd.DataFrame):
-            return pd_value.values.T
-        else:
-            msg = f"Can only deserialize Series or DataFrame, not {type(pd_value)}."
-            raise ValueError(msg)
+        pd_value = dataframe_serializer.deserialize(value)
+        if "1darray" in pd_value.columns:
+            return pd_value["1darray"].to_numpy()
+        return pd_value.to_numpy()
 
 
-numpy_serializer = NumpySerializer()
+array_serializer = ArraySerializer().register()
 """A serializer for numpy arrays."""
-
-register_serializer(numpy_serializer)
```

### Comparing `artigraph-0.0.3/src/artigraph/serializer/polars.py` & `artigraph-0.0.4/src/artigraph/serializer/polars.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import polars as pl
-import pyarrow as pa
 
-from artigraph.serializer._core import register_serializer
+from artigraph.serializer.core import Serializer
+from artigraph.serializer.pyarrow import ArrowSerializer, parquet_serializer
 
 
-class PolarsSerializer:
+class DataFrameSerializer(Serializer[pl.DataFrame]):
     """A serializer for Polars dataframes."""
 
-    types = (pl.DataFrame, pl.Series)
-    name = "artigraph.polars"
+    types = (pl.DataFrame,)
 
-    @staticmethod
-    def serialize(value: pl.DataFrame | pl.Series) -> bytes:
+    def __init__(self, pyarrow_serializer: ArrowSerializer = parquet_serializer):
+        self.pyarrow_serializer = pyarrow_serializer
+        self.name = f"artigraph-polars-{pyarrow_serializer.name}"
+
+    def serialize(self, value: pl.DataFrame) -> bytes:
         """Serialize a Polars dataframe."""
-        pa_value = value.to_arrow()
-        return pa_value.serialize().to_buffer().to_pybytes()
+        return self.pyarrow_serializer.serialize(value.to_arrow())
 
-    @staticmethod
-    def deserialize(value: bytes) -> pl.DataFrame | pl.Series:
+    def deserialize(self, value: bytes) -> pl.DataFrame:
         """Deserialize a Polars dataframe."""
-        pa_value = pa.deserialize(value)
-        return pl.from_arrow(pa_value)
-
+        return pl.from_arrow(self.pyarrow_serializer.deserialize(value))  # type: ignore
 
-polars_serializer = PolarsSerializer()
-"""A serializer for Polars dataframes."""
 
-register_serializer(polars_serializer)
+dataframe_serializer = DataFrameSerializer().register()
+"""A serializer for Polars dataframes that uses the parquet file format."""
```

### Comparing `artigraph-0.0.3/src/artigraph/storage/aws.py` & `artigraph-0.0.4/src/artigraph/storage/aws.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,97 @@
 """S3 storage backend for Artigraph."""
 
 import hashlib
+from contextlib import contextmanager
 from contextvars import ContextVar
-from email import contentmanager
-from functools import partial
-from typing import Callable, TypeVar, cast
+from typing import Callable, Iterator, TypeVar, cast
 
-import boto3
-from anyio import from_thread
+from botocore.client import BaseClient
 from botocore.exceptions import ClientError
 from typing_extensions import ParamSpec
 
-from artigraph.storage._core import register_storage
+from artigraph.storage.core import Storage
+from artigraph.utils import run_in_thread, slugify
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
-_S3_CLIENT: ContextVar[boto3.client] = ContextVar("S3_CLIENT")
+_S3_CLIENT: ContextVar[BaseClient] = ContextVar("S3_CLIENT")
 
 
-def set_s3_client(client: boto3.client) -> None:
+def get_s3_client() -> BaseClient:
+    """Get the current S3 client."""
+    try:
+        return _S3_CLIENT.get()
+    except LookupError:  # nocov
+        msg = "No S3 client is currently set. Did you forget to use s3_client_context()?"
+        raise LookupError(msg) from None
+
+
+def set_s3_client(client: BaseClient) -> Callable[[], None]:
     """Set the current S3 client."""
     token = _S3_CLIENT.set(client)
     return lambda: _S3_CLIENT.reset(token)
 
 
-@contentmanager
-def s3_context(client: boto3.client) -> ContextVar[boto3.client]:
+@contextmanager
+def s3_client_context(client: BaseClient) -> Iterator[BaseClient]:
     """Set the current S3 client."""
     reset = set_s3_client(client)
     try:
-        yield
+        yield client
     finally:
         reset()
 
 
-class S3Storage:
+class S3Storage(Storage):
     """S3 storage backend for Artigraph."""
 
-    def __init__(self, bucket: str, prefix: str) -> None:
+    def __init__(self, bucket: str, prefix: str = "") -> None:
         """Initialize the storage backend."""
-        self.name = f"artigraph.s3.{bucket}.{prefix}"
+        self.name = slugify(f"artigraph-s3-{bucket}-{prefix}")
         self.bucket = bucket
         self.prefix = prefix
-        register_storage(self)
 
     async def create(self, value: bytes) -> str:
         """Create an S3 object and return is key."""
-        client = _S3_CLIENT.get()
+        client = get_s3_client()
 
         hashed_value = hashlib.sha512(value).hexdigest()
         key = f"{self.prefix}/{hashed_value}"
 
         # Only create the object if it doesn't already exist.
         try:
-            await _run_in_thread(client.head_object, Bucket=self.bucket, Key=key)
+            await run_in_thread(client.head_object, Bucket=self.bucket, Key=key)
         except ClientError as error:
-            if error.response["Error"]["Code"] != "NoSuchKey":
-                raise
-            await _run_in_thread(client.put_object, Bucket=self.bucket, Key=key, Body=value)
+            if error.response["Error"]["Code"] != "404":
+                raise  # nocov
+            await run_in_thread(client.put_object, Bucket=self.bucket, Key=key, Body=value)
 
         return key
 
     async def read(self, key: str) -> bytes:
         """Read an S3 object."""
-        client = _S3_CLIENT.get()
-        response = await _run_in_thread(client.get_object, Bucket=self.bucket, Key=key)
+        client = get_s3_client()
+        response = await run_in_thread(client.get_object, Bucket=self.bucket, Key=key)
         return cast(bytes, response["Body"].read())
 
     async def update(self, key: str, value: bytes) -> None:
         """Update an S3 object."""
-        client = _S3_CLIENT.get()
-        await _run_in_thread(client.put_object, Bucket=self.bucket, Key=key, Body=value)
+        client = get_s3_client()
+        await run_in_thread(client.put_object, Bucket=self.bucket, Key=key, Body=value)
 
     async def delete(self, key: str) -> None:
         """Delete an S3 object."""
-        client = _S3_CLIENT.get()
-        await _run_in_thread(client.delete_object, Bucket=self.bucket, Key=key)
+        client = get_s3_client()
+        await run_in_thread(client.delete_object, Bucket=self.bucket, Key=key)
 
-
-async def _run_in_thread(func: Callable[P, R], /, *args: P.args, **kwargs: P.kwargs) -> R:
-    return await from_thread.run(partial(func, *args, **kwargs))
+    async def exists(self, key: str) -> bool:
+        """Check if an S3 object exists."""
+        client = get_s3_client()
+        try:
+            await run_in_thread(client.head_object, Bucket=self.bucket, Key=key)
+        except ClientError as error:
+            if error.response["Error"]["Code"] == "404":
+                return False
+            raise  # nocov
+        return True
```

### Comparing `artigraph-0.0.3/.gitignore` & `artigraph-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.3/LICENSE.txt` & `artigraph-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.3/pyproject.toml` & `artigraph-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,52 +19,68 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["typing_extensions", "sqlalchemy>=2,<3", "anyio>=3,<4"]
 
 [project.optional-dependencies]
+all = ["artigraph[aws,pandas,numpy,polars,pyarrow]"]
 aws = ["boto3>=1,<2"]
-pandas = ["pandas>=2,<3", "pyarrow>=12,<13"]
-numpy = ["numpy>=1,<2", "pandas>=2,<3", "pyarrow>=12,<13"]
-polars = ["polars<1", "pyarrow>=12,<13"]
+pandas = ["pandas>=2,<3", "artigraph[pyarrow]"]
+numpy = ["numpy>=1,<2", "pandas>=2,<3", "artigraph[pyarrow]"]
+polars = ["polars<1", "artigraph[pyarrow]"]
+pyarrow = ["pyarrow>=12,<13"]
 
 [project.urls]
 Documentation = "https://github.com/unknown/artigraph#readme"
 Issues = "https://github.com/unknown/artigraph/issues"
 Source = "https://github.com/unknown/artigraph"
 
+# --- Hatch ----------------------------------------------------------------------------------------
+
 [tool.hatch.version]
 path = "src/artigraph/__init__.py"
 
 [tool.hatch.envs.default]
-dependencies = ["coverage[toml]>=6.5", "pytest"]
+dependencies = [
+  "coverage[toml]>=6.5",
+  "pytest>=7",
+  "pytest-asyncio",
+  "black>=23.1.0",
+  "pyright>=1",
+  "ruff>=0.0.243",
+  "aiosqlite>=0.19,<1",
+  "greenlet>=2,<3",
+  "moto>=4,<5",
+]
+
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
+cov = ["cov-test", "cov-report"]
 cov-report = ["- coverage combine", "coverage report"]
-cov = ["test-cov", "cov-report"]
+cov-test = "coverage run -m pytest {args:tests}"
+format = ["black {args:.}", "ruff --fix {args:.}", "style"]
+lint = ["lint-style", "lint-typing"]
+lint-style = ["ruff {args:.}", "black --check --diff {args:.}"]
+lint-typing = "pyright {args:src}"
+test = "pytest {args:tests}"
+
+# --- Pytest ---------------------------------------------------------------------------------------
 
-[[tool.hatch.envs.all.matrix]]
-python = ["3.9", "3.10", "3.11"]
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
 
-[tool.hatch.envs.lint]
-detached = true
-dependencies = ["black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
-[tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/artigraph tests}"
-style = ["ruff {args:.}", "black --check --diff {args:.}"]
-fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
-all = ["style", "typing"]
+# --- Black ----------------------------------------------------------------------------------------
 
 [tool.black]
 target-version = ["py37"]
 line-length = 100
 skip-string-normalization = true
 
+# --- Ruff -----------------------------------------------------------------------------------------
+
 [tool.ruff]
 target-version = "py37"
 line-length = 100
 select = [
   "A",
   "ARG",
   "B",
@@ -88,14 +104,16 @@
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
 ignore = [
+  # Ignore function call in class definition (see: https://github.com/astral-sh/ruff/issues/4171)
+  "RUF009",
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105",
   "S106",
@@ -118,18 +136,34 @@
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
+# --- Coverage -------------------------------------------------------------------------------------
+
 [tool.coverage.run]
-source_pkgs = ["artigraph", "tests"]
+source_pkgs = ["artigraph"]
 branch = true
 parallel = true
 
 [tool.coverage.paths]
 artigraph = ["src/artigraph"]
-tests = ["tests"]
 
 [tool.coverage.report]
-exclude_lines = ["no ?cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+fail_under = 100
+show_missing = true
+skip_covered = true
+sort = "Name"
+exclude_lines = [
+  "no ?cov",
+  '\.\.\.',
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
+
+# --- PyRight -----------------------------------------------------------------------------------------
+
+[tool.pyright]
+include = ["src", "tests"]
```

