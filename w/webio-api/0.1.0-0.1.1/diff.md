# Comparing `tmp/webio_api-0.1.0.tar.gz` & `tmp/webio_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webio_api-0.1.0.tar", last modified: Thu Jul 20 14:48:22 2023, max compression
+gzip compressed data, was "webio_api-0.1.1.tar", last modified: Thu Aug  3 13:15:17 2023, max compression
```

## Comparing `webio_api-0.1.0.tar` & `webio_api-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-07-20 14:48:22.589938 webio_api-0.1.0/
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     1065 2023-07-20 14:40:23.000000 webio_api-0.1.0/LICENSE
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-07-20 14:48:22.581939 webio_api-0.1.0/PKG-INFO
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      113 2023-07-20 14:41:45.000000 webio_api-0.1.0/README.md
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       38 2023-07-20 14:48:22.589938 webio_api-0.1.0/setup.cfg
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      570 2023-07-20 14:44:04.000000 webio_api-0.1.0/setup.py
-drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-07-20 14:48:22.581939 webio_api-0.1.0/webio_api/
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     6974 2023-07-20 14:41:25.000000 webio_api-0.1.0/webio_api/__init__.py
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      556 2023-07-20 14:41:30.000000 webio_api-0.1.0/webio_api/const.py
-drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-07-20 14:48:22.581939 webio_api-0.1.0/webio_api.egg-info/
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-07-20 14:48:22.000000 webio_api-0.1.0/webio_api.egg-info/PKG-INFO
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      199 2023-07-20 14:48:22.000000 webio_api-0.1.0/webio_api.egg-info/SOURCES.txt
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)        1 2023-07-20 14:48:22.000000 webio_api-0.1.0/webio_api.egg-info/dependency_links.txt
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       10 2023-07-20 14:48:22.000000 webio_api-0.1.0/webio_api.egg-info/top_level.txt
+drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-08-03 13:15:17.700771 webio_api-0.1.1/
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     1065 2023-07-20 14:40:23.000000 webio_api-0.1.1/LICENSE
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-08-03 13:15:17.700771 webio_api-0.1.1/PKG-INFO
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      113 2023-07-20 14:41:45.000000 webio_api-0.1.1/README.md
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       38 2023-08-03 13:15:17.700771 webio_api-0.1.1/setup.cfg
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      570 2023-08-03 12:33:57.000000 webio_api-0.1.1/setup.py
+drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-08-03 13:15:17.700771 webio_api-0.1.1/webio_api/
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     4239 2023-08-03 13:06:18.000000 webio_api-0.1.1/webio_api/__init__.py
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     3996 2023-08-03 13:06:18.000000 webio_api-0.1.1/webio_api/api_client.py
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      676 2023-08-03 13:06:18.000000 webio_api-0.1.1/webio_api/const.py
+drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-08-03 13:15:17.700771 webio_api-0.1.1/webio_api.egg-info/
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-08-03 13:15:17.000000 webio_api-0.1.1/webio_api.egg-info/PKG-INFO
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      223 2023-08-03 13:15:17.000000 webio_api-0.1.1/webio_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)        1 2023-08-03 13:15:17.000000 webio_api-0.1.1/webio_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       10 2023-08-03 13:15:17.000000 webio_api-0.1.1/webio_api.egg-info/top_level.txt
```

### Comparing `webio_api-0.1.0/LICENSE` & `webio_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webio_api-0.1.0/setup.py` & `webio_api-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="webio_api",
-    version="0.1.0",
+    version="0.1.1",
     author="nasWebio",
     author_email="devel_team@chomtech.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nasWebio/webio_api",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webio_api-0.1.0/webio_api/const.py` & `webio_api-0.1.1/webio_api/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 EP_CHECK_CONNECTION = "rest/hello/world"
 EP_DEVICE_INFO = "rest/integration/hass/getDeviceInfo"
 EP_SET_OUTPUT = "rest/integration/hass/setOutput"
+EP_STATUS_SUBSCRIPTION = "rest/integration/hass/statusSubscription"
 KEY_LOGIN = "login"
 KEY_PASSWORD = "password"
 KEY_ERROR = "error"
 KEY_ERROR_CODE = "error_code"
 KEY_SERIAL_NUMBER = "devSN"
 KEY_WEBIO_NAME = "devName"
 KEY_OUTPUT_COUNT = "output_count"
 KEY_RESULT = "result"
 KEY_INDEX = "index"
 KEY_STATUS = "status"
 KEY_TEMP_ENV = "temp_env"
 KEY_OUTPUTS = "outputs"
 KEY_TYPE = "type"
 KEY_ANSWER = "Answer"
+KEY_ADDRESS = "address"
+KEY_SUBSCRIBE = "subscribe"
 TYPE_STATUS_UPDATE = "status_update"
 NOT_AUTHORIZED = "Not Authorized"
```

