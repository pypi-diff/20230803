# Comparing `tmp/mct-nightly-1.9.0.20230801.post450.tar.gz` & `tmp/mct-nightly-1.9.0.20230802.post405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.9.0.20230801.post450.tar", last modified: Tue Aug  1 00:04:51 2023, max compression
+gzip compressed data, was "mct-nightly-1.9.0.20230802.post405.tar", last modified: Wed Aug  2 00:04:06 2023, max compression
```

## Comparing `mct-nightly-1.9.0.20230801.post450.tar` & `mct-nightly-1.9.0.20230802.post405.tar`

### file list

```diff
@@ -1,532 +1,532 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.718755 mct-nightly-1.9.0.20230801.post450/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-08-01 00:04:51.718755 mct-nightly-1.9.0.20230801.post450/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.666754 mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-08-01 00:04:51.000000 mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33089 2023-08-01 00:04:51.000000 mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:04:51.000000 mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 00:04:51.000000 mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 00:04:51.000000 mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.666754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.666754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.670754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.674754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.678754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.678754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.678754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.682754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.682754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.682754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.682754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.686754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.686754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.686754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.686754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.686754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27259 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.690754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.694754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.694754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.694754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.694754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.694754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.694754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.698754 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.702755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/keras_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/pytorch_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.706755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.710755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.714755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.718755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.718755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:04:51.718755 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-01 00:04:05.000000 mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 00:04:51.718755 mct-nightly-1.9.0.20230801.post450/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 00:04:50.000000 mct-nightly-1.9.0.20230801.post450/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.209468 mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-08-02 00:04:05.000000 mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33089 2023-08-02 00:04:06.000000 mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:04:05.000000 mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 00:04:05.000000 mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 00:04:05.000000 mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.213468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.213468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.217468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.217468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.217468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.217468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.217468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.221468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.221468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.221468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.225468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.225468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25244 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.225468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.229468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.233468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.233468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.233468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.237468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.237468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.237468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.241468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.241468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.241468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.245468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.245468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.245468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.245468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.245468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.245468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.249468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.249468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.249468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.249468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.253468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.253468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25792 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.253468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.257468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.261468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.261468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.261468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.265468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.269468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.269468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.269468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.269468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.273468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.273468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.273468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.273468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/keras_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/pytorch_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.277468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.281468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.281468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.281468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.281468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.281468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.281468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.285468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.285468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.285468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.285468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.285468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.285468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.289468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.289468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.289468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.289468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.289468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.293468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:04:06.297468 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-02 00:03:18.000000 mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 00:04:06.301468 mct-nightly-1.9.0.20230802.post405/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 00:04:05.000000 mct-nightly-1.9.0.20230802.post405/setup.py
```

### Comparing `mct-nightly-1.9.0.20230801.post450/LICENSE.md` & `mct-nightly-1.9.0.20230802.post405/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/PKG-INFO` & `mct-nightly-1.9.0.20230802.post405/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230801.post450
+Version: 1.9.0.20230802.post405
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-1.9.0.20230801.post450/README.md` & `mct-nightly-1.9.0.20230802.post405/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230801.post450
+Version: 1.9.0.20230802.post405
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-1.9.0.20230801.post450/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.9.0.20230802.post405/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/constants.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 RANGE_MIN = 'range_min'
 RANGE_MAX = 'range_max'
 
 # BaseNode attributes
 REUSE = 'reuse'
 REUSE_GROUP = 'reuse_group'
 LAST_AXIS = -1
+AXIS = 'axis'
 
 # Data types:
 DATA_TYPE = 'dtype'
 FLOAT_32 = 'float32'
 
 # Number of Tensorboard cosine-similarity plots to add:
 NUM_SAMPLES_DISTANCE_TENSORBOARD = 20
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 # ==============================================================================
 import copy
 
 import numpy as np
 from typing import Callable, Any, List
 
+from model_compression_toolkit.constants import AXIS
 from model_compression_toolkit.core import FrameworkInfo, MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core.common import Graph, BaseNode
+from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.logger import Logger
 
 
 class SensitivityEvaluation:
     """
     Class to wrap and manage the computation on distance metric for Mixed-Precision quantization search.
@@ -274,20 +276,24 @@
 
         assert len(baseline_tensors) == len(self.interest_points)
         num_interest_points = len(baseline_tensors)
         num_samples = len(baseline_tensors[0])
         distance_matrix = np.ndarray((num_interest_points, num_samples))
 
         for i in range(num_interest_points):
+            point_node = self.interest_points[i]
             point_distance_fn = \
-                self.fw_impl.get_node_distance_fn(layer_class=self.interest_points[i].layer_class,
-                                                  framework_attrs=self.interest_points[i].framework_attr,
+                self.fw_impl.get_node_distance_fn(layer_class=point_node.layer_class,
+                                                  framework_attrs=point_node.framework_attr,
                                                   compute_distance_fn=self.quant_config.compute_distance_fn)
 
-            distance_matrix[i] = point_distance_fn(baseline_tensors[i], mp_tensors[i], batch=True)
+            axis = point_node.framework_attr.get(AXIS) if not isinstance(point_node, FunctionalNode) \
+                else point_node.op_call_kwargs.get(AXIS)
+
+            distance_matrix[i] = point_distance_fn(baseline_tensors[i], mp_tensors[i], batch=True, axis=axis)
 
         return distance_matrix
 
     def _build_distance_matrix(self):
         """
         Builds a matrix that contains the distances between the baseline and MP models for each interest point.
         Returns: A distance matrix.
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files 19% similar despite different names*

```diff
@@ -47,27 +47,34 @@
     Returns:
         Lp norm per sample in batch of tensor x.
     """
 
     return (np.abs(x) ** p).sum(axis=-1) ** (1.0/p)
 
 
-def flatten_tensor(t: np.ndarray, batch: bool) -> np.ndarray:
+def flatten_tensor(t: np.ndarray, batch: bool, axis: int = None) -> np.ndarray:
     """
     Flattening the samples batch to allow similarity analysis computation per sample.
 
     Args:
         t: A tensor to be flattened.
         batch: Whether the similarity computation is per image or per tensor.
+        axis: Axis along which the operator has been computed.
 
     Returns: A flattened tensor which has the number of samples as is first dimension.
 
     """
 
-    if batch:
+    if axis is not None and batch:
+        t = np.moveaxis(t, axis, -1)
+        f_t = t.reshape([t.shape[0], -1, t.shape[-1]])
+    elif axis is not None:
+        t = np.moveaxis(t, axis, -1)
+        f_t = t.reshape([-1, t.shape[-1]])
+    elif batch:
         f_t = t.reshape([t.shape[0], -1])
     else:
         f_t = t.flatten()
 
     return f_t
 
 #########################
@@ -75,24 +82,26 @@
 #########################
 
 
 def compute_mse(float_tensor: np.ndarray,
                 fxp_tensor: np.ndarray,
                 norm: bool = False,
                 norm_eps: float = 1e-8,
-                batch: bool = False) -> float:
+                batch: bool = False,
+                axis: int = None) -> float:
     """
     Compute the mean square error between two numpy arrays.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         norm: whether to normalize the error function result.
         norm_eps: epsilon value for error normalization stability.
         batch: Whether to run batch similarity analysis or not.
+        axis: Axis along which the operator has been computed (not used in this function).
 
     Returns:
         The MSE distance between the two tensors.
     """
     validate_before_compute_similarity(float_tensor, fxp_tensor)
 
     float_flat = flatten_tensor(float_tensor, batch)
@@ -105,24 +114,26 @@
     return error
 
 
 def compute_mae(float_tensor: np.ndarray,
                 fxp_tensor: np.ndarray,
                 norm: bool = False,
                 norm_eps: float = 1e-8,
-                batch: bool = False) -> float:
+                batch: bool = False,
+                axis: int = None) -> float:
     """
     Compute the mean average error function between two numpy arrays.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         norm: whether to normalize the error function result.
         norm_eps: epsilon value for error normalization stability.
         batch: Whether to run batch similarity analysis or not.
+        axis: Axis along which the operator has been computed (not used in this function).
 
     Returns:
         The mean average distance between the two tensors.
     """
 
     validate_before_compute_similarity(float_tensor, fxp_tensor)
 
@@ -131,25 +142,27 @@
 
     error = np.abs(float_flat - fxp_flat).mean(axis=-1)
     if norm:
         error /= (np.abs(float_flat).mean(axis=-1) + norm_eps)
     return error
 
 
-def compute_cs(float_tensor: np.ndarray, fxp_tensor: np.ndarray, eps: float = 1e-8, batch: bool = False) -> float:
+def compute_cs(float_tensor: np.ndarray, fxp_tensor: np.ndarray, eps: float = 1e-8, batch: bool = False,
+               axis: int = None) -> float:
     """
     Compute the similarity between two tensor using cosine similarity.
     The returned values is between 0 to 1: the smaller returned value,
     the greater similarity there is between the two tensors.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         eps: Small value to avoid zero division.
         batch: Whether to run batch similarity analysis or not.
+        axis: Axis along which the operator has been computed (not used in this function).
 
     Returns:
         The cosine similarity between two tensors.
     """
 
     validate_before_compute_similarity(float_tensor, fxp_tensor)
     if np.all(fxp_tensor == 0) and np.all(float_tensor == 0):
@@ -170,26 +183,28 @@
 
 
 def compute_lp_norm(float_tensor: np.ndarray,
                     fxp_tensor: np.ndarray,
                     p: int,
                     norm: bool = False,
                     norm_eps: float = 1e-8,
-                    batch: bool = False) -> float:
+                    batch: bool = False,
+                    axis: int = None) -> float:
     """
     Compute the error function between two numpy arrays.
     The error is computed based on Lp-norm distance of the tensors.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         p: p-norm to use for the Lp-norm distance.
         norm: whether to normalize the error function result.
         norm_eps: epsilon value for error normalization stability.
         batch: Whether to run batch similarity analysis or not.
+        axis: Axis along which the operator has been computed (not used in this function).
 
     Returns:
         The Lp-norm distance between the two tensors.
     """
     validate_before_compute_similarity(float_tensor, fxp_tensor)
 
     float_flat = flatten_tensor(float_tensor, batch)
@@ -197,31 +212,33 @@
 
     error = (np.abs(float_flat - fxp_flat) ** p).mean(axis=-1)
     if norm:
         error /= ((np.abs(float_flat) ** p).mean(axis=-1) + norm_eps)
     return error
 
 
-def compute_kl_divergence(float_tensor: np.ndarray, fxp_tensor: np.ndarray, batch: bool = False) -> float:
+def compute_kl_divergence(float_tensor: np.ndarray, fxp_tensor: np.ndarray, batch: bool = False,
+                          axis: int = None) -> float:
     """
     Compute the similarity between two tensor using KL-divergence.
     The returned values is between 0 to 1: the smaller returned value,
     the greater similarity there is between the two tensors.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         batch: Whether to run batch similarity analysis or not.
+        axis: Axis along which the operator has been computed.
 
     Returns:
         The KL-divergence between two tensors.
     """
 
     validate_before_compute_similarity(float_tensor, fxp_tensor)
 
-    float_flat = flatten_tensor(float_tensor, batch)
-    fxp_flat = flatten_tensor(fxp_tensor, batch)
+    float_flat = flatten_tensor(float_tensor, batch, axis)
+    fxp_flat = flatten_tensor(fxp_tensor, batch, axis)
 
     non_zero_fxp_tensor = fxp_flat.copy()
     non_zero_fxp_tensor[non_zero_fxp_tensor == 0] = EPS
 
-    return np.sum(np.where(float_flat != 0, float_flat * np.log(float_flat / non_zero_fxp_tensor), 0), axis=-1)
+    return np.mean(np.sum(np.where(float_flat != 0, float_flat * np.log(float_flat / non_zero_fxp_tensor), 0), axis=-1))
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,18 @@
         n_iter: The number of random iterations to calculate the approximated power of the Jacobian trace for each interest point.
         norm_weights: Whether to normalize the returned weights (to get values between 0 and 1).
 
     Returns: A list of (possibly normalized) jacobian-based weights to be considered as the relevancy that each interest
     point's output has on the model's output.
     """
 
+    if len(interest_points) == 1:
+        # Only one compare point, nothing else to "weight"
+        return [1.0]
+
     if not all([images.shape[0] == 1 for node, images in model_input_tensors.items()]):
         Logger.critical("Iterative jacobian trace computation is only supported on a single image sample")  # pragma: no cover
 
     with tf.GradientTape(persistent=True, watch_accessed_variables=False) as g:
         outputs, interest_points_tensors = _model_outputs_computation(graph_float,
                                                                       model_input_tensors,
                                                                       interest_points,
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,16 +413,16 @@
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
         if node.type == Activation:
             node_type_name = node.framework_attr[keras_constants.ACTIVATION]
             if node_type_name in [keras_constants.SOFTMAX, keras_constants.SIGMOID]:
                 return True
-        elif node.type in [tf.nn.softmax, tf.nn.sigmoid, Conv2D, DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate,
-                           Add, tf.add]:
+        elif node.type in [tf.nn.softmax, tf.keras.layers.Softmax, tf.nn.sigmoid, Conv2D, DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate,
+                           tf.concat, Add, tf.add]:
             return True
 
         return False
 
     def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None) -> Callable:
@@ -444,15 +444,16 @@
 
         if layer_class == Activation:
             node_type_name = framework_attrs[ACTIVATION]
             if node_type_name == SOFTMAX:
                 return compute_kl_divergence
             elif node_type_name == SIGMOID:
                 return compute_cs
-        elif layer_class == tf.nn.softmax:
+        elif layer_class == tf.nn.softmax or layer_class == tf.keras.layers.Softmax \
+                or (layer_class == TFOpLambda and SOFTMAX in framework_attrs[keras_constants.FUNCTION]):
             return compute_kl_divergence
         elif layer_class == tf.nn.sigmoid:
             return compute_cs
         elif layer_class == Dense:
             return compute_cs
         return compute_mse
 
@@ -503,15 +504,15 @@
 
         """
 
         if node.layer_class == TFOpLambda:
             node_attr = getattr(node, 'framework_attr', None)
             if node_attr is not None and (ARGMAX in node_attr[LAYER_NAME] or SOFTMAX in node_attr[LAYER_NAME]):
                 return False
-        elif node.layer_class == tf.nn.softmax or node.layer_class == tf.math.argmax:
+        elif node.layer_class in [tf.nn.softmax, tf.keras.layers.Softmax, tf.math.argmax]:
             return False
 
         return True
 
     def get_node_mac_operations(self,
                                 node: BaseNode,
                                 fw_info: FrameworkInfo) -> float:
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,18 @@
         n_iter: The number of random iterations to calculate the approximated power of the Jacobian trace for each interest point.
         norm_weights: Whether to normalize the returned weights (to get values between 0 and 1).
 
     Returns: A list of (possibly normalized) jacobian-based weights to be considered as the relevancy that each interest
     point's output has on the model's output.
     """
 
+    if len(interest_points) == 1:
+        # Only one compare point, nothing else to "weight"
+        return [1.0]
+
     # Set inputs to require_grad
     for n, input_tensor in model_input_tensors.items():
         input_tensor.requires_grad_()
 
     model_grads_net = PytorchModelGradients(graph_float=graph_float,
                                             interest_points=interest_points,
                                             output_list=output_list)
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,16 @@
         """
         Returns whether a given node in considered as a potential interest point for mp metric computation purposes.
         Args:
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
-        if node.type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax, softmax, operator.add, add, cat]:
+        if node.type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax, softmax, operator.add, add, cat,
+                         operator.concat]:
             return True
         return False
 
     def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None) -> Callable:
         """
@@ -462,15 +463,15 @@
         Args:
             node: A BaseNode object.
 
         Returns: Whether the node is compatible as output for metric computation or not.
 
         """
 
-        return node.layer_class not in [argmax, softmax]
+        return node.layer_class not in [argmax, softmax, Softmax]
 
     def get_node_mac_operations(self,
                                 node: BaseNode,
                                 fw_info: FrameworkInfo) -> float:
         """
         Gets the MAC operation count for a given operation.
```

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/core/runner.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/keras_quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/keras_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/legacy/pytorch_quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/legacy/pytorch_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/logger.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-1.9.0.20230802.post405/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230801.post450/setup.py` & `mct-nightly-1.9.0.20230802.post405/setup.py`

 * *Files identical despite different names*

