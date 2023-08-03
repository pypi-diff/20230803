# Comparing `tmp/petkitaio-0.1.7.tar.gz` & `tmp/petkitaio-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.7.tar", last modified: Tue Jul 18 18:46:41 2023, max compression
+gzip compressed data, was "petkitaio-0.1.8.tar", last modified: Thu Aug  3 19:13:57 2023, max compression
```

## Comparing `petkitaio-0.1.7.tar` & `petkitaio-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-18 18:46:41.846050 petkitaio-0.1.7/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-18 18:42:51.000000 petkitaio-0.1.7/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     6428 2023-07-18 18:46:41.846290 petkitaio-0.1.7/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     4813 2023-07-18 18:42:51.000000 petkitaio-0.1.7/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-18 18:46:41.843588 petkitaio-0.1.7/petkitaio/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1942 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/__init__.py
--rw-r--r--   0 robertdrinovac   (501) staff       (20)    10841 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/constants.py
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1059 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/exceptions.py
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1392 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/model.py
--rw-r--r--   0 robertdrinovac   (501) staff       (20)    43642 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/petkit_client.py
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      680 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-18 18:46:41.845649 petkitaio-0.1.7/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     6428 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/top_level.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-18 18:46:41.846837 petkitaio-0.1.7/setup.cfg
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1050 2023-07-18 18:42:51.000000 petkitaio-0.1.7/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-08-03 19:13:57.865391 petkitaio-0.1.8/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1067 2023-08-03 19:11:43.000000 petkitaio-0.1.8/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    22445 2023-08-03 19:13:57.865750 petkitaio-0.1.8/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    18790 2023-08-03 19:11:43.000000 petkitaio-0.1.8/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-08-03 19:13:57.862967 petkitaio-0.1.8/petkitaio/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1932 2023-08-03 19:11:43.000000 petkitaio-0.1.8/petkitaio/__init__.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    10841 2023-08-03 19:11:43.000000 petkitaio-0.1.8/petkitaio/constants.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1045 2023-08-03 19:11:43.000000 petkitaio-0.1.8/petkitaio/exceptions.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1392 2023-08-03 19:11:43.000000 petkitaio-0.1.8/petkitaio/model.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    44096 2023-08-03 19:11:43.000000 petkitaio-0.1.8/petkitaio/petkit_client.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      680 2023-08-03 19:11:43.000000 petkitaio-0.1.8/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-08-03 19:13:57.865105 petkitaio-0.1.8/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    22445 2023-08-03 19:13:57.000000 petkitaio-0.1.8/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-08-03 19:13:57.000000 petkitaio-0.1.8/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-08-03 19:13:57.000000 petkitaio-0.1.8/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-08-03 19:13:57.000000 petkitaio-0.1.8/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-08-03 19:13:57.000000 petkitaio-0.1.8/petkitaio.egg-info/top_level.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-08-03 19:13:57.866309 petkitaio-0.1.8/setup.cfg
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1050 2023-08-03 19:11:43.000000 petkitaio-0.1.8/setup.py
```

### Comparing `petkitaio-0.1.7/LICENSE` & `petkitaio-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.7/petkitaio/__init__.py` & `petkitaio-0.1.8/petkitaio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     W5_DND_COMMANDS,
     W5_LIGHT_BRIGHTNESS,
     W5_LIGHT_POWER,
     W5_MODE,
     W5_SETTINGS_COMMANDS,
 )
 from .petkit_client import (PetKitClient, LOGGER,)
-from .exceptions import (AccountTypeError, AuthError, BluetoothError, PetKitError, ServerError)
+from .exceptions import (AuthError, BluetoothError, PetKitError, RegionError, ServerError)
 from .model import (Feeder, LitterBox, Pet, PetKitData, Purifier, W5Fountain, )
 from .str_enum import StrEnum
 
-__all__ = ['AccountTypeError', 'AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint', 'FeederCommand',
+__all__ = ['AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint', 'FeederCommand',
            'FEEDER_LIST', 'FeederSetting', 'Header', 'LB_CMD_TO_KEY', 'LB_CMD_TO_TYPE', 'LB_CMD_TO_VALUE', 'LitterBox', 'LitterBoxCommand', 'LitterBoxCommandKey',
            'LitterBoxCommandType', 'LitterBoxSetting', 'LITTER_LIST', 'LOGGER', 'Pet', 'PetKitClient', 'PetKitData', 'PetKitError', 'PetSetting', 'Purifier',
            'PurifierCommand', 'PurifierCommandKey', 'PurifierCommandType', 'PUR_CMD_TO_KEY', 'PUR_CMD_TO_TYPE', 'PUR_CMD_TO_VALUE', 'PURIFIER_LIST', 'PurifierSetting', 'Region',
-           'ServerError', 'SERVER_ERROR_CODES', 'StrEnum', 'TIMEOUT', 'WATER_FOUNTAIN_LIST', 'W5Command', 'W5_COMMAND_TO_CODE', 'W5_DND_COMMANDS', 'W5Fountain', 'W5_LIGHT_BRIGHTNESS',
+           'RegionError', 'ServerError', 'SERVER_ERROR_CODES', 'StrEnum', 'TIMEOUT', 'WATER_FOUNTAIN_LIST', 'W5Command', 'W5_COMMAND_TO_CODE', 'W5_DND_COMMANDS', 'W5Fountain', 'W5_LIGHT_BRIGHTNESS',
            'W5_LIGHT_POWER', 'W5_MODE', 'W5_SETTINGS_COMMANDS',  ]
```

### Comparing `petkitaio-0.1.7/petkitaio/constants.py` & `petkitaio-0.1.8/petkitaio/constants.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.7/petkitaio/exceptions.py` & `petkitaio-0.1.8/petkitaio/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,34 +7,37 @@
     """Error from PetKit api."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
         Exception.__init__(self, *args)
 
 
-class AccountTypeError(Exception):
-    """User has set account region to more than one region."""
-
-    def __init__(self, *args: Any) -> None:
-        """Initialize the exception."""
-        Exception.__init__(self, *args)
-
 class AuthError(Exception):
     """Authentication issue from PetKit api."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
         Exception.__init__(self, *args)
 
+
 class BluetoothError(Exception):
     """Bluetooth issue from PetKit api."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
         Exception.__init__(self, *args)
 
+
 class ServerError(Exception):
     """PetKit server error."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
         Exception.__init__(self, *args)
+
+
+class RegionError(Exception):
+    """Error when user fails to specify region."""
+
+    def __init__(self, *args: Any) -> None:
+        """Initialize the exception."""
+        Exception.__init__(self, *args)
```

### Comparing `petkitaio-0.1.7/petkitaio/model.py` & `petkitaio-0.1.8/petkitaio/model.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.7/petkitaio/petkit_client.py` & `petkitaio-0.1.8/petkitaio/petkit_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,41 +44,42 @@
     W5Command,
     W5_COMMAND_TO_CODE,
     W5_DND_COMMANDS,
     W5_LIGHT_BRIGHTNESS,
     W5_LIGHT_POWER,
     W5_SETTINGS_COMMANDS,
 )
-from petkitaio.exceptions import (AccountTypeError, AuthError, BluetoothError, PetKitError, ServerError)
+from petkitaio.exceptions import (AuthError, BluetoothError, PetKitError, RegionError, ServerError)
 from petkitaio.model import (Feeder, LitterBox, Pet, PetKitData, Purifier, W5Fountain)
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PetKitClient:
     """PetKit client."""
 
     def __init__(
-        self, username: str, password: str, session: ClientSession | None = None, asia_account: bool = False, china_account: bool = False, timeout: int = TIMEOUT
+        self, username: str, password: str, session: ClientSession | None = None, region: str = None, timeout: int = TIMEOUT
     ) -> None:
         """Initialize PetKit Client.
 
         username: PetKit username/email
         password: PetKit account password
         session: aiohttp.ClientSession or None to create a new session
         """
 
-        # Catch if a user is trying to set both asia and china account to true
-        if asia_account and china_account:
-            raise AccountTypeError('Only one region (Asia or China) may be set to True. Not both.')
+        # Catch if a user failed to define a region
+        if region is None:
+            raise RegionError('A region must be specified in order to log into your PetKit account.')
 
         self.username: str = username
         self.password: str = password
-        self.base_url: Region = Region.ASIA if asia_account else Region.CN if china_account else Region.US
-        self.server_list: list | None = None
+        self.region: str = region
+        self.base_url: str = ''
+        self.servers_dict: dict = {}
         self._session: ClientSession = session if session else ClientSession()
         self.tz: str = get_localzone_name()
         self.timeout: int = timeout
         self.token: str | None = None
         self.token_expiration: datetime | None = None
         self.user_id: str | None = None
         self.has_relay: bool = False
@@ -99,18 +100,32 @@
             'X-Api-Version': Header.API_VERSION,
             'Content-Type': Header.CONTENT_TYPE,
             'User-Agent': Header.AGENT,
             'X-Client': Header.CLIENT,
         }
         data = {}
         response = await self._post(url, headers, data)
-        self.server_list = response['result']['list']
+        server_list = response['result']['list']
+        for region in server_list:
+            self.servers_dict[region["name"]] = {
+                "id": region["id"],
+                "url": region["gateway"]
+            }
 
     async def login(self) -> None:
 
+        await self.get_api_server_list()
+        # Determine the user's base URL
+        if self.region == "China":
+            self.base_url = Region.CN
+        elif self.region in self.servers_dict:
+            self.base_url = self.servers_dict[self.region]["url"]
+        else:
+            raise RegionError('Region specified is not a valid region.')
+
         login_url = f'{self.base_url}{Endpoint.LOGIN}'
 
         headers = {
             'Accept': Header.ACCEPT,
             'Accept-Language': Header.ACCEPT_LANG,
             'Accept-Encoding': Header.ENCODING,
             'X-Api-Version': Header.API_VERSION,
@@ -120,14 +135,15 @@
         }
 
         data = {
             'client': str(CLIENT_DICT),
             'encrypt': '1',
             'oldVersion': Header.API_VERSION,
             'password': hashlib.md5(self.password.encode()).hexdigest(),
+            'region': self.servers_dict[self.region]["id"],
             'username': self.username
         }
 
         response = await self._post(login_url, headers, data)
         self.user_id = response['result']['session']['userId']
         self.token = response['result']['session']['id']
         self.token_expiration = datetime.now() + timedelta(seconds=response['result']['session']['expiresIn'])
```

### Comparing `petkitaio-0.1.7/petkitaio/str_enum.py` & `petkitaio-0.1.8/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.7/setup.py` & `petkitaio-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.7",
+    version="0.1.8",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
     keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
```

