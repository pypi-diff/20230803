# Comparing `tmp/flytekitplugins-great_expectations-1.8.3.tar.gz` & `tmp/flytekitplugins-great_expectations-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-great_expectations-1.8.3.tar", last modified: Thu Aug  3 17:08:12 2023, max compression
+gzip compressed data, was "flytekitplugins-great_expectations-1.9.0a0.tar", last modified: Thu Jul 20 18:58:18 2023, max compression
```

## Comparing `flytekitplugins-great_expectations-1.8.3.tar` & `flytekitplugins-great_expectations-1.9.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:12.912305 flytekitplugins-great_expectations-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 17:08:12.912305 flytekitplugins-great_expectations-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 17:07:50.000000 flytekitplugins-great_expectations-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:12.908305 flytekitplugins-great_expectations-1.8.3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:12.912305 flytekitplugins-great_expectations-1.8.3/flytekitplugins/great_expectations/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 17:07:50.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins/great_expectations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-08-03 17:07:50.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins/great_expectations/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-08-03 17:07:50.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins/great_expectations/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:12.912305 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 17:08:12.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 17:08:12.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:08:12.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:12.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 17:08:12.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:12.000000 flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:08:12.912305 flytekitplugins-great_expectations-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-03 17:08:08.000000 flytekitplugins-great_expectations-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.676671 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.676671 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 18:58:12.000000 flytekitplugins-great_expectations-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-great_expectations-1.8.3/PKG-INFO` & `flytekitplugins-great_expectations-1.9.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-great_expectations
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: Great Expectations Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-great_expectations-1.8.3/README.md` & `flytekitplugins-great_expectations-1.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-great_expectations-1.8.3/flytekitplugins/great_expectations/schema.py` & `flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-great_expectations-1.8.3/flytekitplugins/great_expectations/task.py` & `flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,26 +179,18 @@
                     "batch_spec_passthrough": self._batch_request_config.batch_spec_passthrough,
                 }
             )
 
             if is_runtime and issubclass(datatype, str):
                 final_batch_request["runtime_parameters"]["query"] = dataset
             elif is_runtime and issubclass(datatype, FlyteSchema):
-                # if execution engine is SparkDF, transform the data to pyspark.sql.dataframe.DataFrame, else transform the data
-                # to the default pandas.dataframe
-                if selected_datasource[0]["execution_engine"]["class_name"] == "SparkDFExecutionEngine":
-                    import pyspark
-
-                    final_batch_request["runtime_parameters"]["batch_data"] = dataset.open(
-                        pyspark.sql.dataframe.DataFrame
-                    ).all()
-                else:
-                    final_batch_request["runtime_parameters"]["batch_data"] = dataset.open().all()
+                final_batch_request["runtime_parameters"]["batch_data"] = dataset.open().all()
             else:
                 raise AssertionError("Can only use runtime_parameters for query(str)/schema data")
+
         # Great Expectations' BatchRequest
         elif self._batch_request_config:
             final_batch_request.update(
                 {
                     "data_connector_query": self._batch_request_config.data_connector_query,
                     "batch_spec_passthrough": self._batch_request_config.batch_spec_passthrough,
                 }
```

### Comparing `flytekitplugins-great_expectations-1.8.3/flytekitplugins_great_expectations.egg-info/PKG-INFO` & `flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-great-expectations
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: Great Expectations Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-great_expectations-1.8.3/setup.py` & `flytekitplugins-great_expectations-1.9.0a0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "great_expectations"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = [
-    "flytekit>=1.5.0,<2.0.0",
-    "great-expectations>=0.13.30",
-    "sqlalchemy>=1.4.23,<2.0.0",
-    "pyspark==3.3.1",
-    "flytekitplugins-spark>=1.5.0,<2.0.0",
-    "s3fs<2023.6.0",
-]
+plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "great-expectations>=0.13.30", "sqlalchemy>=1.4.23,<2.0.0"]
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Great Expectations Plugin for Flytekit",
```

