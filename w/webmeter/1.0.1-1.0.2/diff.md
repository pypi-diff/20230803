# Comparing `tmp/webmeter-1.0.1.tar.gz` & `tmp/webmeter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/webmeter/webmeter/dist/.tmp-mjxls3fk/webmeter-1.0.1.tar", last modified: Thu Aug  3 09:47:20 2023, max compression
+gzip compressed data, was "/home/runner/work/webmeter/webmeter/dist/.tmp-s4jvp3g7/webmeter-1.0.2.tar", last modified: Thu Aug  3 10:06:19 2023, max compression
```

## Comparing `webmeter-1.0.1.tar` & `webmeter-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 09:47:07.000000 webmeter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 09:47:07.000000 webmeter-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 09:47:20.000000 webmeter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 09:47:07.000000 webmeter-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 09:47:20.000000 webmeter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 09:47:07.000000 webmeter-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/public/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/public/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter/view/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/view/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 09:47:07.000000 webmeter-1.0.1/webmeter/view/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 09:47:20.000000 webmeter-1.0.1/webmeter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 10:06:10.000000 webmeter-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 10:06:10.000000 webmeter-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 10:06:19.000000 webmeter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 10:06:10.000000 webmeter-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-03 10:06:19.000000 webmeter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 10:06:10.000000 webmeter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/public/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/view/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/view/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/top_level.txt
```

### Comparing `webmeter-1.0.1/LICENSE` & `webmeter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.1/PKG-INFO` & `webmeter-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webmeter
-Version: 1.0.1
+Version: 1.0.2
 Summary: WebMeter - A web api-performance tool based on jmeter.
 Home-page: https://github.com/rafa0128/webmeter
 Author: Rafa Chen
 Author-email: laoqi1988_f1@126.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `webmeter-1.0.1/setup.py` & `webmeter-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     install_requires=['fastapi','uvicorn', 'requests', 'logzero', 'fire','pyfiglet','psutil'],
-    version='1.0.1',
+    version='1.0.2',
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="WebMeter - A web api-performance tool based on jmeter.",
     packages=setuptools.find_namespace_packages(include=["webmeter", "webmeter.*"], ),
     include_package_data=True
 )
```

### Comparing `webmeter-1.0.1/webmeter/__main__.py` & `webmeter-1.0.2/webmeter/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,9 +9,9 @@
         logger.error('python version must be 3.10+ ,your python version is {}'.format(platform.python_version()))
         return False
     return True    
 
 if __name__ == '__main__':
     check = checkPyVer()
     if check:
-        from webmeter.main import main
+        from webmeter.web import main
         fire.Fire(main)
```

### Comparing `webmeter-1.0.1/webmeter/main.py` & `webmeter-1.0.2/webmeter/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from fastapi import FastAPI
 from webmeter.view import page,api
 from webmeter.public.utils import utils
 import requests
 import webbrowser
 import multiprocessing
 
-app = FastAPI(debug=True)
+app = FastAPI(debug=False)
 app.include_router(page.router)
 app.include_router(api.router)
 
 
 def status(host: str, port: int):
     r = requests.get('http://{}:{}/plan'.format(host, port), timeout=2.0)
     flag = (True, False)[r.status_code == 200]
```

### Comparing `webmeter-1.0.1/webmeter/static/image/empty.png` & `webmeter-1.0.2/webmeter/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.1/webmeter/templates/index.html` & `webmeter-1.0.2/webmeter/templates/index.html`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.1/webmeter.egg-info/PKG-INFO` & `webmeter-1.0.2/webmeter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webmeter
-Version: 1.0.1
+Version: 1.0.2
 Summary: WebMeter - A web api-performance tool based on jmeter.
 Home-page: https://github.com/rafa0128/webmeter
 Author: Rafa Chen
 Author-email: laoqi1988_f1@126.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

