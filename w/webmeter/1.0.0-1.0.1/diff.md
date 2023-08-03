# Comparing `tmp/webmeter-1.0.0.tar.gz` & `tmp/webmeter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/webmeter/webmeter/dist/.tmp-cwzvoi6x/webmeter-1.0.0.tar", last modified: Thu Aug  3 09:27:47 2023, max compression
+gzip compressed data, was "/home/runner/work/webmeter/webmeter/dist/.tmp-mjxls3fk/webmeter-1.0.1.tar", last modified: Thu Aug  3 09:47:20 2023, max compression
```

## Comparing `webmeter-1.0.0.tar` & `webmeter-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 09:27:35.000000 webmeter-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 09:27:35.000000 webmeter-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-03 09:27:47.000000 webmeter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 09:27:35.000000 webmeter-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 09:27:47.000000 webmeter-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 09:27:35.000000 webmeter-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 09:27:35.000000 webmeter-1.0.0/webmeter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter/public/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 09:27:35.000000 webmeter-1.0.0/webmeter/public/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-08-03 09:27:35.000000 webmeter-1.0.0/webmeter/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-03 09:27:35.000000 webmeter-1.0.0/webmeter/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter/view/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 09:27:35.000000 webmeter-1.0.0/webmeter/view/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 09:27:35.000000 webmeter-1.0.0/webmeter/view/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 09:27:47.000000 webmeter-1.0.0/webmeter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 09:47:07.000000 webmeter-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 09:47:07.000000 webmeter-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 09:47:20.000000 webmeter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 09:47:07.000000 webmeter-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 09:47:20.000000 webmeter-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 09:47:07.000000 webmeter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/public/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/view/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/view/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/top_level.txt
```

### Comparing `webmeter-1.0.0/LICENSE` & `webmeter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.0/setup.py` & `webmeter-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     install_requires=['fastapi','uvicorn', 'requests', 'logzero', 'fire','pyfiglet','psutil'],
-    version='1.0.0',
+    version='1.0.1',
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="WebMeter - A web api-performance tool based on jmeter.",
     packages=setuptools.find_namespace_packages(include=["webmeter", "webmeter.*"], ),
     include_package_data=True
 )
```

### Comparing `webmeter-1.0.0/webmeter/main.py` & `webmeter-1.0.1/webmeter/main.py`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.0/webmeter/static/image/empty.png` & `webmeter-1.0.1/webmeter/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.0/webmeter/templates/index.html` & `webmeter-1.0.1/webmeter/templates/index.html`

 * *Files identical despite different names*

