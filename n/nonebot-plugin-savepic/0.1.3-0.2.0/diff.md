# Comparing `tmp/nonebot_plugin_savepic-0.1.3.tar.gz` & `tmp/nonebot_plugin_savepic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_savepic-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_savepic-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_savepic-0.1.3.tar` & `nonebot_plugin_savepic-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1060 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/LICENSE
--rw-r--r--   0        0        0     1984 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/README.md
--rw-r--r--   0        0        0     5684 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/__init__.py
--rw-r--r--   0        0        0      181 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/config.py
--rw-r--r--   0        0        0      846 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/migrations/1a654e02179b_.py
--rw-r--r--   0        0        0      581 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/model.py
--rw-r--r--   0        0        0     4948 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/pic_sql.py
--rw-r--r--   0        0        0      971 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/rule.py
--rw-r--r--   0        0        0      553 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-08-03 04:29:59.872363 nonebot_plugin_savepic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1984 2023-08-03 04:29:59.872363 nonebot_plugin_savepic-0.2.0/README.md
+-rw-r--r--   0        0        0     6304 2023-08-03 04:29:59.872363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/__init__.py
+-rw-r--r--   0        0        0      206 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/config.py
+-rw-r--r--   0        0        0     1052 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/ext_listener.py
+-rw-r--r--   0        0        0      846 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/migrations/1a654e02179b_.py
+-rw-r--r--   0        0        0      744 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/model.py
+-rw-r--r--   0        0        0     6653 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/pic_sql.py
+-rw-r--r--   0        0        0     1548 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/picture.py
+-rw-r--r--   0        0        0      920 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/rule.py
+-rw-r--r--   0        0        0      642 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_savepic-0.1.3/LICENSE` & `nonebot_plugin_savepic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.3/README.md` & `nonebot_plugin_savepic-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/__init__.py` & `nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,190 @@
 from nonebot import require
 from nonebot import get_driver
-
-require("nonebot_plugin_datastore")
-
-from nonebot import on_command, on_message
+from nonebot import on_command
 from nonebot.params import CommandArg, Arg
 from nonebot.adapters.onebot.v11.message import Message as V11Msg
 from nonebot.adapters.onebot.v11.message import MessageSegment as V11Seg
-from nonebot.adapters.onebot.v11 import Bot
-from nonebot.adapters.onebot.v11.event import MessageEvent
+from nonebot.internal.adapter.bot import Bot
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
-
+from nonebot.plugin import PluginMetadata
 from asyncpg.exceptions import InvalidRegularExpressionError
+from arclet.alconna import Alconna, Option, Args, CommandMeta, append
+import os
+
+require("nonebot_plugin_datastore")
 
 from .config import Config
 from .pic_sql import savepic, rename, delete, write_pic, randpic, load_pic, select_pic
 from .rule import PIC_AMDIN
+from .ext_listener import pic_listen
+from .picture import p_hash
 
-from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="Savepic",
     description="表情包保存",
     usage="""用法:
 /savepic <文件名> <图片>
 /savepic -g <文件名> <全局图片>
 /savepic -d <文件名> 删除图图片
 /savepic -m <原文件名> <新文件名> 重命名图片
 /randpic <关键词> 随机图片
 <文件名> 发送图片""",
     config=Config,
     homepage="https://github.com/Yan-Zero/nonebot-plugin-savepic",
     type="application",
-    supported_adapters=[
-        '~onebot.v11'
-    ]
+    supported_adapters=["~onebot.v11"],
 )
 
 INVALID_FILENAME_CHARACTERS = r'\/:*?"<>|'
 
-global_config = get_driver().config
-p_config = Config.parse_obj(global_config)
+p_config = Config.parse_obj(get_driver().config)
 
 rpic = on_command("randpic", aliases={"随机图"}, priority=5)
+
+
 @rpic.handle()
 async def _(bot: Bot, event, args: V11Msg = CommandArg()):
     reg = args.extract_plain_text().strip()
-    group_id = 'globe' if not isinstance(event, GroupMessageEvent) else f"qq_group:{event.group_id}"
+    group_id = (
+        "globe"
+        if not isinstance(event, GroupMessageEvent)
+        else f"qq_group:{event.group_id}"
+    )
     try:
         pic = await randpic(reg, group_id)
         if pic:
             file_ = await load_pic(pic.url)
             await bot.send(event, V11Msg([pic.name + "\n", V11Seg.image(file=file_)]))
     except InvalidRegularExpressionError:
-        await rpic.finish('正则表达式错误')
+        await rpic.finish("正则表达式错误")
     except Exception as ex:
         await rpic.finish(str(ex))
 
+
 spic = on_command("savepic", aliases={"存图"}, priority=5)
+a_spic = Alconna(
+    "/savepic",
+    Option("-d", help_text="删除图片"),
+    Option("-g", help_text="全局"),
+    Option("-ac", help_text="允许相似碰撞"),
+    Args.filename[str],
+    meta=CommandMeta(description="保存图片，默认保存到本群"),
+)
+
+
 @spic.handle()
-async def _(bot: Bot, matcher: Matcher, event: GroupMessageEvent, state: T_State, args: V11Msg = CommandArg()):
-    if not args:
-        await spic.finish('''用法:
-/savepic <文件名> <图片>
-/savepic -g <文件名> <全局图片>
-/savepic -d <文件名> 删除图图片
-/savepic -m <原文件名> <新文件名> 重命名图片''')
-    params = args.extract_plain_text().strip().split()
-    state['savepiv_group'] = 'globe' if '-g' in params and await PIC_AMDIN(bot, event) else f"qq_group:{event.group_id}"
-    _d = '-d' in params
-    _m = '-m' in params
-    if _d:
-        params.remove('-d')
-    if _m:
-        params.remove('-m')
-    if '-g' in params:
-        params.remove('-g')
-
-    if not params:
-        await spic.finish("文件名？")
-    filename = params[0].strip()
+async def _(
+    bot: Bot,
+    matcher: Matcher,
+    event: GroupMessageEvent,
+    state: T_State,
+):
+    command = a_spic.parse(event.message.extract_plain_text())
+    if not command.matched:
+        await spic.finish(str(command.error_info) + "\n\n" + a_spic.get_help())
+
+    state["savepiv_group"] = "globe" if command.g else f"qq_group:{event.group_id}"
+    filename = command.filename
     for c in INVALID_FILENAME_CHARACTERS:
         filename = filename.replace(c, "-")
-    if not filename.endswith(('.jpg', '.png', '.gif')):
-        filename += '.jpg'
+    if not filename.endswith((".jpg", ".png", ".gif")):
+        filename += ".jpg"
+    state["savepiv_filename"] = filename
+    state["savepiv_ac"] = command.ac is not None
 
-    if _d:
+    if command.d:
         if not await PIC_AMDIN(bot, event):
-            await spic.finish('不支持选项 -d')
+            await spic.finish("不支持选项 -d")
         try:
-            await delete(filename, state['savepiv_group'])
+            await delete(filename, state["savepiv_group"])
         except Exception as ex:
             await spic.finish(str(ex))
-        await spic.finish('图片已删除')
+        await spic.finish("图片已删除")
 
-    if _m:
-        if not await PIC_AMDIN(bot, event):
-            await spic.finish('不支持选项 -m')
-        if len(params) <= 1:
-            await spic.finish("目标文件名？")
-        for c in INVALID_FILENAME_CHARACTERS:
-            params[1] = params[1].replace(c, "-")
-        if not params[1].endswith(('.jpg', '.png', '.gif')):
-            params[1] += '.jpg'
-
-        try:
-            await rename(filename, params[1],  f"qq_group:{event.group_id}", state['savepiv_group'])
-        except Exception as ex:
-            await spic.finish(str(ex))
-        await spic.finish('图片已重命名')
+    pic = await select_pic(filename, state["savepiv_group"])
+    if pic and pic.group == state["savepiv_group"]:
+        spic.finish("文件名已存在。")
 
-    pic = await select_pic(filename, state['savepiv_group'])
-    if pic and pic.group == state['savepiv_group']:
-        spic.finish("图片已存在。")
-    picture = args.get('image')
-    state['savepiv_filename'] = filename
+    picture = event.message.get("image")
     if not picture and event.reply:
-        picture = event.reply.message.get('image')
+        picture = event.reply.message.get("image")
     if picture:
-        matcher.set_arg('picture', picture)
+        matcher.set_arg("picture", picture)
 
-@spic.got('picture', "图呢？")
-async def _(bot: Bot, event: GroupMessageEvent, state: T_State, picture: V11Msg = Arg()):
-    picture = picture.get('image')
+
+@spic.got("picture", "图呢？")
+async def _(state: T_State, picture: V11Msg = Arg()):
+    picture = picture.get("image")
     if not picture:
-        await spic.finish('6，这也不是图啊')
+        await spic.finish("6，这也不是图啊")
+
     try:
-        dir = await write_pic(picture[0].data['url'], p_config.savepic_dir)
+        dir = await write_pic(picture[0].data["url"], p_config.savepic_dir)
     except Exception as ex:
-        await spic.finish("存图失败。" + '\n' + str(ex))
+        await spic.finish("存图失败。" + "\n" + str(ex))
     try:
-        await savepic(state['savepiv_filename'], dir, state['savepiv_group'])
+        await savepic(
+            state["savepiv_filename"],
+            dir,
+            p_hash(await load_pic(dir)),
+            state["savepiv_group"],
+            state["savepiv_ac"],
+        )
         await spic.send("保存成功")
     except Exception as ex:
+        os.remove(dir)
         await spic.finish(str(ex))
 
-async def endswith_pic(event: MessageEvent):
-    text = event.message.extract_plain_text().strip()
-    if ' ' in text:
-        return False
-    return text.endswith(('.jpg', '.png', '.gif'))
-
-pic_listen = on_message(rule=endswith_pic)
-@pic_listen.handle()
-async def _(bot: Bot, event: MessageEvent):
-    name = event.message.extract_plain_text().strip()
-    group_id = 'globe' if not isinstance(event, GroupMessageEvent) else f"qq_group:{event.group_id}"
+
+s_mvpic = on_command("mvpic", priority=5)
+a_mvpic = Alconna(
+    "/mvpic",
+    Option("-l", args=Args.filename[str], help_text="本地图片", action=append),
+    Option("-g", args=Args.filename[str], help_text="全局图片", action=append),
+    meta=CommandMeta(description="重命名图片，按照参数先后判断"),
+)
+
+
+@s_mvpic.handle()
+async def _(
+    bot: Bot,
+    event: GroupMessageEvent,
+):
+    if not await PIC_AMDIN(bot, event):
+        await spic.finish("不支持选项 -m")
+
+    cmd = a_mvpic.parse(event.message.extract_plain_text())
+    if not cmd.matched:
+        await s_mvpic.finish(str(cmd.error_info) + "\n\n" + a_mvpic.get_help())
+    options = cmd.options
+    if not options:
+        await s_mvpic.finish("文件名呢？" + "\n\n" + a_mvpic.get_help())
+
+    sg = "globe" if list(options.keys())[0] == "g" else f"qq_group:{event.group_id}"
+    if len(options["g" if sg == "globe" else "l"].args.get("filename", [])) >= 2:
+        dg = sg
+    else:
+        dg = "globe" if sg != "globe" else f"qq_group:{event.group_id}"
+    if ("g" if dg == "globe" else "l") not in options:
+        await s_mvpic.finish("至多只有一个文件名哦？" + "\n\n" + a_mvpic.get_help())
+
+    sname = options["g" if sg == "globe" else "l"].args["filename"][0]
+    dname = options["g" if dg == "globe" else "l"].args["filename"][
+        1 if sg == dg else 0
+    ]
+    for c in INVALID_FILENAME_CHARACTERS:
+        sname = sname.replace(c, "-")
+        dname = dname.replace(c, "-")
+    if not sname.endswith((".jpg", ".png", ".gif")):
+        sname += ".jpg"
+    if not dname.endswith((".jpg", ".png", ".gif")):
+        dname += ".jpg"
+
     try:
-        pic = await select_pic(name, group_id)
-        if pic:
-            file_ = await load_pic(pic.url)
-            await bot.send(event, V11Seg.image(file=file_))
+        await rename(sname, dname, sg, dg)
     except Exception as ex:
-        await rpic.finish(str(ex))
+        await spic.finish(str(ex))
+    await spic.finish("图片已重命名")
```

### Comparing `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/migrations/1a654e02179b_.py` & `nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/migrations/1a654e02179b_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/rule.py` & `nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 
 This module is used to define the permission of the bot.
 """
 
 import nonebot
 from nonebot.adapters import Bot, Event
-from nonebot_plugin_datastore import get_plugin_data
 from nonebot.internal.permission import Permission
+
 from .config import Config
 
 global_config = nonebot.get_driver().config
 plugin_config = Config.parse_obj(global_config)
 
 
 class Savepic_Admin(Permission):
@@ -28,8 +28,8 @@
         return (
             f"{bot.adapter.get_name().split(maxsplit=1)[0].lower()}:{user_id}"
             in plugin_config.savepic_admin
             or user_id in plugin_config.savepic_admin  # 兼容旧配置
         )
 
 
-PIC_AMDIN = Permission(Savepic_Admin())
+PIC_AMDIN = Permission(Savepic_Admin())
```

### Comparing `nonebot_plugin_savepic-0.1.3/pyproject.toml` & `nonebot_plugin_savepic-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "nonebot-plugin-savepic"
-version = "0.1.3"
+version = "0.2.0"
 description = "保存表情包（语录）与随机出图"
 authors = ["Yan <1964649083@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_savepic"}]
 homepage = "https://github.com/Yan-Zero/nonebot-plugin-savepic"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.10, <3.13"
 nonebot2 = "^2.0.1"
 nonebot-plugin-datastore = "^1.1.0"
 asyncpg = "^0.28.0"
 nonebot-adapter-onebot = "^2.2.3"
+arclet-alconna = "^1.7.14"
+numpy = "^1.25.2"
+scipy = "^1.11.1"
+pillow = "^10.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_savepic-0.1.3/PKG-INFO` & `nonebot_plugin_savepic-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-savepic
-Version: 0.1.3
+Version: 0.2.0
 Summary: 保存表情包（语录）与随机出图
 Home-page: https://github.com/Yan-Zero/nonebot-plugin-savepic
 License: MIT
 Author: Yan
 Author-email: 1964649083@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arclet-alconna (>=1.7.14,<2.0.0)
 Requires-Dist: asyncpg (>=0.28.0,<0.29.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot-plugin-datastore (>=1.1.0,<2.0.0)
 Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
+Requires-Dist: numpy (>=1.25.2,<2.0.0)
+Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.2.0 Summary:
 ä¿å­è¡¨æåï¼è¯­å½ï¼ä¸éæºåºå¾ Home-page: https://github.com/Yan-
 Zero/nonebot-plugin-savepic License: MIT Author: Yan Author-email:
-1964649083@qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+1964649083@qq.com Requires-Python: >=3.10,<3.13 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: asyncpg (>=0.28.0,<0.29.0) Requires-
-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-
-datastore (>=1.1.0,<2.0.0) Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
+Language :: Python :: 3.11 Requires-Dist: arclet-alconna (>=1.7.14,<2.0.0)
+Requires-Dist: asyncpg (>=0.28.0,<0.29.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-datastore (>=1.1.0,<2.0.0)
+Requires-Dist: nonebot2 (>=2.0.1,<3.0.0) Requires-Dist: numpy (>=1.25.2,<2.0.0)
+Requires-Dist: pillow (>=10.0.0,<11.0.0) Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-savepic _â¨ ä¸ä¸ªå­åå¾ççæä»¶ â¨_ ## ð ä»ç»
       éåèª Fran ç Savepic ### savepic ä¿å­è¡¨æå ### randpic
 æ½åè¡¨æå ### ç´æ¥åéæä»¶å åéæä»¶åå³å¯åéè¡¨æå
                ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
```

