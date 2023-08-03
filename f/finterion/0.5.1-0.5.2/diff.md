# Comparing `tmp/finterion-0.5.1.tar.gz` & `tmp/finterion-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterion-0.5.1.tar", last modified: Wed Jul 26 14:27:08 2023, max compression
+gzip compressed data, was "finterion-0.5.2.tar", last modified: Wed Aug  2 21:53:57 2023, max compression
```

## Comparing `finterion-0.5.1.tar` & `finterion-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.988398 finterion-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-26 14:26:58.000000 finterion-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-26 14:27:08.988398 finterion-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 14:26:58.000000 finterion-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.984398 finterion-0.5.1/finterion/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.984398 finterion-0.5.1/finterion/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/configuration/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/finterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.988398 finterion-0.5.1/finterion/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/algorithm_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.984398 finterion-0.5.1/finterion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:27:08.988398 finterion-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-26 14:26:58.000000 finterion-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:53:57.205618 finterion-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-08-02 21:53:48.000000 finterion-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-02 21:53:57.205618 finterion-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-02 21:53:48.000000 finterion-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:53:57.205618 finterion-0.5.2/finterion/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:53:57.205618 finterion-0.5.2/finterion/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/configuration/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/finterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:53:57.205618 finterion-0.5.2/finterion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/algorithm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-08-02 21:53:48.000000 finterion-0.5.2/finterion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:53:57.205618 finterion-0.5.2/finterion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-02 21:53:57.000000 finterion-0.5.2/finterion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 21:53:57.000000 finterion-0.5.2/finterion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:53:57.000000 finterion-0.5.2/finterion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 21:53:57.000000 finterion-0.5.2/finterion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 21:53:57.000000 finterion-0.5.2/finterion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:53:57.205618 finterion-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-02 21:53:48.000000 finterion-0.5.2/setup.py
```

### Comparing `finterion-0.5.1/LICENSE` & `finterion-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/PKG-INFO` & `finterion-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.5.1
+Version: 0.5.2
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.5.1/README.md` & `finterion-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/configuration/urls.py` & `finterion-0.5.2/finterion/configuration/urls.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/finterion.py` & `finterion-0.5.2/finterion/finterion.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,27 +63,27 @@
             "target_symbol": target_symbol,
             "side": order_side,
             "type": order_type,
             "amount": amount,
             "price": price
         }
         return services.create_order(
-            self.api_key, data, base_url=self.base_url
+            self.api_key, base_url=self.base_url, data=data
         )
 
     def create_limit_order(self, target_symbol, order_side, amount, price):
         data = {
             "target_symbol": target_symbol,
             "side": order_side,
             "type": "LIMIT",
             "amount": amount,
             "price": price
         }
         return services.create_order(
-            self.api_key, data, base_url=self.base_url
+            api_key=self.api_key, data=data, base_url=self.base_url
         )
 
     def create_market_order(self, target_symbol, order_side, amount):
 
         if OrderSide.BUY.equals(order_side):
             raise ClientException(
                 "Market orders are not supported for BUY orders"
@@ -92,15 +92,15 @@
         data = {
             "target_symbol": target_symbol,
             "side": order_side,
             "type": "MARKET",
             "amount": amount,
         }
         return services.create_order(
-            self.api_key, data, base_url=self.base_url
+            api_key=self.api_key, data=data, base_url=self.base_url
         )
 
     def get_position(self, position_id):
         return services.get_position(
             self.api_key, position_id, base_url=self.base_url
         )
```

### Comparing `finterion-0.5.1/finterion/models/algorithm.py` & `finterion-0.5.2/finterion/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/algorithm_profile.py` & `finterion-0.5.2/finterion/models/algorithm_profile.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/order.py` & `finterion-0.5.2/finterion/models/order.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/order_side.py` & `finterion-0.5.2/finterion/models/order_side.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/order_status.py` & `finterion-0.5.2/finterion/models/order_status.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/order_type.py` & `finterion-0.5.2/finterion/models/order_type.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/portfolio.py` & `finterion-0.5.2/finterion/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/models/position.py` & `finterion-0.5.2/finterion/models/position.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion/services.py` & `finterion-0.5.2/finterion/services.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/finterion.egg-info/PKG-INFO` & `finterion-0.5.2/finterion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.5.1
+Version: 0.5.2
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.5.1/finterion.egg-info/SOURCES.txt` & `finterion-0.5.2/finterion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterion-0.5.1/setup.py` & `finterion-0.5.2/setup.py`

 * *Files identical despite different names*

