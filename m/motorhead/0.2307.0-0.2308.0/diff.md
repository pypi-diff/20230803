# Comparing `tmp/motorhead-0.2307.0.tar.gz` & `tmp/motorhead-0.2308.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motorhead-0.2307.0.tar", max compression
+gzip compressed data, was "motorhead-0.2308.0.tar", max compression
```

## Comparing `motorhead-0.2307.0.tar` & `motorhead-0.2308.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2307.0/LICENSE
--rw-r--r--   0        0        0     2100 2023-07-29 23:37:28.841882 motorhead-0.2307.0/README.md
--rw-r--r--   0        0        0     1657 2023-07-29 22:32:11.019932 motorhead-0.2307.0/motorhead/__init__.py
--rw-r--r--   0        0        0     3145 2023-07-29 09:07:27.173242 motorhead-0.2307.0/motorhead/bound_method_wrapper.py
--rw-r--r--   0        0        0     2631 2023-07-29 22:34:06.052474 motorhead-0.2307.0/motorhead/delete_rule.py
--rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2307.0/motorhead/model/__init__.py
--rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2307.0/motorhead/model/deleteresultmodel.py
--rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2307.0/motorhead/model/document.py
--rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2307.0/motorhead/model/objectid.py
--rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2307.0/motorhead/model/utcdatetime.py
--rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2307.0/motorhead/py.typed
--rw-r--r--   0        0        0    28158 2023-07-29 22:32:41.356073 motorhead-0.2307.0/motorhead/service.py
--rw-r--r--   0        0        0     5705 2023-07-29 18:51:53.727231 motorhead-0.2307.0/motorhead/typing.py
--rw-r--r--   0        0        0     1631 2023-07-29 22:33:41.152355 motorhead-0.2307.0/motorhead/validator.py
--rw-r--r--   0        0        0     2666 2023-07-29 23:10:18.853151 motorhead-0.2307.0/pyproject.toml
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 motorhead-0.2307.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.0/LICENSE
+-rw-r--r--   0        0        0     2100 2023-07-29 23:37:28.841882 motorhead-0.2308.0/README.md
+-rw-r--r--   0        0        0     2038 2023-08-03 18:52:22.265079 motorhead-0.2308.0/motorhead/__init__.py
+-rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.0/motorhead/bound_method_wrapper.py
+-rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.0/motorhead/delete_rule.py
+-rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.0/motorhead/model/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.0/motorhead/model/deleteresultmodel.py
+-rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.0/motorhead/model/document.py
+-rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.0/motorhead/model/objectid.py
+-rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.0/motorhead/model/utcdatetime.py
+-rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.0/motorhead/operator.py
+-rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.0/motorhead/py.typed
+-rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.0/motorhead/query.py
+-rw-r--r--   0        0        0    28508 2023-08-03 18:51:22.611747 motorhead-0.2308.0/motorhead/service.py
+-rw-r--r--   0        0        0     6022 2023-08-03 18:52:05.408756 motorhead-0.2308.0/motorhead/typing.py
+-rw-r--r--   0        0        0     1678 2023-08-03 18:51:37.484136 motorhead-0.2308.0/motorhead/validator.py
+-rw-r--r--   0        0        0     2824 2023-08-03 21:01:58.639960 motorhead-0.2308.0/pyproject.toml
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 motorhead-0.2308.0/PKG-INFO
```

### Comparing `motorhead-0.2307.0/LICENSE` & `motorhead-0.2308.0/LICENSE`

 * *Files identical despite different names*

### Comparing `motorhead-0.2307.0/README.md` & `motorhead-0.2308.0/README.md`

 * *Files identical despite different names*

### Comparing `motorhead-0.2307.0/motorhead/__init__.py` & `motorhead-0.2308.0/motorhead/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+from . import operator as operator
 from .bound_method_wrapper import BoundMethodWrapper as BoundMethodWrapper
 from .delete_rule import DeleteConfig as DeleteConfig
 from .delete_rule import DeleteError as DeleteError
 from .delete_rule import delete_rule as delete_rule
 from .model import BaseDocument as BaseDocument
 from .model import DeleteResultModel as DeleteResultModel
 from .model import Document as Document
 from .model import ObjectId as ObjectId
 from .model import UTCDatetime as UTCDatetime
+from .operator import ensure_dict as ensure_dict
+from .query import Field as Field
+from .query import Q as Q
+from .query import Query as Query
+from .query import Queryable as Queryable
 from .service import DeleteResult as DeleteResult
 from .service import InsertOneResult as InsertOneResult
 from .service import Service as Service
 from .service import UpdateResult as UpdateResult
 from .typing import AgnosticClient as AgnosticClient
 from .typing import AgnosticCollection as AgnosticCollection
 from .typing import AgnosticDatabase as AgnosticDatabase
+from .typing import Clause as Clause
+from .typing import ClauseOrMongoQuery as ClauseOrMongoQuery
+from .typing import ClauseOrProjecttion as ClauseOrProjecttion
 from .typing import ClientProvider as ClientProvider
 from .typing import Collation as Collation
 from .typing import CollectionOptions as CollectionOptions
 from .typing import DatabaseProvider as DatabaseProvider
 from .typing import DeleteOptions as DeleteOptions
 from .typing import FindOptions as FindOptions
 from .typing import IndexData as IndexData
```

### Comparing `motorhead-0.2307.0/motorhead/bound_method_wrapper.py` & `motorhead-0.2308.0/motorhead/bound_method_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Callable, Coroutine
-from typing import Concatenate, Generic, ParamSpec, Type, TypeVar
+from typing import Concatenate, Generic, ParamSpec, TypeVar
 
 __all__ = ("BoundMethodWrapper",)
 
 TOwner = TypeVar("TOwner")
 TParams = ParamSpec("TParams")
 TConfig = TypeVar("TConfig")
 
@@ -62,15 +62,15 @@
     def name(self) -> str:
         """
         The (qualified) name of the wrapped method.
         """
         return self._func.__qualname__
 
     def __get__(
-        self, owner: TOwner, obj_type: Type[TOwner] | None = None
+        self, owner: TOwner, obj_type: type[TOwner] | None = None
     ) -> Callable[TParams, Coroutine[None, None, None]]:
         """
         Descriptor implementation that makes the wrapper work as a bound method of its owner.
         """
 
         async def do(*args: TParams.args, **kwargs: TParams.kwargs) -> None:
             return await self(owner, *args, **kwargs)
```

### Comparing `motorhead-0.2307.0/motorhead/delete_rule.py` & `motorhead-0.2308.0/motorhead/delete_rule.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2307.0/motorhead/model/document.py` & `motorhead-0.2308.0/motorhead/model/document.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2307.0/motorhead/model/objectid.py` & `motorhead-0.2308.0/motorhead/model/objectid.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2307.0/motorhead/model/utcdatetime.py` & `motorhead-0.2308.0/motorhead/model/utcdatetime.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2307.0/motorhead/service.py` & `motorhead-0.2308.0/motorhead/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 from collections.abc import AsyncGenerator, Callable, Coroutine, Generator, Mapping, Sequence
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, nullcontext
-from typing import TYPE_CHECKING, Any, Generic, Type, TypeVar, get_args
+from typing import TYPE_CHECKING, Any, Generic, TypeVar, get_args
 
 from bson import ObjectId
 from pydantic import BaseModel
 from pymongo.results import DeleteResult, InsertOneResult, UpdateResult
 
+from .operator import ensure_dict
+from .typing import ClauseOrMongoQuery
+
 if TYPE_CHECKING:
     from motor.core import (
         AgnosticClientSession,
         AgnosticCursor,
         AgnosticLatentCommandCursor,
     )
 
@@ -22,15 +25,14 @@
         Collation,
         CollectionOptions,
         DeleteOptions,
         FindOptions,
         IndexData,
         InsertOneOptions,
         MongoProjection,
-        MongoQuery,
         UpdateManyOptions,
         UpdateObject,
         UpdateOneOptions,
     )
 
 from .delete_rule import DeleteRule
 from .validator import Validator
@@ -141,25 +143,28 @@
 
         Arguments:
             pipeline: The aggregation pipeline.
             session: An optional session to use.
         """
         return self.collection.aggregate(pipeline, session=session, **kwargs)
 
-    async def count_documents(self, query: MongoQuery, *, options: FindOptions | None = None) -> int:
+    async def count_documents(
+        self, query: ClauseOrMongoQuery, *, options: FindOptions | None = None
+    ) -> int:
         """
         Returns the number of documents that match the given query.
 
         Arguments:
             query: The query object.
             options: Query options, see the arguments of `collection.count_documents()` for details.
 
         Returns:
             The number of matching documents.
         """
+        query = ensure_dict(query)
         return await self.collection.count_documents(query, **(options or {}))  # type: ignore[no-any-return]
 
     async def create_index(
         self,
         keys: str | Sequence[tuple[str, int | str | Mapping[str, Any]]],
         *,
         name: str,
@@ -275,15 +280,15 @@
         Returns:
             The result of the operation.
         """
         return await self.delete_one({"_id": id}, options=options)
 
     async def delete_many(
         self,
-        query: MongoQuery | None,
+        query: ClauseOrMongoQuery | None,
         *,
         options: DeleteOptions | None = None,
     ) -> DeleteResult:
         """
         The default `delete_many()` implementation of the service.
 
         The method enforces delete rules and executes the operation as follows:
@@ -298,14 +303,15 @@
         Arguments:
             query: Query object that matches the documents that should be deleted.
             options: Delete options, see the arguments of `collection.delete_many()`.
 
         Returns:
             The result of the operation.
         """
+        query = None if query is None else ensure_dict(query)
         session_manager = self._get_session_context_manager(
             options.get("session", None) if options else None
         )
         async with await session_manager() as session:
             opts: DeleteOptions = options or {}
             opts["session"] = session
             ctxman = (
@@ -338,15 +344,15 @@
                         ids,  # type: ignore[arg-type] # can not be None if has_ids is True
                     )
 
                 return result  # type: ignore[no-any-return]
 
     async def delete_one(
         self,
-        query: MongoQuery | None,
+        query: ClauseOrMongoQuery | None,
         *,
         options: DeleteOptions | None = None,
     ) -> DeleteResult:
         """
         The default `delete_one()` implementation of the service.
 
         The method enforces delete rules and executes the operation as follows:
@@ -361,14 +367,15 @@
         Arguments:
             query: Query object that matches the document that should be deleted.
             options: Delete options, see the arguments of `collection.delete_one()`.
 
         Returns:
             The result of the operation.
         """
+        query = None if query is None else ensure_dict(query)
         session_manager = self._get_session_context_manager(
             options.get("session", None) if options else None
         )
         async with await session_manager() as session:
             opts: DeleteOptions = options or {}
             opts["session"] = session
             ctxman = (
@@ -408,15 +415,15 @@
         Returns:
             Whether the document with the given ID exists.
         """
         return await self.count_documents({"_id": id}, options=options) == 1
 
     def find(
         self,
-        query: MongoQuery | None = None,
+        query: ClauseOrMongoQuery | None = None,
         projection: MongoProjection | None = None,
         *,
         options: FindOptions | None = None,
     ) -> AgnosticCursor:
         """
         The default `find()` implementation of the service.
 
@@ -424,40 +431,42 @@
             query: The query object.
             projection: Optional projection.
             options: Query options, see the arguments of `collection.find()` for details.
 
         Returns:
             An async database cursor.
         """
+        query = None if query is None else ensure_dict(query)
         return self.collection.find(query, projection, **(options or {}))
 
     async def find_ids(
         self,
-        query: MongoQuery | None,
+        query: ClauseOrMongoQuery | None,
         *,
         session: AgnosticClientSession | None = None,
     ) -> list[ObjectId]:
         """
         Returns the IDs of all documents that match the given query.
 
         Arguments:
             query: The query object.
             session: An optional database session to use.
 
         Returns:
             The IDs of all matching documents.
         """
+        query = None if query is None else ensure_dict(query)
         return [
             doc["_id"]
             for doc in await self.collection.find(query, {"_id": True}, session=session).to_list(None)
         ]
 
     async def find_one(
         self,
-        query: MongoQuery | None = None,
+        query: ClauseOrMongoQuery | None = None,
         projection: MongoProjection | None = None,
         *,
         options: FindOptions | None = None,
     ) -> dict[str, Any] | None:
         """
         The default `find_one()` implementation of the service.
 
@@ -465,14 +474,15 @@
             query: The query object.
             projection: Optional projection.
             options: Query options, see the arguments of `collection.find()` for details.
 
         Returns:
             A single matching document or `None` if there are no matches.
         """
+        query = None if query is None else ensure_dict(query)
         return await self.collection.find_one(query, projection, **(options or {}))  # type: ignore[no-any-return]
 
     async def get_by_id(
         self,
         id: ObjectId,
         projection: MongoProjection | None = None,
         *,
@@ -533,15 +543,15 @@
         Raises:
             Exception: if the data is invalid.
         """
         return await self.update_one({"_id": id}, changes, options=options)
 
     async def update_many(
         self,
-        query: MongoQuery | None,
+        query: ClauseOrMongoQuery | None,
         changes: TUpdate,
         *,
         options: UpdateManyOptions | None = None,
     ) -> UpdateResult:
         """
         The default `delete_many()` implementation of the service.
 
@@ -552,23 +562,24 @@
 
         Returns:
             The result of the operation.
 
         Raises:
             Exception: if the data is invalid.
         """
+        query = None if query is None else ensure_dict(query)
         return await self.collection.update_many(  # type: ignore[no-any-return]
             query,
             await self._prepare_for_update(query, changes),
             **(options or {}),
         )
 
     async def update_one(
         self,
-        query: MongoQuery | None,
+        query: ClauseOrMongoQuery | None,
         changes: TUpdate,
         *,
         options: UpdateOneOptions | None = None,
     ) -> UpdateResult:
         """
         The default `delete_one()` implementation of the service.
 
@@ -579,22 +590,23 @@
 
         Returns:
             The result of the operation.
 
         Raises:
             Exception: if the data is invalid.
         """
+        query = None if query is None else ensure_dict(query)
         return await self.collection.update_one(  # type: ignore[no-any-return]
             query,
             await self._prepare_for_update(query, changes),
             **(options or {}),
         )
 
     @classmethod
-    def get_objectid_fields(cls, model: Type[BaseModel]) -> set[str]:
+    def get_objectid_fields(cls, model: type[BaseModel]) -> set[str]:
         """
         Returns the names of all `ObjectId` fields.
 
         Arguments:
             model: The model to collect `ObjectId` field
         """
         result: set[str] = set()
@@ -691,17 +703,14 @@
 
     def _mongo_dump(self, data: BaseModel) -> dict[str, Any]:
         """
         Dumps the given model instance for consumption by MongoDB.
 
         Arguments:
             data: The model instance to dump.
-            exclude_none_id: Whether to exclude `None` `ObjectId` fields. This is usually
-                necessary during creation if the client sends `None` in a reference field,
-                to avoid creating a new `ObjectId` that doesn't reference an existing document.
 
         Returns:
             The MongoDB-compatible, dumped dictionary.
         """
         objectid_fields = self.get_objectid_fields(type(data))
         return {
             **{
@@ -717,15 +726,15 @@
                 exclude=objectid_fields,
                 by_alias=True,
                 exclude_unset=True,
                 mode="json",
             ),
         }
 
-    async def _prepare_for_insert(self, query: MongoQuery | None, data: TInsert) -> dict[str, Any]:
+    async def _prepare_for_insert(self, query: ClauseOrMongoQuery | None, data: TInsert) -> dict[str, Any]:
         """
         Validates the given piece of data and converts it into its database representation
         if validation was successful.
 
         Arguments:
             query: Query that matches the documents that will be updated.
             data: The data to be inserted.
@@ -736,15 +745,15 @@
         Raises:
             Exception: if the data is invalid.
         """
         await self._validate_insert(query, data)
         return await self._convert_for_insert(data)
 
     async def _prepare_for_update(
-        self, query: MongoQuery | None, data: TUpdate
+        self, query: ClauseOrMongoQuery | None, data: TUpdate
     ) -> UpdateObject | Sequence[UpdateObject]:
         """
         Validates the given piece of data and converts it into an update object.
 
         Arguments:
             query: Query that matches the documents that will be updated.
             data: The update data.
@@ -754,15 +763,15 @@
 
         Raises:
             Exception: if the data is invalid.
         """
         await self._validate_update(query, data)
         return await self._convert_for_update(data)
 
-    async def _validate_insert(self, query: MongoQuery | None, data: TInsert) -> None:
+    async def _validate_insert(self, query: ClauseOrMongoQuery | None, data: TInsert) -> None:
         """
         Validates the given piece of data for insertion by executing all insert validators.
 
         See `Validator` for more information.
 
         Arguments:
             query: Query that matches the documents that will be updated.
@@ -823,15 +832,15 @@
         Raises:
             DeleteError: if one of the executed delete rules fail.
         """
         for rule in self._delete_rules():
             if isinstance(rule, DeleteRule) and rule.config == "post":
                 await rule(self, session, ids)
 
-    async def _validate_update(self, query: MongoQuery | None, data: TUpdate) -> None:
+    async def _validate_update(self, query: ClauseOrMongoQuery | None, data: TUpdate) -> None:
         """
         Validates the given piece of data for update by executing all update validators.
 
         See `Validator` for more information.
 
         Arguments:
             query: Query that matches the documents that will be updated.
```

### Comparing `motorhead-0.2307.0/motorhead/typing.py` & `motorhead-0.2308.0/motorhead/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Mapping, Sequence
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Protocol, TypedDict
+from typing import TYPE_CHECKING, Any, Protocol, TypedDict, Union
 
 from motor.core import AgnosticClient, AgnosticCollection, AgnosticDatabase
 from pymongo.collation import Collation as PMCollation
 
 if TYPE_CHECKING:
     from bson.codec_options import CodecOptions
     from pymongo.read_concern import ReadConcern
@@ -48,14 +48,28 @@
 
 UpdateObject = dict[str, Any] | Sequence[dict[str, Any]]
 """
 MongoDB update object.
 """
 
 
+class Clause(Protocol):
+    """
+    Protocol for clauses that service methods can convert to dictionaries
+    that can be consumed by MongoDB.
+    """
+
+    def to_mongo(self) -> dict[str, Any]:
+        ...
+
+
+ClauseOrMongoQuery = Union[Clause, MongoQuery]
+ClauseOrProjecttion = Union[Clause, MongoProjection]
+
+
 class CollationDict(TypedDict, total=False):
     """
     Collation definition as a dict.
     """
 
     locale: str
     caseLevel: bool | None
```

### Comparing `motorhead-0.2307.0/motorhead/validator.py` & `motorhead-0.2308.0/motorhead/validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Callable, Coroutine
 from typing import Literal, TypeVar
 
 from .bound_method_wrapper import BoundMethodWrapper
-from .typing import MongoQuery
+from .typing import ClauseOrMongoQuery
 
 __all__ = (
     "ValidationError",
     "Validator",
     "validator",
 )
 
@@ -16,15 +16,17 @@
 
 
 TOwner = TypeVar("TOwner")
 TInsertOrUpdate = TypeVar("TInsertOrUpdate")
 InsertUpdateConfig = Literal["insert", "update", "insert-update"]
 
 
-class Validator(BoundMethodWrapper[TOwner, [MongoQuery | None, TInsertOrUpdate], InsertUpdateConfig]):
+class Validator(
+    BoundMethodWrapper[TOwner, [ClauseOrMongoQuery | None, TInsertOrUpdate], InsertUpdateConfig]
+):
     """
     Validator method wrapper.
 
     Validator methods receive an insert or update object, and execute some - potentially
     async - operations to make sure the inserted or updated data is valid.
     """
 
@@ -32,15 +34,15 @@
 
     exception = ValidationError
 
 
 def validator(
     config: InsertUpdateConfig = "insert-update",
 ) -> Callable[
-    [Callable[[TOwner, MongoQuery | None, TInsertOrUpdate], Coroutine[None, None, None]]],
+    [Callable[[TOwner, ClauseOrMongoQuery | None, TInsertOrUpdate], Coroutine[None, None, None]]],
     "Validator[TOwner, TInsertOrUpdate]",
 ]:
     """
     Service method decorator factory that converts the decorated method into a `Validator` instance.
 
     Example:
 
@@ -52,12 +54,13 @@
     ```
 
     Arguments:
         config: Validatator config.
     """
 
     def decorator(
-        func: Callable[[TOwner, MongoQuery | None, TInsertOrUpdate], Coroutine[None, None, None]], /
+        func: Callable[[TOwner, ClauseOrMongoQuery | None, TInsertOrUpdate], Coroutine[None, None, None]],
+        /,
     ) -> "Validator[TOwner, TInsertOrUpdate]":
         return Validator(func=func, config=config)
 
     return decorator
```

### Comparing `motorhead-0.2307.0/pyproject.toml` & `motorhead-0.2308.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,33 +26,32 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/motorhead"
 Documentation = "https://volfpeter.github.io/motorhead"
 
 [tool.poetry]
 name = "motorhead"
-version = "0.2307.0"
+version = "0.2308.0"
 description = "Async MongoDB with Pydantic - made easy."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "motorhead"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 motor = "^3.1.0"
 pydantic = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 mkdocs-material = "^9.1.21"
-mkdocstrings = "^0.22.0"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mypy = "^1.4.1"
 ruff = "^0.0.280"
 poethepoet = "^0.21.1"
-mongomock = "^4.1.2"
 pytest = "^7.4.0"
 
 [tool.poetry.group.fastapi.dependencies]
 fastapi = {extras = ["all"], version = "^0.100.1"}
 
 [tool.black]
 line-length = 108
@@ -93,19 +92,24 @@
 [tool.ruff.isort]
 known-third-party = [
     "bson",
     "motor",
     "pydantic",
 ]
 
+[tool.ruff.per-file-ignores]
+"tests/**/*" = ["S101"]  # S101: use of assert detected
+
 [tool.poe.tasks]
+serve-docs = "mkdocs serve"
 black = "black ."
 black-check = "black . --check"
 mypy = "mypy ."
 ruff = "ruff check ."
+test = "python -m pytest tests"
 
 static-checks.sequence =  ["ruff", "black-check", "mypy"]
 static-checks.ignore_fail = "return_non_zero"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `motorhead-0.2307.0/PKG-INFO` & `motorhead-0.2308.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motorhead
-Version: 0.2307.0
+Version: 0.2308.0
 Summary: Async MongoDB with Pydantic - made easy.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

