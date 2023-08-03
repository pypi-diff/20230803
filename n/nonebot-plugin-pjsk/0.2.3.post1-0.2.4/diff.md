# Comparing `tmp/nonebot_plugin_pjsk-0.2.3.post1.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.3.post1.tar", last modified: Tue Aug  1 15:30:59 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.4.tar", last modified: Thu Aug  3 13:43:07 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.3.post1.tar` & `nonebot_plugin_pjsk-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-08-01 15:30:39.668224 nonebot_plugin_pjsk-0.2.3.post1/LICENSE
--rw-r--r--   0        0        0     4076 2023-08-01 15:30:39.668224 nonebot_plugin_pjsk-0.2.3.post1/README.md
--rw-r--r--   0        0        0      889 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     8436 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0     1163 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0    11099 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     4002 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2351 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1793 2023-08-01 15:30:59.033798 nonebot_plugin_pjsk-0.2.3.post1/pyproject.toml
--rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.3.post1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-03 13:42:50.179963 nonebot_plugin_pjsk-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4300 2023-08-03 13:42:50.179963 nonebot_plugin_pjsk-0.2.4/README.md
+-rw-r--r--   0        0        0      795 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     8728 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1216 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0    11191 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     4002 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2351 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1787 2023-08-03 13:43:07.929358 nonebot_plugin_pjsk-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.4/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/LICENSE` & `nonebot_plugin_pjsk-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/README.md` & `nonebot_plugin_pjsk-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -147,14 +147,19 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.4
+
+- 在交互模式中提供的参数会去掉指令前缀，以防 Adapter 删掉参数开头的 Bot 昵称，导致参数不对的情况
+- 重写帮助图片的渲染（个人感觉效果还不是很好……）
+
 ### 0.2.3
 
 - 限制了贴纸文本大小，以免 Bot 瞬间爆炸
 - 未提供字体大小时适应性调节 ([#14](https://github.com/Agnes4m/nonebot_plugin_pjsk/issues/14))
 - 参数 `--rotate` 改为提供角度值，正数为顺时针旋转
 - 将指令帮助渲染为图片发送（可以关）
 - 丢掉了 `pil-utils` 依赖
```

#### html2text {}

```diff
@@ -26,16 +26,19 @@
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.3
-- éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.4
+- å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
+å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
+éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
+0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
 nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
 æ¹ä¸ºæä¾è§åº¦å¼ï¼æ­£æ°ä¸ºé¡ºæ¶éæè½¬ -
 å°æä»¤å¸®å©æ¸²æä¸ºå¾çåéï¼å¯ä»¥å³ï¼ - ä¸¢æäº `pil-utils`
 ä¾èµ ### 0.2.2 - ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
 è¯éªæ§å°æ¯æäº Emoji ### 0.2.1 - æ´æ¹æä»¤ `pjskåè¡¨`
 çäº¤äºæ¹å¼ ### 0.2.0 - éææä»¶
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
-    usage="直接使用指令 `pjsk` 进入交互创建模式；\n使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助",
+    usage="使用指令 `pjsk -h` 查看帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
     supported_adapters={
         "~onebot.v11",
         "~onebot.v12",
         "~kaiheila",
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__main__.py` & `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,28 +54,33 @@
     priority=2,
 )
 
 
 HELP = (
     "Project Sekai 表情生成\n"
     "\n"
-    f"{cmd_generate_parser.format_help()}\n"
+    f"{cmd_generate_parser.format_help().strip()}\n"
     "\n"
     "Tips：\n"
     "- 大部分有默认值的数值参数都可以用 ^ 开头指定相对于默认值的偏移量\n"
     "- 不提供任何指令参数时会进入交互创建模式"
 )
 
 
+def remove_cmd_prefix(s: str) -> str:
+    pfx = next((x for x in config.command_start if x and s.startswith(x)), None)
+    return s[len(pfx) :] if pfx else s
+
+
 async def handle_exit(matcher: Matcher, arg: str):
     if arg in ("0", "q", "e", "quit", "exit", "退出"):
         await matcher.finish("已退出交互创建模式")
 
 
-def format_error(error: Exception) -> str:
+def format_draw_error(error: Exception) -> str:
     if isinstance(error, ResolveValueError):
         return f"提供的参数值 `{error.args[0]}` 解析出错"
     if isinstance(error, TextTooLargeError):
         return "你给的参数是不是有点太逆天了 😅"
     logger.opt(exception=error).error("Error occurred while drawing sticker")
     return "生成表情时出错，请检查后台日志"
 
@@ -123,23 +128,23 @@
             font_size=resolve_value(args.size, default_text.s),
             stroke_width=resolve_value(args.stroke_width, DEFAULT_STROKE_WIDTH),
             line_spacing=resolve_value(args.line_spacing, DEFAULT_LINE_SPACING, float),
             font_weight=resolve_value(args.weight, DEFAULT_FONT_WEIGHT),
             auto_adjust=args.size is None,
         )
     except Exception as e:
-        await matcher.finish(format_error(e))
+        await matcher.finish(format_draw_error(e))
 
     await MessageFactory([Image(i2b(image))]).finish(reply=True)
 
 
 # interact mode or sticker list
 @cmd_sticker_list.handle()
 async def _(matcher: Matcher, arg: Message = CommandArg()):
-    if arg.extract_plain_text().strip():
+    if remove_cmd_prefix(arg.extract_plain_text()).strip():
         matcher.set_arg("character", arg)
 
 
 # character list
 @cmd_generate.handle()
 @cmd_sticker_list.handle()
 async def _(matcher: Matcher, state: T_State):
@@ -163,15 +168,15 @@
     await (factory.send if interact else factory.finish)(reply=True)
 
 
 # sticker id list
 @cmd_generate.got("character")
 @cmd_sticker_list.got("character")
 async def _(matcher: Matcher, state: T_State, arg_msg: Message = Arg("character")):
-    character = arg_msg.extract_plain_text().strip()
+    character = remove_cmd_prefix(arg_msg.extract_plain_text()).strip()
     await handle_exit(matcher, character)
 
     interact = state.get("interact", True)
 
     # 交互模式
     if interact:
         if character == "随机":
@@ -202,34 +207,33 @@
     factory = MessageFactory(segments)
     await (factory.send if interact else factory.finish)(reply=True)
 
 
 # below are interact mode handlers
 @cmd_generate.got("sticker_id")
 async def _(matcher: Matcher, arg: str = ArgPlainText("sticker_id")):
-    arg = arg.strip()
+    arg = remove_cmd_prefix(arg).strip()
     await handle_exit(matcher, arg)
 
     if not select_or_get_random(arg or None):  # 上面传过来的空消息转 None 获取随机表情
         await matcher.reject("没有找到对应 ID 的表情，请重新输入")
     await matcher.send("请发送你想要写在表情上的的文字")
 
 
 @cmd_generate.got("text")
 async def _(
     matcher: Matcher,
     sticker_id: str = ArgPlainText(),
     text: str = ArgPlainText(),
 ):
+    sticker_id = remove_cmd_prefix(sticker_id).strip()
+    text = remove_cmd_prefix(text).strip()
+
     sticker_info = select_or_get_random(sticker_id)
     assert sticker_info is not None
 
     try:
-        image = await draw_sticker(
-            sticker_info,
-            text=text,
-            auto_adjust=True,
-        )
+        image = await draw_sticker(sticker_info, text=text, auto_adjust=True)
     except Exception as e:
-        await matcher.finish(format_error(e))
+        await matcher.finish(format_draw_error(e))
 
     await MessageFactory([Image(i2b(image))]).finish(reply=True)
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from typing import Set
+
 from imagetext_py import EmojiSource
 from nonebot import get_driver
 from pydantic import BaseModel, validator
 
 
 class ConfigModel(BaseModel):
+    command_start: Set[str]
+
     pjsk_assets_prefix: str = (
         "https://raw.gitmirror.com/TheOriginalAyaka/sekai-stickers/main/"
     )
     pjsk_repo_prefix: str = "https://raw.gitmirror.com/Agnes4m/nonebot_plugin_pjsk/main/"
 
     pjsk_emoji_source: str = "Apple"
     """Emoji 来源，可选值见 https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/imagetext_py.pyi#L217"""
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/draw.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,17 @@
     EmojiOptions,
     EmojiSource,
     Font,
     Paint,
     TextAlign,
     draw_text_multiline,
     text_size_multiline,
-    text_wrap,
 )
 from numpy import deg2rad, rad2deg
-from PIL import Image
+from PIL import Image, ImageDraw, ImageFont
 
 from .config import config
 from .resource import (
     CACHE_FOLDER,
     FONT_PATHS,
     LOADED_STICKER_INFO,
     RESOURCE_FOLDER,
@@ -120,15 +119,14 @@
     font_weight: int = DEFAULT_FONT_WEIGHT,
     stoke_width: int = DEFAULT_STROKE_WIDTH,
     line_spacing: float = DEFAULT_LINE_SPACING,
     align: TextAlign = TextAlign.Center,
     max_width: Optional[int] = None,
     will_rotate: Optional[float] = None,
     min_size: int = 8,
-    error_when_too_large: bool = True,  # noqa: FBT001
 ) -> Image.Image:
     font = ensure_font()
 
     text_lines = text.splitlines()
     padding = stoke_width
 
     while True:
@@ -155,17 +153,15 @@
             if (will_rotate is None)
             else calc_rotated_size(*size, will_rotate)[0]
         )
         if rotated_width <= max_width:
             break
         font_size -= 1
 
-    if error_when_too_large and (
-        size[0] > MAX_TEXT_IMAGE_SIZE or size[1] > MAX_TEXT_IMAGE_SIZE
-    ):
+    if size[0] > MAX_TEXT_IMAGE_SIZE or size[1] > MAX_TEXT_IMAGE_SIZE:
         raise TextTooLargeError
 
     canvas = Canvas(*size, Color(255, 255, 255, 0))
     await anyio.to_thread.run_sync(
         partial(
             draw_text_multiline,
             canvas=canvas,
@@ -233,31 +229,32 @@
     rotate: Optional[int] = None,
     font_size: Optional[int] = None,
     stroke_width: Optional[int] = None,
     line_spacing: Optional[float] = None,
     font_weight: Optional[int] = None,
     auto_adjust: bool = False,  # noqa: FBT001
 ) -> Image.Image:
+    default_text = info.default_text
     sticker_img = await anyio.Path(RESOURCE_FOLDER / info.img).read_bytes()
     text_img = await render_text(
-        text or info.default_text.text,
+        text or default_text.text,
         info.color,
-        font_size or info.default_text.s,
+        font_size or default_text.s,
         font_weight or DEFAULT_FONT_WEIGHT,
         stroke_width or DEFAULT_STROKE_WIDTH,
         line_spacing or DEFAULT_LINE_SPACING,
         max_width=CANVAS_SIZE[0] if auto_adjust else None,
         will_rotate=rotate,
     )
     return paste_text_on_image(
         Image.open(BytesIO(sticker_img)).convert("RGBA"),
         text_img,
-        x or info.default_text.x,
-        y or info.default_text.y,
-        rotate or rad2deg(info.default_text.r / 10),
+        x or default_text.x,
+        y or default_text.y,
+        rotate or rad2deg(default_text.r / 10),
     )
 
 
 def render_summary_picture(
     image_list: List[Image.Image],
     padding: int = 15,
     line_max: int = 5,
@@ -293,56 +290,51 @@
         await asyncio.gather(*tasks),
         padding,
         line_max,
         background,
     )
 
 
+def wrap_line(line: str, font: ImageFont.FreeTypeFont, width: int) -> List[str]:
+    if font.getlength(line) <= width:
+        return [line]
+
+    wrapped: List[str] = []
+    tail = ""
+    while font.getlength(line) > width:
+        tail = line[-1] + tail
+        line = line[:-1]
+    wrapped.append(line)
+    wrapped.extend(wrap_line(tail, font, width))
+    return wrapped
+
+
 async def render_help_image(text: str) -> Image.Image:
-    font = ensure_font()
+    width = 900
     font_size = 24
-    line_spacing = 1.2
-    width = 950
     padding = 24
+    font = ImageFont.truetype(str(FONT_PATHS[-1]), font_size)
 
-    # 这个空行还有缩进的处理，实属无奈
-    wrapped = [
-        x[1:] if x.startswith(">") else x
-        for x in itertools.chain.from_iterable(
-            (
-                text_wrap(
-                    f">{x}" if x.startswith(" ") else x,
-                    width - padding * 2,
-                    font_size,
-                    font,
-                )
-                if x
-                else " "
-            )
-            for x in text.splitlines()
-        )
-    ]
-    size = text_size_multiline(wrapped, font_size, font, line_spacing)
-
-    canvas = Canvas(width, size[1] + padding * 2, hex_to_color(ONE_DARK_BLACK))
-    draw_text_multiline(
-        canvas,
-        wrapped,
-        padding,
-        padding,
-        0,
-        0,
-        400,
-        font_size,
-        font,
-        Paint(hex_to_color(ONE_DARK_WHITE)),
-        line_spacing,
+    warped_lines: List[str] = list(
+        itertools.chain.from_iterable(
+            wrap_line(line, font, width - padding * 2) for line in text.split("\n")
+        ),
     )
+    text = "\n".join(warped_lines)
+
+    # 什么傻逼设计，为什么要新建一个 ImageDraw 才能拿多行高度
+    empty_draw = ImageDraw.Draw(Image.new("1", (1, 1)))
+    text_bbox = empty_draw.multiline_textbbox((0, 0), text, font=font)
+    text_height = text_bbox[3] - text_bbox[1]
+
+    image = Image.new("RGBA", (width, text_height + padding * 2), ONE_DARK_BLACK)
+    draw = ImageDraw.Draw(image)
+    draw.multiline_text((padding, padding), text, fill=ONE_DARK_WHITE, font=font)
 
-    return canvas.to_image()
+    return image
 
 
 @overload
 def use_image_cache(
     func: Callable[P, Awaitable[Image.Image]],
     filename: str,
     image_format: str = "JPEG",
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/pyproject.toml` & `nonebot_plugin_pjsk-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.3.post1"
+version = "0.2.4"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_pjsk-0.2.3.post1/PKG-INFO` & `nonebot_plugin_pjsk-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.3.post1
+Version: 0.2.4
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -172,14 +172,19 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.4
+
+- 在交互模式中提供的参数会去掉指令前缀，以防 Adapter 删掉参数开头的 Bot 昵称，导致参数不对的情况
+- 重写帮助图片的渲染（个人感觉效果还不是很好……）
+
 ### 0.2.3
 
 - 限制了贴纸文本大小，以免 Bot 瞬间爆炸
 - 未提供字体大小时适应性调节 ([#14](https://github.com/Agnes4m/nonebot_plugin_pjsk/issues/14))
 - 参数 `--rotate` 改为提供角度值，正数为顺时针旋转
 - 将指令帮助渲染为图片发送（可以关）
 - 丢掉了 `pil-utils` 依赖
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.3.post1 Summary:
-Project Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin
-Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email:
-Agnes_Digital
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.4 Summary: Project
+Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
+https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Project-URL:
 Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk Requires-Python:
@@ -41,16 +40,19 @@
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.3
-- éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.4
+- å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
+å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
+éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
+0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
 nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
 æ¹ä¸ºæä¾è§åº¦å¼ï¼æ­£æ°ä¸ºé¡ºæ¶éæè½¬ -
 å°æä»¤å¸®å©æ¸²æä¸ºå¾çåéï¼å¯ä»¥å³ï¼ - ä¸¢æäº `pil-utils`
 ä¾èµ ### 0.2.2 - ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
 è¯éªæ§å°æ¯æäº Emoji ### 0.2.1 - æ´æ¹æä»¤ `pjskåè¡¨`
 çäº¤äºæ¹å¼ ### 0.2.0 - éææä»¶
```

