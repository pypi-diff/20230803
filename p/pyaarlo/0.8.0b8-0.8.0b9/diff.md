# Comparing `tmp/pyaarlo-0.8.0b8.tar.gz` & `tmp/pyaarlo-0.8.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaarlo-0.8.0b8.tar", last modified: Wed May 31 18:16:25 2023, max compression
+gzip compressed data, was "pyaarlo-0.8.0b9.tar", last modified: Wed Jul  5 20:39:12 2023, max compression
```

## Comparing `pyaarlo-0.8.0b8.tar` & `pyaarlo-0.8.0b9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.668292 pyaarlo-0.8.0b8/
--rw-r--r--   0 steve     (1000) steve     (1000)     7652 2019-08-16 18:58:59.000000 pyaarlo-0.8.0b8/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-31 18:16:25.668292 pyaarlo-0.8.0b8/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)    18439 2022-02-13 14:58:05.000000 pyaarlo-0.8.0b8/README.md
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.664292 pyaarlo-0.8.0b8/pyaarlo/
--rw-rw-r--   0 steve     (1000) steve     (1000)    27069 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/pyaarlo/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    42982 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/pyaarlo/backend.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     4925 2023-05-10 01:20:55.000000 pyaarlo-0.8.0b8/pyaarlo/background.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    22075 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/pyaarlo/base.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    50293 2023-04-11 00:17:07.000000 pyaarlo-0.8.0b8/pyaarlo/camera.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6630 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b8/pyaarlo/cfg.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9513 2023-05-31 17:38:42.000000 pyaarlo-0.8.0b8/pyaarlo/constant.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    11646 2023-02-06 16:43:11.000000 pyaarlo-0.8.0b8/pyaarlo/device.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7676 2022-10-27 14:08:34.000000 pyaarlo-0.8.0b8/pyaarlo/doorbell.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2569 2023-02-06 18:29:36.000000 pyaarlo-0.8.0b8/pyaarlo/light.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6190 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b8/pyaarlo/location.py
--rw-r--r--   0 steve     (1000) steve     (1000)    12449 2021-04-08 13:02:02.000000 pyaarlo-0.8.0b8/pyaarlo/main.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    16749 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/media.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5412 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/ratls.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3801 2022-03-03 18:35:12.000000 pyaarlo-0.8.0b8/pyaarlo/security_utils.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1701 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b8/pyaarlo/sensor.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6294 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/sseclient.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2259 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/storage.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5183 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b8/pyaarlo/super.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7381 2022-11-27 01:24:01.000000 pyaarlo-0.8.0b8/pyaarlo/tfa.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3365 2021-11-28 01:11:18.000000 pyaarlo-0.8.0b8/pyaarlo/util.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.664292 pyaarlo-0.8.0b8/pyaarlo.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      623 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       51 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/entry_points.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       82 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        8 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/top_level.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-05-31 18:16:25.668292 pyaarlo-0.8.0b8/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)     1847 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/setup.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.664292 pyaarlo-0.8.0b8/tests/
--rw-rw-r--   0 steve     (1000) steve     (1000)      269 2022-10-27 13:44:57.000000 pyaarlo-0.8.0b8/tests/test_backend.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-07-05 20:39:12.686228 pyaarlo-0.8.0b9/
+-rw-r--r--   0 steve     (1000) steve     (1000)     7652 2019-08-16 18:58:59.000000 pyaarlo-0.8.0b9/LICENSE
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-07-05 20:39:12.686228 pyaarlo-0.8.0b9/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)    18439 2022-02-13 14:58:05.000000 pyaarlo-0.8.0b9/README.md
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-07-05 20:39:12.682228 pyaarlo-0.8.0b9/pyaarlo/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    27069 2023-07-04 17:24:07.000000 pyaarlo-0.8.0b9/pyaarlo/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    43523 2023-07-04 17:24:07.000000 pyaarlo-0.8.0b9/pyaarlo/backend.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4925 2023-05-10 01:20:55.000000 pyaarlo-0.8.0b9/pyaarlo/background.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    22075 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b9/pyaarlo/base.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    50293 2023-04-11 00:17:07.000000 pyaarlo-0.8.0b9/pyaarlo/camera.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6630 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b9/pyaarlo/cfg.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     9510 2023-07-04 17:24:07.000000 pyaarlo-0.8.0b9/pyaarlo/constant.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    11646 2023-02-06 16:43:11.000000 pyaarlo-0.8.0b9/pyaarlo/device.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7676 2022-10-27 14:08:34.000000 pyaarlo-0.8.0b9/pyaarlo/doorbell.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2569 2023-02-06 18:29:36.000000 pyaarlo-0.8.0b9/pyaarlo/light.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6190 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b9/pyaarlo/location.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    12449 2021-04-08 13:02:02.000000 pyaarlo-0.8.0b9/pyaarlo/main.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    16749 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b9/pyaarlo/media.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5412 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b9/pyaarlo/ratls.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3801 2022-03-03 18:35:12.000000 pyaarlo-0.8.0b9/pyaarlo/security_utils.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1701 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b9/pyaarlo/sensor.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6294 2023-07-03 12:15:23.000000 pyaarlo-0.8.0b9/pyaarlo/sseclient.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2259 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b9/pyaarlo/storage.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5183 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b9/pyaarlo/super.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7381 2022-11-27 01:24:01.000000 pyaarlo-0.8.0b9/pyaarlo/tfa.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3365 2021-11-28 01:11:18.000000 pyaarlo-0.8.0b9/pyaarlo/util.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-07-05 20:39:12.686228 pyaarlo-0.8.0b9/pyaarlo.egg-info/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-07-05 20:39:12.000000 pyaarlo-0.8.0b9/pyaarlo.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)      623 2023-07-05 20:39:12.000000 pyaarlo-0.8.0b9/pyaarlo.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-07-05 20:39:12.000000 pyaarlo-0.8.0b9/pyaarlo.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       51 2023-07-05 20:39:12.000000 pyaarlo-0.8.0b9/pyaarlo.egg-info/entry_points.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       82 2023-07-05 20:39:12.000000 pyaarlo-0.8.0b9/pyaarlo.egg-info/requires.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        8 2023-07-05 20:39:12.000000 pyaarlo-0.8.0b9/pyaarlo.egg-info/top_level.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-07-05 20:39:12.686228 pyaarlo-0.8.0b9/setup.cfg
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1847 2023-07-04 17:24:07.000000 pyaarlo-0.8.0b9/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-07-05 20:39:12.686228 pyaarlo-0.8.0b9/tests/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      269 2022-10-27 13:44:57.000000 pyaarlo-0.8.0b9/tests/test_backend.py
```

### Comparing `pyaarlo-0.8.0b8/LICENSE` & `pyaarlo-0.8.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/PKG-INFO` & `pyaarlo-0.8.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaarlo
-Version: 0.8.0b8
+Version: 0.8.0b9
 Summary: PyAarlo is a library that provides asynchronous access to Arlo security cameras.
 Home-page: https://github.com/twrecked/pyaarlo.git
 Author: Steve Herrell
 Author-email: steve.herrell@gmail.com
 License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/twrecked/pyaarlo/issues
 Project-URL: Documentation, https://github.com/twrecked/pyaarlo/blob/master/README.md
```

### Comparing `pyaarlo-0.8.0b8/README.md` & `pyaarlo-0.8.0b9/README.md`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/__init__.py` & `pyaarlo-0.8.0b9/pyaarlo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .storage import ArloStorage
 from .location import ArloLocation
 from .sensor import ArloSensor
 from .util import time_to_arlotime
 
 _LOGGER = logging.getLogger("pyaarlo")
 
-__version__ = "0.8.0b8"
+__version__ = "0.8.0b9"
 
 
 class PyArlo(object):
     """Entry point for all Arlo operations.
 
     This is used to login to Arlo, open and maintain an evenstream with Arlo, find and store devices and device
     state, provide keep-alive services and make sure media sources are kept up to date.
```

### Comparing `pyaarlo-0.8.0b8/pyaarlo/backend.py` & `pyaarlo-0.8.0b9/pyaarlo/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,27 +548,27 @@
         # get stream, restart after requested seconds of inactivity or forced close
         try:
             if self._arlo.cfg.stream_timeout == 0:
                 self.debug("starting stream with no timeout")
                 self._event_client = SSEClient(
                     self._arlo,
                     self._arlo.cfg.host + SUBSCRIBE_PATH,
-                    session=self._session,
+                    headers=self._headers(),
                     reconnect_cb=self._sse_reconnected,
                 )
             else:
                 self.debug(
                     "starting stream with {} timeout".format(
                         self._arlo.cfg.stream_timeout
                     )
                 )
                 self._event_client = SSEClient(
                     self._arlo,
                     self._arlo.cfg.host + SUBSCRIBE_PATH,
-                    session=self._session,
+                    headers=self._headers(),
                     reconnect_cb=self._sse_reconnected,
                     timeout=self._arlo.cfg.stream_timeout,
                 )
 
             for event in self._event_client:
 
                 # stopped?
@@ -669,28 +669,61 @@
         self._token = body["token"]
         self._token64 = to_b64(self._token)
         self._user_id = body["userId"]
         self._web_id = self._user_id + "_web"
         self._sub_id = "subscriptions/" + self._web_id
         self._expires_in = body["expiresIn"]
 
-    def _auth(self):
-        headers = {
+    def _auth_headers(self):
+        return {
             "Accept": "application/json, text/plain, */*",
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
+            "Cache-Control": "no-cache",
             "Origin": ORIGIN_HOST,
+            "Pragma": "no-cache",
             "Referer": REFERER_HOST,
+            # "Sec-Ch-Ua": '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+            # "Sec-Ch-Ua-Mobile": "?0",
+            # "Sec-Ch-Ua-Platform": "Linux",
+            # "Sec-Fetch-Dest": "empty",
+            # "Sec-Fetch-Mode": "cors",
+            # "Sec-Fetch-Site": "same-site",
             "Source": "arloCamWeb",
             "User-Agent": self._user_agent,
-            "x-user-device-id": self._user_device_id,
-            "x-user-device-automation-name": "QlJPV1NFUg==",
-            "x-user-device-type": "BROWSER",
+            "X-User-Device-Automation-name": "QlJPV1NFUg==",
+            "X-User-Device-Id": self._user_device_id,
+            "X-User-Device-Type": "BROWSER",
+        }
+
+    def _headers(self):
+        return {
+            "Accept": "application/json",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
+            "Auth-Version": "2",
+            "Authorization": self._token,
+            "Cache-Control": "no-cache",
+            "Content-Type": "application/json; charset=utf-8;",
+            "Origin": ORIGIN_HOST,
+            "Pragma": "no-cache",
+            "Referer": REFERER_HOST,
+            # "SchemaVersion": "1",
+            # "Sec-Ch-Ua": '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+            # "Sec-Ch-Ua-Mobile": "?0",
+            # "Sec-Ch-Ua-Platform": "Linux",
+            # "Sec-Fetch-Dest": "empty",
+            # "Sec-Fetch-Mode": "cors",
+            # "Sec-Fetch-Site": "same-site",
+            "User-Agent": self._user_agent,
         }
 
+    def _auth(self):
+        headers = self._auth_headers()
+
         # Handle 1015 error
         attempt = 0
         body = None
         while attempt < 3:
             attempt += 1
             self.debug("login attempt #{}".format(attempt))
             body = self.auth_post(
@@ -794,15 +827,20 @@
                     self._arlo.error("2fa finishAuth failed")
                     return False
             else:
                 # start authentication
                 self.debug(
                     "starting auth with {}".format(self._arlo.cfg.tfa_type)
                 )
-                body = self.auth_post(AUTH_START_PATH, {"factorId": factor_id}, headers)
+                payload = {
+                    "factorId": factor_id,
+                    "factorType": "",
+                    "userId": self._user_id
+                }
+                body = self.auth_post(AUTH_START_PATH, payload, headers)
                 if body is None:
                     self._arlo.error("2fa startAuth failed")
                     return False
                 factor_auth_code = body["factorAuthCode"]
                 tries = 1
                 while True:
                     # finish authentication
@@ -825,27 +863,16 @@
 
             # save new login information
             self._update_auth_info(body)
 
         return True
 
     def _validate(self):
-        headers = {
-            "Accept": "application/json, text/plain, */*",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
-            "Authorization": self._token64,
-            "Origin": ORIGIN_HOST,
-            "Referer": REFERER_HOST,
-            "User-Agent": self._user_agent,
-            "Source": "arloCamWeb",
-            "x-user-device-id": self._user_device_id,
-            "x-user-device-automation-name": "QlJPV1NFUg==",
-            "x-user-device-type": "BROWSER",
-        }
+        headers = self._auth_headers()
+        headers["Authorization"] = self._token64
 
         # Validate it!
         validated = self.auth_get(
             AUTH_VALIDATE_PATH + "?data = {}".format(int(time.time())), {}, headers
         )
         if validated is None:
             self._arlo.error("token validation failed")
@@ -880,27 +907,15 @@
             self._session = requests.session()
             self.debug("newish sessions, re-using")
 
         # save session in case we updated it
         self._save_session()
 
         # update sessions headers
-        headers = {
-            "Accept": "application/json",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
-            "Auth-Version": "2",
-            "Authorization": self._token,
-            "Content-Type": "application/json; charset=utf-8;",
-            "Origin": ORIGIN_HOST,
-            "Pragma": "no-cache",
-            "Referer": REFERER_HOST,
-            "SchemaVersion": "1",
-            "User-Agent": self._user_agent,
-        }
+        headers = self._headers()
         self._session.headers.update(headers)
 
         # Grab a session. Needed for new session and used to check existing
         # session. (May not really be needed for existing but will fail faster.)
         if not self._v2_session():
             if not get_new_session:
                 self._expires_in = 0
```

### Comparing `pyaarlo-0.8.0b8/pyaarlo/background.py` & `pyaarlo-0.8.0b9/pyaarlo/background.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/base.py` & `pyaarlo-0.8.0b9/pyaarlo/base.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/camera.py` & `pyaarlo-0.8.0b9/pyaarlo/camera.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/cfg.py` & `pyaarlo-0.8.0b9/pyaarlo/cfg.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/constant.py` & `pyaarlo-0.8.0b9/pyaarlo/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,12 +298,12 @@
         "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) "
         "AppleWebKit/605.1.15 (KHTML, like Gecko) Version/11.1.2 Safari/605.1.15",
     "firefox":
         "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:85.0) "
         "Gecko/20100101 Firefox/85.0",
     "linux":
         "Mozilla/5.0 (X11; Linux x86_64) "
-        "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.96 Safari/537.36"
+        "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
 }
 
 CERT_BEGIN = '-----BEGIN CERTIFICATE-----\n'
 CERT_END = '-----END CERTIFICATE-----\n'
```

### Comparing `pyaarlo-0.8.0b8/pyaarlo/device.py` & `pyaarlo-0.8.0b9/pyaarlo/device.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/doorbell.py` & `pyaarlo-0.8.0b9/pyaarlo/doorbell.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/light.py` & `pyaarlo-0.8.0b9/pyaarlo/light.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/location.py` & `pyaarlo-0.8.0b9/pyaarlo/location.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/main.py` & `pyaarlo-0.8.0b9/pyaarlo/main.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/media.py` & `pyaarlo-0.8.0b9/pyaarlo/media.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/ratls.py` & `pyaarlo-0.8.0b9/pyaarlo/ratls.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/security_utils.py` & `pyaarlo-0.8.0b9/pyaarlo/security_utils.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/sensor.py` & `pyaarlo-0.8.0b9/pyaarlo/sensor.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/sseclient.py` & `pyaarlo-0.8.0b9/pyaarlo/sseclient.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/storage.py` & `pyaarlo-0.8.0b9/pyaarlo/storage.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/super.py` & `pyaarlo-0.8.0b9/pyaarlo/super.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/tfa.py` & `pyaarlo-0.8.0b9/pyaarlo/tfa.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo/util.py` & `pyaarlo-0.8.0b9/pyaarlo/util.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/pyaarlo.egg-info/PKG-INFO` & `pyaarlo-0.8.0b9/pyaarlo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaarlo
-Version: 0.8.0b8
+Version: 0.8.0b9
 Summary: PyAarlo is a library that provides asynchronous access to Arlo security cameras.
 Home-page: https://github.com/twrecked/pyaarlo.git
 Author: Steve Herrell
 Author-email: steve.herrell@gmail.com
 License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/twrecked/pyaarlo/issues
 Project-URL: Documentation, https://github.com/twrecked/pyaarlo/blob/master/README.md
```

### Comparing `pyaarlo-0.8.0b8/pyaarlo.egg-info/SOURCES.txt` & `pyaarlo-0.8.0b9/pyaarlo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b8/setup.py` & `pyaarlo-0.8.0b9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open('README.md') as desc:
         return desc.read()
 
 
 setup(
 
     name='pyaarlo',
-    version='0.8.0b8',
+    version='0.8.0b9',
     packages=['pyaarlo'],
 
     python_requires='>=3.6',
     install_requires=[
         'requests',
         'click',
         'pycryptodome',
```

