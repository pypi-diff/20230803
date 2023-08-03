# Comparing `tmp/selenium_tkit-0.1.0.2.tar.gz` & `tmp/selenium_tkit-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_tkit-0.1.0.2.tar", max compression
+gzip compressed data, was "selenium_tkit-0.1.0.3.tar", max compression
```

## Comparing `selenium_tkit-0.1.0.2.tar` & `selenium_tkit-0.1.0.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/LICENSE
--rw-r--r--   0        0        0     1022 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/README.md
--rw-r--r--   0        0        0      530 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/src/selenium_tkit/__init__.py
--rw-r--r--   0        0        0    16011 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/src/selenium_tkit/chrome.py
--rw-r--r--   0        0        0    27551 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/src/selenium_tkit/custom_webdriver.py
--rw-r--r--   0        0        0     3025 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/src/selenium_tkit/edge.py
--rw-r--r--   0        0        0    10659 2023-02-16 20:41:47.621419 selenium_tkit-0.1.0.2/src/selenium_tkit/firefox.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 selenium_tkit-0.1.0.2/setup.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 selenium_tkit-0.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/LICENSE
+-rw-r--r--   0        0        0     1022 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/README.md
+-rw-r--r--   0        0        0     2966 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/src/selenium_tkit/__init__.py
+-rw-r--r--   0        0        0    16188 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/src/selenium_tkit/chrome.py
+-rw-r--r--   0        0        0    27551 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/src/selenium_tkit/custom_webdriver.py
+-rw-r--r--   0        0        0     3025 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/src/selenium_tkit/edge.py
+-rw-r--r--   0        0        0    10659 2023-08-03 21:20:41.397666 selenium_tkit-0.1.0.3/src/selenium_tkit/firefox.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 selenium_tkit-0.1.0.3/PKG-INFO
```

### Comparing `selenium_tkit-0.1.0.2/LICENSE` & `selenium_tkit-0.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_tkit-0.1.0.2/README.md` & `selenium_tkit-0.1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `selenium_tkit-0.1.0.2/src/selenium_tkit/chrome.py` & `selenium_tkit-0.1.0.3/src/selenium_tkit/chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from selenium.webdriver import Chrome
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.remote.webdriver import WebDriver
 from undetected_chromedriver.patcher import Patcher
 from urllib3.exceptions import MaxRetryError
 from webdriver_manager.chrome import ChromeDriverManager
+from webdriver_manager.core.driver_cache import DriverCacheManager
 
 from .custom_webdriver import CustomWebDriver
 
 # --------------------------------------------------
 
 logger = logging.getLogger(__name__)
 
@@ -77,15 +78,16 @@
 
         driver.open_url("https://www.google.com")
         ```
         """
 
         if isinstance(driver_path, Path):
             driver_path = str(driver_path)
-        self.driver_path = ChromeDriverManager(path=driver_path).install()
+            cache = DriverCacheManager(driver_path)
+        self.driver_path = ChromeDriverManager(cache_manager=cache).install()
 
         if apply_patch:
             patcher = Patcher(executable_path=self.driver_path, force=False)
             patcher.auto()
 
             self.driver_path = patcher.executable_path
 
@@ -310,15 +312,16 @@
         port: int = 64900,
         options: Optional[ChromeOptions] = None,
         **kwargs,
     ) -> None:
 
         if isinstance(driver_path, Path):
             driver_path = str(driver_path)
-        self.driver_path = ChromeDriverManager(path=driver_path).install()
+            cache = DriverCacheManager(driver_path)
+        self.driver_path = ChromeDriverManager(cache_manager=cache).install()
 
         self.implicity_wait = implicity_wait
         self.port = port
         self.options = options
         return
 
     def begin(self):
```

### Comparing `selenium_tkit-0.1.0.2/src/selenium_tkit/custom_webdriver.py` & `selenium_tkit-0.1.0.3/src/selenium_tkit/custom_webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_tkit-0.1.0.2/src/selenium_tkit/edge.py` & `selenium_tkit-0.1.0.3/src/selenium_tkit/edge.py`

 * *Files identical despite different names*

### Comparing `selenium_tkit-0.1.0.2/src/selenium_tkit/firefox.py` & `selenium_tkit-0.1.0.3/src/selenium_tkit/firefox.py`

 * *Files identical despite different names*

### Comparing `selenium_tkit-0.1.0.2/PKG-INFO` & `selenium_tkit-0.1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: selenium-tkit
-Version: 0.1.0.2
+Version: 0.1.0.3
 Summary: Another selenium toolkit
 Author: henrique lino
 Author-email: henrique.lino97@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fake-useragent (>=1.1.1,<2.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: retimer (>=0.1.0.9,<0.2.0.0)
 Requires-Dist: selenium (>=4.7.2,<5.0.0)
 Requires-Dist: undetected-chromedriver (>=3.1.7,<4.0.0)
-Requires-Dist: webdriver-manager (>=3.8.5,<4.0.0)
+Requires-Dist: webdriver-manager (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # selenium_tkit
 
 > This package is under development, it should be used with that in mind, not every system may be compatible
 
 [![PyPI version][pypi-image]][pypi-url]
```

