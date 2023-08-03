# Comparing `tmp/aiomqtt-1.0.0.tar.gz` & `tmp/aiomqtt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomqtt-1.0.0.tar", max compression
+gzip compressed data, was "aiomqtt-1.1.0.tar", max compression
```

## Comparing `aiomqtt-1.0.0.tar` & `aiomqtt-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1464 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/LICENSE
--rw-r--r--   0        0        0     7157 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/README.md
--rw-r--r--   0        0        0      529 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/__init__.py
--rw-r--r--   0        0        0    35189 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/client.py
--rw-r--r--   0        0        0     1686 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/error.py
--rw-r--r--   0        0        0        0 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/py.typed
--rw-r--r--   0        0        0      245 2023-06-16 16:47:32.056140 aiomqtt-1.0.0/aiomqtt/types.py
--rw-r--r--   0        0        0     4800 2023-06-16 16:48:01.404595 aiomqtt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 aiomqtt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1464 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6585 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/README.md
+-rw-r--r--   0        0        0      529 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/aiomqtt/__init__.py
+-rw-r--r--   0        0        0    41844 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/aiomqtt/client.py
+-rw-r--r--   0        0        0     1686 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/aiomqtt/error.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/aiomqtt/py.typed
+-rw-r--r--   0        0        0      245 2023-08-03 12:43:23.226921 aiomqtt-1.1.0/aiomqtt/types.py
+-rw-r--r--   0        0        0     4864 2023-08-03 12:43:56.671048 aiomqtt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 aiomqtt-1.1.0/PKG-INFO
```

### Comparing `aiomqtt-1.0.0/LICENSE` & `aiomqtt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomqtt-1.0.0/README.md` & `aiomqtt-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,52 +4,49 @@
     <a href="https://github.com/sbtinstruments/aiomqtt/blob/main/LICENSE"><img alt="License: BSD-3-Clause" src="https://img.shields.io/github/license/sbtinstruments/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI version" src="https://img.shields.io/pypi/v/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="Supported Python versions" src="https://img.shields.io/pypi/pyversions/aiomqtt.svg"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI downloads" src="https://img.shields.io/pypi/dm/aiomqtt"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml"><img alt="test" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml/badge.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml"><img alt="docs" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/sbtinstruments/aiomqtt"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/sbtinstruments/aiomqtt"></a>
-    <a href="https://results.pre-commit.ci/latest/github/sbtinstruments/aiomqtt/main"><img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/sbtinstruments/aiomqtt/main.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Typing: strict" src="https://img.shields.io/badge/typing-strict-green.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black"></a>
     <a href="https://github.com/charliermarsh/ruff"><img alt="Ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json"></a>
 </p>
 
 <!-- pitch start -->
 
 Write code like this:
 
-**Publisher**
+**Publish**
 
 ```python
 async with Client("test.mosquitto.org") as client:
     await client.publish("humidity/outside", payload=0.38)
 ```
 
-**Subscriber**
+**Subscribe**
 
 ```python
 async with Client("test.mosquitto.org") as client:
     async with client.messages() as messages:
         await client.subscribe("humidity/#")
         async for message in messages:
             print(message.payload)
 ```
 
-aiomqtt combines the stability of the time-proven [paho-mqtt](https://github.com/eclipse/paho.mqtt.python) library with a modern, asyncio-based interface.
+aiomqtt combines the stability of the time-proven [paho-mqtt](https://github.com/eclipse/paho.mqtt.python) library with an intuitive, idiomatic asyncio interface:
 
 - No more callbacks! 👍
 - No more return codes (welcome to the `MqttError`)
 - Graceful disconnection (forget about `on_unsubscribe`, `on_disconnect`, etc.)
-- Compatible with `async` code
+- Supports MQTT versions 5.0, 3.1.1 and 3.1
 - Fully type-hinted
 - Did we mention no more callbacks?
 
-The whole thing is less than [900 lines of code](https://github.com/sbtinstruments/aiomqtt/blob/main/aiomqtt/client.py).
-
 <!-- pitch end -->
 
 ---
 
 **[Read the documentation at sbtinstruments.github.io/aiomqtt](https://sbtinstruments.github.io/aiomqtt)**
 
 ---
@@ -62,55 +59,45 @@
 
 If you can't wait for the latest version and want to install directly from GitHub, use:
 
 `pip install git+https://github.com/sbtinstruments/aiomqtt`
 
 ### Note for Windows users
 
-Since Python 3.8, the default asyncio event loop is the `ProactorEventLoop`. Said loop [doesn't support the `add_reader` method](https://docs.python.org/3/library/asyncio-platforms.html#windows) that is required by aiomqtt. Please switch to an event loop that supports the `add_reader` method such as the built-in `SelectorEventLoop`:
+Since Python `3.8`, the default asyncio event loop is the `ProactorEventLoop`. Said loop [doesn't support the `add_reader` method](https://docs.python.org/3/library/asyncio-platforms.html#windows) that is required by aiomqtt. Please switch to an event loop that supports the `add_reader` method such as the built-in `SelectorEventLoop`:
 
 ```python
 # Change to the "Selector" event loop if platform is Windows
 if sys.platform.lower() == "win32" or os.name.lower() == "nt":
-    # only import if platform/os is win32/nt, otherwise "WindowsSelectorEventLoopPolicy" is not present
-    from asyncio import (
-        set_event_loop_policy,
-        WindowsSelectorEventLoopPolicy
-    )
-    # set the event loop
+    from asyncio import set_event_loop_policy, WindowsSelectorEventLoopPolicy
     set_event_loop_policy(WindowsSelectorEventLoopPolicy())
 # Run your async application as usual
 asyncio.run(main())
-
 ```
 
 ## License
 
 This project is licensed under the [BSD 3-clause License](https://opensource.org/licenses/BSD-3-Clause).
 
 Note that the underlying paho-mqtt library is dual-licensed. One of the licenses is the so-called [Eclipse Distribution License v1.0](https://www.eclipse.org/org/documents/edl-v10.php). It is almost word-for-word identical to the BSD 3-clause License. The only differences are:
 
 - One use of "COPYRIGHT OWNER" (EDL) instead of "COPYRIGHT HOLDER" (BSD)
 - One use of "Eclipse Foundation, Inc." (EDL) instead of "copyright holder" (BSD)
 
 ## Contributing
 
-We're happy about your contributions to the project!
-
-You can get started by reading the [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CONTRIBUTING.md).
+We're very happy about contributions to the project! You can get started by reading [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CONTRIBUTING.md).
 
 ## Versioning
 
-This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-
-Expect API changes until we reach version `1.0.0`. After `1.0.0`, breaking changes will only occur in a major release (e.g., `2.0.0`, `3.0.0`, etc.).
+This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Breaking changes will only occur in major `X.0.0` releases.
 
 ## Changelog
 
-The changelog lives in the [CHANGELOG.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md) document. It adheres to the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
+The changelog lives in [CHANGELOG.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md). It follows the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Related projects
 
 Is aiomqtt not what you're looking for? There are a few other clients you can try:
 
 - [paho-mqtt](https://github.com/eclipse/paho.mqtt.python) — Own protocol implementation. Synchronous.<br>![GitHub stars](https://img.shields.io/github/stars/eclipse/paho.mqtt.python) ![license](https://img.shields.io/github/license/eclipse/paho.mqtt.python)
 - [gmqtt](https://github.com/wialon/gmqtt) — Own protocol implementation. Asynchronous.<br>![GitHub stars](https://img.shields.io/github/stars/wialon/gmqtt) ![license](https://img.shields.io/github/license/wialon/gmqtt)
```

#### html2text {}

```diff
@@ -1,61 +1,55 @@
              ****** The idiomatic asyncio MQTT client ð ******
                        (formerly known as asyncio-mqtt)
    [License:_BSD-3-Clause] [PyPI_version] [Supported_Python_versions] [PyPI
- downloads] [test] [docs] [Coverage] [pre-commit.ci_status] [Typing:_strict]
-                          [Code_style:_black] [Ruff]
- Write code like this: **Publisher** ```python async with Client
+downloads] [test] [docs] [Coverage] [Typing:_strict] [Code_style:_black] [Ruff]
+ Write code like this: **Publish** ```python async with Client
 ("test.mosquitto.org") as client: await client.publish("humidity/outside",
-payload=0.38) ``` **Subscriber** ```python async with Client
+payload=0.38) ``` **Subscribe** ```python async with Client
 ("test.mosquitto.org") as client: async with client.messages() as messages:
 await client.subscribe("humidity/#") async for message in messages: print
 (message.payload) ``` aiomqtt combines the stability of the time-proven [paho-
-mqtt](https://github.com/eclipse/paho.mqtt.python) library with a modern,
-asyncio-based interface. - No more callbacks! ð - No more return codes
+mqtt](https://github.com/eclipse/paho.mqtt.python) library with an intuitive,
+idiomatic asyncio interface: - No more callbacks! ð - No more return codes
 (welcome to the `MqttError`) - Graceful disconnection (forget about
-`on_unsubscribe`, `on_disconnect`, etc.) - Compatible with `async` code - Fully
-type-hinted - Did we mention no more callbacks? The whole thing is less than
-[900 lines of code](https://github.com/sbtinstruments/aiomqtt/blob/main/
-aiomqtt/client.py).  --- **[Read the documentation at sbtinstruments.github.io/
-aiomqtt](https://sbtinstruments.github.io/aiomqtt)** ---  ## Installation
-aiomqtt can be installed via `pip install aiomqtt`. It requires Python `3.7+`
-to run. The only dependency is [paho-mqtt](https://github.com/eclipse/
-paho.mqtt.python). If you can't wait for the latest version and want to install
-directly from GitHub, use: `pip install git+https://github.com/sbtinstruments/
-aiomqtt` ### Note for Windows users Since Python 3.8, the default asyncio event
-loop is the `ProactorEventLoop`. Said loop [doesn't support the `add_reader`
-method](https://docs.python.org/3/library/asyncio-platforms.html#windows) that
-is required by aiomqtt. Please switch to an event loop that supports the
-`add_reader` method such as the built-in `SelectorEventLoop`: ```python #
-Change to the "Selector" event loop if platform is Windows if
-sys.platform.lower() == "win32" or os.name.lower() == "nt": # only import if
-platform/os is win32/nt, otherwise "WindowsSelectorEventLoopPolicy" is not
-present from asyncio import ( set_event_loop_policy,
-WindowsSelectorEventLoopPolicy ) # set the event loop set_event_loop_policy
+`on_unsubscribe`, `on_disconnect`, etc.) - Supports MQTT versions 5.0, 3.1.1
+and 3.1 - Fully type-hinted - Did we mention no more callbacks?  --- **[Read
+the documentation at sbtinstruments.github.io/aiomqtt](https://
+sbtinstruments.github.io/aiomqtt)** ---  ## Installation aiomqtt can be
+installed via `pip install aiomqtt`. It requires Python `3.7+` to run. The only
+dependency is [paho-mqtt](https://github.com/eclipse/paho.mqtt.python). If you
+can't wait for the latest version and want to install directly from GitHub,
+use: `pip install git+https://github.com/sbtinstruments/aiomqtt` ### Note for
+Windows users Since Python `3.8`, the default asyncio event loop is the
+`ProactorEventLoop`. Said loop [doesn't support the `add_reader` method](https:
+//docs.python.org/3/library/asyncio-platforms.html#windows) that is required by
+aiomqtt. Please switch to an event loop that supports the `add_reader` method
+such as the built-in `SelectorEventLoop`: ```python # Change to the "Selector"
+event loop if platform is Windows if sys.platform.lower() == "win32" or
+os.name.lower() == "nt": from asyncio import set_event_loop_policy,
+WindowsSelectorEventLoopPolicy set_event_loop_policy
 (WindowsSelectorEventLoopPolicy()) # Run your async application as usual
 asyncio.run(main()) ``` ## License This project is licensed under the [BSD 3-
 clause License](https://opensource.org/licenses/BSD-3-Clause). Note that the
 underlying paho-mqtt library is dual-licensed. One of the licenses is the so-
 called [Eclipse Distribution License v1.0](https://www.eclipse.org/org/
 documents/edl-v10.php). It is almost word-for-word identical to the BSD 3-
 clause License. The only differences are: - One use of "COPYRIGHT OWNER" (EDL)
 instead of "COPYRIGHT HOLDER" (BSD) - One use of "Eclipse Foundation, Inc."
-(EDL) instead of "copyright holder" (BSD) ## Contributing We're happy about
-your contributions to the project! You can get started by reading the
+(EDL) instead of "copyright holder" (BSD) ## Contributing We're very happy
+about contributions to the project! You can get started by reading
 [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/
 CONTRIBUTING.md). ## Versioning This project adheres to [Semantic Versioning]
-(https://semver.org/spec/v2.0.0.html). Expect API changes until we reach
-version `1.0.0`. After `1.0.0`, breaking changes will only occur in a major
-release (e.g., `2.0.0`, `3.0.0`, etc.). ## Changelog The changelog lives in the
-[CHANGELOG.md](https://github.com/sbtinstruments/aiomqtt/blob/main/
-CHANGELOG.md) document. It adheres to the principles of [Keep a Changelog]
-(https://keepachangelog.com/en/1.0.0/). ## Related projects Is aiomqtt not what
-you're looking for? There are a few other clients you can try: - [paho-mqtt]
-(https://github.com/eclipse/paho.mqtt.python) â Own protocol implementation.
-Synchronous.
+(https://semver.org/spec/v2.0.0.html). Breaking changes will only occur in
+major `X.0.0` releases. ## Changelog The changelog lives in [CHANGELOG.md]
+(https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md). It follows
+the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). ##
+Related projects Is aiomqtt not what you're looking for? There are a few other
+clients you can try: - [paho-mqtt](https://github.com/eclipse/paho.mqtt.python)
+â Own protocol implementation. Synchronous.
 ![GitHub stars](https://img.shields.io/github/stars/eclipse/paho.mqtt.python) !
 [license](https://img.shields.io/github/license/eclipse/paho.mqtt.python) -
 [gmqtt](https://github.com/wialon/gmqtt) â Own protocol implementation.
 Asynchronous.
 ![GitHub stars](https://img.shields.io/github/stars/wialon/gmqtt) ![license]
 (https://img.shields.io/github/license/wialon/gmqtt) - [fastapi-mqtt](https://
 github.com/sabuhish/fastapi-mqtt) â Asynchronous wrapper around gmqtt.
```

### Comparing `aiomqtt-1.0.0/aiomqtt/__init__.py` & `aiomqtt-1.1.0/aiomqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomqtt-1.0.0/aiomqtt/client.py` & `aiomqtt-1.1.0/aiomqtt/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -123,17 +123,24 @@
 
 
 MAX_TOPIC_LENGTH = 65535
 
 
 @dataclass(frozen=True)
 class Wildcard:
-    """MQTT wildcard that can only be subscribed to.
+    """MQTT wildcard that can be subscribed to, but not published to.
 
-    A wildcard is similar to a topic, but can optionally contain + and # characters.
+    A wildcard is similar to a topic, but can optionally contain ``+`` and ``#``
+    placeholders.
+
+    Args:
+        value: The wildcard string.
+
+    Attributes:
+        value: The wildcard string.
     """
 
     value: str
 
     def __str__(self) -> str:
         return self.value
 
@@ -157,15 +164,22 @@
 
 
 WildcardLike: TypeAlias = "str | Wildcard"
 
 
 @dataclass(frozen=True)
 class Topic(Wildcard):
-    """MQTT topic that can be published and subscribed to."""
+    """MQTT topic that can be published and subscribed to.
+
+    Args:
+        value: The topic string.
+
+    Attributes:
+        value: The topic string.
+    """
 
     def __post_init__(self) -> None:
         """Validate the topic."""
         if not isinstance(self.value, str):
             msg = "topic must be a string"
             raise TypeError(msg)
         if (
@@ -174,27 +188,34 @@
             or "+" in self.value
             or "#" in self.value
         ):
             msg = f"Invalid topic: {self.value}"
             raise ValueError(msg)
 
     def matches(self, wildcard: WildcardLike) -> bool:
-        """Check if the topic matches a given wildcard."""
+        """Check if the topic matches a given wildcard.
+
+        Args:
+            wildcard: The wildcard to match against.
+
+        Returns:
+            True if the topic matches the wildcard, False otherwise.
+        """
         if not isinstance(wildcard, Wildcard):
             wildcard = Wildcard(wildcard)
         # Split topics into levels to compare them one by one
         topic_levels = self.value.split("/")
         wildcard_levels = str(wildcard).split("/")
         if wildcard_levels[0] == "$share":
             # Shared subscriptions use the topic structure: $share/<group_id>/<topic>
             wildcard_levels = wildcard_levels[2:]
 
         def recurse(x: list[str], y: list[str]) -> bool:
             if not x:
-                if not y:
+                if not y or y[0] == "#":
                     return True
                 return False
             if not y:
                 return False
             if y[0] == "#":
                 return True
             if x[0] == y[0] or y[0] == "+":
@@ -204,15 +225,41 @@
         return recurse(topic_levels, wildcard_levels)
 
 
 TopicLike: TypeAlias = "str | Topic"
 
 
 class Message:
-    """Wrap paho-mqtt message class that allows us to use our own Topic class."""
+    """Wraps the paho-mqtt message class to allow using our own matching logic.
+
+    This class is not meant to be instantiated by the user. Instead, it is yielded by
+    the async generator returned from ``Client.messages()``.
+
+    Args:
+        topic: The topic the message was published to.
+        payload: The message payload.
+        qos: The quality of service level of the subscription that matched the message.
+        retain: Whether the message is a retained message.
+        mid: The message ID.
+        properties: (MQTT v5.0 only) The properties associated with the message.
+
+    Attributes:
+        topic (aiomqtt.client.Topic):
+            The topic the message was published to.
+        payload (str | bytes | bytearray | int | float | None):
+            The message payload.
+        qos (int):
+            The quality of service level of the subscription that matched the message.
+        retain (bool):
+            Whether the message is a retained message.
+        mid (int):
+            The message ID.
+        properties (paho.mqtt.properties.Properties | None):
+            (MQTT v5.0 only) The properties associated with the message.
+    """
 
     def __init__(  # noqa: PLR0913
         self,
         topic: TopicLike,
         payload: PayloadType,
         qos: int,
         retain: bool,
@@ -238,25 +285,66 @@
         )
 
     def __lt__(self, other: Message) -> bool:
         return self.mid < other.mid
 
 
 class Client:
+    """The async context manager that manages the connection to the broker.
+
+    Args:
+        hostname: The hostname or IP address of the remote broker.
+        port: The network port of the remote broker.
+        username: The username to authenticate with.
+        password: The password to authenticate with.
+        logger: Custom logger instance.
+        client_id: The client ID to use. If ``None``, one will be generated
+            automatically.
+        tls_context: The SSL/TLS context.
+        tls_params: The SSL/TLS configuration to use.
+        tls_insecure: Enable/disable server hostname verification when using SSL/TLS.
+        proxy: Configure a proxy for the connection.
+        protocol: The version of the MQTT protocol.
+        will: The will message to publish if the client disconnects unexpectedly.
+        clean_session: If ``True``, the broker will remove all information about this
+            client when it disconnects. If ``False``, the client is a persistent client
+            and subscription information and queued messages will be retained when the
+            client disconnects.
+        transport: The transport protocol to use. Either ``"tcp"`` or ``"websockets"``.
+        timeout: The default timeout for all communication with the broker in seconds.
+        keepalive: The keepalive timeout for the client in seconds.
+        bind_address: The IP address of a local network interface to bind this client
+            to.
+        bind_port: The network port to bind this client to.
+        clean_start: (MQTT v5.0 only) Set the clean start flag always, never, or only
+            on the first successful connection to the broker.
+        properties: (MQTT v5.0 only) The properties associated with the client.
+        message_retry_set: Deprecated.
+        socket_options: Options to pass to the underlying socket.
+        max_concurrent_outgoing_calls: The maximum number of concurrent outgoing calls.
+        websocket_path: The path to use for websockets.
+        websocket_headers: The headers to use for websockets.
+        max_inflight_messages: The maximum number of messages with QoS > ``0`` that can
+            be part way through their network flow at once.
+        max_queued_messages: The maximum number of messages in the outgoing message
+            queue. ``0`` means unlimited.
+    """
+
     def __init__(  # noqa: C901, PLR0912, PLR0913, PLR0915
         self,
         hostname: str,
         port: int = 1883,
         *,
         username: str | None = None,
         password: str | None = None,
         logger: logging.Logger | None = None,
         client_id: str | None = None,
         tls_context: ssl.SSLContext | None = None,
         tls_params: TLSParameters | None = None,
+        tls_insecure: bool | None = None,
         proxy: ProxySettings | None = None,
         protocol: ProtocolVersion | None = None,
         will: Will | None = None,
         clean_session: bool | None = None,
         transport: str = "tcp",
         timeout: float | None = None,
         keepalive: int = 60,
@@ -352,14 +440,17 @@
                 keyfile=tls_params.keyfile,
                 cert_reqs=tls_params.cert_reqs,
                 tls_version=tls_params.tls_version,
                 ciphers=tls_params.ciphers,
                 keyfile_password=tls_params.keyfile_password,
             )
 
+        if tls_insecure is not None:
+            self._client.tls_insecure_set(tls_insecure)
+
         if proxy is not None:
             self._client.proxy_set(**proxy.proxy_args)
 
         if websocket_path is not None:
             self._client.ws_set_options(path=websocket_path, headers=websocket_headers)
 
         if will is not None:
@@ -421,23 +512,28 @@
         except (OSError, mqtt.WebsocketConnectionError) as error:
             raise MqttError(str(error)) from None
         await self._wait_for(self._connected, timeout=timeout)
         # If _disconnected is already completed after connecting, reset it.
         if self._disconnected.done():
             self._disconnected = asyncio.Future()
 
-    async def disconnect(self, *, timeout: float | None = None) -> None:
-        """Disconnect from the broker."""
+    def _early_out_on_disconnected(self) -> bool:
         # Early out if already disconnected...
         if self._disconnected.done():
             disc_exc = self._disconnected.exception()
             if disc_exc is not None:
                 # ...by raising the error that caused the disconnect
                 raise disc_exc
             # ...by returning since the disconnect was intentional
+            return True
+        return False
+
+    async def disconnect(self, *, timeout: float | None = None) -> None:
+        """Disconnect from the broker."""
+        if self._early_out_on_disconnected():
             return
         # Try to gracefully disconnect from the broker
         rc = self._client.disconnect()
         # Early out on error
         if rc != mqtt.MQTT_ERR_SUCCESS:
             raise MqttCodeError(rc, "Could not disconnect")
         # Wait for acknowledgement
@@ -457,14 +553,29 @@
         qos: int = 0,
         options: mqtt.SubscribeOptions | None = None,
         properties: Properties | None = None,
         *args: Any,
         timeout: float | None = None,
         **kwargs: Any,
     ) -> tuple[int] | list[mqtt.ReasonCodes]:
+        """Subscribe to a topic or wildcard.
+
+        Args:
+            topic: The topic or wildcard to subscribe to.
+            qos: The requested QoS level for the subscription.
+            options: (MQTT v5.0 only) Optional paho-mqtt subscription options.
+            properties: (MQTT v5.0 only) Optional paho-mqtt properties.
+            *args: Additional positional arguments to pass to paho-mqtt's subscribe
+                method.
+            timeout: The maximum time in seconds to wait for the subscription to
+                complete. Use ``math.inf`` to wait indefinitely.
+            **kwargs: Additional keyword arguments to pass to paho-mqtt's subscribe
+                method.
+
+        """
         result, mid = self._client.subscribe(
             topic, qos, options, properties, *args, **kwargs
         )
         # Early out on error
         if result != mqtt.MQTT_ERR_SUCCESS:
             raise MqttCodeError(result, "Could not subscribe to topic")
         # Create future for when the on_subscribe callback is called
@@ -480,14 +591,26 @@
         self,
         topic: str | list[str],
         properties: Properties | None = None,
         *args: Any,
         timeout: float | None = None,
         **kwargs: Any,
     ) -> None:
+        """Unsubscribe from a topic or wildcard.
+
+        Args:
+            topic: The topic or wildcard to unsubscribe from.
+            properties: (MQTT v5.0 only) Optional paho-mqtt properties.
+            *args: Additional positional arguments to pass to paho-mqtt's unsubscribe
+                method.
+            timeout: The maximum time in seconds to wait for the unsubscription to
+                complete. Use ``math.inf`` to wait indefinitely.
+            **kwargs: Additional keyword arguments to pass to paho-mqtt's unsubscribe
+                method.
+        """
         result, mid = self._client.unsubscribe(topic, properties, *args, **kwargs)
         # Early out on error
         if result != mqtt.MQTT_ERR_SUCCESS:
             raise MqttCodeError(result, "Could not unsubscribe from topic")
         # Create event for when the on_unsubscribe callback is called
         confirmation = asyncio.Event()
         with self._pending_call(mid, confirmation, self._pending_unsubscribes):
@@ -502,14 +625,29 @@
         qos: int = 0,
         retain: bool = False,
         properties: Properties | None = None,
         *args: Any,
         timeout: float | None = None,
         **kwargs: Any,
     ) -> None:
+        """Publish a message to the broker.
+
+        Args:
+            topic: The topic to publish to.
+            payload: The message payload.
+            qos: The QoS level to use for publication.
+            retain: If set to ``True``, the message will be retained by the broker.
+            properties: (MQTT v5.0 only) Optional paho-mqtt properties.
+            *args: Additional positional arguments to pass to paho-mqtt's publish
+                method.
+            timeout: The maximum time in seconds to wait for publication to complete.
+                Use ``math.inf`` to wait indefinitely.
+            **kwargs: Additional keyword arguments to pass to paho-mqtt's publish
+                method.
+        """
         info = self._client.publish(
             topic, payload, qos, retain, properties, *args, **kwargs
         )  # [2]
         # Early out on error
         if info.rc != mqtt.MQTT_ERR_SUCCESS:
             raise MqttCodeError(info.rc, "Could not publish message")
         # Early out on immediate success
@@ -568,19 +706,27 @@
     @asynccontextmanager
     async def messages(
         self,
         *,
         queue_class: type[asyncio.Queue[Message]] = asyncio.Queue,
         queue_maxsize: int = 0,
     ) -> AsyncGenerator[AsyncGenerator[Message, None], None]:
-        """Return async generator of incoming messages.
+        """Async context manager that creates a queue for incoming messages.
 
-        Use queue_maxsize to restrict the queue size. If the queue is full,
-        incoming messages will be discarded (and a warning is logged).
-        If queue_maxsize is less than or equal to zero, the queue size is infinite.
+        Args:
+            queue_class: The class to use for the queue. The default is
+                ``asyncio.Queue``, which returns messages in FIFO order. For LIFO order,
+                you can use ``asyncio.LifoQueue``; For priority order you can subclass
+                ``asyncio.PriorityQueue``.
+            queue_maxsize: Restricts the queue size. If the queue is full, incoming
+                messages will be discarded and a warning logged. If set to ``0`` or
+                less, the queue size is infinite.
+
+        Returns:
+            An async generator that yields messages from the underlying queue.
         """
         callback, generator = self._callback_and_generator(
             queue_class=queue_class, queue_maxsize=queue_maxsize
         )
         try:
             # Add to the list of callbacks to call when a message is received
             self._on_message_callbacks.append(callback)
@@ -895,23 +1041,26 @@
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         tb: TracebackType | None,
     ) -> None:
-        # Try to gracefully disconnect from the broker
+        """Try to gracefully disconnect from the broker."""
         try:
-            await self.disconnect()
-        except MqttError as error:
-            # We tried to be graceful. Now there is no mercy.
-            self._logger.warning(
-                f'Could not gracefully disconnect due to "{error}". Forcing'
-                " disconnection."
-            )
+            if self._early_out_on_disconnected():
+                return
+            try:
+                await self.disconnect()
+            except MqttError as error:
+                # We tried to be graceful. Now there is no mercy.
+                self._logger.warning(
+                    f'Could not gracefully disconnect due to "{error}". Forcing'
+                    " disconnection."
+                )
         finally:
             self._force_disconnect()
             self._lock.release()
 
 
 def _set_client_socket_defaults(
     client_socket: _PahoSocket | None, socket_options: Iterable[SocketOption]
```

### Comparing `aiomqtt-1.0.0/aiomqtt/error.py` & `aiomqtt-1.1.0/aiomqtt/error.py`

 * *Files identical despite different names*

### Comparing `aiomqtt-1.0.0/pyproject.toml` & `aiomqtt-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiomqtt"
-version = "1.0.0"  # Placeholder: Managed by poetry-dynamic-versioning
+version = "1.1.0"  # Placeholder: Managed by poetry-dynamic-versioning
 description = "The idiomatic asyncio MQTT client, wrapped around paho-mqtt"
 license = "BSD-3-Clause"
 authors = ["Frederik Aalund <fpa@sbtinstruments.com>", "Felix Böhm <felix@felixboehm.dev>", "Jonathan Plasse <jonathan.plasse@live.fr>"]
 readme = "README.md"
 packages = [{include = "aiomqtt"}]
 repository = "https://github.com/sbtinstruments/aiomqtt"
 documentation = "https://sbtinstruments.github.io/aiomqtt"
@@ -122,15 +122,15 @@
     "S101", # assert-used
 ]
 "tests/test_client.py" = [
     "SLF001", # private-member-access
 ]
 
 [tool.ruff.pydocstyle] # https://github.com/charliermarsh/ruff#pydocstyle
-convention = "pep257"
+convention = "google"
 
 [tool.mypy] # https://mypy.readthedocs.io/en/latest/config_file.html
 python_version = "3.8"
 strict = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
@@ -139,14 +139,17 @@
 no_strict_concatenate = true   # TODO(jonathan): remove when dropping python 3.7
 
 [tool.pytest.ini_options] # https://docs.pytest.org/en/latest/reference/reference.html#ini-options-ref
 filterwarnings = [
     "error",
     "ignore:ssl.PROTOCOL_TLS is deprecated:DeprecationWarning",
 ]
+markers = [
+    "network: tests that requires network access"
+]
 xfail_strict = true
 
 [tool.coverage.run] # https://coverage.readthedocs.io/en/latest/config.html#run
 branch = true
 data_file = "reports/.coverage"
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html#report
```

### Comparing `aiomqtt-1.0.0/PKG-INFO` & `aiomqtt-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomqtt
-Version: 1.0.0
+Version: 1.1.0
 Summary: The idiomatic asyncio MQTT client, wrapped around paho-mqtt
 Home-page: https://github.com/sbtinstruments/aiomqtt
 License: BSD-3-Clause
 Keywords: mqtt,iot,internet-of-things,asyncio,paho-mqtt,mqttv5
 Author: Frederik Aalund
 Author-email: fpa@sbtinstruments.com
 Requires-Python: >=3.7,<4.0
@@ -31,52 +31,49 @@
     <a href="https://github.com/sbtinstruments/aiomqtt/blob/main/LICENSE"><img alt="License: BSD-3-Clause" src="https://img.shields.io/github/license/sbtinstruments/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI version" src="https://img.shields.io/pypi/v/aiomqtt"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="Supported Python versions" src="https://img.shields.io/pypi/pyversions/aiomqtt.svg"></a>
     <a href="https://pypi.org/project/aiomqtt"><img alt="PyPI downloads" src="https://img.shields.io/pypi/dm/aiomqtt"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml"><img alt="test" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/test.yml/badge.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml"><img alt="docs" src="https://github.com/sbtinstruments/aiomqtt/actions/workflows/docs.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/sbtinstruments/aiomqtt"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/sbtinstruments/aiomqtt"></a>
-    <a href="https://results.pre-commit.ci/latest/github/sbtinstruments/aiomqtt/main"><img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/sbtinstruments/aiomqtt/main.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Typing: strict" src="https://img.shields.io/badge/typing-strict-green.svg"></a>
     <a href="https://github.com/sbtinstruments/aiomqtt"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black"></a>
     <a href="https://github.com/charliermarsh/ruff"><img alt="Ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json"></a>
 </p>
 
 <!-- pitch start -->
 
 Write code like this:
 
-**Publisher**
+**Publish**
 
 ```python
 async with Client("test.mosquitto.org") as client:
     await client.publish("humidity/outside", payload=0.38)
 ```
 
-**Subscriber**
+**Subscribe**
 
 ```python
 async with Client("test.mosquitto.org") as client:
     async with client.messages() as messages:
         await client.subscribe("humidity/#")
         async for message in messages:
             print(message.payload)
 ```
 
-aiomqtt combines the stability of the time-proven [paho-mqtt](https://github.com/eclipse/paho.mqtt.python) library with a modern, asyncio-based interface.
+aiomqtt combines the stability of the time-proven [paho-mqtt](https://github.com/eclipse/paho.mqtt.python) library with an intuitive, idiomatic asyncio interface:
 
 - No more callbacks! 👍
 - No more return codes (welcome to the `MqttError`)
 - Graceful disconnection (forget about `on_unsubscribe`, `on_disconnect`, etc.)
-- Compatible with `async` code
+- Supports MQTT versions 5.0, 3.1.1 and 3.1
 - Fully type-hinted
 - Did we mention no more callbacks?
 
-The whole thing is less than [900 lines of code](https://github.com/sbtinstruments/aiomqtt/blob/main/aiomqtt/client.py).
-
 <!-- pitch end -->
 
 ---
 
 **[Read the documentation at sbtinstruments.github.io/aiomqtt](https://sbtinstruments.github.io/aiomqtt)**
 
 ---
@@ -89,55 +86,45 @@
 
 If you can't wait for the latest version and want to install directly from GitHub, use:
 
 `pip install git+https://github.com/sbtinstruments/aiomqtt`
 
 ### Note for Windows users
 
-Since Python 3.8, the default asyncio event loop is the `ProactorEventLoop`. Said loop [doesn't support the `add_reader` method](https://docs.python.org/3/library/asyncio-platforms.html#windows) that is required by aiomqtt. Please switch to an event loop that supports the `add_reader` method such as the built-in `SelectorEventLoop`:
+Since Python `3.8`, the default asyncio event loop is the `ProactorEventLoop`. Said loop [doesn't support the `add_reader` method](https://docs.python.org/3/library/asyncio-platforms.html#windows) that is required by aiomqtt. Please switch to an event loop that supports the `add_reader` method such as the built-in `SelectorEventLoop`:
 
 ```python
 # Change to the "Selector" event loop if platform is Windows
 if sys.platform.lower() == "win32" or os.name.lower() == "nt":
-    # only import if platform/os is win32/nt, otherwise "WindowsSelectorEventLoopPolicy" is not present
-    from asyncio import (
-        set_event_loop_policy,
-        WindowsSelectorEventLoopPolicy
-    )
-    # set the event loop
+    from asyncio import set_event_loop_policy, WindowsSelectorEventLoopPolicy
     set_event_loop_policy(WindowsSelectorEventLoopPolicy())
 # Run your async application as usual
 asyncio.run(main())
-
 ```
 
 ## License
 
 This project is licensed under the [BSD 3-clause License](https://opensource.org/licenses/BSD-3-Clause).
 
 Note that the underlying paho-mqtt library is dual-licensed. One of the licenses is the so-called [Eclipse Distribution License v1.0](https://www.eclipse.org/org/documents/edl-v10.php). It is almost word-for-word identical to the BSD 3-clause License. The only differences are:
 
 - One use of "COPYRIGHT OWNER" (EDL) instead of "COPYRIGHT HOLDER" (BSD)
 - One use of "Eclipse Foundation, Inc." (EDL) instead of "copyright holder" (BSD)
 
 ## Contributing
 
-We're happy about your contributions to the project!
-
-You can get started by reading the [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CONTRIBUTING.md).
+We're very happy about contributions to the project! You can get started by reading [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CONTRIBUTING.md).
 
 ## Versioning
 
-This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-
-Expect API changes until we reach version `1.0.0`. After `1.0.0`, breaking changes will only occur in a major release (e.g., `2.0.0`, `3.0.0`, etc.).
+This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Breaking changes will only occur in major `X.0.0` releases.
 
 ## Changelog
 
-The changelog lives in the [CHANGELOG.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md) document. It adheres to the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
+The changelog lives in [CHANGELOG.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md). It follows the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Related projects
 
 Is aiomqtt not what you're looking for? There are a few other clients you can try:
 
 - [paho-mqtt](https://github.com/eclipse/paho.mqtt.python) — Own protocol implementation. Synchronous.<br>![GitHub stars](https://img.shields.io/github/stars/eclipse/paho.mqtt.python) ![license](https://img.shields.io/github/license/eclipse/paho.mqtt.python)
 - [gmqtt](https://github.com/wialon/gmqtt) — Own protocol implementation. Asynchronous.<br>![GitHub stars](https://img.shields.io/github/stars/wialon/gmqtt) ![license](https://img.shields.io/github/license/wialon/gmqtt)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiomqtt Version: 1.0.0 Summary: The idiomatic
+Metadata-Version: 2.1 Name: aiomqtt Version: 1.1.0 Summary: The idiomatic
 asyncio MQTT client, wrapped around paho-mqtt Home-page: https://github.com/
 sbtinstruments/aiomqtt License: BSD-3-Clause Keywords: mqtt,iot,internet-of-
 things,asyncio,paho-mqtt,mqttv5 Author: Frederik Aalund Author-email:
 fpa@sbtinstruments.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
@@ -14,65 +14,59 @@
 Documentation, https://sbtinstruments.github.io/aiomqtt Project-URL: Issue
 tracker, https://github.com/sbtinstruments/aiomqtt/issues Project-URL:
 Repository, https://github.com/sbtinstruments/aiomqtt Description-Content-Type:
 text/markdown
              ****** The idiomatic asyncio MQTT client ð ******
                        (formerly known as asyncio-mqtt)
    [License:_BSD-3-Clause] [PyPI_version] [Supported_Python_versions] [PyPI
- downloads] [test] [docs] [Coverage] [pre-commit.ci_status] [Typing:_strict]
-                          [Code_style:_black] [Ruff]
- Write code like this: **Publisher** ```python async with Client
+downloads] [test] [docs] [Coverage] [Typing:_strict] [Code_style:_black] [Ruff]
+ Write code like this: **Publish** ```python async with Client
 ("test.mosquitto.org") as client: await client.publish("humidity/outside",
-payload=0.38) ``` **Subscriber** ```python async with Client
+payload=0.38) ``` **Subscribe** ```python async with Client
 ("test.mosquitto.org") as client: async with client.messages() as messages:
 await client.subscribe("humidity/#") async for message in messages: print
 (message.payload) ``` aiomqtt combines the stability of the time-proven [paho-
-mqtt](https://github.com/eclipse/paho.mqtt.python) library with a modern,
-asyncio-based interface. - No more callbacks! ð - No more return codes
+mqtt](https://github.com/eclipse/paho.mqtt.python) library with an intuitive,
+idiomatic asyncio interface: - No more callbacks! ð - No more return codes
 (welcome to the `MqttError`) - Graceful disconnection (forget about
-`on_unsubscribe`, `on_disconnect`, etc.) - Compatible with `async` code - Fully
-type-hinted - Did we mention no more callbacks? The whole thing is less than
-[900 lines of code](https://github.com/sbtinstruments/aiomqtt/blob/main/
-aiomqtt/client.py).  --- **[Read the documentation at sbtinstruments.github.io/
-aiomqtt](https://sbtinstruments.github.io/aiomqtt)** ---  ## Installation
-aiomqtt can be installed via `pip install aiomqtt`. It requires Python `3.7+`
-to run. The only dependency is [paho-mqtt](https://github.com/eclipse/
-paho.mqtt.python). If you can't wait for the latest version and want to install
-directly from GitHub, use: `pip install git+https://github.com/sbtinstruments/
-aiomqtt` ### Note for Windows users Since Python 3.8, the default asyncio event
-loop is the `ProactorEventLoop`. Said loop [doesn't support the `add_reader`
-method](https://docs.python.org/3/library/asyncio-platforms.html#windows) that
-is required by aiomqtt. Please switch to an event loop that supports the
-`add_reader` method such as the built-in `SelectorEventLoop`: ```python #
-Change to the "Selector" event loop if platform is Windows if
-sys.platform.lower() == "win32" or os.name.lower() == "nt": # only import if
-platform/os is win32/nt, otherwise "WindowsSelectorEventLoopPolicy" is not
-present from asyncio import ( set_event_loop_policy,
-WindowsSelectorEventLoopPolicy ) # set the event loop set_event_loop_policy
+`on_unsubscribe`, `on_disconnect`, etc.) - Supports MQTT versions 5.0, 3.1.1
+and 3.1 - Fully type-hinted - Did we mention no more callbacks?  --- **[Read
+the documentation at sbtinstruments.github.io/aiomqtt](https://
+sbtinstruments.github.io/aiomqtt)** ---  ## Installation aiomqtt can be
+installed via `pip install aiomqtt`. It requires Python `3.7+` to run. The only
+dependency is [paho-mqtt](https://github.com/eclipse/paho.mqtt.python). If you
+can't wait for the latest version and want to install directly from GitHub,
+use: `pip install git+https://github.com/sbtinstruments/aiomqtt` ### Note for
+Windows users Since Python `3.8`, the default asyncio event loop is the
+`ProactorEventLoop`. Said loop [doesn't support the `add_reader` method](https:
+//docs.python.org/3/library/asyncio-platforms.html#windows) that is required by
+aiomqtt. Please switch to an event loop that supports the `add_reader` method
+such as the built-in `SelectorEventLoop`: ```python # Change to the "Selector"
+event loop if platform is Windows if sys.platform.lower() == "win32" or
+os.name.lower() == "nt": from asyncio import set_event_loop_policy,
+WindowsSelectorEventLoopPolicy set_event_loop_policy
 (WindowsSelectorEventLoopPolicy()) # Run your async application as usual
 asyncio.run(main()) ``` ## License This project is licensed under the [BSD 3-
 clause License](https://opensource.org/licenses/BSD-3-Clause). Note that the
 underlying paho-mqtt library is dual-licensed. One of the licenses is the so-
 called [Eclipse Distribution License v1.0](https://www.eclipse.org/org/
 documents/edl-v10.php). It is almost word-for-word identical to the BSD 3-
 clause License. The only differences are: - One use of "COPYRIGHT OWNER" (EDL)
 instead of "COPYRIGHT HOLDER" (BSD) - One use of "Eclipse Foundation, Inc."
-(EDL) instead of "copyright holder" (BSD) ## Contributing We're happy about
-your contributions to the project! You can get started by reading the
+(EDL) instead of "copyright holder" (BSD) ## Contributing We're very happy
+about contributions to the project! You can get started by reading
 [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/
 CONTRIBUTING.md). ## Versioning This project adheres to [Semantic Versioning]
-(https://semver.org/spec/v2.0.0.html). Expect API changes until we reach
-version `1.0.0`. After `1.0.0`, breaking changes will only occur in a major
-release (e.g., `2.0.0`, `3.0.0`, etc.). ## Changelog The changelog lives in the
-[CHANGELOG.md](https://github.com/sbtinstruments/aiomqtt/blob/main/
-CHANGELOG.md) document. It adheres to the principles of [Keep a Changelog]
-(https://keepachangelog.com/en/1.0.0/). ## Related projects Is aiomqtt not what
-you're looking for? There are a few other clients you can try: - [paho-mqtt]
-(https://github.com/eclipse/paho.mqtt.python) â Own protocol implementation.
-Synchronous.
+(https://semver.org/spec/v2.0.0.html). Breaking changes will only occur in
+major `X.0.0` releases. ## Changelog The changelog lives in [CHANGELOG.md]
+(https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md). It follows
+the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). ##
+Related projects Is aiomqtt not what you're looking for? There are a few other
+clients you can try: - [paho-mqtt](https://github.com/eclipse/paho.mqtt.python)
+â Own protocol implementation. Synchronous.
 ![GitHub stars](https://img.shields.io/github/stars/eclipse/paho.mqtt.python) !
 [license](https://img.shields.io/github/license/eclipse/paho.mqtt.python) -
 [gmqtt](https://github.com/wialon/gmqtt) â Own protocol implementation.
 Asynchronous.
 ![GitHub stars](https://img.shields.io/github/stars/wialon/gmqtt) ![license]
 (https://img.shields.io/github/license/wialon/gmqtt) - [fastapi-mqtt](https://
 github.com/sabuhish/fastapi-mqtt) â Asynchronous wrapper around gmqtt.
```

