# Comparing `tmp/helium-3.2.4.tar.gz` & `tmp/helium-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helium-3.2.4.tar", last modified: Mon Jul 31 13:06:04 2023, max compression
+gzip compressed data, was "helium-3.2.5.tar", last modified: Thu Aug  3 16:27:00 2023, max compression
```

## Comparing `helium-3.2.4.tar` & `helium-3.2.5.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.310652 helium-3.2.4/
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2022-11-20 07:50:07.000000 helium-3.2.4/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)    30695 2022-11-20 07:50:07.000000 helium-3.2.4/NOTICE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1120 2023-07-31 13:06:04.310652 helium-3.2.4/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     6181 2023-07-31 12:15:50.000000 helium-3.2.4/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/
--rw-r--r--   0 michael   (1000) michael   (1000)    36009 2023-07-31 12:15:50.000000 helium-3.2.4/helium/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/
--rw-r--r--   0 michael   (1000) michael   (1000)    44901 2023-07-31 12:15:50.000000 helium-3.2.4/helium/_impl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-07-31 12:31:47.000000 helium-3.2.4/helium/_impl/chromedriver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1140 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/match_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5411 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/selenium_wrappers.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/util/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/dictionary.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6355 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/geom.py
--rw-r--r--   0 michael   (1000) michael   (1000)      979 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/html.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1210 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/inspect_.py
--rw-r--r--   0 michael   (1000) michael   (1000)      570 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/lang.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/os_.py
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/path.py
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/system.py
--rw-r--r--   0 michael   (1000) michael   (1000)      466 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/xpath.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/webdrivers/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/webdrivers/linux/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  7008696 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/webdrivers/linux/geckodriver
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.306651 helium-3.2.4/helium/_impl/webdrivers/mac/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  5259056 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/webdrivers/mac/geckodriver
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.310652 helium-3.2.4/helium/_impl/webdrivers/windows/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  3566280 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/webdrivers/windows/geckodriver.exe
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1120 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      759 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2022-11-20 07:50:55.000000 helium-3.2.4/helium.egg-info/not-zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-31 13:06:04.310652 helium-3.2.4/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     1464 2023-07-31 13:05:24.000000 helium-3.2.4/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.019639 helium-3.2.5/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1125 2023-08-03 16:27:00.019639 helium-3.2.5/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     6181 2023-07-05 14:17:27.000000 helium-3.2.5/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.011638 helium-3.2.5/helium/
+-rw-r--r--   0 michael   (1000) michael   (1000)    36009 2023-07-05 14:11:03.000000 helium-3.2.5/helium/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.011638 helium-3.2.5/helium/_impl/
+-rw-r--r--   0 michael   (1000) michael   (1000)    44901 2023-07-17 12:37:25.000000 helium-3.2.5/helium/_impl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      545 2023-08-03 16:12:55.000000 helium-3.2.5/helium/_impl/chromedriver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1140 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/match_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5411 2023-07-03 06:19:15.000000 helium-3.2.5/helium/_impl/selenium_wrappers.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.011638 helium-3.2.5/helium/_impl/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/dictionary.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6355 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/geom.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      979 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/html.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1210 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/inspect_.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      570 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/lang.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/os_.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      466 2021-03-16 06:48:50.000000 helium-3.2.5/helium/_impl/util/xpath.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.011638 helium-3.2.5/helium/_impl/webdrivers/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.011638 helium-3.2.5/helium/_impl/webdrivers/linux/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  7008696 2023-06-12 05:45:47.000000 helium-3.2.5/helium/_impl/webdrivers/linux/geckodriver
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.015638 helium-3.2.5/helium/_impl/webdrivers/mac/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  5259056 2023-06-12 05:45:47.000000 helium-3.2.5/helium/_impl/webdrivers/mac/geckodriver
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.019639 helium-3.2.5/helium/_impl/webdrivers/windows/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  3566280 2023-06-12 05:45:47.000000 helium-3.2.5/helium/_impl/webdrivers/windows/geckodriver.exe
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:27:00.011638 helium-3.2.5/helium.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1125 2023-08-03 16:26:59.000000 helium-3.2.5/helium.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      736 2023-08-03 16:26:59.000000 helium-3.2.5/helium.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-03 16:26:59.000000 helium-3.2.5/helium.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2021-03-16 06:50:17.000000 helium-3.2.5/helium.egg-info/not-zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-08-03 16:26:59.000000 helium-3.2.5/helium.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-08-03 16:26:59.000000 helium-3.2.5/helium.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-08-03 16:27:00.019639 helium-3.2.5/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     1464 2023-08-03 16:09:21.000000 helium-3.2.5/setup.py
```

### Comparing `helium-3.2.4/PKG-INFO` & `helium-3.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: helium
-Version: 3.2.4
+Version: 3.2.5
 Summary: Lighter browser automation based on Selenium.
 Home-page: https://github.com/mherrmann/selenium-python-helium
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
+License: UNKNOWN
+Description: UNKNOWN
 Keywords: helium selenium browser automation
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
@@ -18,9 +21,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3
-License-File: LICENSE.txt
-License-File: NOTICE.txt
```

### Comparing `helium-3.2.4/README.md` & `helium-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/__init__.py` & `helium-3.2.5/helium/__init__.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/__init__.py` & `helium-3.2.5/helium/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/match_type.py` & `helium-3.2.5/helium/_impl/match_type.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/selenium_wrappers.py` & `helium-3.2.5/helium/_impl/selenium_wrappers.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/util/geom.py` & `helium-3.2.5/helium/_impl/util/geom.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/util/html.py` & `helium-3.2.5/helium/_impl/util/html.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/util/inspect_.py` & `helium-3.2.5/helium/_impl/util/inspect_.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/util/lang.py` & `helium-3.2.5/helium/_impl/util/lang.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/util/path.py` & `helium-3.2.5/helium/_impl/util/path.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/webdrivers/linux/geckodriver` & `helium-3.2.5/helium/_impl/webdrivers/linux/geckodriver`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/webdrivers/mac/geckodriver` & `helium-3.2.5/helium/_impl/webdrivers/mac/geckodriver`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium/_impl/webdrivers/windows/geckodriver.exe` & `helium-3.2.5/helium/_impl/webdrivers/windows/geckodriver.exe`

 * *Files identical despite different names*

### Comparing `helium-3.2.4/helium.egg-info/PKG-INFO` & `helium-3.2.5/helium.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: helium
-Version: 3.2.4
+Version: 3.2.5
 Summary: Lighter browser automation based on Selenium.
 Home-page: https://github.com/mherrmann/selenium-python-helium
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
+License: UNKNOWN
+Description: UNKNOWN
 Keywords: helium selenium browser automation
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
@@ -18,9 +21,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3
-License-File: LICENSE.txt
-License-File: NOTICE.txt
```

### Comparing `helium-3.2.4/helium.egg-info/SOURCES.txt` & `helium-3.2.5/helium.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-LICENSE.txt
-NOTICE.txt
 README.md
 setup.py
 helium/__init__.py
 helium.egg-info/PKG-INFO
 helium.egg-info/SOURCES.txt
 helium.egg-info/dependency_links.txt
 helium.egg-info/not-zip-safe
```

### Comparing `helium-3.2.4/setup.py` & `helium-3.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'helium',
 	# Also update docs/conf.py when you change this:
-	version = '3.2.4',
+	version = '3.2.5',
 	author = 'Michael Herrmann',
 	author_email = 'michael+removethisifyouarehuman@herrmann.io',
 	description = 'Lighter browser automation based on Selenium.',
 	keywords = 'helium selenium browser automation',
 	url = 'https://github.com/mherrmann/selenium-python-helium',
 	python_requires='>=3',
 	packages = find_packages(exclude=['tests', 'tests.*']),
 	install_requires = [
 		# Also update requirements/base.txt when you make changes here.
 		'selenium==3.141.0',
 		# Selenium 3 is incompatible with urllib3 >= 2:
 		'urllib3<2',
-		'webdriver-manager==4.0.0'
+		'webdriver-manager>=4.0.0'
 	],
 	package_data = {
 		'helium._impl': ['webdrivers/**/*']
 	},
 	zip_safe = False,
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
```

