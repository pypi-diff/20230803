# Comparing `tmp/nonebot-plugin-uvdiviner-2.1.0.tar.gz` & `tmp/nonebot-plugin-uvdiviner-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-uvdiviner-2.1.0.tar", last modified: Thu Aug  3 10:18:28 2023, max compression
+gzip compressed data, was "nonebot-plugin-uvdiviner-2.1.1.tar", last modified: Thu Aug  3 10:59:10 2023, max compression
```

## Comparing `nonebot-plugin-uvdiviner-2.1.0.tar` & `nonebot-plugin-uvdiviner-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 10:18:28.255884 nonebot-plugin-uvdiviner-2.1.0/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 nonebot-plugin-uvdiviner-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1295 2023-08-03 10:18:28.254886 nonebot-plugin-uvdiviner-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-08-03 10:17:59.000000 nonebot-plugin-uvdiviner-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 10:18:28.218370 nonebot-plugin-uvdiviner-2.1.0/nonebot-plugin-uvdiviner/
--rw-rw-rw-   0        0        0     3411 2023-08-03 10:09:31.000000 nonebot-plugin-uvdiviner-2.1.0/nonebot-plugin-uvdiviner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:18:28.253886 nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1295 2023-08-03 10:18:28.000000 nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-08-03 10:18:28.000000 nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 10:18:28.000000 nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 10:18:28.000000 nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-03 10:18:28.000000 nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 10:18:28.255884 nonebot-plugin-uvdiviner-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-08-03 10:12:41.000000 nonebot-plugin-uvdiviner-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:59:10.457419 nonebot-plugin-uvdiviner-2.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 nonebot-plugin-uvdiviner-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1295 2023-08-03 10:59:10.457419 nonebot-plugin-uvdiviner-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-08-03 10:17:59.000000 nonebot-plugin-uvdiviner-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 10:59:10.431417 nonebot-plugin-uvdiviner-2.1.1/nonebot-plugin-uvdiviner/
+-rw-rw-rw-   0        0        0     3411 2023-08-03 10:58:29.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot-plugin-uvdiviner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:59:10.456437 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1295 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 10:59:10.457419 nonebot-plugin-uvdiviner-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-08-03 10:12:41.000000 nonebot-plugin-uvdiviner-2.1.1/setup.py
```

### Comparing `nonebot-plugin-uvdiviner-2.1.0/LICENSE` & `nonebot-plugin-uvdiviner-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-uvdiviner-2.1.0/PKG-INFO` & `nonebot-plugin-uvdiviner-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-uvdiviner
-Version: 2.1.0
+Version: 2.1.1
 Summary: 基于周易蓍草算法的 QQ 占卜师.
 Home-page: https://gitee.com/unvisitor/nonebot-plugin-uvdiviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/nonebot-plugin-uvdiviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-uvdiviner-2.1.0/README.md` & `nonebot-plugin-uvdiviner-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-uvdiviner-2.1.0/nonebot-plugin-uvdiviner/__init__.py` & `nonebot-plugin-uvdiviner-2.1.1/nonebot-plugin-uvdiviner/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from nonebot.matcher import Matcher
 from nonebot.plugin import on_startswith
 from nonebot.adapters import Bot
 from uvdiviner.divine import quick_check, make_trigram
 from uvdiviner.evolution import trigram, diagram
 from uvdiviner.main import get_useful_data
 
+import nonebot
+import logging
+import sys
+import asyncio
+
 driver = nonebot.get_driver()
 if driver._adapters.get("OneBot V12"):
     from nonebot.adapters.onebot.v12 import MessageEvent, GroupMessageEvent
 else:
     from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
 
-import nonebot
-import logging
-import sys
-import asyncio
-
 DEBUG = True
 current_dir = Path(__file__).resolve().parent
 limit = 2
 
 divinecommand = on_startswith(".divine", priority=2, block=True)
 dqccommand = on_startswith(".dqc", priority=2, block=True)
```

### Comparing `nonebot-plugin-uvdiviner-2.1.0/nonebot_plugin_uvdiviner.egg-info/PKG-INFO` & `nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-uvdiviner
-Version: 2.1.0
+Version: 2.1.1
 Summary: 基于周易蓍草算法的 QQ 占卜师.
 Home-page: https://gitee.com/unvisitor/nonebot-plugin-uvdiviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/nonebot-plugin-uvdiviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-uvdiviner-2.1.0/setup.py` & `nonebot-plugin-uvdiviner-2.1.1/setup.py`

 * *Files identical despite different names*

