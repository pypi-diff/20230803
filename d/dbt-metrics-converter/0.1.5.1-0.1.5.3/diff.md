# Comparing `tmp/dbt_metrics_converter-0.1.5.1.tar.gz` & `tmp/dbt_metrics_converter-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_metrics_converter-0.1.5.1.tar", max compression
+gzip compressed data, was "dbt_metrics_converter-0.1.5.3.tar", max compression
```

## Comparing `dbt_metrics_converter-0.1.5.1.tar` & `dbt_metrics_converter-0.1.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1820 2023-07-27 02:07:20.857604 dbt_metrics_converter-0.1.5.1/README.md
--rw-r--r--   0        0        0        0 2023-06-27 22:07:13.604392 dbt_metrics_converter-0.1.5.1/converter/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-27 02:07:53.646399 dbt_metrics_converter-0.1.5.1/converter/dbt_metrics_to_semantic_model_converter.py
--rwxr-xr-x   0        0        0     1035 2023-07-27 02:07:20.857952 dbt_metrics_converter-0.1.5.1/converter/main.py
--rw-r--r--   0        0        0     3378 2023-06-29 20:23:23.763615 dbt_metrics_converter-0.1.5.1/converter/spec_upgrade.py
--rw-r--r--   0        0        0        0 2023-06-27 22:07:13.606341 dbt_metrics_converter-0.1.5.1/metricflow_parsing/__init__.py
--rw-r--r--   0        0        0     1807 2023-06-27 22:07:13.606510 dbt_metrics_converter-0.1.5.1/metricflow_parsing/dbt_dir_to_model.py
--rw-r--r--   0        0        0    19978 2023-06-27 22:07:13.606691 dbt_metrics_converter-0.1.5.1/metricflow_parsing/dbt_to_metricflow.py
--rw-r--r--   0        0        0      612 2023-07-27 02:15:17.755470 dbt_metrics_converter-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 dbt_metrics_converter-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1820 2023-07-27 02:07:20.857604 dbt_metrics_converter-0.1.5.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 22:07:13.604392 dbt_metrics_converter-0.1.5.3/converter/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-27 02:07:53.646399 dbt_metrics_converter-0.1.5.3/converter/dbt_metrics_to_semantic_model_converter.py
+-rwxr-xr-x   0        0        0     1035 2023-07-27 02:07:20.857952 dbt_metrics_converter-0.1.5.3/converter/main.py
+-rw-r--r--   0        0        0     3378 2023-06-29 20:23:23.763615 dbt_metrics_converter-0.1.5.3/converter/spec_upgrade.py
+-rw-r--r--   0        0        0        0 2023-06-27 22:07:13.606341 dbt_metrics_converter-0.1.5.3/metricflow_parsing/__init__.py
+-rw-r--r--   0        0        0     1807 2023-06-27 22:07:13.606510 dbt_metrics_converter-0.1.5.3/metricflow_parsing/dbt_dir_to_model.py
+-rw-r--r--   0        0        0    19978 2023-08-03 00:27:49.630003 dbt_metrics_converter-0.1.5.3/metricflow_parsing/dbt_to_metricflow.py
+-rw-r--r--   0        0        0      612 2023-08-03 00:39:46.320478 dbt_metrics_converter-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 dbt_metrics_converter-0.1.5.3/PKG-INFO
```

### Comparing `dbt_metrics_converter-0.1.5.1/README.md` & `dbt_metrics_converter-0.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.5.1/converter/dbt_metrics_to_semantic_model_converter.py` & `dbt_metrics_converter-0.1.5.3/converter/dbt_metrics_to_semantic_model_converter.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.5.1/converter/main.py` & `dbt_metrics_converter-0.1.5.3/converter/main.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.5.1/converter/spec_upgrade.py` & `dbt_metrics_converter-0.1.5.3/converter/spec_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.5.1/metricflow_parsing/dbt_dir_to_model.py` & `dbt_metrics_converter-0.1.5.3/metricflow_parsing/dbt_dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.5.1/metricflow_parsing/dbt_to_metricflow.py` & `dbt_metrics_converter-0.1.5.3/metricflow_parsing/dbt_to_metricflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         forms the individual statment '{field} {operator} {value}' and joins
         them with an 'AND'. Thus we do the same.
 
         Note:
             TODO: We could probably replace this with whatever method dbt uses to
             build the statement.
         """
-        clauses = [f"{{{{dimension(\'{filter.field}\')}}}} {filter.operator} {filter.value}" for filter in filters]
+        clauses = [f"{{{{Dimension(\'{filter.field}\')}}}} {filter.operator} {filter.value}" for filter in filters]
         return " AND ".join(clauses)
 
     def build_proxy_metric(self, dbt_metric: DbtMetric) -> PydanticMetric:
         """Attempt to build a proxy metric for the given DbtMetric
 
         For DbtMetrics which have a calculation method != 'derived',
         we have separately created a measure of the appropriate type.
```

### Comparing `dbt_metrics_converter-0.1.5.1/pyproject.toml` & `dbt_metrics_converter-0.1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-metrics-converter"
-version = "0.1.5.1"
+version = "0.1.5.3"
 description = "Easily convert an out of date dbt metrics spec into the latest suported metrics spec in dbt"
 authors = ["Jordan Stein <jordan.stein77@gmail.com>"]
 readme = "README.md"
 packages = [{include = "converter"},{include = "metricflow_parsing"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
```

### Comparing `dbt_metrics_converter-0.1.5.1/PKG-INFO` & `dbt_metrics_converter-0.1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-metrics-converter
-Version: 0.1.5.1
+Version: 0.1.5.3
 Summary: Easily convert an out of date dbt metrics spec into the latest suported metrics spec in dbt
 Author: Jordan Stein
 Author-email: jordan.stein77@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

