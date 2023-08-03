# Comparing `tmp/ngdataenginterface-0.1.2.tar.gz` & `tmp/ngdataenginterface-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.1.2.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.1.3.tar", max compression
```

## Comparing `ngdataenginterface-0.1.2.tar` & `ngdataenginterface-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2934 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/README.md
--rw-r--r--   0        0        0      348 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0     3778 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/analytical.py
--rw-r--r--   0        0        0     3392 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/aws_interface.py
--rw-r--r--   0        0        0     2704 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/process.py
--rw-r--r--   0        0        0      517 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/__init__.py
--rw-r--r--   0        0        0     2124 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/create_analytical_tables.py
--rw-r--r--   0        0        0     1516 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/landing_to_raw.py
--rw-r--r--   0        0        0     2015 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/raw_to_trusted.py
--rw-r--r--   0        0        0     1508 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/trusted_to_analytics.py
--rw-r--r--   0        0        0     1850 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/spark_manager.py
--rw-r--r--   0        0        0    13389 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/table.py
--rw-r--r--   0        0        0     2720 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/utils.py
--rw-r--r--   0        0        0      395 2023-06-26 16:53:29.875136 ngdataenginterface-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/README.md
+-rw-r--r--   0        0        0      348 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0     3778 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/analytical.py
+-rw-r--r--   0        0        0     3392 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/aws_interface.py
+-rw-r--r--   0        0        0     2704 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/process.py
+-rw-r--r--   0        0        0      517 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/scripts/__init__.py
+-rw-r--r--   0        0        0     2124 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/scripts/create_analytical_tables.py
+-rw-r--r--   0        0        0     1516 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/scripts/landing_to_raw.py
+-rw-r--r--   0        0        0     2015 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/scripts/raw_to_trusted.py
+-rw-r--r--   0        0        0     1508 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/scripts/trusted_to_analytics.py
+-rw-r--r--   0        0        0     1850 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/spark_manager.py
+-rw-r--r--   0        0        0    13389 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/table.py
+-rw-r--r--   0        0        0     2720 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/ngdataenginterface/utils.py
+-rw-r--r--   0        0        0      395 2023-08-03 18:33:45.743506 ngdataenginterface-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.3/PKG-INFO
```

### Comparing `ngdataenginterface-0.1.2/README.md` & `ngdataenginterface-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/analytical.py` & `ngdataenginterface-0.1.3/ngdataenginterface/analytical.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/aws_interface.py` & `ngdataenginterface-0.1.3/ngdataenginterface/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/process.py` & `ngdataenginterface-0.1.3/ngdataenginterface/process.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/scripts/__init__.py` & `ngdataenginterface-0.1.3/ngdataenginterface/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/scripts/create_analytical_tables.py` & `ngdataenginterface-0.1.3/ngdataenginterface/scripts/create_analytical_tables.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/scripts/landing_to_raw.py` & `ngdataenginterface-0.1.3/ngdataenginterface/scripts/landing_to_raw.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/scripts/raw_to_trusted.py` & `ngdataenginterface-0.1.3/ngdataenginterface/scripts/raw_to_trusted.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/scripts/trusted_to_analytics.py` & `ngdataenginterface-0.1.3/ngdataenginterface/scripts/trusted_to_analytics.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/spark_manager.py` & `ngdataenginterface-0.1.3/ngdataenginterface/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/table.py` & `ngdataenginterface-0.1.3/ngdataenginterface/table.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/ngdataenginterface/utils.py` & `ngdataenginterface-0.1.3/ngdataenginterface/utils.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.2/PKG-INFO` & `ngdataenginterface-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataenginterface
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for facilitating the development of data engineering pipelines
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

