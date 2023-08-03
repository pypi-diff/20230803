# Comparing `tmp/finterion_investing_algorithm_framework-0.8-py3-none-any.whl.zip` & `tmp/finterion_investing_algorithm_framework-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10457 bytes, number of entries: 13
--rw-r--r--  2.0 unx      107 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/__init__.py
--rw-r--r--  2.0 unx     1455 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/create_app.py
--rw-r--r--  2.0 unx      197 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/exceptions.py
--rw-r--r--  2.0 unx     1948 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/market_service.py
--rw-r--r--  2.0 unx      102 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/configuration/__init__.py
--rw-r--r--  2.0 unx       93 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/configuration/constants.py
--rw-r--r--  2.0 unx      176 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/models/__init__.py
--rw-r--r--  2.0 unx      515 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework/models/portfolio_configuration.py
--rw-r--r--  2.0 unx    11343 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework-0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3289 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework-0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1462 b- defN 23-Aug-03 09:35 finterion_investing_algorithm_framework-0.8.dist-info/RECORD
-13 files, 20819 bytes uncompressed, 7877 bytes compressed:  62.2%
+Zip file size: 10655 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      107 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/__init__.py
+-rw-r--r--  2.0 unx     1455 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/create_app.py
+-rw-r--r--  2.0 unx      197 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/exceptions.py
+-rw-r--r--  2.0 unx     3223 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/market_service.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/configuration/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/configuration/constants.py
+-rw-r--r--  2.0 unx      176 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/models/__init__.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework/models/portfolio_configuration.py
+-rw-r--r--  2.0 unx    11343 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework-0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3289 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework-0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1462 b- defN 23-Aug-03 11:21 finterion_investing_algorithm_framework-0.9.dist-info/RECORD
+13 files, 22094 bytes uncompressed, 8075 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: finterion_investing_algorithm_framework/models/__init__.py
 Comment: 
 
 Filename: finterion_investing_algorithm_framework/models/portfolio_configuration.py
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.8.dist-info/LICENSE
+Filename: finterion_investing_algorithm_framework-0.9.dist-info/LICENSE
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.8.dist-info/METADATA
+Filename: finterion_investing_algorithm_framework-0.9.dist-info/METADATA
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.8.dist-info/WHEEL
+Filename: finterion_investing_algorithm_framework-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.8.dist-info/top_level.txt
+Filename: finterion_investing_algorithm_framework-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.8.dist-info/RECORD
+Filename: finterion_investing_algorithm_framework-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## finterion_investing_algorithm_framework/market_service.py

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 
 from investing_algorithm_framework.infrastructure.services import MarketService
+from investing_algorithm_framework import Order
 from finterion import Finterion
 
 
 class FinterionMarketService(MarketService):
 
     def __init__(self, api_key, base_url=None):
         self._api_key = api_key
@@ -14,18 +15,20 @@
         else:
             self._finterion = Finterion(api_key)
 
     def initialize(self, portfolio_configuration):
         pass
 
     def get_order(self, order):
-        return self._finterion.get_order(order.external_id)
+        order = self._finterion.get_order(order.external_id)
+        return self._conver_order(order)
 
     def get_orders(self, symbol, since: datetime = None):
-        return self._finterion.get_orders(symbol=symbol)
+        orders = self._finterion.get_orders(symbol=symbol)
+        return [self._conver_order(order) for order in orders]
 
     def get_balance(self):
         positions = self._finterion.get_positions()
         entries = {}
 
         for position in positions:
             entries[position["symbol"]] = {
@@ -36,40 +39,63 @@
 
     def create_market_sell_order(
         self,
         target_symbol: str,
         trading_symbol: str,
         amount: float,
     ):
-        return self._finterion.create_market_order(
+        order = self._finterion.create_market_order(
             order_side="sell",
             amount=amount,
             target_symbol=target_symbol,
         )
+        return self._conver_order(order)
 
     def create_limit_sell_order(
         self,
         target_symbol: str,
         trading_symbol: str,
         amount: float,
         price: float
     ):
-        return self._finterion.create_limit_order(
+        order = self._finterion.create_limit_order(
             order_side="sell",
             amount=amount,
             target_symbol=target_symbol,
             price=price
         )
+        return self._conver_order(order)
 
     def create_limit_buy_order(
         self,
         target_symbol: str,
         trading_symbol: str,
         amount: float,
         price: float
     ):
-        return self._finterion.create_limit_order(
+        order = self._finterion.create_limit_order(
             order_side="buy",
             amount=amount,
             target_symbol=target_symbol,
             price=price
         )
+        return self._conver_order(order)
+
+    def _conver_order(self, finterion_order):
+        return Order(
+            external_id=finterion_order.get("id"),
+            type=finterion_order.get("order_type"),
+            side=finterion_order.get("order_side"),
+            status=finterion_order.get("status"),
+            amount=finterion_order.get("amount"),
+            target_symbol=finterion_order.get("target_symbol"),
+            trading_symbol=finterion_order.get("trading_symbol"),
+            price=finterion_order.get("price"),
+            created_at=finterion_order.get("created_at"),
+            updated_at=finterion_order.get("updated_at"),
+            trade_closed_at=finterion_order.get("trade_closed_at"),
+            trade_closed_price=finterion_order.get("trade_closed_price"),
+            filled_amount=finterion_order.get("filled_amount"),
+            remaining_amount=finterion_order.get("remaining_amount"),
+            cost=finterion_order.get("cost"),
+            fee=finterion_order.get("fee"),
+        )
```

## Comparing `finterion_investing_algorithm_framework-0.8.dist-info/LICENSE` & `finterion_investing_algorithm_framework-0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `finterion_investing_algorithm_framework-0.8.dist-info/METADATA` & `finterion_investing_algorithm_framework-0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion-investing-algorithm-framework
-Version: 0.8
+Version: 0.9
 Summary: Official Finterion plugin for the investing algorithm framework
 Home-page: https://github.com/finterion/finterion-investing-algorithm-framework.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,investing-algorithm-framework,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: investing-algorithm-framework (>=1.3.1)
-Requires-Dist: finterion (>=0.5.2)
+Requires-Dist: finterion (>=0.6.0)
 
 # Finterion Investing Algorithm Framework Plugin
 This is the official plugin for the [investing algorithm framework](https://investing-algorithm-framework.com) open source project.
 
 ## Installation
 You can install the plugin with pip.
 ```shell
```

## Comparing `finterion_investing_algorithm_framework-0.8.dist-info/RECORD` & `finterion_investing_algorithm_framework-0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 finterion_investing_algorithm_framework/__init__.py,sha256=u-srn87VlLUPUJHWR5hgMAHqw2BWtb1v0eH0tQ8M16w,107
 finterion_investing_algorithm_framework/create_app.py,sha256=9ULhy8MR0yQNaSMXShri_YGpXreoI214hppZfqSqZ8Q,1455
 finterion_investing_algorithm_framework/exceptions.py,sha256=KOaDjHQC7vNpKwYYNxJ2nuaJYceMmvExW3BLSzPSWJk,197
-finterion_investing_algorithm_framework/market_service.py,sha256=viv_eQNPaY00akFMN3-i76E3vBLRO8_35Bef4UXx3aA,1948
+finterion_investing_algorithm_framework/market_service.py,sha256=127maeiI6fXd2yHkG2IrVpgU8q1_rTZ-xxJX5AU_Cos,3223
 finterion_investing_algorithm_framework/configuration/__init__.py,sha256=370OXcHya0GtGhrA59sIuznTYSn8xJy-dciCOSTsfl8,102
 finterion_investing_algorithm_framework/configuration/constants.py,sha256=bhabsdZ8omPvAZlQmdPGM70vHQHS2pcJm2olpkSEciU,93
 finterion_investing_algorithm_framework/models/__init__.py,sha256=96Cq_doBIVXfK9OJW3SnMTiXx9WPnd9LITlpT5vEFzw,176
 finterion_investing_algorithm_framework/models/portfolio_configuration.py,sha256=1QesgEDUDoPk50ZFsDZFpFNldP_PExoUgdhKHp3w908,515
-finterion_investing_algorithm_framework-0.8.dist-info/LICENSE,sha256=wbVEDvoZiMPHufRY3sLEffvAr7GH5hOIngHF8y4HFQg,11343
-finterion_investing_algorithm_framework-0.8.dist-info/METADATA,sha256=MjhyLBiOrtJJA3zY7PJ8lJ0KXiBpAQvr_eTRRwLQQMY,3289
-finterion_investing_algorithm_framework-0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-finterion_investing_algorithm_framework-0.8.dist-info/top_level.txt,sha256=B97hJPQAFX_vRhcLE8uVZ6ac3a5ndS79p-O8-C2y-zw,40
-finterion_investing_algorithm_framework-0.8.dist-info/RECORD,,
+finterion_investing_algorithm_framework-0.9.dist-info/LICENSE,sha256=wbVEDvoZiMPHufRY3sLEffvAr7GH5hOIngHF8y4HFQg,11343
+finterion_investing_algorithm_framework-0.9.dist-info/METADATA,sha256=58VY6DoxGNwtnvzWjH1DilYCRJQm-asXsje8FYRScbs,3289
+finterion_investing_algorithm_framework-0.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+finterion_investing_algorithm_framework-0.9.dist-info/top_level.txt,sha256=B97hJPQAFX_vRhcLE8uVZ6ac3a5ndS79p-O8-C2y-zw,40
+finterion_investing_algorithm_framework-0.9.dist-info/RECORD,,
```

