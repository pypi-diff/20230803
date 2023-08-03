# Comparing `tmp/edx_event_bus_kafka-5.1.0.tar.gz` & `tmp/edx_event_bus_kafka-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_kafka-5.1.0.tar", last modified: Wed May 17 16:56:09 2023, max compression
+gzip compressed data, was "edx_event_bus_kafka-5.2.0.tar", last modified: Thu Aug  3 17:34:16 2023, max compression
```

## Comparing `edx_event_bus_kafka-5.1.0.tar` & `edx_event_bus_kafka-5.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    12438 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19886 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6755 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.967654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.971654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30796 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    15097 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.971654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    31454 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    18850 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7678 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.971654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.963654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.971654 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19886 2023-05-17 16:56:09.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-17 16:56:09.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 16:56:09.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 16:56:09.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-17 16:56:09.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-17 16:56:09.000000 edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:56:09.975654 edx_event_bus_kafka-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-17 16:56:05.000000 edx_event_bus_kafka-5.1.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    12572 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20020 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6755 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.787995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30796 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15751 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31454 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19122 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7678 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.787995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20020 2023-08-03 17:34:16.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-08-03 17:34:16.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:34:16.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:34:16.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-03 17:34:16.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-08-03 17:34:16.000000 edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-08-03 17:34:16.795995 edx_event_bus_kafka-5.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:34:16.791995 edx_event_bus_kafka-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-03 17:34:12.000000 edx_event_bus_kafka-5.2.0/tests/test_models.py
```

### Comparing `edx_event_bus_kafka-5.1.0/CHANGELOG.rst` & `edx_event_bus_kafka-5.2.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.2.0] - 2023-08-03
+********************
+Changed
+=======
+* Added event_data_as_dict to ProducingContext for easier replay from logs
+
 [5.1.0] - 2023-05-17
 ********************
 Changed
 =======
 * Reconfigured serializers to use topic_record_name_strategy, allowing multiple event types per topic
 
 [5.0.0] - 2023-05-17
```

### Comparing `edx_event_bus_kafka-5.1.0/LICENSE.txt` & `edx_event_bus_kafka-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/PKG-INFO` & `edx_event_bus_kafka-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_kafka
-Version: 5.1.0
+Version: 5.2.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -204,14 +204,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.2.0] - 2023-08-03
+********************
+Changed
+=======
+* Added event_data_as_dict to ProducingContext for easier replay from logs
+
 [5.1.0] - 2023-05-17
 ********************
 Changed
 =======
 * Reconfigured serializers to use topic_record_name_strategy, allowing multiple event types per topic
 
 [5.0.0] - 2023-05-17
```

### Comparing `edx_event_bus_kafka-5.1.0/README.rst` & `edx_event_bus_kafka-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/config.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/consumer.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/consumer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/producer.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/producer.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,34 +132,50 @@
         The key's schema, as a string.
     """
     subschema = descend_avro_schema(signal_serializer.schema, event_key_field.split("."))
     # Same as used by AvroSignalSerializer#schema_string in openedx-events
     return json.dumps(subschema, sort_keys=True)
 
 
+@lru_cache()
+def get_signal_serializer(signal: OpenEdxPublicSignal):
+    """
+    Get the AvroSignalSerializer for a signal
+
+    This is cached in order to save work re-transforming classes into Avro schemas.
+
+    Arguments:
+        signal: The OpenEdxPublicSignal to make a serializer for.
+
+    Returns:
+        An AvroSignalSerializer configured to serialize event data to dictionaries
+    """
+    return AvroSignalSerializer(signal)
+
+
 @lru_cache
 def get_serializers(signal: OpenEdxPublicSignal, event_key_field: str):
     """
-    Get the key and value serializers for a signal and a key field path.
+    Get the full key and value serializers for a signal and a key field path.
 
-    This is cached in order to save work re-transforming classes into Avro schemas.
+    This is cached in order to save work re-transforming AvroSignalSerializers into AvroSerializers.
 
     Arguments:
         signal: The OpenEdxPublicSignal to make a serializer for.
         event_key_field: Path to descend in the signal schema to find the subschema for the key
           (period-delimited string naming the field names to descend).
 
     Returns:
-        2-tuple of AvroSignalSerializers, for event key and value
+        2-tuple of AvroSerializers, for event key and value
     """
     client = get_schema_registry_client()
     if client is None:
         raise Exception('Cannot create Kafka serializers -- missing library or settings')
 
-    signal_serializer = AvroSignalSerializer(signal)
+    signal_serializer = get_signal_serializer(signal)
 
     def inner_to_dict(event_data, ctx=None):  # pylint: disable=unused-argument
         """Tells Avro how to turn objects into dictionaries."""
         return signal_serializer.to_dict(event_data)
 
     # Serializers for key and value components of Kafka event
     key_serializer = AvroSerializer(
@@ -187,14 +203,15 @@
     full_topic = attr.ib(type=str, default=None)
     event_key = attr.ib(type=str, default=None)
     signal = attr.ib(type=OpenEdxPublicSignal, default=None)
     initial_topic = attr.ib(type=str, default=None)
     event_key_field = attr.ib(type=str, default=None)
     event_data = attr.ib(type=dict, default=None)
     event_metadata = attr.ib(type=EventsMetadata, default=None)
+    event_data_as_json = attr.ib(type=str, default=None)
 
     def __repr__(self):
         """Create a logging-friendly string"""
         return " ".join([f"{key}={value!r}" for key, value in attr.asdict(self, recurse=False).items()])
 
     def on_event_deliver(self, err, evt):
         """
@@ -262,14 +279,15 @@
             event_metadata: An EventsMetadata object with all the metadata necessary for the CloudEvent spec
         """
 
         # keep track of the initial arguments for recreating the event in the logs if necessary later
         context = ProducingContext(signal=signal, initial_topic=topic, event_key_field=event_key_field,
                                    event_data=event_data, event_metadata=event_metadata)
         try:
+            context.event_data_as_json = json.dumps(get_signal_serializer(signal).to_dict(event_data))
             full_topic = get_full_topic(topic)
             context.full_topic = full_topic
 
             event_key = extract_event_key(event_data, event_key_field)
             context.event_key = event_key
             headers = _get_headers_from_metadata(event_metadata=event_metadata)
 
@@ -357,7 +375,8 @@
     return KafkaEventProducer(Producer(producer_settings))
 
 
 @receiver(setting_changed)
 def _reset_caches(sender, **kwargs):  # pylint: disable=unused-argument
     """Reset caches when settings change during unit tests."""
     get_serializers.cache_clear()
+    get_signal_serializer.cache_clear()
```

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_config.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_consumer.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_producer.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_producer.py`

 * *Files 3% similar despite different names*

```diff
@@ -241,14 +241,16 @@
         assert "initial_topic='topic'" in error_string
         assert "full_topic='dev-topic'" in error_string
         assert "event_key_field='bad_field'" in error_string
         assert "event_type='simple.signal'" in error_string
         assert "source='openedx/test/web'" in error_string
         assert f"id=UUID('{metadata.id}')" in error_string
         assert f"sourcehost='{metadata.sourcehost}'" in error_string
+        assert "event_data_as_json='{\"test_data\": {\"course_id\": \"id\", \"sub_name\": \"name\"}}'"\
+               in error_string
 
     @patch(
         'edx_event_bus_kafka.internal.producer.get_serializers', autospec=True,
         return_value=(
             lambda _key, _ctx: b'key-bytes-here',
             lambda _value, _ctx: b'value-bytes-here',
         )
@@ -279,14 +281,16 @@
         assert "event_key_field='test_data.course_id'" in error_string
         assert "source='openedx/test/web'" in error_string
         assert f"id=UUID('{metadata.id}')" in error_string
         assert f"sourcehost='{metadata.sourcehost}'" in error_string
         # since we didn't fail until after key extraction we should have an event_key to report
         assert "event_key='ABCx'" in error_string
         assert "error=bad!" in error_string
+        assert "event_data_as_json='{\"test_data\": {\"course_id\": \"ABCx\", \"sub_name\": \"name\"}}'"\
+               in error_string
 
     @override_settings(EVENT_BUS_KAFKA_POLL_INTERVAL_SEC=0.05)
     def test_polling_loop_terminates(self):
         """
         Test that polling loop stops as soon as the producer is garbage-collected.
         """
         call_count = 0
```

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/tests/test_utils.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/internal/utils.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/management/commands/produce_event.py` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/PKG-INFO` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-bus-kafka
-Version: 5.1.0
+Version: 5.2.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -204,14 +204,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.2.0] - 2023-08-03
+********************
+Changed
+=======
+* Added event_data_as_dict to ProducingContext for easier replay from logs
+
 [5.1.0] - 2023-05-17
 ********************
 Changed
 =======
 * Reconfigured serializers to use topic_record_name_strategy, allowing multiple event types per topic
 
 [5.0.0] - 2023-05-17
```

### Comparing `edx_event_bus_kafka-5.1.0/edx_event_bus_kafka.egg-info/SOURCES.txt` & `edx_event_bus_kafka-5.2.0/edx_event_bus_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/requirements/constraints.txt` & `edx_event_bus_kafka-5.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.1.0/setup.py` & `edx_event_bus_kafka-5.2.0/setup.py`

 * *Files identical despite different names*

