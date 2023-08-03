# Comparing `tmp/sinetstream-1.8.0.tar.gz` & `tmp/sinetstream-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-1.8.0.tar", last modified: Tue May 16 06:32:29 2023, max compression
+gzip compressed data, was "sinetstream-1.8.1.tar", last modified: Thu Aug  3 07:43:35 2023, max compression
```

## Comparing `sinetstream-1.8.0.tar` & `sinetstream-1.8.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.654585 sinetstream-1.8.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)     2914 2023-05-16 06:32:29.654585 sinetstream-1.8.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     2446 2023-01-12 00:12:25.000000 sinetstream-1.8.0/README.md
--rw-rw-r--   0 koie      (1004) koie      (1004)     1435 2023-05-16 06:32:29.654585 sinetstream-1.8.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-1.8.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.630585 sinetstream-1.8.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.642585 sinetstream-1.8.0/src/sinetstream/
--rw-rw-r--   0 koie      (1004) koie      (1004)     1686 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/__init__.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     1169 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/__main__.py
--rw-rw-r--   0 koie      (1004) koie      (1004)    28081 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/api.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     2759 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/compression.py
--rw-rw-r--   0 koie      (1004) koie      (1004)    11484 2023-05-16 06:28:20.000000 sinetstream-1.8.0/src/sinetstream/config_client.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     9012 2023-05-16 06:28:20.000000 sinetstream-1.8.0/src/sinetstream/configs.py
--rw-rw-r--   0 koie      (1004) koie      (1004)    11450 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/crypto.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     1403 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/error.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     3215 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/marshal.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     4488 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/spi.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     2502 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/utils.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     1741 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/value_type.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.654585 sinetstream-1.8.0/src/sinetstream.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)     2914 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      586 2023-05-16 06:32:29.000000 sinetstream-1.8.0/src/sinetstream.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:50.000000 sinetstream-1.8.0/src/sinetstream.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       61 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       12 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:43:35.145679 sinetstream-1.8.1/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2914 2023-08-03 07:43:35.145679 sinetstream-1.8.1/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2446 2023-08-02 07:22:54.000000 sinetstream-1.8.1/README.md
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1435 2023-08-03 07:43:35.149679 sinetstream-1.8.1/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-08-02 07:22:54.000000 sinetstream-1.8.1/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:43:35.141679 sinetstream-1.8.1/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:43:35.145679 sinetstream-1.8.1/src/sinetstream/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1818 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/__init__.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1169 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/__main__.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)    28728 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/api.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     3341 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/codec.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2759 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/compression.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)    11484 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/config_client.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     9017 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/configs.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)    11450 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/crypto.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1403 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/error.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     3215 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/marshal.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     4488 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/spi.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2502 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/utils.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1741 2023-08-02 07:22:54.000000 sinetstream-1.8.1/src/sinetstream/value_type.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:43:35.145679 sinetstream-1.8.1/src/sinetstream.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2914 2023-08-03 07:43:35.000000 sinetstream-1.8.1/src/sinetstream.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      611 2023-08-03 07:43:35.000000 sinetstream-1.8.1/src/sinetstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:43:35.000000 sinetstream-1.8.1/src/sinetstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 06:47:41.000000 sinetstream-1.8.1/src/sinetstream.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       61 2023-08-03 07:43:35.000000 sinetstream-1.8.1/src/sinetstream.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       12 2023-08-03 07:43:35.000000 sinetstream-1.8.1/src/sinetstream.egg-info/top_level.txt
```

### Comparing `sinetstream-1.8.0/PKG-INFO` & `sinetstream-1.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sinetstream
-Version: 1.8.0
+Version: 1.8.1
 Summary: Library for operating messaging systems such as Apache Kafka and MQTT with the same API.
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
 Description-Content-Type: text/markdown
 
 <!--
 Copyright (C) 2020 National Institute of Informatics
 
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
```

### Comparing `sinetstream-1.8.0/README.md` & `sinetstream-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/setup.cfg` & `sinetstream-1.8.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream
-version = 1.8.0
+version = 1.8.1
 description = Library for operating messaging systems such as Apache Kafka and MQTT with the same API.
 long_description = file: README.en.md
 long_description_content_type = text/markdown
 url = https://github.com/nii-gakunin-cloud/sinetstream
 license = Apache License, Version 2.0
 license_files = 
 	../LICENSE
@@ -34,15 +34,15 @@
 	pytest-flake8
 	pytest-timeout
 	pytest-html==3.2.0
 	requests_mock
 	flake8>=4.0.0,<5.0.0  # workaround: https://github.com/tholo/pytest-flake8/issues/87
 setup_requires = 
 	pytest-runner
-python_requires = >= 3.7
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [aliases]
 test = pytest
```

### Comparing `sinetstream-1.8.0/src/sinetstream/__init__.py` & `sinetstream-1.8.1/src/sinetstream/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 )
 from .error import (
     SinetError, NoServiceError, NoConfigError, InvalidArgumentError,
     ConnectionError, AlreadyConnectedError, UnsupportedServiceTypeError,
     InvalidMessageError, AuthorizationError, InvalidConfigError,
 )
 from .value_type import TEXT, BYTE_ARRAY
+from .codec import SINETStreamMessageEncoder, SINETStreamMessageDecoder
 
 __all__ = [
     MessageReader, MessageWriter, AsyncMessageWriter, AsyncMessageReader,
     AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE, DEFAULT_CLIENT_ID,
     Metrics,
 
     SinetError, NoServiceError, NoConfigError, InvalidArgumentError,
     ConnectionError, AlreadyConnectedError, UnsupportedServiceTypeError,
     InvalidMessageError, AuthorizationError, InvalidConfigError,
 
-    TEXT, BYTE_ARRAY
+    TEXT, BYTE_ARRAY,
+
+    SINETStreamMessageEncoder, SINETStreamMessageDecoder,
 ]
```

### Comparing `sinetstream-1.8.0/src/sinetstream/__main__.py` & `sinetstream-1.8.1/src/sinetstream/__main__.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/api.py` & `sinetstream-1.8.1/src/sinetstream/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,16 +165,16 @@
     crypto = params["crypto"]
     if "password" in crypto:
         password = crypto["password"]
         if type(password) is str:
             crypto["password"] = {"value": password}
 
 
-def merge_parameter(service, kwargs, default_values, config=None, config_file=None):
-    service, raw_params = get_config_params(service, config, config_file)
+def merge_parameter(service, kwargs, default_values, config=None, config_file=None, no_config=False):
+    service, raw_params = get_config_params(service, config, config_file) if not no_config else (None, {})
     svc_params = convert_params(raw_params)
     # Merge parameters
     # Priority:
     #  ctor's argument (highest)
     #  config file
     #  sinetstream's default parameter
     #  plugin's default parameter (lowest)
@@ -467,27 +467,38 @@
             return {k: f(ipath, kwargs) for k, f in lst.items()}
         else:
             f = lst.get(ipath[0], None)
             if f is None:
                 return None
             return f(ipath[1:], kwargs)
 
+    def _debug_get_plugin(self):
+        return self._plugin
+
 
 class BaseMessageReader(MessageIO):
     default_params = {
         **default_params,
         "receive_timeout_ms": float("inf"),
     }
 
-    def __init__(self, registry, service, topics=None, config=None, config_file=None, **kwargs):
+    def __init__(self,
+                 registry,
+                 service=None,
+                 topics=None,
+                 config=None,
+                 config_file=None,
+                 no_config=False,
+                 **kwargs):
         service, params = merge_parameter(service,
                                           kwargs,
                                           BaseMessageReader.default_params,
                                           config=config,
-                                          config_file=config_file)
+                                          config_file=config_file,
+                                          no_config=no_config)
         params["topics"] = _setup_topics(params, topics)
         super().__init__(service, params, registry)
         self.unmarshaller = Unmarshaller() if not params.get("user_data_only") else None
         self.value_deserializer = self._setup_deserializer()
         self.decompressor = self._setup_decompressor()
 
     @property
@@ -545,25 +556,25 @@
         self._plugin.seek_to_beginning()
 
     def seek_to_end(self):
         self._plugin.seek_to_end()
 
 
 READER_USAGE = '''MessageReader(
-    service=SERVICE,                 # Service name defined in the configuration file. (REQUIRED)
+    service=SERVICE,                 # Service name defined in the configuration file.
     topics=TOPICS,                   # The topic to receive.
     config=CONFIG,                   # Config name on the config-server.
     consistency=AT_MOST_ONCE,        # consistency: AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE
     client_id=DEFAULT_CLIENT_ID,     # If not specified, the value is automatically generated.
     value_type=BYTE_ARRAY,           # The type of message.
     value_deserializer=None          # If not specified, use default deserializer according to valueType.
 )'''
 
 ASYNC_READER_USAGE = '''AsyncMessageReader(
-    service=SERVICE,                 # Service name defined in the configuration file. (REQUIRED)
+    service=SERVICE,                 # Service name defined in the configuration file.
     topics=TOPICS,                   # The topic to receive.
     config=CONFIG,                   # Config name on the config-server.
     consistency=AT_MOST_ONCE,        # consistency: AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE
     client_id=DEFAULT_CLIENT_ID,     # If not specified, the value is automatically generated.
     value_type=BYTE_ARRAY,           # The type of message.
     value_deserializer=None          # If not specified, use default deserializer according to valueType.
 )'''
@@ -572,15 +583,15 @@
 class MessageReader(BaseMessageReader):
     registry = Registry("sinetstream.reader", PluginMessageReader)
 
     @staticmethod
     def usage():
         return READER_USAGE
 
-    def __init__(self, service, topics=None, config=None, config_file=None, **kwargs):
+    def __init__(self, service=None, topics=None, config=None, config_file=None, **kwargs):
         logger.debug("MessageReader:init")
         super().__init__(MessageReader.registry, service, topics, config, config_file, **kwargs)
         self.debug_inject_msg_bytes = None  # for injection: None or tuple (message, topic, raw)
 
     def __iter__(self):
         logger.debug("MessageReader:iter")
         self._iter = self._plugin.__iter__()
@@ -596,55 +607,63 @@
             return self._make_message(message, topic, raw)
         except Exception:
             self.iometrics.update_err()
             raise
 
 
 WRITER_USAGE = '''MessageWriter(
-    service=SERVICE,                 # Service name defined in the configuration file. (REQUIRED)
+    service=SERVICE,                 # Service name defined in the configuration file.
     topic=TOPIC,                     # The topic to send.
     config=CONFIG,                   # Config name on the config-server.
     consistency=AT_MOST_ONCE,        # consistency: AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE
     client_id=DEFAULT_CLIENT_ID,     # If not specified, the value is automatically generated.
     value_type=BYTE_ARRAY,           # The type of message.
     value_serializer=None            # If not specified, use default serializer according to valueType.
 )'''
 
 ASYNC_WRITER_USAGE = '''AsyncMessageWriter(
-    service=SERVICE,                 # Service name defined in the configuration file. (REQUIRED)
+    service=SERVICE,                 # Service name defined in the configuration file.
     topic=TOPIC,                     # The topic to send.
     config=CONFIG,                   # Config name on the config-server.
     consistency=AT_MOST_ONCE,        # consistency: AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE
     client_id=DEFAULT_CLIENT_ID,     # If not specified, the value is automatically generated.
     value_type=BYTE_ARRAY,           # The type of message.
     value_serializer=None            # If not specified, use default serializer according to valueType.
 )'''
 
 
 class BaseMessageWriter(MessageIO):
     default_params = {
         **default_params
     }
 
-    def __init__(self, registry, service, topic=None, config=None, config_file=None, **kwargs):
+    def __init__(self,
+                 registry,
+                 service=None,
+                 topic=None,
+                 config=None,
+                 config_file=None,
+                 no_config=False,
+                 **kwargs):
         logger.debug("MessageWriter:init")
         service, params = merge_parameter(service,
                                           kwargs,
                                           MessageWriter.default_params,
                                           config=config,
-                                          config_file=config_file)
+                                          config_file=config_file,
+                                          no_config=no_config)
         params["topic"] = _setup_topic(params, topic)
         super().__init__(service, params, registry)
         self.marshaller = Marshaller() if not params.get("user_data_only") else None
         self.value_serializer = self._setup_serializer()
         self.compressor = self._setup_compressor()
         self.debug_last_msg_bytes = None  # for inspection
 
-    def _publish(self, msg):
-        tstamp = int(time.time() * 1000_000)
+    def _publish(self, msg, timestamp):
+        tstamp = int((timestamp if timestamp is not None else time.time()) * 1000_000)
         msg_bytes = PluginMessage(self._to_bytes(msg, tstamp))
         msg_bytes.set_timestamp(tstamp)  # for s3-broker
         if self.debug_last_msg_bytes is not None:
             self.debug_last_msg_bytes = msg_bytes
             return True
         return self._plugin.publish(msg_bytes)
 
@@ -703,32 +722,33 @@
 class MessageWriter(BaseMessageWriter):
     registry = Registry("sinetstream.writer", PluginMessageWriter)
 
     @staticmethod
     def usage():
         return WRITER_USAGE
 
-    def __init__(self, service, topic=None, config=None, config_file=None, **kwargs):
+    def __init__(self, service=None, topic=None, config=None, config_file=None, **kwargs):
         super().__init__(MessageWriter.registry, service, topic, config, config_file, **kwargs)
 
-    def publish(self, msg):
+    def publish(self, msg, timestamp=None):
         try:
-            return super()._publish(msg)
+            return super()._publish(msg, timestamp)
         except Exception:
             self.iometrics.update_err()
             raise
 
 
 def _setup_topic(params, topic):
     if topic is not None:
         ret = topic
     elif "topic" in params:
         ret = params["topic"]
     else:
-        raise InvalidArgumentError("You must specify a topic.")
+        # raise InvalidArgumentError("You must specify a topic.")
+        return None
 
     if isinstance(ret, list):
         num_topic = len(ret)
         if num_topic > 1:
             raise InvalidArgumentError("You cannot specify multiple topics.")
         elif num_topic == 0:
             raise InvalidArgumentError("You must specify a topic.")
@@ -741,48 +761,49 @@
     if topics is not None:
         ret = topics
     elif "topics" in params:
         ret = params["topics"]
     elif "topic" in params:
         ret = params["topic"]
     else:
-        raise InvalidArgumentError("You must specify several topics.")
+        # raise InvalidArgumentError("You must specify several topics.")
+        return None
 
     if isinstance(ret, list) and len(ret) == 0:
         raise InvalidArgumentError("You must specify several topics.")
     return ret
 
 
 class AsyncMessageWriter(BaseMessageWriter):
     registry = Registry("sinetstream.async_writer", PluginAsyncMessageWriter)
 
     @staticmethod
     def usage():
         return ASYNC_WRITER_USAGE
 
-    def __init__(self, service, topic=None, config=None, config_file=None, **kwargs):
+    def __init__(self, service=None, topic=None, config=None, config_file=None, **kwargs):
         super().__init__(AsyncMessageWriter.registry, service, topic, config, config_file, **kwargs)
 
     def _err(self, e):
         self.iometrics.update_err()
         raise e
 
-    def publish(self, msg):
-        promise = super()._publish(msg)
+    def publish(self, msg, timestamp=None):
+        promise = super()._publish(msg, timestamp)
         return promise.catch(lambda e: self._err(e))
 
 
 class AsyncMessageReader(BaseMessageReader):
     registry = Registry("sinetstream.async_reader", PluginAsyncMessageReader)
 
     @staticmethod
     def usage():
         return ASYNC_READER_USAGE
 
-    def __init__(self, service, topics=None, config=None, config_file=None, **kwargs):
+    def __init__(self, service=None, topics=None, config=None, config_file=None, **kwargs):
         logger.debug("AsyncMessageReader:init")
         super().__init__(AsyncMessageReader.registry, service, topics, config, config_file, **kwargs)
         self._executor = None
         self._on_message = None
         self._on_failure = None
 
     def open(self):
```

### Comparing `sinetstream-1.8.0/src/sinetstream/compression.py` & `sinetstream-1.8.1/src/sinetstream/compression.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/config_client.py` & `sinetstream-1.8.1/src/sinetstream/config_client.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/configs.py` & `sinetstream-1.8.1/src/sinetstream/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     elif isinstance(x, SecretValue):
         ev, fp = x.get()
         return decrypt_sec_data(ev, fp)
     else:
         return x
 
 
-def get_config_params(service, config=None, config_file=None, **kwargs):
+def get_config_params(service=None, config=None, config_file=None, **kwargs):
     if config is None:
         service, params = get_config_params_local(service, config_file, **kwargs)
     else:
         service, params = get_config_params_server(service, config, **kwargs)
     if params is None:
         logger.error(f"invalid service: {service}")
         raise NoServiceError()
```

### Comparing `sinetstream-1.8.0/src/sinetstream/crypto.py` & `sinetstream-1.8.1/src/sinetstream/crypto.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/error.py` & `sinetstream-1.8.1/src/sinetstream/error.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/marshal.py` & `sinetstream-1.8.1/src/sinetstream/marshal.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/spi.py` & `sinetstream-1.8.1/src/sinetstream/spi.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/utils.py` & `sinetstream-1.8.1/src/sinetstream/utils.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream/value_type.py` & `sinetstream-1.8.1/src/sinetstream/value_type.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.8.0/src/sinetstream.egg-info/PKG-INFO` & `sinetstream-1.8.1/src/sinetstream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sinetstream
-Version: 1.8.0
+Version: 1.8.1
 Summary: Library for operating messaging systems such as Apache Kafka and MQTT with the same API.
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
 Description-Content-Type: text/markdown
 
 <!--
 Copyright (C) 2020 National Institute of Informatics
 
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
```

### Comparing `sinetstream-1.8.0/src/sinetstream.egg-info/SOURCES.txt` & `sinetstream-1.8.1/src/sinetstream.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.cfg
 setup.py
 src/sinetstream/__init__.py
 src/sinetstream/__main__.py
 src/sinetstream/api.py
+src/sinetstream/codec.py
 src/sinetstream/compression.py
 src/sinetstream/config_client.py
 src/sinetstream/configs.py
 src/sinetstream/crypto.py
 src/sinetstream/error.py
 src/sinetstream/marshal.py
 src/sinetstream/spi.py
```

