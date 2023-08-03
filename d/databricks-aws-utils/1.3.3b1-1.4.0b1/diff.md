# Comparing `tmp/databricks_aws_utils-1.3.3b1.tar.gz` & `tmp/databricks_aws_utils-1.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_aws_utils-1.3.3b1.tar", max compression
+gzip compressed data, was "databricks_aws_utils-1.4.0b1.tar", max compression
```

## Comparing `databricks_aws_utils-1.3.3b1.tar` & `databricks_aws_utils-1.4.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2021-11-22 20:10:33.420205 databricks_aws_utils-1.3.3b1/LICENSE
--rw-r--r--   0        0        0      489 2021-11-22 20:21:50.459403 databricks_aws_utils-1.3.3b1/README.md
--rw-r--r--   0        0        0     2087 2021-11-22 20:10:54.570545 databricks_aws_utils-1.3.3b1/databricks_aws_utils/__init__.py
--rw-r--r--   0        0        0    11831 2023-07-25 10:15:22.221825 databricks_aws_utils-1.3.3b1/databricks_aws_utils/delta_table.py
--rw-r--r--   0        0        0     4331 2021-11-22 20:10:54.576363 databricks_aws_utils-1.3.3b1/databricks_aws_utils/rds.py
--rw-r--r--   0        0        0     2174 2021-11-22 20:10:54.577305 databricks_aws_utils-1.3.3b1/databricks_aws_utils/s3.py
--rw-r--r--   0        0        0     1499 2021-11-22 20:10:54.578167 databricks_aws_utils-1.3.3b1/databricks_aws_utils/session.py
--rw-r--r--   0        0        0      961 2023-07-25 10:15:34.229899 databricks_aws_utils-1.3.3b1/pyproject.toml
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.3b1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-11-22 20:10:33.420205 databricks_aws_utils-1.4.0b1/LICENSE
+-rw-r--r--   0        0        0      489 2021-11-22 20:21:50.459403 databricks_aws_utils-1.4.0b1/README.md
+-rw-r--r--   0        0        0     2087 2021-11-22 20:10:54.570545 databricks_aws_utils-1.4.0b1/databricks_aws_utils/__init__.py
+-rw-r--r--   0        0        0    12212 2023-07-25 10:27:54.566105 databricks_aws_utils-1.4.0b1/databricks_aws_utils/delta_table.py
+-rw-r--r--   0        0        0     4331 2021-11-22 20:10:54.576363 databricks_aws_utils-1.4.0b1/databricks_aws_utils/rds.py
+-rw-r--r--   0        0        0     2174 2021-11-22 20:10:54.577305 databricks_aws_utils-1.4.0b1/databricks_aws_utils/s3.py
+-rw-r--r--   0        0        0     1499 2021-11-22 20:10:54.578167 databricks_aws_utils-1.4.0b1/databricks_aws_utils/session.py
+-rw-r--r--   0        0        0      961 2023-08-03 09:47:19.119531 databricks_aws_utils-1.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 databricks_aws_utils-1.4.0b1/PKG-INFO
```

### Comparing `databricks_aws_utils-1.3.3b1/LICENSE` & `databricks_aws_utils-1.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.3b1/databricks_aws_utils/__init__.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.3b1/databricks_aws_utils/delta_table.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/delta_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from typing import Any, Dict, List, Optional, Tuple
 
 import botocore
 from delta.tables import DeltaTable
+from pyspark.sql.catalog import Column
 from pyspark.sql.session import SparkSession
 
 from databricks_aws_utils import DatabrickAWSUtils
 
 
 class DeltaTableUtils(DatabrickAWSUtils):
     """
@@ -185,41 +186,58 @@
         """
         columns = []
         partitions = []
         self.logger.info("Extracting table schema...")
         delta_columns = self.spark.catalog.listColumns(self.name)
 
         for column in delta_columns:
-            data_type = column.dataType
-
-            if self._is_data_type_truncated(data_type):
-                self.logger.warning(f"Data type for the column '{column.name}' is truncated, " +
-                                    "using the Spark SQL to extract the data type")
-                col_details = self.spark.sql(f"DESC TABLE FORMATTED {self.name} {column.name}").collect()
-                row = next((row for row in col_details if row.info_name == "data_type"), None)
-                if row:
-                    data_type = row.info_value
-                else:
-                    data_type = 'string'
-                    self.logger.warning(f"Data type for the column '{column.name}' not found, using 'string'")
-
             col = {
                 'Name': column.name,
-                'Type': data_type,
+                'Type': self._get_column_data_type(column),
                 'Comment': column.description or ''
             }
             if column.isPartition:
                 partitions.append(col)
             else:
                 columns.append(col)
 
         self.logger.debug(f"Columns: {columns}")
         self.logger.debug(f"Partitions: {partitions}")
         return columns, partitions
 
+    def _get_column_data_type(self, column: Column) -> str:
+        """
+        Resolve the column data type.
+
+        If the data type is truncated, the method uses the Spark SQL to extract the data type.
+
+        Args:
+            column (`Column`): column object
+
+        Returns:
+            `str`: column data type
+        """
+        data_type = column.dataType
+
+        if self._is_data_type_truncated(data_type):
+            self.logger.warning(f"Data type for the column '{column.name}' is truncated, " +
+                                "using the Spark SQL to extract the data type")
+
+            col_details = self.spark.sql(f"DESC TABLE FORMATTED {self.name} {column.name}").collect()
+
+            row = next((row for row in col_details if row.info_name == "data_type"), None)
+
+            if row:
+                data_type = row.info_value
+            else:
+                data_type = 'string'
+                self.logger.warning(f"Data type for the column '{column.name}' not found, using 'string'")
+
+        return data_type
+
     def _is_data_type_truncated(self, value: str) -> bool:
         """
         Identify if the data type value returned by the spark.catalog.listColumns is truncated.
 
         Pattern: `2 more fields`
 
         Args:
```

### Comparing `databricks_aws_utils-1.3.3b1/databricks_aws_utils/rds.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/rds.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.3b1/databricks_aws_utils/s3.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/s3.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.3b1/databricks_aws_utils/session.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/session.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.3b1/pyproject.toml` & `databricks_aws_utils-1.4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "databricks-aws-utils"
-version = "1.3.3b1"
+version = "1.4.0b1"
 description = "Databricks AWS Utils"
 license = "Proprietary"
 authors = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 maintainers = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 readme = "README.md"
 repository = "https://github.com/lucasvieirasilva/databricks-aws-utils"
 
   [[tool.poetry.packages]]
   include = "databricks_aws_utils"
 
   [tool.poetry.dependencies]
-  python = ">=3.7,<3.10"
+  python = ">=3.7,<3.11"
 
   [tool.poetry.group.dev.dependencies]
   flake8 = "3.9.2"
   autopep8 = "1.5.7"
   delta-spark = "^2.3.0"
   pyspark = "3.3.2"
   boto3 = "1.20.5"
```

### Comparing `databricks_aws_utils-1.3.3b1/PKG-INFO` & `databricks_aws_utils-1.4.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: databricks-aws-utils
-Version: 1.3.3b1
+Version: 1.4.0b1
 Summary: Databricks AWS Utils
 Home-page: https://github.com/lucasvieirasilva/databricks-aws-utils
 License: Proprietary
 Author: Lucas Vieira
 Author-email: lucas.vieira94@outlook.com
 Maintainer: Lucas Vieira
 Maintainer-email: lucas.vieira94@outlook.com
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Project-URL: Repository, https://github.com/lucasvieirasilva/databricks-aws-utils
 Description-Content-Type: text/markdown
 
 # Databricks AWS Utils
 
 Databricks AWS Utils is a library to abstract Databricks integration with AWS Services
```

