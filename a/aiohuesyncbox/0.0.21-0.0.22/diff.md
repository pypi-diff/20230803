# Comparing `tmp/aiohuesyncbox-0.0.21.tar.gz` & `tmp/aiohuesyncbox-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohuesyncbox-0.0.21.tar", last modified: Sun Feb 20 15:12:56 2022, max compression
+gzip compressed data, was "aiohuesyncbox-0.0.22.tar", last modified: Thu Jul 27 18:39:03 2023, max compression
```

## Comparing `aiohuesyncbox-0.0.21.tar` & `aiohuesyncbox-0.0.22.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 15:12:56.638702 aiohuesyncbox-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3879 2022-02-20 15:12:56.638702 aiohuesyncbox-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 15:12:56.638702 aiohuesyncbox-0.0.21/aiohuesyncbox/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/device.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6528 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/execution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/hdmi.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/hsb_cacert.py
--rw-r--r--   0 runner    (1001) docker     (121)     3749 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/hue.py
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/aiohuesyncbox/huesyncbox.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 15:12:56.638702 aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3879 2022-02-20 15:12:56.000000 aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-02-20 15:12:56.000000 aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-20 15:12:56.000000 aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-20 15:12:56.000000 aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-20 15:12:56.000000 aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-20 15:12:56.638702 aiohuesyncbox-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-02-20 15:12:48.000000 aiohuesyncbox-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:39:03.943561 aiohuesyncbox-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-27 18:39:03.943561 aiohuesyncbox-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:39:03.943561 aiohuesyncbox-0.0.22/aiohuesyncbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/hdmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/hsb_cacert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/hue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/huesyncbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/aiohuesyncbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:39:03.943561 aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-27 18:39:03.000000 aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-27 18:39:03.000000 aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:39:03.000000 aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 18:39:03.000000 aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 18:39:03.000000 aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 18:39:03.947561 aiohuesyncbox-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-27 18:38:54.000000 aiohuesyncbox-0.0.22/setup.py
```

### Comparing `aiohuesyncbox-0.0.21/LICENSE` & `aiohuesyncbox-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.21/PKG-INFO` & `aiohuesyncbox-0.0.22/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiohuesyncbox
-Version: 0.0.21
+Version: 0.0.22
 Summary: Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.
 Home-page: https://github.com/mvdwetering/aiohuesyncbox
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering@gmail.com
 License: Apache License 2.0
 Keywords: automation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
@@ -41,21 +40,21 @@
 
 *Note on changing bridge*
 
 Changing a bridge is a bit more involved than other calls.
 After calling `box.hue.set_bridge()` the syncbox will start switching which takes a while (seems to take about 15 seconds).
 You will have to wait until the attributes match the expected endstate, but the status displayed on the API can be a bit confusing during the process.
 
-These are the statussus I see when switching from bridge A to bridge B.
+These are the status changes I see when switching from bridge A to bridge B.
 
 * ID: Bridge A, IP: Bridge A, Status: connected
 * Call `box.hue.set_bridge()` with info for bridge B
 * ID: Bridge B, IP: Bridge A, Status: connecting
 * ID: Bridge B, IP: Bridge B, Status: disconnected
-* ID: Bridge B, IP: Bridge B, Status: invalidgroup
+* ID: Bridge B, IP: Bridge B, Status: connected or ID: Bridge B, IP: Bridge B, Status: invalidgroup
 
 
 Examples
 ========
 
 The examples below are available as a runnable script in the repository.
 There is also an example on using `zeroconf` for device discovery.
@@ -96,15 +95,15 @@
 -----------
 
 .. code-block:: python
 
     from aiohuesyncbox import HueSyncBox
 
     # host and id can be obtained through mDNS/zeroconf discovery
-    # (or for testing look them up in the official Hue Sync app)
+    # (or for testing look them up in the official Hue app)
     box = HueSyncBox(host, id, access_token_from_registration_info)
 
     # Call initialize before interacting with the box
     await box.initialize()
     print(box.device.name)
     print(box.execution.sync_active)
     print(box.execution.mode)
@@ -113,9 +112,7 @@
     await box.execution.set_state(sync_active=True, mode="video", hdmi_source="input4")
 
     # Call update() to update with latest status from the box
     await box.execution.update()
     print(box.execution.sync_active)
     print(box.execution.mode)
 
-
-
```

### Comparing `aiohuesyncbox-0.0.21/README.rst` & `aiohuesyncbox-0.0.22/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 
 *Note on changing bridge*
 
 Changing a bridge is a bit more involved than other calls.
 After calling `box.hue.set_bridge()` the syncbox will start switching which takes a while (seems to take about 15 seconds).
 You will have to wait until the attributes match the expected endstate, but the status displayed on the API can be a bit confusing during the process.
 
-These are the statussus I see when switching from bridge A to bridge B.
+These are the status changes I see when switching from bridge A to bridge B.
 
 * ID: Bridge A, IP: Bridge A, Status: connected
 * Call `box.hue.set_bridge()` with info for bridge B
 * ID: Bridge B, IP: Bridge A, Status: connecting
 * ID: Bridge B, IP: Bridge B, Status: disconnected
-* ID: Bridge B, IP: Bridge B, Status: invalidgroup
+* ID: Bridge B, IP: Bridge B, Status: connected or ID: Bridge B, IP: Bridge B, Status: invalidgroup
 
 
 Examples
 ========
 
 The examples below are available as a runnable script in the repository.
 There is also an example on using `zeroconf` for device discovery.
@@ -77,15 +77,15 @@
 -----------
 
 .. code-block:: python
 
     from aiohuesyncbox import HueSyncBox
 
     # host and id can be obtained through mDNS/zeroconf discovery
-    # (or for testing look them up in the official Hue Sync app)
+    # (or for testing look them up in the official Hue app)
     box = HueSyncBox(host, id, access_token_from_registration_info)
 
     # Call initialize before interacting with the box
     await box.initialize()
     print(box.device.name)
     print(box.execution.sync_active)
     print(box.execution.mode)
```

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/device.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
             "ip_address",
             "api_level",
             "firmware_version",
         ]
         return generate_attribute_string(self, attributes)
 
     def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Device):
+            return NotImplemented
         return self._raw == other._raw
 
     @property
     def name(self) -> str:
         """Friendly name of the device."""
         return self._raw["name"]
```

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/errors.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/errors.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/execution.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             "video",
             "game",
             "music",
         ]
         return generate_attribute_string(self, attributes)
 
     def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Execution):
+            return NotImplemented
         return self._raw == other._raw
 
     def _update_syncmodes(self) -> None:
         self._syncmode_video = SyncMode(self._raw["video"])
         self._syncmode_game = SyncMode(self._raw["game"])
         self._syncmode_music = SyncMode(self._raw["music"])
```

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/hdmi.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/hdmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             "audio_sync_supported",
             "inputs",
             "output",
         ]
         return generate_attribute_string(self, attributes)
 
     def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Hdmi):
+            return NotImplemented
         return self._raw == other._raw
 
     def _update_inputs_and_output(self) -> None:
         inputs = []
         for key, value in self._raw.items():
             if key.startswith("input"):
                 inputs.append(Input(key, value))
```

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/hsb_cacert.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/hsb_cacert.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/hue.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/hue.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @property
     def active(self) -> bool:
         """Indicates if the group is actively streaming (either from Syncbox or other source)."""
         return self._raw["active"]
 
     @property
-    def owner(self) -> str:
+    def owner(self) -> str | None:
         """
         User friendly name of the application that is streaming on the associated bridge.
         Only exposed if active is true
         """
         return self._raw["owner"] if "owner" in self._raw else None
 
 
@@ -52,14 +52,16 @@
             "bridge_ip_address",
             "connection_state",
             "groups",
         ]
         return generate_attribute_string(self, attributes)
 
     def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Hue):
+            return NotImplemented
         return self._raw == other._raw
 
     @staticmethod
     def _build_groups(raw) -> List[Group]:
         groups = []
         for key, value in raw["groups"].items():
             groups.append(Group(key, value))
```

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox/huesyncbox.py` & `aiohuesyncbox-0.0.22/aiohuesyncbox/huesyncbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
         self._access_token = access_token
         self._port = port
         self._path = path
 
         self._clientsession = self._get_clientsession()
 
         # API endpoints
-        self.device = None
-        self.execution = None
-        self.hue = None
-        self.hdmi = None
+        self.device: Device
+        self.execution: Execution
+        self.hue: Hue
+        self.hdmi: Hdmi
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
 
@@ -97,15 +97,15 @@
                 self._id
             ),  # Use custom resolver to get certificate validation on common_name working
         )
 
         return aiohttp.ClientSession(connector=connector)
 
     @property
-    def access_token(self) -> str:
+    def access_token(self) -> str | None:
         return self._access_token
 
     async def is_registered(self):
         try:
             await self.request("get", "/registrations")
             return True
         except Unauthorized:
@@ -206,15 +206,18 @@
             ) as resp:
                 logger.debug("%s, %s" % (resp.status, await resp.text("utf-8")))
 
                 data = None
                 if resp.content_type == "application/json":
                     data = await resp.json()
                     if resp.status != 200:
-                        _raise_on_error(data)
+                        if isinstance(data, dict):
+                            _raise_on_error(data)
+                        else:
+                            logger.error("Received unexpected data format: %s" % str(data))
                 return data
         except aiohttp.client_exceptions.ClientError as err:
             raise RequestError(
                 "Error requesting data from {}: {}".format(self._host, err)
             ) from None
```

### Comparing `aiohuesyncbox-0.0.21/aiohuesyncbox.egg-info/PKG-INFO` & `aiohuesyncbox-0.0.22/aiohuesyncbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiohuesyncbox
-Version: 0.0.21
+Version: 0.0.22
 Summary: Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.
 Home-page: https://github.com/mvdwetering/aiohuesyncbox
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering@gmail.com
 License: Apache License 2.0
 Keywords: automation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
@@ -41,21 +40,21 @@
 
 *Note on changing bridge*
 
 Changing a bridge is a bit more involved than other calls.
 After calling `box.hue.set_bridge()` the syncbox will start switching which takes a while (seems to take about 15 seconds).
 You will have to wait until the attributes match the expected endstate, but the status displayed on the API can be a bit confusing during the process.
 
-These are the statussus I see when switching from bridge A to bridge B.
+These are the status changes I see when switching from bridge A to bridge B.
 
 * ID: Bridge A, IP: Bridge A, Status: connected
 * Call `box.hue.set_bridge()` with info for bridge B
 * ID: Bridge B, IP: Bridge A, Status: connecting
 * ID: Bridge B, IP: Bridge B, Status: disconnected
-* ID: Bridge B, IP: Bridge B, Status: invalidgroup
+* ID: Bridge B, IP: Bridge B, Status: connected or ID: Bridge B, IP: Bridge B, Status: invalidgroup
 
 
 Examples
 ========
 
 The examples below are available as a runnable script in the repository.
 There is also an example on using `zeroconf` for device discovery.
@@ -96,15 +95,15 @@
 -----------
 
 .. code-block:: python
 
     from aiohuesyncbox import HueSyncBox
 
     # host and id can be obtained through mDNS/zeroconf discovery
-    # (or for testing look them up in the official Hue Sync app)
+    # (or for testing look them up in the official Hue app)
     box = HueSyncBox(host, id, access_token_from_registration_info)
 
     # Call initialize before interacting with the box
     await box.initialize()
     print(box.device.name)
     print(box.execution.sync_active)
     print(box.execution.mode)
@@ -113,9 +112,7 @@
     await box.execution.set_state(sync_active=True, mode="video", hdmi_source="input4")
 
     # Call update() to update with latest status from the box
     await box.execution.update()
     print(box.execution.sync_active)
     print(box.execution.mode)
 
-
-
```

### Comparing `aiohuesyncbox-0.0.21/setup.py` & `aiohuesyncbox-0.0.22/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="aiohuesyncbox",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.21",
+    version="0.0.22",
     description="Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.",
     long_description=long_description,
     # The project's main homepage.
     url="https://github.com/mvdwetering/aiohuesyncbox",
     # Author details
     author="Michel van de Wetering",
     author_email="michel.van.de.wetering@gmail.com",
@@ -72,17 +72,17 @@
     # extras_require={
     #    'dev': ['check-manifest'],
     #    'test': ['coverage'],
     # },
     # If there are data files included in your packages that need to be
     # installed, specify them here.  If using Python 2.6 or less, then these
     # have to be included in MANIFEST.in as well.
-    # package_data={
-    #    'sample': ['package_data.dat'],
-    # },
+    package_data={
+        "aiohuesyncbox": ["py.typed"],
+    },
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files # noqa
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
     # data_files=[('my_data', ['data/data_file'])],
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
```

