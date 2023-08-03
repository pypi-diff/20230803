# Comparing `tmp/pyintesishome-1.8.4.tar.gz` & `tmp/pyintesishome-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintesishome-1.8.4.tar", last modified: Sun Sep 25 10:35:49 2022, max compression
+gzip compressed data, was "pyintesishome-1.8.5.tar", last modified: Thu Aug  3 01:47:56 2023, max compression
```

## Comparing `pyintesishome-1.8.4.tar` & `pyintesishome-1.8.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 10:35:49.119932 pyintesishome-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-09-25 10:35:49.119932 pyintesishome-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 10:35:49.115931 pyintesishome-1.8.4/pyintesishome/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14114 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    21590 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/intesisbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     8513 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/intesisbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     8302 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/intesishome.py
--rw-r--r--   0 runner    (1001) docker     (121)     8791 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/pyintesishome/intesishomelocal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 10:35:49.119932 pyintesishome-1.8.4/pyintesishome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-09-25 10:35:49.000000 pyintesishome-1.8.4/pyintesishome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-25 10:35:49.000000 pyintesishome-1.8.4/pyintesishome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 10:35:49.000000 pyintesishome-1.8.4/pyintesishome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-25 10:35:49.000000 pyintesishome-1.8.4/pyintesishome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-25 10:35:49.000000 pyintesishome-1.8.4/pyintesishome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-25 10:35:49.119932 pyintesishome-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-09-25 10:35:37.000000 pyintesishome-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:47:56.569323 pyintesishome-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-03 01:47:56.569323 pyintesishome-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:47:56.569323 pyintesishome-1.8.5/pyintesishome/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/intesisbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/intesisbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/intesishome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/pyintesishome/intesishomelocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:47:56.569323 pyintesishome-1.8.5/pyintesishome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-03 01:47:56.000000 pyintesishome-1.8.5/pyintesishome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-03 01:47:56.000000 pyintesishome-1.8.5/pyintesishome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:47:56.000000 pyintesishome-1.8.5/pyintesishome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 01:47:56.000000 pyintesishome-1.8.5/pyintesishome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 01:47:56.000000 pyintesishome-1.8.5/pyintesishome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 01:47:56.569323 pyintesishome-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:47:56.569323 pyintesishome-1.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-08-03 01:47:47.000000 pyintesishome-1.8.5/tests/test_pyintesishome.py
```

### Comparing `pyintesishome-1.8.4/LICENSE` & `pyintesishome-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyintesishome-1.8.4/PKG-INFO` & `pyintesishome-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintesishome
-Version: 1.8.4
+Version: 1.8.5
 Summary: A python3 library for running asynchronus communications with IntesisHome Smart AC Controllers
 Home-page: https://github.com/jnimmo/pyIntesisHome
 Author: James Nimmo
 Author-email: james@nimmo.net.nz
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `pyintesishome-1.8.4/README.md` & `pyintesishome-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyintesishome-1.8.4/pyintesishome/const.py` & `pyintesishome-1.8.5/pyintesishome/const.py`

 * *Files identical despite different names*

### Comparing `pyintesishome-1.8.4/pyintesishome/intesisbase.py` & `pyintesishome-1.8.5/pyintesishome/intesisbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self,
         username=None,
         password=None,
         host=None,
         loop=None,
         websession=None,
         device_type=DEVICE_INTESISHOME,
-    ):
+    ) -> None:
         """Initialize IntesisBox controller."""
         # Select correct API for device type
         self._username = username
         self._password = password
         self._host = host
         self._device_type = device_type
         self._devices = {}
@@ -46,15 +46,15 @@
         self._connection_retries = 0
         self._update_callbacks = []
         self._keepalive_task: asyncio.Task = None
         self._receive_task: asyncio.Task = None
         self._error_message = None
         self._web_session = websession
         self._own_session = False
-        self._controller_id = username
+        self._controller_id = None
         self._controller_name = username
         self._writer: StreamWriter = None
         self._reader: StreamReader = None
         self._received_response: asyncio.Event = asyncio.Event()
         self._data_delimiter = b"}}"
 
         if loop:
@@ -83,14 +83,15 @@
                 try:
                     await asyncio.wait_for(
                         self._received_response.wait(),
                         timeout=5.0,
                     )
                 except asyncio.TimeoutError:
                     print("oops took longer than 5s!")
+                    await self.stop()
         except OSError as exc:
             _LOGGER.error("%s Exception. %s / %s", type(exc), exc.args, exc)
 
     async def _data_received(self):
         try:
             while self._reader:
                 raw_data = await self._reader.readuntil(self._data_delimiter)
@@ -100,26 +101,26 @@
                 _LOGGER.debug("Received: %s", data)
                 await self._parse_response(data)
 
                 if not self._received_response.is_set():
                     _LOGGER.debug("Resolving set_value's await")
                     self._received_response.set()
         except IncompleteReadError:
-            _LOGGER.info(
-                "pyIntesisHome lost connection to the %s server.", self._device_type
+            _LOGGER.debug(
+                "pyIntesisHome lost connection to the %s server", self._device_type
             )
         except asyncio.CancelledError:
             pass
         except (
             TimeoutError,
             ConnectionResetError,
             OSError,
         ) as exc:
             _LOGGER.error(
-                "pyIntesisHome lost connection to the %s server. Exception: %s",
+                "PyIntesisHome lost connection to the %s server. Exception: %s",
                 self._device_type,
                 exc,
             )
         finally:
             self._connected = False
             self._connecting = False
             await self._send_update_callback()
@@ -513,15 +514,15 @@
         return self._device_type
 
     @property
     def controller_id(self) -> str:
         """Returns an account/device identifier - Serial, MAC or username."""
         if self._controller_id:
             return self._controller_id.lower()
-        return None
+        raise ValueError("Controller ID has not been set yet")
 
     @property
     def name(self) -> str:
         """Returns an account/device identifier - Serial, MAC or username."""
         if self._controller_name:
             return self._controller_name
         return None
```

### Comparing `pyintesishome-1.8.4/pyintesishome/intesisbox.py` & `pyintesishome-1.8.5/pyintesishome/intesisbox.py`

 * *Files identical despite different names*

### Comparing `pyintesishome-1.8.4/pyintesishome/intesishome.py` & `pyintesishome-1.8.5/pyintesishome/intesishome.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             websession=websession,
         )
         self._api_url = API_URL[device_type]
         self._api_ver = API_VER[device_type]
         self._cmd_server = None
         self._cmd_server_port = None
         self._auth_token = None
+        self._controller_id = username
 
     async def _parse_response(self, decoded_data):
         _LOGGER.debug("%s API Received: %s", self._device_type, decoded_data)
         resp = json.loads(decoded_data)
         # Parse response
         if resp["command"] == "connect_rsp":
             # New connection success
@@ -147,15 +148,15 @@
         status_response = None
         try:
             async with self._web_session.post(
                 url=self._api_url, data=get_status
             ) as resp:
                 status_response = await resp.json(content_type=None)
                 _LOGGER.debug(status_response)
-        except (aiohttp.client_exceptions.ClientConnectorError) as exc:
+        except aiohttp.client_exceptions.ClientConnectorError as exc:
             raise IHConnectionError from exc
         except (aiohttp.client_exceptions.ClientError, socket.gaierror) as exc:
             self._error_message = f"Error connecting to {self._device_type} API: {exc}"
             _LOGGER.error("%s Exception. %s / %s", type(exc), repr(exc.args), exc)
             raise IHConnectionError from exc
 
         if status_response:
```

### Comparing `pyintesishome-1.8.4/pyintesishome/intesishomelocal.py` & `pyintesishome-1.8.5/pyintesishome/intesishomelocal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Main submodule for pyintesishome."""
 
 import asyncio
 import logging
+from json import JSONDecodeError
 
 import aiohttp
 
 from .const import (
     COMMAND_MAP,
     DEVICE_INTESISHOME_LOCAL,
     INTESIS_MAP,
@@ -21,15 +22,15 @@
 _LOGGER = logging.getLogger("pyintesishome")
 
 
 # pylint: disable=too-many-instance-attributes, too-many-arguments, too-many-public-methods
 class IntesisHomeLocal(IntesisBase):
     """pyintesishome local class."""
 
-    def __init__(self, host, username, password, loop=None, websession=None):
+    def __init__(self, host, username, password, loop=None, websession=None) -> None:
         """Constructor"""
         device_type = DEVICE_INTESISHOME_LOCAL
         self._session_id: str = ""
         self._datapoints: dict = {}
         self._scan_interval = 6
         self._device_id: str = ""
         self._values: dict = {}
@@ -66,80 +67,137 @@
             while self._connected:
                 try:
                     values = await self._request_values()
                     for uid, value in values.items():
                         self._update_device_state(self._device_id, uid, value)
 
                     await self._send_update_callback(self._device_id)
-                except (IHConnectionError) as exc:
+                except IHConnectionError as exc:
                     _LOGGER.error("Error during updater task: %s", exc)
                 await asyncio.sleep(self._scan_interval)
         except asyncio.CancelledError:
             _LOGGER.debug("Cancelled the updater task")
         _LOGGER.debug("Updater task is exiting")
 
     async def _authenticate(self) -> bool:
         """Authenticate using username and password."""
         payload = {
             "command": LOCAL_CMD_LOGIN,
             "data": {"username": self._username, "password": self._password},
         }
-        async with self._web_session.post(
-            f"http://{self._host}/api.cgi", json=payload
-        ) as response:
-            if response.status != 200:
-                raise IHConnectionError("HTTP response status is unexpected (not 200)")
-            json_response = await response.json()
-            self._session_id = json_response["data"].get("id").get("sessionID")
-            _LOGGER.debug("Authenticated with new session ID %s", self._session_id)
+        try:
+            async with self._web_session.post(
+                f"http://{self._host}/api.cgi", json=payload
+            ) as response:
+                if response.status != 200:
+                    raise IHConnectionError(
+                        "HTTP response status is unexpected (not 200)"
+                    )
+                json_response = await response.json()
+                # Check if the response has the expected format
+                if (
+                    "data" in json_response
+                    and "id" in json_response["data"]
+                    and "sessionID" in json_response["data"]["id"]
+                ):
+                    self._session_id = json_response["data"]["id"]["sessionID"]
+                    _LOGGER.debug(
+                        "Authenticated with new session ID %s", self._session_id
+                    )
+                else:
+                    _LOGGER.error("Unexpected response format during authentication")
+        except (
+            aiohttp.ClientConnectionError,
+            aiohttp.ClientResponseError,
+            aiohttp.ClientPayloadError,
+            aiohttp.ContentTypeError,
+            JSONDecodeError,
+        ) as exception:
+            _LOGGER.error("Error during authentication: %s", str(exception))
 
     async def _request(self, command: str, **kwargs) -> dict:
         """Make a request."""
         connection_attempts = 0
 
         while connection_attempts < 2:
             connection_attempts += 1
             if not self._session_id:
                 await self._authenticate()
 
             payload = {
                 "command": command,
                 "data": {"sessionID": self._session_id, **kwargs},
             }
-            _LOGGER.debug("Sending intesishome_local command %s", command)
+            _LOGGER.debug(
+                "Sending intesishome_local command %s to %s", command, self._host
+            )
             timeout = aiohttp.ClientTimeout(total=10)
             json_response = {}
             try:
                 async with self._web_session.post(
                     f"http://{self._host}/api.cgi",
                     json=payload,
                     timeout=timeout,
                 ) as response:
                     if response.status != 200:
                         raise IHConnectionError(
-                            "HTTP response status is unexpected (not 200)"
+                            f"HTTP response status is unexpected for {self._host}"
+                            "(got {response.status}, want 200)"
                         )
                     json_response = await response.json()
             except asyncio.exceptions.TimeoutError as exc:
                 _LOGGER.error(
-                    "IntesisHome HTTP timeout error: %s",
+                    "IntesisHome HTTP timeout error for %s: %s",
+                    self._host,
                     exc,
                 )
-            except (aiohttp.ClientError) as exc:
+            except aiohttp.ClientError as exc:
                 _LOGGER.error(
-                    "IntesisHome HTTP error: %s",
+                    "IntesisHome HTTP error for %s: %s",
+                    self._host,
                     exc,
                 )
 
-            if "success" in json_response:
+            # If the response has a non-false "success", return the data.
+            #
+            # If the key doesn't exist, treat it as "false" and continue with
+            # error handling.
+            #
+            # If the error code is one we know requires re-authentication,
+            # clear the session key so we re-authenticate on the next attempt,
+            # otherwise just log the code and error message.
+            #
+            # If there's neither a "success" or "error" key, something is very
+            # wonky, so log an error plus the entire response.
+            if json_response.get("success", False):
                 return json_response.get("data")
-
-            if "error" in json_response and json_response["error"]["code"] in [1, 5]:
-                self._session_id = ""
-                _LOGGER.debug("Request failed. Clearing session key")
+            if "error" in json_response:
+                error = json_response["error"]
+                if error.get("code") in [1, 5]:
+                    self._session_id = ""
+                    _LOGGER.debug(
+                        "Request failed for %s (code=%s, message=%r)."
+                        "Clearing session key to force re-authentication",
+                        self._host,
+                        error.get("code"),
+                        error.get("message"),
+                    )
+                else:
+                    _LOGGER.debug(
+                        "Request failed for %s (code=%s, message=%r). Error not handled",
+                        self._host,
+                        error.get("code"),
+                        error.get("message"),
+                    )
+            else:
+                _LOGGER.debug(
+                    "Request failed for %s - no 'success' or 'error' keys. json_response=%r",
+                    self._host,
+                    json_response,
+                )
 
     async def _request_value(self, name: str) -> dict:
         """Get entity value by uid."""
         response = await self._request(
             LOCAL_CMD_GET_DP_VALUE, uid=COMMAND_MAP[name]["uid"]
         )
         return response["dpval"]["value"]
@@ -168,56 +226,67 @@
         if datapoint not in COMMAND_MAP:
             return False
         return COMMAND_MAP[datapoint]["uid"] in self._datapoints
 
     async def connect(self):
         """Connect to the device and start periodic updater."""
         await self.poll_status()
-        _LOGGER.debug("Successful authenticated and polled. Fetching Datapoints.")
+        _LOGGER.debug("Successful authenticated and polled. Fetching Datapoints")
         await self.get_datapoints()
         self._connected = True
-        _LOGGER.debug("Starting updater task.")
+        _LOGGER.debug("Starting updater task")
         self._update_task = asyncio.create_task(self._run_updater())
 
     async def stop(self):
         """Disconnect and stop periodic updater."""
-        _LOGGER.debug("Stopping updater task.")
+        _LOGGER.debug("Stopping updater task")
         await self._cancel_task_if_exists(self._update_task)
         self._connected = False
 
         if self._own_session:
             await self._web_session.close()
 
     async def get_info(self) -> dict:
         """Get device info."""
         response = await self._request(LOCAL_CMD_GET_INFO)
         self._info = response["info"]
         return self._info
 
     async def poll_status(self, sendcallback=False):
         """Get device info for setup purposes."""
-        await self._authenticate()
-        info = await self.get_info()
-        self._device_id = info["sn"]
-        self._controller_id = info["sn"].lower()
-        self._controller_name = f"{self._info['deviceModel']} ({info['ownSSID']})"
-        # Setup devices
-        self._devices[self._device_id] = {
-            "name": info["ownSSID"],
-            "widgets": [],
-            "model": info["deviceModel"],
-        }
+        try:
+            await self._authenticate()
+            info = await self.get_info()
 
-        await self.get_datapoints()
-        _LOGGER.debug(repr(self._devices))
+            # Extract device_id up to the first space, if there is a space
+            raw_id = info.get("sn")
+            if raw_id:
+                device_id, *_ = raw_id.split(" ")
+                self._device_id = device_id
+                self._controller_id = device_id.lower()
+
+            self._controller_name = (
+                f"{self._info.get('deviceModel')} ({info.get('ownSSID')})"
+            )
+            # Setup devices
+            self._devices[self._device_id] = {
+                "name": info.get("ownSSID"),
+                "widgets": [],
+                "model": info.get("deviceModel"),
+            }
+
+            await self.get_datapoints()
+            _LOGGER.debug(repr(self._devices))
 
-        self._update_device_state(self._device_id, "acStatus", info["acStatus"])
+            self._update_device_state(self._device_id, "acStatus", info.get("acStatus"))
 
-        if sendcallback:
-            await self._send_update_callback(str(self._device_id))
+            if sendcallback:
+                await self._send_update_callback(str(self._device_id))
+        except (IHConnectionError, KeyError) as exception:
+            _LOGGER.error("Error during polling status: %s", str(exception))
 
     def get_mode_list(self, device_id) -> list:
         """Get possible entity modes."""
         uid = COMMAND_MAP["mode"]["uid"]
         return [
             INTESIS_MAP[uid]["values"][i]
             for i in self._datapoints[uid]["descr"]["states"]
```

### Comparing `pyintesishome-1.8.4/pyintesishome.egg-info/PKG-INFO` & `pyintesishome-1.8.5/pyintesishome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintesishome
-Version: 1.8.4
+Version: 1.8.5
 Summary: A python3 library for running asynchronus communications with IntesisHome Smart AC Controllers
 Home-page: https://github.com/jnimmo/pyIntesisHome
 Author: James Nimmo
 Author-email: james@nimmo.net.nz
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `pyintesishome-1.8.4/setup.py` & `pyintesishome-1.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pyintesishome",
-    version="1.8.4",
+    version="1.8.5",
     description="A python3 library for running asynchronus communications with IntesisHome Smart AC Controllers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jnimmo/pyIntesisHome",
     author="James Nimmo",
     author_email="james@nimmo.net.nz",
     license="MIT",
```

