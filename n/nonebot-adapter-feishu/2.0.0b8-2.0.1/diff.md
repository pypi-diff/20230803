# Comparing `tmp/nonebot_adapter_feishu-2.0.0b8.tar.gz` & `tmp/nonebot_adapter_feishu-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_feishu-2.0.0b8.tar", max compression
+gzip compressed data, was "nonebot_adapter_feishu-2.0.1.tar", max compression
```

## Comparing `nonebot_adapter_feishu-2.0.0b8.tar` & `nonebot_adapter_feishu-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/LICENSE
--rw-r--r--   0        0        0      259 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/README.md
--rw-r--r--   0        0        0      597 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/__init__.py
--rw-r--r--   0        0        0    12438 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/adapter.py
--rw-r--r--   0        0        0     6489 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/bot.py
--rw-r--r--   0        0        0     1393 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/config.py
--rw-r--r--   0        0        0    19848 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/event.py
--rw-r--r--   0        0        0     1373 2023-04-17 02:24:39.698280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/exception.py
--rw-r--r--   0        0        0     8305 2023-04-17 02:24:39.702280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/message.py
--rw-r--r--   0        0        0     1499 2023-04-17 02:24:39.702280 nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/utils.py
--rw-r--r--   0        0        0     1944 2023-04-17 02:24:39.702280 nonebot_adapter_feishu-2.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/LICENSE
+-rw-r--r--   0        0        0      259 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/README.md
+-rw-r--r--   0        0        0      611 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/__init__.py
+-rw-r--r--   0        0        0    12636 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/adapter.py
+-rw-r--r--   0        0        0     6498 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/bot.py
+-rw-r--r--   0        0        0     1393 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/config.py
+-rw-r--r--   0        0        0    19904 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/event.py
+-rw-r--r--   0        0        0     1348 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/exception.py
+-rw-r--r--   0        0        0     8279 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/message.py
+-rw-r--r--   0        0        0     1491 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/utils.py
+-rw-r--r--   0        0        0     2130 2023-08-03 00:06:41.861460 nonebot_adapter_feishu-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1382 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.0.1/PKG-INFO
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/LICENSE` & `nonebot_adapter_feishu-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/__init__.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """飞书协议适配"""
 
-from .event import *
 from .bot import Bot as Bot
 from .utils import log as log
+from .event import *  # noqa: F403
 from .adapter import Adapter as Adapter
 from .message import Message as Message
 from .exception import ActionFailed as ActionFailed
 from .exception import NetworkError as NetworkError
 from .message import MessageSegment as MessageSegment
 from .exception import ApiNotAvailable as ApiNotAvailable
 from .message import MessageSerializer as MessageSerializer
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/adapter.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import asyncio
 import inspect
-from datetime import timedelta
 from typing import Any, Dict, List, Type, Union, Callable, Optional, cast
 
 import httpx
 from pygtrie import StringTrie
 from pydantic import parse_obj_as
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
@@ -53,28 +52,28 @@
     def get_name(cls) -> str:
         """适配器名称: `Feishu`"""
         return "Feishu"
 
     def setup(self) -> None:
         if not isinstance(self.driver, ReverseDriver):
             raise RuntimeError(
-                f"Current driver {self.config.driver} doesn't support reverse connections!"
+                f"Current driver {self.config.driver} "
+                "doesn't support reverse connections!"
                 "Feishu Adapter need a ReverseDriver to work."
             )
 
         @self.driver.on_startup
         async def _():
             async with httpx.AsyncClient() as client:
                 for bot_config in self.feishu_config.feishu_bots:
                     try:
+                        token = await self.get_tenant_access_token(bot_config)
                         response = await client.get(
                             self._construct_url(bot_config, "bot/v3/info"),
-                            headers={
-                                "Authorization": f"Bearer {await self._fetch_tenant_access_token(bot_config)}"
-                            },
+                            headers={"Authorization": f"Bearer {token}"},
                         )
                         if 200 <= response.status_code < 300:
                             result = response.json()
                         else:
                             raise NetworkError(
                                 f"HTTP request received unexpected "
                                 f"status code: {response.status_code}"
@@ -85,15 +84,20 @@
                         raise NetworkError("HTTP request failed")
 
                     self.bot_apps[bot_config.app_id] = bot_config
                     bot_info = parse_obj_as(BotInfo, result.get("bot", {}))
 
                     bot = self.bots.get(bot_config.app_id)
                     if not bot:
-                        bot = Bot(self, bot_config, bot_info)
+                        bot = Bot(
+                            self,
+                            bot_config.app_id,
+                            bot_config=bot_config,
+                            bot_info=bot_info,
+                        )
                         self.bot_connect(bot)
                         log(
                             "INFO",
                             f"<y>Bot {escape_tag(bot_config.app_id)}</y> connected",
                         )
                     setup = HTTPServerSetup(
                         URL(f"/feishu/{bot.self_id}"),
@@ -108,15 +112,15 @@
             self.feishu_config.feishu_lark_api_base
             if bot_config.is_lark
             else self.feishu_config.feishu_api_base
         )
 
         return api_base + path
 
-    async def _fetch_tenant_access_token(self, bot_config: BotConfig) -> str:
+    async def get_tenant_access_token(self, bot_config: BotConfig) -> str:
         token_key = f"feishu_tenant_access_token_{bot_config.app_id}"
         cached_token = await cache.get(token_key)
         if cached_token is not None:
             return cached_token
 
         try:
             async with httpx.AsyncClient() as client:
@@ -131,20 +135,23 @@
                     timeout=self.config.api_timeout,
                 )
 
             if 200 <= response.status_code < 300:
                 result = response.json()
                 expire = result["expire"]
                 # token 有效期为 2 小时，在此期间调用该接口 token 不会改变
-                # 当 token 有效期小于 30 分的时候，再次请求获取 token 的时候，会生成一个新的 token，与此同时老的 token 依然有效
+                # 当 token 有效期小于 30 分的时候，再次请求获取 token 的时候，
+                # 会生成一个新的 token，与此同时老的 token 依然有效
                 # 在有效期小于 30 分时使 token 过期，确保 token 时效性
                 if expire > 30 * 60:
                     expire -= 30 * 60
 
-                await cache.set(token_key, result["tenant_access_token"], expire)  # type: ignore
+                await cache.set(
+                    token_key, result["tenant_access_token"], expire
+                )  # type: ignore
                 return result["tenant_access_token"]
             else:
                 raise NetworkError(
                     f"HTTP request received unexpected "
                     f"status code: {response.status_code}"
                 )
         except httpx.InvalidURL:
@@ -153,17 +160,16 @@
             raise NetworkError("HTTP request failed")
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         timeout: float = data.get("_timeout", self.config.api_timeout)
         log("DEBUG", f"Calling API <y>{api}</y>")
 
-        headers = {
-            "Authorization": f"Bearer {await self._fetch_tenant_access_token(bot.bot_config)}"
-        }
+        token = await self.get_tenant_access_token(bot.bot_config)
+        headers = {"Authorization": f"Bearer {token}"}
 
         try:
             async with httpx.AsyncClient(timeout=timeout) as client:
                 request = data.get(
                     "request",
                     httpx.Request(
                         data["method"],
@@ -219,15 +225,15 @@
         if challenge:
             return Response(200, content=json.dumps({"challenge": challenge}).encode())
 
         schema = data.get("schema")
         if not schema:
             return Response(
                 400,
-                content="Missing `schema` in POST body, only accept event of version 2.0",
+                content=("Missing `schema` in POST body, only accept event V2"),
             )
 
         headers = data.get("header")
         if headers:
             token = headers.get("token")
         else:
             log("WARNING", "Missing `header` in POST body")
@@ -312,15 +318,17 @@
         """
         if not hasattr(model, "__event__"):
             raise ValueError("Event model's `__event__` attribute must be set")
         cls.event_models["." + model.__event__] = model
 
     @classmethod
     def get_event_model(cls, event_name: str) -> List[Type[Event]]:
-        """根据事件名获取对应 `Event Model` 及 `FallBack Event Model` 列表，不包括基类 `Event`。"""
+        """根据事件名获取对应 `Event Model` 及 `FallBack Event Model` 列表，
+        不包括基类 `Event`。
+        """
         return [model.value for model in cls.event_models.prefixes("." + event_name)][
             ::-1
         ]
 
     @classmethod
     def custom_send(
         cls,
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/bot.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         "body": {
             "receive_id": receive_id,
             "content": content,
             "msg_type": msg_type,
         },
     }
 
-    return await bot.call_api(f"im/v1/messages", **params)
+    return await bot.call_api("im/v1/messages", **params)
 
 
 class BotInfo(BaseModel):
     activate_status: int = Field(alias="activate_status")
     app_name: str = Field(alias="app_name")
     avatar_url: HttpUrl = Field(alias="avatar_url")
     ip_white_list: List[str] = Field(alias="ip_white_list")
@@ -148,23 +148,26 @@
     """
 
     send_handler: Callable[
         ["Bot", Event, Union[str, Message, MessageSegment]], Any
     ] = send
 
     @overrides(BaseBot)
-    def __init__(self, adapter: "Adapter", bot_config: BotConfig, bot_info: BotInfo):
-        super().__init__(adapter, bot_config.app_id)
+    def __init__(
+        self,
+        adapter: "Adapter",
+        self_id: str,
+        *,
+        bot_config: BotConfig,
+        bot_info: BotInfo,
+    ):
+        super().__init__(adapter, self_id)
         self.bot_config: BotConfig = bot_config
         self.bot_info: BotInfo = bot_info
 
-    @property
-    def type(self) -> str:
-        return "feishu"
-
     @overrides(BaseBot)
     async def send(
         self,
         event: Event,
         message: Union[str, Message, MessageSegment],
         **kwargs: Any,
     ) -> Any:
@@ -176,15 +179,15 @@
             kwargs: 其他参数，可以与 {ref}`nonebot.adapters.feishu.adapter.Adapter.custom_send` 配合使用
         返回:
             API 调用返回数据
         异常:
             ValueError: 缺少 `user_id`, `group_id`
             NetworkError: 网络错误
             ActionFailed: API 调用失败
-        """
+        """  # noqa: E501
         return await self.__class__.send_handler(self, event, message, **kwargs)
 
     @overrides(BaseBot)
     async def call_api(self, api: str, **data) -> Any:
         """
         :说明:
           调用 OneBot 协议 API
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/config.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/event.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,19 @@
         return self.event.sender.sender_id.open_id
 
     def get_all_user_id(self) -> UserId:
         return self.event.sender.sender_id
 
     @overrides(Event)
     def get_session_id(self) -> str:
-        return f"{self.event.message.chat_type}_{self.event.message.chat_id}_{self.get_user_id()}"
+        return (
+            f"{self.event.message.chat_type}"
+            f"_{self.event.message.chat_id}"
+            f"_{self.get_user_id()}"
+        )
 
     @overrides(Event)
     def is_tome(self) -> bool:
         return self.to_me
 
 
 class GroupMessageEvent(MessageEvent):
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/exception.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 
     def __init__(self, **kwargs):
         super().__init__()
         self.info = kwargs
 
     def __repr__(self):
         return (
-            f"<ActionFailed "
-            + ", ".join(f"{k}={v}" for k, v in self.info.items())
-            + ">"
+            "<ActionFailed " + ", ".join(f"{k}={v}" for k, v in self.info.items()) + ">"
         )
 
     def __str__(self):
         return self.__repr__()
 
 
 class NetworkError(BaseNetworkError, FeishuAdapterException):
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/message.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,23 +132,23 @@
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
 
     @overrides(BaseMessage)
     def __add__(
         self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
     ) -> "Message":
-        return super(Message, self).__add__(
+        return super().__add__(
             MessageSegment.text(other) if isinstance(other, str) else other
         )
 
     @overrides(BaseMessage)
     def __radd__(
         self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
     ) -> "Message":
-        return super(Message, self).__radd__(
+        return super().__radd__(
             MessageSegment.text(other) if isinstance(other, str) else other
         )
 
     @staticmethod
     @overrides(BaseMessage)
     def _construct(
         msg: Union[str, Mapping, Iterable[Mapping]]
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/nonebot/adapters/feishu/utils.py` & `nonebot_adapter_feishu-2.0.1/nonebot/adapters/feishu/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if result.get("code") != 0:
             raise ActionFailed(**result)
         return result.get("data")
     else:
         return result
 
 
-class AESCipher(object):
+class AESCipher:
     def __init__(self, key):
         self.block_size = AES.block_size
         self.key = hashlib.sha256(AESCipher.str_to_bytes(key)).digest()
 
     @staticmethod
     def str_to_bytes(data):
         u_type = type(b"".decode("utf8"))
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/pyproject.toml` & `nonebot_adapter_feishu-2.0.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-feishu"
-version = "2.0.0-beta.8"
+version = "2.0.1"
 description = "feishu(larksuite) adapter for nonebot2"
 authors = ["StarHeartHunt <starheart233@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://feishu.adapters.nonebot.dev/"
 repository = "https://github.com/nonebot/adapter-feishu"
 documentation = "https://feishu.adapters.nonebot.dev/"
@@ -19,25 +19,25 @@
 packages = [
   { include = "nonebot" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pycryptodome = "^3.10.1"
-httpx = ">=0.18.0, <1.0.0"
-nonebot2 = ">=2.0.0-beta.1"
-cashews = ">=5,<7"
+httpx = ">=0.20.0, <1.0.0"
+nonebot2 = ">=2.0.0"
+cashews = ">=6.0.0, <7.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pycln = "^2.1.2"
+ruff = "^0.0.282"
 isort = "^5.10.1"
 black = "^23.1.0"
 nonemoji = "^0.1.2"
 pre-commit = "^3.0.0"
-nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
+nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", branch = "master", extras = ["fastapi"] }
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.0.2"
 pytest-asyncio = ">=0.20,<0.22"
 nonebug = { git = "https://github.com/nonebot/nonebug.git" }
 
@@ -55,27 +55,31 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
-[tool.pycln]
-path = "."
-all = false
+[tool.ruff]
+select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q"]
+ignore = ["E402", "C901"]
+
+line-length = 88
+target-version = "py38"
+
+[tool.ruff.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
 
 [tool.pyright]
-reportShadowedImports = false
 pythonVersion = "3.8"
 pythonPlatform = "All"
 executionEnvironments = [
   { root = "./" },
 ]
-exclude = [
-  "**/node_modules",
-  "**/__pycache__",
-  "**/tests"
-]
+
+typeCheckingMode = "basic"
+reportShadowedImports = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_adapter_feishu-2.0.0b8/PKG-INFO` & `nonebot_adapter_feishu-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-feishu
-Version: 2.0.0b8
+Version: 2.0.1
 Summary: feishu(larksuite) adapter for nonebot2
 Home-page: https://feishu.adapters.nonebot.dev/
 License: MIT
 Keywords: bot,feishu,larksuite
 Author: StarHeartHunt
 Author-email: starheart233@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,18 +14,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: cashews (>=5,<7)
-Requires-Dist: httpx (>=0.18.0,<1.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.1)
+Requires-Dist: cashews (>=6.0.0,<7.0.0)
+Requires-Dist: httpx (>=0.20.0,<1.0.0)
+Requires-Dist: nonebot2 (>=2.0.0)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Project-URL: Documentation, https://feishu.adapters.nonebot.dev/
 Project-URL: Repository, https://github.com/nonebot/adapter-feishu
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://feishu.adapters.nonebot.dev/"><img src="https://feishu.adapters.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.0.0b8 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.0.1 Summary:
 feishu(larksuite) adapter for nonebot2 Home-page: https://
 feishu.adapters.nonebot.dev/ License: MIT Keywords: bot,feishu,larksuite
 Author: StarHeartHunt Author-email: starheart233@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Framework :: Robot Framework Classifier: Framework :: Robot Framework ::
 Library Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Requires-Dist: cashews (>=5,<7) Requires-Dist: httpx
-(>=0.18.0,<1.0.0) Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist:
-pycryptodome (>=3.10.1,<4.0.0) Project-URL: Documentation, https://
-feishu.adapters.nonebot.dev/ Project-URL: Repository, https://github.com/
-nonebot/adapter-feishu Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: cashews
+(>=6.0.0,<7.0.0) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot2
+(>=2.0.0) Requires-Dist: pycryptodome (>=3.10.1,<4.0.0) Project-URL:
+Documentation, https://feishu.adapters.nonebot.dev/ Project-URL: Repository,
+https://github.com/nonebot/adapter-feishu Description-Content-Type: text/
+markdown
                                    [nonebot]
              # NoneBot-Adapter-Feishu _â¨ é£ä¹¦åè®®éé â¨_
```

