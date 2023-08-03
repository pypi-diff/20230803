# Comparing `tmp/gog_price_checker-0.1.9.tar.gz` & `tmp/gog-price-checker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.9.tar", last modified: Fri Jul 28 16:58:59 2023, max compression
+gzip compressed data, was "gog-price-checker-1.0.0.tar", last modified: Thu Aug  3 16:27:09 2023, max compression
```

## Comparing `gog_price_checker-0.1.9.tar` & `gog-price-checker-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/gog_price_checker/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/gog_price_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/gog_price_checker/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/gog_price_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:09.044191 gog-price-checker-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-03 16:27:09.044191 gog-price-checker-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-03 16:26:57.000000 gog-price-checker-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:09.040191 gog-price-checker-1.0.0/gog_price_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 16:26:57.000000 gog-price-checker-1.0.0/gog_price_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-08-03 16:26:57.000000 gog-price-checker-1.0.0/gog_price_checker/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:09.044191 gog-price-checker-1.0.0/gog_price_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-03 16:27:09.000000 gog-price-checker-1.0.0/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 16:27:09.000000 gog-price-checker-1.0.0/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:27:09.000000 gog-price-checker-1.0.0/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 16:27:09.000000 gog-price-checker-1.0.0/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 16:27:09.000000 gog-price-checker-1.0.0/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:27:09.044191 gog-price-checker-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 16:26:57.000000 gog-price-checker-1.0.0/setup.py
```

### Comparing `gog_price_checker-0.1.9/PKG-INFO` & `gog-price-checker-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: gog_price_checker
-Version: 0.1.9
+Name: gog-price-checker
+Version: 1.0.0
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
+![Latest build status](https://github.com/iampopovich/gog_price_checker/workflows/upload-python-package/badge.svg)
 
 The **Game Price Checker** is a Python script that allows you to extract a URL from the clipboard, download the web page content, and retrieve the price of a game from the GOG API. The script is designed to work on macOS systems.
 
 ## Requirements
 
 - Python 3.x
 - Requests library (for making HTTP requests)
@@ -37,15 +38,15 @@
     - `-u`, `--url`: The URL of the game page to scrape (required).
     - `-n`, `--normalize`: (Optional) Normalize currencies to USD.
     - `-c`, `--count` : (Optional) default = 10, number of countries to show in sorted prices result
     - `-p`, `--pretty` : (Optional) shows result as pretty table
 
 Example:
 ```
-gog_price_checker -u https://www.gog.com/game/diablo -n -p
+gog-price-checker -u https://www.gog.com/game/diablo -n -p
 ```
 Output:
 ```
 Country                   Price      Currency
 ---------------------------------------------
 Ukraine                   5.51       USD
 Moldova                   5.51       USD
```

### Comparing `gog_price_checker-0.1.9/README.md` & `gog-price-checker-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
+![Latest build status](https://github.com/iampopovich/gog_price_checker/workflows/upload-python-package/badge.svg)
 
 The **Game Price Checker** is a Python script that allows you to extract a URL from the clipboard, download the web page content, and retrieve the price of a game from the GOG API. The script is designed to work on macOS systems.
 
 ## Requirements
 
 - Python 3.x
 - Requests library (for making HTTP requests)
@@ -25,15 +26,15 @@
     - `-u`, `--url`: The URL of the game page to scrape (required).
     - `-n`, `--normalize`: (Optional) Normalize currencies to USD.
     - `-c`, `--count` : (Optional) default = 10, number of countries to show in sorted prices result
     - `-p`, `--pretty` : (Optional) shows result as pretty table
 
 Example:
 ```
-gog_price_checker -u https://www.gog.com/game/diablo -n -p
+gog-price-checker -u https://www.gog.com/game/diablo -n -p
 ```
 Output:
 ```
 Country                   Price      Currency
 ---------------------------------------------
 Ukraine                   5.51       USD
 Moldova                   5.51       USD
```

### Comparing `gog_price_checker-0.1.9/gog_price_checker/__main__.py` & `gog-price-checker-1.0.0/gog_price_checker/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import re
 from threading import Thread
 import logging
 from argparse import ArgumentParser
 from urllib import request as urllib_request
 import json
 
+
+class Price:
+    country_code = None
+    country_name = None
+    currency = None
+    value = None
+
+    def __init__(self, country_code, country_name):
+        self.country_name = country_name
+        self.country_code = country_code
+
+
 COUNTRIES = {
     "US": "United States",
     "AR": "Argentina",
     "BS": "Bahamas",
     "BR": "Brazil",
     "CA": "Canada",
     "CL": "Chile",
@@ -86,15 +98,15 @@
     "MA": "Morocco",
     "NG": "Nigeria",
     "QA": "Qatar",
     "SA": "Saudi Arabia",
     "ZA": "South Africa",
     "AE": "United Arab Emirates"}
 
-COUNTRY_PRICES = {}
+COUNTRY_PRICES = [Price(key, value) for key, value in COUNTRIES.items()]
 
 logging.basicConfig(
     level=logging.INFO,
 )
 
 
 def extract_product_id(url):
@@ -102,67 +114,68 @@
     raw_card_product = re.search(r"card-product=\"\d*\"", html).group()
     product_id = re.search(r"(\d+)", raw_card_product).group()
     logging.debug(f"raw product id: {raw_card_product}")
     logging.debug(f"product id: {product_id}")
     return product_id
 
 
-def request_price(product_id, country_code, normalize=None):
+def request_price(product_id, price, normalize=None):
     data = None
-    url = f"https://api.gog.com/products/{product_id}/prices?countryCode={country_code}"
+    url = f"https://api.gog.com/products/{product_id}/prices?countryCode={price.country_code}"
     if normalize:
         url += "&currency=USD"
     try:
         logging.debug(url)
         response = urllib_request.urlopen(url).read().decode('utf-8')
         data = json.loads(response)
         logging.debug(data)
-        price = data['_embedded']['prices'][0]['finalPrice'].split(" ")
-        price[0] = int(price[0]) / 100
+        final_price = data['_embedded']['prices'][0]['finalPrice'].split(" ")
+        final_price[0] = int(final_price[0]) / 100
         logging.debug(price)
-        COUNTRY_PRICES[COUNTRIES[country_code]] = price
+        price.value = final_price[0]
+        price.currency = final_price[1]
     except KeyError as no_key_error:
         logging.error(no_key_error)
         logging.error(data)
 
 
 def request_prices(product_id, normalize=None):
     threads = []
-    for country_code in COUNTRIES:
-        t = Thread(target=request_price, args=(product_id, country_code, normalize))
+    for price in COUNTRY_PRICES:
+        t = Thread(target=request_price, args=(product_id, price, normalize))
         threads.append(t)
         t.start()
-
     for t in threads:
         t.join()
 
 
 def sort_prices():
-    return sorted(COUNTRY_PRICES.items(), key=lambda x: x[1], reverse=False)
+    return sorted(COUNTRY_PRICES, key=lambda x: x.value, reverse=False)
 
 
 def out_result(count, pretty=None):
     sorted_prices = sort_prices()
     count = min(abs(count), len(sorted_prices))
+    out_string = ""
     if pretty:
         shift_country = 25
         shift_price = 10
-        header = f"{'Country':<{shift_country}} {'Price':<{shift_price}} {'Currency'}"
-        print(header)
-        print("-" * len(header))
+        header = f"{'Country':<{shift_country}} {'Price':<{shift_price}} {'Currency'}\n"
+        out_string += header
+        out_string += "-" * (len(header)-1)
         for i, price in enumerate(sorted_prices):
             if i == count:
                 break
-            country, price_val, currency = price[0], price[1][0], price[1][1]
-            print(f"{country:<{shift_country}} {price_val:<{shift_price}} {currency}")
+            out_string += f"\n{price.country_name:<{shift_country}} {price.value:<{shift_price}} {price.currency}"
     else:
         for i, price in enumerate(sorted_prices):
             if i == count:
                 break
-            print(f"{price[0]}: {price[1][0]} {price[1][1]}")
+            out_string += f"\n{price.country_name}: {price.value} {price.currency}"
+    print(out_string)
 
 
 def main():
     args = init_parser().parse_args()
     if "gogdb.org" in args.url:
         product_id = args.url.split("/")[-1]
     else:
```

### Comparing `gog_price_checker-0.1.9/gog_price_checker.egg-info/PKG-INFO` & `gog-price-checker-1.0.0/gog_price_checker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.9
+Version: 1.0.0
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
+![Latest build status](https://github.com/iampopovich/gog_price_checker/workflows/upload-python-package/badge.svg)
 
 The **Game Price Checker** is a Python script that allows you to extract a URL from the clipboard, download the web page content, and retrieve the price of a game from the GOG API. The script is designed to work on macOS systems.
 
 ## Requirements
 
 - Python 3.x
 - Requests library (for making HTTP requests)
@@ -37,15 +38,15 @@
     - `-u`, `--url`: The URL of the game page to scrape (required).
     - `-n`, `--normalize`: (Optional) Normalize currencies to USD.
     - `-c`, `--count` : (Optional) default = 10, number of countries to show in sorted prices result
     - `-p`, `--pretty` : (Optional) shows result as pretty table
 
 Example:
 ```
-gog_price_checker -u https://www.gog.com/game/diablo -n -p
+gog-price-checker -u https://www.gog.com/game/diablo -n -p
 ```
 Output:
 ```
 Country                   Price      Currency
 ---------------------------------------------
 Ukraine                   5.51       USD
 Moldova                   5.51       USD
```

### Comparing `gog_price_checker-0.1.9/setup.py` & `gog-price-checker-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name="gog_price_checker",
-    version="0.1.9",
+    name="gog-price-checker",
+    version="1.0.0",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
     entry_points={
         "console_scripts": [
-            "gog_price_checker = gog_price_checker.__main__:main"
+            "gog-price-checker = gog_price_checker.__main__:main"
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

