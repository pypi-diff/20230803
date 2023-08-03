# Comparing `tmp/nonebot_plugin_setu_now-0.6.2.tar.gz` & `tmp/nonebot_plugin_setu_now-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_setu_now-0.6.2.tar", last modified: Tue Jun 27 09:17:54 2023, max compression
+gzip compressed data, was "nonebot_plugin_setu_now-0.6.3.tar", last modified: Thu Aug  3 14:41:12 2023, max compression
```

## Comparing `nonebot_plugin_setu_now-0.6.2.tar` & `nonebot_plugin_setu_now-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-06-27 09:17:42.000607 nonebot_plugin_setu_now-0.6.2/LICENSE
--rw-r--r--   0        0        0     3403 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/README.md
--rwxr-xr-x   0        0        0     7534 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/__init__.py
--rw-r--r--   0        0        0      305 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/aioutils/__init__.py
--rw-r--r--   0        0        0     3922 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/aioutils/_main.py
--rw-r--r--   0        0        0     1030 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/config.py
--rw-r--r--   0        0        0     2340 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/data_source.py
--rw-r--r--   0        0        0     1047 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/database.py
--rw-r--r--   0        0        0     4262 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/img_utils.py
--rw-r--r--   0        0        0      959 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/models.py
--rw-r--r--   0        0        0      613 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/perf_timer.py
--rw-r--r--   0        0        0     1640 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/r18_whitelist.py
--rw-r--r--   0        0        0     2964 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/utils.py
--rw-r--r--   0        0        0      797 2023-06-27 09:17:54.784708 nonebot_plugin_setu_now-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3403 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/README.md
+-rwxr-xr-x   0        0        0     7534 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/__init__.py
+-rw-r--r--   0        0        0      305 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/aioutils/__init__.py
+-rw-r--r--   0        0        0     3922 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/aioutils/_main.py
+-rw-r--r--   0        0        0     1116 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/config.py
+-rw-r--r--   0        0        0     2340 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/data_source.py
+-rw-r--r--   0        0        0     1047 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/database.py
+-rw-r--r--   0        0        0     4400 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/img_utils.py
+-rw-r--r--   0        0        0      959 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/models.py
+-rw-r--r--   0        0        0      613 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/perf_timer.py
+-rw-r--r--   0        0        0     1640 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/r18_whitelist.py
+-rw-r--r--   0        0        0     2964 2023-08-03 14:41:01.659961 nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/utils.py
+-rw-r--r--   0        0        0      797 2023-08-03 14:41:12.728351 nonebot_plugin_setu_now-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.3/PKG-INFO
```

### Comparing `nonebot_plugin_setu_now-0.6.2/LICENSE` & `nonebot_plugin_setu_now-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/README.md` & `nonebot_plugin_setu_now-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/__init__.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/aioutils/_main.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/aioutils/_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/config.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from nonebot import get_driver
-from pydantic import BaseModel, Extra
+from pydantic import Extra, BaseModel
 
 
 class Config(BaseModel, extra=Extra.ignore):
     superusers: set
     debug: Optional[bool] = False
     setu_cd: int = 60
     setu_path: Optional[str] = None
@@ -13,20 +13,22 @@
     setu_withdraw: Optional[int] = None
     setu_reverse_proxy: str = "i.pixiv.re"
     setu_size: str = "regular"
     setu_api_url: str = "https://api.lolicon.app/setu/v2"
     setu_max: int = 30
     setu_add_random_effect: bool = True
     setu_minimum_send_interval: int = 3
+    setu_send_as_bytes: bool = False
 
 
 plugin_config = Config.parse_obj(get_driver().config.dict())
 CDTIME = plugin_config.setu_cd
 SETU_PATH = plugin_config.setu_path
 PROXY = plugin_config.setu_proxy
 WITHDRAW_TIME = plugin_config.setu_withdraw
 REVERSE_PROXY = plugin_config.setu_reverse_proxy
 SETU_SIZE = plugin_config.setu_size
 API_URL = plugin_config.setu_api_url
 MAX = plugin_config.setu_max
 EFFECT = plugin_config.setu_add_random_effect
 SEND_INTERVAL = plugin_config.setu_minimum_send_interval
+SEND_AS_BYTES = plugin_config.setu_send_as_bytes
```

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/data_source.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/database.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/database.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/img_utils.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/img_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from io import BytesIO
-from pathlib import Path
 from random import choice, randint
 from typing import Union
+from pathlib import Path
 
-from nonebot.adapters.onebot.v11 import MessageSegment
-from nonebot.log import logger
 from PIL import Image, ImageFilter
+from nonebot.log import logger
+from nonebot.adapters.onebot.v11 import MessageSegment
 
+from .config import SEND_AS_BYTES
 from .perf_timer import PerfTimer
 
 
 def image_param_converter(source: Union[Path, Image.Image, bytes]) -> Image.Image:
     FORCE_RESIZE = True
     IMAGE_RESIZE_RES = 1080  # 限制被处理图片最大为1080P
 
@@ -113,15 +114,19 @@
 
 def do_nothing(img: Path) -> Path:
     return img
 
 
 def image_segment_convert(img: Union[Path, Image.Image, bytes]) -> MessageSegment:
     if isinstance(img, Path):
-        return MessageSegment.image(img)
+        # 将图片读取
+        if SEND_AS_BYTES:
+            img = Image.open(img)
+        else:
+            return MessageSegment.image(img)
     elif isinstance(img, bytes):
         img = Image.open(BytesIO(img))
     elif isinstance(img, Image.Image):
         pass
     else:
         raise ValueError(f"Unsopported image type: {type(img)}")
     image_bytesio = BytesIO()
```

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/models.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/perf_timer.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/perf_timer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/r18_whitelist.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/r18_whitelist.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/utils.py` & `nonebot_plugin_setu_now-0.6.3/nonebot_plugin_setu_now/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.2/pyproject.toml` & `nonebot_plugin_setu_now-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-setu-now"
-version = "0.6.2"
+version = "0.6.3"
 description = "另一个色图插件"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_setu_now-0.6.2/PKG-INFO` & `nonebot_plugin_setu_now-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-setu-now
-Version: 0.6.2
+Version: 0.6.3
 Summary: 另一个色图插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-setu-now
 Author-Email: kexue <xana278@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/kexue-z/nonebot-plugin-setu-now
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx<1.0.0,>=0.18.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.3 Summary:
 å¦ä¸ä¸ªè²å¾æä»¶ Home-page: https://github.com/kexue-z/nonebot-plugin-
 setu-now Author-Email: kexue
 foxmail.com> License: MIT Project-URL: Homepage, https://github.com/kexue-z/
 nonebot-plugin-setu-now Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx<1.0.0,>=0.18.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0 Requires-Dist: pydantic>=1.5.0 Requires-Dist:
 pillow>=8.0.0 Requires-Dist: nonebot-plugin-tortoise-orm>=0.1.0 Requires-Dist:
```

