# Comparing `tmp/pytest-sosu-0.2.2.tar.gz` & `tmp/pytest-sosu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-sosu-0.2.2.tar", last modified: Tue Feb 14 10:33:00 2023, max compression
+gzip compressed data, was "/Users/andrzejpragacz/projects/github.com/apragacz/pytest-sosu/dist/.tmp-04odsykv/pytest-sosu-0.3.0.tar", last modified: Wed Aug  2 22:43:48 2023, max compression
```

## Comparing `pytest-sosu-0.2.2.tar` & `pytest-sosu-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-02-14 10:33:00.859652 pytest-sosu-0.2.2/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1072 2020-02-24 11:36:45.000000 pytest-sosu-0.2.2/LICENSE
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       49 2021-06-29 11:09:48.000000 pytest-sosu-0.2.2/MANIFEST.in
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2803 2023-02-14 10:33:00.859898 pytest-sosu-0.2.2/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1260 2022-02-21 10:05:32.000000 pytest-sosu-0.2.2/README.md
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-02-14 10:33:00.848600 pytest-sosu-0.2.2/pytest_sosu/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       59 2021-06-29 11:53:51.000000 pytest-sosu-0.2.2/pytest_sosu/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-02-14 10:32:27.000000 pytest-sosu-0.2.2/pytest_sosu/_version.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2176 2022-11-16 23:31:27.000000 pytest-sosu-0.2.2/pytest_sosu/config.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      329 2022-02-19 00:17:09.000000 pytest-sosu-0.2.2/pytest_sosu/exceptions.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3647 2023-02-13 23:47:50.000000 pytest-sosu-0.2.2/pytest_sosu/logging.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5637 2022-11-17 13:49:20.000000 pytest-sosu-0.2.2/pytest_sosu/plugin.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2278 2022-02-18 23:32:06.000000 pytest-sosu-0.2.2/pytest_sosu/plugin_helpers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      530 2022-01-18 13:38:52.000000 pytest-sosu-0.2.2/pytest_sosu/typing.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3016 2023-02-13 12:03:21.000000 pytest-sosu-0.2.2/pytest_sosu/utils.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-02-14 10:33:00.858854 pytest-sosu-0.2.2/pytest_sosu/webdriver/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      625 2023-02-13 23:59:40.000000 pytest-sosu-0.2.2/pytest_sosu/webdriver/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     7681 2023-02-13 23:47:50.000000 pytest-sosu-0.2.2/pytest_sosu/webdriver/capabilities.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2932 2023-02-14 10:30:28.000000 pytest-sosu-0.2.2/pytest_sosu/webdriver/driver.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-11-17 00:56:32.000000 pytest-sosu-0.2.2/pytest_sosu/webdriver/platforms.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2048 2022-11-17 00:48:08.000000 pytest-sosu-0.2.2/pytest_sosu/webdriver/url.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-02-14 10:33:00.853392 pytest-sosu-0.2.2/pytest_sosu.egg-info/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2803 2023-02-14 10:33:00.000000 pytest-sosu-0.2.2/pytest_sosu.egg-info/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      642 2023-02-14 10:33:00.000000 pytest-sosu-0.2.2/pytest_sosu.egg-info/SOURCES.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-02-14 10:33:00.000000 pytest-sosu-0.2.2/pytest_sosu.egg-info/dependency_links.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       38 2023-02-14 10:33:00.000000 pytest-sosu-0.2.2/pytest_sosu.egg-info/entry_points.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       16 2023-02-14 10:33:00.000000 pytest-sosu-0.2.2/pytest_sosu.egg-info/requires.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       12 2023-02-14 10:33:00.000000 pytest-sosu-0.2.2/pytest_sosu.egg-info/top_level.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2631 2023-02-14 10:33:00.861350 pytest-sosu-0.2.2/setup.cfg
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2023-02-13 23:47:50.000000 pytest-sosu-0.2.2/setup.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.360939 pytest-sosu-0.3.0/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1072 2020-02-24 11:36:45.000000 pytest-sosu-0.3.0/LICENSE
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       49 2021-06-29 11:09:48.000000 pytest-sosu-0.3.0/MANIFEST.in
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3642 2023-08-02 22:43:48.360218 pytest-sosu-0.3.0/PKG-INFO
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1296 2023-08-02 22:29:12.000000 pytest-sosu-0.3.0/README.md
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3001 2023-08-02 21:23:45.000000 pytest-sosu-0.3.0/pyproject.toml
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.337503 pytest-sosu-0.3.0/pytest_sosu/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       59 2021-06-29 11:53:51.000000 pytest-sosu-0.3.0/pytest_sosu/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-08-02 22:43:26.000000 pytest-sosu-0.3.0/pytest_sosu/_version.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2215 2023-07-04 21:50:23.000000 pytest-sosu-0.3.0/pytest_sosu/config.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      329 2022-02-19 00:17:09.000000 pytest-sosu-0.3.0/pytest_sosu/exceptions.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3647 2023-02-13 23:47:50.000000 pytest-sosu-0.3.0/pytest_sosu/logging.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5684 2023-08-02 21:27:18.000000 pytest-sosu-0.3.0/pytest_sosu/plugin.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2278 2022-02-18 23:32:06.000000 pytest-sosu-0.3.0/pytest_sosu/plugin_helpers.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      530 2022-01-18 13:38:52.000000 pytest-sosu-0.3.0/pytest_sosu/typing.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3016 2023-02-13 12:03:21.000000 pytest-sosu-0.3.0/pytest_sosu/utils.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.358505 pytest-sosu-0.3.0/pytest_sosu/webdriver/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      517 2023-08-02 21:25:56.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     7728 2023-07-04 21:48:57.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/capabilities.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      184 2023-08-02 21:25:04.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/compat.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-11-17 00:56:32.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/platforms.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3089 2023-08-02 22:27:39.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/selenium.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2048 2022-11-17 00:48:08.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/url.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.344941 pytest-sosu-0.3.0/pytest_sosu.egg-info/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3642 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/PKG-INFO
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      681 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/SOURCES.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/dependency_links.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       37 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/entry_points.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/requires.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       12 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/top_level.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       38 2023-08-02 22:43:48.361263 pytest-sosu-0.3.0/setup.cfg
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2023-02-13 23:47:50.000000 pytest-sosu-0.3.0/setup.py
```

### Comparing `pytest-sosu-0.2.2/LICENSE` & `pytest-sosu-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/README.md` & `pytest-sosu-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 ## Basic Usage
 
 Assuming you have `SAUCE_USERNAME` and `SAUCE_ACCESS_KEY` environment variables set
 (credentials can be obtained [here](https://app.saucelabs.com/user-settings)),
 you can write a simple test:
 
 ```python
-def test_visit(sosu_webdriver):
-    driver = sosu_webdriver
+def test_visit(sosu_selenium_webdriver):
+    driver = sosu_selenium_webdriver
     driver.get("http://example.com/")
     assert driver.title == "Example Domain"
 ```
 
 ## Examples
 
 ```python
@@ -43,10 +43,10 @@
 @pytest.fixture(scope="session")
 def sosu_build_basename():
     return 'my-project-name'
 
 
 # alias for sosu_webdriver
 @pytest.fixture
-def driver(sosu_webdriver):
-    yield sosu_webdriver
+def driver(sosu_selenium_webdriver):
+    yield sosu_selenium_webdriver
 ```
```

### Comparing `pytest-sosu-0.2.2/pytest_sosu/config.py` & `pytest-sosu-0.3.0/pytest_sosu/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         access_key=access_key,
         region=region,
         webdriver_url_data=webdriver_url_data,
     )
 
 
 def get_host_by_region(region: Optional[str]) -> str:
-    if not region or region == "global":
+    if not region:
+        region = "us"
+    if region in ["global", "legacy"]:
         return "ondemand.saucelabs.com"
     host_region = REGION_MAP.get(region, region)
     return f"ondemand.{host_region}.saucelabs.com"
 
 
 REGION_MAP = {
     "us": "us-west-1",
```

### Comparing `pytest-sosu-0.2.2/pytest_sosu/logging.py` & `pytest-sosu-0.3.0/pytest_sosu/logging.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/pytest_sosu/plugin.py` & `pytest-sosu-0.3.0/pytest_sosu/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Browser,
     Capabilities,
     Platform,
     SauceOptions,
     WebDriverTestFailed,
     WebDriverTestInterrupted,
     WebDriverUrlData,
-    remote_webdriver_ctx,
 )
+from pytest_sosu.webdriver.selenium import remote_webdriver_ctx
 
 logger = get_struct_logger(__name__)
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("sosu plugin sauce labs configuration")
 
@@ -178,15 +178,15 @@
     sosu_webdriver_capabilities: Capabilities,
     sosu_webdriver_parameter_capabilities: Capabilities,
 ) -> Capabilities:
     return sosu_webdriver_capabilities.merge(sosu_webdriver_parameter_capabilities)
 
 
 @pytest.fixture
-def sosu_webdriver(
+def sosu_selenium_webdriver(
     request,
     sosu_webdriver_url_data: WebDriverUrlData,
     sosu_webdriver_combined_capabilities: Capabilities,
 ):
     with remote_webdriver_ctx(
         sosu_webdriver_url_data,
         sosu_webdriver_combined_capabilities,
```

### Comparing `pytest-sosu-0.2.2/pytest_sosu/plugin_helpers.py` & `pytest-sosu-0.3.0/pytest_sosu/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/pytest_sosu/typing.py` & `pytest-sosu-0.3.0/pytest_sosu/typing.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/pytest_sosu/utils.py` & `pytest-sosu-0.3.0/pytest_sosu/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/pytest_sosu/webdriver/capabilities.py` & `pytest-sosu-0.3.0/pytest_sosu/webdriver/capabilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     PUBLIC = "public"
     PUBLIC_RESTRICTED = "public restricted"
     SHARE = "share"
     TEAM = "team"
     PRIVATE = "private"
 
 
+# pylint: disable=too-many-instance-attributes
 @dataclass(frozen=True)
 class SauceOptions:
     name: Optional[str] = None
     build: Optional[str] = None
     tags: Optional[List[str]] = None
     username: Optional[str] = None
     access_key: Optional[str] = None
```

### Comparing `pytest-sosu-0.2.2/pytest_sosu/webdriver/driver.py` & `pytest-sosu-0.3.0/pytest_sosu/webdriver/selenium.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import contextlib
 from typing import Optional
 
 from selenium.webdriver import Remote as WebDriver  # type: ignore
 from selenium.webdriver.common.by import By  # noqa: F401 type: ignore
+from selenium.webdriver.common.options import ArgOptions  # type: ignore
 
 from pytest_sosu.exceptions import WebDriverTestFailed, WebDriverTestInterrupted
 from pytest_sosu.logging import get_struct_logger
 from pytest_sosu.webdriver.capabilities import Capabilities
 from pytest_sosu.webdriver.url import WebDriverUrlData
 
 logger = get_struct_logger(__name__)
@@ -72,17 +73,19 @@
     setup_timeouts: bool = True,
 ) -> WebDriver:
     wd_url = wd_url_data.to_url()
     caps = capabilities.to_dict()
     logger.debug("Dumping caps data", caps=caps)
     wd_safe_url = wd_url_data.to_safe_url()
     logger.debug("Using webdriver URL", wd_url=wd_safe_url)
+    options = ArgOptions()
+    options._caps.update(caps)  # pylint: disable=protected-access
     driver = WebDriver(
         command_executor=wd_url,
-        desired_capabilities=caps,
+        options=options,
     )
     if setup_timeouts:
         timeout = capabilities.sauce_options.command_timeout
         if timeout is not None:
             driver.set_page_load_timeout(timeout)
             driver.implicitly_wait(timeout)
             driver.set_script_timeout(timeout)
```

### Comparing `pytest-sosu-0.2.2/pytest_sosu/webdriver/platforms.py` & `pytest-sosu-0.3.0/pytest_sosu/webdriver/platforms.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/pytest_sosu/webdriver/url.py` & `pytest-sosu-0.3.0/pytest_sosu/webdriver/url.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.2.2/pytest_sosu.egg-info/SOURCES.txt` & `pytest-sosu-0.3.0/pytest_sosu.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 pytest_sosu/__init__.py
 pytest_sosu/_version.py
 pytest_sosu/config.py
 pytest_sosu/exceptions.py
 pytest_sosu/logging.py
 pytest_sosu/plugin.py
@@ -16,10 +16,11 @@
 pytest_sosu.egg-info/SOURCES.txt
 pytest_sosu.egg-info/dependency_links.txt
 pytest_sosu.egg-info/entry_points.txt
 pytest_sosu.egg-info/requires.txt
 pytest_sosu.egg-info/top_level.txt
 pytest_sosu/webdriver/__init__.py
 pytest_sosu/webdriver/capabilities.py
-pytest_sosu/webdriver/driver.py
+pytest_sosu/webdriver/compat.py
 pytest_sosu/webdriver/platforms.py
+pytest_sosu/webdriver/selenium.py
 pytest_sosu/webdriver/url.py
```

