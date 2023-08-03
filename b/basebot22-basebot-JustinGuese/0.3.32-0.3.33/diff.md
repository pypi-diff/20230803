# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.32.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.32.tar", last modified: Thu Aug  3 16:08:00 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.33.tar", last modified: Thu Aug  3 16:08:46 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.32.tar` & `basebot22-basebot_JustinGuese-0.3.33.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:00.698613 basebot22-basebot_JustinGuese-0.3.32/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:08:00.698613 basebot22-basebot_JustinGuese-0.3.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:07:49.000000 basebot22-basebot_JustinGuese-0.3.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:00.698613 basebot22-basebot_JustinGuese-0.3.32/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:07:49.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:07:49.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-03 16:07:49.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:07:49.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:00.698613 basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:08:00.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:08:00.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:08:00.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:08:00.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:08:00.000000 basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:07:51.000000 basebot22-basebot_JustinGuese-0.3.32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:08:00.698613 basebot22-basebot_JustinGuese-0.3.32/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:46.013149 basebot22-basebot_JustinGuese-0.3.33/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:08:37.000000 basebot22-basebot_JustinGuese-0.3.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.32/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.32
+Version: 0.3.33
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.32/README.md` & `basebot22-basebot_JustinGuese-0.3.33/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.32/basebot22/backtest.py` & `basebot22-basebot_JustinGuese-0.3.33/basebot22/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 crntRow[stockname] = self.data[stockname].loc[date]
             datasSub = self.datas
             crntRowSub = crntRow
             if len(crntRow) == 1:
                 # simple mode
                 crntRowSub = crntRow[list(crntRow.keys())[0]]
                 datasSub = self.datas[list(self.datas.keys())[0]]
-            decisions: List[Order] = self.decisionFunction(crntRowSub, datasSub, self.portfolio)
+            decisions: List[Order] = self.decisionFunction(crntRowSub, datasSub, self.portfolio, self.portfolioWorth)
             assert isinstance(decisions, list), "Decision function must return a list of orders or empty list"
             
             for order in decisions:
                 assert isinstance(order, Order), "Decision function must return a list of orders or empty list"
                 if order.buy:
                     if order.amountInUSD == -1:
                         # all we have
@@ -139,15 +139,15 @@
                         raise ValueError("this combination should not be allowed!!!")
                 self.portfolioWorth = self.getValueOfPortfolio(crntRow)
                 portfolio.append(self.portfolioWorth)
         return portfolio
 
 
 if __name__ == "__main__":
-    def callback(row, all_data, portfolio):
+    def callback(row, all_data, portfolio, portfolioWorth):
         if row["SMA50"] > row["SMA200"] and portfolio.get("AAPL", 0) == 0:
             return [Order(buy = True, stockname="AAPL")] # if sma cross buy all
         elif row["SMA50"] < row["SMA200"] and portfolio.get("AAPL", 0) > 0:
             return [Order(buy = False, stockname="AAPL")] # sell all if sma cross down
         return []
 
     bt = Backtest(["AAPL"], callback)
```

### Comparing `basebot22-basebot_JustinGuese-0.3.32/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.33/basebot22/basebot.py`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.32/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.32
+Version: 0.3.33
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.32/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.32"
+version = "0.3.33"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

