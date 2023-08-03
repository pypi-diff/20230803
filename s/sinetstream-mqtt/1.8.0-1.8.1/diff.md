# Comparing `tmp/sinetstream-mqtt-1.8.0.tar.gz` & `tmp/sinetstream-mqtt-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-mqtt-1.8.0.tar", last modified: Tue May 16 06:40:05 2023, max compression
+gzip compressed data, was "sinetstream-mqtt-1.8.1.tar", last modified: Thu Aug  3 07:51:35 2023, max compression
```

## Comparing `sinetstream-mqtt-1.8.0.tar` & `sinetstream-mqtt-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      545 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1658 2023-05-16 06:40:05.726483 sinetstream-mqtt-1.8.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-mqtt-1.8.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.714484 sinetstream-mqtt-1.8.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      545 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      410 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)      273 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:57.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       42 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/src/sinetstreamplugin/
--rw-rw-r--   0 koie      (1004) koie      (1004)    14595 2023-05-16 06:28:56.000000 sinetstream-mqtt-1.8.0/src/sinetstreamplugin/mqtt.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:35.745122 sinetstream-mqtt-1.8.1/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      545 2023-08-03 07:51:35.745122 sinetstream-mqtt-1.8.1/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1658 2023-08-03 07:51:35.745122 sinetstream-mqtt-1.8.1/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-08-02 07:22:54.000000 sinetstream-mqtt-1.8.1/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:35.741122 sinetstream-mqtt-1.8.1/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:35.741122 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      545 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      410 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)      273 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       42 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:35.000000 sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:35.741122 sinetstream-mqtt-1.8.1/src/sinetstreamplugin/
+-rw-rw-r--   0 koie      (1004) koie      (1004)    15512 2023-08-02 07:22:54.000000 sinetstream-mqtt-1.8.1/src/sinetstreamplugin/mqtt.py
```

### Comparing `sinetstream-mqtt-1.8.0/PKG-INFO` & `sinetstream-mqtt-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-mqtt
-Version: 1.8.0
+Version: 1.8.1
 Summary: MQTT plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `sinetstream-mqtt-1.8.0/setup.cfg` & `sinetstream-mqtt-1.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-mqtt
-version = 1.8.0
+version = 1.8.1
 description = MQTT plugin for SINETStream library
 license = Apache License, Version 2.0
 license_files = 
 	../../../../LICENSE
 url = https://github.com/nii-gakunin-cloud/sinetstream
 classifiers = 
 	Development Status :: 4 - Beta
@@ -16,29 +16,29 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 install_requires = 
-	sinetstream>=1.8.0
+	sinetstream>=1.8.1
 	paho-mqtt>=1.5
 	promise
 tests_require = 
 	pytest
 	pytest-cov
 	pytest-flake8
 	pytest-timeout
 	pytest-html==3.2.0
 	flake8>=4.0.0,<5.0.0  # workaround: https://github.com/tholo/pytest-flake8/issues/87
 setup_requires = 
 	pytest-runner
 namespace_packages = 
 	sinetstreamplugin
-python_requires = >= 3.7
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [aliases]
 test = pytest
```

### Comparing `sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/PKG-INFO` & `sinetstream-mqtt-1.8.1/src/sinetstream_mqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-mqtt
-Version: 1.8.0
+Version: 1.8.1
 Summary: MQTT plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `sinetstream-mqtt-1.8.0/src/sinetstreamplugin/mqtt.py` & `sinetstream-mqtt-1.8.1/src/sinetstreamplugin/mqtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,20 +37,25 @@
 from promise import Promise
 
 from sinetstream import (
     AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE,
     InvalidArgumentError, ConnectionError,
     SinetError)
 
+from sinetstream import SINETStreamMessageEncoder
+
 logger = logging.getLogger(__name__)
 
 QOS_MAP = {
     AT_MOST_ONCE: 0,
     AT_LEAST_ONCE: 1,
     EXACTLY_ONCE: 2,
+    'AT_MOST_ONCE': 0,
+    'AT_LEAST_ONCE': 1,
+    'EXACTLY_ONCE': 2,
 }
 
 
 def _to_qos(params):
     qos = params.get('qos')
     if qos is not None:
         if qos not in QOS_MAP.values():
@@ -200,19 +205,36 @@
     ])
 
 
 def _replace_will_params(params):
     if 'will_set' not in params:
         return
     will_params = params['will_set']
+
+    for k in ['topic', 'payload']:
+        if k not in will_params:
+            raise InvalidArgumentError(f'the parameter {k} in will_set must be specified')
+
     if 'delay_interval' in will_params:
         props = Properties(PacketTypes.WILLMESSAGE)
         props.WillDelayInterval = will_params.pop('delay_interval')
         will_params['properties'] = props
 
+    will_params['qos'] = _to_qos(will_params)
+    will_params.pop('consistency', None)  # note: del will_params['consistency'] safely.
+
+    args = ['topic', 'payload', 'qos', 'retain', 'properties']
+    will_params2 = {k: will_params[k] for k in args if k in will_params}
+    writer_params = {k: will_params[k] for k in will_params.keys() if k not in args}
+    with SINETStreamMessageEncoder(**writer_params) as enc:
+        payload = will_params['payload']
+        will_params2['payload'] = enc.encode(payload, timestamp=0)
+
+    params['will_set'] = will_params2
+
 
 class MqttClient(object):
     def __init__(self, params):
         self._params = _translate_tls_params(params)
         self._params.update(params)
         _replace_ssl_params(self._params)
         _replace_will_params(self._params)
@@ -320,14 +342,17 @@
         logger.debug(f"MQTT:on_connect: rc={rc}")
         if rc != 0:
             logger.error(f"MQTT: {connack_string(rc)}: {rc}")
         with self._conn_cond:
             self._connection_result = rc
             self._conn_cond.notify_all()
 
+    def _debug_get_socket(self):
+        return self._mqttc.socket()
+
 
 class BaseMqttReader(MqttClient):
     def __init__(self, params):
         super().__init__(params)
         self.topics = self._get_topics()
         timeout_ms = self._params["receive_timeout_ms"]
         self._timeout = timeout_ms / 1000.0 if timeout_ms != inf else None
```

