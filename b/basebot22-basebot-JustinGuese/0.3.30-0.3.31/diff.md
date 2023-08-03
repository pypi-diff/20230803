# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.30.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.30.tar", last modified: Thu Aug  3 15:58:50 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.31.tar", last modified: Thu Aug  3 16:02:36 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.30.tar` & `basebot22-basebot_JustinGuese-0.3.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 15:58:41.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 15:58:50.000000 basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 15:58:43.000000 basebot22-basebot_JustinGuese-0.3.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:58:50.922249 basebot22-basebot_JustinGuese-0.3.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:02:36.470575 basebot22-basebot_JustinGuese-0.3.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:02:36.470575 basebot22-basebot_JustinGuese-0.3.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:02:26.000000 basebot22-basebot_JustinGuese-0.3.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:02:36.466575 basebot22-basebot_JustinGuese-0.3.31/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:02:26.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:02:26.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-08-03 16:02:26.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:02:26.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:02:36.470575 basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:02:36.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:02:36.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:02:36.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:02:36.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:02:36.000000 basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:02:28.000000 basebot22-basebot_JustinGuese-0.3.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:02:36.470575 basebot22-basebot_JustinGuese-0.3.31/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.30/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.30
+Version: 0.3.31
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.30/README.md` & `basebot22-basebot_JustinGuese-0.3.31/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.30/basebot22/backtest.py` & `basebot22-basebot_JustinGuese-0.3.31/basebot22/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,26 @@
     MAX = "max"
 
 class Order(BaseModel):
     buy: bool
     stockname: str
     amountInUSD: float = -1 # 1 means all
 
+def getValueOfPortfolio(crntRow, portfolio, boughtAt):
+    worth = 0
+    for ticker, amount in portfolio.items():
+        if ticker == "USD":
+            worth += amount
+            continue
+        if amount > 0:
+            worth += amount * crntRow[ticker]["Close"]
+        elif amount < 0:
+            worth += amount * (boughtAt[ticker] - crntRow[ticker]["Close"]) + amount * boughtAt[ticker]
+    return worth
+
 class Backtest:
     def __init__(self, stocknames: List[str], decisionFunction, startMoney: int = 10000, interval: Interval = Interval.ONE_DAY, period: Period = Period.THREE_YEARS):
         assert len(stocknames) > 0, "Stocknames must be a list of stock names"
         self.data = {}
         for stockname in stocknames:
             self.data[stockname] = yf.download(stockname, period=period.value, interval=interval.value, progress=False)
             assert len(self.data) > 0, "No data found, please check your stock name"
@@ -62,26 +74,17 @@
         self.datas = {} # datas will be used to get the current data
         self.portfolio = {"USD" : startMoney}
         self.commission = 0.005 # 0.5% commission
         self.fees = 0.
         self.boughtAt = {}
 
     def getValueOfPortfolio(self, crntRow):
-        worth = 0
-        for ticker, amount in self.portfolio.items():
-            if ticker == "USD":
-                worth += amount
-                continue
-            if amount > 0:
-                worth += amount * crntRow[ticker]["Close"]
-            elif amount < 0:
-                worth += amount * (self.boughtAt[ticker] - crntRow[ticker]["Close"]) + amount * self.boughtAt[ticker]
-        return worth
+        return getValueOfPortfolio(crntRow, self.portfolio, self.boughtAt)
     
-    def oneRun(self):
+    def oneRun(self) -> List[float]:
         portfolio = []
         for date in self.data[list(self.data.keys())[0]].index:
             crntRow = {}
             for stockname in self.data.keys():
                 self.datas[stockname] = self.data[stockname].loc[:date]
                 crntRow[stockname] = self.data[stockname].loc[date]
             datasSub = self.datas
```

### Comparing `basebot22-basebot_JustinGuese-0.3.30/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.31/basebot22/basebot.py`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.30/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.31/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.30
+Version: 0.3.31
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.30/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.30"
+version = "0.3.31"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

