# Comparing `tmp/dbt-graph-builder-0.5.0.tar.gz` & `tmp/dbt-graph-builder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.5.0.tar", last modified: Fri Jul  7 10:22:12 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.6.0.tar", last modified: Thu Aug  3 11:49:29 2023, max compression
```

## Comparing `dbt-graph-builder-0.5.0.tar` & `dbt-graph-builder-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.485221 dbt-graph-builder-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.807108 dbt-graph-builder-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-03 11:49:11.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:49:29.811108 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 11:49:29.000000 dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/top_level.txt
```

### Comparing `dbt-graph-builder-0.5.0/LICENSE` & `dbt-graph-builder-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.5.0/PKG-INFO` & `dbt-graph-builder-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.5.0
+Version: 0.6.0
 Summary: DBT Graph Builder
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-graph-builder
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
 [![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
 
 ## Overview
 This library provides a set of tools for building a graph of dbt models and their dependencies. It can be used to create an Airflow DAG for dbt models
 or to create a graph of dbt models and their dependencies in a format that can be used by other tools like GCP Workflows.
```

### Comparing `dbt-graph-builder-0.5.0/README.md` & `dbt-graph-builder-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # dbt-graph-builder
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
 [![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
 
 ## Overview
 This library provides a set of tools for building a graph of dbt models and their dependencies. It can be used to create an Airflow DAG for dbt models
 or to create a graph of dbt models and their dependencies in a format that can be used by other tools like GCP Workflows.
```

### Comparing `dbt-graph-builder-0.5.0/pyproject.toml` & `dbt-graph-builder-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.5.0/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.6.0/src/dbt_graph_builder/builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         dbt_airflow_graph.add_external_dependencies(manifest)
     dbt_airflow_graph.create_edges_from_dependencies(graph_config.enable_dags_dependencies)
     if not graph_config.show_ephemeral_models:
         LOGGER.debug("Removing ephemeral nodes from graph")
         dbt_airflow_graph.remove_ephemeral_nodes_from_graph()
     LOGGER.debug("Contracting test nodes")
     dbt_airflow_graph.contract_test_nodes()
+    LOGGER.debug("Creating multple deps tests dependencies")
+    dbt_airflow_graph.create_multiple_deps_test_dependencies(graph_config.check_all_deps_for_multiple_deps_tests)
     return dbt_airflow_graph
 
 
 def load_dbt_manifest(manifest_path: os.PathLike[str] | str) -> dict[str, Any]:
     """Load dbt manifest.
 
     Args:
```

### Comparing `dbt-graph-builder-0.5.0/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.6.0/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.5.0/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.6.0/src/dbt_graph_builder/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 class GraphConfiguration:
     """Graph configuration."""
 
     gateway_config: GatewayConfiguration = field(default_factory=_default_gateway_config)
     dbt_manifest_props: dict[str, str] = field(default_factory=dict)
     enable_dags_dependencies: bool = False
     show_ephemeral_models: bool = False
+    check_all_deps_for_multiple_deps_tests: bool = False
 
 
 class DbtManifestGraph:
     """DbtManifestGraph class is used to create a DAG from DBT manifest.json file."""
 
     def __init__(self, configuration: GraphConfiguration) -> None:
         """Create DbtManifestGraph.
@@ -161,14 +162,59 @@
                 itertools.product(
                     list(self._graph.predecessors(node_name)),
                     list(self._graph.successors(node_name)),
                 )
             )
             self._graph.remove_node(node_name)
 
+    def create_multiple_deps_test_dependencies(self, check_all_predecessors: bool) -> None:
+        """Create edges from dependencies to multiple deps test.
+
+        Args:
+            check_all_predecessors (bool): If True, check all predecessors when creating dependencies.
+                Defaults to False.
+        """
+        for test_node_name, node in self._graph.nodes(data=True):
+            if node["node_type"] != NodeType.MULTIPLE_DEPS_TEST:
+                continue
+            for node_name in self._graph.nodes():
+                if self._check_if_node_predecessors_are_superset_of_test_deps(
+                    node_name, test_node_name, check_all_predecessors=check_all_predecessors
+                ):
+                    self._graph.add_edge(test_node_name, node_name)
+
+    def _get_all_node_predecessors(self, node_name: str) -> set[str]:
+        predecessors: set[str] = set()
+        node_predecessors = set(self._graph.predecessors(node_name))
+        predecessors |= node_predecessors
+        for predecessor in node_predecessors:
+            predecessors |= self._get_all_node_predecessors(predecessor)
+        return predecessors
+
+    def _check_if_node_predecessors_are_superset_of_test_deps(
+        self, node_name: str, test_node_name: str, check_all_predecessors: bool
+    ) -> bool:
+        node = self._graph.nodes[node_name]
+        test_node = self._graph.nodes[test_node_name]
+        if node["node_type"] != NodeType.RUN_TEST:
+            return False
+        test_deps: set[str] = set(test_node["depends_on"])
+        if node_name in test_deps:
+            return False
+        if test_deps.issubset(set(node["depends_on"])):
+            return True
+        if not check_all_predecessors:
+            return False
+        predecessors = self._get_all_node_predecessors(node_name)
+        if not test_deps.issubset(predecessors):
+            return False
+        if test_node_name in predecessors:
+            return False
+        return True
+
     def contract_test_nodes(self) -> None:
         """Contract test nodes."""
         tests_with_more_deps = self._get_test_with_multiple_deps_names_by_deps()
         for depends_on_tuple, test_node_names in tests_with_more_deps.items():
             self._contract_test_nodes_same_deps(depends_on_tuple, test_node_names)
 
     def get_default_node_values(self, manifest_node: dict[str, Any]) -> dict[str, Any]:
@@ -236,20 +282,21 @@
 
     def _get_test_with_multiple_deps_names_by_deps(
         self,
     ) -> dict[tuple[str, ...], list[str]]:
         tests_with_more_deps: dict[tuple[str, ...], list[str]] = {}
 
         for node_name, node in self._graph.nodes(data=True):
-            if node["node_type"] == NodeType.MULTIPLE_DEPS_TEST:
-                model_dependencies = node["depends_on"]
-                model_dependencies.sort()
-                if tuple(model_dependencies) not in tests_with_more_deps:
-                    tests_with_more_deps[tuple(model_dependencies)] = []
-                tests_with_more_deps[tuple(model_dependencies)].append(node_name)
+            if node["node_type"] != NodeType.MULTIPLE_DEPS_TEST:
+                continue
+            model_dependencies: list[str] = sorted(node["depends_on"])
+            test_key = tuple(model_dependencies)
+            if test_key not in tests_with_more_deps:
+                tests_with_more_deps[test_key] = []
+            tests_with_more_deps[test_key].append(node_name)
 
         return tests_with_more_deps
 
     def _contract_test_nodes_same_deps(self, depends_on_tuple: tuple[str, ...], test_node_names: list[str]) -> None:
         test_names = [self._graph.nodes[test_node]["select"] for test_node in test_node_names]
 
         first_test_node = test_node_names[0]
```

### Comparing `dbt-graph-builder-0.5.0/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.6.0/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.5.0/src/dbt_graph_builder/workflow.py` & `dbt-graph-builder-0.6.0/src/dbt_graph_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.6.0/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.5.0
+Version: 0.6.0
 Summary: DBT Graph Builder
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-graph-builder
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
 [![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
 
 ## Overview
 This library provides a set of tools for building a graph of dbt models and their dependencies. It can be used to create an Airflow DAG for dbt models
 or to create a graph of dbt models and their dependencies in a format that can be used by other tools like GCP Workflows.
```

