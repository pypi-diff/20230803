# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.33.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.33.tar", last modified: Thu Aug  3 16:08:46 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.34.tar", last modified: Thu Aug  3 16:19:36 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.33.tar` & `basebot22-basebot_JustinGuese-0.3.34.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:46.013149 basebot22-basebot_JustinGuese-0.3.33/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:08:35.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:08:46.000000 basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:08:37.000000 basebot22-basebot_JustinGuese-0.3.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:08:46.017149 basebot22-basebot_JustinGuese-0.3.33/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:19:28.000000 basebot22-basebot_JustinGuese-0.3.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.33/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.33
+Version: 0.3.34
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.33/README.md` & `basebot22-basebot_JustinGuese-0.3.34/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.33/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.34/basebot22/basebot.py`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.33/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.33
+Version: 0.3.34
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.33/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.33"
+version = "0.3.34"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

