# Comparing `tmp/wipac-rest-tools-1.4.9.tar.gz` & `tmp/wipac-rest-tools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.4.9.tar", last modified: Wed Feb 15 17:45:07 2023, max compression
+gzip compressed data, was "wipac-rest-tools-1.5.0.tar", last modified: Thu Aug  3 15:25:30 2023, max compression
```

## Comparing `wipac-rest-tools-1.4.9.tar` & `wipac-rest-tools-1.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3324 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2326 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.879011 wipac-rest-tools-1.4.9/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2023-02-15 17:45:05.000000 wipac-rest-tools-1.4.9/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.879011 wipac-rest-tools-1.4.9/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      438 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     6607 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.879011 wipac-rest-tools-1.4.9/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      691 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8781 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    12144 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    18070 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4833 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3324 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      353 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.578420 wipac-rest-tools-1.5.0/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-08-03 15:25:27.000000 wipac-rest-tools-1.5.0/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.578420 wipac-rest-tools-1.5.0/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14381 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     7380 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8781 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    12754 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    19405 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-08-03 15:25:30.586421 wipac-rest-tools-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      815 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      531 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.4.9/LICENSE` & `wipac-rest-tools-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/PKG-INFO` & `wipac-rest-tools-1.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.4.9
+Version: 1.5.0
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: telemetry
 Provides-Extra: tests
 Provides-Extra: dev
+Provides-Extra: mypy
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/wipac-rest-tools)](https://pypi.org/project/wipac-rest-tools/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/WIPACrepo/rest-tools?include_prereleases)](https://github.com/WIPACrepo/rest-tools/) [![PyPI - License](https://img.shields.io/pypi/l/wipac-rest-tools)](https://github.com/WIPACrepo/rest-tools/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/WIPACrepo/rest-tools)](https://github.com/WIPACrepo/rest-tools/) [![GitHub issues](https://img.shields.io/github/issues/WIPACrepo/rest-tools)](https://github.com/WIPACrepo/rest-tools/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/WIPACrepo/rest-tools)](https://github.com/WIPACrepo/rest-tools/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # rest-tools
 
@@ -38,36 +39,54 @@
 happens elsewhere - they do not start the loop themselves.
 
 ## Client
 
 A REST API client exists under `rest_tools.client`.  Use as:
 
 ```python
-    from rest_tools.client import RestClient
+from rest_tools.client import RestClient
 
-    api = RestClient('http://my.site.here/api', token='XXXX')
-    ret = await api.request('GET', '/fruits/apple')
-    ret = await api.request('POST', '/fruits', {'name': 'banana'})
+api = RestClient('http://my.site.here/api', token='XXXX')
+ret = await api.request('GET', '/fruits/apple')
+ret = await api.request('POST', '/fruits', {'name': 'banana'})
 ```
 
+There are several variations of the client for OAuth2/OpenID support:
+
+* [`OpenIDRestClient`](rest_tools/client/openid_client.py#L19) : A child of
+  `RestClient` that supports OAuth2 token refresh using the OpenID Connect
+  Discovery protocol for an authentication server.
+
+* [`ClientCredentialsAuth`](rest_tools/client/client_credentials.py#L11) : Uses
+  `OpenIDRestClient` in combination with OAuth2 client credentials (client ID
+  and secret) for service-based auth. Use this for long-lived services that
+  need to perform REST API calls.
+
+* [`DeviceGrantAuth`](rest_tools/client/device_client.py#L125) /
+  [`SavedDeviceGrantAuth`](rest_tools/client/device_client.py#L162) : Uses
+  `OpenIDRestClient` to perform a "device" login for a user. Use this for
+  user-based terminal applications that need to perform REST API calls.
+  The `SavedDeviceGrantAuth` can save the refresh token to disk, allowing
+  repeated application sessions without having to log in again.
+
 ## Server
 
 A REST API server exists under `rest_tools.server`. Use as:
 
 ```python
-    import asyncio
-    from rest_tools.server import RestServer, RestHandler
+import asyncio
+from rest_tools.server import RestServer, RestHandler
 
-    class Fruits(RestHandler):
-        def post(self):
-            # handle a new fruit
-            self.write({})
-
-    server = RestServer()
-    server.add_route('/fruits', Fruits)
-    server.startup(address='my.site.here', port=8080)
-    asyncio.get_event_loop().run_forever()
+class Fruits(RestHandler):
+    def post(self):
+        # handle a new fruit
+        self.write({})
+
+server = RestServer()
+server.add_route('/fruits', Fruits)
+server.startup(address='my.site.here', port=8080)
+asyncio.get_event_loop().run_forever()
 ```
 
 The server uses [Tornado](https://tornado.readthedocs.io) to handle HTTP
 connections. It is recommended to use Apache or Nginx as a front-facing proxy,
 to handle TLS sessions and non-standard HTTP requests in production.
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/__init__.py` & `wipac-rest-tools-1.5.0/rest_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.4.9"
+__version__ = "1.5.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/client/client.py` & `wipac-rest-tools-1.5.0/rest_tools/client/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,64 +2,178 @@
 
 .. _requests: http://docs.python-requests.org
 
 The REST protocol is built on http(s), with the body containing
 a json-encoded dictionary as necessary.
 """
 
-# fmt:off
+# fmt:quotes-ok
 
 import asyncio
+import dataclasses as dc
 import logging
+import math
 import os
 import time
 from typing import Any, Callable, Dict, Generator, Optional, Tuple, Union
 
 import jwt
 import requests
 
 from .. import telemetry as wtt
 from ..utils.json_util import JSONType, json_decode
 from .session import AsyncSession, Session
 
+MAX_RETRIES = 15
+
 
 def _to_str(s: Union[str, bytes]) -> str:
     if isinstance(s, bytes):
         return s.decode('utf-8')
     return s
 
 
+@dc.dataclass
+class CalcRetryFromBackoffMax:
+    """An indicator to auto-calculate the # of retries using a backoff_max.
+
+    `backoff_max` is the maximum allowed backoff time for the final
+    retry
+    """
+
+    backoff_max: float
+
+    def calculate_retries(self, backoff_factor: float) -> int:
+        """Calculate the number of retries."""
+        #                        backoff_last     =  backoff_factor * 2^(retries-1)
+        #       backoff_last / backoff_factor     =  2^(retries-1)
+        # lg( backoff_last / backoff_factor )     =  retries - 1
+        # lg( backoff_last / backoff_factor ) + 1 =  retries - 1
+        return max(
+            0,
+            int(math.log2(self.backoff_max / backoff_factor) + 1),
+        )
+
+
+@dc.dataclass
+class CalcRetryFromWaittimeMax:
+    """An indicator to auto-calculate the # of retries from total waittime.
+
+    `waittime_max` includes each attempt's timeout and each backoff time
+    """
+
+    waittime_max: float
+
+    def calculate_retries(self, timeout: float, backoff_factor: float) -> int:
+        """Calculate the number of retries (max returned -> MAX_RETRIES+1)."""
+        if self.waittime_max < timeout:
+            raise ValueError(
+                f"waittime_max ({self.waittime_max}) cannot be less than timeout ({timeout})"
+            )
+
+        # the first backoff is always 0 sec, factor applies after 2nd attempt
+        #    T + 0 + sum{n=1,retries-1}(T + 2^n * B)     + T
+        # =  T + 0 + ( T*k + B*2^((retries-1)+1) - 2*B ) + T
+        # not easily solvable (for k) in a closed form
+        for k in range(0, MAX_RETRIES + 2):  # last val -> MAX_RETRIES+1
+            if self.waittime_max > (
+                timeout
+                + (timeout * k)
+                + (backoff_factor * 2 ** (k))
+                - (2 * backoff_factor)
+                + timeout
+            ):
+                retries = k  # gets overwritten each iteration
+            else:
+                break
+        return retries
+
+
+def _log_retries_values(
+    retries: int, timeout: float, backoff_factor: float, logger: logging.Logger
+) -> None:
+    logger.info(f"using {retries=} {timeout=} {backoff_factor=}")
+    if retries:
+        retries_schema = ' '.join(
+            [f'<0.0s> {timeout}s']
+            + [f'<{(backoff_factor * 2**i)}s> {timeout}s' for i in range(1, retries)]
+        )
+        logger.info(
+            f"retry scheme (TIMEOUT [<BACKOFF> TIMEOUT ...]): "
+            f"{timeout}s {retries_schema}"
+        )
+
+
 class RestClient:
     """A REST client with token handling.
 
     Args:
-        address (str): base address of REST API
-        token (str): (optional) access token, or a function generating an access token
-        timeout (int): (optional) request timeout (default: 60s)
-        retries (int): (optional) number of retries to attempt (default: 10)
-        username (str): (optional) auth-basic username
-        password (str): (optional) auth-basic password
-        logger (logging.Logger): (optional) supply a logger to use
+        address (str):
+            base address of REST API
+        token (str):
+            (optional) access token, or a function generating an access token
+        timeout (int):
+            (optional) request timeout (default: 60s)
+        retries (int | CalcRetryFromBackoffMax | CalcRetryFromWaittimeMax):
+            (optional) number of retries to attempt (default: 10)
+            alternatively, pass in a `CalcRetryFromBackoffMax` or
+            `CalcRetryFromWaittimeMax` instance to have this auto-calculated
+        backoff_factor (float):
+            (optional) backoff factor to apply between attempts after the second try --
+            sleep for `{backoff factor} * (2 ** ({number of previous retries}))` seconds
+            "For example, if the backoff_factor is 0.1, then Retry.sleep() will sleep for [0.0s, 0.2s, 0.4s, 0.8s, ...] between retries."
+            see: https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
+        username (str):
+            (optional) auth-basic username
+        password (str):
+            (optional) auth-basic password
+        logger (logging.Logger):
+            (optional) supply a logger to use
     """
 
     def __init__(
         self,
         address: str,
         token: Optional[Union[str, bytes, Callable[[], Union[str, bytes]]]] = None,
         timeout: float = 60.0,
-        retries: int = 10,
+        retries: Union[int, CalcRetryFromBackoffMax, CalcRetryFromWaittimeMax] = 10,
+        backoff_factor: float = 0.3,
         logger: Optional[logging.Logger] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         self.address = address
-        self.timeout = timeout
-        self.retries = retries
         self.kwargs = kwargs
         self.logger = logger if logger else logging.getLogger('RestClient')
 
+        self.timeout = float(timeout)
+        if self.timeout < 0.0:
+            raise ValueError(f"timeout must be positive: {self.timeout}")
+
+        self.backoff_factor = float(backoff_factor)
+        if self.backoff_factor < 0.0:
+            raise ValueError(f"backoff_factor must be positive: {self.backoff_factor}")
+
+        # get numerical retries value
+        if isinstance(retries, CalcRetryFromBackoffMax):
+            self.retries = retries.calculate_retries(self.backoff_factor)
+        elif isinstance(retries, CalcRetryFromWaittimeMax):
+            self.retries = retries.calculate_retries(self.timeout, self.backoff_factor)
+        elif isinstance(retries, int) and retries >= 0:
+            self.retries = retries
+        else:
+            raise ValueError(
+                f"Cannot set and/or auto-calculate # of retries: {retries}"
+            )
+        # + validate
+        if self.retries > MAX_RETRIES:
+            raise ValueError(f"Cannot set # of retries above {MAX_RETRIES}")
+        _log_retries_values(
+            self.retries, self.timeout, self.backoff_factor, self.logger
+        )
+
         # token handling
         self._token_expire_delay_offset = 5
         self.access_token: Optional[Union[str, bytes]] = None
         self.token_func: Optional[Callable[[], Union[str, bytes]]] = None
         if token:
             if isinstance(token, (str, bytes)):
                 self.access_token = token
@@ -68,17 +182,23 @@
 
         self.session = self.open()  # start session
 
     def open(self, sync: bool = False) -> requests.Session:
         """Open the http session."""
         self.logger.debug('establish REST http session')
         if sync:
-            self.session = Session(self.retries)
+            self.session = Session(
+                self.retries,
+                backoff_factor=self.backoff_factor,
+            )
         else:
-            self.session = AsyncSession(self.retries)
+            self.session = AsyncSession(
+                self.retries,
+                backoff_factor=self.backoff_factor,
+            )
         self.session.headers = {  # type: ignore[assignment]
             'Content-Type': 'application/json',
         }
         if 'username' in self.kwargs and 'password' in self.kwargs:
             self.session.auth = (self.kwargs['username'], self.kwargs['password'])
         if 'sslcert' in self.kwargs:
             if 'sslkey' in self.kwargs:
@@ -101,15 +221,15 @@
             # check if expired
             try:
                 # NOTE: PyJWT mis-type-hinted arg #1 as a str, but byte is also fine
                 # https://github.com/jpadilla/pyjwt/pull/605#issuecomment-772082918
                 data = jwt.decode(
                     self.access_token,  # type: ignore[arg-type]
                     algorithms=['RS256', 'RS512'],
-                    options={"verify_signature": False}
+                    options={"verify_signature": False},
                 )
                 # account for an X second delay over the wire, so expire sooner
                 if data['exp'] < time.time() + self._token_expire_delay_offset:
                     raise Exception()
                 return
             except Exception:
                 self.access_token = None
@@ -171,15 +291,15 @@
         except Exception:
             self.logger.info('json data: %r', content)
             raise
 
     @wtt.spanned(
         span_namer=wtt.SpanNamer(use_this_arg='method'),
         these=['method', 'path', 'self.address'],
-        kind=wtt.SpanKind.CLIENT
+        kind=wtt.SpanKind.CLIENT,
     )
     async def request(
         self,
         method: str,
         path: str,
         args: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
@@ -208,15 +328,15 @@
                 raise  # skip the logging for an expected error
             self.logger.info('bad request: %s %s %r', method, path, args, exc_info=True)
             raise
 
     @wtt.spanned(
         span_namer=wtt.SpanNamer(use_this_arg='method'),
         these=['method', 'path', 'self.address'],
-        kind=wtt.SpanKind.CLIENT
+        kind=wtt.SpanKind.CLIENT,
     )
     def request_seq(
         self,
         method: str,
         path: str,
         args: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
@@ -243,15 +363,15 @@
             return self._decode(r.content)
         finally:
             self.session = s
 
     @wtt.spanned(
         span_namer=wtt.SpanNamer(use_this_arg='method'),
         these=['method', 'path', 'self.address'],
-        kind=wtt.SpanKind.CLIENT
+        kind=wtt.SpanKind.CLIENT,
     )
     def request_stream(
         self,
         method: str,
         path: str,
         args: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.5.0/rest_tools/client/client_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         self.auth = OpenIDAuth(token_url)
         self.client_id = client_id
         self.client_secret = client_secret
         super().__init__(address=address, token=self.make_access_token, logger=logging.getLogger('ClientCredentialsAuth'),
                          **kwargs)
 
     def make_access_token(self) -> str:
+        if not self.auth.token_url:
+            self.auth._refresh_keys()
+
         # try making a new token
         args = {
             'grant_type': 'client_credentials',
             'client_id': self.client_id,
             'client_secret': self.client_secret,
             'scope': 'offline_access',
         }
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/client/device_client.py` & `wipac-rest-tools-1.5.0/rest_tools/client/device_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # fmt:off
 import io
 from itertools import zip_longest
 import logging
 from pathlib import Path
 import time
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 import qrcode  # type: ignore[import]
 import requests
 
 from ..utils.auth import OpenIDAuth
 from .openid_client import OpenIDRestClient
 
@@ -122,35 +122,38 @@
     return req['refresh_token']
 
 
 def DeviceGrantAuth(
     address: str, token_url: str, client_id: str,
     client_secret: Optional[str] = None,
     scopes: Optional[List[str]] = None,
+    **kwargs: Any,
 ) -> OpenIDRestClient:
     """A REST client that can handle OpenID and the OAuth2 Device Client flow.
 
     Args:
         address (str): base address of REST API
         token_url (str): base address of token service
         client_id (str): client id
         client_secret (str): client secret (optional - required for confidential clients)
         scopes (list): token scope list (optional)
+        timeout (int): request timeout (optional)
+        retries (int): number of retries to attempt (optional)
     """
     logger = logging.getLogger('DeviceGrantAuth')
 
     auth = OpenIDAuth(token_url)
     if 'device_authorization_endpoint' not in auth.provider_info:
         raise RuntimeError('Device grant not supported by server')
     endpoint = auth.provider_info['device_authorization_endpoint']
 
     refresh_token = _perform_device_grant(logger, endpoint, auth.token_url, client_id, client_secret, scopes)
 
     return OpenIDRestClient(address=address, token_url=token_url, client_id=client_id,
-                            client_secret=client_secret, refresh_token=refresh_token)
+                            client_secret=client_secret, refresh_token=refresh_token, **kwargs)
 
 
 def _load_token_from_file(filepath: Path) -> Optional[str]:
     if filepath.exists():
         return filepath.read_text()
     return None
 
@@ -161,39 +164,51 @@
 
 def SavedDeviceGrantAuth(
     address: str, token_url: str,
     filename: str,
     client_id: str,
     client_secret: Optional[str] = None,
     scopes: Optional[List[str]] = None,
+    **kwargs: Any,
 ) -> OpenIDRestClient:
     """
     A REST client that can handle OpenID and the OAuth2 Device Client flow,
     and saves a refresh token to a file for quick access.
 
     Args:
         address (str): base address of REST API
         token_url (str): base address of token service
         filename (str): name of file to save/load refresh token
         client_id (str): client id
         client_secret (str): client secret (optional - required for confidential clients)
         scopes (list): token scope list (optional)
+        timeout (int): request timeout (optional)
+        retries (int): number of retries to attempt (optional)
     """
     logger = logging.getLogger('SavedDeviceGrantAuth')
+    filepath = Path(filename)
+
+    def update_func(access, refresh):
+        _save_token_to_file(filepath, refresh)
+
+    refresh_token = _load_token_from_file(filepath)
+    if refresh_token:
+        try:
+            # this will try to refresh, and raise if it fails
+            return OpenIDRestClient(address=address, token_url=token_url, client_id=client_id,
+                                    client_secret=client_secret, refresh_token=refresh_token,
+                                    update_func=update_func, **kwargs)
+        except Exception:
+            pass
 
     auth = OpenIDAuth(token_url)
+    if not auth.provider_info:
+        raise RuntimeError('Token service does not support .well-known discovery')
     if 'device_authorization_endpoint' not in auth.provider_info:
         raise RuntimeError('Device grant not supported by server')
     endpoint = auth.provider_info['device_authorization_endpoint']
 
-    filepath = Path(filename)
-    refresh_token = _load_token_from_file(filepath)
-
-    if not refresh_token:
-        refresh_token = _perform_device_grant(logger, endpoint, auth.token_url, client_id, client_secret, scopes)
-
-    def update_func(access, refresh):
-        _save_token_to_file(filepath, refresh)
+    refresh_token = _perform_device_grant(logger, endpoint, auth.token_url, client_id, client_secret, scopes)
 
     return OpenIDRestClient(address=address, token_url=token_url, client_id=client_id,
                             client_secret=client_secret, refresh_token=refresh_token,
-                            update_func=update_func)
+                            update_func=update_func, **kwargs)
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.5.0/rest_tools/client/openid_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         super().__init__(address, logger=logging.getLogger('OpenIDRestClient'),
                          token=self._openid_token, **kwargs)
 
         # initial call to verify things work
         self._openid_token()
 
     def _openid_token(self) -> str:
+        if not self.auth.token_url:
+            self.auth._refresh_keys()
+
         # try the refresh token
         args = {
             'grant_type': 'refresh_token',
             'refresh_token': self.refresh_token,
             'client_id': self.client_id,
         }
         if self.client_secret:
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/client/session.py` & `wipac-rest-tools-1.5.0/rest_tools/client/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 .. _requests: http://docs.python-requests.org
 """
 
 # fmt:off
 # pylint: skip-file
 
-from typing import Iterable
+from typing import Collection
 
 import requests
 from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry  # type: ignore[import]
 from requests_futures.sessions import FuturesSession  # type: ignore[import]
+from urllib3.util.retry import Retry
 
 
 def AsyncSession(
-    retries: int = 10,
-    backoff_factor: float = 0.3,
-    allowed_methods: Iterable[str] = ('HEAD', 'TRACE', 'GET', 'POST', 'PUT', 'OPTIONS', 'DELETE'),
-    status_forcelist: Iterable[int] = (408, 429, 500, 502, 503, 504),
+    retries: int,
+    backoff_factor: float,
+    allowed_methods: Collection[str] = ('HEAD', 'TRACE', 'GET', 'POST', 'PUT', 'OPTIONS', 'DELETE'),
+    status_forcelist: Collection[int] = (408, 429, 500, 502, 503, 504),
 ) -> FuturesSession:
     """Return a Session object with full retry capabilities.
 
     Args:
         retries (int): number of retries
         backoff_factor (float): speed factor for retries (in seconds)
-        allowed_methods (iterable): http methods to retry on
-        status_forcelist (iterable): http status codes to retry on
+        allowed_methods (collection): http methods to retry on
+        status_forcelist (collection): http status codes to retry on
 
     Returns:
         :py:class:`requests.Session`: session object
     """
     session = FuturesSession()
     retry = Retry(
         total=retries,
@@ -45,26 +45,26 @@
     adapter = HTTPAdapter(max_retries=retry)
     session.mount('http://', adapter)
     session.mount('https://', adapter)
     return session
 
 
 def Session(
-    retries: int = 10,
-    backoff_factor: float = 0.3,
-    allowed_methods: Iterable[str] = ('HEAD', 'TRACE', 'GET', 'POST', 'PUT', 'OPTIONS', 'DELETE'),
-    status_forcelist: Iterable[int] = (408, 429, 500, 502, 503, 504),
+    retries: int,
+    backoff_factor: float,
+    allowed_methods: Collection[str] = ('HEAD', 'TRACE', 'GET', 'POST', 'PUT', 'OPTIONS', 'DELETE'),
+    status_forcelist: Collection[int] = (408, 429, 500, 502, 503, 504),
 ) -> requests.Session:
     """Return a Session object with full retry capabilities.
 
     Args:
         retries (int): number of retries
         backoff_factor (float): speed factor for retries (in seconds)
-        allowed_methods (iterable): http methods to retry on
-        status_forcelist (iterable): http status codes to retry on
+        allowed_methods (collection): http methods to retry on
+        status_forcelist (collection): http status codes to retry on
 
     Returns:
         :py:class:`requests.Session`: session object
     """
     session = requests.Session()
     retry = Retry(
         total=retries,
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/server/__init__.py` & `wipac-rest-tools-1.5.0/rest_tools/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     scope_role_auth,
     keycloak_role_auth,
     token_attribute_role_mapping_auth,
 )
 from .handler import (
     RestHandler,
     RestHandlerSetup,
-    OpenIDWebHandlerMixin,
     KeycloakUsernameMixin,
+    OpenIDCookieHandlerMixin,
     OpenIDLoginHandler,
 )
 from .server import RestServer
 
 __all__ = [
     "RestServer",
     "RestHandlerSetup",
     "RestHandler",
-    "OpenIDWebHandlerMixin",
     "KeycloakUsernameMixin",
+    "OpenIDCookieHandlerMixin",
     "OpenIDLoginHandler",
     "authenticated",
     "catch_error",
     "role_authorization",
     "scope_role_auth",
     "keycloak_role_auth",
     "token_attribute_role_mapping_auth",
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.5.0/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/rest_tools/server/decorators.py` & `wipac-rest-tools-1.5.0/rest_tools/server/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from functools import wraps
 from inspect import isawaitable
 import logging
 import re
 
+import requests.exceptions
 import tornado.web
 
 from .. import telemetry as wtt
 
 logger = logging.getLogger('auth_decorators')
 
 
@@ -46,14 +47,27 @@
                 return await ret
             else:
                 return ret
         except tornado.web.HTTPError:
             raise  # tornado can handle this
         except tornado.httpclient.HTTPError:
             raise  # tornado can handle this
+        except requests.exceptions.HTTPError as e:
+            logger.warning('Error in website handler', exc_info=True)
+            try:
+                self.statsd.incr(self.__class__.__name__+'.error')
+            except Exception:
+                pass  # ignore statsd errors
+            if e.response.status_code == 403:
+                code = 403
+                message = 'Error authenticating user'
+            else:
+                code = 500
+                message = 'Error contacting backend in '+self.__class__.__name__
+            self.send_error(code, reason=message)
         except Exception:
             logger.warning('Error in website handler', exc_info=True)
             try:
                 self.statsd.incr(self.__class__.__name__+'.error')
             except Exception:
                 pass  # ignore statsd errors
             message = 'Error in '+self.__class__.__name__
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/server/handler.py` & `wipac-rest-tools-1.5.0/rest_tools/server/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,36 +264,14 @@
             type,
             choices,
             forbiddens,
             strict_type,
         )
 
 
-class OpenIDWebHandlerMixin:
-    """Load current user from `OpenIDLoginHandler` cookies."""
-    def get_current_user(self):
-        """Get the current user, and set auth-related attributes."""
-        try:
-            access_token = self.get_secure_cookie('access_token')
-            logging.debug('access_token: %r', access_token)
-            refresh_token = self.get_secure_cookie('refresh_token')
-            if isinstance(access_token, str):
-                access_token = access_token.encode('utf8')
-            data = self.auth.validate(access_token)
-            self.auth_data = data
-            self.auth_key = access_token
-            self.auth_refresh_token = refresh_token
-            return data['sub']
-        # Auth Failed
-        except Exception:
-            logger.info('failed auth', exc_info=True)
-
-        return None
-
-
 class KeycloakUsernameMixin:
     """Get the username correctly from Keycloak tokens.
 
     Note: will not work on service account tokens.
     """
     def get_current_user(self):
         if not super().get_current_user():
@@ -302,17 +280,76 @@
         if not username:
             username = self.auth_data.get('upn', None)
             if not username:
                 logger.info('could not find auth username')
         return username
 
 
-class OpenIDLoginHandler(RestHandler, OAuth2Mixin):
+class OpenIDCookieHandlerMixin:
+    """Store/load current user's `OpenIDLoginHandler` tokens in cookies."""
+    def get_current_user(self):
+        """Get the current user, and set auth-related attributes."""
+        try:
+            access_token = self.get_secure_cookie('access_token')
+            data = self.auth.validate(access_token)
+            self.auth_data = data
+            self.auth_key = access_token
+            refresh_token = self.get_secure_cookie('refresh_token')
+            self.auth_refresh_token = refresh_token
+            return data['sub']
+        # Auth Failed
+        except Exception:
+            logger.debug('failed auth', exc_info=True)
+
+        return None
+
+    def store_tokens(
+        self,
+        access_token,
+        access_token_exp,
+        refresh_token=None,
+        refresh_token_exp=None,
+        user_info=None,
+        user_info_exp=None,
+    ):
+        """
+        Store jwt tokens and user info from OpenID-compliant auth source.
+
+        Args:
+            access_token (str): jwt access token
+            access_token_exp (int): access token expiration in seconds
+            refresh_token (str): jwt refresh token
+            refresh_token_exp (int): refresh token expiration in seconds
+            user_info (dict): user info (from id token or user info lookup)
+            user_info_exp (int): user info expiration in seconds
+        """
+        self.set_secure_cookie('access_token', access_token,
+                               expires_days=float(access_token_exp)/3600/24)
+        if refresh_token and refresh_token_exp:
+            self.set_secure_cookie('refresh_token', refresh_token,
+                                   expires_days=float(refresh_token_exp)/3600/24)
+        if user_info and user_info_exp:
+            self.set_secure_cookie('user_info', tornado.escape.json_encode(user_info),
+                                   expires_days=float(user_info_exp)/3600/24)
+
+    def clear_tokens(self):
+        """
+        Clear token data, usually on logout.
+        """
+        self.clear_cookie('access_token')
+        self.clear_cookie('refresh_token')
+        self.clear_cookie('user_info')
+
+
+class OpenIDLoginHandler(OpenIDCookieHandlerMixin, OAuth2Mixin, RestHandler):
     """Handle OpenID Connect logins.
 
+    Should be combined with an appropriate mixin to store the token(s).
+    `OpenIDCookieHandlerMixin` is used by default, but can be overridden.
+
     Requires the `login_url` application setting to be a full url.
     """
     _pkcs_challenges: MutableMapping[str, str] = TTLCache(maxsize=10000, ttl=3600)
 
     def initialize(self, oauth_client_id, oauth_client_secret, oauth_client_scope=None, **kwargs):
         super().initialize(**kwargs)
         if not isinstance(self.auth, OpenIDAuth):
@@ -419,22 +456,24 @@
             access_expire = user.get('expires_in', 0)
             if not access_expire:
                 access_expire = 1800
             refresh_expire = user.get('refresh_expires_in', 0)
             if not refresh_expire:
                 refresh_expire = 86400
 
-            # Save the user with e.g. set_secure_cookie
-            self.set_secure_cookie('access_token', user['access_token'],
-                                   expires_days=float(access_expire)/3600/24)
-            if 'refresh_token' in user:
-                self.set_secure_cookie('refresh_token', user['refresh_token'],
-                                       expires_days=float(refresh_expire)/3600/24)
-            self.set_secure_cookie('identity', tornado.escape.json_encode(user['id_token']),
-                                   expires_days=float(refresh_expire)/3600/24)
+            # Save the user data
+            self.store_tokens(
+                access_token=user['access_token'],
+                access_token_exp=access_expire,
+                refresh_token=user.get('refresh_token'),
+                refresh_token_exp=refresh_expire,
+                user_info=user.get('id_token'),
+                user_info_exp=refresh_expire if user.get('refresh_token') else access_expire,
+            )
+
             if data.get('redirect', None):
                 url = data['redirect']
                 if 'state' in data:
                     url = tornado.httputil.url_concact(url, {'state': data['state']})
                 self.redirect(url)
             elif self.settings.get('debug', False):
                 self.write(user)
```

### Comparing `wipac-rest-tools-1.4.9/rest_tools/server/server.py` & `wipac-rest-tools-1.5.0/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/rest_tools/server/stats.py` & `wipac-rest-tools-1.5.0/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/rest_tools/telemetry.py` & `wipac-rest-tools-1.5.0/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/rest_tools/utils/auth.py` & `wipac-rest-tools-1.5.0/rest_tools/utils/auth.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.5.0/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.5.0/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.9/setup.cfg` & `wipac-rest-tools-1.5.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -37,23 +37,24 @@
 	Tracker = https://github.com/WIPACrepo/rest-tools/issues
 	Source = https://github.com/WIPACrepo/rest-tools
 
 [semantic_release]
 version_variable = rest_tools/__init__.py:__version__
 upload_to_pypi = True
 patch_without_tag = True
-commit_parser = semantic_release.history.tag_parser
-minor_tag = [minor]
-fix_tag = [fix]
+commit_parser = semantic_release.history.emoji_parser
+major_emoji = [major]
+minor_emoji = [minor]
+patch_emoji = [fix], [patch]
 branch = master
 
 [options]
 install_requires = 
 	cachetools
-	pyjwt[crypto]<=2.5.0
+	pyjwt[crypto]!=2.6.0
 	qrcode
 	requests
 	requests-futures
 	tornado
 	wipac-dev-tools
 python_requires = >=3.8, <3.12
 packages = find:
@@ -67,26 +68,32 @@
 	httpretty
 	pycycle
 	pytest
 	pytest-asyncio
 	pytest-cov
 	pytest-mock
 	requests-mock
+	ruff
 	types-requests
 dev = 
 	cryptography
 	flake8
 	httpretty
 	mypy
 	pytest
 	pytest-asyncio
 	pytest-mock
 	requests-mock
+	ruff
 	types-requests
 	wheel
+mypy = 
+	%(telemetry)s
+	%(tests)s
+	%(dev)s
 
 [options.package_data]
 * = py.typed
 
 [options.packages.find]
 exclude = 
 	test
```

### Comparing `wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.4.9
+Version: 1.5.0
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: telemetry
 Provides-Extra: tests
 Provides-Extra: dev
+Provides-Extra: mypy
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/wipac-rest-tools)](https://pypi.org/project/wipac-rest-tools/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/WIPACrepo/rest-tools?include_prereleases)](https://github.com/WIPACrepo/rest-tools/) [![PyPI - License](https://img.shields.io/pypi/l/wipac-rest-tools)](https://github.com/WIPACrepo/rest-tools/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/WIPACrepo/rest-tools)](https://github.com/WIPACrepo/rest-tools/) [![GitHub issues](https://img.shields.io/github/issues/WIPACrepo/rest-tools)](https://github.com/WIPACrepo/rest-tools/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/WIPACrepo/rest-tools)](https://github.com/WIPACrepo/rest-tools/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # rest-tools
 
@@ -38,36 +39,54 @@
 happens elsewhere - they do not start the loop themselves.
 
 ## Client
 
 A REST API client exists under `rest_tools.client`.  Use as:
 
 ```python
-    from rest_tools.client import RestClient
+from rest_tools.client import RestClient
 
-    api = RestClient('http://my.site.here/api', token='XXXX')
-    ret = await api.request('GET', '/fruits/apple')
-    ret = await api.request('POST', '/fruits', {'name': 'banana'})
+api = RestClient('http://my.site.here/api', token='XXXX')
+ret = await api.request('GET', '/fruits/apple')
+ret = await api.request('POST', '/fruits', {'name': 'banana'})
 ```
 
+There are several variations of the client for OAuth2/OpenID support:
+
+* [`OpenIDRestClient`](rest_tools/client/openid_client.py#L19) : A child of
+  `RestClient` that supports OAuth2 token refresh using the OpenID Connect
+  Discovery protocol for an authentication server.
+
+* [`ClientCredentialsAuth`](rest_tools/client/client_credentials.py#L11) : Uses
+  `OpenIDRestClient` in combination with OAuth2 client credentials (client ID
+  and secret) for service-based auth. Use this for long-lived services that
+  need to perform REST API calls.
+
+* [`DeviceGrantAuth`](rest_tools/client/device_client.py#L125) /
+  [`SavedDeviceGrantAuth`](rest_tools/client/device_client.py#L162) : Uses
+  `OpenIDRestClient` to perform a "device" login for a user. Use this for
+  user-based terminal applications that need to perform REST API calls.
+  The `SavedDeviceGrantAuth` can save the refresh token to disk, allowing
+  repeated application sessions without having to log in again.
+
 ## Server
 
 A REST API server exists under `rest_tools.server`. Use as:
 
 ```python
-    import asyncio
-    from rest_tools.server import RestServer, RestHandler
+import asyncio
+from rest_tools.server import RestServer, RestHandler
 
-    class Fruits(RestHandler):
-        def post(self):
-            # handle a new fruit
-            self.write({})
-
-    server = RestServer()
-    server.add_route('/fruits', Fruits)
-    server.startup(address='my.site.here', port=8080)
-    asyncio.get_event_loop().run_forever()
+class Fruits(RestHandler):
+    def post(self):
+        # handle a new fruit
+        self.write({})
+
+server = RestServer()
+server.add_route('/fruits', Fruits)
+server.startup(address='my.site.here', port=8080)
+asyncio.get_event_loop().run_forever()
 ```
 
 The server uses [Tornado](https://tornado.readthedocs.io) to handle HTTP
 connections. It is recommended to use Apache or Nginx as a front-facing proxy,
 to handle TLS sessions and non-standard HTTP requests in production.
```

### Comparing `wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

