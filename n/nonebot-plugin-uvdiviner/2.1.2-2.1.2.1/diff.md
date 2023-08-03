# Comparing `tmp/nonebot-plugin-uvdiviner-2.1.2.tar.gz` & `tmp/nonebot-plugin-uvdiviner-2.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-uvdiviner-2.1.2.tar", last modified: Thu Aug  3 11:03:57 2023, max compression
+gzip compressed data, was "nonebot-plugin-uvdiviner-2.1.2.1.tar", last modified: Thu Aug  3 11:12:34 2023, max compression
```

## Comparing `nonebot-plugin-uvdiviner-2.1.2.tar` & `nonebot-plugin-uvdiviner-2.1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 11:03:57.511859 nonebot-plugin-uvdiviner-2.1.2/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 nonebot-plugin-uvdiviner-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     1295 2023-08-03 11:03:57.511859 nonebot-plugin-uvdiviner-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-08-03 10:17:59.000000 nonebot-plugin-uvdiviner-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 11:03:57.505818 nonebot-plugin-uvdiviner-2.1.2/nonebot-plugin-uvdiviner/
--rw-rw-rw-   0        0        0     3353 2023-08-03 11:02:53.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot-plugin-uvdiviner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:03:57.510856 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1295 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-03 11:03:57.000000 nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 11:03:57.511859 nonebot-plugin-uvdiviner-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-08-03 11:03:35.000000 nonebot-plugin-uvdiviner-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:12:34.449711 nonebot-plugin-uvdiviner-2.1.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 nonebot-plugin-uvdiviner-2.1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1297 2023-08-03 11:12:34.449711 nonebot-plugin-uvdiviner-2.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-08-03 10:17:59.000000 nonebot-plugin-uvdiviner-2.1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 11:12:34.439621 nonebot-plugin-uvdiviner-2.1.2.1/nonebot-plugin-uvdiviner/
+-rw-rw-rw-   0        0        0     3351 2023-08-03 11:12:22.000000 nonebot-plugin-uvdiviner-2.1.2.1/nonebot-plugin-uvdiviner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:12:34.448625 nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1297 2023-08-03 11:12:34.000000 nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-08-03 11:12:34.000000 nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:12:34.000000 nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 11:12:34.000000 nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 11:12:34.000000 nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:12:34.449711 nonebot-plugin-uvdiviner-2.1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-08-03 11:11:29.000000 nonebot-plugin-uvdiviner-2.1.2.1/setup.py
```

### Comparing `nonebot-plugin-uvdiviner-2.1.2/LICENSE` & `nonebot-plugin-uvdiviner-2.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-uvdiviner-2.1.2/PKG-INFO` & `nonebot-plugin-uvdiviner-2.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-uvdiviner
-Version: 2.1.2
+Version: 2.1.2.1
 Summary: 基于周易蓍草算法的 QQ 占卜师.
 Home-page: https://gitee.com/unvisitor/nonebot-plugin-uvdiviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/nonebot-plugin-uvdiviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-uvdiviner-2.1.2/README.md` & `nonebot-plugin-uvdiviner-2.1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-uvdiviner-2.1.2/nonebot-plugin-uvdiviner/__init__.py` & `nonebot-plugin-uvdiviner-2.1.2.1/nonebot-plugin-uvdiviner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 async def divine(matcher: Matcher):
     global DEBUG
     
     await matcher.send("\r" +
                        "天何言哉，叩之即应；神之灵矣，感而遂通。\n"
                        "今有某人，有事关心，罔知休咎，罔释厥疑，\n"
-                       "惟神惟灵，望垂昭报，若可若否，尚明告之。\n"
+                       "惟神惟灵，望垂昭报，若可若否，尚明告之。"
                        )
 
     trigrams = [make_trigram(), make_trigram(), make_trigram(),] if not DEBUG else [trigram(8), trigram(8), trigram(6),]
 
     for _ in range(1, 28):
         if not DEBUG:
             await asyncio.wait(1)
@@ -63,15 +63,15 @@
     if not DEBUG: await asyncio.wait(1)
 
     await matcher.send("本卦: " + static["卦名"] + "\n" + "卦辞: " + static["卦辞"])
 
     if not DEBUG: await asyncio.wait(1)
 
     if dia.variated != 0:
-        await matcher.send("变卦:" + variable["卦名"] + "\n   卦辞: " + variable["卦辞"] + "\n" + "变爻数:", dia.variated, "\n")
+        await matcher.send("变卦:" + variable["卦名"] + "\n   卦辞: " + variable["卦辞"] + "\n" + "变爻数:" + str(dia.variated))
     
     if not DEBUG: await asyncio.wait(2)
 
     await matcher.send(result)
 
 @driver.on_startup
 async def _():
```

### Comparing `nonebot-plugin-uvdiviner-2.1.2/nonebot_plugin_uvdiviner.egg-info/PKG-INFO` & `nonebot-plugin-uvdiviner-2.1.2.1/nonebot_plugin_uvdiviner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-uvdiviner
-Version: 2.1.2
+Version: 2.1.2.1
 Summary: 基于周易蓍草算法的 QQ 占卜师.
 Home-page: https://gitee.com/unvisitor/nonebot-plugin-uvdiviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/nonebot-plugin-uvdiviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-uvdiviner-2.1.2/setup.py` & `nonebot-plugin-uvdiviner-2.1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name = "nonebot-plugin-uvdiviner",
-    version = "2.1.2",
+    version = "2.1.2.1",
     author = "Night Resurgent <fu050409@163.com>",
     author_email = "fu050409@163.com",
     description = "基于周易蓍草算法的 QQ 占卜师.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://gitee.com/unvisitor/nonebot-plugin-uvdiviner",
     project_urls = {
```

