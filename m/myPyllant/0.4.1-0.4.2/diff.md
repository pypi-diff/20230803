# Comparing `tmp/mypyllant-0.4.1.tar.gz` & `tmp/mypyllant-0.4.2.tar.gz`

## Comparing `mypyllant-0.4.1.tar` & `mypyllant-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,48 @@
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.1/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.1/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.1/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.1/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    19167 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/api.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/export.py
--rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.4.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.1/LICENSE
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 mypyllant-0.4.1/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 mypyllant-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.dockerignore
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.2/Dockerfile
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.2/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.2/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.2/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/api.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
+-rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 mypyllant-0.4.2/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 mypyllant-0.4.2/PKG-INFO
```

### Comparing `mypyllant-0.4.1/.pre-commit-config.yaml` & `mypyllant-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/logo.png` & `mypyllant-0.4.2/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/.github/workflows/build-test.yaml` & `mypyllant-0.4.2/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/src/myPyllant/api.py` & `mypyllant-0.4.2/src/myPyllant/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,27 +30,36 @@
     DHWOperationMode,
     DomesticHotWater,
     System,
     Zone,
     ZoneCurrentSpecialFunction,
     ZoneHeatingOperatingMode,
 )
-from myPyllant.utils import datetime_format, dict_to_snake_case, generate_code
+from myPyllant.utils import (
+    datetime_format,
+    dict_to_snake_case,
+    generate_code,
+    get_realm,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AuthenticationFailed(ConnectionError):
     pass
 
 
 class LoginEndpointInvalid(ConnectionError):
     pass
 
 
+class RealmInvalid(ConnectionError):
+    pass
+
+
 async def on_request_start(session, context, params: aiohttp.TraceRequestStartParams):
     """
     See https://docs.aiohttp.org/en/stable/tracing_reference.html#aiohttp.TraceConfig.on_request_start
     """
     logger.debug(f"Starting request {params}")
 
 
@@ -64,23 +73,28 @@
 class MyPyllantAPI:
     username: str
     password: str
     aiohttp_session: aiohttp.ClientSession
     oauth_session: dict = {}
     oauth_session_expires: datetime.datetime | None = None
 
-    def __init__(self, username: str, password: str, country: str, brand: str) -> None:
+    def __init__(
+        self, username: str, password: str, brand: str, country: str | None = None
+    ) -> None:
         if brand not in BRANDS.keys():
             raise ValueError(
                 f"Invalid brand, must be one of {', '.join(BRANDS.keys())}"
             )
-        if country not in COUNTRIES[brand].keys():
-            raise ValueError(
+        if country and country not in COUNTRIES[brand].keys():
+            raise RealmInvalid(
                 f"Invalid country, {BRANDS[brand]} only supports {', '.join(COUNTRIES[brand].keys())}"
             )
+        if not country and brand in COUNTRIES and COUNTRIES[brand]:
+            # If a brand has countries defined, a country needs to be provided
+            raise RealmInvalid(f"{BRANDS[brand]} requires country to be passed")
         self.username = username
         self.password = password
         self.country = country
         self.brand = brand
         trace_config = aiohttp.TraceConfig()
         trace_config.on_request_start.append(on_request_start)
         trace_config.on_request_end.append(on_request_end)
@@ -126,24 +140,24 @@
             "code_challenge_method": "S256",
             "code_challenge": code_challenge,
         }
 
         # Grabbing the login URL from the HTML form of the login page
         try:
             async with self.aiohttp_session.get(
-                AUTHENTICATE_URL.format(country=self.country, brand=self.brand)
+                AUTHENTICATE_URL.format(realm=get_realm(self.brand, self.country))
                 + "?"
                 + urlencode(auth_querystring)
             ) as resp:
                 login_html = await resp.text()
         except ClientResponseError as e:
             raise LoginEndpointInvalid from e
 
         result = re.search(
-            LOGIN_URL.format(country=self.country, brand=self.brand) + r"\?([^\"]*)",
+            LOGIN_URL.format(realm=get_realm(self.brand, self.country)) + r"\?([^\"]*)",
             login_html,
         )
         login_url = unescape(result.group())
 
         logger.debug(f"Got login url {login_url}")
 
         login_payload = {
@@ -170,15 +184,15 @@
             "client_id": "myvaillant",
             "code": code,
             "code_verifier": code_verifier,
             "redirect_uri": "enduservaillant.page.link://login",
         }
 
         async with self.aiohttp_session.post(
-            TOKEN_URL.format(country=self.country, brand=self.brand),
+            TOKEN_URL.format(realm=get_realm(self.brand, self.country)),
             data=token_payload,
             raise_for_status=False,
         ) as resp:
             login_json = await resp.json()
             if resp.status >= 400:
                 logger.error(
                     f"Could not log in, got status {resp.status} this response: {login_json}"
@@ -197,15 +211,15 @@
     async def refresh_token(self):
         refresh_payload = {
             "refresh_token": self.oauth_session["refresh_token"],
             "client_id": CLIENT_ID,
             "grant_type": "refresh_token",
         }
         async with self.aiohttp_session.post(
-            TOKEN_URL.format(country=self.country, brand=self.brand),
+            TOKEN_URL.format(realm=get_realm(self.brand, self.country)),
             data=refresh_payload,
         ) as resp:
             self.oauth_session = await resp.json()
             self.set_session_expires()
             return self.oauth_session
 
     @property
```

### Comparing `mypyllant-0.4.1/src/myPyllant/const.py` & `mypyllant-0.4.2/src/myPyllant/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,56 @@
-LOGIN_URL = "https://identity.vaillant-group.com/auth/realms/{brand}-{country}-b2c/login-actions/authenticate"
-AUTHENTICATE_URL = "https://identity.vaillant-group.com/auth/realms/{brand}-{country}-b2c/protocol/openid-connect/auth"
-TOKEN_URL = "https://identity.vaillant-group.com/auth/realms/{brand}-{country}-b2c/protocol/openid-connect/token"
+LOGIN_URL = (
+    "https://identity.vaillant-group.com/auth/realms/{realm}/login-actions/authenticate"
+)
+AUTHENTICATE_URL = "https://identity.vaillant-group.com/auth/realms/{realm}/protocol/openid-connect/auth"
+TOKEN_URL = "https://identity.vaillant-group.com/auth/realms/{realm}/protocol/openid-connect/token"
 CLIENT_ID = "myvaillant"
 API_URL_BASE = (
     "https://api.vaillant-group.com/service-connected-control/end-user-app-api/v1"
 )
 BRANDS = {
     "vaillant": "Vaillant",
     "sdbg": "Saunier Duval",
+    "bulex": "Bulex",
 }
 DEFAULT_BRAND = "vaillant"
 COUNTRIES = {
     "vaillant": {
+        "albania": "Albania",
         "austria": "Austria",
         "belgium": "Belgium",
         "bulgaria": "Bulgaria",
         "croatia": "Croatia",
         "czechrepublic": "Czechia",
         "denmark": "Denmark",
         "estonia": "Estonia",
         "finland": "Finland",
         "france": "France",
+        "georgia": "Georgia",
         "germany": "Germany",
         "greece": "Greece",
         "hungary": "Hungary",
         "italy": "Italy",
         "latvia": "Latvia",
         "lithuania": "Lithuania",
+        "luxembourg": "Luxembourg",
         "netherlands": "Netherlands",
         "norway": "Norway",
         "poland": "Poland",
         "portugal": "Portugal",
         "romania": "Romania",
         "serbia": "Serbia",
         "slovakia": "Slovakia",
         "slovenia": "Slovenia",
         "spain": "Spain",
         "sweden": "Sweden",
         "switzerland": "Switzerland",
+        "ukraine": "Ukraine",
         "unitedkingdom": "United Kingdom",
+        "uzbekistan": "Uzbekistan",
     },
     "sdbg": {
         "austria": "Austria",
         "czechrepublic": "Czechia",
         "finland": "Finland",
         "france": "France",
         "greece": "Greece",
```

### Comparing `mypyllant-0.4.1/src/myPyllant/export.py` & `mypyllant-0.4.2/src/myPyllant/export.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,31 +4,19 @@
 import asyncio
 import json
 import logging
 import sys
 from datetime import datetime
 
 from myPyllant.api import MyPyllantAPI
-from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 from myPyllant.models import DeviceDataBucketResolution
+from myPyllant.utils import add_default_parser_args
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API.")
-parser.add_argument("user", help="Username (email address) for the myVaillant app")
-parser.add_argument("password", help="Password for the myVaillant app")
-parser.add_argument(
-    "country",
-    help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
-)
-parser.add_argument(
-    "brand",
-    help="Brand your account is registered in, i.e. 'vaillant'",
-    default=DEFAULT_BRAND,
-    choices=BRANDS.keys(),
-)
+add_default_parser_args(parser)
 parser.add_argument(
     "-d",
     "--data",
     action=argparse.BooleanOptionalAction,
     help="Export historical device data",
 )
 parser.add_argument(
@@ -53,17 +41,24 @@
 )
 parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
 async def main(
-    user, password, country, brand, data=False, resolution=None, start=None, end=None
+    user,
+    password,
+    brand,
+    country=None,
+    data=False,
+    resolution=None,
+    start=None,
+    end=None,
 ):
-    async with MyPyllantAPI(user, password, country, brand) as api:
+    async with MyPyllantAPI(user, password, brand, country) as api:
         async for system in api.get_systems():
             if data:
                 data_list = []
                 for device in system.devices:
                     data = [
                         d.dict()
                         async for d in api.get_data_by_device(
```

### Comparing `mypyllant-0.4.1/src/myPyllant/models.py` & `mypyllant-0.4.2/src/myPyllant/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         The Vaillant API returns information about zones, circuits, and dhw separately as
         configuration, state, and properties.
 
         This function merges everything together into one big dict for a given object (i.e. zones)
         """
         indexes = [o["index"] for o in self.configuration.get(obj_name, [])]
         for idx in indexes:
-            # deepcopy() avoids unintentional changes to the referenced objects
+            # State and properties get merged into configuration
             configuration = next(
                 c for c in self.configuration.get(obj_name, []) if c["index"] == idx
             )
             try:
                 state = next(
                     c for c in self.state.get(obj_name, []) if c["index"] == idx
                 )
@@ -238,30 +238,40 @@
             return None
 
 
 class Device(BaseModel):
     system_id: str
     device_uuid: str
     name: str = ""
-    product_name: str
+    product_name: str = ""
     diagnostic_trouble_codes: list = []
     properties: list = []
     ebus_id: str
     article_number: str
     device_serial_number: str
     type: str
     device_type: str
     first_data: datetime.datetime
     last_data: datetime.datetime
     operational_data: dict = {}
     data: list["DeviceData"] = []
 
     @property
     def name_display(self) -> str:
-        return self.name if self.name else self.product_name.title()
+        """
+        Product name might be empty, fall back to title-cased device type
+        """
+        return self.name or self.product_name_display
+
+    @property
+    def product_name_display(self) -> str:
+        """
+        Product name might be None, fall back to title-cased device type
+        """
+        return self.product_name or self.device_type.replace("_", "").title()
 
 
 class DeviceDataBucket(BaseModel):
     start_date: datetime.datetime
     end_date: datetime.datetime
     value: float | None
```

### Comparing `mypyllant-0.4.1/src/myPyllant/sample.py` & `mypyllant-0.4.2/src/myPyllant/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
-    "country",
-    help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
-)
-parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
 parser.add_argument(
+    "--country",
+    help="Country your account is registered in, i.e. 'germany'",
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+    required=False,
+)
+parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
-async def main(user, password, country, brand):
-    async with MyPyllantAPI(user, password, country, brand) as api:
+async def main(user, password, brand, country):
+    async with MyPyllantAPI(user, password, brand, country) as api:
         async for system in api.get_systems():
             print(await api.get_time_zone(system))
             print(await api.set_holiday(system))
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
@@ -51,8 +52,8 @@
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
-    asyncio.run(main(args.user, args.password, args.country, args.brand))
+    asyncio.run(main(args.user, args.password, args.brand, args.country))
```

### Comparing `mypyllant-0.4.1/src/myPyllant/utils.py` & `mypyllant-0.4.2/src/myPyllant/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import argparse
 import base64
 import hashlib
 import random
 import re
 import string
 from datetime import datetime
 
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
+
 
 def dict_to_snake_case(d):
     """
     Convert {'camelCase': value} to {'camel_case': value} recursively
     """
 
     snake_pattern = re.compile(r"(?<!^)(?=[A-Z])")
@@ -51,7 +54,34 @@
         return date.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
     else:
         return date.strftime("%Y-%m-%dT%H:%M:%S") + "Z"
 
 
 def datetime_parse(date_string: str) -> datetime:
     return datetime.strptime(date_string, "%Y-%m-%dT%H:%M:%SZ")
+
+
+def get_realm(brand: str, country: str) -> str:
+    """
+    Vaillant and SDBG use `brand-country-b2c` as the realm, Bulex doesn't use a country
+    """
+    if brand == "bulex":
+        return f"{brand}-b2c"
+    else:
+        return f"{brand}-{country}-b2c"
+
+
+def add_default_parser_args(parser: argparse.ArgumentParser):
+    parser.add_argument("user", help="Username (email address) for the myVaillant app")
+    parser.add_argument("password", help="Password for the myVaillant app")
+    parser.add_argument(
+        "brand",
+        help="Brand your account is registered in, i.e. 'vaillant'",
+        default=DEFAULT_BRAND,
+        choices=BRANDS.keys(),
+    )
+    parser.add_argument(
+        "--country",
+        help="Country your account is registered in, i.e. 'germany'",
+        choices=COUNTRIES[DEFAULT_BRAND].keys(),
+        required=False,
+    )
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/find_countries.py` & `mypyllant-0.4.2/src/myPyllant/tests/find_countries.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         if r.status_code == 200:
             yield country_name, country
 
 
 def main():
     print("COUNTRIES = {")
     for brand in BRANDS.keys():
+        if brand == "bulex":
+            # Bulex has no country-specific realms
+            continue
         print(f'    "{brand}": {{')
         for country_name, country in countries_with_realm(brand):
             print(f'        "{country_name}": "{country}",')
         print("    },")
     print("}")
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.4.2/src/myPyllant/tests/generate_test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,23 @@
 import secrets
 import signal
 import sys
 from datetime import datetime, timedelta
 from pathlib import Path
 from urllib.parse import urlencode
 
-from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
+from myPyllant.utils import add_default_parser_args
 
 logger = logging.getLogger(__name__)
 
 
 parser = argparse.ArgumentParser(
     description="Generates test data necessary to run integration tests."
 )
-parser.add_argument("user", help="Username (email address) for the myVaillant app")
-parser.add_argument("password", help="Password for the myVaillant app")
-parser.add_argument(
-    "country",
-    help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
-)
-parser.add_argument(
-    "brand",
-    help="Brand your account is registered in, i.e. 'vaillant'",
-    default=DEFAULT_BRAND,
-    choices=BRANDS.keys(),
-)
+add_default_parser_args(parser)
 parser.add_argument(
     "--debug", help="Print debug information", action=argparse.BooleanOptionalAction
 )
 
 SALT = secrets.token_bytes(16)
 JSON_DIR = Path(__file__).resolve().parent / "json"
 ANONYMIZE_ATTRIBUTES = (
@@ -52,33 +40,33 @@
 def user_json_dir(user: str) -> Path:
     return (
         JSON_DIR
         / hashlib.sha1(user.encode("UTF-8") + SALT, usedforsecurity=False).hexdigest()
     )
 
 
-async def main(user, password, country, brand):
+async def main(user, password, brand, country=None):
     """
     Generate json data for running testcases.
 
     :param user:
     :param password:
-    :param country:
     :param brand:
+    :param country:
     :return:
     """
     from myPyllant.api import MyPyllantAPI
     from myPyllant.const import API_URL_BASE
     from myPyllant.models import DeviceDataBucketResolution
     from myPyllant.utils import datetime_format
 
     json_dir = user_json_dir(user)
     json_dir.mkdir(parents=True, exist_ok=True)
 
-    async with MyPyllantAPI(user, password, country, brand) as api:
+    async with MyPyllantAPI(user, password, brand, country) as api:
         claims_url = f"{API_URL_BASE}/claims"
         async with api.aiohttp_session.get(
             claims_url, headers=api.get_authorized_headers()
         ) as claims_resp:
             claims = await claims_resp.json()
             with open(json_dir / "claims.json", "w") as fh:
                 anonymized_system = _recursive_data_anonymize(
@@ -153,14 +141,15 @@
         )
         async with api.aiohttp_session.get(
             device_buckets_url, headers=api.get_authorized_headers()
         ) as device_buckets_resp:
             with open(json_dir / "device_buckets.json", "w") as fh:
                 device_buckets = await device_buckets_resp.json()
                 fh.write(json.dumps(device_buckets, indent=2))
+        print(f"Wrote test data to {json_dir}")
 
 
 def _recursive_data_anonymize(
     data: str | dict | list, salt: bytes = b""
 ) -> str | dict | list:
     if isinstance(data, list):
         for elem in data:
@@ -185,8 +174,8 @@
 
     def signal_handler(sig, frame):
         user_json_dir(args.user).rmdir()
         sys.exit(sig)
 
     signal.signal(signal.SIGINT, signal_handler)
 
-    asyncio.run(main(args.user, args.password, args.country, args.brand))
+    asyncio.run(main(args.user, args.password, args.brand, args.country))
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/test_api.py` & `mypyllant-0.4.2/src/myPyllant/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         test_data.append(user_data)
     return test_data
 
 
 async def test_login(mypyllant_aioresponses) -> None:
     with mypyllant_aioresponses() as _:
         async with MyPyllantAPI(
-            "test@example.com", "test", "germany", "vaillant"
+            "test@example.com", "test", "vaillant", "germany"
         ) as mocked_api:
             assert isinstance(mocked_api.oauth_session_expires, datetime)
             assert mocked_api.oauth_session_expires > datetime.now()
             assert mocked_api.access_token == "access_token"
             assert "Authorization" in mocked_api.get_authorized_headers()
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/test_countries.py` & `mypyllant-0.4.2/src/myPyllant/tests/test_countries.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from unittest import mock
 
 import pytest
 
-from myPyllant.api import MyPyllantAPI
+from myPyllant.api import MyPyllantAPI, RealmInvalid
 from myPyllant.tests.find_countries import countries_with_realm
 
 
 async def test_invalid_country() -> None:
-    with pytest.raises(ValueError) as _:
-        MyPyllantAPI("test@example.com", "test", "invalid", "vaillant")
+    with pytest.raises(RealmInvalid) as _:
+        MyPyllantAPI("test@example.com", "test", "vaillant", "invalid")
 
 
 async def test_invalid_country_for_brand() -> None:
-    with pytest.raises(ValueError) as _:
-        MyPyllantAPI("test@example.com", "test", "germany", "sdbg")
+    with pytest.raises(RealmInvalid) as _:
+        MyPyllantAPI("test@example.com", "test", "sdbg", "germany")
 
 
 async def test_invalid_brand() -> None:
     with pytest.raises(ValueError) as _:
-        MyPyllantAPI("test@example.com", "test", "germany", "invalid")
+        MyPyllantAPI("test@example.com", "test", "invalid", "germany")
 
 
 async def test_find_countries(mocker) -> None:
     mocker.patch(
         "country_list.countries_for_language", return_value=[("de", "Germany")]
     )
     with mock.patch("requests.head") as patched_head:
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/test_export.py` & `mypyllant-0.4.2/src/myPyllant/tests/test_export.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from ..export import main as export_main
 from .test_api import get_test_data
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_export(mypyllant_aioresponses, capsys, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
-        await export_main("test@example.com", "test", "germany", "vaillant")
+        await export_main("test@example.com", "test", "vaillant", "germany")
         captured = capsys.readouterr()
         assert isinstance(json.loads(captured.out), dict)
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_export_data(mypyllant_aioresponses, capsys, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
-        await export_main("test@example.com", "test", "germany", "vaillant", data=True)
+        await export_main("test@example.com", "test", "vaillant", "germany", data=True)
         captured = capsys.readouterr()
         assert isinstance(json.loads(captured.out), list)
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.4.2/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/update_sample.py` & `mypyllant-0.4.2/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/utils.py` & `mypyllant-0.4.2/src/myPyllant/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import re
 
 from aioresponses import aioresponses
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import API_URL_BASE, LOGIN_URL
+from myPyllant.utils import get_realm
 
 
 def _mypyllant_aioresponses():
     class _mypyllant_aioresponses(aioresponses):
         def __init__(self, test_data=None, **kwargs):
             self.test_data = test_data
             super().__init__(**kwargs)
 
         def __enter__(self):
             super().__enter__()
 
             # auth endpoints
             self.get(
                 re.compile(r".*openid-connect/auth\?"),
-                body=f"{LOGIN_URL.format(brand='vaillant', country='germany')}?test=test",
+                body=f"{LOGIN_URL.format(realm=get_realm('vaillant', 'germany'))}?test=test",
                 status=200,
                 repeat=True,
             )
             self.post(
                 re.compile(r".*login-actions/authenticate\?"),
                 status=200,
                 headers={"Location": "test?code=code"},
@@ -149,15 +150,15 @@
                 )
             return self
 
     return _mypyllant_aioresponses
 
 
 async def _mocked_api(*args, **kwargs) -> MyPyllantAPI:
-    api = MyPyllantAPI("test@example.com", "test", "germany", "vaillant")
+    api = MyPyllantAPI("test@example.com", "test", "vaillant", "germany")
     api.oauth_session = {
         "access_token": "access_token",
         "refresh_token": "refresh_token",
         "expires_in": 3600,
     }
     api.set_session_expires()
     return api
```

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json` & `mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json` & `mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json` & `mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/.gitignore` & `mypyllant-0.4.2/.dockerignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
+.DS_Store
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `mypyllant-0.4.1/LICENSE` & `mypyllant-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/README.md` & `mypyllant-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,24 @@
 
 > **Warning**
 > 
 > You need at least Python 3.10
 
 ```shell
 pip install myPyllant
-python3 -m myPyllant.export user password country brand
+python3 -m myPyllant.export user password brand --country country
 # See python3 -m myPyllant.export -h for more options and a list of countries
 ```
 
+..or use Docker:
+
+```shell
+docker run -ti ghcr.io/signalkraft/mypyllant:latest python3 -m myPyllant.export user password brand --country country
+```
+
 The `--data` argument exports historical data of the devices in your system.
 Without this keyword, information about your system will be exported as JSON.
 
 ## Usage
 
 ```python
 #!/usr/bin/env python3
@@ -37,31 +43,32 @@
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
-    "country",
-    help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
-)
-parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
 parser.add_argument(
+    "--country",
+    help="Country your account is registered in, i.e. 'germany'",
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+    required=False,
+)
+parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
-async def main(user, password, country, brand):
-    async with MyPyllantAPI(user, password, country, brand) as api:
+async def main(user, password, brand, country):
+    async with MyPyllantAPI(user, password, brand, country) as api:
         async for system in api.get_systems():
             print(await api.get_time_zone(system))
             print(await api.set_holiday(system))
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
@@ -80,15 +87,15 @@
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
-    asyncio.run(main(args.user, args.password, args.country, args.brand))
+    asyncio.run(main(args.user, args.password, args.brand, args.country))
 
 ```
 
 ### Tested Configurations
 
 See https://github.com/signalkraft/mypyllant-component/blob/main/README.md#tested-setups
 
@@ -124,21 +131,26 @@
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
 python3 -m myPyllant.tests.generate_test_data -h
-python3 -m myPyllant.tests.generate_test_data username password country brand
+python3 -m myPyllant.tests.generate_test_data username password brand --country country
+```
+
+..or use Docker:
+
+```shell
+docker run -v $(pwd)/test_data:/build/src/myPyllant/tests/json -ti ghcr.io/signalkraft/mypyllant:latest python3 -m myPyllant.tests.generate_test_data username password brand --country country
 ```
 
-This creates a new folder with JSON values from the API in `src/myPyllant/tests/json`.
-Check the timestamp on the folders, if you're unsure which one is yours.
+With docker, the results will be put into `test_data/`.
 
-You can then either create a PR with the newly created folder, or zip it and attach it to an issue.
+You can then either create a PR with the created folder, or zip it and attach it to an issue.
 
 ### Reverse Engineering API requests of the myVAILLANT app
 
 You'll need an Android device and a computer with ADB on the same network.
 
 1. Run mitmproxy, for example in Docker: `docker run --rm -it -v ~/.mitmproxy:/home/mitmproxy/.mitmproxy -p 0.0.0.0:8080:8080 -p 127.0.0.1:8081:8081 mitmproxy/mitmproxy mitmweb --web-host 0.0.0.0`
 2. In the WIFI connection settings of your Android device, set a manual proxy to the IP of the computer running mitmproxy on port 8080, with an exception for `identity.vaillant-group.com` (which opens in your browser and uses HSTS)
```

### Comparing `mypyllant-0.4.1/pyproject.toml` & `mypyllant-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.1/PKG-INFO` & `mypyllant-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,18 +29,24 @@
 
 > **Warning**
 > 
 > You need at least Python 3.10
 
 ```shell
 pip install myPyllant
-python3 -m myPyllant.export user password country brand
+python3 -m myPyllant.export user password brand --country country
 # See python3 -m myPyllant.export -h for more options and a list of countries
 ```
 
+..or use Docker:
+
+```shell
+docker run -ti ghcr.io/signalkraft/mypyllant:latest python3 -m myPyllant.export user password brand --country country
+```
+
 The `--data` argument exports historical data of the devices in your system.
 Without this keyword, information about your system will be exported as JSON.
 
 ## Usage
 
 ```python
 #!/usr/bin/env python3
@@ -53,31 +59,32 @@
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
-    "country",
-    help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
-)
-parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
 parser.add_argument(
+    "--country",
+    help="Country your account is registered in, i.e. 'germany'",
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+    required=False,
+)
+parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
-async def main(user, password, country, brand):
-    async with MyPyllantAPI(user, password, country, brand) as api:
+async def main(user, password, brand, country):
+    async with MyPyllantAPI(user, password, brand, country) as api:
         async for system in api.get_systems():
             print(await api.get_time_zone(system))
             print(await api.set_holiday(system))
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
@@ -96,15 +103,15 @@
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
-    asyncio.run(main(args.user, args.password, args.country, args.brand))
+    asyncio.run(main(args.user, args.password, args.brand, args.country))
 
 ```
 
 ### Tested Configurations
 
 See https://github.com/signalkraft/mypyllant-component/blob/main/README.md#tested-setups
 
@@ -140,21 +147,26 @@
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
 python3 -m myPyllant.tests.generate_test_data -h
-python3 -m myPyllant.tests.generate_test_data username password country brand
+python3 -m myPyllant.tests.generate_test_data username password brand --country country
+```
+
+..or use Docker:
+
+```shell
+docker run -v $(pwd)/test_data:/build/src/myPyllant/tests/json -ti ghcr.io/signalkraft/mypyllant:latest python3 -m myPyllant.tests.generate_test_data username password brand --country country
 ```
 
-This creates a new folder with JSON values from the API in `src/myPyllant/tests/json`.
-Check the timestamp on the folders, if you're unsure which one is yours.
+With docker, the results will be put into `test_data/`.
 
-You can then either create a PR with the newly created folder, or zip it and attach it to an issue.
+You can then either create a PR with the created folder, or zip it and attach it to an issue.
 
 ### Reverse Engineering API requests of the myVAILLANT app
 
 You'll need an Android device and a computer with ADB on the same network.
 
 1. Run mitmproxy, for example in Docker: `docker run --rm -it -v ~/.mitmproxy:/home/mitmproxy/.mitmproxy -p 0.0.0.0:8080:8080 -p 127.0.0.1:8081:8081 mitmproxy/mitmproxy mitmweb --web-host 0.0.0.0`
 2. In the WIFI connection settings of your Android device, set a manual proxy to the IP of the computer running mitmproxy on port 8080, with an exception for `identity.vaillant-group.com` (which opens in your browser and uses HSTS)
```

