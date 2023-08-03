# Comparing `tmp/stakefish-web3-utils-0.1.0.tar.gz` & `tmp/stakefish-web3-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/stakefish/code/web3-utils/dist/.tmp-jwu7va52/stakefish-web3-utils-0.1.0.tar", last modified: Mon Jul 17 08:06:42 2023, max compression
+gzip compressed data, was "stakefish-web3-utils-0.2.0.tar", last modified: Thu Aug  3 13:20:42 2023, max compression
```

## Comparing `stakefish-web3-utils-0.1.0.tar` & `stakefish-web3-utils-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.705100 stakefish-web3-utils-0.1.0/
--rw-r--r--   0 stakefish   (502) staff       (20)     1082 2023-01-12 15:11:34.000000 stakefish-web3-utils-0.1.0/LICENSE.md
--rw-r--r--   0 stakefish   (502) staff       (20)     1370 2023-07-17 08:06:42.705369 stakefish-web3-utils-0.1.0/PKG-INFO
--rw-r--r--   0 stakefish   (502) staff       (20)      810 2023-01-12 15:11:34.000000 stakefish-web3-utils-0.1.0/README.rst
--rw-r--r--   0 stakefish   (502) staff       (20)      187 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/pyproject.toml
--rw-r--r--   0 stakefish   (502) staff       (20)      796 2023-07-17 08:06:42.706436 stakefish-web3-utils-0.1.0/setup.cfg
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.686877 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/
--rw-r--r--   0 stakefish   (502) staff       (20)     1370 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/PKG-INFO
--rw-r--r--   0 stakefish   (502) staff       (20)     1060 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/SOURCES.txt
--rw-r--r--   0 stakefish   (502) staff       (20)        1 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/dependency_links.txt
--rw-r--r--   0 stakefish   (502) staff       (20)        1 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/not-zip-safe
--rw-r--r--   0 stakefish   (502) staff       (20)       62 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/requires.txt
--rw-r--r--   0 stakefish   (502) staff       (20)       11 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/top_level.txt
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.695702 stakefish-web3-utils-0.1.0/tests/
--rw-r--r--   0 stakefish   (502) staff       (20)     2799 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/tests/test_async_beacon.py
--rw-r--r--   0 stakefish   (502) staff       (20)      207 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_compute_time_at_slot.py
--rw-r--r--   0 stakefish   (502) staff       (20)      269 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_convert_to_standard_notation.py
--rw-r--r--   0 stakefish   (502) staff       (20)      635 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/tests/test_divide_chunks.py
--rw-r--r--   0 stakefish   (502) staff       (20)      320 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/tests/test_gwei_to_wei.py
--rw-r--r--   0 stakefish   (502) staff       (20)      228 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_hash_event_param.py
--rw-r--r--   0 stakefish   (502) staff       (20)      256 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_is_null_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)      289 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/tests/test_normalize_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)     3991 2023-03-30 11:06:22.000000 stakefish-web3-utils-0.1.0/tests/test_retryable_eth_module.py
--rw-r--r--   0 stakefish   (502) staff       (20)      628 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_split_validator_pubkey_bytes.py
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.704613 stakefish-web3-utils-0.1.0/web3_utils/
--rw-r--r--   0 stakefish   (502) staff       (20)        0 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/web3_utils/__init__.py
--rw-r--r--   0 stakefish   (502) staff       (20)     3779 2023-07-17 07:58:36.000000 stakefish-web3-utils-0.1.0/web3_utils/async_beacon.py
--rw-r--r--   0 stakefish   (502) staff       (20)      343 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/calculate_max_fees.py
--rw-r--r--   0 stakefish   (502) staff       (20)      130 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/compute_time_at_slot.py
--rw-r--r--   0 stakefish   (502) staff       (20)      168 2023-03-30 10:43:41.000000 stakefish-web3-utils-0.1.0/web3_utils/convert_to_standard_notation.py
--rw-r--r--   0 stakefish   (502) staff       (20)      284 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/current_utc_timestamp.py
--rw-r--r--   0 stakefish   (502) staff       (20)      138 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/web3_utils/divide_chunks.py
--rw-r--r--   0 stakefish   (502) staff       (20)      111 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/gwei_to_wei.py
--rw-r--r--   0 stakefish   (502) staff       (20)      126 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/hash_event_param.py
--rw-r--r--   0 stakefish   (502) staff       (20)      241 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/is_null_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)      301 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/normalize_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)     3050 2023-03-30 10:45:11.000000 stakefish-web3-utils-0.1.0/web3_utils/retryable_eth_module.py
--rw-r--r--   0 stakefish   (502) staff       (20)      336 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/split_validator_pubkey_bytes.py
+drwxr-xr-x   0 mbaranovski   (501) staff       (20)        0 2023-08-03 13:20:42.520993 stakefish-web3-utils-0.2.0/
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     1082 2023-02-03 11:51:15.000000 stakefish-web3-utils-0.2.0/LICENSE.md
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     1370 2023-08-03 13:20:42.521047 stakefish-web3-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      810 2023-02-03 11:51:15.000000 stakefish-web3-utils-0.2.0/README.rst
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      187 2023-01-06 10:24:44.000000 stakefish-web3-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      796 2023-08-03 13:20:42.521278 stakefish-web3-utils-0.2.0/setup.cfg
+drwxr-xr-x   0 mbaranovski   (501) staff       (20)        0 2023-08-03 13:20:42.517232 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     1370 2023-08-03 13:20:42.000000 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     1060 2023-08-03 13:20:42.000000 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaranovski   (501) staff       (20)        1 2023-08-03 13:20:42.000000 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaranovski   (501) staff       (20)        1 2023-08-03 13:20:42.000000 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/not-zip-safe
+-rw-r--r--   0 mbaranovski   (501) staff       (20)       62 2023-08-03 13:20:42.000000 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/requires.txt
+-rw-r--r--   0 mbaranovski   (501) staff       (20)       11 2023-08-03 13:20:42.000000 stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mbaranovski   (501) staff       (20)        0 2023-08-03 13:20:42.519014 stakefish-web3-utils-0.2.0/tests/
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     2799 2023-01-09 10:39:33.000000 stakefish-web3-utils-0.2.0/tests/test_async_beacon.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      207 2023-01-10 12:25:40.000000 stakefish-web3-utils-0.2.0/tests/test_compute_time_at_slot.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      269 2023-01-10 12:25:40.000000 stakefish-web3-utils-0.2.0/tests/test_convert_to_standard_notation.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      635 2023-01-06 10:24:44.000000 stakefish-web3-utils-0.2.0/tests/test_divide_chunks.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      320 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/tests/test_gwei_to_wei.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      228 2023-01-10 12:25:40.000000 stakefish-web3-utils-0.2.0/tests/test_hash_event_param.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      256 2023-01-10 12:25:40.000000 stakefish-web3-utils-0.2.0/tests/test_is_null_address.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      289 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/tests/test_normalize_address.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     4429 2023-08-03 13:19:47.000000 stakefish-web3-utils-0.2.0/tests/test_retryable_eth_module.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      628 2023-01-10 12:25:40.000000 stakefish-web3-utils-0.2.0/tests/test_split_validator_pubkey_bytes.py
+drwxr-xr-x   0 mbaranovski   (501) staff       (20)        0 2023-08-03 13:20:42.520881 stakefish-web3-utils-0.2.0/web3_utils/
+-rw-r--r--   0 mbaranovski   (501) staff       (20)        0 2023-01-06 10:24:44.000000 stakefish-web3-utils-0.2.0/web3_utils/__init__.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     3779 2023-08-03 13:17:31.000000 stakefish-web3-utils-0.2.0/web3_utils/async_beacon.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      343 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/calculate_max_fees.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      130 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/compute_time_at_slot.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      168 2023-02-03 13:28:48.000000 stakefish-web3-utils-0.2.0/web3_utils/convert_to_standard_notation.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      284 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/current_utc_timestamp.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      138 2023-01-06 10:24:44.000000 stakefish-web3-utils-0.2.0/web3_utils/divide_chunks.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      111 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/gwei_to_wei.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      126 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/hash_event_param.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      241 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/is_null_address.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      301 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/normalize_address.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)     3547 2023-08-03 13:19:47.000000 stakefish-web3-utils-0.2.0/web3_utils/retryable_eth_module.py
+-rw-r--r--   0 mbaranovski   (501) staff       (20)      336 2023-01-09 10:39:07.000000 stakefish-web3-utils-0.2.0/web3_utils/split_validator_pubkey_bytes.py
```

### Comparing `stakefish-web3-utils-0.1.0/LICENSE.md` & `stakefish-web3-utils-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/PKG-INFO` & `stakefish-web3-utils-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stakefish-web3-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Stakefish’s web3 utils for Python
 Home-page: https://github.com/stakefish/web3-utils
 Author: Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `stakefish-web3-utils-0.1.0/README.rst` & `stakefish-web3-utils-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/setup.cfg` & `stakefish-web3-utils-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stakefish-web3-utils
-version = 0.1.0
+version = 0.2.0
 description = Stakefish’s web3 utils for Python
 author = Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 url = https://github.com/stakefish/web3-utils
 long_description = file: README.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
```

### Comparing `stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/PKG-INFO` & `stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stakefish-web3-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Stakefish’s web3 utils for Python
 Home-page: https://github.com/stakefish/web3-utils
 Author: Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/SOURCES.txt` & `stakefish-web3-utils-0.2.0/stakefish_web3_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/tests/test_async_beacon.py` & `stakefish-web3-utils-0.2.0/tests/test_async_beacon.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/tests/test_divide_chunks.py` & `stakefish-web3-utils-0.2.0/tests/test_divide_chunks.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/tests/test_retryable_eth_module.py` & `stakefish-web3-utils-0.2.0/tests/test_retryable_eth_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pytest
 from pytest_mock import MockerFixture
 from requests import HTTPError, ConnectionError
 from web3 import HTTPProvider
 from web3.eth import Eth
 from web3.exceptions import BlockNotFound, TransactionNotFound
 from web3.main import get_default_modules, Web3
+from web3.types import RPCError
 
 from web3_utils.retryable_eth_module import get_retryable_eth_module
 
 
 @pytest.fixture(autouse=True)
 def isolation(fn_isolation):
     pass
@@ -137,7 +138,19 @@
 
     web3 = retryable_web3()
 
     with pytest.raises(BlockNotFound):
         web3.eth.get_block(123)
 
     mocked_fn.assert_called()
+
+
+def test_rpc_timeout_error_retry(mocker):
+    rpc_timeout_error = RPCError(code=-32603, message="request failed or timed out")
+    mocked_fn: MagicMock = mocker.patch(
+        "web3.module.retrieve_blocking_method_call_fn",
+        return_value=trigger_fake_error(error_to_raise=ValueError(rpc_timeout_error)),
+    )
+
+    web3 = retryable_web3()
+    web3.eth.get_block(123)
+    mocked_fn.assert_called()
```

### Comparing `stakefish-web3-utils-0.1.0/tests/test_split_validator_pubkey_bytes.py` & `stakefish-web3-utils-0.2.0/tests/test_split_validator_pubkey_bytes.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/web3_utils/async_beacon.py` & `stakefish-web3-utils-0.2.0/web3_utils/async_beacon.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.1.0/web3_utils/retryable_eth_module.py` & `stakefish-web3-utils-0.2.0/web3_utils/retryable_eth_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import asyncio
+from http import HTTPStatus
 import logging
 import time
 from typing import Type
 
 import typing
 from aiohttp import ClientConnectorError
 from requests import HTTPError, ConnectionError
@@ -46,28 +47,43 @@
     return log_it
 
 
 def before(retry_state: "RetryCallState"):
     retry_state.start_time = time.monotonic()
 
 
+def is_retryable_http_error(e) -> bool:
+    """Check for retryable HTTP status codes"""
+    return isinstance(e, HTTPError) and e.response.status_code in [
+        HTTPStatus.TOO_MANY_REQUESTS,
+        HTTPStatus.BAD_GATEWAY,
+        HTTPStatus.GATEWAY_TIMEOUT,
+    ]
+
+
+def is_timeout_value_error(e) -> bool:
+    """Check if a ValueError is due to an rpc request timeout."""
+    return isinstance(e, ValueError) and "request failed or timed out" in str(e)
+
+
 def get_retryable_eth_module(base: Type[Eth] | Type[AsyncEth], logger: logging.Logger, retry_stop: typing.Callable or None = None):
     class RetryableModule(base):
         def __getattribute__(self, name):
             """
             "retrieve_caller_fn" returns a function which raises errors based on RPC results.
             We can also catch HTTPErrors and ConnectionErrors here
             """
             if name == "retrieve_caller_fn":
                 return lambda *args, **kargs: retry(
                     retry=retry_any(
                         retry_if_exception_type(
                             (BlockNotFound, TransactionNotFound, ConnectionError, ClientConnectorError, asyncio.TimeoutError)
                         ),
-                        retry_if_exception(lambda e: isinstance(e, HTTPError) and e.response.status_code in [429, 502, 504]),
+                        retry_if_exception(is_retryable_http_error),
+                        retry_if_exception(is_timeout_value_error),
                     ),
                     wait=wait_fixed(5),
                     reraise=True,
                     before=before,
                     before_sleep=before_sleep_log(logger=logger, log_level=logging.WARNING),
                     stop=retry_stop() if retry_stop else stop_never,
                 )(object.__getattribute__(self, name)(*args, *kargs))
```

