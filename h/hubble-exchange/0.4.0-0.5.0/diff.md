# Comparing `tmp/hubble_exchange-0.4.0.tar.gz` & `tmp/hubble_exchange-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.4.0.tar", last modified: Tue Jul 25 07:26:08 2023, max compression
+gzip compressed data, was "hubble_exchange-0.5.0.tar", last modified: Thu Aug  3 07:50:07 2023, max compression
```

## Comparing `hubble_exchange-0.4.0.tar` & `hubble_exchange-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.069373 hubble_exchange-0.4.0/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.4.0/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.4.0/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)     6421 2023-07-25 07:26:08.069117 hubble_exchange-0.4.0/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     4764 2023-07-25 07:13:22.000000 hubble_exchange-0.4.0/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.067297 hubble_exchange-0.4.0/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      369 2023-07-25 06:59:23.000000 hubble_exchange-0.4.0/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     7500 2023-07-25 07:15:33.000000 hubble_exchange-0.4.0/hubble_exchange/client.py
--rw-r--r--   0 shubham    (501) staff       (20)      202 2023-07-25 07:14:44.000000 hubble_exchange-0.4.0/hubble_exchange/constants.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.068671 hubble_exchange-0.4.0/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    15194 2023-07-25 05:55:50.000000 hubble_exchange-0.4.0/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.4.0/hubble_exchange/eip712.py
--rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.4.0/hubble_exchange/errors.py
--rw-r--r--   0 shubham    (501) staff       (20)     5612 2023-07-25 07:10:52.000000 hubble_exchange-0.4.0/hubble_exchange/eth.py
--rw-r--r--   0 shubham    (501) staff       (20)     3467 2023-07-25 06:36:39.000000 hubble_exchange-0.4.0/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)     5176 2023-07-25 07:14:09.000000 hubble_exchange-0.4.0/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)      562 2023-07-22 11:56:49.000000 hubble_exchange-0.4.0/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.068510 hubble_exchange-0.4.0/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     6421 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      531 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       88 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-07-25 07:16:14.000000 hubble_exchange-0.4.0/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-07-25 07:26:08.069455 hubble_exchange-0.4.0/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.4.0/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.958679 hubble_exchange-0.5.0/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.5.0/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.5.0/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)     8140 2023-08-03 07:50:07.958531 hubble_exchange-0.5.0/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     6483 2023-08-03 07:06:01.000000 hubble_exchange-0.5.0/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.955711 hubble_exchange-0.5.0/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      369 2023-07-25 06:59:23.000000 hubble_exchange-0.5.0/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)    10087 2023-08-03 07:48:30.000000 hubble_exchange-0.5.0/hubble_exchange/client.py
+-rw-r--r--   0 shubham    (501) staff       (20)      288 2023-08-03 07:09:05.000000 hubble_exchange-0.5.0/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.958101 hubble_exchange-0.5.0/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    17033 2023-08-02 10:06:29.000000 hubble_exchange-0.5.0/hubble_exchange/contract_abis/AMM.json
+-rw-r--r--   0 shubham    (501) staff       (20)    23347 2023-08-02 10:07:52.000000 hubble_exchange-0.5.0/hubble_exchange/contract_abis/ClearingHouse.json
+-rw-r--r--   0 shubham    (501) staff       (20)    17505 2023-08-02 10:26:02.000000 hubble_exchange-0.5.0/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.5.0/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.5.0/hubble_exchange/errors.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5612 2023-08-03 07:46:15.000000 hubble_exchange-0.5.0/hubble_exchange/eth.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3730 2023-08-02 07:54:20.000000 hubble_exchange-0.5.0/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)     6175 2023-08-03 07:47:45.000000 hubble_exchange-0.5.0/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)      562 2023-07-22 11:56:49.000000 hubble_exchange-0.5.0/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.956586 hubble_exchange-0.5.0/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     8140 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      619 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       88 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-08-03 07:49:51.000000 hubble_exchange-0.5.0/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-08-03 07:50:07.958718 hubble_exchange-0.5.0/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.5.0/setup.py
```

### Comparing `hubble_exchange-0.4.0/LICENSE` & `hubble_exchange-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.4.0/PKG-INFO` & `hubble_exchange-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.4.0
+Version: 0.5.0
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,41 +61,42 @@
 async def main():
 
     async def callback(response):
         print(f"Received response: {response}")
         return response
 
     client = HubbleClient(os.getenv("PRIVATE_KEY"))
-    # place an order for market = 0, amount = 0.2, price = 1800, reduce_only = False
-    order = await client.place_single_order(0, 0.2, 1800, False, callback)
+
+    # get a dict of all market ids and names - for example {0: "ETH-Perp", 1: "AVAX-Perp"}
+    markets = await client.get_markets()
 
     # place multiple orders at once
     orders = []
     orders.append(Order.new(3, 1, 1.2, False)) # market = 3, qty = 1, price = 1.2, reduce_only = False
     orders.append(Order.new(0, 0.1, 1800, False)) # market = 0, qty = 0.1, price = 1800, reduce_only = False
     # placed_orders list will contain the order ids for the orders placed
-    placed_orders = await client.place_orders(orders, callback)
+    placed_orders = await client.place_orders(orders, True, callback)
 
     # get order status
-    order_status = await client.get_order_status(order.Id, callback)
+    order_status = await client.get_order_status(order.id, callback)
     
     # cancel an order
-    await client.cancel_orders([order], callback)
+    await client.cancel_orders([order], True, True, callback)
 
     # order can also be cancelled by order id
-    await client.cancel_order_by_id(order.id, callback)
+    await client.cancel_order_by_id(order.id, True, callback)
 
     # get current order book for market = 1
     order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
     positions = await client.get_margin_and_positions(callback)
 
     # get order fills
-    order_fills = await client.get_order_fills
+    order_fills = await client.get_order_fills()
 
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
     async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
     asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
@@ -123,14 +124,43 @@
 placed_orders = await client.place_orders(orders, callback, {
     "gas": 500_000,
     "maxFeePerGas": Web3.to_wei(80, 'gwei'),
     "maxPriorityFeePerGas": Web3.to_wei(20, 'gwei'),
 })
 ```
 
+## Trader feed
+
+All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
+It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
+```
+
+## Market feed
+
+All trades of a particular market can be subscribed to using the `subscribe_to_market_updates` method.
+Similar to the trader feed, it has 2 confirmation modes - head block or accepted block.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    # subscribe to market id 0
+    await client.subscribe_to_market_updates(0, ConfirmationMode.accepted, callback)
+```
+
 ## Transaction modes
 
 There are different modes in which the client can wait for acknowledgement of the transaction. The default behaviour is to send the transaction and not wait for the acknowledgement.
 This can be changed by explicitly asking the function to wait while sending the trasaction.
 
 - TransactionMode.no_wait: The default behaviour is to send transactions to the blockchain and NOT wait for the acknowledgement.
 - TransactionMode.wait_for_head: Wait for the transaction to be included in the canonical chain. At this time the block is preferred but not yet finalized. However, once the block in included in the canonical chain, the matching engine will start processing the order.
@@ -143,20 +173,19 @@
 placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
 # or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
 
-## Trader feed
+## Waiting for response in place_orders and cancel_orders
 
-All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
-It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+The `place_orders` and `cancel_orders` methods can be called in 2 modes - wait for response or don't wait for response.
+To get the acknowledgement of the transaction, use wait_for_response=True. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
+When using wait_for_response=True, the sdk will automatically set the transaction mode to TransactionMode.wait_for_accept because the response can be confirmed only after the transaction is mined.
 
-```python
-import os
-from hubble_exchange import HubbleClient, ConfirmationMode
+Alternatively, the client can also use trader feed to listen to all the updates. This is faster when done with ConfirmationMode.head
 
-async def main():
-    client = HubbleClient(os.getenv("PRIVATE_KEY"))
-    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
-```
+## Atomic in cancel_orders
+
+The `cancel_orders` method can be called in 2 modes - atomic or non-atomic. In atomic mode, all the orders will be cancelled only if all the orders are successfully cancelled. In non-atomic mode, the orders will be cancelled one by one and the response will be a list of dicts with order ids and success boolean.
+When used in combination with wait_for_response=True, the response will be a list of dicts with order ids and success boolean.
```

### Comparing `hubble_exchange-0.4.0/README.md` & `hubble_exchange-0.5.0/hubble_exchange.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: hubble-exchange
+Version: 0.5.0
+Summary: Official python SDK for Hubble Exchange
+Author-email: Lumos <lumos@hubble.exchange>
+License: MIT License
+        
+        Copyright (c) 2023 Hubble Exchange
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/hubble-exchange/python-sdk
+Keywords: hubble,exchange,orderbook,perpetual,futures,dex,sdk,python,avalanche,ethereum,web3,crypto
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Python SDK for Hubble Exchange
 
 [Hubble Exchange](https://hubble.exchange) is a Layer 1 Blockchain for a Decentralised Perps OrderBook
 <br>[Twitter](https://twitter.com/HubbleExchange)
 
 
 ## Installation
@@ -28,41 +61,42 @@
 async def main():
 
     async def callback(response):
         print(f"Received response: {response}")
         return response
 
     client = HubbleClient(os.getenv("PRIVATE_KEY"))
-    # place an order for market = 0, amount = 0.2, price = 1800, reduce_only = False
-    order = await client.place_single_order(0, 0.2, 1800, False, callback)
+
+    # get a dict of all market ids and names - for example {0: "ETH-Perp", 1: "AVAX-Perp"}
+    markets = await client.get_markets()
 
     # place multiple orders at once
     orders = []
     orders.append(Order.new(3, 1, 1.2, False)) # market = 3, qty = 1, price = 1.2, reduce_only = False
     orders.append(Order.new(0, 0.1, 1800, False)) # market = 0, qty = 0.1, price = 1800, reduce_only = False
     # placed_orders list will contain the order ids for the orders placed
-    placed_orders = await client.place_orders(orders, callback)
+    placed_orders = await client.place_orders(orders, True, callback)
 
     # get order status
-    order_status = await client.get_order_status(order.Id, callback)
+    order_status = await client.get_order_status(order.id, callback)
     
     # cancel an order
-    await client.cancel_orders([order], callback)
+    await client.cancel_orders([order], True, True, callback)
 
     # order can also be cancelled by order id
-    await client.cancel_order_by_id(order.id, callback)
+    await client.cancel_order_by_id(order.id, True, callback)
 
     # get current order book for market = 1
     order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
     positions = await client.get_margin_and_positions(callback)
 
     # get order fills
-    order_fills = await client.get_order_fills
+    order_fills = await client.get_order_fills()
 
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
     async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
     asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
@@ -90,14 +124,43 @@
 placed_orders = await client.place_orders(orders, callback, {
     "gas": 500_000,
     "maxFeePerGas": Web3.to_wei(80, 'gwei'),
     "maxPriorityFeePerGas": Web3.to_wei(20, 'gwei'),
 })
 ```
 
+## Trader feed
+
+All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
+It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
+```
+
+## Market feed
+
+All trades of a particular market can be subscribed to using the `subscribe_to_market_updates` method.
+Similar to the trader feed, it has 2 confirmation modes - head block or accepted block.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    # subscribe to market id 0
+    await client.subscribe_to_market_updates(0, ConfirmationMode.accepted, callback)
+```
+
 ## Transaction modes
 
 There are different modes in which the client can wait for acknowledgement of the transaction. The default behaviour is to send the transaction and not wait for the acknowledgement.
 This can be changed by explicitly asking the function to wait while sending the trasaction.
 
 - TransactionMode.no_wait: The default behaviour is to send transactions to the blockchain and NOT wait for the acknowledgement.
 - TransactionMode.wait_for_head: Wait for the transaction to be included in the canonical chain. At this time the block is preferred but not yet finalized. However, once the block in included in the canonical chain, the matching engine will start processing the order.
@@ -110,20 +173,19 @@
 placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
 # or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
 
-## Trader feed
+## Waiting for response in place_orders and cancel_orders
 
-All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
-It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+The `place_orders` and `cancel_orders` methods can be called in 2 modes - wait for response or don't wait for response.
+To get the acknowledgement of the transaction, use wait_for_response=True. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
+When using wait_for_response=True, the sdk will automatically set the transaction mode to TransactionMode.wait_for_accept because the response can be confirmed only after the transaction is mined.
 
-```python
-import os
-from hubble_exchange import HubbleClient, ConfirmationMode
+Alternatively, the client can also use trader feed to listen to all the updates. This is faster when done with ConfirmationMode.head
 
-async def main():
-    client = HubbleClient(os.getenv("PRIVATE_KEY"))
-    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
-```
+## Atomic in cancel_orders
+
+The `cancel_orders` method can be called in 2 modes - atomic or non-atomic. In atomic mode, all the orders will be cancelled only if all the orders are successfully cancelled. In non-atomic mode, the orders will be cancelled one by one and the response will be a list of dicts with order ids and success boolean.
+When used in combination with wait_for_response=True, the response will be a list of dicts with order ids and success boolean.
```

### Comparing `hubble_exchange-0.4.0/hubble_exchange/client.py` & `hubble_exchange-0.5.0/hubble_exchange/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 from typing import Dict, List
 
 import websockets
 from hexbytes import HexBytes
 
+from hubble_exchange.eip712 import get_order_hash
 from hubble_exchange.eth import get_async_web3_client, get_websocket_endpoint
 from hubble_exchange.models import (AsyncOrderBookDepthCallback,
                                     AsyncOrderStatusCallback,
                                     AsyncPlaceOrdersCallback,
                                     AsyncPositionCallback,
                                     AsyncSubscribeToOrderBookDepthCallback,
-                                    ConfirmationMode, Order,
+                                    ConfirmationMode, MarketFeedUpdate, Order,
                                     OrderBookDepthUpdateResponse,
                                     OrderStatusResponse, TraderFeedUpdate,
                                     WebsocketResponse)
 from hubble_exchange.order_book import OrderBookClient, TransactionMode
 from hubble_exchange.utils import (float_to_scaled_int,
                                    get_address_from_private_key, get_new_salt)
 
@@ -30,27 +31,30 @@
         self.web3_client = get_async_web3_client()
         self.websocket_endpoint = get_websocket_endpoint()
         self.order_book_client = OrderBookClient(private_key)
 
     def set_transaction_mode(self, mode: TransactionMode):
         self.order_book_client.set_transaction_mode(mode)
 
+    async def get_markets(self):
+        return await self.order_book_client.get_markets()
+
     async def get_order_book(self, market: int, callback: AsyncOrderBookDepthCallback):
         order_book_depth = await self.web3_client.eth.get_order_book_depth(market)
         return await callback(order_book_depth)
 
     async def get_margin_and_positions(self, callback: AsyncPositionCallback):
         response = await self.web3_client.eth.get_margin_and_positions(self.trader_address)
         return await callback(response)
 
     async def get_order_status(self, order_id: HexBytes, callback: AsyncOrderStatusCallback):
         response = await self.web3_client.eth.get_order_status(order_id.hex()) # type: ignore
         return await callback(response)
 
-    async def place_orders(self, orders: List[Order], callback: AsyncPlaceOrdersCallback, tx_options = None, mode=None):
+    async def place_orders(self, orders: List[Order], wait_for_response: bool, callback: AsyncPlaceOrdersCallback, tx_options = None, mode=None):
         if len(orders) > 75:
             raise ValueError("Cannot place more than 75 orders at once")
 
         for order in orders:
             if order.amm_index is None:
                 raise ValueError("Order AMM index is not set")
             if order.base_asset_quantity is None:
@@ -62,55 +66,87 @@
 
             # trader and salt can be set automatically
             if order.trader in [None, "0x", ""]:
                 order.trader = self.trader_address
             if order.salt in [None, 0]:
                 order.salt = get_new_salt()
 
-        response = await self.order_book_client.place_orders(orders, tx_options, mode)
-        return await callback(response)
+        for order in orders:
+            order_hash = get_order_hash(order)
+            order.id = order_hash
 
-    async def place_single_order(
-        self, market: int, base_asset_quantity: float, price: float, reduce_only: bool, callback, tx_options = None, mode=None
-    ) -> Order:
-        order = Order(
-            id=None,
-            amm_index=market,
-            trader=self.trader_address,
-            base_asset_quantity=float_to_scaled_int(base_asset_quantity, 18),
-            price=float_to_scaled_int(price, 6),
-            salt=get_new_salt(),
-            reduce_only=reduce_only,
-        )
-        order_hash = await self.order_book_client.place_order(order, tx_options, mode)
-        order.id = order_hash
-        return await callback(order)
+        # if the response if requested then we'll have to wait for the transaction to be mined
+        # This is because the receipt is generated only after the transaction is mined(accepted)
+        if wait_for_response:
+            mode = TransactionMode.wait_for_accept
+
+        tx_hash = await self.order_book_client.place_orders(orders, tx_options, mode)
+        if wait_for_response:
+            receipt = await self.web3_client.eth.get_transaction_receipt(tx_hash)
+
+            events = self.order_book_client.get_events_from_receipt(receipt, "OrderPlaced")
+            response = []
+            for event in events:
+                order_id = event.args.orderHash
+                response.append({
+                    "order_id": order_id,
+                    "success": True
+                })
+            return await callback(response)
+        else:
+            return await callback(orders)
 
-    async def cancel_orders(self, orders: List[Order], callback, tx_options = None, mode=None):
+    async def cancel_orders(self, orders: List[Order], atomic: bool, wait_for_response: bool, callback, tx_options = None, mode=None):
         if len(orders) > 100:
             raise ValueError("Cannot cancel more than 100 orders at once")
 
-        await self.order_book_client.cancel_orders(orders, tx_options, mode)
-        return await callback()
+        if atomic is None:
+            atomic = True  # default mode
 
-    async def cancel_order_by_id(self, order_id: HexBytes, callback, tx_options = None, mode=None):
+        # if the response if requested then we'll have to wait for the transaction to be mined
+        # This is because the receipt is generated only after the transaction is mined(accepted)
+        if wait_for_response:
+            mode = TransactionMode.wait_for_accept
+
+        tx_hash = await self.order_book_client.cancel_orders(orders, atomic, tx_options, mode)
+
+        if wait_for_response:
+            receipt = await self.web3_client.eth.get_transaction_receipt(tx_hash)
+
+            response = []
+            cancelled_events = self.order_book_client.get_events_from_receipt(receipt, "OrderCancelled")
+            for event in cancelled_events:
+                response.append({
+                    "order_id": event.args.orderHash,
+                    "success": True
+                })
+            skipped_events = self.order_book_client.get_events_from_receipt(receipt, "SkippedCancelOrder")
+            for event in skipped_events:
+                response.append({
+                    "order_id": event.args.orderHash,
+                    "success": False,
+                })
+            return await callback(response)
+        else:
+            return await callback(orders)
+
+    async def cancel_order_by_id(self, order_id: HexBytes, wait_for_response: bool, callback, tx_options = None, mode=None):
         async def order_status_callback(response: OrderStatusResponse) -> Order:
             position_side_multiplier = 1 if response.positionSide == "LONG" else -1
             return Order(
                 id=order_id,
                 amm_index=response.symbol,
                 trader=self.trader_address,
                 base_asset_quantity=float_to_scaled_int(float(response.origQty) * position_side_multiplier, 18),
                 price=float_to_scaled_int(float(response.price), 6),
                 salt=int(response.salt),
                 reduce_only=response.reduceOnly,
             )
         order = await self.get_order_status(order_id, order_status_callback)
-        response = await self.cancel_orders([order], callback, tx_options, mode)
-        return await callback(response)
+        return await self.cancel_orders([order], wait_for_response, callback, tx_options, mode)
 
     async def get_order_fills(self, order_id: str) -> List[Dict]:
         return await self.order_book_client.get_order_fills(order_id)
 
     async def subscribe_to_order_book_depth(
         self, market: int, callback: AsyncSubscribeToOrderBookDepthCallback
     ) -> None:
@@ -155,7 +191,29 @@
                 if message_json.get('result'):
                     # ignore because it's a subscription confirmation with subscription id
                     continue
                 response = WebsocketResponse(**message_json)
                 if response.method and response.method == "trading_subscription":
                     response = TraderFeedUpdate(**response.params['result'])
                     await callback(ws, response)
+
+    async def subscribe_to_market_updates(
+        self, market, update_type: ConfirmationMode, callback
+    ) -> None:
+        async with websockets.connect(self.websocket_endpoint) as ws:
+            msg = {
+                "jsonrpc": "2.0",
+                "id": 1,
+                "method": "trading_subscribe",
+                "params": ["streamMarketTrades", market, update_type.value]
+            }
+            await ws.send(json.dumps(msg))
+
+            async for message in ws:
+                message_json = json.loads(message)
+                if message_json.get('result'):
+                    # ignore because it's a subscription confirmation with subscription id
+                    continue
+                response = WebsocketResponse(**message_json)
+                if response.method and response.method == "trading_subscription":
+                    response = MarketFeedUpdate(**response.params['result'])
+                    await callback(ws, response)
```

### Comparing `hubble_exchange-0.4.0/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.5.0/hubble_exchange/contract_abis/OrderBook.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {'insert': "[(7, OrderedDict([('anonymous', False), ('inputs', [OrderedDict([('indexed', True), "*

 * *           "('internalType', 'address'), ('name', 'trader'), ('type', 'address')]), "*

 * *           "OrderedDict([('indexed', True), ('internalType', 'bytes32'), ('name', 'orderHash'), "*

 * *           "('type', 'bytes32')]), OrderedDict([('indexed', False), ('internalType', 'uint256'), "*

 * *           "('name', 'timestamp'), ('type', 'uint256')])]), ('name', 'SkippedCancelOrder'), "*

 * *           "('type', 'event')])), (8, […]*

```diff
@@ -275,14 +275,77 @@
                 "type": "uint256"
             }
         ],
         "name": "OrdersMatched",
         "type": "event"
     },
     {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": true,
+                "internalType": "address",
+                "name": "trader",
+                "type": "address"
+            },
+            {
+                "indexed": true,
+                "internalType": "bytes32",
+                "name": "orderHash",
+                "type": "bytes32"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "SkippedCancelOrder",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": true,
+                "internalType": "address",
+                "name": "trader",
+                "type": "address"
+            },
+            {
+                "indexed": true,
+                "internalType": "address",
+                "name": "authority",
+                "type": "address"
+            }
+        ],
+        "name": "TradingAuthorityRevoked",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": true,
+                "internalType": "address",
+                "name": "trader",
+                "type": "address"
+            },
+            {
+                "indexed": true,
+                "internalType": "address",
+                "name": "authority",
+                "type": "address"
+            }
+        ],
+        "name": "TradingAuthorityWhitelisted",
+        "type": "event"
+    },
+    {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "ammIndex",
                         "type": "uint256"
@@ -367,14 +430,59 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "ammIndex",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "trader",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "int256",
+                        "name": "baseAssetQuantity",
+                        "type": "int256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "price",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "salt",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "bool",
+                        "name": "reduceOnly",
+                        "type": "bool"
+                    }
+                ],
+                "internalType": "struct ILimitOrderBook.Order[]",
+                "name": "orders",
+                "type": "tuple[]"
+            }
+        ],
+        "name": "cancelOrdersNoisy",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "bytes[2]",
                 "name": "orders",
                 "type": "bytes[2]"
             },
             {
                 "internalType": "int256",
                 "name": "fillAmount",
```

### Comparing `hubble_exchange-0.4.0/hubble_exchange/eip712.py` & `hubble_exchange-0.5.0/hubble_exchange/eip712.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.4.0/hubble_exchange/eth.py` & `hubble_exchange-0.5.0/hubble_exchange/eth.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.4.0/hubble_exchange/models.py` & `hubble_exchange-0.5.0/hubble_exchange/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,28 @@
     OrderType: str
     Removed: bool
     EventName: str
     Args: Dict
     BlockNumber: int
     BlockStatus: str
     Timestamp: int
+    TransactionHash: HexBytes
+
+@dataclass
+class MarketFeedUpdate:
+    Trader: Address
+    Market: int
+    Size: float
+    Price: float
+    Removed: bool
+    EventName: str
+    BlockNumber: int
+    BlockStatus: str
+    Timestamp: int
+    TransactionHash: HexBytes
 
 
 class AsyncOrderBookDepthCallback(Protocol):
     def __call__(self, response: OrderBookDepthResponse) -> Coroutine[Any, Any, Any]: ...
 
 
 class AsyncPositionCallback(Protocol):
```

### Comparing `hubble_exchange-0.4.0/hubble_exchange/order_book.py` & `hubble_exchange-0.5.0/hubble_exchange/order_book.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,111 @@
 import json
 import os
-import time
 from enum import Enum
 from typing import Any, Dict, List
 
 from hexbytes import HexBytes
+from web3.logs import DISCARD
 
 from hubble_exchange.constants import (CHAIN_ID, GAS_PER_ORDER, MAX_GAS_LIMIT,
+                                       ClearingHouseContractAddress,
                                        OrderBookContractAddress)
 from hubble_exchange.eip712 import get_order_hash
-from hubble_exchange.eth import HubblenetWeb3 as Web3
 from hubble_exchange.eth import get_async_web3_client, get_sync_web3_client
 from hubble_exchange.models import Order
 from hubble_exchange.utils import (get_address_from_private_key,
                                    int_to_scaled_float)
 
 # read abi from file
 HERE = os.path.dirname(__file__)
 with open(f"{HERE}/contract_abis/OrderBook.json", 'r') as abi_file:
     abi_str = abi_file.read()
-    ABI = json.loads(abi_str)
+    ORDERBOOK_ABI = json.loads(abi_str)
+
+with open(f"{HERE}/contract_abis/ClearingHouse.json", 'r') as abi_file:
+    abi_str = abi_file.read()
+    CLEARINGHOUSE_ABI = json.loads(abi_str)
+
+with open(f"{HERE}/contract_abis/AMM.json", 'r') as abi_file:
+    abi_str = abi_file.read()
+    AMM_ABI = json.loads(abi_str)
 
 
 class TransactionMode(Enum):
     no_wait = 0
     wait_for_head = 1
     wait_for_accept = 2
 
 
 class OrderBookClient(object):
     def __init__(self, private_key: str):
         self._private_key = private_key
         self.public_address = get_address_from_private_key(private_key)
 
         self.web3_client = get_async_web3_client()
-        self.order_book = self.web3_client.eth.contract(address=OrderBookContractAddress, abi=ABI)
+        self.order_book_contract = self.web3_client.eth.contract(address=OrderBookContractAddress, abi=ORDERBOOK_ABI)
 
         # get nonce from sync web3 client
         sync_web3 = get_sync_web3_client()
         self.nonce = sync_web3.eth.get_transaction_count(self.public_address)
 
         self.transaction_mode = TransactionMode.no_wait  # default
 
     def set_transaction_mode(self, mode: TransactionMode):
         self.transaction_mode = mode
 
+    async def get_markets(self):
+        clearing_house_contract = self.web3_client.eth.contract(address=ClearingHouseContractAddress, abi=CLEARINGHOUSE_ABI)
+        amm_addresses = await clearing_house_contract.functions.getAMMs().call()
+
+        markets = {}
+        for i, amm_address in enumerate(amm_addresses):
+            amm_contract = self.web3_client.eth.contract(address=amm_address, abi=AMM_ABI)
+            name = await amm_contract.functions.name().call()
+            markets[i] = name
+
+        return markets
+
     async def place_order(self, order: Order, custom_tx_options=None, mode=None) -> HexBytes:
         order_hash = get_order_hash(order)
 
         tx_options = {'gas': GAS_PER_ORDER}
         tx_options.update(custom_tx_options or {})
 
         await self._send_orderbook_transaction("placeOrder", [order.to_dict()], tx_options, mode)
         return order_hash
 
-    async def place_orders(self, orders: List[Order], custom_tx_options=None, mode=None) -> List[Order]:
+    async def place_orders(self, orders: List[Order], custom_tx_options=None, mode=None):
         """
         Place multiple orders at once. This is more efficient than placing them one by one.
         """
         place_order_payload = []
 
         for order in orders:
             order_hash = get_order_hash(order)
             order.id = order_hash
             place_order_payload.append(order.to_dict())
 
         tx_options = {'gas': min(GAS_PER_ORDER * len(orders), MAX_GAS_LIMIT)}
         tx_options.update(custom_tx_options or {})
-        await self._send_orderbook_transaction("placeOrders", [place_order_payload], tx_options, mode)
-        return orders
+        return await self._send_orderbook_transaction("placeOrders", [place_order_payload], tx_options, mode)
 
-    async def cancel_orders(self, orders: list[Order], custom_tx_options=None, mode=None) -> None:
+    async def cancel_orders(self, orders: list[Order], atomic, custom_tx_options=None, mode=None):
         cancel_order_payload = []
         for order in orders:
             cancel_order_payload.append(order.to_dict())
 
         tx_options = {'gas': min(GAS_PER_ORDER * len(orders), MAX_GAS_LIMIT)}
         tx_options.update(custom_tx_options or {})
 
-        await self._send_orderbook_transaction("cancelOrders", [cancel_order_payload], tx_options, mode)
+        method_name = "cancelOrdersNoisy" if atomic else "cancelOrders"
+        return await self._send_orderbook_transaction(method_name, [cancel_order_payload], tx_options, mode)
 
     async def get_order_fills(self, order_id: str) -> List[Dict]:
-        orders_matched_events = await self.order_book.events.OrderMatched().get_logs(
+        orders_matched_events = await self.order_book_contract.events.OrderMatched().get_logs(
             {"orderHash": order_id},
             fromBlock='earliest',
         )
 
         fills = []
         for event in orders_matched_events:
             fills.append({
@@ -93,32 +113,34 @@
                 "transaction_hash": event.transactionHash,
                 "timestamp": event.args.timestamp,
                 "fill_amount": int_to_scaled_float(event.args.fillAmount, 18),
                 "price": int_to_scaled_float(event.args.price, 6),
             })
         return fills
 
+    def get_events_from_receipt(self, receipt, event_name):
+        event = getattr(self.order_book_contract.events, event_name)
+        return event().process_receipt(receipt, DISCARD)
+
     async def _get_nonce(self) -> int:
         if self.nonce is None:
             self.nonce = await self.web3_client.eth.get_transaction_count(self.public_address)
         else:
             self.nonce += 1
         return self.nonce - 1
 
     async def _send_orderbook_transaction(self, method_name: str, args: List[Any], tx_options: Dict, mode: TransactionMode) -> HexBytes:
         if mode is None:
             mode = self.transaction_mode
 
-        method = getattr(self.order_book.functions, method_name)
+        method = getattr(self.order_book_contract.functions, method_name)
         nonce = await self._get_nonce()
         tx_params = {
             'from': self.public_address,
             'chainId': CHAIN_ID,
-            'maxFeePerGas': Web3.to_wei(60, 'gwei'),  # base + tip
-            'maxPriorityFeePerGas': 0,  # tip
             'nonce': nonce,
         }
         if tx_options:
             tx_params.update(tx_options)
 
         transaction = await method(*args).build_transaction(tx_params)
         signed_tx = self.web3_client.eth.account.sign_transaction(transaction, self._private_key)
```

### Comparing `hubble_exchange-0.4.0/hubble_exchange/utils.py` & `hubble_exchange-0.5.0/hubble_exchange/utils.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.4.0/hubble_exchange.egg-info/SOURCES.txt` & `hubble_exchange-0.5.0/hubble_exchange.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -13,8 +13,10 @@
 hubble_exchange/order_book.py
 hubble_exchange/utils.py
 hubble_exchange.egg-info/PKG-INFO
 hubble_exchange.egg-info/SOURCES.txt
 hubble_exchange.egg-info/dependency_links.txt
 hubble_exchange.egg-info/requires.txt
 hubble_exchange.egg-info/top_level.txt
+hubble_exchange/contract_abis/AMM.json
+hubble_exchange/contract_abis/ClearingHouse.json
 hubble_exchange/contract_abis/OrderBook.json
```

### Comparing `hubble_exchange-0.4.0/pyproject.toml` & `hubble_exchange-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.4.0"
+version = "0.5.0"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
```

