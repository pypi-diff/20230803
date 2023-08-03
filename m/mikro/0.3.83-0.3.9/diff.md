# Comparing `tmp/mikro-0.3.83.tar.gz` & `tmp/mikro-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikro-0.3.83.tar", max compression
+gzip compressed data, was "mikro-0.3.9.tar", max compression
```

## Comparing `mikro-0.3.83.tar` & `mikro-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,23 @@
--rw-r--r--   0        0        0      314 2023-07-27 14:06:00.188223 mikro-0.3.83/mikro/__init__.py
--rw-r--r--   0        0        0       38 2022-11-21 13:25:24.312569 mikro-0.3.83/mikro/api/__init__.py
--rw-r--r--   0        0        0   411398 2023-07-19 17:10:18.210794 mikro-0.3.83/mikro/api/schema.py
--rw-r--r--   0        0        0        0 2023-01-24 14:42:54.553770 mikro-0.3.83/mikro/cli/__init__.py
--rw-r--r--   0        0        0     3237 2023-03-09 16:01:04.382912 mikro-0.3.83/mikro/cli/main.py
--rw-r--r--   0        0        0    92815 2023-01-24 15:15:30.502724 mikro-0.3.83/mikro/cli/schemas/v1.graphql
--rw-r--r--   0        0        0      166 2023-03-09 13:07:49.776971 mikro-0.3.83/mikro/cli/utils.py
--rw-r--r--   0        0        0        0 2022-08-25 14:13:51.564206 mikro-0.3.83/mikro/contrib/__init__.py
--rw-r--r--   0        0        0        0 2022-02-03 16:40:05.361043 mikro-0.3.83/mikro/contrib/fakts/__init__.py
--rw-r--r--   0        0        0     1167 2023-08-02 11:42:03.780201 mikro-0.3.83/mikro/contrib/fakts/datalayer.py
--rw-r--r--   0        0        0     9060 2023-07-31 16:32:06.321548 mikro-0.3.83/mikro/datalayer.py
--rw-r--r--   0        0        0      156 2022-03-21 13:01:57.991994 mikro-0.3.83/mikro/errors.py
--rw-r--r--   0        0        0     1070 2023-07-27 14:07:48.088787 mikro-0.3.83/mikro/funcs.py
--rw-r--r--   0        0        0        0 2023-07-23 08:07:45.702571 mikro-0.3.83/mikro/io/__init__.py
--rw-r--r--   0        0        0      326 2023-07-23 08:23:30.387050 mikro-0.3.83/mikro/io/download.py
--rw-r--r--   0        0        0      351 2023-07-23 08:25:11.851531 mikro-0.3.83/mikro/io/errors.py
--rw-r--r--   0        0        0      532 2023-08-03 15:43:00.397835 mikro-0.3.83/mikro/io/namers.py
--rw-r--r--   0        0        0     1272 2023-07-23 08:56:01.748546 mikro-0.3.83/mikro/io/types.py
--rw-r--r--   0        0        0     3826 2023-08-03 15:43:00.397835 mikro-0.3.83/mikro/io/upload.py
--rw-r--r--   0        0        0       92 2022-03-21 13:01:58.083994 mikro-0.3.83/mikro/links/__init__.py
--rw-r--r--   0        0        0     2441 2023-08-02 18:49:54.960874 mikro-0.3.83/mikro/links/datalayer.py
--rw-r--r--   0        0        0        0 2022-05-17 11:20:06.504915 mikro-0.3.83/mikro/links/errors.py
--rw-r--r--   0        0        0      978 2023-08-02 18:55:59.886659 mikro-0.3.83/mikro/mikro.py
--rw-r--r--   0        0        0     1682 2023-08-02 18:59:27.027675 mikro-0.3.83/mikro/rath.py
--rw-r--r--   0        0        0    14412 2023-06-12 10:09:46.191178 mikro-0.3.83/mikro/scalars.py
--rw-r--r--   0        0        0     8085 2023-07-27 14:08:46.205091 mikro-0.3.83/mikro/structures.py
--rw-r--r--   0        0        0        0 2023-03-04 15:06:28.973785 mikro-0.3.83/mikro/testing/__init__.py
--rw-r--r--   0        0        0     1225 2023-03-04 15:22:43.161911 mikro-0.3.83/mikro/testing/datalayer.py
--rw-r--r--   0        0        0    12346 2023-06-07 08:20:53.944356 mikro-0.3.83/mikro/traits.py
--rw-r--r--   0        0        0     1314 2023-05-19 13:15:39.685195 mikro-0.3.83/mikro/utils.py
--rw-r--r--   0        0        0     2090 2023-07-19 17:11:48.407394 mikro-0.3.83/mikro/widgets.py
--rw-r--r--   0        0        0     1760 2023-08-03 15:43:45.790099 mikro-0.3.83/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 mikro-0.3.83/PKG-INFO
+-rw-r--r--   0        0        0      101 2022-08-25 11:10:14.051638 mikro-0.3.9/mikro/__init__.py
+-rw-r--r--   0        0        0       38 2022-11-21 13:25:24.312569 mikro-0.3.9/mikro/api/__init__.py
+-rw-r--r--   0        0        0   242929 2022-12-15 13:54:09.942241 mikro-0.3.9/mikro/api/schema.py
+-rw-r--r--   0        0        0        0 2022-11-21 13:19:21.452118 mikro-0.3.9/mikro/builders.py
+-rw-r--r--   0        0        0     4468 2022-12-08 12:30:42.620796 mikro-0.3.9/mikro/cli/main.py
+-rw-r--r--   0        0        0        0 2022-08-25 14:13:51.564206 mikro-0.3.9/mikro/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-03 16:40:05.361043 mikro-0.3.9/mikro/contrib/fakts/__init__.py
+-rw-r--r--   0        0        0     1303 2022-11-21 13:24:56.296558 mikro-0.3.9/mikro/contrib/fakts/datalayer.py
+-rw-r--r--   0        0        0     4531 2022-11-21 17:10:07.795408 mikro-0.3.9/mikro/datalayer.py
+-rw-r--r--   0        0        0      156 2022-03-21 13:01:57.991994 mikro-0.3.9/mikro/errors.py
+-rw-r--r--   0        0        0     1174 2022-11-21 13:16:43.067875 mikro-0.3.9/mikro/funcs.py
+-rw-r--r--   0        0        0       92 2022-03-21 13:01:58.083994 mikro-0.3.9/mikro/links/__init__.py
+-rw-r--r--   0        0        0     2413 2022-11-21 13:12:09.135444 mikro-0.3.9/mikro/links/datalayer.py
+-rw-r--r--   0        0        0        0 2022-05-17 11:20:06.504915 mikro-0.3.9/mikro/links/errors.py
+-rw-r--r--   0        0        0      903 2022-11-21 13:21:58.284355 mikro-0.3.9/mikro/mikro.py
+-rw-r--r--   0        0        0     1522 2022-11-21 13:25:20.364567 mikro-0.3.9/mikro/rath.py
+-rw-r--r--   0        0        0    12037 2022-12-15 13:54:02.174160 mikro-0.3.9/mikro/scalars.py
+-rw-r--r--   0        0        0     4098 2022-12-12 14:45:25.646781 mikro-0.3.9/mikro/structures.py
+-rw-r--r--   0        0        0     5750 2022-12-15 10:05:28.013204 mikro-0.3.9/mikro/traits.py
+-rw-r--r--   0        0        0      805 2022-09-26 09:28:04.741028 mikro-0.3.9/mikro/widgets.py
+-rw-r--r--   0        0        0     1241 2022-12-15 14:13:59.916979 mikro-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 mikro-0.3.9/setup.py
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 mikro-0.3.9/PKG-INFO
```

### Comparing `mikro-0.3.83/mikro/contrib/fakts/datalayer.py` & `mikro-0.3.9/mikro/contrib/fakts/datalayer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from typing import Any, Dict, Optional
 
 from fakts.fakt.base import Fakt
-from fakts.fakts import Fakts
+from fakts.fakts import Fakts, get_current_fakts
 from herre.herre import Herre, current_herre
 from mikro.datalayer import DataLayer
 
 
 class DataLayerFakt(Fakt):
     endpoint_url: str
 
     class Config:
         group = "mikro.datalayer"
 
 
 class FaktsDataLayer(DataLayer):
-    """A fakts implementation of the datalayer. This will allow you to connect to a datalayer
+    """ A fakts implementation of the datalayer. This will allow you to connect to a datalayer
     that is defined asnychronously in fakts. This is useful for connecting to a datalayer that
     is not known at compile time. Will get the server configuration from fakts and connect to the
-    datalayer."""
-
+    datalayer. """
     fakts_group: str
-    fakts: Fakts
-    herre: Herre
+    fakts: Optional[Fakts] = None
+    herre: Optional[Herre] = None
 
     _old_fakt: Dict[str, Any] = {}
 
     def configure(self, fakt: DataLayerFakt) -> None:
+        self.herre = self.herre or current_herre.get()
         self.endpoint_url = fakt.endpoint_url
 
     async def aconnect(self):
-        if self.fakts.has_changed(self._old_fakt, self.fakts_group):
-            self._old_fakt = await self.fakts.aget(self.fakts_group)
+        fakts = get_current_fakts()
+
+        if fakts.has_changed(self._old_fakt, self.fakts_group):
+            self._old_fakt = await fakts.aget(self.fakts_group)
             self.configure(DataLayerFakt(**self._old_fakt))
         return await super().aconnect()
 
     async def __aenter__(self):
         return await super().__aenter__()
```

### Comparing `mikro-0.3.83/mikro/funcs.py` & `mikro-0.3.9/mikro/funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """ This module provides helpers for the mikro rath api
 they are wrapped functions for the turms generated api"""
 from mikro.rath import MikroRath, current_mikro_rath
-from koil.helpers import unkoil
 
 
-async def aexecute(
+def execute(
     operation,
     variables,
     rath: MikroRath = None,
 ):
     rath = rath or current_mikro_rath.get()
-    x = await rath.aquery(operation.Meta.document, operation.Arguments(**variables))
-    return operation(**x.data)
+    return operation(
+        **rath.query(
+            operation.Meta.document,
+            operation.Arguments(**variables),
+        ).data
+    )
 
 
-def execute(
+async def aexecute(
     operation,
     variables,
     rath: MikroRath = None,
 ):
-    return unkoil(aexecute, operation, variables, rath)
+    rath = rath or current_mikro_rath.get()
+    x = await rath.aquery(operation.Meta.document, operation.Arguments(**variables))
+    return operation(**x.data)
 
 
 def subscribe(operation, variables, rath: MikroRath = None):
     rath = rath or current_mikro_rath.get()
     for ev in rath.subscribe(operation.Meta.document, operation.Arguments(**variables)):
         yield operation(**ev.data)
```

### Comparing `mikro-0.3.83/mikro/links/datalayer.py` & `mikro-0.3.9/mikro/links/datalayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 
 from mikro.datalayer import DataLayer, current_datalayer
-from mikro.scalars import XArrayInput, ParquetInput, BigFile
+from mikro.scalars import XArrayInput, ParquetInput
 from rath.links.parsing import ParsingLink
-from rath.operation import Operation, opify
-import ntpath
+from rath.operation import Operation
 
 
 async def apply_recursive(func, obj, typeguard):
     if isinstance(obj, dict):  # if dict, apply to each key
         return {k: await apply_recursive(func, v, typeguard) for k, v in obj.items()}
     elif isinstance(obj, list):  # if list, apply to each element
         return await asyncio.gather(
@@ -40,15 +39,18 @@
 
     """
 
     FILEVERSION = "0.1"
     _connected = False
     _lock: asyncio.Lock = False
 
-    datalayer: DataLayer
+    _datalayer: DataLayer = None
+
+    async def aconnect(self):
+        self._datalayer = current_datalayer.get()
 
     async def aparse(self, operation: Operation) -> Operation:
         """Parse the operation (Async)
 
         Extracts the DataFrame from the operation and uploads it to the DataLayer.
 
         Args:
@@ -57,25 +59,24 @@
         Returns:
             Operation: _description_
         """
 
         if not self._lock:
             self._lock = asyncio.Lock()
 
-        if not self.datalayer._connected:
-            await self.datalayer.aconnect()
+        if not self._datalayer._connected:
+            await self._datalayer.aconnect()
+
+        datalayer: DataLayer = current_datalayer.get()
 
         operation.variables = await apply_recursive(
-            self.datalayer.astore_array_input, operation.variables, XArrayInput
-        )
-        operation.variables = await apply_recursive(
-            self.datalayer.astore_parquet_input, operation.variables, ParquetInput
+            datalayer.astore_array_input, operation.variables, XArrayInput
         )
         operation.variables = await apply_recursive(
-            self.datalayer.astore_bigfile, operation.variables, BigFile
+            datalayer.astore_parquet_input, operation.variables, ParquetInput
         )
 
         return operation
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
```

### Comparing `mikro-0.3.83/mikro/mikro.py` & `mikro-0.3.9/mikro/mikro.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pydantic import Field
 from koil import koilable
 from koil.composition import Composition
-from mikro.rath import MikroRath
 from mikro.datalayer import DataLayer
+from mikro.rath import MikroRath
 
 
+@koilable(add_connectors=True)
 class Mikro(Composition):
-    """The Mikro Composition
-
+    """ The Mikro Composition
+    
     This composition provides a datalayer and a rath for interacting with the
-    mikro api and beyond
+    mikro api.
 
     You shouldn't need to create this directly, instead use the builder functions
     to generate a new instance of this composition.
 
     ```python
 
     from mikro import Mikro
@@ -24,12 +25,10 @@
     m = Mikro(
         datalayer= DataLayer(endpoint_url="s3.amazonaws.com", access_key="XXXX", secret_key="XXXX"),
         mikro = MikroRath(link=MikroLinkComposition(auth=AuthTokenLink(token_loader=aget_token)))),
     )
     ```
     """
 
-    datalayer: DataLayer
-    rath: MikroRath
 
-    def _repr_html_inline_(self):
-        return f"<table></tr><tr><td>rath</td><td>{self.rath._repr_html_inline_()}</td></tr></table>"
+    datalayer: DataLayer
+    rath: MikroRath = Field(default_factory=MikroRath)
```

### Comparing `mikro-0.3.83/mikro/rath.py` & `mikro-0.3.9/mikro/rath.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,43 +5,37 @@
 from rath.links.auth import AuthTokenLink
 from rath.links.compose import TypedComposedLink
 from rath.links.dictinglink import DictingLink
 from rath.links.file import FileExtraction
 from rath.links.split import SplitLink
 
 
-current_mikro_rath = contextvars.ContextVar("current_mikro_rath_unpickable")
+current_mikro_rath = contextvars.ContextVar("current_mikro_rath")
 
 
 class MikroLinkComposition(TypedComposedLink):
-    datalayer: DataLayerUploadLink
+    datalayer: DataLayerUploadLink = Field(default_factory=DataLayerUploadLink)
     fileextraction: FileExtraction = Field(default_factory=FileExtraction)
     dicting: DictingLink = Field(default_factory=DictingLink)
     auth: AuthTokenLink
-    split: SplitLink  # order is important here, split must be last
+    split: SplitLink
 
 
 class MikroRath(rath.Rath):
-    """Mikro Rath
+    """ Mikro Rath
 
     Mikro Rath is the GraphQL client for Mikro. It is a thin wrapper around Rath
     that provides some default links and a context manager to set the current
     client. (This allows you to use the `mikro.rath.current` function to get the
     current client, within the context of mikro app).
-
+    
     This is a subclass of Rath that adds some default links to convert files and array to support
     the graphql multipart request spec."""
-
     link: MikroLinkComposition
 
-    def _repr_html_inline_(self):
-        return (
-            f"<table><tr><td>auto_connect</td><td>{self.auto_connect}</td></tr></table>"
-        )
-
     async def __aenter__(self):
         await super().__aenter__()
         current_mikro_rath.set(self)
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await super().__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `mikro-0.3.83/mikro/scalars.py` & `mikro-0.3.9/mikro/scalars.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,109 +2,48 @@
 Custom scalars for Mikro.
 
 
 """
 
 
 import os
-from typing import Any, List, IO, Optional
+from typing import Any
 import xarray as xr
+import pyarrow.parquet as pq
 import pandas as pd
 import numpy as np
-import io
-from typing import TYPE_CHECKING
-from .utils import rechunk
-import logging
-
-if TYPE_CHECKING:
-    from mikro.datalayer import DataLayer
-
-
-class AssignationID(str):
-    """A custom scalar to represent an affine matrix."""
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Validate the input array and convert it to a xr.DataArray."""
-        return cls(v)
-
-
-try:
-    from rekuest.actors.vars import (
-        get_current_assignation_helper,
-        NotWithinAnAssignationError,
-    )
-
-    def get_current_id(cls, value) -> AssignationID:
-        try:
-            return value or get_current_assignation_helper().assignment.assignation
-        except NotWithinAnAssignationError:
-            return value
-
-except ImportError:
-
-    def get_current_id(cls, value):
-        return value
 
 
 class XArrayConversionException(Exception):
-    """An exception that is raised when a conversion to xarray fails."""
-
     pass
 
 
 MetricValue = Any
 FeatureValue = Any
 
 
-class AffineMatrix(list):
-    """A custom scalar to represent an affine matrix."""
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Validate the input array and convert it to a xr.DataArray."""
-        if isinstance(v, np.ndarray):
-            assert v.ndim == 2
-            assert v.shape[0] == v.shape[1]
-            assert v.shape == (3, 3)
-            v = v.tolist()
-
-        assert isinstance(v, list)
-        return cls(v)
-
-    def as_matrix(self):
-        return np.array(self).reshape(3, 3)
-
 
 class XArrayInput:
     """A custom scalar for wrapping of every supported array like structure on
     the mikro platform. This scalar enables validation of various array formats
     into a mikro api compliant xr.DataArray.."""
 
     def __init__(self, value: xr.DataArray) -> None:
         self.value = value
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
-    def validate(cls, v: xr.DataArray):
+    def validate(cls, v):
         """Validate the input array and convert it to a xr.DataArray."""
 
         if isinstance(v, np.ndarray):
-            dims = ["c", "t", "z", "y", "x"]
+            dims = ["c", "t", "z", "x", "y"]
             v = xr.DataArray(v, dims=dims[5 - v.ndim :])
 
         if not isinstance(v, xr.DataArray):
             raise ValueError("This needs to be a instance of xarray.DataArray")
 
         if "x" not in v.dims:
             raise ValueError("Representations must always have a 'x' Dimension")
@@ -115,58 +54,34 @@
         if "t" not in v.dims:
             v = v.expand_dims("t")
         if "c" not in v.dims:
             v = v.expand_dims("c")
         if "z" not in v.dims:
             v = v.expand_dims("z")
 
-        chunks = rechunk(
-            v.sizes, itemsize=v.data.itemsize, chunksize_in_bytes=20_000_000
-        )
+        chunks = {
+            "t": 1,
+            "x": v.sizes["x"],
+            "y": v.sizes["y"],
+            "z": 1,
+            "c": 1,
+        }
 
         v = v.chunk(
             {key: chunksize for key, chunksize in chunks.items() if key in v.dims}
         )
 
         v = v.transpose(*"ctzyx")
 
         return cls(v)
 
     def __repr__(self):
         return f"InputArray({self.value})"
 
 
-class BigFile:
-    """A custom scalar for wrapping of every supported array like structure on
-    the mikro platform. This scalar enables validation of various array formats
-    into a mikro api compliant xr.DataArray.."""
-
-    def __init__(self, value: IO) -> None:
-        self.value = value
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Validate the input array and convert it to a xr.DataArray."""
-
-        if isinstance(v, str):
-            v = open(v, "rb")
-
-        if not isinstance(v, io.IOBase):
-            raise ValueError("This needs to be a instance of a file")
-
-        return cls(v)
-
-    def __repr__(self):
-        return f"BigFile({self.value})"
-
-
 class ParquetInput:
     """A custom scalar for ensuring a common format to support write to the
     parquet api supported by mikro. It converts the passed value into
     a compliant format.."""
 
     def __init__(self, value: pd.DataFrame) -> None:
         self.value = value
@@ -176,14 +91,15 @@
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
+
         if not isinstance(v, pd.DataFrame):
             raise ValueError("This needs to be a instance of pandas DataFrame")
 
         return cls(v)
 
     def __repr__(self):
         return f"ParquetInput({self.value})"
@@ -203,15 +119,15 @@
         self._openstore = None
 
     def arequest(self):
         """ToDO Imepelemtn, each store needs to have a request first to the resource owner
         and then we can access the data
         """
 
-    def open(self, dl: Optional["DataLayer"] = None):
+    def open(self, dl=None):
         """Opens the store and returns the zarr store object.
 
         The store is opened on the first access and then cached for later use. This is done to avoid
         opening the store on every access.
 
 
         Args:
@@ -220,17 +136,25 @@
         Returns:
             xr.DataArray: the data array
         """
         from mikro.datalayer import current_datalayer
 
         dl = dl or current_datalayer.get()
 
-        return xr.open_zarr(store=dl.open_store(self.value), consolidated=True)["data"]
+        assert (
+            dl
+        ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
+        if self._openstore is None:
+            self._openstore = xr.open_zarr(
+                store=dl.fs.get_mapper(self.value), consolidated=True
+            )["data"]
+
+        return self._openstore
 
-    async def aopen(self, dl=None, retry=True):
+    def aopen(self, dl=None):
         """Opens the store and returns the zarr store object.
 
         The store is opened on the first access and then cached for later use. This is done to avoid
         opening the store on every access.
 
 
         Args:
@@ -239,15 +163,23 @@
         Returns:
             xr.DataArray: the data array
         """
         from mikro.datalayer import current_datalayer
 
         dl = dl or current_datalayer.get()
 
-        return xr.open_zarr(store=dl.open_store(self.value), consolidated=True)["data"]
+        assert (
+            dl
+        ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
+        if self._openstore is None:
+            self._openstore = xr.open_zarr(
+                store=dl.fs.get_mapper(self.value), consolidated=True
+            )["data"]
+
+        return self._openstore
 
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
@@ -269,21 +201,20 @@
 class Parquet:
     """A custom scalar for ensuring an interface to the datalayer api supported by mikro. It converts the graphql value
     (a string pointed to a zarr store) into a parquet dataset and then a dataframe. This is used to access the data
     in the datalayer. The store is opened on the first access and then cached for later use. This is done to avoid
     opening the store on every access. This is done to avoid unnecessary requests to the datalayer api.
     """
 
-    def __init__(self, value: str) -> None:
+    def __init__(self, value) -> None:
         self.value = value
         self._openstore = None
 
-    def open(self, dl: Optional["DataLayer"] = None):
+    def open(self, dl=None):
         from mikro.datalayer import current_datalayer
-        import pyarrow.parquet as pq
 
         dl = dl or current_datalayer.get()
 
         assert (
             dl
         ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
         if not self._openstore:
@@ -315,36 +246,22 @@
     """
 
     __file__ = True
 
     def __init__(self, value) -> None:
         self.value = value
 
-    def download(
-        self, dl: Optional["DataLayer"] = None, filename: Optional[str] = None
-    ) -> str:
-        """Downloads the file to the current working directory.
-
-        Args:
-            dl (DataLayer, optional): The datalayer. Defaults to active datalayer.
-            filename (str, optional): The filename to save the file as. Defaults to the original filename.
-
-        Returns:
-            str: The filename of the downloaded file.
-        """
+    def download(self, dl=None):
         from mikro.datalayer import current_datalayer
         import requests
         import shutil
 
         dl = dl or current_datalayer.get()
-        assert (
-            dl
-        ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
         url = f"{dl.endpoint_url}{self.value}"
-        local_filename = filename or self.value.split("/")[-1].split("?")[0]
+        local_filename = self.value.split("/")[-1].split("?")[0]
         with requests.get(url, stream=True) as r:
             with open(local_filename, "wb") as f:
                 shutil.copyfileobj(r.raw, f)
                 return local_filename
 
     def __enter__(self):
         self.local_file = self.download()
@@ -368,48 +285,54 @@
         # exactly
         return cls(v)
 
     def __repr__(self):
         return f"File({self.value})"
 
 
+
 class ModelFile:
     """A custom scalar to enable uploading files to the datalayer
     it enables serialization of everythign
     """
 
     __file__ = True
 
     def __init__(self, value) -> None:
         self.value = value
 
+
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
 
+
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         # you could also return a string here which would mean model.post_code
         # would be a string, pydantic won't care but you could end up with some
         # confusion since the value's type won't match the type annotation
         # exactly
         if isinstance(v, str):
             return cls(open(v, "rb"))
+        
 
         return cls(v)
 
     def __repr__(self):
         return f"ModelFile({self.value})"
 
 
-class ModelData:
+
+
+class Model:
     """A custom scalar for ensuring an interface to files api supported by mikro. It converts the graphql value
     (a string pointed to a zarr store) into a downloadable file. To access the file you need to call the download
     method. This is done to avoid unnecessary requests to the datalayer api.
     """
 
     __file__ = True
 
@@ -438,14 +361,15 @@
 
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
 
+
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         # you could also return a string here which would mean model.post_code
         # would be a string, pydantic won't care but you could end up with some
         # confusion since the value's type won't match the type annotation
```

### Comparing `mikro-0.3.83/pyproject.toml` & `mikro-0.3.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,44 @@
 [tool.poetry]
 name = "mikro"
-version = "0.3.83"
+version = "0.3.9"
 description = "images for arkitekt"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "mikro" }]
 
 [tool.poetry.dependencies]
-python = "^3.8, <=3.12"
-zarr = "^2.14.2"
-xarray = ">=2022.12.0"
-s3fs = "^2023.1.0"
-pandas = "^1.5.3"
-pyarrow = { version = ">=11.0", python = ">=3.8", optional = true }
-dask = "^2023.3.0"
-rath = ">=0.4.0"
+python = "^3.8"
+zarr = "^2.11.1"
+xarray = "^2022.3.0"
+s3fs = "^2022.2.0"
+pandas = "^1.3.4"
+pyarrow = "^6.0.1"
+dask = "^2022.2.1"
+turms = { version = "^0.2.3", python = ">=3.9", optional = true }
+rath = ">=0.3.3"
 
 [tool.poetry.extras]
 turms = ["turms"]
-table = ["pyarrow"]
-complete = ["turms", "pyarrow"]
+complete = ["turms"]
 
-[tool.mypy]
-exclude = ["venv/"]
-ignore_missing_imports = true
-
-
-[tool.ruff]
-extend-select = ["ANN", "D1"]
-
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-]
-
-# Same as Black.
-line-length = 100
 
 [tool.poetry.group.dev.dependencies]
 testcontainers = "3.7.0"
 autoflake = "^1.7.7"
 pytest = "^7.2.0"
+PyQtWebEngine = "^5.15.5"
+PyQt5 = "^5.15.6"
+pytest-qt = "^4.2.0"
 pytest-asyncio = "^0.20.2"
-turms = { version = ">=0.3.1", python = "^3.9" }
+turms = { version = ">=0.2.3", python = "^3.9" }
 aiohttp = "^3.8.3"
 websockets = "^10.4"
-black = "^23.1.0"
+black = "^22.10.0"
 pytest-cov = "^4.0.0"
-pytest-aiohttp = "^1.0.4"
-ruff = "^0.0.254"
-mypy = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 qt_api = "pyqt5"
```

### Comparing `mikro-0.3.83/PKG-INFO` & `mikro-0.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mikro
-Version: 0.3.83
+Version: 0.3.9
 Summary: images for arkitekt
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
-Requires-Python: >=3.8,<=3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: complete
-Provides-Extra: table
 Provides-Extra: turms
-Requires-Dist: dask (>=2023.3.0,<2024.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pyarrow (>=11.0) ; (python_version >= "3.8") and (extra == "table" or extra == "complete")
-Requires-Dist: rath (>=0.4.0)
-Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
-Requires-Dist: xarray (>=2022.12.0)
-Requires-Dist: zarr (>=2.14.2,<3.0.0)
+Requires-Dist: dask (>=2022.2.1,<2023.0.0)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: pyarrow (>=6.0.1,<7.0.0)
+Requires-Dist: rath (>=0.3.3)
+Requires-Dist: s3fs (>=2022.2.0,<2023.0.0)
+Requires-Dist: turms (>=0.2.3,<0.3.0); (python_version >= "3.9") and (extra == "turms" or extra == "complete")
+Requires-Dist: xarray (>=2022.3.0,<2023.0.0)
+Requires-Dist: zarr (>=2.11.1,<3.0.0)
```

