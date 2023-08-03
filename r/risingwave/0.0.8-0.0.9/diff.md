# Comparing `tmp/risingwave-0.0.8.tar.gz` & `tmp/risingwave-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risingwave-0.0.8.tar", last modified: Tue Jun 13 10:36:45 2023, max compression
+gzip compressed data, was "risingwave-0.0.9.tar", last modified: Thu Aug  3 08:22:26 2023, max compression
```

## Comparing `risingwave-0.0.8.tar` & `risingwave-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-06-13 10:36:45.251929 risingwave-0.0.8/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-06-13 10:36:45.251782 risingwave-0.0.8/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.8/README.md
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-06-13 10:36:45.250857 risingwave-0.0.8/risingwave/
--rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.8/risingwave/__init__.py
--rw-r--r--   0 wangrunji   (501) staff       (20)     3120 2023-05-18 08:37:35.000000 risingwave-0.0.8/risingwave/test_udf.py
--rw-r--r--   0 wangrunji   (501) staff       (20)    13962 2023-06-13 10:35:58.000000 risingwave-0.0.8/risingwave/udf.py
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-06-13 10:36:45.251560 risingwave-0.0.8/risingwave.egg-info/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)      251 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       23 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/requires.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/top_level.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-06-13 10:36:45.251987 risingwave-0.0.8/setup.cfg
--rw-r--r--   0 wangrunji   (501) staff       (20)      647 2023-06-13 10:35:58.000000 risingwave-0.0.8/setup.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-08-03 08:22:26.272343 risingwave-0.0.9/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     4190 2023-08-03 08:22:26.272189 risingwave-0.0.9/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)     3834 2023-07-03 08:11:05.000000 risingwave-0.0.9/README.md
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-08-03 08:22:26.269754 risingwave-0.0.9/risingwave/
+-rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.9/risingwave/__init__.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)     5919 2023-06-21 07:14:23.000000 risingwave-0.0.9/risingwave/test_udf.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)    16772 2023-08-03 07:09:14.000000 risingwave-0.0.9/risingwave/udf.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-08-03 08:22:26.272002 risingwave-0.0.9/risingwave.egg-info/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     4190 2023-08-03 08:22:26.000000 risingwave-0.0.9/risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)      251 2023-08-03 08:22:26.000000 risingwave-0.0.9/risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-08-03 08:22:26.000000 risingwave-0.0.9/risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       23 2023-08-03 08:22:26.000000 risingwave-0.0.9/risingwave.egg-info/requires.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-08-03 08:22:26.000000 risingwave-0.0.9/risingwave.egg-info/top_level.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-08-03 08:22:26.272379 risingwave-0.0.9/setup.cfg
+-rw-r--r--   0 wangrunji   (501) staff       (20)      647 2023-06-21 07:14:23.000000 risingwave-0.0.9/setup.py
```

### Comparing `risingwave-0.0.8/risingwave/udf.py` & `risingwave-0.0.9/risingwave/udf.py`

 * *Files 20% similar despite different names*

```diff
@@ -338,15 +338,34 @@
         )
 
     def add_function(self, udf: UserDefinedFunction):
         """Add a function to the server."""
         name = udf._name
         if name in self._functions:
             raise ValueError("Function already exists: " + name)
-        print("added function:", name)
+
+        input_types = ",".join(
+            [_data_type_to_string(t) for t in udf._input_schema.types]
+        )
+        if isinstance(udf, TableFunction):
+            output_type = udf._result_schema.types[-1]
+            if isinstance(output_type, pa.StructType):
+                output_type = ",".join(
+                    f"field_{i} {_data_type_to_string(field.type)}"
+                    for i, field in enumerate(output_type)
+                )
+                output_type = f"TABLE({output_type})"
+            else:
+                output_type = _data_type_to_string(output_type)
+                output_type = f"TABLE(output {output_type})"
+        else:
+            output_type = _data_type_to_string(udf._result_schema.types[-1])
+
+        sql = f"CREATE FUNCTION {name}({input_types}) RETURNS {output_type} AS '{name}' USING LINK 'http://{self._location}';"
+        print(f"added function: {name}, corresponding SQL:\n{sql}\n")
         self._functions[name] = udf
 
     def do_exchange(self, context, descriptor, reader, writer):
         """Call a function from the client."""
         udf = self._functions[descriptor.path[0].decode("utf-8")]
         writer.begin(udf._result_schema)
         try:
@@ -356,63 +375,123 @@
                     writer.write_batch(output_batch)
         except Exception as e:
             print(traceback.print_exc())
             raise e
 
     def serve(self):
         """Start the server."""
-        print(f"listening on {self._location}")
+        print(
+            "Note: You can use arbitrary function names and struct field names in CREATE FUNCTION statements."
+            f"\n\nlistening on {self._location}"
+        )
         super(UdfServer, self).serve()
 
 
 def _to_data_type(t: Union[str, pa.DataType]) -> pa.DataType:
     """
-    Convert a string or pyarrow.DataType to pyarrow.DataType.
+    Convert a SQL data type string or `pyarrow.DataType` to `pyarrow.DataType`.
     """
     if isinstance(t, str):
         return _string_to_data_type(t)
     else:
         return t
 
 
 def _string_to_data_type(type_str: str):
+    """
+    Convert a SQL data type string to `pyarrow.DataType`.
+    """
     type_str = type_str.upper()
-    if type_str in ("BOOLEAN", "BOOL"):
+    if type_str.endswith("[]"):
+        return pa.list_(_string_to_data_type(type_str[:-2]))
+    elif type_str in ("BOOLEAN", "BOOL"):
         return pa.bool_()
     elif type_str in ("SMALLINT", "INT2"):
         return pa.int16()
     elif type_str in ("INT", "INTEGER", "INT4"):
         return pa.int32()
     elif type_str in ("BIGINT", "INT8"):
         return pa.int64()
     elif type_str in ("FLOAT4", "REAL"):
         return pa.float32()
     elif type_str in ("FLOAT8", "DOUBLE PRECISION"):
         return pa.float64()
     elif type_str.startswith("DECIMAL") or type_str.startswith("NUMERIC"):
-        return pa.decimal128(28)
+        if type_str == "DECIMAL" or type_str == "NUMERIC":
+            return pa.decimal128(38)
+        rest = type_str[8:-1]  # remove "DECIMAL(" and ")"
+        if "," in rest:
+            precision, scale = rest.split(",")
+            return pa.decimal128(int(precision), int(scale))
+        else:
+            return pa.decimal128(int(rest), 0)
     elif type_str in ("DATE"):
         return pa.date32()
     elif type_str in ("TIME", "TIME WITHOUT TIME ZONE"):
-        return pa.time32("ms")
+        return pa.time64("us")
     elif type_str in ("TIMESTAMP", "TIMESTAMP WITHOUT TIME ZONE"):
-        return pa.timestamp("ms")
+        return pa.timestamp("us")
     elif type_str.startswith("INTERVAL"):
-        return pa.duration("us")
+        return pa.month_day_nano_interval()
     elif type_str in ("VARCHAR"):
         return pa.string()
     elif type_str in ("JSONB"):
         return pa.large_string()
     elif type_str in ("BYTEA"):
         return pa.binary()
-    elif type_str.endswith("[]"):
-        return pa.list_(_string_to_data_type(type_str[:-2]))
     elif type_str.startswith("STRUCT"):
         # extract 'STRUCT<INT, VARCHAR, ...>'
         type_list = type_str[6:].strip("<>")
         fields = []
         for type_str in type_list.split(","):
             type_str = type_str.strip()
             fields.append(pa.field("", _string_to_data_type(type_str)))
         return pa.struct(fields)
 
     raise ValueError(f"Unsupported type: {type_str}")
+
+
+def _data_type_to_string(t: pa.DataType) -> str:
+    """
+    Convert a `pyarrow.DataType` to a SQL data type string.
+    """
+    if isinstance(t, pa.ListType):
+        return _data_type_to_string(t.value_type) + "[]"
+    elif t.equals(pa.bool_()):
+        return "BOOLEAN"
+    elif t.equals(pa.int16()):
+        return "SMALLINT"
+    elif t.equals(pa.int32()):
+        return "INT"
+    elif t.equals(pa.int64()):
+        return "BIGINT"
+    elif t.equals(pa.float32()):
+        return "FLOAT4"
+    elif t.equals(pa.float64()):
+        return "FLOAT8"
+    elif t.equals(pa.decimal128(38)):
+        return "DECIMAL"
+    elif t.equals(pa.date32()):
+        return "DATE"
+    elif t.equals(pa.time64("us")):
+        return "TIME"
+    elif t.equals(pa.timestamp("us")):
+        return "TIMESTAMP"
+    elif t.equals(pa.month_day_nano_interval()):
+        return "INTERVAL"
+    elif t.equals(pa.string()):
+        return "VARCHAR"
+    elif t.equals(pa.large_string()):
+        return "JSONB"
+    elif t.equals(pa.binary()):
+        return "BYTEA"
+    elif isinstance(t, pa.StructType):
+        return (
+            "STRUCT<"
+            + ",".join(
+                f"field_{i} {_data_type_to_string(field.type)}"
+                for i, field in enumerate(t)
+            )
+            + ">"
+        )
+    else:
+        raise ValueError(f"Unsupported type: {t}")
```

### Comparing `risingwave-0.0.8/setup.py` & `risingwave-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="risingwave",
-    version="0.0.8",
+    version="0.0.9",
     author="RisingWave Labs",
     description="RisingWave Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/risingwavelabs/risingwave",
     packages=find_packages(),
     classifiers=[
```

