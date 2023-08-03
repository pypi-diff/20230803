# Comparing `tmp/nonebot_plugin_nonememe-0.1.1.post1.tar.gz` & `tmp/nonebot_plugin_nonememe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nonememe-0.1.1.post1.tar", last modified: Thu Jul 27 08:19:59 2023, max compression
+gzip compressed data, was "nonebot_plugin_nonememe-0.2.0.tar", last modified: Thu Aug  3 10:49:39 2023, max compression
```

## Comparing `nonebot_plugin_nonememe-0.1.1.post1.tar` & `nonebot_plugin_nonememe-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/LICENSE
--rw-r--r--   0        0        0     3532 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/README.md
--rw-r--r--   0        0        0      853 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__init__.py
--rw-r--r--   0        0        0     2287 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__main__.py
--rw-r--r--   0        0        0      381 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/config.py
--rw-r--r--   0        0        0     1843 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/data_source.py
--rw-r--r--   0        0        0      641 2023-07-27 08:19:59.217320 nonebot_plugin_nonememe-0.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3613 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/README.md
+-rw-r--r--   0        0        0      891 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__init__.py
+-rw-r--r--   0        0        0     2240 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__main__.py
+-rw-r--r--   0        0        0      842 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/config.py
+-rw-r--r--   0        0        0     3282 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/data_source.py
+-rw-r--r--   0        0        0      728 2023-08-03 10:49:39.554132 nonebot_plugin_nonememe-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_nonememe-0.1.1.post1/LICENSE` & `nonebot_plugin_nonememe-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.1.post1/README.md` & `nonebot_plugin_nonememe-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,10 +141,15 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.0
+
+- 自动更新图片列表
+- 缓存获取到的图片和图片列表
+
 ### 0.1.1
 
 - 发送梗图会回复指令消息
```

#### html2text {}

```diff
@@ -24,9 +24,10 @@
 (https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [NoneMeme](https://nonememe.icu/) - æ¢å¾æ¥æº ##
 ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - èªå¨æ´æ°å¾çåè¡¨ -
+ç¼å­è·åå°çå¾çåå¾çåè¡¨ ### 0.1.1 -
 åéæ¢å¾ä¼åå¤æä»¤æ¶æ¯
```

### Comparing `nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__init__.py` & `nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from nonebot import require
 from nonebot.plugin import PluginMetadata
 
+require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __plugin_meta__ = PluginMetadata(
     name="NoneMeme",
     description="NoneBot 群大佬的日常",
     usage=(
         "指令：`nonememe` / `nb草图` / `nb梗图`\n"
         "不带参数则随机选取一个，带上参数可以进行搜索，参数使用 `/` 开头及结尾使用正则表达式搜索"
     ),
```

### Comparing `nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__main__.py` & `nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,21 @@
 from nonebot.internal.adapter import Event
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 from nonebot.typing import T_State
 from nonebot_plugin_saa import Image, MessageFactory, Text
 
 from .config import config
-from .data_source import MemeItem, fetch_meme, meme_list, search_meme_items
+from .data_source import MemeItem, get_meme, meme_list, search_meme_items
 
 
 async def finish_with_meme(meme_item: MemeItem) -> NoReturn:
-    image_bytes = await fetch_meme(meme_item.path)
+    image_bytes = await get_meme(meme_item)
     await MessageFactory(
-        [
-            Text(f"# {meme_item.name}"),
-            Image(image_bytes),
-        ],
+        [Text(f"# {meme_item.name}"), Image(image_bytes)],
     ).finish(reply=True)
 
 
 cmd_meme = on_command("nonememe", aliases={"nb草图", "nb梗图"})
 
 
 @cmd_meme.handle()
@@ -34,15 +31,15 @@
 
     use_regex = arg.startswith("/") and arg.endswith("/")
     if use_regex:
         arg = arg[1:-1]
 
     searched = search_meme_items(arg, use_regex=use_regex)
     if not searched:
-        await matcher.finish("没有找到相关 NoneMeme")
+        await matcher.finish("没有找到相关图片")
     if len(searched) == 1:
         await finish_with_meme(searched[0])
 
     over_length = len(searched) > config.nonememe_search_limit
     if over_length:
         searched = searched[: config.nonememe_search_limit]
     state["items"] = searched
```

### Comparing `nonebot_plugin_nonememe-0.1.1.post1/pyproject.toml` & `nonebot_plugin_nonememe-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "nonebot-plugin-nonememe"
-version = "0.1.1.post1"
+version = "0.2.0"
 description = "The daily life of the NoneBot group members"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
-    "pydantic>=1.10.4,<2",
     "nonebot-plugin-send-anything-anywhere>=0.2.7",
+    "nonebot-plugin-apscheduler>=0.3.0",
+    "pydantic>=1.10.4,<2",
     "httpx>=0.24.1",
     "json5>=0.9.14",
+    "anyio>=3.7.1",
+    "typing-extensions>=4.7.1",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_nonememe-0.1.1.post1/PKG-INFO` & `nonebot_plugin_nonememe-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nonememe
-Version: 0.1.1.post1
+Version: 0.2.0
 Summary: The daily life of the NoneBot group members
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
-Requires-Dist: pydantic<2,>=1.10.4
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
+Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
+Requires-Dist: pydantic<2,>=1.10.4
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: json5>=0.9.14
+Requires-Dist: anyio>=3.7.1
+Requires-Dist: typing-extensions>=4.7.1
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
@@ -157,10 +160,15 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.0
+
+- 自动更新图片列表
+- 缓存获取到的图片和图片列表
+
 ### 0.1.1
 
 - 发送梗图会回复指令消息
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.1.1.post1
-Summary: The daily life of the NoneBot group members Home-page: https://
-github.com/lgc-NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.2.0 Summary: The
+daily life of the NoneBot group members Home-page: https://github.com/lgc-
+NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-nonememe Requires-Python: <4.0,>=3.8 Requires-Dist:
-nonebot2>=2.0.0 Requires-Dist: pydantic<2,>=1.10.4 Requires-Dist: nonebot-
-plugin-send-anything-anywhere>=0.2.7 Requires-Dist: httpx>=0.24.1 Requires-
-Dist: json5>=0.9.14 Description-Content-Type: text/markdown
+nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
+Requires-Dist: nonebot-plugin-apscheduler>=0.3.0 Requires-Dist:
+pydantic<2,>=1.10.4 Requires-Dist: httpx>=0.24.1 Requires-Dist: json5>=0.9.14
+Requires-Dist: anyio>=3.7.1 Requires-Dist: typing-extensions>=4.7.1
+Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # NoneBot-Plugin-NoneMeme _â¨ çç NoneBot ç¾¤å¤§ä½¬ä»¬çæ¥å¸¸ â¨_
                       [python] [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç» ### æå¥½èå ![æå¥½èå](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/nonememe/intro.png) ## ð¿
@@ -32,9 +34,10 @@
 (https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [NoneMeme](https://nonememe.icu/) - æ¢å¾æ¥æº ##
 ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - èªå¨æ´æ°å¾çåè¡¨ -
+ç¼å­è·åå°çå¾çåå¾çåè¡¨ ### 0.1.1 -
 åéæ¢å¾ä¼åå¤æä»¤æ¶æ¯
```

