# Comparing `tmp/dicergirl-3.0.8.tar.gz` & `tmp/dicergirl-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.8.tar", last modified: Mon Jul 31 09:40:52 2023, max compression
+gzip compressed data, was "dicergirl-3.0.9.tar", last modified: Mon Jul 31 09:59:35 2023, max compression
```

## Comparing `dicergirl-3.0.8.tar` & `dicergirl-3.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.069190 dicergirl-3.0.8/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.8/LICENSE
--rw-rw-rw-   0        0        0     9363 2023-07-31 09:40:52.069190 dicergirl-3.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.015192 dicergirl-3.0.8/dicergirl/
--rw-rw-rw-   0        0        0    18920 2023-07-31 05:49:32.000000 dicergirl-3.0.8/dicergirl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.053189 dicergirl-3.0.8/dicergirl/coc/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:17:05.000000 dicergirl-3.0.8/dicergirl/coc/__init__.py
--rw-rw-rw-   0        0        0     4362 2023-07-31 05:29:50.000000 dicergirl-3.0.8/dicergirl/coc/coccards.py
--rw-rw-rw-   0        0        0     9165 2023-07-31 08:22:11.000000 dicergirl-3.0.8/dicergirl/coc/cocutils.py
--rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.0.8/dicergirl/coc/investigator.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.057191 dicergirl-3.0.8/dicergirl/dnd/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.0.8/dicergirl/dnd/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-07-31 09:32:44.000000 dicergirl-3.0.8/dicergirl/dnd/adventurer.py
--rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.0.8/dicergirl/dnd/dndcards.py
--rw-rw-rw-   0        0        0     4024 2023-07-31 09:35:10.000000 dicergirl-3.0.8/dicergirl/dnd/dndutils.py
--rw-rw-rw-   0        0        0    17465 2023-07-31 09:30:37.000000 dicergirl-3.0.8/dicergirl/main.py
--rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.0.8/dicergirl/run.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.060190 dicergirl-3.0.8/dicergirl/scp/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:30:31.000000 dicergirl-3.0.8/dicergirl/scp/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.0.8/dicergirl/scp/agent.py
--rw-rw-rw-   0        0        0     2824 2023-07-31 06:08:08.000000 dicergirl-3.0.8/dicergirl/scp/scpcards.py
--rw-rw-rw-   0        0        0     5188 2023-07-31 09:33:55.000000 dicergirl-3.0.8/dicergirl/scp/scputils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.068189 dicergirl-3.0.8/dicergirl/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.8/dicergirl/utils/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.8/dicergirl/utils/chat.py
--rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.8/dicergirl/utils/decorators.py
--rw-rw-rw-   0        0        0     8656 2023-07-31 09:37:09.000000 dicergirl-3.0.8/dicergirl/utils/dicer.py
--rw-rw-rw-   0        0        0    22438 2023-07-31 08:50:24.000000 dicergirl-3.0.8/dicergirl/utils/handlers.py
--rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.0.8/dicergirl/utils/messages.py
--rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.8/dicergirl/utils/settings.py
--rw-rw-rw-   0        0        0     5839 2023-07-31 09:40:17.000000 dicergirl-3.0.8/dicergirl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.049232 dicergirl-3.0.8/dicergirl.egg-info/
--rw-rw-rw-   0        0        0     9363 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 09:40:52.070191 dicergirl-3.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-07-31 07:36:19.000000 dicergirl-3.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.772390 dicergirl-3.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9363 2023-07-31 09:59:35.771356 dicergirl-3.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.727379 dicergirl-3.0.9/dicergirl/
+-rw-rw-rw-   0        0        0    20079 2023-07-31 09:57:16.000000 dicergirl-3.0.9/dicergirl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.759439 dicergirl-3.0.9/dicergirl/coc/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:17:05.000000 dicergirl-3.0.9/dicergirl/coc/__init__.py
+-rw-rw-rw-   0        0        0     4362 2023-07-31 05:29:50.000000 dicergirl-3.0.9/dicergirl/coc/coccards.py
+-rw-rw-rw-   0        0        0     9165 2023-07-31 08:22:11.000000 dicergirl-3.0.9/dicergirl/coc/cocutils.py
+-rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.0.9/dicergirl/coc/investigator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.761910 dicergirl-3.0.9/dicergirl/dnd/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.0.9/dicergirl/dnd/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-07-31 09:32:44.000000 dicergirl-3.0.9/dicergirl/dnd/adventurer.py
+-rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.0.9/dicergirl/dnd/dndcards.py
+-rw-rw-rw-   0        0        0     4024 2023-07-31 09:35:10.000000 dicergirl-3.0.9/dicergirl/dnd/dndutils.py
+-rw-rw-rw-   0        0        0    17465 2023-07-31 09:30:37.000000 dicergirl-3.0.9/dicergirl/main.py
+-rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.0.9/dicergirl/run.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.764594 dicergirl-3.0.9/dicergirl/scp/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:31.000000 dicergirl-3.0.9/dicergirl/scp/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.0.9/dicergirl/scp/agent.py
+-rw-rw-rw-   0        0        0     2824 2023-07-31 06:08:08.000000 dicergirl-3.0.9/dicergirl/scp/scpcards.py
+-rw-rw-rw-   0        0        0     5188 2023-07-31 09:33:55.000000 dicergirl-3.0.9/dicergirl/scp/scputils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.770191 dicergirl-3.0.9/dicergirl/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.9/dicergirl/utils/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.9/dicergirl/utils/chat.py
+-rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.9/dicergirl/utils/decorators.py
+-rw-rw-rw-   0        0        0     8656 2023-07-31 09:37:09.000000 dicergirl-3.0.9/dicergirl/utils/dicer.py
+-rw-rw-rw-   0        0        0    22438 2023-07-31 08:50:24.000000 dicergirl-3.0.9/dicergirl/utils/handlers.py
+-rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.0.9/dicergirl/utils/messages.py
+-rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.9/dicergirl/utils/settings.py
+-rw-rw-rw-   0        0        0     5839 2023-07-31 09:43:51.000000 dicergirl-3.0.9/dicergirl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.755176 dicergirl-3.0.9/dicergirl.egg-info/
+-rw-rw-rw-   0        0        0     9363 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:59:35.772390 dicergirl-3.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-07-31 07:36:19.000000 dicergirl-3.0.9/setup.py
```

### Comparing `dicergirl-3.0.8/LICENSE` & `dicergirl-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/PKG-INFO` & `dicergirl-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.8
+Version: 3.0.9
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.8/README.md` & `dicergirl-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/__init__.py` & `dicergirl-3.0.9/dicergirl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,29 @@
 except ValueError:
     set_package("qqguild")
 
 package = get_package()
 
 if package == "nonebot2":
     from .coc.investigator import Investigator
-    from .scp.agent import Agent
-    from .coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
     from .coc.coccards import cards, cache_cards, sa_handler
+    from .coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
+
+    from .scp.agent import Agent
     from .scp.scpcards import scp_cards, scp_cache_cards
     from .scp.scputils import sra, scp_dam, at as sat
-    from .utils.messages import help_message
-    from .utils.utils import logger as _log, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, version
-    from .utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, set_handler, show_handler, del_handler
+
+    from .dnd.adventurer import Adventurer
+    from .dnd.dndcards import dnd_cards, dnd_cache_cards
+    from .dnd.dndutils import dra
+
+    from .utils.decorators import Commands
+    from .utils.messages import help_message, version
+    from .utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config, modes
+    from .utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, coc_set_handler, coc_show_handler, coc_del_handler, dnd_set_handler, dnd_show_handler, dnd_del_handler
     from .utils.chat import chat
 
     from nonebot.rule import Rule
     from nonebot.matcher import Matcher
     from nonebot.plugin import on_startswith
     from nonebot.adapters import Bot as Bot
     from nonebot.adapters.onebot.v11 import Bot as V11Bot
@@ -45,14 +52,16 @@
         from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
 
     testcommand = on_startswith(".test", priority=2, block=True)
     debugcommand = on_startswith(".debug", priority=2, block=True)
     superusercommand = on_startswith(".su", priority=2, block=True)# | on_startswith(".sudo", priority=2, block=True)
     botcommand = on_startswith(".bot", priority=1, block=True)
     coccommand = on_startswith(".coc", priority=1, block=True)
+    scpcommand = on_startswith(".scp", priority=1, block=True)
+    dndcommand = on_startswith(".dnd", priority=1, block=True)
     showcommand = on_startswith(".show", priority=2, block=True)# | on_startswith(".display", priority=2, block=True)
     setcommand = on_startswith(".set", priority=2, block=True)
     helpcommand = on_startswith(".help", priority=2, block=True)# | on_startswith(".h", priority=2, block=True)
     modecommand = on_startswith(".mode", priority=2, block=True)# | on_startswith(".m", priority=2, block=True)
     stcommand = on_startswith(".sht", priority=2, block=True)
     attackcommand = on_startswith(".at", priority=2, block=True)# | on_startswith(".attack", priority=2, block=True)
     damcommand = on_startswith(".dam", priority=2, block=True)# | on_startswith(".damage", priority=2, block=True)
@@ -62,16 +71,14 @@
     rhacommand = on_startswith(".rha", priority=1, block=True)
     rcommand = on_startswith(".r", priority=3, block=True)
     ticommand = on_startswith(".ti", priority=2, block=True)
     licommand = on_startswith(".li", priority=2, block=True)
     sccommand = on_startswith(".sc", priority=2, block=True)
     sacommand = on_startswith(".sa", priority=2, block=True)
     delcommand = on_startswith(".del", priority=2, block=True)# | on_startswith(".delete", priority=2, block=True)
-    scpcommand = on_startswith(".scp", priority=1, block=True)
-    scpracommand = on_startswith(".sra", priority=2, block=True)
     chatcommand = on_startswith(".chat", priority=2, block=True)
     versioncommand = on_startswith(".version", priority=2, block=True)# | on_startswith(".v", priority=2, block=True)
 
     @driver.on_startup
     async def _():
         global DEBUG
         logger.info("欧若可骰娘初始化中...")
@@ -93,16 +100,16 @@
         return Rule(_is_group_message)
 
     @testcommand.handle()
     async def testhandler(matcher: Matcher, event: GroupMessageEvent):
         if not is_super_user(event):
             await matcher.send("[Oracle] 权限不足, 拒绝执行指令.")
             return
-        _log.info("发送消息:" + str(event.get_message()))
-        _log.info(event.get_message().__repr__())
+        logger.info("发送消息:" + str(event.get_message()))
+        logger.info(event.get_message().__repr__())
         msg = format_msg(event.get_message())
         if not msg:
             msg = "[]"
         if msg[-1] == "markdown":
             mp = ""
             await matcher.send(group_id=event.group_id, message=mp)
             return
@@ -115,15 +122,15 @@
         global DEBUG
         args = format_msg(event.get_message(), begin=".debug")
         if not is_super_user(event):
             await matcher.send("[Oracle] 权限不足, 拒绝执行指令.")
             return
 
         if args:
-            _log.debug(args)
+            logger.debug(args)
             if args[0] == "off":
                 DEBUG = False
                 logging.getLogger().setLevel(logging.INFO)
                 logger.remove()
                 logger.add(
                     sys.stdout,
                     level = "INFO"
@@ -170,15 +177,15 @@
                 return
 
         if is_super_user(event):
             await matcher.send("[Oracle] 你已经是超级管理员.")
             return
 
         if not args:
-            _log.critical(f"超级令牌: {su_uuid}")
+            logger.critical(f"超级令牌: {su_uuid}")
             await matcher.send("[Oracle] 启动超级管理员鉴权, 鉴权令牌已在控制终端展示.")
         else:
             if not args == su_uuid:
                 await matcher.send("[Oracle] 鉴权失败!")
             else:
                 add_super_user(event)
                 await matcher.send("[Oracle] 你取得了管理员权限.")
@@ -203,15 +210,15 @@
         else:
             await matcher.send(help_message("bot"))
 
     @coccommand.handle()
     async def cochandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=".coc")
         if len(args) > 1:
-            _log.info("指令错误, 驳回.")
+            logger.info("指令错误, 驳回.")
             await matcher.send("[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
             return False
 
         try:
             if len(args) == 0:
                 raise ValueError
             args = int(args[0])
@@ -222,71 +229,115 @@
         inv = Investigator()
         await matcher.send(inv.age_change(args))
 
         if 15 <= args and args < 90:
             cache_cards.update(event, inv.__dict__, save=False)
             await matcher.send(str(inv.output()))
 
+    @scpcommand.handle()
+    async def scp_handler(matcher: Matcher, event: GroupMessageEvent):
+        args = format_msg(event.get_message(), begin=".scp")
+        if len(args) > 1:
+            logger.info("指令错误, 驳回.")
+            await matcher.send("[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
+            return
+
+        try:
+            if len(args) == 0:
+                raise ValueError
+            args = int(args[0])
+        except ValueError:
+            await matcher.send(f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
+            args = 20
+
+        agt = Agent()
+        agt.age_check(args)
+        agt.init()
+
+        if 15 <= args and args < 90:
+            scp_cache_cards.update(event, agt.__dict__, save=False)
+            await matcher.send(str(agt.output()))
+
+    @dndcommand.handle()
+    async def dnd_handler(matcher: Matcher, event: GroupMessageEvent):
+        args = format_msg(event.get_message(), begin=".dnd")
+        if len(args) > 1:
+            logger.info("指令错误, 驳回.")
+            await matcher.send("[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
+            return True
+
+        try:
+            if len(args) == 0:
+                raise ValueError
+            args = int(args[0])
+        except ValueError:
+            await matcher.send(f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
+            args = 20
+
+        adv = Adventurer()
+        adv.age_check(args)
+        adv.init()
+        
+        if adv.int[0] <= 8:
+            await matcher.send("[Orcale] 很遗憾, 检定新的冒险者智力不足, 弱智是不允许成为冒险者的, 请重新进行车卡检定.")
+            return True
+
+        if 15 <= args and args < 90:
+            dnd_cache_cards.update(event, adv.__dict__, save=False)
+            await matcher.send(str(adv.output()))
+        return True
+
     @showcommand.handle()
     async def showhandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=(".show", ".display"))
         if not args:
-            if mode == "scp":
-                sh = scp_show_handler(event, args)
-            elif mode == "coc":
-                sh = show_handler(event, args)
+            if mode in modes:
+                try:
+                    sh = eval(f"{mode}_show_handler(event, args)")
+                except:
+                    sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
             else:
                 await matcher.send("未知的跑团模式.")
-                return
+                return True
 
             for msg in sh:
                 await matcher.send(str(msg))
-            return
+            return True
 
-        if args[0] in ["s", "scp"]:
-            args.remove(args[0])
-            sh = scp_show_handler(event, args)
-        elif args[0] in ["c", "coc"]:
+        if args[0] in modes:
             args.remove(args[0])
-            sh = show_handler(event, args)
+            sh = eval(f"{args[0]}_show_handler(event, args)")
         else:
-            if mode == "scp":
-                sh = scp_show_handler(event, args)
-            elif mode == "coc":
-                sh = show_handler(event, args)
-            else:
-                await matcher.send("未知的跑团模式.")
-                return
+            try:
+                sh = eval(f"{mode}_show_handler(event, args)")
+            except:
+                sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
 
         for msg in sh:
             await matcher.send(str(msg))
-
+        return
 
     @setcommand.handle()
     async def sethandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=".set")
         if not args:
             args.append(mode)
 
-        if args[0] in ["s", "scp"]:
-            args.remove(args[0])
-            sh = scp_set_handler(event, args)
-        elif args[0] in ["c", "coc"]:
-            args.remove(args[0])
-            sh = set_handler(event, args)
+        if args[0] in modes:
+            try:
+                now = args[0]
+                args.remove(args[0])
+                sh = eval(f"{now}_set_handler(event, args)")
+            except:
+                sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
         else:
-            if mode == "scp":
-                sh = scp_set_handler(event, args)
-            elif mode == "coc":
-                sh = set_handler(event, args)
-            else:
-                await matcher.send("未知的跑团模式.")
-                return
+            sh = [f"[Oracle] 错误: 未知的跑团模式."]
 
         await matcher.send(sh)
+        return
 
 
     @helpcommand.handle()
     async def rdhelphandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(str(event.get_message()), begin=(".help", ".h"))
         if args:
             arg = args[0]
@@ -353,15 +404,22 @@
         args = format_str(event.get_message(), begin=".en")
         await matcher.send(en(args, event.get_message()))
 
 
     @racommand.handle()
     async def rahandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=".ra")
-        await matcher.send(ra(args, event))
+        if mode in ["coc", "scp", "dnd"]:
+            if mode == "scp":
+                await matcher.send(sra(args, event))
+            elif mode == "coc":
+                await matcher.send(ra(args, event))
+            elif mode == "dnd":
+                await matcher.send(dra(args, event))
+        return
 
     @rhcommand.handle()
     async def rhhandler(bot: Bot, matcher: Matcher, event: GroupMessageEvent):
         args = format_str(event.get_message(), begin=".rh")
         await matcher.send("[Oracle] 暗骰: 命运的骰子在滚动.")
         await bot.send_private_msg(user_id=event.get_user_id(), message=rd0(args))
 
@@ -422,53 +480,20 @@
     async def sahandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_str(event.get_message(), begin=".sa")
         await matcher.send(sa_handler(event, args))
 
 
     @delcommand.handle()
     async def delhandler(matcher: Matcher, event: GroupMessageEvent):
-        args = format_str(event.get_message(), begin=(".del", ".delete"))
-        if mode == "coc":
-            for msg in del_handler(event, args):
-                await matcher.send(msg)
-        elif mode == "scp":
-            for msg in scp_del_handler(event, args):
+        args = format_str(event, begin=(".del", ".delete"))
+        if mode in modes:
+            for msg in eval(f"{mode}_del_handler(event, args)"):
                 await matcher.send(msg)
         return
 
-    @scpcommand.handle()
-    async def scp_handler(matcher: Matcher, event: GroupMessageEvent):
-        args = format_msg(event.get_message(), begin=".scp")
-        if len(args) > 1:
-            _log.info("指令错误, 驳回.")
-            await matcher.send("[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
-            return
-
-        try:
-            if len(args) == 0:
-                raise ValueError
-            args = int(args[0])
-        except ValueError:
-            await matcher.send(f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
-            args = 20
-
-        agt = Agent()
-        agt.age_check(args)
-        agt.init()
-
-        if 15 <= args and args < 90:
-            scp_cache_cards.update(event, agt.__dict__, save=False)
-            await matcher.send(str(agt.output()))
-
-    @scpracommand.handle()
-    async def scp_rahandler(matcher: Matcher, event: GroupMessageEvent):
-        args = format_msg(event.get_message(), begin=".sra")
-        await matcher.send(sra(args, event))
-
-
     @chatcommand.handle()
     async def chathandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_str(event.get_message(), begin=".chat")
         if not args:
             await matcher.send("[Oracle] 空消息是不被允许的.")
             return
         await matcher.send(chat(args))
```

### Comparing `dicergirl-3.0.8/dicergirl/coc/coccards.py` & `dicergirl-3.0.9/dicergirl/coc/coccards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/coc/cocutils.py` & `dicergirl-3.0.9/dicergirl/coc/cocutils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/coc/investigator.py` & `dicergirl-3.0.9/dicergirl/coc/investigator.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/dnd/adventurer.py` & `dicergirl-3.0.9/dicergirl/dnd/adventurer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/dnd/dndcards.py` & `dicergirl-3.0.9/dicergirl/dnd/dndcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/dnd/dndutils.py` & `dicergirl-3.0.9/dicergirl/dnd/dndutils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/main.py` & `dicergirl-3.0.9/dicergirl/main.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/run.py` & `dicergirl-3.0.9/dicergirl/run.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/scp/agent.py` & `dicergirl-3.0.9/dicergirl/scp/agent.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/scp/scpcards.py` & `dicergirl-3.0.9/dicergirl/scp/scpcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/scp/scputils.py` & `dicergirl-3.0.9/dicergirl/scp/scputils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/chat.py` & `dicergirl-3.0.9/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/decorators.py` & `dicergirl-3.0.9/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/dicer.py` & `dicergirl-3.0.9/dicergirl/utils/dicer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/handlers.py` & `dicergirl-3.0.9/dicergirl/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/messages.py` & `dicergirl-3.0.9/dicergirl/utils/messages.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/settings.py` & `dicergirl-3.0.9/dicergirl/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/dicergirl/utils/utils.py` & `dicergirl-3.0.9/dicergirl/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     try:
         from botpy.message import Message
     except ModuleNotFoundError:
         logger.warning("未找到依赖`qq-botpy`, 请检查你的配置.")
         class Message:
             pass
 
-version = "3.0.8"
+version = "3.0.9"
 current_dir = Path(__file__).resolve().parent
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
 _dnd_cachepath = data_dir / "dnd_cards.json"
 _super_user = data_dir / "super_user.json"
```

### Comparing `dicergirl-3.0.8/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.0.9/dicergirl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.8
+Version: 3.0.9
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.8/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.0.9/dicergirl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.8/setup.py` & `dicergirl-3.0.9/setup.py`

 * *Files identical despite different names*

