# Comparing `tmp/gridworks-0.2.7.tar.gz` & `tmp/gridworks-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.7.tar", max compression
+gzip compressed data, was "gridworks-0.2.8.tar", max compression
```

## Comparing `gridworks-0.2.7.tar` & `gridworks-0.2.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1065 2023-06-25 19:40:25.796958 gridworks-0.2.7/LICENSE
--rw-r--r--   0        0        0     5587 2023-06-25 19:40:42.877121 gridworks-0.2.7/README.md
--rw-r--r--   0        0        0     2579 2023-06-25 19:40:42.877121 gridworks-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      249 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/__main__.py
--rw-r--r--   0        0        0    51618 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2016 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0    23522 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/base_g_node.py
--rw-r--r--   0        0        0     6726 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6405 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0     5011 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/g_node_strategy.py
--rw-r--r--   0        0        0      694 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1214 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2547 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     2734 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/errors.py
--rw-r--r--   0        0        0     8749 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/message.py
--rw-r--r--   0        0        0    17029 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     1476 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    20321 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/base_g_node_gt.py
--rw-r--r--   0        0        0    24525 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0        0 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     5788 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/utils.py
--rw-r--r--   0        0        0      788 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks_test/__init__.py
--rw-r--r--   0        0        0     6947 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks_test/stub_actors.py
--rw-r--r--   0        0        0     4047 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks_test/wait.py
--rw-r--r--   0        0        0     7078 1970-01-01 00:00:00.000000 gridworks-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-03 16:39:47.639297 gridworks-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5584 2023-08-03 16:40:08.451467 gridworks-0.2.8/README.md
+-rw-r--r--   0        0        0     2562 2023-08-03 16:40:08.451467 gridworks-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    51618 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6726 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6405 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0     5011 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/g_node_strategy.py
+-rw-r--r--   0        0        0      694 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1214 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2547 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     2734 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/errors.py
+-rw-r--r--   0        0        0     8749 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/utils.py
+-rw-r--r--   0        0        0      788 2023-08-03 16:39:47.727298 gridworks-0.2.8/src/gridworks_test/__init__.py
+-rw-r--r--   0        0        0     6947 2023-08-03 16:39:47.727298 gridworks-0.2.8/src/gridworks_test/stub_actors.py
+-rw-r--r--   0        0        0     4047 2023-08-03 16:39:47.727298 gridworks-0.2.8/src/gridworks_test/wait.py
+-rw-r--r--   0        0        0     7036 1970-01-01 00:00:00.000000 gridworks-0.2.8/PKG-INFO
```

### Comparing `gridworks-0.2.7/LICENSE` & `gridworks-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/README.md` & `gridworks-0.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,15 @@
 
 ## Usage
 
 `pip install gridworks` to install the foundational package.
 
 ## RabbitMQ Infrastructure
 
-GridWorks uses the  `rabbit` subfolder for maintaining dev rabbit brokers as well as their own live rabbit brokers. 
-
+GridWorks uses the `rabbit` subfolder for maintaining dev rabbit brokers as well as their own live rabbit brokers.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `gridworks-0.2.7/pyproject.toml` & `gridworks-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.7"
+version = "0.2.8"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
@@ -29,15 +29,14 @@
 
 pika = "^1.3.1"
 pika-stubs = "^0.1.3"
 beaker-pyteal = "^0.4.0"
 fastapi-utils = "^0.2.1"
 uvicorn = {extras = ["standard"], version = "^0.19.0"}
 requests = "^2.28.1"
-rich = "^12.6.0"
 requests-async = "^0.6.2"
 types-requests = "^2.28.11.2"
 aiocache = {version = "^0.11.1", extras = ["redis,memcached"]}
 aioredis = "1.3.1"
 sphinx-rtd-theme = "^1.1.1" # move to dev dependencies. Look to cookie cutter online help.
```

### Comparing `gridworks-0.2.7/src/gridworks/actor_base.py` & `gridworks-0.2.8/src/gridworks/actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/algo_utils.py` & `gridworks-0.2.8/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/api_utils.py` & `gridworks-0.2.8/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/base_api_types.py` & `gridworks-0.2.8/src/gridworks/base_api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/base_g_node.py` & `gridworks-0.2.8/src/gridworks/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.8/src/gridworks/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.8/src/gridworks/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/g_node_strategy.py` & `gridworks-0.2.8/src/gridworks/data_classes/g_node_strategy.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.8/src/gridworks/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.8/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.8/src/gridworks/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.8/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/__init__.py` & `gridworks-0.2.8/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.8/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.8/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.8/src/gridworks/enums/g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.8/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/gni_status.py` & `gridworks-0.2.8/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.8/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.8/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.8/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/message_category.py` & `gridworks-0.2.8/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.8/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.8/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/strategy_name.py` & `gridworks-0.2.8/src/gridworks/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.8/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/enums/universe_type.py` & `gridworks-0.2.8/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/gw_config.py` & `gridworks-0.2.8/src/gridworks/gw_config.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/message.py` & `gridworks-0.2.8/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/property_format.py` & `gridworks-0.2.8/src/gridworks/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/rest_api.py` & `gridworks-0.2.8/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/__init__.py` & `gridworks-0.2.8/src/gridworks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/base_g_node_gt.py` & `gridworks-0.2.8/src/gridworks/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.8/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.8/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.8/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.8/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.8/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/ready.py` & `gridworks-0.2.8/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.8/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/super_starter.py` & `gridworks-0.2.8/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.8/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks/utils.py` & `gridworks-0.2.8/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks_test/__init__.py` & `gridworks-0.2.8/src/gridworks_test/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks_test/stub_actors.py` & `gridworks-0.2.8/src/gridworks_test/stub_actors.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/src/gridworks_test/wait.py` & `gridworks-0.2.8/src/gridworks_test/wait.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.7/PKG-INFO` & `gridworks-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.7
+Version: 0.2.8
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,14 @@
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pika-stubs (>=0.1.3,<0.2.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pytz (>=2022.7,<2023.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-async (>=0.6.2,<0.7.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: types-requests (>=2.28.11.2,<3.0.0.0)
 Requires-Dist: uvicorn[standard] (>=0.19.0,<0.20.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks/releases
 Project-URL: Documentation, https://gridworks.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks
 Description-Content-Type: text/markdown
@@ -87,16 +86,15 @@
 
 ## Usage
 
 `pip install gridworks` to install the foundational package.
 
 ## RabbitMQ Infrastructure
 
-GridWorks uses the  `rabbit` subfolder for maintaining dev rabbit brokers as well as their own live rabbit brokers. 
-
+GridWorks uses the `rabbit` subfolder for maintaining dev rabbit brokers as well as their own live rabbit brokers.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

