# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.29.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.29.tar", last modified: Thu Aug  3 15:46:04 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.30.tar", last modified: Thu Aug  3 15:58:50 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.29.tar` & `basebot22-basebot_JustinGuese-0.3.30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:46:04.096346 basebot22-basebot_JustinGuese-0.3.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 15:46:04.096346 basebot22-basebot_JustinGuese-0.3.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 15:45:54.000000 basebot22-basebot_JustinGuese-0.3.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:46:04.096346 basebot22-basebot_JustinGuese-0.3.29/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:54.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:54.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-08-03 15:45:54.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 15:45:54.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:46:04.096346 basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 15:46:04.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 15:46:04.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:46:04.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 15:46:04.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 15:46:04.000000 basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 15:45:56.000000 basebot22-basebot_JustinGuese-0.3.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:46:04.096346 basebot22-basebot_JustinGuese-0.3.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 15:58:43.000000 basebot22-basebot_JustinGuese-0.3.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.29/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.29
+Version: 0.3.30
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.29/README.md` & `basebot22-basebot_JustinGuese-0.3.30/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.29/basebot22/backtest.py` & `basebot22-basebot_JustinGuese-0.3.30/basebot22/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,24 @@
         self.startMoney = startMoney
         self.datas = {} # datas will be used to get the current data
         self.portfolio = {"USD" : startMoney}
         self.commission = 0.005 # 0.5% commission
         self.fees = 0.
         self.boughtAt = {}
 
-    def getValueOfPortfolio(self, crntRow, boughtAt):
+    def getValueOfPortfolio(self, crntRow):
         worth = 0
         for ticker, amount in self.portfolio.items():
             if ticker == "USD":
                 worth += amount
                 continue
             if amount > 0:
                 worth += amount * crntRow[ticker]["Close"]
             elif amount < 0:
-                worth += amount * (boughtAt[ticker] - crntRow[ticker]["Close"]) + amount * boughtAt[ticker]
+                worth += amount * (self.boughtAt[ticker] - crntRow[ticker]["Close"]) + amount * self.boughtAt[ticker]
         return worth
     
     def oneRun(self):
         portfolio = []
         for date in self.data[list(self.data.keys())[0]].index:
             crntRow = {}
             for stockname in self.data.keys():
@@ -132,21 +132,20 @@
                         # all we have
                         amount = -self.portfolio.get(order.stockname)
                         win = (self.boughtAt[order.stockname] - crntRow[order.stockname]["Close"]) * amount + amount * self.boughtAt[order.stockname] * (1-self.commission)
                         self.portfolio["USD"] += win
                         self.portfolio[order.stockname] = 0
                     else:
                         raise ValueError("this combination should not be allowed!!!")
-                portfolio.append(self.getValueOfPortfolio(crntRow, self.boughtAt))
+                portfolio.append(self.getValueOfPortfolio(crntRow))
         return portfolio
 
 
 if __name__ == "__main__":
     def callback(row, all_data, portfolio):
-        medVolume = all_data["Volume"].median()
         if row["SMA50"] > row["SMA200"] and portfolio.get("AAPL", 0) == 0:
             return [Order(buy = True, stockname="AAPL")] # if sma cross buy all
         elif row["SMA50"] < row["SMA200"] and portfolio.get("AAPL", 0) > 0:
             return [Order(buy = False, stockname="AAPL")] # sell all if sma cross down
         return []
 
     bt = Backtest(["AAPL"], callback)
```

### Comparing `basebot22-basebot_JustinGuese-0.3.29/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.30/basebot22/basebot.py`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.29/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.29
+Version: 0.3.30
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.29/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.30/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.29"
+version = "0.3.30"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

