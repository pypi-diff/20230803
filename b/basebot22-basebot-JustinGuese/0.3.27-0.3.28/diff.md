# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.27.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.27.tar", last modified: Tue Jul 25 14:53:07 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.28.tar", last modified: Thu Aug  3 07:59:21 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.27.tar` & `basebot22-basebot_JustinGuese-0.3.28.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:53:07.731315 basebot22-basebot_JustinGuese-0.3.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-25 14:53:07.731315 basebot22-basebot_JustinGuese-0.3.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-25 14:52:52.000000 basebot22-basebot_JustinGuese-0.3.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:53:07.731315 basebot22-basebot_JustinGuese-0.3.27/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:52:52.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:52:52.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-07-25 14:52:52.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:53:07.731315 basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-25 14:53:07.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 14:53:07.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:53:07.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 14:53:07.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 14:53:07.000000 basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-25 14:52:58.000000 basebot22-basebot_JustinGuese-0.3.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:53:07.731315 basebot22-basebot_JustinGuese-0.3.27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:59:21.741337 basebot22-basebot_JustinGuese-0.3.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 07:59:21.741337 basebot22-basebot_JustinGuese-0.3.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 07:59:12.000000 basebot22-basebot_JustinGuese-0.3.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:59:21.741337 basebot22-basebot_JustinGuese-0.3.28/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:59:12.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:59:12.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 07:59:12.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:59:21.741337 basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 07:59:21.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-03 07:59:21.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:59:21.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 07:59:21.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 07:59:21.000000 basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 07:59:14.000000 basebot22-basebot_JustinGuese-0.3.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:59:21.741337 basebot22-basebot_JustinGuese-0.3.28/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.27/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.27
+Version: 0.3.28
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.27/README.md` & `basebot22-basebot_JustinGuese-0.3.28/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.27/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.28/basebot22/basebot.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,18 @@
             response = self.session.put(self.backendurl + "/bot", json=json_data, headers=self.headers)
         return name
 
     def getPortfolio(self) -> dict:
         response = self.session.get(self.backendurl + '/bot/' + quote_plus(self.name), headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting portfolio: ", response.text)
-        return response.json()["portfolio"]
+        portfolio = response.json()["portfolio"]
+        # only keep portfolio values that are not 0
+        portfolio = {k: v for k, v in portfolio.items() if v != 0}
+        return portfolio
 
     def getPortfolioWorth(self) -> float:
         response = self.session.get(self.backendurl + '/bot/%s/portfolioworth' % quote_plus(self.name), headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting portfolio worth: ", response.text)
         return float(response.text)
```

### Comparing `basebot22-basebot_JustinGuese-0.3.27/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.28/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.27
+Version: 0.3.28
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.27/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.28/pyproject.toml`

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
-version = "0.3.27"
+version = "0.3.28"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

