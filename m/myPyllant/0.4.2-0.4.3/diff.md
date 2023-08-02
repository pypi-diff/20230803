# Comparing `tmp/mypyllant-0.4.2.tar.gz` & `tmp/mypyllant-0.4.3.tar.gz`

## Comparing `mypyllant-0.4.2.tar` & `mypyllant-0.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.dockerignore
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.2/Dockerfile
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.2/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.2/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.2/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.github/workflows/docker.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/api.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/export.py
--rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/sample.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.2/LICENSE
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 mypyllant-0.4.2/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 mypyllant-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.dockerignore
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.3/Dockerfile
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.3/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.3/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.3/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/api.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
+-rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 mypyllant-0.4.3/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 mypyllant-0.4.3/PKG-INFO
```

### Comparing `mypyllant-0.4.2/.dockerignore` & `mypyllant-0.4.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/.pre-commit-config.yaml` & `mypyllant-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/logo.png` & `mypyllant-0.4.3/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/.github/workflows/build-test.yaml` & `mypyllant-0.4.3/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/.github/workflows/docker.yaml` & `mypyllant-0.4.3/.github/workflows/docker.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/api.py` & `mypyllant-0.4.3/src/myPyllant/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,21 +80,23 @@
     def __init__(
         self, username: str, password: str, brand: str, country: str | None = None
     ) -> None:
         if brand not in BRANDS.keys():
             raise ValueError(
                 f"Invalid brand, must be one of {', '.join(BRANDS.keys())}"
             )
-        if country and country not in COUNTRIES[brand].keys():
-            raise RealmInvalid(
-                f"Invalid country, {BRANDS[brand]} only supports {', '.join(COUNTRIES[brand].keys())}"
-            )
-        if not country and brand in COUNTRIES and COUNTRIES[brand]:
-            # If a brand has countries defined, a country needs to be provided
-            raise RealmInvalid(f"{BRANDS[brand]} requires country to be passed")
+        if brand in COUNTRIES:
+            # Only need to valid country, if the brand exists as a key in COUNTRIES
+            if not country:
+                raise RealmInvalid(f"{BRANDS[brand]} requires country to be passed")
+            elif country not in COUNTRIES[brand].keys():
+                raise RealmInvalid(
+                    f"Invalid country, {BRANDS[brand]} only supports {', '.join(COUNTRIES[brand].keys())}"
+                )
+
         self.username = username
         self.password = password
         self.country = country
         self.brand = brand
         trace_config = aiohttp.TraceConfig()
         trace_config.on_request_start.append(on_request_start)
         trace_config.on_request_end.append(on_request_end)
```

### Comparing `mypyllant-0.4.2/src/myPyllant/const.py` & `mypyllant-0.4.3/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/export.py` & `mypyllant-0.4.3/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/models.py` & `mypyllant-0.4.3/src/myPyllant/models.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/sample.py` & `mypyllant-0.4.3/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/utils.py` & `mypyllant-0.4.3/src/myPyllant/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,20 +56,22 @@
         return date.strftime("%Y-%m-%dT%H:%M:%S") + "Z"
 
 
 def datetime_parse(date_string: str) -> datetime:
     return datetime.strptime(date_string, "%Y-%m-%dT%H:%M:%SZ")
 
 
-def get_realm(brand: str, country: str) -> str:
+def get_realm(brand: str, country: str | None = None) -> str:
     """
     Vaillant and SDBG use `brand-country-b2c` as the realm, Bulex doesn't use a country
     """
     if brand == "bulex":
         return f"{brand}-b2c"
+    elif not country:
+        return f"{brand}-b2c"
     else:
         return f"{brand}-{country}-b2c"
 
 
 def add_default_parser_args(parser: argparse.ArgumentParser):
     parser.add_argument("user", help="Username (email address) for the myVaillant app")
     parser.add_argument("password", help="Password for the myVaillant app")
```

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/find_countries.py` & `mypyllant-0.4.3/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.4.3/src/myPyllant/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/test_api.py` & `mypyllant-0.4.3/src/myPyllant/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from datetime import datetime, timedelta, tzinfo
 
 import pytest
 from freezegun import freeze_time
 
-from myPyllant.api import MyPyllantAPI
+from myPyllant.api import MyPyllantAPI, RealmInvalid
 from myPyllant.models import (
     Device,
     DeviceData,
     DeviceDataBucket,
     System,
     Zone,
     ZoneCurrentSpecialFunction,
@@ -25,25 +25,46 @@
         user_data = {}
         for f in d.glob("*.json"):
             user_data[f.stem] = json.loads(f.read_text())
         test_data.append(user_data)
     return test_data
 
 
-async def test_login(mypyllant_aioresponses) -> None:
+async def test_login_vaillant(mypyllant_aioresponses) -> None:
     with mypyllant_aioresponses() as _:
         async with MyPyllantAPI(
             "test@example.com", "test", "vaillant", "germany"
         ) as mocked_api:
             assert isinstance(mocked_api.oauth_session_expires, datetime)
             assert mocked_api.oauth_session_expires > datetime.now()
             assert mocked_api.access_token == "access_token"
             assert "Authorization" in mocked_api.get_authorized_headers()
 
 
+async def test_login_bulex(mypyllant_aioresponses) -> None:
+    with mypyllant_aioresponses() as _:
+        async with MyPyllantAPI(
+            "test@example.com", "test", "bulex", None
+        ) as mocked_api:
+            assert isinstance(mocked_api.oauth_session_expires, datetime)
+            assert mocked_api.oauth_session_expires > datetime.now()
+            assert mocked_api.access_token == "access_token"
+            assert "Authorization" in mocked_api.get_authorized_headers()
+
+
+async def test_login_invalid_country(mypyllant_aioresponses) -> None:
+    with pytest.raises(RealmInvalid):
+        MyPyllantAPI("test@example.com", "test", "sdbg", "germany")
+
+
+async def test_login_country_missing(mypyllant_aioresponses) -> None:
+    with pytest.raises(RealmInvalid):
+        MyPyllantAPI("test@example.com", "test", "sdbg")
+
+
 async def test_refresh_token(mypyllant_aioresponses, mocked_api) -> None:
     with mypyllant_aioresponses() as _:
         with freeze_time(datetime.now() + timedelta(hours=1)):
             await mocked_api.refresh_token()
             session_expires = mocked_api.oauth_session_expires
         assert session_expires - datetime.now() > timedelta(hours=1)
         await mocked_api.aiohttp_session.close()
```

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/test_countries.py` & `mypyllant-0.4.3/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/test_export.py` & `mypyllant-0.4.3/src/myPyllant/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.4.3/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/update_sample.py` & `mypyllant-0.4.3/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/utils.py` & `mypyllant-0.4.3/src/myPyllant/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,25 @@
             super().__init__(**kwargs)
 
         def __enter__(self):
             super().__enter__()
 
             # auth endpoints
             self.get(
-                re.compile(r".*openid-connect/auth\?"),
+                re.compile(r".*vaillant-germany-b2c/protocol/openid-connect/auth\?"),
                 body=f"{LOGIN_URL.format(realm=get_realm('vaillant', 'germany'))}?test=test",
                 status=200,
                 repeat=True,
             )
+            self.get(
+                re.compile(r".*bulex-b2c/protocol/openid-connect/auth\?"),
+                body=f"{LOGIN_URL.format(realm=get_realm('bulex'))}?test=test",
+                status=200,
+                repeat=True,
+            )
             self.post(
                 re.compile(r".*login-actions/authenticate\?"),
                 status=200,
                 headers={"Location": "test?code=code"},
                 repeat=True,
             )
             self.post(
```

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json` & `mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json` & `mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json` & `mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json` & `mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json` & `mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json` & `mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/.gitignore` & `mypyllant-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/LICENSE` & `mypyllant-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/README.md` & `mypyllant-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/pyproject.toml` & `mypyllant-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.2/PKG-INFO` & `mypyllant-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

