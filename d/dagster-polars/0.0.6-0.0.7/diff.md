# Comparing `tmp/dagster_polars-0.0.6.tar.gz` & `tmp/dagster_polars-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.6.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.7.tar", max compression
```

## Comparing `dagster_polars-0.0.6.tar` & `dagster_polars-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11344 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/LICENSE
--rw-r--r--   0        0        0     3911 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/README.md
--rw-r--r--   0        0        0      415 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/dagster_polars/__init__.py
--rw-r--r--   0        0        0       76 2023-07-30 21:04:40.356696 dagster_polars-0.0.6/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-30 21:04:07.793471 dagster_polars-0.0.6/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     7200 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/bigquery.py
--rw-r--r--   0        0        0     5027 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/delta.py
--rw-r--r--   0        0        0     2143 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0     3936 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/io_managers/utils.py
--rw-r--r--   0        0        0        0 2023-07-30 21:04:07.797472 dagster_polars-0.0.6/dagster_polars/py.typed
--rw-r--r--   0        0        0     2878 2023-07-30 21:04:40.356696 dagster_polars-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5250 1970-01-01 00:00:00.000000 dagster_polars-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3985 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/README.md
+-rw-r--r--   0        0        0      415 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       76 2023-08-03 09:59:32.223318 dagster_polars-0.0.7/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     6184 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     7200 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0     5027 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/io_managers/delta.py
+-rw-r--r--   0        0        0     2143 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     3936 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 09:58:54.824902 dagster_polars-0.0.7/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2878 2023-08-03 09:59:32.223318 dagster_polars-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 dagster_polars-0.0.7/PKG-INFO
```

### Comparing `dagster_polars-0.0.6/LICENSE` & `dagster_polars-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.6/README.md` & `dagster_polars-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # `dagster-polars`
 
 [Polars](https://github.com/pola-rs/polars) integration library for [Dagster](https://github.com/dagster-io/dagster).
 
+All IOManagers log various metadata about the DataFrame - size, schema, sample, stats.
+
+For all IOManagers the `columns` input metadata can be used to select a subset of columns to load.
+
 ## Features
- - All IOManagers log various metadata about the DataFrame - size, schema, sample, stats, ...
- - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
+   - doesn't raise an error on missing data if `Optional[...]` type annotation is used
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
      - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `mode`, `overwrite_schema` and `version` can be set via config parameters. `partition_by` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). The IOManager won't manage partitioning in this case, and all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
  - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
```

### Comparing `dagster_polars-0.0.6/dagster_polars/io_managers/base.py` & `dagster_polars-0.0.7/dagster_polars/io_managers/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from abc import abstractmethod
-from typing import Any, Dict, Mapping, Optional, Union
+from typing import Any, Dict, Mapping, Optional, Union, get_args, get_origin
 
 import polars as pl
 from dagster import (
     ConfigurableIOManager,
     InitResourceContext,
     InputContext,
     MetadataValue,
@@ -14,33 +14,45 @@
 )
 from dagster import _check as check
 from pydantic.fields import Field, PrivateAttr
 from upath import UPath
 
 from dagster_polars.io_managers.utils import get_polars_metadata
 
-POLARS_DATA_FRAME_ANNOTATIONS = [
+POLARS_EAGER_FRAME_ANNOTATIONS = [
     Any,
     pl.DataFrame,
+    Optional[pl.DataFrame],
     Dict[str, pl.DataFrame],
+    Dict[str, Optional[pl.DataFrame]],
     Mapping[str, pl.DataFrame],
+    Mapping[str, Optional[pl.DataFrame]],
     type(None),
     None,
 ]
 
 POLARS_LAZY_FRAME_ANNOTATIONS = [
     pl.LazyFrame,
+    Optional[pl.LazyFrame],
     Dict[str, pl.LazyFrame],
+    Dict[str, Optional[pl.LazyFrame]],
     Mapping[str, pl.LazyFrame],
+    Mapping[str, Optional[pl.LazyFrame]],
 ]
 
 
 if sys.version >= "3.9":
-    POLARS_DATA_FRAME_ANNOTATIONS.append(dict[str, pl.DataFrame])  # type: ignore
-    POLARS_LAZY_FRAME_ANNOTATIONS.append(dict[str, pl.DataFrame])  # type: ignore
+    POLARS_EAGER_FRAME_ANNOTATIONS.append(dict[str, pl.DataFrame])  # type: ignore
+    POLARS_EAGER_FRAME_ANNOTATIONS.append(dict[str, Optional[pl.DataFrame]])  # type: ignore
+    POLARS_LAZY_FRAME_ANNOTATIONS.append(dict[str, pl.LazyFrame])  # type: ignore
+    POLARS_LAZY_FRAME_ANNOTATIONS.append(dict[str, Optional[pl.LazyFrame]])  # type: ignore
+
+
+def annotation_is_typing_optional(annotation):
+    return get_origin(annotation) == Union and type(None) in get_args(annotation)
 
 
 class BasePolarsUPathIOManager(ConfigurableIOManager, UPathIOManager):
     # This is a base class which doesn't define the specific format (parquet, csv, etc) to use
     """
     `IOManager` for `polars` based on the `UPathIOManager`.
     Features:
@@ -69,25 +81,29 @@
     @abstractmethod
     def scan_df_from_path(self, path: UPath, context: InputContext) -> pl.LazyFrame:
         ...
 
     def dump_to_path(self, context: OutputContext, obj: pl.DataFrame, path: UPath):
         self.dump_df_to_path(context=context, df=obj, path=path)
 
-    def load_from_path(self, path: UPath, context: InputContext) -> Union[pl.DataFrame, pl.LazyFrame]:
+    def load_from_path(self, path: UPath, context: InputContext) -> Union[pl.DataFrame, pl.LazyFrame, None]:
+        if annotation_is_typing_optional(context.dagster_type.typing_type) and not path.exists():
+            context.log.warning(self.get_missing_optional_input_log_message(context, path))
+            return None
+
         assert context.metadata is not None
 
         ldf = self.scan_df_from_path(path=path, context=context)
 
         columns = context.metadata.get("columns")
         if columns is not None:
             context.log.debug(f"Loading {columns=}")
             ldf = ldf.select(columns)
 
-        if context.dagster_type.typing_type in POLARS_DATA_FRAME_ANNOTATIONS:
+        if context.dagster_type.typing_type in POLARS_EAGER_FRAME_ANNOTATIONS:
             return ldf.collect(streaming=True)
         elif context.dagster_type.typing_type in POLARS_LAZY_FRAME_ANNOTATIONS:
             return ldf
         else:
             raise NotImplementedError(f"Can't load object for type annotation {context.dagster_type.typing_type}")
 
     def get_metadata(self, context: OutputContext, obj: pl.DataFrame) -> Dict[str, MetadataValue]:
@@ -135,7 +151,10 @@
         ]
 
         asset_path = self._get_path_without_extension(context)
         return {
             partition: self._with_extension(self.get_path_for_partition(context, asset_path, partition))
             for partition in formatted_partition_keys
         }
+
+    def get_missing_optional_input_log_message(self, context: InputContext, path: UPath) -> str:
+        return f"Optional input {context.name} at {path} doesn't exist in the filesystem and won't be loaded!"
```

### Comparing `dagster_polars-0.0.6/dagster_polars/io_managers/bigquery.py` & `dagster_polars-0.0.7/dagster_polars/io_managers/bigquery.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.6/dagster_polars/io_managers/delta.py` & `dagster_polars-0.0.7/dagster_polars/io_managers/delta.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.6/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.0.7/dagster_polars/io_managers/parquet.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.6/dagster_polars/io_managers/utils.py` & `dagster_polars-0.0.7/dagster_polars/io_managers/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.6/pyproject.toml` & `dagster_polars-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.6"
+version = "0.0.7"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
```

### Comparing `dagster_polars-0.0.6/PKG-INFO` & `dagster_polars-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -30,19 +30,22 @@
 Project-URL: Repository, https://github.com/danielgafni/dagster-polars
 Description-Content-Type: text/markdown
 
 # `dagster-polars`
 
 [Polars](https://github.com/pola-rs/polars) integration library for [Dagster](https://github.com/dagster-io/dagster).
 
+All IOManagers log various metadata about the DataFrame - size, schema, sample, stats.
+
+For all IOManagers the `columns` input metadata can be used to select a subset of columns to load.
+
 ## Features
- - All IOManagers log various metadata about the DataFrame - size, schema, sample, stats, ...
- - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
  - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
+   - doesn't raise an error on missing data if `Optional[...]` type annotation is used
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark). All read/write options can be set via metadata values.
      - `PolarsDeltaIOManager` - for reading and writing Delta Lake. All read/write options can be set via metadata values. `mode`, `overwrite_schema` and `version` can be set via config parameters. `partition_by` metadata value can be set to use native Delta Lake partitioning (it's passed to `delta_write_options` of `write_delta`). The IOManager won't manage partitioning in this case, and all the asset partitions will be stored in the same Delta Table directory. You are responsible for filtering correct partitions when reading the data in the downstream assets. Extra dependencies can be installed with `pip install 'dagster-polars[deltalake]'`.
  - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified). Extra dependencies can be installed with `pip install 'dagster-polars[gcp]'`.
```

