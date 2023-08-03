# Comparing `tmp/dbt-graph-builder-0.6.0.tar.gz` & `tmp/dbt-graph-builder-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.6.0.tar", last modified: Thu Aug  3 11:49:29 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.6.1.tar", last modified: Thu Aug  3 12:11:03 2023, max compression
```

## Comparing `dbt-graph-builder-0.6.0.tar` & `dbt-graph-builder-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.807108 dbt-graph-builder-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/top_level.txt
```

### Comparing `dbt-graph-builder-0.6.0/LICENSE` & `dbt-graph-builder-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/PKG-INFO` & `dbt-graph-builder-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.6.0
+Version: 0.6.1
 Summary: DBT Graph Builder
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dbt-graph-builder-0.6.0/README.md` & `dbt-graph-builder-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/pyproject.toml` & `dbt-graph-builder-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.6.1/src/dbt_graph_builder/builder.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.6.1/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.6.1/src/dbt_graph_builder/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,18 +196,20 @@
         node = self._graph.nodes[node_name]
         test_node = self._graph.nodes[test_node_name]
         if node["node_type"] != NodeType.RUN_TEST:
             return False
         test_deps: set[str] = set(test_node["depends_on"])
         if node_name in test_deps:
             return False
-        if test_deps.issubset(set(node["depends_on"])):
-            return True
         if not check_all_predecessors:
-            return False
+            if not test_deps.issubset(set(node["depends_on"])):
+                return False
+            if test_node_name in self._get_all_node_predecessors(node_name):
+                return False
+            return True
         predecessors = self._get_all_node_predecessors(node_name)
         if not test_deps.issubset(predecessors):
             return False
         if test_node_name in predecessors:
             return False
         return True
```

### Comparing `dbt-graph-builder-0.6.0/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.6.1/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/src/dbt_graph_builder/workflow.py` & `dbt-graph-builder-0.6.1/src/dbt_graph_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.6.0
+Version: 0.6.1
 Summary: DBT Graph Builder
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

