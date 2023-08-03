# Comparing `tmp/nonebot_plugin_bilibilibot-2.3.2.tar.gz` & `tmp/nonebot_plugin_bilibilibot-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilibilibot-2.3.2.tar", last modified: Sun May 14 05:46:11 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilibilibot-2.3.3.tar", last modified: Thu Aug  3 13:47:40 2023, max compression
```

## Comparing `nonebot_plugin_bilibilibot-2.3.2.tar` & `nonebot_plugin_bilibilibot-2.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    35149 2022-03-08 12:03:37.000000 nonebot_plugin_bilibilibot-2.3.2/LICENSE
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       53 2022-04-15 09:07:46.000000 nonebot_plugin_bilibilibot-2.3.2/MANIFEST.in
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/PKG-INFO
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      689 2022-04-17 08:31:02.000000 nonebot_plugin_bilibilibot-2.3.2/README.rst
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.656836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    18719 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/__init__.py
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     2736 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/basicFunc.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     9051 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliStream.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    10417 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     8897 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliVideo.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    36042 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_client.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    13242 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     8410 2022-12-25 13:05:59.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    26482 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_task.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    21245 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/db.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     2594 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/exception.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      707 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/rule.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      168 2022-08-27 03:42:13.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/config.py
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.656836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      109 2022-04-15 08:25:37.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/announcement.json
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      815 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/help.json
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.656836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/PKG-INFO
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     1013 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)        1 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/dependency_links.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       56 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/requires.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       27 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/top_level.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       38 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/setup.cfg
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      904 2023-05-14 05:42:59.000000 nonebot_plugin_bilibilibot-2.3.2/setup.py
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-08-03 13:47:40.304682 nonebot_plugin_bilibilibot-2.3.3/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    35149 2022-03-08 12:03:37.000000 nonebot_plugin_bilibilibot-2.3.3/LICENSE
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       53 2022-04-15 09:07:46.000000 nonebot_plugin_bilibilibot-2.3.3/MANIFEST.in
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2023-08-03 13:47:40.304682 nonebot_plugin_bilibilibot-2.3.3/PKG-INFO
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      689 2022-04-17 08:31:02.000000 nonebot_plugin_bilibilibot-2.3.3/README.rst
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-08-03 13:47:40.288682 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    18719 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/__init__.py
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-08-03 13:47:40.288682 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     2736 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/basicFunc.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     9168 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/biliStream.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    10473 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     8998 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/biliVideo.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    40210 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_client.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    13326 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     8410 2022-12-25 13:05:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    26482 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_task.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    22719 2023-08-03 13:46:59.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/db.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     2594 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/exception.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      707 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/rule.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      168 2022-08-27 03:42:13.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/config.py
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-08-03 13:47:40.284682 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/file/
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-08-03 13:47:40.304682 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/file/source/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      109 2022-04-15 08:25:37.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/file/source/announcement.json
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      815 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/file/source/help.json
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-08-03 13:47:40.288682 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2023-08-03 13:47:39.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/PKG-INFO
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     1013 2023-08-03 13:47:39.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)        1 2023-08-03 13:47:39.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       56 2023-08-03 13:47:39.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/requires.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       27 2023-08-03 13:47:39.000000 nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/top_level.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       38 2023-08-03 13:47:40.304682 nonebot_plugin_bilibilibot-2.3.3/setup.cfg
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      904 2023-08-03 13:47:15.000000 nonebot_plugin_bilibilibot-2.3.3/setup.py
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/LICENSE` & `nonebot_plugin_bilibilibot-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/PKG-INFO` & `nonebot_plugin_bilibilibot-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_bilibilibot
-Version: 2.3.2
+Version: 2.3.3
 Summary: 基于Nonebot的bilibili通知插件，可将up主，主播以及番剧的更新/直播动态推送到QQ
 Home-page: https://github.com/TDK1969/nonebot_plugin_bilibilibot
 Author: TDK
 Author-email: tdk1969@foxmail.com
 License: GNU
 Keywords: nonebot
 Platform: UNKNOWN
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/README.rst` & `nonebot_plugin_bilibilibot-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/__init__.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/basicFunc.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/basicFunc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliStream.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/biliStream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Tuple, List
 import sys
 import traceback
 import nonebot
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot.adapters.onebot.v11.adapter import Adapter
 from .basicFunc import *
 from .exception import *
 import asyncio
 from .bili_client import bili_client
 from .bili_task import bili_task_manager
 __PLUGIN_NAME = "[bilibilibot~直播]"
 async def check_bili_live() -> None:
@@ -18,28 +19,27 @@
     如果主播开播状态改变,则更新数据库
     ---------
     @param  :
     -------
     @Returns  :
     -------
     """
-    logger.debug("running check_bili_live")
     liver_list = list(bili_task_manager.liver_list.values())
     
     sched_bot = nonebot.get_bot()
     
     """results = await asyncio.gather(
         *[bili_client.get_live_status(liver_info[0], liver_info[3]) for liver_info in liver_list],
         return_exceptions=True
     )"""
-
-    results = await asyncio.gather(
-        *[bili_client.get_live_status(liver_info["liver_uid"], liver_info["room_id"]) for liver_info in liver_list],
-        return_exceptions=True
-    )
+    async with httpx.AsyncClient(headers={"User-Agent":"Mozilla/5.0"}) as client:
+        results = await asyncio.gather(
+            *[bili_client.get_live_status(client, liver_info["liver_uid"], liver_info["room_id"]) for liver_info in liver_list],
+            return_exceptions=True
+        )
     for i in range(len(liver_list)):
         if isinstance(results[i], tuple):
             if results[i][0] and not liver_list[i]["is_live"]:
                 logger.info(f'[{__PLUGIN_NAME}]检测到主播 <{liver_list[i]["liver_name"]}> 已开播！')
                 text_msg = '【直播动态】\n<{}>正在直播!\n标题: {}\n链接: {}'.format(liver_list[i]["liver_name"], results[i][1], f"https://live.bilibili.com/{liver_list[i]['room_id']}")
                 reported_msg = text_msg + MessageSegment.image(results[i][2])
                 logger.info(f'[{__PLUGIN_NAME}]向粉丝发送开播通知')
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     @param  :
     无
     -------
     @Returns  :
     无
     -------
     """
-    logger.debug("running check_telegram_update")
     telegram_list = list(bili_task_manager.telegram_list.values())
     telegram_list = [i for i in telegram_list if i["is_finish"] is False]
     sched_bot = nonebot.get_bot()
     # 只对未完结的番剧进行检查
-    results = await asyncio.gather(
-        *[bili_client.get_telegram_latest_episode(telegram_info["season_id"], telegram_info["episode"]) for telegram_info in telegram_list],
-        return_exceptions=True
-    )
+    async with httpx.AsyncClient(headers={"User-Agent":"Mozilla/5.0"}) as client:
+        results = await asyncio.gather(
+            *[bili_client.get_telegram_latest_episode(client, telegram_info["season_id"], telegram_info["episode"]) for telegram_info in telegram_list],
+            return_exceptions=True
+        )
 
     for i in range(len(telegram_list)):
         if isinstance(results[i], tuple):
             if results[i][0] is True:
                 logger.info(f'[{__PLUGIN_NAME}]检测到影视剧 <{telegram_list[i]["telegram_title"]}> 更新')
                 text_msg = "【B站动态】\n《{}》已更新第{}集\n标题: {}\n链接: {}\n".format(
                         telegram_list[i]["telegram_title"], results[i][1], results[i][2], results[i][3]
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliVideo.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/biliVideo.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     -------
     """
     logger.debug("running check_up_update")
     schedBot = nonebot.get_bot()
     #assert status == True, "数据库发生错误"
     check_up_list = bili_task_manager.get_up_check_update_list()
     #logger.debug(f'{__PLUGIN_NAME}check_up_list = {check_up_list}')
-    
-    results = await asyncio.gather(
-        *[bili_client.get_latest_video(uid, bili_task_manager.up_list[uid]["latest_timestamp"]) for uid in check_up_list],
-        return_exceptions=True
-    )
+    async with httpx.AsyncClient(headers={"User-Agent":"Mozilla/5.0"}) as client:
+        results = await asyncio.gather(
+            *[bili_client.get_latest_video(client, uid, bili_task_manager.up_list[uid]["latest_timestamp"]) for uid in check_up_list],
+            return_exceptions=True
+        )
     
     for i in range(len(check_up_list)):
         if isinstance(results[i], tuple):
             if results[i][0] is True:
                 up_uid = check_up_list[i]
                 up_name = bili_task_manager.up_list[up_uid]["up_name"]
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_client.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+import json
 import httpx
-from random import choice, uniform
+from random import choice, uniform, randint
 import asyncio
 import time
 from typing import List, Tuple, Dict
 from .exception import BiliAPI404Error, BiliAPIRetCodeError, BiliConnectionError, BiliDatebaseError, BiliInvalidRoomId, BiliInvalidShortUrl, BiliNoLiveRoom, BiliStatusCodeError
 from nonebot.log import logger
+from functools import reduce
+from hashlib import md5
+import urllib.parse
+import uuid
+import re
+from nonebot import require
 
 __PLUGIN_NAME__ = "[bilibilibot~Client]"
 class BiliClient():
     def __init__(self) -> None:
         self.__proxy_pool__ = [None]
         self.__retry_times__ = 3
         self.__ua_list__ = [
@@ -59,71 +66,144 @@
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.90 Safari/537.36",
             "Mozilla/5.0 (X11; NetBSD) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.116 Safari/537.36",
             "Mozilla/5.0 (X11; CrOS i686 3912.101.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.116 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1312.60 Safari/537.17",
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_2) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1309.0 Safari/537.17"
         ]
-        self.__usable_ip_list__ = set()
 
         self.API = {
             # 用于获取临时cookie
             "get_bili_cookie": "https://www.bilibili.com",
-            "get_user_info_by_uid": "https://api.bilibili.com/x/space/wbi/acc/info?mid={}",
-            "get_latest_video_by_uid": "https://api.bilibili.com/x/space/wbi/arc/search?mid={}&ps=1&tid=0&pn=1&order=pubdate&jsonp=jsonp",
-            "get_live_info_by_room_id": "https://api.live.bilibili.com/room/v1/Room/get_info?room_id={}",
-            "get_liver_info_by_uid": "https://api.live.bilibili.com/live_user/v1/Master/info?uid={}",
-            "get_telegram_info_by_media_id": "https://api.bilibili.com/pgc/review/user?media_id={}",
-            "get_telegram_info_by_ep_id": "https://api.bilibili.com/pgc/view/web/season?ep_id={}",
-            "get_telegram_info_by_season_id": "https://api.bilibili.com/pgc/view/web/season?season_id={}",
-            "get_telegram_latest_episode": "https://api.bilibili.com/pgc/view/web/season?season_id={}",
-            "get_dynamic_list_by_uid": "https://api.bilibili.com/x/polymer/web-dynamic/v1/feed/space?host_mid={}&timezone_offset=-480",
-            "get_detail_dynamic_by_id": "https://t.bilibili.com/{}"
+            "get_user_info_by_uid": "https://api.bilibili.com/x/space/wbi/acc/info",
+            "get_latest_video_by_uid": "https://api.bilibili.com/x/space/wbi/arc/search",
+            "get_live_info_by_room_id": "https://api.live.bilibili.com/room/v1/Room/get_info",
+            "get_liver_info_by_uid": "https://api.live.bilibili.com/live_user/v1/Master/info",
+            "get_telegram_info_by_media_id": "https://api.bilibili.com/pgc/review/user",
+            "get_telegram_info_by_ep_id": "https://api.bilibili.com/pgc/view/web/season",
+            "get_telegram_info_by_season_id": "https://api.bilibili.com/pgc/view/web/season",
+            "get_telegram_latest_episode": "https://api.bilibili.com/pgc/view/web/season",
+            "get_dynamic_list_by_uid": "https://api.bilibili.com/x/polymer/web-dynamic/v1/feed/space",
+            "get_detail_dynamic_by_id": "https://t.bilibili.com/{}",
+            "get_api_access": "https://api.bilibili.com/x/internal/gaia-gateway/ExClimbWuzhi",
+            "get_img_sub_key": "https://api.bilibili.com/x/web-interface/nav",
         }
-
-        self.__proxy_lock__ = asyncio.Lock()
-
-    @classmethod
-    async def async_client_init(cls) -> "BiliClient":
-        self = cls()
-        await self.update_proxy_pool()
-        return self
+        self.headers = {"User-Agent": "Mozilla/5.0"}
+        self.img_key = self.sub_key = ""
+        self.get_img_key_and_sub_key()
+        self.dynamic_cookie = httpx.Cookies()
+        self.update_dynamic_cookie()
 
 
     def __request_header__(self) -> httpx.Headers:
         '''返回随机UA的header
 
         Returns:
             httpx.Headers: 返回header
         '''
         headers = {
             'User-Agent': choice(self.__ua_list__),
         }
         return httpx.Headers(headers)
 
+    async def get_today_img_key_and_sub_key(self) -> Tuple[str, str]:
+        '''获取今天的img_key和sub_key参数
+
+        Returns:
+            Tuple[str, str]: (img_key, sub_key)
+        '''
+        try:
+            async with httpx.AsyncClient(headers=self.headers) as client:
+                r1 = await client.get("https://api.bilibili.com/x/web-interface/nav")
+        except Exception as e:
+            pass
+        
+        r1_json = r1.json()
+        img_url: str = r1_json['data']['wbi_img']['img_url']
+        sub_url: str = r1_json['data']['wbi_img']['sub_url']
+
+        img_key = img_url.rsplit('/', 1)[1].split('.')[0]
+        sub_key = sub_url.rsplit('/', 1)[1].split('.')[0]
+
+        return img_key, sub_key
+
+    def get_img_key_and_sub_key(self) -> None:
+        '''获取今天的img_key和sub_key参数
+
+        Returns:
+            Tuple[str, str]: (img_key, sub_key)
+        '''
+        try:
+            r1 = httpx.get(self.API["get_img_sub_key"], headers=self.headers)
+        except Exception as e:
+            logger.error(f"获取img_key和sub_key时发生错误: {e}")
+            return "", ""
+        
+        r1_json = r1.json()
+        img_url: str = r1_json['data']['wbi_img']['img_url']
+        sub_url: str = r1_json['data']['wbi_img']['sub_url']
+
+        img_key = img_url.rsplit('/', 1)[1].split('.')[0]
+        sub_key = sub_url.rsplit('/', 1)[1].split('.')[0]
+
+        self.img_key = img_key
+        self.sub_key = sub_key
+
+    def get_mixinkey(self, orig: str):
+        '对 imgKey 和 subKey 进行字符顺序打乱编码'
+        mixinKeyEncTab = [
+            46, 47, 18, 2, 53, 8, 23, 32, 15, 50, 10, 31, 58, 3, 45, 35, 27, 43, 5, 49,
+            33, 9, 42, 19, 29, 28, 14, 39, 12, 38, 41, 13, 37, 48, 7, 16, 24, 55, 40,
+            61, 26, 17, 0, 1, 60, 51, 30, 4, 22, 25, 54, 21, 56, 59, 6, 63, 57, 62, 11,
+            36, 20, 34, 44, 52
+        ]
+        return reduce(lambda s, i: s + orig[i], mixinKeyEncTab, '')[:32]
     
-    
-    async def get_latest_video(self, uid: str, last_udpate_time: int) -> Tuple[bool, str, str, int, str]:
+    def wbi_sign(self, params: dict):
+        '为请求参数进行 wbi 签名'
+        mixin_key = self.get_mixinkey(self.img_key + self.sub_key)
+        curr_time = round(time.time())
+        params['wts'] = curr_time                                   # 添加 wts 字段
+        params = dict(sorted(params.items()))                       # 按照 key 重排参数
+        # 过滤 value 中的 "!'()*" 字符
+        params = {
+            k : ''.join(filter(lambda chr: chr not in "!'()*", str(v)))
+            for k, v
+            in params.items()
+        }
+        query = urllib.parse.urlencode(params)                      # 序列化参数
+        wbi_sign = md5((query + mixin_key).encode()).hexdigest()    # 计算 w_rid
+        params['w_rid'] = wbi_sign
+        return params
+
+    async def get_latest_video(self, client: httpx.AsyncClient, uid: str, last_udpate_time: int) -> Tuple[bool, str, str, int, str]:
         """
         @description  :
         根据uid和时间戳, 返回元组，表示存在新视频或无新视频
         ---------
         @param  :
+        client: httpx.AsyncClient
         uid: 查询新视频用户的uid
         last_udpate_time: 数据库中记录的最新视频的时间戳
         -------
         @Returns  :
         返回一个元组[是否更新，bv号，标题，发布时间戳，封面的链接]
         -------
         """
         try:
-            async with httpx.AsyncClient(headers=self.__request_header__()) as client:
-                await client.get(url=self.API["get_bili_cookie"])
-                time.sleep(uniform(2, 4))
-                response = await client.get(url=self.API["get_latest_video_by_uid"].format(uid))
+            """mid={}&ps=1&tid=0&pn=1&order=pubdate&jsonp=jsonp"""
+            params = {
+                "mid": uid,
+                "ps": 1,
+                "tid": 0,
+                "pn": 1,
+                "order": "pubdate",
+                "jsonp": "jsonp"
+            }
+            response = await client.get(url=self.API["get_latest_video_by_uid"], params=self.wbi_sign(params))
         except Exception as e:
             raise BiliConnectionError(0, uid, e.args[0])
 
         if response.status_code != 200:
             raise BiliStatusCodeError(0, uid, response.status_code)
 
         response = response.json()
@@ -154,33 +234,32 @@
         -------
         @Returns  :
         返回一个元组
         [up主名字，最新视频的时间戳]
         -------
         """
         
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(self.API["get_bili_cookie"])
-                response1 = await client.get(url=self.API["get_user_info_by_uid"].format(uid))
+                response1 = await client.get(url=self.API["get_user_info_by_uid"], params=self.wbi_sign({"mid": uid}))
             except Exception as e:
                 raise BiliConnectionError(0, uid, e.args[0])
 
             if response1.status_code != 200:
                 raise  BiliStatusCodeError(0, uid, response1.status_code)
             
             response1 = response1.json()
             if response1["code"] == -404:
                 raise BiliAPI404Error()
             elif response1["code"] != 0:
                 raise BiliAPIRetCodeError(0, uid, response1["code"], response1["message"])
             
             user_name = response1["data"]["name"]
             try:
-                response2 = await client.get(url=self.API["get_latest_video_by_uid"].format(uid))
+                response2 = await client.get(url=self.API["get_latest_video_by_uid"], params=self.wbi_sign({"mid": uid,"ps": 1,"tid": 0,"pn": 1,"order": "pubdate","jsonp": "jsonp"}))
             except Exception as e:
                 raise BiliConnectionError(0, uid, e.args[0])
 
             if response2.status_code != 200:
                 raise  BiliStatusCodeError(0, uid, response2.status_code)
     
             response2 = response2.json()
@@ -188,51 +267,49 @@
                 raise BiliAPIRetCodeError(0, uid, response2["code"], response2["message"])
             
             latest_video = response2['data']['list']['vlist'][0] if len(response2['data']['list']['vlist']) != 0 else {}
             post_time = latest_video.get("created", 0)
 
             return (user_name, post_time)
            
-    async def get_live_status(self, uid: str, room_id: str) -> Tuple[bool, str, str]:
+    async def get_live_status(self, client:httpx.AsyncClient, uid: str, room_id: str) -> Tuple[bool, str, str]:
         """
         @description  :
         根据房间号,获取直播间是否开播
         ---------
         @param  :
         uid: 主播的uid
         room_id: 直播间号
         -------
         @Returns  :
         返回一个元组
         [是否正在直播，直播间标题，直播间封面链接]
         -------
         """
         
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
-            try:
-                await client.get(self.API["get_bili_cookie"])
-                response = await client.get(self.API["get_live_info_by_room_id"].format(room_id))
-            except Exception as e:
-                raise BiliConnectionError(1, uid, e.args[0])
-            
-            if response.status_code != 200:
-                raise BiliStatusCodeError(1, uid, response.status_code)
-            
-            response = response.json()
-            if response["code"] != 0:
-                raise BiliAPIRetCodeError(1, uid, response["code"], response["message"])
-            
-            live_status = response["data"]["live_status"]
-            title = response["data"]["title"]
-            cover_url = response["data"]["user_cover"]
+        try:
+            response = await client.get(self.API["get_live_info_by_room_id"], params={"room_id": room_id})
+        except Exception as e:
+            raise BiliConnectionError(1, uid, e.args[0])
         
-            if live_status == 1:
-                return (True, title, cover_url)
-            else:
-                return (False, "", "")
+        if response.status_code != 200:
+            raise BiliStatusCodeError(1, uid, response.status_code)
+        
+        response = response.json()
+        if response["code"] != 0:
+            raise BiliAPIRetCodeError(1, uid, response["code"], response["message"])
+        
+        live_status = response["data"]["live_status"]
+        title = response["data"]["title"]
+        cover_url = response["data"]["user_cover"]
+    
+        if live_status == 1:
+            return (True, title, cover_url)
+        else:
+            return (False, "", "")
     
     async def init_liver_info(self, uid: str) -> Tuple[str, str]:
         """
         @description  :
         根据uid，返回直播间信息
         ---------
         @param  :
@@ -240,18 +317,17 @@
         -------
         @Returns  :
         返回一个元组
         [用户名，直播间房间号]
         -------
         """
 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(self.API["get_bili_cookie"])
-                response = await client.get(self.API["get_liver_info_by_uid"].format(uid))
+                response = await client.get(self.API["get_liver_info_by_uid"], params={"uid": uid})
             except Exception as e:
                 raise BiliConnectionError(0, uid, e.args[0])
             
         if response.status_code != 200:
             raise BiliStatusCodeError(1, uid, response.status_code)
         
         response = response.json()
@@ -274,18 +350,17 @@
 
         Returns:
             Tuple[str, str]: 
             返回一个元组
             [主播uid, 主播用户名]
         '''
 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(url=self.API["get_bili_cookie"])
-                response1 = await client.get(url=self.API["get_live_info_by_room_id"].format(room_id))
+                response1 = await client.get(url=self.API["get_live_info_by_room_id"], params={"room_id": room_id})
             except Exception as e:
                 raise BiliConnectionError(1, f"房间号:{room_id}", e.args[0])
             
             if response1.status_code != 200:
                 raise BiliStatusCodeError(1, f"房间号:{room_id}", response1.status_code)
 
             response1 = response1.json()
@@ -293,15 +368,15 @@
                 raise BiliInvalidRoomId(room_id)
             if response1["code"] != 0:
                 raise BiliAPIRetCodeError(1, f"房间号:{room_id}", response1["code"], response1["message"])
             
             uid = str(response1["data"]["uid"])
 
             try:
-                response2 = await client.get(self.API["get_liver_info_by_uid"].format(uid))
+                response2 = await client.get(self.API["get_liver_info_by_uid"], params={"uid": uid})
             except Exception as e:
                 raise BiliConnectionError(0, uid, e.args[0])
             
             if response2.status_code != 200:
                 raise  BiliStatusCodeError(1, uid, response2.status_code)
     
             response2 = response2.json()
@@ -320,18 +395,17 @@
 
         Returns:
             Tuple[int, str, int, bool]: 
             返回一个元组
             [season_id, 番剧名, 最新集, 是否完结]
         '''
 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(url=self.API["get_bili_cookie"])
-                response = await client.get(url=self.API["get_telegram_info_by_ep_id"].format(ep_id))
+                response = await client.get(url=self.API["get_telegram_info_by_ep_id"], params={"ep_id": ep_id})
             except Exception as e:
                 raise BiliConnectionError(2, f"ep_id:{ep_id}", e.args[0])
             
             if response.status_code != 200:
                 raise BiliStatusCodeError(2, f"ep_id:{ep_id}", response.status_code)
     
             response = response.json()
@@ -340,16 +414,14 @@
             elif response["code"] != 0:
                 raise BiliAPIRetCodeError(2, f"ep_id:{ep_id}", response["code"], response["message"])
 
             season_id = response["result"]["season_id"]
             season_title = response["result"]["season_title"]
             is_finish = bool(response["result"]["publish"]["is_finish"])
             latest_episode = len(response["result"]["episodes"])
-    
-
 
             return (season_id, season_title, latest_episode, is_finish)
 
     async def init_telegram_info_by_season_id(self, season_id: int) -> Tuple[int, str, int, bool]:
         ''' 根据season_id初始化番剧信息
 
         Args:
@@ -357,18 +429,17 @@
 
         Returns:
             Tuple[int, str, int, bool]: 
             返回一个元组
             [season_id, 番剧名, 最新集, 是否完结]
         '''
 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(url=self.API["get_bili_cookie"])
-                response = await client.get(url=self.API["get_telegram_info_by_season_id"].format(season_id))
+                response = await client.get(url=self.API["get_telegram_info_by_season_id"], params={"season_id": season_id})
             except Exception as e:
                 raise BiliConnectionError(2, f"season_id:{season_id}", e.args[0])
             
             if response.status_code != 200:
                 raise BiliStatusCodeError(2, f"season_id:{season_id}", response.status_code)
     
             response = response.json()
@@ -391,18 +462,17 @@
 
         Returns:
             Tuple[int, str, int, bool]: 
             返回一个元组
             [season_id, 番剧名, 最新集, 是否完结]
         '''
 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(url=self.API["get_bili_cookie"])
-                response = await client.get(url=self.API["get_telegram_info_by_media_id"].format(media_id))
+                response = await client.get(url=self.API["get_telegram_info_by_media_id"], params={"media_id": media_id})
             except Exception as e:
                 raise BiliConnectionError(2, f"media_id:{media_id}", e.args[0])
             
             if response.status_code != 200:
                 raise BiliStatusCodeError(2, f"media_id:{media_id}", response.status_code)
     
             response = response.json()
@@ -414,68 +484,66 @@
             season_id = response["result"]["media"]["season_id"]
             season_title = response["result"]["media"]["title"]
             is_finish = False
             latest_episode = int(response["result"]["media"]["new_ep"]["index"])
 
             return (season_id, season_title, latest_episode, is_finish)
     
-    async def get_telegram_latest_episode(self, season_id: int, index: int) -> Tuple[bool, int, str, str, str, bool]:
+    async def get_telegram_latest_episode(self, client: httpx.AsyncClient, season_id: int, index: int) -> Tuple[bool, int, str, str, str, bool]:
         '''根据season_id获取番剧的最新集信息
 
         Args:
             season_id (int): season_id
             index (int): 记录的最新集数
 
         Returns:
             Tuple[bool, int, str, str, str, bool]: 
             返回一个元组
             [是否更新, 最新集数, 最新集标题, 最新集链接, 封面链接, 是否完结]
         '''
 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
-            try:
-                await client.get(url=self.API["get_bili_cookie"])
-                response = await client.get(url=self.API["get_telegram_latest_episode"].format(season_id))
-            except Exception as e:
-                raise BiliConnectionError(2, f"season_id:{season_id}", e.args[0])
-            
-            if response.status_code != 200:
-                raise BiliStatusCodeError(2, f"season_id:{season_id}", response.status_code)
-    
-            response = response.json()
-            if response["code"] != 0:
-                raise BiliAPIRetCodeError(2, f"season_id:{season_id}", response["code"], response["message"])
+        
+        try:
+            response = await client.get(url=self.API["get_telegram_latest_episode"], params={"season_id": season_id})
+        except Exception as e:
+            raise BiliConnectionError(2, f"season_id:{season_id}", e.args[0])
+        
+        if response.status_code != 200:
+            raise BiliStatusCodeError(2, f"season_id:{season_id}", response.status_code)
 
-            episodes = response['result']['episodes']
-            is_finish = bool(response["result"]["publish"]["is_finish"])
+        response = response.json()
+        if response["code"] != 0:
+            raise BiliAPIRetCodeError(2, f"season_id:{season_id}", response["code"], response["message"])
 
-            if len(episodes) > index:
-                latest_episode = episodes[-1]
-                cover_url = latest_episode['cover']
-                title = latest_episode['long_title']
-                play_url = latest_episode['share_url']
-                
-                return (True, len(episodes), title, play_url, cover_url, is_finish)
-            else:
-                return (False, 0, "", "", "", is_finish)
+        episodes = response['result']['episodes']
+        is_finish = bool(response["result"]["publish"]["is_finish"])
+
+        if len(episodes) > index:
+            latest_episode = episodes[-1]
+            cover_url = latest_episode['cover']
+            title = latest_episode['long_title']
+            play_url = latest_episode['share_url']
+            
+            return (True, len(episodes), title, play_url, cover_url, is_finish)
+        else:
+            return (False, 0, "", "", "", is_finish)
     
     async def parse_short_url(self, short_url: str) -> Tuple[int, str]:
         '''解析b23.tv的短链接,返回短链接类型以及目标id
 
         Args:
             short_url (str): 短链接
 
         Returns:
             Tuple[int, str]: 
             返回一个元组
             [类型:0-up的uid,1-主播的房间号,2-番剧的ep_id, 目标id]
         '''
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(url=self.API["get_bili_cookie"])
                 response = await client.get(url=short_url)
             except Exception as e:
                 raise BiliConnectionError(3, short_url, e.args[0])
             
             if response.status_code != 302:
                 raise BiliStatusCodeError(3, short_url, response.status_code)
             
@@ -487,48 +555,93 @@
             elif "live" in origin_url:
                 return (1, target_id)
             elif "bangumi" in origin_url:
                 return (2, target_id)
             
             raise BiliInvalidShortUrl(short_url)
 
+    def update_dynamic_cookie(self) -> None:
+        headers = {
+            'user-agent': 'Mozilla/5.0',
+            'referer': 'https://www.bilibili.com/',
+            "Host": "space.bilibili.com",
+            'accept-language': 'zh-CN,zh;q=0.9',
+        }
+        with httpx.Client(headers=headers) as client:
+            cookies = httpx.Cookies({'_uuid': f'{str(uuid.uuid4()).upper()}{randint(0, 99999):05d}infoc'})
+            
+            response = client.get(
+                'https://www.bilibili.com/1/dynamic',
+                cookies=cookies
+            )
+            spm_prefix = re.search(r'<meta name="spm_prefix" content="([^"]+?)">', response.text).group(1)
+            cookies.update(response.cookies)
+
+            data = {
+                '3064': 1,
+                '39c8': f'{spm_prefix}.fp.risk',
+                '3c43': {
+                    'adca': 'Linux',
+                },
+                # 'df35': cookies['_uuid']
+            }
+
+            json_data = {
+                'payload': json.dumps(data, separators=(',', ':'))
+            }
+
+            response = client.post(
+                'https://api.bilibili.com/x/internal/gaia-gateway/ExClimbWuzhi',
+                cookies=cookies,
+                json=json_data,
+            )
+
+            self.dynamic_cookie.clear()
+            self.dynamic_cookie.update(cookies)
+
     async def init_dynamic_info(self, uid: str) -> Tuple[str, str, int]:
         """
         @description  :
         根据uid查询动态主信息
         ---------
         @param  :
         uid: 用户的uid
         -------
         @Returns  :
         返回一个元组
         [动态主名字，置顶动态id, 最新动态的时间戳]
         -------
         """
-        
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
+
+        async with httpx.AsyncClient(headers=self.headers) as client:
             try:
-                await client.get(self.API["get_bili_cookie"])
-                response1 = await client.get(url=self.API["get_user_info_by_uid"].format(uid))
+                response1 = await client.get(url=self.API["get_user_info_by_uid"], params=self.wbi_sign({"mid": uid}))
             except Exception as e:
                 raise BiliConnectionError(4, uid, e.args[0])
 
             if response1.status_code != 200:
                 raise  BiliStatusCodeError(4, uid, response1.status_code)
     
             response1 = response1.json()
             if response1["code"] == -404:
-                raise BiliAPI404Error()
+                raise BiliAPI404Error() 
             elif response1["code"] != 0:
                 raise BiliAPIRetCodeError(3, uid, response1["code"], response1["message"])
             
             user_name = response1["data"]["name"]
 
             try:
-                response2 = await client.get(url=self.API["get_dynamic_list_by_uid"].format(uid))
+                response2 = await client.get(
+                    url=self.API["get_dynamic_list_by_uid"],
+                    params={
+                        "host_mid": uid,
+                        "timezone_offset": -480
+                    },
+                    cookies=self.dynamic_cookie,
+                )
             except Exception as e:
                 raise BiliConnectionError(4, uid, e.args[0])
 
             if response2.status_code != 200:
                 raise  BiliStatusCodeError(4, uid, response2.status_code)
     
             response2 = response2.json()
@@ -552,41 +665,46 @@
             
             latest_timestamp = news_list[1]["modules"]["module_author"]["pub_ts"]
             return (user_name, top_news_id, latest_timestamp)
         else:
             latest_timestamp = news_list[0]["modules"]["module_author"]["pub_ts"]
             return (user_name, "", latest_timestamp)
 
-    async def get_latest_dynamic(self, uid: str, pin_news_id: str, latest_timestamp: int) -> Tuple[bool, bool, str, List[Dict]]:
+    async def get_latest_dynamic(self, client: httpx.AsyncClient, uid: str, pin_news_id: str, latest_timestamp: int) -> Tuple[bool, bool, str, List[Dict]]:
         '''根据uid获取最新的动态
 
         Args:
             uid (str): 查询的uid
             pin_news_id (str): 数据库中记录置顶动态的id,无则返为""
             latest_timestamp (int): 数据库中记录最新动态的时间戳
 
         Returns:
             Tuple[bool, bool, str, Dict]: 
             bool - 置顶动态是否更新
             bool - 是否有更新的动态
             str - 置顶动态id
             List[Dict] - 更新的动态内容
         ''' 
-        async with httpx.AsyncClient(headers=self.__request_header__()) as client:
-            try:
-                await client.get(url=self.API["get_bili_cookie"])
-                response = await client.get(url=self.API["get_dynamic_list_by_uid"].format(uid))
-            except Exception as e:
-                raise BiliConnectionError(4, f"uid:{uid}", e.args[0])
+        try:
+            response = await client.get(
+                url=self.API["get_dynamic_list_by_uid"],
+                params={
+                    "host_mid": uid,
+                    "timezone_offset": -480
+                },
+                cookies=self.dynamic_cookie,
+            )
+        except Exception as e:
+            raise BiliConnectionError(4, f"uid:{uid}", e.args[0])
 
-            if response.status_code != 200:
-                raise BiliStatusCodeError(4, f"uid:{uid}", response.status_code)
-            response = response.json()
-            if response["code"] != 0:
-                raise BiliAPIRetCodeError(3, uid, response["code"], response["message"])
+        if response.status_code != 200:
+            raise BiliStatusCodeError(4, f"uid:{uid}", response.status_code)
+        response = response.json()
+        if response["code"] != 0:
+            raise BiliAPIRetCodeError(3, uid, response["code"], response["message"])
             
         news_list: List = response["data"]["items"]
 
         # 如果动态列表长度为0则直接返回
         if len(news_list) == 0:
             return (False, False, "", [])
         
@@ -728,22 +846,22 @@
 
         Args:
             url (str): 目标网站
 
         Returns:
             httpx.Response: 返回响应
         '''
-        with httpx.Client(headers=self.__request_header__()) as client:
+        with httpx.Client(headers=self.headers) as client:
             try:
                 response = client.get(url=url)
             except Exception as e:
                 logger.debug(f'出现网络连接错误:{e}')
                 return None
             else:
                 return response
                 
-            
-
-
-
     
-bili_client = BiliClient()
+bili_client = BiliClient()
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
+scheduler.add_job(bili_client.update_dynamic_cookie, "interval", hours=12, id="update_dynamic_cookie", misfire_grace_time=90)
+scheduler.add_job(bili_client.get_img_key_and_sub_key, "interval", minutes=10, id="update_img_sub_key",misfire_grace_time=90)
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,27 @@
     检查关注动态主是否更新新视频，如果更新则通知用户并更新缓存和数据库
     ---------
     @param  :
     -------
     @Returns  :
     -------
     """
-    logger.debug("running check_dynamic_update")
     schedBot = nonebot.get_bot()
     check_dynamic_list = bili_task_manager.get_dynamic_check_update_list()
     #logger.debug(f'{__PLUGIN_NAME}check_dynamic_list = {check_dynamic_list}')
-    
-    results = await asyncio.gather(
-        *[bili_client.get_latest_dynamic(
-            uid, 
-            bili_task_manager.dynamic_list[uid]["pin_id_str"],
-            bili_task_manager.dynamic_list[uid]["latest_timestamp"]
-        ) for uid in check_dynamic_list],
-        return_exceptions=True
-    )
+    async with httpx.AsyncClient(headers={"User-Agent":"Mozilla/5.0"}) as client:
+        results = await asyncio.gather(
+            *[bili_client.get_latest_dynamic(
+                client,
+                uid, 
+                bili_task_manager.dynamic_list[uid]["pin_id_str"],
+                bili_task_manager.dynamic_list[uid]["latest_timestamp"]
+            ) for uid in check_dynamic_list],
+            return_exceptions=True
+        )
     
     for i in range(len(check_dynamic_list)):
         if isinstance(results[i], tuple):
             uid = check_dynamic_list[i]
             u_name = bili_task_manager.dynamic_list[uid]["u_name"]
             if results[i][0] is True:
                 # 修改缓存中的置顶动态信息
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_task.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/bili_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         self.user_follower_list = dict()
         self.group_follower_list = dict()
     
         self.__up_update_check_ptr__ = 0
         self.__dynamic_update_check_ptr__ = 0
 
-        self.__update_check_len__ = 8
+        self.__update_check_len__ = 5
 
         self.__init_from_database__()
         
 
     def __init_from_database__(self):
         '''从数据库中进行初始化
         '''
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/db.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,23 @@
                 id INTERGER PRIMARY KEY,
                 up_uid VARCHAR(20) NOT NULL,
                 user_id VARCHAR(20),
                 group_id VARCHAR(20)
             )
             ''')
 
+        # 创建wbi参数记录表
+        cur.execute('''CREATE TABLE IF NOT EXISTS wbi_record
+            (
+                date INTERGER NOT NULL,
+                img_key VARCHAR(32) NOT NULL,
+                sub_key VARCHAR(32) NOT NULL
+            )
+            ''')
+
         # 创建索引
         cur.execute("CREATE INDEX IF NOT EXISTS up_index ON up_follower (up_uid)")
         cur.execute("CREATE INDEX IF NOT EXISTS up_user_index ON up_follower (user_id)")
         cur.execute("CREATE INDEX IF NOT EXISTS up_group_index ON up_follower (group_id)")
 
         # 创建关注主播表
         cur.execute('''CREATE TABLE IF NOT EXISTS liver_follower
@@ -539,9 +548,46 @@
             cur.execute("SELECT rowid, season_id, user_id, group_id FROM telegram_follower")
         except Exception as e:
             ##logger.error(f'查询群组关注时发生错误:\n{e}')
             raise BiliDatebaseError(f"数据库查询群组关注时发生错误:{e.args[0]}")
         else:
             temp = cur.fetchall()
             return temp
+    
+    def get_wbi_param(self) -> Tuple[str, str, str]:
+        '''获取数据库中的wbi参数
+
+        Returns:
+            Tuple[str, str, str]: (date, img_key, sub_key)
+        '''
+        cur = self.conn.cursor()
+        try:
+            cur.execute("SELECT date, img_key, sub_key FROM wbi_record")
+        except Exception as e:
+            raise BiliDatebaseError(f"数据库获取wbi参数时发生错误:{e.args[0]}")
+        else:
+            temp = cur.fetchone()
+            return temp
+
+    def set_wbi_param(self, date: int, img_key: str, sub_key: str) -> bool:
+        '''设置新的wbi参数
+
+        Args:
+            date (int): 日期
+            img_key (str): img_key
+            sub_key (str): sub_key
+        '''
+        cur = self.conn.cursor()
+        try:
+            cur.execute("TRUNCATE wbi_record")
+            cur.execute("INSERT INTO wbi_record VALUES (?, ?, ?)", (date, img_key, sub_key))
+        except Exception as e:
+            cur.close()
+            self.conn.rollback()
+            raise BiliDatebaseError(f"数据库设置wbi参数时发生错误:{e.args[0]}")
+        else:
+            cur.close()
+            self.conn.commit()
+            return True
+
         
 bili_database = BiliDatabase()
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/exception.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/rule.py` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/bili_src/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/help.json` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot/file/source/help.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/PKG-INFO` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilibilibot
-Version: 2.3.2
+Version: 2.3.3
 Summary: 基于Nonebot的bilibili通知插件，可将up主，主播以及番剧的更新/直播动态推送到QQ
 Home-page: https://github.com/TDK1969/nonebot_plugin_bilibilibot
 Author: TDK
 Author-email: tdk1969@foxmail.com
 License: GNU
 Keywords: nonebot
 Platform: UNKNOWN
```

### Comparing `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt` & `nonebot_plugin_bilibilibot-2.3.3/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.2/setup.py` & `nonebot_plugin_bilibilibot-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import sys
 import os
 
 setup(
     name="nonebot_plugin_bilibilibot",
-    version="2.3.2",
+    version="2.3.3",
     author="TDK",
     author_email="tdk1969@foxmail.com",
     description="基于Nonebot的bilibili通知插件，可将up主，主播以及番剧的更新/直播动态推送到QQ",
     long_description=open("README.rst", "r").read(),
     include_package_data=True,
     license="GNU",
     url="https://github.com/TDK1969/nonebot_plugin_bilibilibot",
```

