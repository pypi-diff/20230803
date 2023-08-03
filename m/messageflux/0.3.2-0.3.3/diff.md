# Comparing `tmp/messageflux-0.3.2.tar.gz` & `tmp/messageflux-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.3.2.tar", last modified: Sat Jul 29 07:16:22 2023, max compression
+gzip compressed data, was "messageflux-0.3.3.tar", last modified: Thu Aug  3 12:45:28 2023, max compression
```

## Comparing `messageflux-0.3.2.tar` & `messageflux-0.3.3.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-29 07:16:11.000000 messageflux-0.3.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 07:16:11.000000 messageflux-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 07:16:11.000000 messageflux-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-29 07:16:22.460383 messageflux-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-29 07:16:11.000000 messageflux-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 07:16:12.000000 messageflux-0.3.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:11.000000 messageflux-0.3.2/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-29 07:16:11.000000 messageflux-0.3.2/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 07:16:11.000000 messageflux-0.3.2/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-29 07:16:11.000000 messageflux-0.3.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-29 07:16:11.000000 messageflux-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-29 07:16:11.000000 messageflux-0.3.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 07:16:22.000000 messageflux-0.3.2/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:16:22.460383 messageflux-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 12:45:12.000000 messageflux-0.3.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 12:45:12.000000 messageflux-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 12:45:12.000000 messageflux-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-03 12:45:28.869708 messageflux-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-03 12:45:12.000000 messageflux-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 12:45:14.000000 messageflux-0.3.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:12.000000 messageflux-0.3.3/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 12:45:12.000000 messageflux-0.3.3/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 12:45:12.000000 messageflux-0.3.3/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/fastmessage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 12:45:12.000000 messageflux-0.3.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-03 12:45:12.000000 messageflux-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-03 12:45:12.000000 messageflux-0.3.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-03 12:45:28.000000 messageflux-0.3.3/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-fastmessage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-objectstorage_mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-rabbitmq_mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:45:28.869708 messageflux-0.3.3/setup.cfg
```

### Comparing `messageflux-0.3.2/LICENSE` & `messageflux-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/PKG-INFO` & `messageflux-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.2
+Version: 0.3.3
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
@@ -14,17 +14,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: rabbitmq
-Provides-Extra: objectstorage
 Provides-Extra: fastmessage
+Provides-Extra: objectstorage
+Provides-Extra: objectstorage_mypy
+Provides-Extra: rabbitmq
+Provides-Extra: rabbitmq_mypy
 Provides-Extra: all
 License-File: LICENSE
 
 # MessageFlux
 
 [![stars](https://badgen.net/github/stars/Avivsalem/MessageFlux)](https://github.com/Avivsalem/MessageFlux/stargazers)
 [![license](https://badgen.net/github/license/Avivsalem/MessageFlux/)](https://github.com/Avivsalem/MessageFlux/blob/main/LICENSE)
```

### Comparing `messageflux-0.3.2/README.md` & `messageflux-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/_custom_build/make_all_extra_requirements.py` & `messageflux-0.3.3/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/base_service.py` & `messageflux-0.3.3/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/fastmessage_handler.py` & `messageflux-0.3.3/messageflux/fastmessage_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
 import json
 import logging
 from dataclasses import dataclass
 from typing import Optional, Callable, Dict, List, Any, TypeVar, Union
 
 from messageflux import InputDevice
+from messageflux.iodevices.base import InputDeviceManager, OutputDeviceManager
 from messageflux.iodevices.base.common import MessageBundle, Message
-from messageflux.pipeline_service import PipelineHandlerBase, PipelineResult
+from messageflux.pipeline_service import PipelineHandlerBase, PipelineResult, PipelineService
 
 try:
     from pydantic.typing import get_all_type_hints
     from pydantic import BaseModel, parse_raw_as, create_model, ValidationError, Extra
     from pydantic.config import get_config
 except ImportError as ex:
     raise ImportError('Please Install the required extra: messageflux[fastmessage]') from ex
@@ -32,14 +33,18 @@
     pass
 
 
 class SpecialDefaultValueException(FastMessageException):
     pass
 
 
+class UnnamedCallableException(FastMessageException):
+    pass
+
+
 class InputDeviceName(str):
     """
     a place holder class for input_device name
     """
     pass
 
 
@@ -180,15 +185,16 @@
             output_data = json.dumps(value, default=json_encoder).encode()
             output_bundle = MessageBundle(message=Message(data=output_data))
 
         return PipelineResult(output_device_name=output_device, message_bundle=output_bundle)
 
 
 class FastMessage(PipelineHandlerBase):
-    def __init__(self, default_output_device: Optional[str] = None,
+    def __init__(self,
+                 default_output_device: Optional[str] = None,
                  validation_error_handler: Optional[Callable[
                      [InputDevice, MessageBundle, ValidationError],
                      Optional[Union[PipelineResult, List[PipelineResult]]]]] = None):
         """
 
         :param default_output_device: an optional default output device to send callaback results to,
         unless mapped otherwise
@@ -213,39 +219,48 @@
         """
         registers optional handler that will be called on validation errors,
         in order to give the user a chance to handle them gracefully
         :param handler: the handler to register
         """
         self._validation_error_handler = handler
 
+    def _get_callable_name(self, callback: Callable) -> str:
+        try:
+            return getattr(callback, "__name__")
+        except AttributeError as ex:
+            raise UnnamedCallableException(f"Callable {repr(callback)} doesn't have a name") from ex
+
     def register_callback(self,
                           callback: Callable,
-                          input_device: str,
+                          input_device: str = _DEFAULT,
                           output_device: Optional[str] = _DEFAULT):
         """
         registers a callback to a device
 
         :param callback: the callback to register
         :param input_device: the input device to register the callback to
         :param output_device:  optional output device to route the return value of the callback to.
         None means no output routing.
         if callback returns None, no routing will be made even if 'output_device' is not None
         """
+        if input_device is _DEFAULT:
+            input_device = self._get_callable_name(callback)
+
         if input_device in self._wrappers:
             raise DuplicateCallbackException(f"Can't register more than one callback on device '{input_device}'")
 
         if output_device is _DEFAULT:
             output_device = self._default_output_device
 
         self._wrappers[input_device] = _CallbackWrapper(callback=callback,
                                                         input_device=input_device,
                                                         output_device=output_device)
 
     def map(self,
-            input_device: str,
+            input_device: str = _DEFAULT,
             output_device: Optional[str] = _DEFAULT) -> Callable[[_CALLABLE_TYPE], _CALLABLE_TYPE]:
         """
         this is the decorator method
 
         :param input_device: the input device to register the decorated method on
         :param output_device: optional output device to route the return value of the callback to.
         if callback returns None, no routing will be made even if 'output_device' is not None
@@ -269,7 +284,31 @@
         try:
             return callback_wrapper(input_device=input_device, message_bundle=message_bundle)
         except ValidationError as ve:
             if self._validation_error_handler is None:
                 raise
 
             return self._validation_error_handler(input_device, message_bundle, ve)
+
+    def create_service(self, *,
+                       input_device_manager: InputDeviceManager,
+                       input_device_names: Optional[Union[List[str], str]] = None,
+                       output_device_manager: Optional[OutputDeviceManager] = None,
+                       **kwargs) -> PipelineService:
+        """
+        creates a PipelineService, with this FastMessage object as its handler
+
+        :param input_device_manager: the input device manager to read items from
+        :param input_device_names: Optional. the list of input device names to read from
+        (defaults to all the registered mappings)
+        :param output_device_manager: Optional. the output device manager to use
+        :param **kwargs: passed to PipelineService __init__ as is
+        :return: the created PipelineService
+        """
+        if input_device_names is None:
+            input_device_names = self.input_devices
+
+        return PipelineService(input_device_manager=input_device_manager,
+                               input_device_names=input_device_names,
+                               pipeline_handler=self,
+                               output_device_manager=output_device_manager,
+                               **kwargs)
```

### Comparing `messageflux-0.3.2/messageflux/iodevices/base/__init__.py` & `messageflux-0.3.3/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/base/common.py` & `messageflux-0.3.3/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/base/input_devices.py` & `messageflux-0.3.3/messageflux/iodevices/base/input_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.3.3/messageflux/iodevices/base/input_transaction.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/base/output_devices.py` & `messageflux-0.3.3/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.3.3/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.3.3/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.3.3/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
 import os
 import re
 from abc import abstractmethod, ABCMeta
 from hashlib import md5
-from typing import Optional, BinaryIO, Dict, Any, Tuple
+from typing import Optional, BinaryIO, Dict, Any, Tuple, TYPE_CHECKING
 
 from messageflux.iodevices.base.common import MessageBundle, Message
 from messageflux.iodevices.message_store_device_wrapper.message_store_base import MessageStoreException, \
     MessageStoreBase
-from messageflux.iodevices.objectstorage.s3api.s3bucket import BUCKET_NAME_VALIDATOR, S3Bucket, S3ServiceResource
+from messageflux.iodevices.objectstorage.s3api.s3bucket import BUCKET_NAME_VALIDATOR, S3Bucket
 from messageflux.metadata_headers import MetadataHeaders
 from messageflux.utils import get_random_id, json_safe_encoder
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3ServiceResource
+
 KEY_HEADER_CONST = "__KEY__"
 
 _S3_TIMEOUT = int(os.environ.get("S3_TIMEOUT", 1))
 _S3_RETRIES = int(os.environ.get("S3_RETRIES", 2))
 
 
 class BucketNameFormatterBase:
@@ -60,15 +63,15 @@
 class _S3MessageStoreBase(MessageStoreBase, metaclass=ABCMeta):
     """
     a message store that uses S3 as it's base
     """
     _ORIGINAL_HEADERS_KEY = "originalheaders"
 
     def __init__(self,
-                 s3_resource: S3ServiceResource,
+                 s3_resource: 'S3ServiceResource',
                  magic: bytes,
                  auto_create_bucket: bool = False,
                  bucket_name_formatter: Optional[BucketNameFormatterBase] = None):
         """
         An S3 based message store
 
         :param s3_resource: the s3 resource from boto
@@ -192,15 +195,15 @@
 
 class S3MessageStore(_S3MessageStoreBase):
     """
     a message store that uses S3 as it's base
     """
 
     def __init__(self,
-                 s3_resource: S3ServiceResource,
+                 s3_resource: 'S3ServiceResource',
                  magic: bytes = b"__S3_MSGSTORE__",
                  auto_create_bucket: bool = False,
                  bucket_name_formatter: Optional[BucketNameFormatterBase] = None,
                  put_object_extra_args: Optional[Dict[str, Any]] = None):
         """
         An S3 based message store
 
@@ -231,15 +234,15 @@
 
 class S3UploadMessageStore(_S3MessageStoreBase):
     """
     a message store that uses S3 as it's base (using upload_file method)
     """
 
     def __init__(self,
-                 s3_resource: S3ServiceResource,
+                 s3_resource: 'S3ServiceResource',
                  magic: bytes = b"__S3_UPLOAD_MSGSTORE__",
                  auto_create_bucket: bool = False,
                  bucket_name_formatter: Optional[BucketNameFormatterBase] = None,
                  upload_extra_args: Optional[Dict[str, Any]] = None):
         """
         An S3 based message store
```

### Comparing `messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from datetime import datetime
 from io import BytesIO
 from typing import Optional, Dict, Any, Iterator, TYPE_CHECKING, Union, IO
 from typing_extensions import Literal
 from urllib.parse import urljoin
 
 try:
-    from mypy_boto3_s3 import S3ServiceResource
-    from mypy_boto3_s3.service_resource import ObjectSummary
-    from mypy_boto3_s3.type_defs import LifecycleConfigurationTypeDef, GetObjectOutputTypeDef
     from boto3.s3.inject import ClientError
 except ImportError as ex:
     raise ImportError('Please Install the required extra: messageflux[objectstorage]') from ex
 
 BUCKET_NAME_VALIDATOR = re.compile(r'^[a-z0-9][a-z0-9.\-]{1,61}[a-z0-9]$')
 
 if TYPE_CHECKING:
+    from mypy_boto3_s3.type_defs import LifecycleConfigurationTypeDef, GetObjectOutputTypeDef
+    from mypy_boto3_s3 import S3ServiceResource
+    from mypy_boto3_s3.service_resource import ObjectSummary
     from _typeshed import SupportsRead
 
 
 class S3BucketException(Exception):
     """
     represents errors thrown from S3 bucket
     """
@@ -42,22 +42,22 @@
 
 
 class S3Object:
     """
     represents an s3 object with lazy content get
     """
 
-    def __init__(self, object_summery: ObjectSummary, object_cache: Optional[GetObjectOutputTypeDef] = None):
+    def __init__(self, object_summery: 'ObjectSummary', object_cache: Optional['GetObjectOutputTypeDef'] = None):
         self._object_summery = object_summery
         self._object_cache = object_cache
         self._body: Optional[BytesIO] = None
         self._metadata: Optional[Dict[str, str]] = None
 
     @property
-    def _object_dict(self) -> GetObjectOutputTypeDef:
+    def _object_dict(self) -> 'GetObjectOutputTypeDef':
         if self._object_cache is None:
             self._object_cache = self._object_summery.get()
         return self._object_cache
 
     @property
     def key(self) -> str:
         """
@@ -112,15 +112,15 @@
 
 class S3Bucket:
     """
     this class represents a single S3 Bucket
     """
 
     @staticmethod
-    def create_bucket(s3_resource: S3ServiceResource,
+    def create_bucket(s3_resource: 'S3ServiceResource',
                       bucket_name: str,
                       lifetime_in_days: Optional[int] = None,
                       allow_public_access=False) -> 'S3Bucket':
         """
         creates and returns a bucket
 
         :param s3_resource: the s3 resource to use
@@ -135,25 +135,25 @@
 
         if allow_public_access:
             bucket.allow_public_access()
 
         return bucket
 
     @staticmethod
-    def list_buckets(s3_resource: S3ServiceResource) -> Iterator['S3Bucket']:
+    def list_buckets(s3_resource: 'S3ServiceResource') -> Iterator['S3Bucket']:
         """
         returns a list of all the buckets in this client
 
         :param s3_resource: the s3 resource to use
         :return: iterator of bucket objects
         """
         for bucket in s3_resource.buckets.all():
             yield S3Bucket(bucket_name=bucket.name, s3_resource=s3_resource)
 
-    def __init__(self, bucket_name: str, s3_resource: S3ServiceResource, auto_create: bool = False):
+    def __init__(self, bucket_name: str, s3_resource: 'S3ServiceResource', auto_create: bool = False):
         """
         this class represents a single S3 Bucket
 
         :param bucket_name: the name of the bucket to work with
         :param s3_resource: the s3 resource to use
         :param auto_create: should we create the bucket if it doesn't exist?
         """
@@ -184,15 +184,15 @@
         :param force: True will delete all objects on bucket, before deleting the bucket
         """
         if force:
             self.clear_objects()
         self._s3bucket.delete()
 
     @property
-    def s3_resource(self) -> S3ServiceResource:
+    def s3_resource(self) -> 'S3ServiceResource':
         """
         the client for this bucket
         """
         return self._s3_resource
 
     @property
     def name(self) -> str:
@@ -242,15 +242,15 @@
         try:
             status: Literal['Disabled', 'Enabled']
             if days <= 0:
                 status = 'Disabled'
                 days = 1
             else:
                 status = 'Enabled'
-            lc: LifecycleConfigurationTypeDef = {
+            lc: 'LifecycleConfigurationTypeDef' = {
                 'Rules': [{
                     'Status': status,
                     'Prefix': '',
                     'Expiration': {
                         'Days': days
                     },
                     'ID': 'expire'
```

### Comparing `messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from typing import TYPE_CHECKING
+
 try:
     from boto3.session import Config, Session  # type: ignore
-    from mypy_boto3_s3 import S3ServiceResource
 except ImportError as ex:
     raise ImportError('Please Install the required extra: messageflux[objectstorage]') from ex
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3ServiceResource
+
 _S3_DEFAULT_TIMEOUT = 1
 _S3_DEFAULT_RETRIES = 2
 
 
 class S3Client:
     """
     This class exists for compatibility purposes only.
@@ -23,27 +27,27 @@
         """
         represents an s3 client object
 
         :param endpoint: the endpoint to s3 (url)
         :param access_key: the access key
         :param secret_key: the secret key
         """
-        self._s3: S3ServiceResource = Session().resource('s3',
-                                                         aws_access_key_id=access_key,
-                                                         aws_secret_access_key=secret_key,
-                                                         endpoint_url=endpoint,
-                                                         verify=False,
-                                                         config=Config(
-                                                             signature_version='s3',
-                                                             connect_timeout=timeout,
-                                                             retries={
-                                                                 "max_attempts": retries},
-                                                             s3={'addressing_style': 'path'}))
+        self._s3: 'S3ServiceResource' = Session().resource('s3',
+                                                           aws_access_key_id=access_key,
+                                                           aws_secret_access_key=secret_key,
+                                                           endpoint_url=endpoint,
+                                                           verify=False,
+                                                           config=Config(
+                                                               signature_version='s3',
+                                                               connect_timeout=timeout,
+                                                               retries={
+                                                                   "max_attempts": retries},
+                                                               s3={'addressing_style': 'path'}))
 
     @property
-    def s3_resource(self) -> S3ServiceResource:
+    def s3_resource(self) -> 'S3ServiceResource':
         """
         returns the actual s3 client
 
         :return: the actual s3 client
         """
         return self._s3
```

### Comparing `messageflux-0.3.2/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.3.3/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.3.3/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.3.3/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.3.3/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/message_handling_service.py` & `messageflux-0.3.3/messageflux/message_handling_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.3.3/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.3.3/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/pipeline_service.py` & `messageflux-0.3.3/messageflux/pipeline_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,20 @@
     a service that uses a PipelineHandler object to process messages from input, and send to output
     """
 
     def __init__(self, *,
                  pipeline_handler: PipelineHandlerBase,
                  output_device_manager: Optional[OutputDeviceManager] = None,
                  **kwargs):
+        """
+
+        :param pipeline_handler: the pipeline handler to use for handling the messages
+        :param output_device_manager: Optional. the output device manager to send messages to
+        :param **kwargs: passed to parent as is
+        """
         super().__init__(**kwargs)
         self._output_device_manager = output_device_manager
         self._pipeline_handler = pipeline_handler
 
     def _prepare_service(self):
         super()._prepare_service()
         if self._output_device_manager is not None:
```

### Comparing `messageflux-0.3.2/messageflux/server_loop_service.py` & `messageflux-0.3.3/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.3.3/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/utils/__init__.py` & `messageflux-0.3.3/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/utils/context.py` & `messageflux-0.3.3/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux/utils/filesystem.py` & `messageflux-0.3.3/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.2/messageflux.egg-info/PKG-INFO` & `messageflux-0.3.3/messageflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.2
+Version: 0.3.3
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
@@ -14,17 +14,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: rabbitmq
-Provides-Extra: objectstorage
 Provides-Extra: fastmessage
+Provides-Extra: objectstorage
+Provides-Extra: objectstorage_mypy
+Provides-Extra: rabbitmq
+Provides-Extra: rabbitmq_mypy
 Provides-Extra: all
 License-File: LICENSE
 
 # MessageFlux
 
 [![stars](https://badgen.net/github/stars/Avivsalem/MessageFlux)](https://github.com/Avivsalem/MessageFlux/stargazers)
 [![license](https://badgen.net/github/license/Avivsalem/MessageFlux/)](https://github.com/Avivsalem/MessageFlux/blob/main/LICENSE)
```

### Comparing `messageflux-0.3.2/messageflux.egg-info/SOURCES.txt` & `messageflux-0.3.3/messageflux.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements-all.txt
 requirements-dev.txt
 requirements-fastmessage.txt
 requirements-objectstorage.txt
+requirements-objectstorage_mypy.txt
 requirements-rabbitmq.txt
+requirements-rabbitmq_mypy.txt
 requirements.txt
 _custom_build/__init__.py
 _custom_build/backend.py
 _custom_build/make_all_extra_requirements.py
 messageflux/__init__.py
 messageflux/base_service.py
 messageflux/fastmessage_handler.py
```

### Comparing `messageflux-0.3.2/pyproject.toml` & `messageflux-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,17 @@
 [tool.setuptools.dynamic]
 dependencies = { file = "requirements.txt" }
 version = { file = "VERSION" }
 
 
 [tool.setuptools.dynamic.optional-dependencies]
 dev = { file = "requirements-dev.txt" }
-rabbitmq = { file = "requirements-rabbitmq.txt" }
-objectstorage = { file = "requirements-objectstorage.txt" }
 fastmessage = { file = "requirements-fastmessage.txt" }
+objectstorage = { file = "requirements-objectstorage.txt" }
+objectstorage_mypy = { file = "requirements-objectstorage_mypy.txt" }
+rabbitmq = { file = "requirements-rabbitmq.txt" }
+rabbitmq_mypy = { file = "requirements-rabbitmq_mypy.txt" }
 all = { file = "requirements-all.txt" }
```

