# Comparing `tmp/kocoafab-0.0.3.tar.gz` & `tmp/kocoafab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kocoafab-0.0.3.tar", last modified: Wed Jul 26 02:00:12 2023, max compression
+gzip compressed data, was "kocoafab-0.0.4.tar", last modified: Thu Aug  3 02:08:10 2023, max compression
```

## Comparing `kocoafab-0.0.3.tar` & `kocoafab-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 02:00:12.278733 kocoafab-0.0.3/
--rw-rw-rw-   0        0        0      559 2023-07-26 02:00:12.276732 kocoafab-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      133 2023-07-19 08:25:19.000000 kocoafab-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 02:00:12.255728 kocoafab-0.0.3/kocoafab/
--rw-rw-rw-   0        0        0       21 2023-07-26 02:00:01.000000 kocoafab-0.0.3/kocoafab/__init__.py
--rw-rw-rw-   0        0        0     3828 2023-07-15 01:40:17.000000 kocoafab-0.0.3/kocoafab/ble_library.py
--rw-rw-rw-   0        0        0     3383 2023-07-18 11:20:46.000000 kocoafab-0.0.3/kocoafab/i2c_lcd.py
--rw-rw-rw-   0        0        0     7461 2023-07-15 08:01:13.000000 kocoafab-0.0.3/kocoafab/lcd_api.py
-drwxrwxrwx   0        0        0        0 2023-07-26 02:00:12.272733 kocoafab-0.0.3/kocoafab.egg-info/
--rw-rw-rw-   0        0        0      559 2023-07-26 02:00:12.000000 kocoafab-0.0.3/kocoafab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-26 02:00:12.000000 kocoafab-0.0.3/kocoafab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 02:00:12.000000 kocoafab-0.0.3/kocoafab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 02:00:12.000000 kocoafab-0.0.3/kocoafab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 02:00:12.278733 kocoafab-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-26 01:59:53.000000 kocoafab-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:08:10.641311 kocoafab-0.0.4/
+-rw-rw-rw-   0        0        0      671 2023-08-03 02:08:10.641311 kocoafab-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2023-07-19 08:25:19.000000 kocoafab-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 02:08:10.640310 kocoafab-0.0.4/kocoafab.egg-info/
+-rw-rw-rw-   0        0        0      671 2023-08-03 02:08:10.000000 kocoafab-0.0.4/kocoafab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-08-03 02:08:10.000000 kocoafab-0.0.4/kocoafab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 02:08:10.000000 kocoafab-0.0.4/kocoafab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 02:08:10.000000 kocoafab-0.0.4/kocoafab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 02:08:10.643311 kocoafab-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-08-03 00:48:28.000000 kocoafab-0.0.4/setup.py
```

### Comparing `kocoafab-0.0.3/PKG-INFO` & `kocoafab-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: kocoafab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to get readings from sensors on a ESP32.
 Home-page: https://kocoafab.cc
 Author: kocoafab
 Author-email: kocoafab@kocoa.or.kr
+License: UNKNOWN
+Description: Read the kocoafab at
+        `kocoafab.cc <https://kocoafab.cc/>`_.
+        
+        Installation
+        ------------
+        
+        Install from Pypi::
+        
+            pip install kocoafab
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-Read the kocoafab at
-`kocoafab.cc <https://kocoafab.cc/>`_.
-
-Installation
-------------
-
-Install from Pypi::
-
-    pip install kocoafab
```

### Comparing `kocoafab-0.0.3/kocoafab.egg-info/PKG-INFO` & `kocoafab-0.0.4/kocoafab.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: kocoafab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to get readings from sensors on a ESP32.
 Home-page: https://kocoafab.cc
 Author: kocoafab
 Author-email: kocoafab@kocoa.or.kr
+License: UNKNOWN
+Description: Read the kocoafab at
+        `kocoafab.cc <https://kocoafab.cc/>`_.
+        
+        Installation
+        ------------
+        
+        Install from Pypi::
+        
+            pip install kocoafab
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-Read the kocoafab at
-`kocoafab.cc <https://kocoafab.cc/>`_.
-
-Installation
-------------
-
-Install from Pypi::
-
-    pip install kocoafab
```

### Comparing `kocoafab-0.0.3/setup.py` & `kocoafab-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kocoafab", # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="kocoafab",
     author_email="kocoafab@kocoa.or.kr",
     description="Library to get readings from sensors on a ESP32.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://kocoafab.cc",
     packages=setuptools.find_packages(),
```

