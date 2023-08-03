# Comparing `tmp/rath-0.3.6.tar.gz` & `tmp/rath-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rath-0.3.6.tar", max compression
+gzip compressed data, was "rath-0.4.0.tar", max compression
```

## Comparing `rath-0.3.6.tar` & `rath-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0     4921 2022-11-21 12:07:57.958148 rath-0.3.6/README.md
--rw-r--r--   0        0        0     1454 2023-02-24 17:43:31.125237 rath-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       43 2022-04-12 10:04:18.856216 rath-0.3.6/rath/__init__.py
--rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.3.6/rath/contrib/fakts/__init__.py
--rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.3.6/rath/contrib/fakts/links/__init__.py
--rw-r--r--   0        0        0     1171 2022-11-17 17:51:17.154953 rath-0.3.6/rath/contrib/fakts/links/aiohttp.py
--rw-r--r--   0        0        0      819 2022-10-22 15:39:42.485197 rath-0.3.6/rath/contrib/fakts/links/httpx.py
--rw-r--r--   0        0        0      924 2022-11-17 17:51:39.507050 rath-0.3.6/rath/contrib/fakts/links/websocket.py
--rw-r--r--   0        0        0      611 2022-07-24 12:46:45.543098 rath-0.3.6/rath/contrib/herre/links/auth.py
--rw-r--r--   0        0        0      418 2022-11-21 12:24:05.838929 rath-0.3.6/rath/errors.py
--rw-r--r--   0        0        0       86 2022-04-12 10:04:18.856216 rath-0.3.6/rath/links/__init__.py
--rw-r--r--   0        0        0     5047 2022-11-21 12:26:06.227007 rath-0.3.6/rath/links/aiohttp.py
--rw-r--r--   0        0        0     2596 2022-11-21 13:28:21.224668 rath-0.3.6/rath/links/auth.py
--rw-r--r--   0        0        0     2623 2022-11-21 12:32:18.159322 rath-0.3.6/rath/links/base.py
--rw-r--r--   0        0        0     3979 2022-11-21 12:35:00.035481 rath-0.3.6/rath/links/compose.py
--rw-r--r--   0        0        0     1717 2022-11-21 12:36:55.759600 rath-0.3.6/rath/links/dictinglink.py
--rw-r--r--   0        0        0      660 2022-11-21 12:37:32.047639 rath-0.3.6/rath/links/errors.py
--rw-r--r--   0        0        0     2402 2022-11-21 12:38:21.551691 rath-0.3.6/rath/links/file.py
--rw-r--r--   0        0        0     3189 2022-11-21 13:28:24.380670 rath-0.3.6/rath/links/httpx.py
--rw-r--r--   0        0        0      630 2022-11-21 12:41:14.159878 rath-0.3.6/rath/links/parsing.py
--rw-r--r--   0        0        0     1690 2022-11-21 12:44:56.872125 rath-0.3.6/rath/links/retry.py
--rw-r--r--   0        0        0      739 2022-11-21 12:41:55.931923 rath-0.3.6/rath/links/shrink.py
--rw-r--r--   0        0        0     2158 2022-11-21 12:43:02.391997 rath-0.3.6/rath/links/split.py
--rw-r--r--   0        0        0        0 2022-02-18 09:52:41.143787 rath-0.3.6/rath/links/testing/__init__.py
--rw-r--r--   0        0        0       91 2022-03-14 16:31:19.964012 rath-0.3.6/rath/links/testing/check.py
--rw-r--r--   0        0        0     4441 2022-04-12 10:04:18.856216 rath-0.3.6/rath/links/testing/mock.py
--rw-r--r--   0        0        0     7161 2022-07-24 12:46:45.543098 rath-0.3.6/rath/links/testing/statefulmock.py
--rw-r--r--   0        0        0     9887 2022-04-12 10:04:18.856216 rath-0.3.6/rath/links/transpile.py
--rw-r--r--   0        0        0     3109 2022-04-12 10:04:18.856216 rath-0.3.6/rath/links/utils.py
--rw-r--r--   0        0        0     4025 2022-11-21 12:46:52.128255 rath-0.3.6/rath/links/validate.py
--rw-r--r--   0        0        0    10243 2023-02-06 14:01:14.722574 rath-0.3.6/rath/links/websockets.py
--rw-r--r--   0        0        0     2884 2022-11-21 12:23:39.234913 rath-0.3.6/rath/operation.py
--rw-r--r--   0        0        0       60 2022-04-12 10:04:18.856216 rath-0.3.6/rath/qt/__init__.py
--rw-r--r--   0        0        0      839 2022-09-23 09:27:15.868008 rath-0.3.6/rath/qt/helpers.py
--rw-r--r--   0        0        0     8550 2023-01-19 14:32:13.834198 rath-0.3.6/rath/rath.py
--rw-r--r--   0        0        0     1029 2022-07-24 12:46:45.543098 rath-0.3.6/rath/scalars.py
--rw-r--r--   0        0        0        0 2022-01-28 15:19:12.944704 rath-0.3.6/rath/turms/__init__.py
--rw-r--r--   0        0        0      826 2022-04-12 10:04:18.856216 rath-0.3.6/rath/turms/funcs.py
--rw-r--r--   0        0        0        0 2022-03-14 16:31:19.964012 rath-0.3.6/rath/turms/plugins/__init__.py
--rw-r--r--   0        0        0     1350 2022-08-25 12:16:33.053621 rath-0.3.6/rath/turms/plugins/funcs.py
--rw-r--r--   0        0        0     6120 1970-01-01 00:00:00.000000 rath-0.3.6/setup.py
--rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 rath-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     4921 2022-11-21 12:07:57.958148 rath-0.4.0/README.md
+-rw-r--r--   0        0        0     1425 2023-08-02 15:27:45.537807 rath-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2022-04-12 10:04:18.856216 rath-0.4.0/rath/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.4.0/rath/contrib/fakts/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-24 12:46:45.543098 rath-0.4.0/rath/contrib/fakts/links/__init__.py
+-rw-r--r--   0        0        0     1188 2023-08-02 10:24:16.092036 rath-0.4.0/rath/contrib/fakts/links/aiohttp.py
+-rw-r--r--   0        0        0      836 2023-08-02 11:51:30.163471 rath-0.4.0/rath/contrib/fakts/links/graphql_ws.py
+-rw-r--r--   0        0        0      836 2023-08-02 10:25:04.696296 rath-0.4.0/rath/contrib/fakts/links/httpx.py
+-rw-r--r--   0        0        0      965 2023-08-02 11:51:35.203500 rath-0.4.0/rath/contrib/fakts/links/subscription_transport_ws.py
+-rw-r--r--   0        0        0      410 2023-08-02 10:25:47.464525 rath-0.4.0/rath/contrib/herre/links/auth.py
+-rw-r--r--   0        0        0      429 2023-08-02 09:25:39.868383 rath-0.4.0/rath/errors.py
+-rw-r--r--   0        0        0       86 2022-04-12 10:04:18.856216 rath-0.4.0/rath/links/__init__.py
+-rw-r--r--   0        0        0     5117 2023-08-02 09:25:17.348258 rath-0.4.0/rath/links/aiohttp.py
+-rw-r--r--   0        0        0     3022 2023-08-02 09:25:52.976455 rath-0.4.0/rath/links/auth.py
+-rw-r--r--   0        0        0     2624 2023-08-02 09:26:14.480573 rath-0.4.0/rath/links/base.py
+-rw-r--r--   0        0        0     3680 2023-08-02 09:26:26.408638 rath-0.4.0/rath/links/compose.py
+-rw-r--r--   0        0        0     1733 2023-08-02 09:24:27.551981 rath-0.4.0/rath/links/dictinglink.py
+-rw-r--r--   0        0        0      658 2023-08-02 09:24:27.535981 rath-0.4.0/rath/links/errors.py
+-rw-r--r--   0        0        0     2402 2022-11-21 12:38:21.551691 rath-0.4.0/rath/links/file.py
+-rw-r--r--   0        0        0      758 2023-07-31 15:05:51.639285 rath-0.4.0/rath/links/foward.py
+-rw-r--r--   0        0        0    12157 2023-08-02 09:24:00.691830 rath-0.4.0/rath/links/graphql_ws.py
+-rw-r--r--   0        0        0     3083 2023-08-02 09:26:31.284665 rath-0.4.0/rath/links/httpx.py
+-rw-r--r--   0        0        0      755 2023-08-02 09:26:38.880706 rath-0.4.0/rath/links/log.py
+-rw-r--r--   0        0        0      628 2023-08-02 09:24:27.535981 rath-0.4.0/rath/links/parsing.py
+-rw-r--r--   0        0        0     1688 2023-05-28 12:40:04.463984 rath-0.4.0/rath/links/retry.py
+-rw-r--r--   0        0        0      735 2023-08-02 09:24:27.539981 rath-0.4.0/rath/links/shrink.py
+-rw-r--r--   0        0        0     1947 2023-07-31 14:50:32.714120 rath-0.4.0/rath/links/split.py
+-rw-r--r--   0        0        0    11681 2023-08-02 09:26:43.452731 rath-0.4.0/rath/links/subscription_transport_ws.py
+-rw-r--r--   0        0        0        0 2022-02-18 09:52:41.143787 rath-0.4.0/rath/links/testing/__init__.py
+-rw-r--r--   0        0        0       91 2022-03-14 16:31:19.964012 rath-0.4.0/rath/links/testing/check.py
+-rw-r--r--   0        0        0     4441 2022-04-12 10:04:18.856216 rath-0.4.0/rath/links/testing/mock.py
+-rw-r--r--   0        0        0     7576 2023-08-02 09:27:12.180888 rath-0.4.0/rath/links/testing/statefulmock.py
+-rw-r--r--   0        0        0     9937 2023-08-02 09:29:11.489529 rath-0.4.0/rath/links/transpile.py
+-rw-r--r--   0        0        0     3109 2022-04-12 10:04:18.856216 rath-0.4.0/rath/links/utils.py
+-rw-r--r--   0        0        0     4022 2023-08-02 09:24:27.583981 rath-0.4.0/rath/links/validate.py
+-rw-r--r--   0        0        0     2973 2023-07-31 15:17:57.763465 rath-0.4.0/rath/operation.py
+-rw-r--r--   0        0        0       60 2022-04-12 10:04:18.856216 rath-0.4.0/rath/qt/__init__.py
+-rw-r--r--   0        0        0      839 2022-09-23 09:27:15.868008 rath-0.4.0/rath/qt/helpers.py
+-rw-r--r--   0        0        0     6889 2023-07-31 16:51:14.008216 rath-0.4.0/rath/rath.py
+-rw-r--r--   0        0        0     1029 2022-07-24 12:46:45.543098 rath-0.4.0/rath/scalars.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:19:12.944704 rath-0.4.0/rath/turms/__init__.py
+-rw-r--r--   0        0        0      826 2022-04-12 10:04:18.856216 rath-0.4.0/rath/turms/funcs.py
+-rw-r--r--   0        0        0        0 2022-03-14 16:31:19.964012 rath-0.4.0/rath/turms/plugins/__init__.py
+-rw-r--r--   0        0        0     1350 2022-08-25 12:16:33.053621 rath-0.4.0/rath/turms/plugins/funcs.py
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 rath-0.4.0/PKG-INFO
```

### Comparing `rath-0.3.6/README.md` & `rath-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/pyproject.toml` & `rath-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "rath"
-version = "0.3.6"
+version = "0.4.0"
 description = "async transport-agnostic graphql client"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "rath" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-koil = ">=0.2.10"
+koil = "0.3.3"
 graphql-core = "^3.2.0"
 pydantic = "^1.9.0"
 websockets = { version = "^10.2", optional = true }
 aiohttp = { version = "^3.8.2", optional = true }
 certifi = { version = ">2021", optional = true }
 httpx = { version = "^0.23.0", optional = true }
 
@@ -22,24 +22,23 @@
 httpx = ["httpx"]
 
 
 [tool.poetry.group.dev.dependencies]
 httpx = "^0.23.0"
 autoflake = "^1.7.7"
 pytest = "^7.2.0"
-PyQtWebEngine = "^5.15.5"
-PyQt5 = "^5.15.6"
 testcontainers = "^3.7.0"
 pytest-qt = "^4.2.0"
 pytest-asyncio = "^0.20.2"
 turms = { version = ">=0.2.3", python = "^3.9" }
 aiohttp = "^3.8.3"
 websockets = "^10.4"
 black = "^22.10.0"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.282"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.pydoc-markdown.loaders]]
 type = "python"
```

### Comparing `rath-0.3.6/rath/contrib/fakts/links/aiohttp.py` & `rath-0.4.0/rath/contrib/fakts/links/aiohttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Provides  a fakts implementaiton of the aiohttp link"""
 
 from typing import Any, Dict, Optional
 from fakts.fakt import Fakt
-from fakts.fakts import get_current_fakts
+from fakts.fakts import get_current_fakts, Fakts
 from rath.links.aiohttp import AIOHttpLink
 
 
 class AioHttpConfig(Fakt):
     """AioHttpConfig
 
     AioHttpConfig is a Fakt that can be used to configure the aiohttp client.
@@ -19,26 +19,25 @@
     """FaktsAIOHttpLink
 
     A FaktsAIOHttpLink is a link that retrieves the configuration
     from a sorounding fakts context.
 
     """
 
+    fakts: Fakts
     endpoint_url: Optional[str]
 
     fakts_group: str
     """ The fakts group within the fakts context to use for configuration """
 
     _old_fakt: Dict[str, Any] = None
 
     def configure(self, fakt: AioHttpConfig) -> None:
         """Configure the link with the given fakt"""
         self.endpoint_url = fakt.endpoint_url
 
-    async def aconnect(self):
-        fakts = get_current_fakts()
-
-        if fakts.has_changed(self._old_fakt, self.fakts_group):
-            self._old_fakt = await fakts.aget(self.fakts_group)
+    async def aconnect(self, operation):
+        if self.fakts.has_changed(self._old_fakt, self.fakts_group):
+            self._old_fakt = await self.fakts.aget(self.fakts_group)
             self.configure(AioHttpConfig(**self._old_fakt))
 
-        return await super().aconnect()
+        return await super().aconnect(operation)
```

### Comparing `rath-0.3.6/rath/contrib/fakts/links/httpx.py` & `rath-0.4.0/rath/contrib/fakts/links/httpx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from typing import Any, Dict, Optional
 from fakts.fakt.base import Fakt
-from fakts.fakts import get_current_fakts
+from fakts.fakts import get_current_fakts, Fakts
 from rath.links.httpx import HttpxLink
 
 
 class FaltsHttpXConfig(Fakt):
     endpoint_url: str
 
     class Config:
         group = "aiohttp"
 
 
 class FaktsHttpXLink(HttpxLink):
     endpoint_url: Optional[str]
     fakts_group: str
     fakt: Optional[FaltsHttpXConfig]
+    fakts: Fakts
 
     _old_fakt: Dict[str, Any] = None
 
     def configure(self, fakt: FaltsHttpXConfig) -> None:
         self.endpoint_url = fakt.endpoint_url
 
-    async def aconnect(self):
-        fakts = get_current_fakts()
-
-        if fakts.has_changed(self._old_fakt, self.fakts_group):
-            self._old_fakt = await fakts.aget(self.fakts_group)
+    async def aconnect(self, operation):
+        if self.fakts.has_changed(self._old_fakt, self.fakts_group):
+            self._old_fakt = await self.fakts.aget(self.fakts_group)
             self.configure(FaltsHttpXConfig(**self._old_fakt))
 
-        return await super().aconnect()
+        return await super().aconnect(operation)
```

### Comparing `rath-0.3.6/rath/contrib/fakts/links/websocket.py` & `rath-0.4.0/rath/contrib/fakts/links/subscription_transport_ws.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from typing import Any, Dict, Optional
 
 from fakts.fakt.base import Fakt
-from fakts.fakts import get_current_fakts
+from fakts.fakts import Fakts
 from herre import current_herre
-from rath.links.websockets import WebSocketLink
+from rath.links.subscription_transport_ws import SubscriptionTransportWsLink
 
 
 class WebsocketHttpConfig(Fakt):
     ws_endpoint_url: str
 
     class Config:
         group = "aiohttp"
 
 
-class FaktsWebsocketLink(WebSocketLink):
+class FaktsWebsocketLink(SubscriptionTransportWsLink):
+    fakts: Fakts
     ws_endpoint_url: Optional[str]
     fakts_group: str = "websocket"
 
     _old_fakt: Dict[str, Any] = {}
 
     def configure(self, fakt: WebsocketHttpConfig) -> None:
         self.ws_endpoint_url = fakt.ws_endpoint_url
         self.token_loader = current_herre.get().aget_token
 
-    async def aconnect(self):
-        fakts = get_current_fakts()
-
-        if fakts.has_changed(self._old_fakt, self.fakts_group):
-            self._old_fakt = await fakts.aget(self.fakts_group)
+    async def aconnect(self, operation):
+        if self.fakts.has_changed(self._old_fakt, self.fakts_group):
+            self._old_fakt = await self.fakts.aget(self.fakts_group)
             self.configure(WebsocketHttpConfig(**self._old_fakt))
 
-        return await super().aconnect()
+        return await super().aconnect(operation)
```

### Comparing `rath-0.3.6/rath/links/aiohttp.py` & `rath-0.4.0/rath/links/aiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     """AIOHttpLink is a terminating link that sends operations over HTTP using aiohttp.
 
     Aiohttp is a Python library for asynchronous HTTP requests. This link uses the
     standard aiohttp library to send operations over HTTP, but provides an ssl context
     that is configured to use the certifi CA bundle by default. You can override this
     behavior by passing your own SSLContext to the constructor.
     """
+
     endpoint_url: str
     """endpoint_url is the URL to send operations to."""
     ssl_context: SSLContext = Field(
         default_factory=lambda: ssl.create_default_context(cafile=certifi.where())
     )
     """ssl_context is the SSLContext to use for the aiohttp session. By default, this
     is a context that uses the certifi CA bundle."""
@@ -47,25 +48,32 @@
     """auth_errors is a list of HTTPStatus codes that indicate that the request was
     unauthorized. By default, this is just HTTPStatus.FORBIDDEN, but you can
     override this to include other status codes that indicate that the request was
     unauthorized."""
 
     json_encoder: Type[json.JSONEncoder] = Field(default=DateTimeEncoder, exclude=True)
     """json_encoder is the JSONEncoder to use when serializing the payload. By default,
-    this is a DateTimeEncoder that extends the default python json decoder to serializes datetime objects to ISO 8601 strings."""
+    this is a DateTimeEncoder that extends the default python json decoder to serialize 
+    datetime objects to ISO 8601 strings."""
 
-    _session = None
+    _connected = False
 
     async def __aenter__(self) -> None:
-        self._session = await aiohttp.ClientSession().__aenter__()
+        pass
+
+    async def aconnect(self, operation: Operation):
+        self._connected = True
 
     async def __aexit__(self, *args, **kwargs) -> None:
-        await self._session.__aexit__(*args, **kwargs)
+        pass
 
     async def aexecute(self, operation: Operation) -> GraphQLResult:
+        if not self._connected:
+            await self.aconnect(operation)
+
         payload = {"query": operation.document}
 
         if operation.node.operation == OperationType.SUBSCRIPTION:
             raise NotImplementedError(
                 "Aiohttp Transport does not support subscriptions"
             )
 
@@ -104,15 +112,14 @@
         async with aiohttp.ClientSession(
             connector=aiohttp.TCPConnector(ssl=self.ssl_context),
             json_serialize=lambda x: json.dumps(x, cls=self.json_encoder),
         ) as session:
             async with session.post(
                 self.endpoint_url, headers=operation.context.headers, **post_kwargs
             ) as response:
-
                 if response.status == HTTPStatus.OK:
                     result = await response.json()
 
                 if response.status in self.auth_errors:
                     raise AuthenticationError(
                         f"Token Expired Error {operation.context.headers}"
                     )
@@ -121,15 +128,14 @@
 
                 if "errors" in json_response:
                     raise GraphQLException(
                         "\n".join([e["message"] for e in json_response["errors"]])
                     )
 
                 if "data" not in json_response:
-
                     raise Exception(f"Response does not contain data {json_response}")
 
                 yield GraphQLResult(data=json_response["data"])
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
```

### Comparing `rath-0.3.6/rath/links/auth.py` & `rath-0.4.0/rath/links/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import AsyncIterator, Awaitable, Callable, Optional
 
-from pydantic import Field
 from rath.links.base import ContinuationLink
 from rath.operation import GraphQLResult, Operation
 from rath.links.errors import AuthenticationError
 
 
 async def fake_loader():
     raise Exception("No Token loader specified")
@@ -16,52 +15,63 @@
     If the wrapped link raises an AuthenticationError, the token_refresher function
     is called again to refresh the token.
 
     This link is statelss, and does not store the token. It is up to the user to
     store the token and pass it to the token_loader function.
     """
 
-    token_loader: Callable[[], Awaitable[str]]
-    """The function used to load the authentication token. This function should
-        return a string containing the authentication token."""
-    token_refresher: Callable[[], Awaitable[str]]
-    """The function used to refresh the authentication token. This function should
-        return a string containing the authentication token."""
-
     maximum_refresh_attempts: int = 3
     """The maximum number of times the token_refresher function will be called, before the operation fails."""
 
     load_token_on_connect: bool = True
     """If True, the token_loader function will be called when the link is connected."""
     load_token_on_enter: bool = True
     """If True, the token_loader function will be called when the link is entered."""
 
-    async def aconnect(self):
-        if self.load_token_on_connect:
-            await self.token_loader()
+    async def aload_token(self):
+        raise Exception("No Token loader specified")
+
+    async def arefresh_token(self):
+        raise Exception("No Token refresher specified")
 
     async def aexecute(
         self, operation: Operation, retry=0, **kwargs
     ) -> AsyncIterator[GraphQLResult]:
+        token = await self.aload_token()
+        operation.context.headers["Authorization"] = f"Bearer {token}"
+        operation.context.initial_payload["token"] = token
 
-        operation.context.headers[
-            "Authorization"
-        ] = f"Bearer {await self.token_loader()}"
         try:
-
             async for result in self.next.aexecute(operation, **kwargs):
                 yield result
 
         except AuthenticationError as e:
             retry = retry + 1
-            operation.context.headers[
-                "Authorization"
-            ] = f"Bearer {await self.token_refresher()}"
+            await self.arefresh_token()
             if retry > self.maximum_refresh_attempts:
                 raise AuthenticationError("Maximum refresh attempts reached") from e
 
             async for result in self.aexecute(operation, retry=retry + 1, **kwargs):
                 yield result
 
     class Config:
         underscore_attrs_are_private = True
         arbitary_types_allowed = True
+
+
+class ComposedAuthLink(AuthTokenLink):
+    token_loader: Optional[Callable[[], Awaitable[str]]]
+    """The function used to load the authentication token. This function should
+        return a string containing the authentication token."""
+    token_refresher: Optional[Callable[[], Awaitable[str]]]
+    """The function used to refresh the authentication token. This function should
+        return a string containing the authentication token."""
+
+    async def aload_token(self):
+        if self.token_loader is None:
+            raise Exception("No Token loader specified")
+        return await self.token_loader()
+
+    async def arefresh_token(self):
+        if self.token_refresher is None:
+            raise Exception("No Token refresher specified")
+        return await self.token_refresher()
```

### Comparing `rath-0.3.6/rath/links/base.py` & `rath-0.4.0/rath/links/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class Link(KoiledModel):
     """A Link is a class that can be used to send operations to a GraphQL API.
     its main method is aexecute, which takes an operation and returns an
     AsyncIterator of GraphQLResults.
 
     Links can be composed to form a chain of links. The last link in the chain
     is the terminating link, which is responsible for sending the operation to
-    the server. 
+    the server.
 
     """
 
     async def aconnect(self):
         """A coroutine that is called when the link is connected."""
         pass
 
@@ -25,30 +25,29 @@
     async def __aenter__(self) -> None:
         pass
 
     async def __aexit__(self, *args, **kwargs) -> None:
         pass
 
     def aexecute(self, operation: Operation, **kwargs) -> AsyncIterator[GraphQLResult]:
-        """ A coroutine that takes an operation and returns an AsyncIterator of GraphQLResults.
-        This method should be implemented by subclasses."""
+        """A coroutine that takes an operation and returns an AsyncIterator
+        of GraphQLResults. This method should be implemented by subclasses."""
         raise NotImplementedError(
             f"Please overwrite the asubscribe method in {self.__class__.__name__}"
         )
 
 
 class TerminatingLink(Link):
     """A TerminatingLink is a link that is responsible for sending the operation to the server.
 
     The last link in a link chain MUST always a TerminatingLink. It cannot delegate the operation
     to another link.
     """
 
 
-
 class AsyncTerminatingLink(TerminatingLink):
     """An Async Termination Link
 
     This is a link that terminates the query or subscription, aka
     it is a link that does not have a next link. It normally
     is used to make network requests with the already parsed
     operations
@@ -59,16 +58,16 @@
 
     async def aexecute(self, operation: Operation) -> AsyncIterator[GraphQLResult]:
         raise NotImplementedError("Your Async Transport needs to overwrite this method")
 
 
 class ContinuationLink(Link):
     """A ContinuationLink is a link that delegates the operation to the next link in the chain.
-    It can be either provided a next link or it can be set once the link is composed together"""
-
+    It can be either provided a next link or it can be set once the link is composed together
+    """
 
     next: Optional[Link] = None
     """The next link in the chain. This is also set when the link is composed together."""
 
     def set_next(self, next: Link):
         self.next = next
```

### Comparing `rath-0.3.6/rath/links/compose.py` & `rath-0.4.0/rath/links/compose.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import List
 
-from pydantic import validator, root_validator
+from pydantic import validator
 from rath.links.base import ContinuationLink, Link, TerminatingLink
 from rath.operation import Operation
 
 
 class ComposedLink(TerminatingLink):
     """A composed link is a link that is composed of multiple links. The links
     are executed in the order they are passed to the constructor.
 
     The first link in the chain is the first link that is executed. The last
     link in the chain is the terminating link, which is responsible for sending
     the operation to the server.
     """
+
     links: List[Link]
-    """The links that are composed to form the chain. pydantic will validate that the last link is a terminating link."""
+    """The links that are composed to form the chain. pydantic will validate 
+    that the last link is a terminating link."""
 
     @validator("links")
     def validate(cls, value):
         if not value:
             raise ValueError("ComposedLink requires at least one link")
 
         if not all(isinstance(link, Link) for link in value):
@@ -39,15 +41,14 @@
             await link.aconnect()
 
     async def adisconnect(self):
         for link in self.links:
             await link.adisconnect()
 
     async def __aenter__(self):
-
         # We need to make sure that the links are connected in the correct order
         for i in range(len(self.links) - 1):
             self.links[i].set_next(self.links[i + 1])
 
         for link in self.links:
             await link.__aenter__()
 
@@ -63,28 +64,18 @@
 class TypedComposedLink(TerminatingLink):
     """A typed composed link is a base class to create a definition for
     a composed link. It is a link that is composed of multiple links that
     will be set at compile time and not at runtime. Just add links
     that you want to use to the class definition and they will be
     automatically composed together.
     """
-    _firstlink: Link = None
-
-    async def aconnect(self):
-        for key, link in self:
-            if isinstance(link, Link):
-                await link.aconnect()
 
-    async def adisconnect(self):
-        for key, link in self:
-            if isinstance(link, Link):
-                await link.adisconnect()
+    _firstlink: Link = None
 
     async def __aenter__(self):
-
         current_link = None
 
         for key, link in self:
             if isinstance(link, Link):
                 if current_link:
                     current_link.set_next(link)
                     await current_link.__aenter__()
@@ -98,25 +89,24 @@
 
     async def __aexit__(self, *args, **kwargs):
         for key, link in self:
             if isinstance(link, Link):
                 await link.__aexit__(*args, **kwargs)
 
     async def aexecute(self, operation: Operation, **kwargs):
-
         async for result in self._firstlink.aexecute(operation):
             yield result
 
     class Config:
         underscore_attrs_are_private = True
 
 
 def compose(*links: Link) -> ComposedLink:
     """Compose a chain of links together. The first link in the chain is the first link that is executed.
     The last link in the chain is the terminating link, which is responsible for sending the operation to the server.
 
 
     Returns:
         ComposedLink: The composed link
-    """   
+    """
 
     return ComposedLink(links=links)
```

### Comparing `rath-0.3.6/rath/links/dictinglink.py` & `rath-0.4.0/rath/links/dictinglink.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     return dicted_variables
 
 
 class DictingLink(ParsingLink):
     """Dicting Link is a link that converts pydantic models to dicts.
     It traversed the variables dict, and converts any (nested) pydantic models to dicts
     by callind their .json() method."""
+
     by_alias = True
     """Converts pydantic models to dicts by calling their .json() method with by_alias=True"""
-    
-
-
 
     async def aparse(self, operation: Operation) -> Operation:
-        shrinked_variables = parse_variables(operation.variables, by_alias=self.by_alias)
+        shrinked_variables = parse_variables(
+            operation.variables, by_alias=self.by_alias
+        )
         operation.variables.update(shrinked_variables)
         return operation
```

### Comparing `rath-0.3.6/rath/links/errors.py` & `rath-0.4.0/rath/links/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from rath.errors import RathException
 
 
 class LinkError(RathException):
     """Base class for all link errors."""
 
 
-
 class LinkNotConnectedError(LinkError):
     """LinkNotConnectedError is raised when the link is not connected and autoload is set to false."""
 
     pass
 
     def __init__(self, message) -> None:
         super().__init__(
@@ -18,14 +17,13 @@
         )
 
 
 class TerminatingLinkError(LinkError):
     """Raised when a terminating link is called."""
 
 
-
 class ContinuationLinkError(LinkError):
     pass
 
 
 class AuthenticationError(TerminatingLinkError):
     pass
```

### Comparing `rath-0.3.6/rath/links/file.py` & `rath-0.4.0/rath/links/file.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/rath/links/httpx.py` & `rath-0.4.0/rath/links/httpx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from datetime import datetime
 from http import HTTPStatus
 import json
-from ssl import SSLContext
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List
 import httpx
-import aiohttp
 from graphql import OperationType
 from pydantic import Field
 from rath.operation import GraphQLException, GraphQLResult, Operation
 from rath.links.base import AsyncTerminatingLink
 from rath.links.errors import AuthenticationError
 import logging
-import certifi
-import ssl
 
 logger = logging.getLogger(__name__)
 
 
 class HttpxLink(AsyncTerminatingLink):
     """HttpxLink is a terminating link that sends operations over HTTP using httpx"""
 
@@ -75,24 +70,22 @@
 
         if response.status_code in self.auth_errors:
             raise AuthenticationError(
                 f"Token Expired Error {operation.context.headers}"
             )
 
         if response.status_code == HTTPStatus.OK:
-
             json_response = response.json()
 
             if "errors" in json_response:
                 raise GraphQLException(
                     "\n".join([e["message"] for e in json_response["errors"]])
                 )
 
             if "data" not in json_response:
-
                 raise Exception(f"Response does not contain data {json_response}")
 
             yield GraphQLResult(data=json_response["data"])
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
```

### Comparing `rath-0.3.6/rath/links/parsing.py` & `rath-0.4.0/rath/links/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from rath.links.base import ContinuationLink
 from rath.operation import Operation
 
 
 class ParsingLink(ContinuationLink):
-    """ ParsingLink is a link that parses operation and returns a new operation.
+    """ParsingLink is a link that parses operation and returns a new operation.
     It is an abstract class that needs to be implemented by the user.
     """
 
-
     async def aparse(self, operation: Operation) -> Operation:
         raise NotImplementedError("Please implement this method")
 
     async def aexecute(self, operation: Operation, **kwargs) -> Operation:
         operation = await self.aparse(operation)
         async for result in self.next.aexecute(operation, **kwargs):
             yield result
```

### Comparing `rath-0.3.6/rath/links/retry.py` & `rath-0.4.0/rath/links/retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     """The maximum number of times the operation function will be called, before the operation fails."""
     sleep_interval: Optional[int]
     """The number of seconds to wait before retrying the operation."""
 
     async def aexecute(
         self, operation: Operation, retry=0, **kwargs
     ) -> AsyncIterator[GraphQLResult]:
-
         try:
-
             async for result in self.next.aexecute(operation, **kwargs):
                 yield result
 
         except SubscriptionDisconnect as e:
             if retry > self.maximum_retry_attempts:
                 raise GraphQLException(
                     "Maximum refresh attempts reached. Trying to rescribe to"
```

### Comparing `rath-0.3.6/rath/links/shrink.py` & `rath-0.4.0/rath/links/shrink.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         return self.id
 
     def shrink(self):
         return self.id
 
 
 class ShrinkingLink(ParsingLink):
-    
+
     """Shrinking Link is a link that shrinks operation variables.
     It traverses the variables dict, and converts any model that has a .ashrink() method to its id."""
 
     async def aparse(self, operation: Operation) -> Operation:
 
         shrinked_variables = {
             key: await var.ashrink()
```

### Comparing `rath-0.3.6/rath/links/split.py` & `rath-0.4.0/rath/links/split.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from pydantic import Field
 from rath.operation import Operation
 from rath.links.base import TerminatingLink
 
 
 class SplitLink(TerminatingLink):
     """SplitLink is a link that splits the operation into two paths. The operation is sent to the left path if the predicate returns true, otherwise to the right path.
-    
+
     This is useful for exampole when implementing a cache link, where the operation is sent to the cache if it is a query, and to the network if it is a mutation.
-    Or when subscriptions and queries are sent to different links (e.g. a websocket link and a http link)."""
+    Or when subscriptions and queries are sent to different links (e.g. a websocket link and a http link).
+    """
+
     left: TerminatingLink
     """The link that is used if the predicate returns true."""
     right: TerminatingLink
     """The link that is used if the predicate returns false."""
     split: Callable[[Operation], bool] = Field(exclude=True)
     """The function used to split the operation. This function should return a boolean. If true, the operation is sent to the left path, otherwise to the right path."""
 
@@ -23,22 +25,14 @@
             if self.split(operation)
             else self.right.aexecute(operation, **kwargs)
         )
 
         async for res in iterator:
             yield res
 
-    async def aconnect(self):
-        await self.left.aconnect()
-        await self.right.aconnect()
-
-    async def adisconnect(self):
-        await self.left.adisconnect()
-        await self.right.adisconnect()
-
     async def __aenter__(self):
         await self.left.__aenter__()
         await self.right.__aenter__()
 
     async def __aexit__(self, *args, **kwargs):
         await self.left.__aexit__(*args, **kwargs)
         await self.right.__aexit__(*args, **kwargs)
```

### Comparing `rath-0.3.6/rath/links/testing/mock.py` & `rath-0.4.0/rath/links/testing/mock.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/rath/links/testing/statefulmock.py` & `rath-0.4.0/rath/links/testing/statefulmock.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     subscription_resolver: Dict[str, Callable[[Operation], Awaitable[Dict]]] = Field(
         default_factory=dict, exclude=True
     )
     resolver: Dict[str, Callable[[Operation], Awaitable[Dict]]] = Field(
         default_factory=dict, exclude=True
     )
 
+    _connection_lock: asyncio.Lock = None
     _connected: bool = False
     _futures: Optional[Dict[str, asyncio.Future]] = None
     _inqueue: Optional[asyncio.Queue] = None
     _connection_task: Optional[asyncio.Task] = None
 
     @validator(
         "query_resolver",
@@ -68,40 +69,46 @@
     )
     @classmethod
     def coerce_resolver(cls, v):
         if isinstance(v, AsyncMockResolver):
             return v.to_dict()
         return v
 
+    async def __aenter__(self) -> None:
+        self._connection_lock = asyncio.Lock()
+        return await super().__aenter__()
+
     async def aconnect(self):
         self._futures = {}
         self._inqueue = asyncio.Queue()
-        self._connection_task = asyncio.create_task(self.resolving())
-        self._connected = True
+        _connection_future = asyncio.Future()
+        self._connection_task = asyncio.create_task(self.resolving(_connection_future))
+        await _connection_future
 
     async def adisconnect(self):
         self._connection_task.cancel()
         self._connected = False
 
         try:
             await self._connection_task
         except asyncio.CancelledError:
             pass
 
     async def __aexit__(self, *args, **kwargs) -> None:
         if self._connection_task:
             await self.adisconnect()
 
-    async def resolving(self):
+    async def resolving(self, connection_future: asyncio.Future):
         """A coroutine that resolves the incoming operations in
         an inifite Loop
 
         Raises:
             NotImplementedError: If the operation is not supported (aka not implemented)
         """
+        connection_future.set_result(True)
         while True:
             operation, id = await self._inqueue.get()
 
             resolve_futures = []
 
             try:
                 if operation.node.operation == OperationType.QUERY:
@@ -112,30 +119,32 @@
                             )
                         elif op.name.value in self.resolver:
                             resolve_futures.append(
                                 self.resolver[op.name.value](operation)
                             )
                         else:
                             raise NotImplementedError(
-                                f"Mocked Resolver for Query '{op.name.value}' not in resolvers: {self.query_resolver}, {self.resolver}  for AsyncMockLink"
+                                f"Mocked Resolver for Query '{op.name.value}' not in resolvers"
+                                f": {self.query_resolver}, {self.resolver}  for AsyncMockLink"
                             )
 
                 if operation.node.operation == OperationType.MUTATION:
                     for op in operation.node.selection_set.selections:
                         if op.name.value in self.mutation_resolver:
                             resolve_futures.append(
                                 self.mutation_resolver[op.name.value](operation)
                             )
                         elif op.name.value in self.resolver:
                             resolve_futures.append(
                                 self.resolver[op.name.value](operation)
                             )
                         else:
                             raise NotImplementedError(
-                                f"Mocked Resolver for Query '{op.name.value}' not in resolvers: {self.mutation_resolver}, {self.resolver}  for AsyncMockLink"
+                                f"Mocked Resolver for Query '{op.name.value}' not in resolvers:"
+                                f"{self.mutation_resolver}, {self.resolver}  for AsyncMockLink"
                             )
                 resolved = await asyncio.gather(*resolve_futures)
 
                 self._futures[id].set_result(
                     GraphQLResult(
                         data={
                             target_from_node(op): resolved[i]
@@ -153,16 +162,17 @@
 
             self._inqueue.task_done()
 
     async def submit(self, o, id):
         await self._inqueue.put((o, id))
 
     async def aexecute(self, operation: Operation) -> AsyncIterator[GraphQLResult]:
-        if not self._connected:
-            raise TerminatingLinkError("Not connected")
+        async with self._connection_lock:
+            if not self._connected:
+                await self.aconnect()
 
         if (
             operation.node.operation == OperationType.QUERY
             or operation.node.operation == OperationType.MUTATION
         ):
             uniqueid = uuid.uuid4()
             self._futures[uniqueid] = asyncio.Future()
```

### Comparing `rath-0.3.6/rath/links/transpile.py` & `rath-0.4.0/rath/links/transpile.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     VariableNode,
 )
 from pydantic import BaseModel, Field
 from rath.links.parsing import ParsingLink
 from rath.operation import Operation
 import logging
 
-logger = logging.getLogger(__name__)
-
 
 class TranspileHandler(BaseModel):
     """A Transpilation Handler
 
     A TranspileHandler is a function that takes any Any and returns a
     GraphQLType. It is used to implement custom type resolution.
 
@@ -130,15 +128,15 @@
                 return [InputVector(x) for x in x]
             ```
         Args:
             graphql_type (str): The graphql Type to act upon
             predicate (Callable[[Any], bool]): A predicate Function
             handle_list (bool, optional): Should we act on lists of this type. Defaults to False.
             name (_type_, optional): A name for this hanlder. Defaults to the function name.
-        """
+        """  # noqa: E501
 
         def decorator(func):
             """The decorator function
 
             Args:
                 func (_type_): The function to use as a handler
 
@@ -169,15 +167,16 @@
     its definition
 
     Args:
         key (_type_): The key of the variable
         var (VariableNode): The variable definition node correspoin to this variable
         value (Any): The to transpile valued
         registry (TranspileRegistry): The transpile registry to use
-        in_list (bool, optional): Recursive Parameter. That will be set to the list depth. Defaults to False.
+        in_list (bool, optional): Recursive Parameter. That will be set to the list depth.
+                                 Defaults to False.
         strict (bool, optional): Should we error on predicate errors. Defaults to False.
 
     Raises:
         TranspilationError: _description_
 
     Returns:
         Any: The transpiled value or the original value if no handler matched
@@ -200,23 +199,24 @@
                             predicate = handler.predicate(value, in_list)
                         except Exception as e:
                             if strict:
                                 raise TranspilationHandlerException(
                                     f"Handler {handler} predicate failed"
                                 ) from e
                             logger.warning(
-                                f"Handler {handler} failed on predicating {value}. Please check your predicate for edge cases"
+                                f"Handler {handler} failed on predicating {value}."
+                                "Please check your predicate for edge cases"
                             )
                             continue
 
                         if predicate:
                             parsed_value = handler.parser(value, in_list)
                             assert (
                                 parsed_value is not None
-                            ), f"Handler {handler} failed on parsing {value}. Please check your parser for edge cases"
+                            ), f"Handler {handler} failed on parsing {value} Please check your parser for edge cases"
                             return parsed_value
 
                 return value
 
             else:
                 if var.name.value in registry.item_handlers:
                     for k, handler in registry.item_handlers[var.name.value].items():
@@ -255,15 +255,16 @@
 
     Transpiles a operations variabels to a dictionary of variables, with
     json serializable values according to a transpile registry.
 
     Args:
         op (OperationDefinitionNode): The operation definition node,
         registry (TranspileRegistry): The registry
-        strict (bool, optional): Should we fail if a handler predicate fails. Defaults to False.
+        strict (bool, optional): Should we fail if a handler predicate fails. Defaults
+        to False.
 
     Returns:
         Dict: The transpiled variables
     """
     variable_nodes = {
         var_node.variable.name.value: var_node.type
         for var_node in op.variable_definitions
```

### Comparing `rath-0.3.6/rath/links/utils.py` & `rath-0.4.0/rath/links/utils.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/rath/links/validate.py` & `rath-0.4.0/rath/links/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,17 @@
 
 class ValidatingLink(ContinuationLink):
     """ValidatingLink validates the operation againt as schema before passing it on to the next link.
 
     The schema can be provided as a dsl string, or as a glob to a set of graphql files.
     If the schema is not provided, the link will introspect the server to get the schema if allow_introspection is set to True.
 
-    
+
     """
+
     schema_dsl: Optional[str] = None
     """ The schema (as a string) to validate against. If not provided, the link will introspect the server to get the schema if allow_introspection is set to True."""
     schema_glob: Optional[str] = None
     """ The glob to a set of graphql files to validate against. If not provided, the link will introspect the server to get the schema if allow_introspection is set to True."""
     allow_introspection: bool = False
     """ If set to True, the link will introspect the server to get the schema if it is not provided."""
```

### Comparing `rath-0.3.6/rath/links/websockets.py` & `rath-0.4.0/rath/links/graphql_ws.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pydantic import Field
 import websockets
 import json
 import asyncio
 from websockets.exceptions import (
     ConnectionClosedError,
 )
+import asyncio
 import logging
 import uuid
 import ssl
 import certifi
 from rath.links.errors import LinkNotConnectedError, TerminatingLinkError
 
 from rath.operation import (
@@ -36,14 +37,17 @@
 GQL_CONNECTION_ERROR = "connection_error"
 GQL_CONNECTION_ACK = "connection_ack"
 GQL_DATA = "data"
 GQL_ERROR = "error"
 GQL_COMPLETE = "complete"
 GQL_CONNECTION_KEEP_ALIVE = "ka"
 
+GQL_PING = "ping"
+GQL_PONG = "pong"
+
 WEBSOCKET_DEAD = "websocket_dead"
 WEBSOCKET_CANCELLED = "websocket_cancelled"
 
 
 class CorrectableConnectionFail(TerminatingLinkError):
     pass
 
@@ -52,20 +56,22 @@
     pass
 
 
 class InvalidPayload(TerminatingLinkError):
     pass
 
 
-async def none_token_loader():
-    raise Exception("Token loader was not set")
+async def default_pong_handler(payload):
+    return payload
 
 
-class WebSocketLink(AsyncTerminatingLink):
-    """WebSocketLink is a terminating link that sends operations over websockets using websockets
+class GraphQLWSLink(AsyncTerminatingLink):
+    """GraphQLWSLink is a terminating link that sends operations over websockets using
+      websockets via the graphql-ws protocol. This is a
+      new standard protocol, and should not be used for new projects.
 
     This is a terminating link, so it should be the last link in the chain.
     This is a stateful link, keeing a connection open and sending messages over it.
 
     """
 
     ws_endpoint_url: str
@@ -75,71 +81,89 @@
     time_between_retries = 4
     """ The sleep time between retries """
     max_retries = 3
     """ The maximum amount of retries before giving up """
     ssl_context: SSLContext = Field(
         default_factory=lambda: ssl.create_default_context(cafile=certifi.where())
     )
-    """ The SSL Context to use for the connection """
-    token_loader: Callable[[], Awaitable[str]] = Field(
-        default_factory=lambda: none_token_loader, exclude=True
-    )
-    """ A function that returns the token to use for the connection as a query parameter """
 
+    on_connect: Optional[Callable[[], Awaitable[None]]] = Field(exclude=True)
+    on_pong: Optional[Callable[[], Awaitable[None]]] = Field(
+        default=default_pong_handler, exclude=True
+    )
+    """ A function that is called when the connection is established """
+    heartbeat_interval_ms: Optional[int] = None
+    """ The heartbeat interval in milliseconds (None means no heartbeats are 
+    being send) """
 
+    _connection_lock: Optional[asyncio.Lock] = None
     _connected: bool = False
     _alive: bool = False
     _send_queue: asyncio.Queue = None
     _connection_task: asyncio.Task = None
     _ongoing_subscriptions: Optional[Dict[str, asyncio.Queue]] = None
 
     async def aforward(self, message):
         await self._send_queue.put(message)
 
     async def __aenter__(self):
         self._ongoing_subscriptions = {}
+        self._connection_lock = asyncio.Lock()
         self._send_queue = asyncio.Queue()
 
-    async def aconnect(self):
+    async def aconnect(self, operation: Operation):
         logger.info("Connecting Websockets")
-        self._connection_task = asyncio.create_task(self.websocket_loop())
-        self._connected = True
+        initial_connection_future = asyncio.get_running_loop().create_future()
+        self._connection_task = asyncio.create_task(
+            self.websocket_loop(operation, initial_connection_future)
+        )
+        await initial_connection_future
 
     async def adisconnect(self):
         self._connection_task.cancel()
 
         try:
             await self._connection_task
         except asyncio.CancelledError:
-            logger.info(f"Websocket Transport {self} succesfully disconnected")
+            logger.info(f"Websocket Transport succesfully disconnected")
 
     async def __aexit__(self, *args, **kwargs):
         if self._connection_task:
             await self.adisconnect()
 
-    async def websocket_loop(self, retry=0):
+    async def abuild_url(self):
+        return self.ws_endpoint_url
+
+    async def websocket_loop(
+        self,
+        initiating_operation: Operation,
+        initial_connection_future: asyncio.Future,
+        retry=0,
+    ):
         send_task = None
         receive_task = None
         try:
             try:
-                token = await self.token_loader()
-                url = (
-                    f"{self.ws_endpoint_url}?token={token}"
-                    if token
-                    else self.ws_endpoint_url
-                )
+                url = await self.abuild_url()
                 async with websockets.connect(
                     url,
                     subprotocols=[GQL_WS_SUBPROTOCOL],
                     ssl=self.ssl_context if url.startswith("wss") else None,
                 ) as client:
                     logger.info("Websocket successfully connected")
 
-                    send_task = asyncio.create_task(self.sending(client))
-                    receive_task = asyncio.create_task(self.receiving(client))
+                    send_task = asyncio.create_task(
+                        self.sending(
+                            client,
+                            initiating_operation,
+                        )
+                    )
+                    receive_task = asyncio.create_task(
+                        self.receiving(client, initial_connection_future)
+                    )
 
                     self._alive = True
                     done, pending = await asyncio.wait(
                         [send_task, receive_task],
                         return_when=asyncio.FIRST_EXCEPTION,
                     )
                     self._alive = False
@@ -184,74 +208,88 @@
             raise e
 
         except Exception as e:
             logger.error("Websocket excepted", exc_info=True)
             self.connection_dead = True
             raise e
 
-    async def sending(self, client, headers=None):
-        payload = {"type": GQL_CONNECTION_INIT, "payload": {"headers": headers}}
+    async def sending(self, client, initiating_operation: Operation):
+        payload = {
+            "type": GQL_CONNECTION_INIT,
+            "payload": initiating_operation.context.initial_payload,
+        }
         await client.send(json.dumps(payload))
 
         try:
             while True:
                 message = await self._send_queue.get()
                 logger.debug("GraphQL Websocket: >>>>>> " + message)
                 await client.send(message)
                 self._send_queue.task_done()
         except asyncio.CancelledError as e:
             logger.debug("Sending Task sucessfully Cancelled")  #
             raise e
 
-    async def receiving(self, client):
+    async def receiving(self, client, initial_connection_future: asyncio.Future):
         try:
             async for message in client:
                 logger.debug("GraphQL Websocket: <<<<<<< " + message)
                 try:
                     message = json.loads(message)
-                    await self.broadcast(message)
+                    await self.broadcast(message, initial_connection_future)
                 except json.JSONDecodeError as err:
                     logger.warning(
                         "Ignoring. Server sent invalid JSON data: %s \n %s",
                         message,
                         err,
                     )
         except Exception as e:
             logger.warning("Websocket excepted. Trying to recover", exc_info=True)
             raise e
 
-    async def broadcast(self, message: dict):
+    async def broadcast(self, message: dict, initial_connection_future: asyncio.Future):
         type = message["type"]
 
-        if type == GQL_CONNECTION_KEEP_ALIVE:
+        if type == GQL_CONNECTION_ACK:
+            if self.on_connect:
+                await self.on_connect(message.get("payload", {}))
+            initial_connection_future.set_result(True)
             return
 
+        if type == GQL_PING:
+            if self.on_pong:
+                payload = await self.on_pong(message.get("payload", {}))
+            else:
+                payload = message.get("payload", {})
+            await self.aforward(json.dumps({"type": GQL_PONG, "payload": payload}))
+
         if type == GQL_CONNECTION_KEEP_ALIVE:
             return
 
         if type == WEBSOCKET_DEAD:
             # notify all subscriptipns that the websocket is dead
             for subscription in self._ongoing_subscriptions.values():
                 await subscription.put(message)
             return
 
-        if type in [GQL_DATA, GQL_COMPLETE]:
-
+        if type in [GQL_DATA, GQL_COMPLETE, GQL_ERROR]:
             if "id" not in message:
                 raise InvalidPayload(f"Protocol Violation. Expected 'id' in {message}")
 
             id = message["id"]
             assert (
                 id in self._ongoing_subscriptions
             ), "Received Result for subscription that is no longer or was never active"
             await self._ongoing_subscriptions[id].put(message)
 
     async def aexecute(self, operation: Operation):
-        if self._connection_task == False:
-            raise LinkNotConnectedError("Websocket_link is not connected")
+        async with self._connection_lock:
+            if self._connection_task is None or self._connection_task.done():
+                # we need to start a new connection
+                await self.aconnect(operation)
 
         assert (
             operation.node.operation == OperationType.SUBSCRIPTION
         ), "Operation is not a subscription"
         assert not operation.context.files, "We cannot send files through websockets"
 
         id = operation.id
@@ -268,14 +306,25 @@
             frame = {"id": id, "type": GQL_START, "payload": payload}
             await self.aforward(json.dumps(frame))
             logger.debug(f"Subcription started {operation}")
 
             while True:
                 answer = await subscribe_queue.get()
 
+                if answer["type"] == GQL_ERROR:
+                    payload = answer["payload"]
+                    if isinstance(payload, list):
+                        error_list = payload
+                    else:
+                        error_list = [payload]
+
+                    raise GraphQLException(
+                        "\n".join([e["message"] for e in error_list])
+                    )
+
                 if answer["type"] == GQL_DATA:
                     payload = answer["payload"]
 
                     if "errors" in payload:
                         raise GraphQLException(
                             "\n".join([e["message"] for e in payload["errors"]])
                         )
@@ -294,11 +343,10 @@
                     return
 
         except asyncio.CancelledError as e:
             logger.debug(f"Subcription ended {operation}")
             await self.aforward(json.dumps({"id": id, "type": GQL_STOP}))
             raise e
 
-
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
```

### Comparing `rath-0.3.6/rath/operation.py` & `rath-0.4.0/rath/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from typing import Optional, Dict, Any, Union
-from graphql.language import OperationDefinitionNode, parse
+from graphql.language import OperationDefinitionNode, parse, OperationType
 from graphql import (
     DocumentNode,
     get_operation_ast,
     parse,
 )
 from pydantic import BaseModel, Field
 import uuid
 
 
 class Context(BaseModel):
     """Context provides a way to pass arbitrary data to resolvers on the context"""
+
     headers: Optional[Dict[str, str]] = Field(default_factory=dict)
     files: Optional[Dict[str, Any]] = Field(default_factory=dict)
+    initial_payload: Optional[Dict[str, Any]] = Field(default_factory=dict)
     kwargs: Optional[Dict[str, Any]] = Field(default_factory=dict)
 
 
 class Extensions(BaseModel):
-    """ Extensions is a map of additional metadata that can be used by the links in the chain"""
+    """Extensions is a map of additional metadata that can be used by the links in the chain"""
+
     pollInterval: Optional[int] = None
     maxPolls: Optional[int] = None
 
 
 class Operation(BaseModel):
     """A GraphQL operation.
-    
+
     An Operation is a GraphQL operation that can be executed by a GraphQL client.
     It is a combination of a query, variables, and headers, as well as a context
     that can be used to pass additional information to the link chain and
     extensions that can be used to pass additional information to the server.
     """
 
-
     id: str = Field(default_factory=lambda: str(uuid.uuid4()))
     document_node: DocumentNode
     node: OperationDefinitionNode
     document: str
     variables: Dict[str, Any]
     operation_name: Optional[str]
     extensions: Extensions
@@ -43,19 +45,21 @@
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class GraphQLResult(BaseModel):
     """GraphQLResult is the result of a GraphQL operation."""
+
     data: Dict[str, Any]
 
 
 class GraphQLException(Exception):
     """GraphQLException is the base exception for all GraphQL errors."""
+
     pass
 
 
 class SubscriptionDisconnect(GraphQLException):
     pass
```

### Comparing `rath-0.3.6/rath/qt/helpers.py` & `rath-0.4.0/rath/qt/helpers.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/rath/rath.py` & `rath-0.4.0/rath/rath.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DocumentNode,
 )
 from rath.operation import GraphQLResult, opify
 from contextvars import ContextVar
 from koil import unkoil_gen, unkoil
 
 
-current_rath = ContextVar("current_rath")
+current_rath = ContextVar("current_rath_unpicklable")
 
 
 class Rath(KoiledModel):
     """A Rath is a client for a GraphQL API.
 
     Links are used to define the transport logic of the Rath. A Rath can be
     connected to a GraphQL API using a terminating link. By composing links to
@@ -45,59 +45,28 @@
         rath = Rath(link=compose(retry, link))
         async with rath as rath:
             await rath.aquery(...)
         ```
 
     """
 
-
-
-
     link: Optional[TerminatingLink] = None
     """The terminating link used to send operations to the server. Can be a composed link chain."""
 
     _connected = False
     _entered = False
     _context_token = None
-    auto_connect = True
-    """If true, the Rath will automatically connect to the server when a query is executed."""
-    connect_on_enter: bool = False
     """If true, the Rath will automatically connect to the server when entering the context manager."""
 
-    async def aconnect(self):
-        """Connect to the server.
-
-        This method needs to be called within the context of a Rath instance,
-        to always ensure that the Rath is disconnected when the context is
-        exited.
-
-        This method is called automatically when a query is executed if
-        `auto_connect` is set to True. 
-
-        Raises:
-            NotEnteredError: Raises an error if the Rath is not entered.
-        """
-        if not self._entered:
-            raise NotEnteredError(
-                "You need to use enter `async with Rath(...) as rath`"
-            )
-        await self.link.aconnect()
-        self._connected = True
-
-    async def adisconnect(self):
-        """Disconnect from the server."""
-        await self.link.adisconnect()
-        self._connected = False
-
     async def aquery(
         self,
         query: Union[str, DocumentNode],
         variables: Dict[str, Any] = None,
         headers: Dict[str, Any] = None,
-        operation_name: str =None,
+        operation_name: str = None,
         **kwargs,
     ) -> GraphQLResult:
         """Query the GraphQL API.
 
         Takes a querystring, variables, and headers and returns the result.
         If provided, the operation_name will be used to identify which operation
         to execute.
@@ -111,34 +80,25 @@
 
         Raises:
             NotConnectedError: An error when the Rath is not connected and autoload is set to false
 
         Returns:
             GraphQLResult: The result of the query
         """
-
-
-        if not self._connected:
-            if not self.auto_connect:
-                raise NotConnectedError(
-                    "Rath is not connected. Please use `async with Rath(..., auto_connect=True) as rath` or use `await rath.aconnect() before`"
-                )
-            await self.aconnect()
-
         op = opify(query, variables, headers, operation_name, **kwargs)
 
         async for data in self.link.aexecute(op):
             return data
 
     def query(
         self,
         query: Union[str, DocumentNode],
         variables: Dict[str, Any] = None,
         headers: Dict[str, Any] = None,
-        operation_name: str =None,
+        operation_name: str = None,
         **kwargs,
     ) -> GraphQLResult:
         """Query the GraphQL API.
 
         Takes a querystring, variables, and headers and returns the result.
         If provided, the operation_name will be used to identify which operation
         to execute.
@@ -159,15 +119,15 @@
         return unkoil(self.aquery, query, variables, headers, operation_name, **kwargs)
 
     def subscribe(
         self,
         query: str,
         variables: Dict[str, Any] = None,
         headers: Dict[str, Any] = None,
-        operation_name: str =None,
+        operation_name: str = None,
         **kwargs,
     ) -> Iterator[GraphQLResult]:
         """Subscripe to a GraphQL API.
 
         Takes a querystring, variables, and headers and returns an async iterator
         that yields the results.
 
@@ -179,15 +139,15 @@
             **kwargs: Additional arguments to pass to the link chain
 
         Raises:
             NotConnectedError: An error when the Rath is not connected and autoload is set to false
 
         Yields:
             Iterator[GraphQLResult]: The result of the query as an async iterator
-        """ 
+        """
         return unkoil_gen(
             self.asubscribe, query, variables, headers, operation_name, **kwargs
         )
 
     async def asubscribe(
         self,
         query: str,
@@ -209,41 +169,27 @@
             **kwargs: Additional arguments to pass to the link chain
 
         Raises:
             NotConnectedError: An error when the Rath is not connected and autoload is set to false
 
         Yields:
             Iterator[GraphQLResult]: The result of the query as an async iterator
-        """        """"""
-        if not self._connected:
-            if not self.auto_connect:
-                raise NotConnectedError(
-                    "Rath is not connected. Please use `async with Rath(..., auto_connect=True) as rath` or use `await rath.aconnect() before`"
-                )
-            await self.aconnect()
+        """
 
         op = opify(query, variables, headers, operation_name, **kwargs)
         async for data in self.link.aexecute(op):
             yield data
 
     async def __aenter__(self):
         self._entered = True
         self._context_token = current_rath.set(self)
         await self.link.__aenter__()
         return self
 
     async def __aexit__(self, *args, **kwargs):
-        if self._connected:
-            await self.adisconnect()
-
         await self.link.__aexit__(*args, **kwargs)
         self._entered = False
         if self._context_token:
             current_rath.set(None)
 
-    
-
     class Config:
         underscore_attrs_are_private = True
-
-
-
```

### Comparing `rath-0.3.6/rath/scalars.py` & `rath-0.4.0/rath/scalars.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/rath/turms/funcs.py` & `rath-0.4.0/rath/turms/funcs.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/rath/turms/plugins/funcs.py` & `rath-0.4.0/rath/turms/plugins/funcs.py`

 * *Files identical despite different names*

### Comparing `rath-0.3.6/PKG-INFO` & `rath-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: rath
-Version: 0.3.6
+Version: 0.4.0
 Summary: async transport-agnostic graphql client
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aiohttp
 Provides-Extra: httpx
 Provides-Extra: websockets
-Requires-Dist: aiohttp (>=3.8.2,<4.0.0); extra == "aiohttp"
-Requires-Dist: certifi (>2021); extra == "aiohttp"
+Requires-Dist: aiohttp (>=3.8.2,<4.0.0) ; extra == "aiohttp"
+Requires-Dist: certifi (>2021) ; extra == "aiohttp"
 Requires-Dist: graphql-core (>=3.2.0,<4.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0); extra == "httpx"
-Requires-Dist: koil (>=0.2.10)
+Requires-Dist: httpx (>=0.23.0,<0.24.0) ; extra == "httpx"
+Requires-Dist: koil (==0.3.3)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
-Requires-Dist: websockets (>=10.2,<11.0); extra == "websockets"
+Requires-Dist: websockets (>=10.2,<11.0) ; extra == "websockets"
 Description-Content-Type: text/markdown
 
 # rath
 
 [![codecov](https://codecov.io/gh/jhnnsrs/rath/branch/master/graph/badge.svg?token=UGXEA2THBV)](https://codecov.io/gh/jhnnsrs/rath)
 [![PyPI version](https://badge.fury.io/py/rath.svg)](https://pypi.org/project/rath/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://pypi.org/project/rath/)
```

