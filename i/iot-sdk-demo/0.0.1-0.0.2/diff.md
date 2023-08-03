# Comparing `tmp/iot-sdk-demo-0.0.1.tar.gz` & `tmp/iot-sdk-demo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iot-sdk-demo-0.0.1.tar", last modified: Wed Aug  2 12:26:22 2023, max compression
+gzip compressed data, was "dist\iot-sdk-demo-0.0.2.tar", last modified: Thu Aug  3 01:30:19 2023, max compression
```

## Comparing `iot-sdk-demo-0.0.1.tar` & `iot-sdk-demo-0.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/
--rw-rw-rw-   0        0        0    11357 2023-08-02 09:48:52.000000 iot-sdk-demo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       49 2023-08-02 12:26:00.000000 iot-sdk-demo-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      604 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-08-02 10:00:57.000000 iot-sdk-demo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/
--rw-rw-rw-   0        0        0      604 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1437 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 12:13:14.000000 iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1214 2023-08-02 12:13:08.000000 iot-sdk-demo-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/
--rw-rw-rw-   0        0        0       97 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     2315 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.1/src/config.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/core/
--rw-rw-rw-   0        0        0      832 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.1/src/core/applicationContext.py
--rw-rw-rw-   0        0        0     3294 2023-07-25 14:09:38.000000 iot-sdk-demo-0.0.1/src/core/eventInvoker.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/core/exception/
--rw-rw-rw-   0        0        0      176 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/core/exception/commonException.py
--rw-rw-rw-   0        0        0        0 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/core/exception/sdkException.py
--rw-rw-rw-   0        0        0     2327 2023-07-24 10:35:34.000000 iot-sdk-demo-0.0.1/src/core/exception/serviceException.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/core/job/
--rw-rw-rw-   0        0        0      905 2023-07-20 08:12:22.000000 iot-sdk-demo-0.0.1/src/core/job/contextUpLoadJob.py
--rw-rw-rw-   0        0        0      475 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/core/job/eventListenerJob.py
--rw-rw-rw-   0        0        0      271 2023-07-21 08:49:20.000000 iot-sdk-demo-0.0.1/src/core/job/mqttCheckMessageJob.py
--rw-rw-rw-   0        0        0      256 2023-07-21 02:43:53.000000 iot-sdk-demo-0.0.1/src/core/job/mqttHealthJob.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/core/loader/
--rw-rw-rw-   0        0        0     1350 2023-07-26 15:52:31.000000 iot-sdk-demo-0.0.1/src/core/loader/hardwareInfoLoader.py
--rw-rw-rw-   0        0        0     1555 2023-07-25 10:09:39.000000 iot-sdk-demo-0.0.1/src/core/loader/proxyLoader.py
--rw-rw-rw-   0        0        0     8251 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.1/src/core/loader/serversLoader.py
--rw-rw-rw-   0        0        0      210 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/core/loader/thingProxyFuncLoader.py
--rw-rw-rw-   0        0        0     2303 2023-07-21 03:01:27.000000 iot-sdk-demo-0.0.1/src/core/scheduleService.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/core/sender/
--rw-rw-rw-   0        0        0       67 2023-07-27 02:11:41.000000 iot-sdk-demo-0.0.1/src/core/sender/baseSender.py
--rw-rw-rw-   0        0        0      369 2023-07-27 02:49:45.000000 iot-sdk-demo-0.0.1/src/core/sender/hardwareUpLoadSender.py
--rw-rw-rw-   0        0        0     2998 2023-07-24 08:14:24.000000 iot-sdk-demo-0.0.1/src/core/serverInvoker.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/factory/
--rw-rw-rw-   0        0        0      392 2023-06-15 10:40:11.000000 iot-sdk-demo-0.0.1/src/factory/systemEventFactory.py
--rw-rw-rw-   0        0        0      690 2023-06-27 09:17:54.000000 iot-sdk-demo-0.0.1/src/factory/systemServiceFactory.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/model/
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/model/ujinja/
--rw-rw-rw-   0        0        0     7700 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/model/ujinja/source.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/pojo/
--rw-rw-rw-   0        0        0      746 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/pojo/capabilityBean.py
--rw-rw-rw-   0        0        0      545 2023-06-12 06:53:14.000000 iot-sdk-demo-0.0.1/src/pojo/eventBean.py
--rw-rw-rw-   0        0        0      892 2023-07-20 10:25:24.000000 iot-sdk-demo-0.0.1/src/pojo/serviceBean.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/proxy/
--rw-rw-rw-   0        0        0      166 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/proxy/proxyBase.py
--rw-rw-rw-   0        0        0      677 2023-07-24 10:01:52.000000 iot-sdk-demo-0.0.1/src/proxy/pythonServiceProxy.py
--rw-rw-rw-   0        0        0      570 2023-07-20 10:06:16.000000 iot-sdk-demo-0.0.1/src/proxy/thingProxy.py
--rw-rw-rw-   0        0        0     4213 2023-07-28 05:32:09.000000 iot-sdk-demo-0.0.1/src/proxySDK.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/router/
--rw-rw-rw-   0        0        0     1173 2023-07-25 09:57:46.000000 iot-sdk-demo-0.0.1/src/router/httpRouter.py
--rw-rw-rw-   0        0        0     2996 2023-07-24 07:55:12.000000 iot-sdk-demo-0.0.1/src/router/mqttRouter.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/systemService/
--rw-rw-rw-   0        0        0      153 2023-07-25 09:53:27.000000 iot-sdk-demo-0.0.1/src/systemService/httpService.py
--rw-rw-rw-   0        0        0     3176 2023-07-25 14:18:36.000000 iot-sdk-demo-0.0.1/src/systemService/mqttService.py
--rw-rw-rw-   0        0        0     3274 2023-07-24 08:17:36.000000 iot-sdk-demo-0.0.1/src/systemService/updateService.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:26:22.000000 iot-sdk-demo-0.0.1/src/utils/
--rw-rw-rw-   0        0        0      191 2023-07-20 08:17:40.000000 iot-sdk-demo-0.0.1/src/utils/TimeUtil.py
--rw-rw-rw-   0        0        0      247 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/utils/copyUtils.py
--rw-rw-rw-   0        0        0     1014 2023-07-26 10:19:45.000000 iot-sdk-demo-0.0.1/src/utils/fileUtils.py
--rw-rw-rw-   0        0        0      619 2023-07-24 07:47:42.000000 iot-sdk-demo-0.0.1/src/utils/logutil.py
--rw-rw-rw-   0        0        0     1304 2023-07-24 03:42:08.000000 iot-sdk-demo-0.0.1/src/utils/netUtils.py
--rw-rw-rw-   0        0        0      128 2023-07-24 08:13:35.000000 iot-sdk-demo-0.0.1/src/utils/pathUtils.py
--rw-rw-rw-   0        0        0      859 2023-07-24 07:35:22.000000 iot-sdk-demo-0.0.1/src/utils/tarGzUtils.py
--rw-rw-rw-   0        0        0     1441 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/utils/taskUtils.py
--rw-rw-rw-   0        0        0      955 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.1/src/utils/templateUtils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/
+-rw-rw-rw-   0        0        0       97 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/__init__.py
+-rw-rw-rw-   0        0        0     2315 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/config.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/
+-rw-rw-rw-   0        0        0      832 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/applicationContext.py
+-rw-rw-rw-   0        0        0     3294 2023-07-25 14:09:38.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/eventInvoker.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/exception/
+-rw-rw-rw-   0        0        0      176 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/exception/commonException.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/exception/sdkException.py
+-rw-rw-rw-   0        0        0     2327 2023-07-24 10:35:34.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/exception/serviceException.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/job/
+-rw-rw-rw-   0        0        0      905 2023-07-20 08:12:22.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/job/contextUpLoadJob.py
+-rw-rw-rw-   0        0        0      475 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/job/eventListenerJob.py
+-rw-rw-rw-   0        0        0      271 2023-07-21 08:49:20.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/job/mqttCheckMessageJob.py
+-rw-rw-rw-   0        0        0      256 2023-07-21 02:43:53.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/job/mqttHealthJob.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/
+-rw-rw-rw-   0        0        0     1350 2023-07-26 15:52:31.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py
+-rw-rw-rw-   0        0        0     1555 2023-07-25 10:09:39.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/proxyLoader.py
+-rw-rw-rw-   0        0        0     8251 2023-07-27 07:46:37.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/serversLoader.py
+-rw-rw-rw-   0        0        0      210 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/thingProxyFuncLoader.py
+-rw-rw-rw-   0        0        0     2303 2023-07-21 03:01:27.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/scheduleService.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/sender/
+-rw-rw-rw-   0        0        0       67 2023-07-27 02:11:41.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/sender/baseSender.py
+-rw-rw-rw-   0        0        0      369 2023-07-27 02:49:45.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/sender/hardwareUpLoadSender.py
+-rw-rw-rw-   0        0        0     2998 2023-07-24 08:14:24.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/serverInvoker.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/factory/
+-rw-rw-rw-   0        0        0      392 2023-06-15 10:40:11.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/factory/systemEventFactory.py
+-rw-rw-rw-   0        0        0      690 2023-06-27 09:17:54.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/factory/systemServiceFactory.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/model/
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/model/ujinja/
+-rw-rw-rw-   0        0        0     7700 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/model/ujinja/source.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/
+-rw-rw-rw-   0        0        0      746 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/capabilityBean.py
+-rw-rw-rw-   0        0        0      545 2023-06-12 06:53:14.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/eventBean.py
+-rw-rw-rw-   0        0        0      892 2023-07-20 10:25:24.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/serviceBean.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxy/
+-rw-rw-rw-   0        0        0      166 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxy/proxyBase.py
+-rw-rw-rw-   0        0        0      677 2023-07-24 10:01:52.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxy/pythonServiceProxy.py
+-rw-rw-rw-   0        0        0      570 2023-07-20 10:06:16.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxy/thingProxy.py
+-rw-rw-rw-   0        0        0     4213 2023-07-28 05:32:09.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxySDK.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/router/
+-rw-rw-rw-   0        0        0     1173 2023-07-25 09:57:46.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/router/httpRouter.py
+-rw-rw-rw-   0        0        0     2996 2023-07-24 07:55:12.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/router/mqttRouter.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/systemService/
+-rw-rw-rw-   0        0        0      153 2023-07-25 09:53:27.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/systemService/httpService.py
+-rw-rw-rw-   0        0        0     3176 2023-07-25 14:18:36.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/systemService/mqttService.py
+-rw-rw-rw-   0        0        0     3274 2023-07-24 08:17:36.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/systemService/updateService.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/
+-rw-rw-rw-   0        0        0      191 2023-07-20 08:17:40.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/TimeUtil.py
+-rw-rw-rw-   0        0        0      247 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/copyUtils.py
+-rw-rw-rw-   0        0        0     1014 2023-07-26 10:19:45.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/fileUtils.py
+-rw-rw-rw-   0        0        0      619 2023-07-24 07:47:42.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/logutil.py
+-rw-rw-rw-   0        0        0     1304 2023-07-24 03:42:08.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/netUtils.py
+-rw-rw-rw-   0        0        0      128 2023-07-24 08:13:35.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/pathUtils.py
+-rw-rw-rw-   0        0        0      859 2023-07-24 07:35:22.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/tarGzUtils.py
+-rw-rw-rw-   0        0        0     1441 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/taskUtils.py
+-rw-rw-rw-   0        0        0      955 2023-06-07 09:59:47.000000 iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/templateUtils.py
+-rw-rw-rw-   0        0        0    11357 2023-08-02 09:48:52.000000 iot-sdk-demo-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       68 2023-08-03 01:28:35.000000 iot-sdk-demo-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      604 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-08-02 10:00:57.000000 iot-sdk-demo-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/
+-rw-rw-rw-   0        0        0      604 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2254 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 12:13:14.000000 iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 01:30:19.000000 iot-sdk-demo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1214 2023-08-03 01:29:22.000000 iot-sdk-demo-0.0.2/setup.py
```

### Comparing `iot-sdk-demo-0.0.1/LICENSE` & `iot-sdk-demo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/PKG-INFO` & `iot-sdk-demo-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-sdk-demo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: HFC
 Author-email: 2898534520@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iot-sdk-demo-0.0.1/iot_sdk_demo.egg-info/PKG-INFO` & `iot-sdk-demo-0.0.2/iot_sdk_demo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-sdk-demo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: HFC
 Author-email: 2898534520@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iot-sdk-demo-0.0.1/setup.py` & `iot-sdk-demo-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="iot-sdk-demo", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",    #包版本号，便于维护版本
+    version="0.0.2",    #包版本号，便于维护版本
     author="HFC",    #作者，可以写自己的姓名
     author_email="2898534520@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),  # Make sure to include 'where' argument
```

### Comparing `iot-sdk-demo-0.0.1/src/config.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/config.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/applicationContext.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/applicationContext.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/eventInvoker.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/eventInvoker.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/exception/serviceException.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/exception/serviceException.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/job/contextUpLoadJob.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/job/contextUpLoadJob.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/loader/hardwareInfoLoader.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/loader/proxyLoader.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/proxyLoader.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/loader/serversLoader.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/loader/serversLoader.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/scheduleService.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/scheduleService.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/core/serverInvoker.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/core/serverInvoker.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/factory/systemServiceFactory.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/factory/systemServiceFactory.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/model/ujinja/source.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/model/ujinja/source.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/pojo/capabilityBean.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/capabilityBean.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/pojo/eventBean.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/eventBean.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/pojo/serviceBean.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/pojo/serviceBean.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/proxy/pythonServiceProxy.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxy/pythonServiceProxy.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/proxy/thingProxy.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxy/thingProxy.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/proxySDK.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/proxySDK.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/router/httpRouter.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/router/httpRouter.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/router/mqttRouter.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/router/mqttRouter.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/systemService/mqttService.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/systemService/mqttService.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/systemService/updateService.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/systemService/updateService.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/utils/fileUtils.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/fileUtils.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/utils/logutil.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/logutil.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/utils/netUtils.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/utils/tarGzUtils.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/tarGzUtils.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/utils/taskUtils.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/taskUtils.py`

 * *Files identical despite different names*

### Comparing `iot-sdk-demo-0.0.1/src/utils/templateUtils.py` & `iot-sdk-demo-0.0.2/IotPervasiveServiceSDK/utils/templateUtils.py`

 * *Files identical despite different names*

