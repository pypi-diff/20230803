# Comparing `tmp/volstreet-1.0.8.tar.gz` & `tmp/volstreet-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.8.tar", last modified: Tue Jul 25 18:08:46 2023, max compression
+gzip compressed data, was "volstreet-1.0.9.tar", last modified: Wed Jul 26 20:59:19 2023, max compression
```

## Comparing `volstreet-1.0.8.tar` & `volstreet-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:08:46.106504 volstreet-1.0.8/
--rw-rw-rw-   0        0        0      497 2023-07-25 18:08:46.107499 volstreet-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.8/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-25 18:08:46.107499 volstreet-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 18:08:46.102415 volstreet-1.0.8/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.8/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.8/volstreet/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.8/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.8/volstreet/constants.py
--rw-rw-rw-   0        0        0    43796 2023-07-25 18:04:18.000000 volstreet-1.0.8/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   192160 2023-07-25 17:19:23.000000 volstreet-1.0.8/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.8/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.8/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.8/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13488 2023-07-25 17:19:23.000000 volstreet-1.0.8/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:08:46.106504 volstreet-1.0.8/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 20:59:19.381528 volstreet-1.0.9/
+-rw-rw-rw-   0        0        0      497 2023-07-26 20:59:19.382520 volstreet-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.9/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-26 20:59:19.382520 volstreet-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 20:59:19.376541 volstreet-1.0.9/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.9/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.9/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.9/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.9/volstreet/constants.py
+-rw-rw-rw-   0        0        0    43796 2023-07-25 18:04:18.000000 volstreet-1.0.9/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   192627 2023-07-26 20:57:45.000000 volstreet-1.0.9/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.9/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.9/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.9/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13488 2023-07-25 17:19:23.000000 volstreet-1.0.9/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:59:19.381528 volstreet-1.0.9/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.8/setup.cfg` & `volstreet-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a61  rsion = 1.0.8..a
+00000020: 7273 696f 6e20 3d20 312e 302e 390d 0a61  rsion = 1.0.9..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.8/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.9/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet/blackscholes.py` & `volstreet-1.0.9/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet/constants.py` & `volstreet-1.0.9/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet/datamodule.py` & `volstreet-1.0.9/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet/dealingroom.py` & `volstreet-1.0.9/volstreet/dealingroom.py`

 * *Files 1% similar despite different names*

```diff
@@ -903,32 +903,31 @@
         self.symbol, self.token = fetch_symbol_token(self.name)
         self.lot_size = fetch_lot_size(self.name)
         self.fetch_expirys(self.symbol)
         self.freeze_qty = self.fetch_freeze_limit()
         self.available_strikes = None
         self.available_straddle_strikes = None
         self.intraday_straddle_forced_exit = False
+        self.base = get_base(self.name)
 
         if self.name == "BANKNIFTY":
-            self.base = 100
             self.exchange_type = 1
         elif self.name == "NIFTY":
-            self.base = 50
             self.exchange_type = 1
         elif self.name in [
             "FINNIFTY",
             "MIDCPNIFTY",
         ]:  # Finnifty and Midcpnifty temp fix
-            self.base = 50
             self.exchange_type = 2
         else:
-            self.base = get_base(self.name)
             self.exchange_type = 1
-            logger.info(f"Base for {self.name} is {self.base}")
-            # print(f"Base for {self.name} is {self.base}")
+
+        logger.info(
+            f"Initialized {self.name} with lot size {self.lot_size}, base {self.base} and freeze qty {self.freeze_qty}"
+        )
 
         if websocket:
             try:
                 websocket.subscribe(
                     websocket.correlation_id,
                     1,
                     [{"exchangeType": self.exchange_type, "tokens": [self.token]}],
@@ -2658,15 +2657,15 @@
                 )
                 hedge_total_ltp = h_strangle.fetch_total_ltp()
 
                 hedge_profit = (
                     info_dict["total_avg_price"] - hedge_total_ltp - self.base
                 )
 
-                logging.info(
+                logger.info(
                     f"{self.name} CTB threshold: {profit_threshold}, Hedge working: {hedge_profit}"
                 )
 
                 if hedge_profit >= profit_threshold:
                     return h_strangle
                 else:
                     return None
@@ -2748,15 +2747,15 @@
                             info_dict["exit_triggers"].update(
                                 {"convert_to_butterfly": True}
                             )
                             ctb_message = f"Hedged with: {ctb_hedge}\n"
                             info_dict["ctb_hedge"] = ctb_hedge
                             ctb_notification_sent = True
                     except Exception as _e:
-                        logging.info(f"Error in process_ctb: {_e}")
+                        logger.error(f"Error in process_ctb: {_e}")
 
                 message = (
                     f"\nUnderlying: {self.name}\n"
                     f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
                     f"Underlying LTP: {spot_price}\n"
                     f"Call Strike: {traded_strangle.call_strike}\n"
                     f"Put Strike: {traded_strangle.put_strike}\n"
@@ -3268,31 +3267,27 @@
                 "BUY",
                 quantity_in_lots,
                 "LIMIT",
                 order_tag,
                 self.webhook_url,
                 return_avg_price=False,
             )
-            if (
-                shared_info_dict["call_stop_loss_order_ids"]
-                and shared_info_dict["put_stop_loss_order_ids"]
-            ):
+            if place_sl_orders:
                 cancel_pending_orders(
                     shared_info_dict["call_stop_loss_order_ids"]
                     + shared_info_dict["put_stop_loss_order_ids"]
                 )
             notifier(f"{self.name}: Converted to butterfly", self.webhook_url)
             while currenttime().time() < time(*exit_time):
                 sleep(3)
 
         call_sl = shared_info_dict["call_sl"]
         put_sl = shared_info_dict["put_sl"]
 
-        if not call_sl and not put_sl:
-            # Both stop losses not hit
+        if not call_sl and not put_sl:  # Both stop losses not hit
             if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
                 call_exit_avg_price, put_exit_avg_price = (
                     shared_info_dict["call_ltp"],
                     shared_info_dict["put_ltp"],
                 )
             else:
                 call_exit_avg_price, put_exit_avg_price = place_option_order_and_notify(
@@ -3300,14 +3295,20 @@
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
                     self.webhook_url,
                     return_avg_price=True,
                 )
+            # noinspection PyTypeChecker
+            if place_sl_orders and not shared_info_dict["exit_triggers"]["convert_to_butterfly"]:
+                cancel_pending_orders(
+                    shared_info_dict["call_stop_loss_order_ids"]
+                    + shared_info_dict["put_stop_loss_order_ids"]
+                )
             shared_info_dict["call_exit_price"] = call_exit_avg_price
             shared_info_dict["put_exit_price"] = put_exit_avg_price
 
         elif (call_sl or put_sl) and not (call_sl and put_sl):  # Only one stop loss hit
             exit_option_type: str = "put" if call_sl else "call"
             if shared_info_dict["time_left_day_start"] * 365 < 1:  # expiry day
                 non_sl_exit_price = shared_info_dict[f"{exit_option_type}_ltp"]
@@ -3317,14 +3318,16 @@
                     exit_option,
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
                     self.webhook_url,
                 )
+            if place_sl_orders:
+                cancel_pending_orders(shared_info_dict[f"{exit_option_type}_stop_loss_order_ids"])
             shared_info_dict[f"{exit_option_type}_exit_price"] = non_sl_exit_price
 
         else:  # Both stop losses hit
             pass
 
         # Calculate profit
         total_exit_price = (
@@ -4247,14 +4250,17 @@
     strike_array = scrips.loc[
         (scrips.name == name) & (scrips.exch_seg == "NFO")
     ].sort_values("expiry_dt")
     closest_expiry = strike_array.expiry_dt.iloc[0]
     strike_array = (
         strike_array.loc[strike_array.expiry_dt == closest_expiry]["strike"] / 100
     )
+    upper_bound = np.percentile(strike_array, 90)
+    lower_bound = np.percentile(strike_array, 30)
+    strike_array = strike_array[strike_array.between(lower_bound, upper_bound, inclusive='both')]
     strike_differences = np.diff(strike_array.sort_values().unique())
     values, counts = np.unique(strike_differences, return_counts=True)
     mode = values[np.argmax(counts)]
     return mode
 
 
 def fetch_symbol_token(
```

### Comparing `volstreet-1.0.8/volstreet/discord_bot.py` & `volstreet-1.0.9/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet/nsefunctions.py` & `volstreet-1.0.9/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet/strategies.py` & `volstreet-1.0.9/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.8/volstreet.egg-info/requires.txt` & `volstreet-1.0.9/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

