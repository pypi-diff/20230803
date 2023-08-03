# Comparing `tmp/hubble_exchange-0.5.0.tar.gz` & `tmp/hubble_exchange-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.5.0.tar", last modified: Thu Aug  3 07:50:07 2023, max compression
+gzip compressed data, was "hubble_exchange-0.5.1.tar", last modified: Thu Aug  3 07:59:33 2023, max compression
```

## Comparing `hubble_exchange-0.5.0.tar` & `hubble_exchange-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.958679 hubble_exchange-0.5.0/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.5.0/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.5.0/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)     8140 2023-08-03 07:50:07.958531 hubble_exchange-0.5.0/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     6483 2023-08-03 07:06:01.000000 hubble_exchange-0.5.0/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.955711 hubble_exchange-0.5.0/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      369 2023-07-25 06:59:23.000000 hubble_exchange-0.5.0/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)    10087 2023-08-03 07:48:30.000000 hubble_exchange-0.5.0/hubble_exchange/client.py
--rw-r--r--   0 shubham    (501) staff       (20)      288 2023-08-03 07:09:05.000000 hubble_exchange-0.5.0/hubble_exchange/constants.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.958101 hubble_exchange-0.5.0/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    17033 2023-08-02 10:06:29.000000 hubble_exchange-0.5.0/hubble_exchange/contract_abis/AMM.json
--rw-r--r--   0 shubham    (501) staff       (20)    23347 2023-08-02 10:07:52.000000 hubble_exchange-0.5.0/hubble_exchange/contract_abis/ClearingHouse.json
--rw-r--r--   0 shubham    (501) staff       (20)    17505 2023-08-02 10:26:02.000000 hubble_exchange-0.5.0/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.5.0/hubble_exchange/eip712.py
--rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.5.0/hubble_exchange/errors.py
--rw-r--r--   0 shubham    (501) staff       (20)     5612 2023-08-03 07:46:15.000000 hubble_exchange-0.5.0/hubble_exchange/eth.py
--rw-r--r--   0 shubham    (501) staff       (20)     3730 2023-08-02 07:54:20.000000 hubble_exchange-0.5.0/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)     6175 2023-08-03 07:47:45.000000 hubble_exchange-0.5.0/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)      562 2023-07-22 11:56:49.000000 hubble_exchange-0.5.0/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:50:07.956586 hubble_exchange-0.5.0/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     8140 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      619 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       88 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2023-08-03 07:50:07.000000 hubble_exchange-0.5.0/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-08-03 07:49:51.000000 hubble_exchange-0.5.0/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-08-03 07:50:07.958718 hubble_exchange-0.5.0/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.5.0/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:59:33.044106 hubble_exchange-0.5.1/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.5.1/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.5.1/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)     8148 2023-08-03 07:59:33.043943 hubble_exchange-0.5.1/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     6491 2023-08-03 07:57:43.000000 hubble_exchange-0.5.1/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:59:33.041272 hubble_exchange-0.5.1/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      369 2023-07-25 06:59:23.000000 hubble_exchange-0.5.1/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)    10087 2023-08-03 07:48:30.000000 hubble_exchange-0.5.1/hubble_exchange/client.py
+-rw-r--r--   0 shubham    (501) staff       (20)      288 2023-08-03 07:56:24.000000 hubble_exchange-0.5.1/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:59:33.043527 hubble_exchange-0.5.1/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    17033 2023-08-02 10:06:29.000000 hubble_exchange-0.5.1/hubble_exchange/contract_abis/AMM.json
+-rw-r--r--   0 shubham    (501) staff       (20)    23347 2023-08-02 10:07:52.000000 hubble_exchange-0.5.1/hubble_exchange/contract_abis/ClearingHouse.json
+-rw-r--r--   0 shubham    (501) staff       (20)    17505 2023-08-02 10:26:02.000000 hubble_exchange-0.5.1/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.5.1/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.5.1/hubble_exchange/errors.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5612 2023-08-03 07:46:15.000000 hubble_exchange-0.5.1/hubble_exchange/eth.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3730 2023-08-02 07:54:20.000000 hubble_exchange-0.5.1/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)     6175 2023-08-03 07:47:45.000000 hubble_exchange-0.5.1/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)      562 2023-07-22 11:56:49.000000 hubble_exchange-0.5.1/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-08-03 07:59:33.042033 hubble_exchange-0.5.1/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     8148 2023-08-03 07:59:33.000000 hubble_exchange-0.5.1/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      619 2023-08-03 07:59:33.000000 hubble_exchange-0.5.1/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-08-03 07:59:33.000000 hubble_exchange-0.5.1/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       88 2023-08-03 07:59:33.000000 hubble_exchange-0.5.1/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2023-08-03 07:59:33.000000 hubble_exchange-0.5.1/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-08-03 07:59:26.000000 hubble_exchange-0.5.1/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-08-03 07:59:33.044157 hubble_exchange-0.5.1/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.5.1/setup.py
```

### Comparing `hubble_exchange-0.5.0/LICENSE` & `hubble_exchange-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/PKG-INFO` & `hubble_exchange-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.5.0
+Version: 0.5.1
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -176,16 +176,16 @@
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
 
 ## Waiting for response in place_orders and cancel_orders
 
 The `place_orders` and `cancel_orders` methods can be called in 2 modes - wait for response or don't wait for response.
-To get the acknowledgement of the transaction, use wait_for_response=True. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
-When using wait_for_response=True, the sdk will automatically set the transaction mode to TransactionMode.wait_for_accept because the response can be confirmed only after the transaction is mined.
+To get the acknowledgement of the transaction, use `wait_for_response=True`. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
+When using `wait_for_response=True`, the sdk will automatically set the transaction mode to `TransactionMode.wait_for_accept` because the response can be confirmed only after the transaction is mined.
 
 Alternatively, the client can also use trader feed to listen to all the updates. This is faster when done with ConfirmationMode.head
 
 ## Atomic in cancel_orders
 
 The `cancel_orders` method can be called in 2 modes - atomic or non-atomic. In atomic mode, all the orders will be cancelled only if all the orders are successfully cancelled. In non-atomic mode, the orders will be cancelled one by one and the response will be a list of dicts with order ids and success boolean.
-When used in combination with wait_for_response=True, the response will be a list of dicts with order ids and success boolean.
+When used in combination with `wait_for_response=True`, the response will be a list of dicts with order ids and success boolean.
```

### Comparing `hubble_exchange-0.5.0/README.md` & `hubble_exchange-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -143,16 +143,16 @@
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
 
 ## Waiting for response in place_orders and cancel_orders
 
 The `place_orders` and `cancel_orders` methods can be called in 2 modes - wait for response or don't wait for response.
-To get the acknowledgement of the transaction, use wait_for_response=True. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
-When using wait_for_response=True, the sdk will automatically set the transaction mode to TransactionMode.wait_for_accept because the response can be confirmed only after the transaction is mined.
+To get the acknowledgement of the transaction, use `wait_for_response=True`. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
+When using `wait_for_response=True`, the sdk will automatically set the transaction mode to `TransactionMode.wait_for_accept` because the response can be confirmed only after the transaction is mined.
 
 Alternatively, the client can also use trader feed to listen to all the updates. This is faster when done with ConfirmationMode.head
 
 ## Atomic in cancel_orders
 
 The `cancel_orders` method can be called in 2 modes - atomic or non-atomic. In atomic mode, all the orders will be cancelled only if all the orders are successfully cancelled. In non-atomic mode, the orders will be cancelled one by one and the response will be a list of dicts with order ids and success boolean.
-When used in combination with wait_for_response=True, the response will be a list of dicts with order ids and success boolean.
+When used in combination with `wait_for_response=True`, the response will be a list of dicts with order ids and success boolean.
```

### Comparing `hubble_exchange-0.5.0/hubble_exchange/client.py` & `hubble_exchange-0.5.1/hubble_exchange/client.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/contract_abis/AMM.json` & `hubble_exchange-0.5.1/hubble_exchange/contract_abis/AMM.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/contract_abis/ClearingHouse.json` & `hubble_exchange-0.5.1/hubble_exchange/contract_abis/ClearingHouse.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.5.1/hubble_exchange/contract_abis/OrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/eip712.py` & `hubble_exchange-0.5.1/hubble_exchange/eip712.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/eth.py` & `hubble_exchange-0.5.1/hubble_exchange/eth.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/models.py` & `hubble_exchange-0.5.1/hubble_exchange/models.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/order_book.py` & `hubble_exchange-0.5.1/hubble_exchange/order_book.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange/utils.py` & `hubble_exchange-0.5.1/hubble_exchange/utils.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/hubble_exchange.egg-info/PKG-INFO` & `hubble_exchange-0.5.1/hubble_exchange.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble-exchange
-Version: 0.5.0
+Version: 0.5.1
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -176,16 +176,16 @@
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
 
 ## Waiting for response in place_orders and cancel_orders
 
 The `place_orders` and `cancel_orders` methods can be called in 2 modes - wait for response or don't wait for response.
-To get the acknowledgement of the transaction, use wait_for_response=True. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
-When using wait_for_response=True, the sdk will automatically set the transaction mode to TransactionMode.wait_for_accept because the response can be confirmed only after the transaction is mined.
+To get the acknowledgement of the transaction, use `wait_for_response=True`. The response will be a list of dicts with order ids and success boolean. Waiting for response will be slower because this can be confirmed only after the transaction is mined(accepted).
+When using `wait_for_response=True`, the sdk will automatically set the transaction mode to `TransactionMode.wait_for_accept` because the response can be confirmed only after the transaction is mined.
 
 Alternatively, the client can also use trader feed to listen to all the updates. This is faster when done with ConfirmationMode.head
 
 ## Atomic in cancel_orders
 
 The `cancel_orders` method can be called in 2 modes - atomic or non-atomic. In atomic mode, all the orders will be cancelled only if all the orders are successfully cancelled. In non-atomic mode, the orders will be cancelled one by one and the response will be a list of dicts with order ids and success boolean.
-When used in combination with wait_for_response=True, the response will be a list of dicts with order ids and success boolean.
+When used in combination with `wait_for_response=True`, the response will be a list of dicts with order ids and success boolean.
```

### Comparing `hubble_exchange-0.5.0/hubble_exchange.egg-info/SOURCES.txt` & `hubble_exchange-0.5.1/hubble_exchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.5.0/pyproject.toml` & `hubble_exchange-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.5.0"
+version = "0.5.1"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
```

