# Comparing `tmp/nonebot-plugin-uvdiviner-2.1.1.tar.gz` & `tmp/nonebot-plugin-uvdiviner-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-uvdiviner-2.1.1.tar", last modified: Thu Aug  3 10:59:10 2023, max compression
+gzip compressed data, was "nonebot-plugin-uvdiviner-2.1.2.tar", last modified: Thu Aug  3 11:03:57 2023, max compression
```

## Comparing `nonebot-plugin-uvdiviner-2.1.1.tar` & `nonebot-plugin-uvdiviner-2.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 10:59:10.457419 nonebot-plugin-uvdiviner-2.1.1/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 nonebot-plugin-uvdiviner-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     1295 2023-08-03 10:59:10.457419 nonebot-plugin-uvdiviner-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-08-03 10:17:59.000000 nonebot-plugin-uvdiviner-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 10:59:10.431417 nonebot-plugin-uvdiviner-2.1.1/nonebot-plugin-uvdiviner/
--rw-rw-rw-   0        0        0     3411 2023-08-03 10:58:29.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot-plugin-uvdiviner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:59:10.456437 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1295 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-03 10:59:10.000000 nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 10:59:10.457419 nonebot-plugin-uvdiviner-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-08-03 10:12:41.000000 nonebot-plugin-uvdiviner-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:03:57.511859 nonebot-plugin-uvdiviner-2.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 nonebot-plugin-uvdiviner-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1295 2023-08-03 11:03:57.511859 nonebot-plugin-uvdiviner-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-08-03 10:17:59.000000 nonebot-plugin-uvdiviner-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 11:03:57.505818 nonebot-plugin-uvdiviner-2.1.2/nonebot-plugin-uvdiviner/
+-rw-rw-rw-   0        0        0     3353 2023-08-03 11:02:53.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot-plugin-uvdiviner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:03:57.510856 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1295 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:03:57.511859 nonebot-plugin-uvdiviner-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-08-03 11:03:35.000000 nonebot-plugin-uvdiviner-2.1.2/setup.py
```

### Comparing `nonebot-plugin-uvdiviner-2.1.1/LICENSE` & `nonebot-plugin-uvdiviner-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-uvdiviner-2.1.1/PKG-INFO` & `nonebot-plugin-uvdiviner-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-uvdiviner
-Version: 2.1.1
+Version: 2.1.2
 Summary: 基于周易蓍草算法的 QQ 占卜师.
 Home-page: https://gitee.com/unvisitor/nonebot-plugin-uvdiviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/nonebot-plugin-uvdiviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-uvdiviner-2.1.1/README.md` & `nonebot-plugin-uvdiviner-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-uvdiviner-2.1.1/nonebot-plugin-uvdiviner/__init__.py` & `nonebot-plugin-uvdiviner-2.1.2/nonebot-plugin-uvdiviner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from pathlib import Path
 from loguru import logger
-from nonebot.rule import Rule
 from nonebot.matcher import Matcher
 from nonebot.plugin import on_startswith
-from nonebot.adapters import Bot
 from uvdiviner.divine import quick_check, make_trigram
 from uvdiviner.evolution import trigram, diagram
 from uvdiviner.main import get_useful_data
 
 import nonebot
 import logging
 import sys
@@ -90,13 +88,13 @@
     logger.success("欧若可卜师初始化完毕.")
 
 @divinecommand.handle()
 async def divinehandler(matcher: Matcher, event: GroupMessageEvent):
     global limit
     if limit <= 0 and not DEBUG:
         await matcher.send("今日占卜次数已达安全上限, 欧若可拒绝继续进行占卜.")
-    await divine()
+    await divine(matcher)
     limit -= 1
 
 @dqccommand.handle()
 async def dqchandler(matcher: Matcher, event: GroupMessageEvent):
     await matcher.send(str(quick_check()))
```

### Comparing `nonebot-plugin-uvdiviner-2.1.1/nonebot_plugin_uvdiviner.egg-info/PKG-INFO` & `nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-uvdiviner
-Version: 2.1.1
+Version: 2.1.2
 Summary: 基于周易蓍草算法的 QQ 占卜师.
 Home-page: https://gitee.com/unvisitor/nonebot-plugin-uvdiviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/nonebot-plugin-uvdiviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-uvdiviner-2.1.1/setup.py` & `nonebot-plugin-uvdiviner-2.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from uvdiviner import __version__
-
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name = "nonebot-plugin-uvdiviner",
-    version = __version__,
+    version = "2.1.2",
     author = "Night Resurgent <fu050409@163.com>",
     author_email = "fu050409@163.com",
     description = "基于周易蓍草算法的 QQ 占卜师.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://gitee.com/unvisitor/nonebot-plugin-uvdiviner",
     project_urls = {
```

