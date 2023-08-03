# Comparing `tmp/iotPervasiveServiceSDK-0.0.2.tar.gz` & `tmp/iotPervasiveServiceSDK-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iotPervasiveServiceSDK-0.0.2.tar", last modified: Thu Aug  3 07:12:44 2023, max compression
+gzip compressed data, was "dist\iotPervasiveServiceSDK-0.0.3.tar", last modified: Thu Aug  3 07:26:14 2023, max compression
```

## Comparing `iotPervasiveServiceSDK-0.0.2.tar` & `iotPervasiveServiceSDK-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/
--rw-rw-rw-   0        0        0    11357 2023-08-02 09:48:52.000000 iotPervasiveServiceSDK-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       68 2023-08-03 06:38:15.000000 iotPervasiveServiceSDK-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      564 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-08-02 10:00:57.000000 iotPervasiveServiceSDK-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/
--rw-rw-rw-   0        0        0      123 2023-08-03 06:44:05.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/__init__.py
--rw-rw-rw-   0        0        0     2315 2023-07-27 07:46:37.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/config.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/
--rw-rw-rw-   0        0        0      832 2023-07-27 07:46:37.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/applicationContext.py
--rw-rw-rw-   0        0        0     3294 2023-07-25 14:09:38.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/eventInvoker.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/exception/
--rw-rw-rw-   0        0        0      176 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/exception/commonException.py
--rw-rw-rw-   0        0        0        0 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/exception/sdkException.py
--rw-rw-rw-   0        0        0     2327 2023-07-24 10:35:34.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/exception/serviceException.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/job/
--rw-rw-rw-   0        0        0      905 2023-07-20 08:12:22.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py
--rw-rw-rw-   0        0        0      475 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/job/eventListenerJob.py
--rw-rw-rw-   0        0        0      271 2023-07-21 08:49:20.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/job/mqttCheckMessageJob.py
--rw-rw-rw-   0        0        0      256 2023-07-21 02:43:53.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/job/mqttHealthJob.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/
--rw-rw-rw-   0        0        0     1350 2023-07-26 15:52:31.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py
--rw-rw-rw-   0        0        0     1555 2023-07-25 10:09:39.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/proxyLoader.py
--rw-rw-rw-   0        0        0     8251 2023-07-27 07:46:37.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/serversLoader.py
--rw-rw-rw-   0        0        0      210 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/thingProxyFuncLoader.py
--rw-rw-rw-   0        0        0     2303 2023-07-21 03:01:27.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/scheduleService.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/sender/
--rw-rw-rw-   0        0        0       67 2023-07-27 02:11:41.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/sender/baseSender.py
--rw-rw-rw-   0        0        0      369 2023-07-27 02:49:45.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/sender/hardwareUpLoadSender.py
--rw-rw-rw-   0        0        0        0 2023-08-03 03:28:07.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/serverInvoker.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/factory/
--rw-rw-rw-   0        0        0      392 2023-06-15 10:40:11.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/factory/systemEventFactory.py
--rw-rw-rw-   0        0        0      690 2023-06-27 09:17:54.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/factory/systemServiceFactory.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/model/
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/model/ujinja/
--rw-rw-rw-   0        0        0     7700 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/model/ujinja/source.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/
--rw-rw-rw-   0        0        0      746 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/capabilityBean.py
--rw-rw-rw-   0        0        0      545 2023-06-12 06:53:14.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/eventBean.py
--rw-rw-rw-   0        0        0      892 2023-07-20 10:25:24.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/serviceBean.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxy/
--rw-rw-rw-   0        0        0      166 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxy/proxyBase.py
--rw-rw-rw-   0        0        0      675 2023-08-03 06:39:25.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py
--rw-rw-rw-   0        0        0      568 2023-08-03 06:40:16.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxy/thingProxy.py
--rw-rw-rw-   0        0        0     4208 2023-08-03 02:50:57.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxySDK.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/router/
--rw-rw-rw-   0        0        0     1173 2023-07-25 09:57:46.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/router/httpRouter.py
--rw-rw-rw-   0        0        0     2996 2023-07-24 07:55:12.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/router/mqttRouter.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/systemService/
--rw-rw-rw-   0        0        0      153 2023-07-25 09:53:27.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/systemService/httpService.py
--rw-rw-rw-   0        0        0     3176 2023-07-25 14:18:36.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/systemService/mqttService.py
--rw-rw-rw-   0        0        0     3274 2023-07-24 08:17:36.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/systemService/updateService.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/
--rw-rw-rw-   0        0        0      191 2023-07-20 08:17:40.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/TimeUtil.py
--rw-rw-rw-   0        0        0      247 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/copyUtils.py
--rw-rw-rw-   0        0        0     1014 2023-07-26 10:19:45.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/fileUtils.py
--rw-rw-rw-   0        0        0      619 2023-07-24 07:47:42.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/logutil.py
--rw-rw-rw-   0        0        0     1304 2023-07-24 03:42:08.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/netUtils.py
--rw-rw-rw-   0        0        0      128 2023-07-24 08:13:35.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/pathUtils.py
--rw-rw-rw-   0        0        0      859 2023-07-24 07:35:22.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/tarGzUtils.py
--rw-rw-rw-   0        0        0     1441 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/taskUtils.py
--rw-rw-rw-   0        0        0      955 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/templateUtils.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/
--rw-rw-rw-   0        0        0      564 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       87 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-08-03 06:42:32.000000 iotPervasiveServiceSDK-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/
+-rw-rw-rw-   0        0        0    11357 2023-08-02 09:48:52.000000 iotPervasiveServiceSDK-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       68 2023-08-03 06:38:15.000000 iotPervasiveServiceSDK-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      564 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-08-02 10:00:57.000000 iotPervasiveServiceSDK-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/
+-rw-rw-rw-   0        0        0      123 2023-08-03 06:44:05.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/__init__.py
+-rw-rw-rw-   0        0        0     2315 2023-07-27 07:46:37.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/config.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/
+-rw-rw-rw-   0        0        0      832 2023-07-27 07:46:37.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/applicationContext.py
+-rw-rw-rw-   0        0        0     3294 2023-07-25 14:09:38.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/eventInvoker.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/exception/
+-rw-rw-rw-   0        0        0      176 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/exception/commonException.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/exception/sdkException.py
+-rw-rw-rw-   0        0        0     2327 2023-07-24 10:35:34.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/exception/serviceException.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/job/
+-rw-rw-rw-   0        0        0      905 2023-07-20 08:12:22.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py
+-rw-rw-rw-   0        0        0      475 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/job/eventListenerJob.py
+-rw-rw-rw-   0        0        0      271 2023-07-21 08:49:20.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/job/mqttCheckMessageJob.py
+-rw-rw-rw-   0        0        0      256 2023-07-21 02:43:53.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/job/mqttHealthJob.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/
+-rw-rw-rw-   0        0        0     1350 2023-07-26 15:52:31.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py
+-rw-rw-rw-   0        0        0     1555 2023-07-25 10:09:39.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/proxyLoader.py
+-rw-rw-rw-   0        0        0     8251 2023-07-27 07:46:37.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/serversLoader.py
+-rw-rw-rw-   0        0        0      210 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/thingProxyFuncLoader.py
+-rw-rw-rw-   0        0        0     2303 2023-07-21 03:01:27.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/scheduleService.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/sender/
+-rw-rw-rw-   0        0        0       67 2023-07-27 02:11:41.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/sender/baseSender.py
+-rw-rw-rw-   0        0        0      369 2023-07-27 02:49:45.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/sender/hardwareUpLoadSender.py
+-rw-rw-rw-   0        0        0     2998 2023-08-03 07:25:01.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/serverInvoker.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/factory/
+-rw-rw-rw-   0        0        0      392 2023-06-15 10:40:11.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/factory/systemEventFactory.py
+-rw-rw-rw-   0        0        0      690 2023-06-27 09:17:54.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/factory/systemServiceFactory.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/model/
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/model/ujinja/
+-rw-rw-rw-   0        0        0     7700 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/model/ujinja/source.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/
+-rw-rw-rw-   0        0        0      746 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/capabilityBean.py
+-rw-rw-rw-   0        0        0      545 2023-06-12 06:53:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/eventBean.py
+-rw-rw-rw-   0        0        0      892 2023-07-20 10:25:24.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/serviceBean.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxy/
+-rw-rw-rw-   0        0        0      166 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxy/proxyBase.py
+-rw-rw-rw-   0        0        0      675 2023-08-03 06:39:25.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py
+-rw-rw-rw-   0        0        0      568 2023-08-03 06:40:16.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxy/thingProxy.py
+-rw-rw-rw-   0        0        0     4208 2023-08-03 02:50:57.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxySDK.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/router/
+-rw-rw-rw-   0        0        0     1173 2023-07-25 09:57:46.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/router/httpRouter.py
+-rw-rw-rw-   0        0        0     2996 2023-07-24 07:55:12.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/router/mqttRouter.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/systemService/
+-rw-rw-rw-   0        0        0      153 2023-07-25 09:53:27.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/systemService/httpService.py
+-rw-rw-rw-   0        0        0     3176 2023-07-25 14:18:36.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/systemService/mqttService.py
+-rw-rw-rw-   0        0        0     3274 2023-07-24 08:17:36.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/systemService/updateService.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/
+-rw-rw-rw-   0        0        0      191 2023-07-20 08:17:40.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/TimeUtil.py
+-rw-rw-rw-   0        0        0      247 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/copyUtils.py
+-rw-rw-rw-   0        0        0     1014 2023-07-26 10:19:45.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/fileUtils.py
+-rw-rw-rw-   0        0        0      619 2023-07-24 07:47:42.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/logutil.py
+-rw-rw-rw-   0        0        0     1304 2023-07-24 03:42:08.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/netUtils.py
+-rw-rw-rw-   0        0        0      128 2023-07-24 08:13:35.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/pathUtils.py
+-rw-rw-rw-   0        0        0      859 2023-07-24 07:35:22.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/tarGzUtils.py
+-rw-rw-rw-   0        0        0     1441 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/taskUtils.py
+-rw-rw-rw-   0        0        0      955 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/templateUtils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 07:12:44.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       87 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:26:14.000000 iotPervasiveServiceSDK-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2023-08-03 07:25:50.000000 iotPervasiveServiceSDK-0.0.3/setup.py
```

### Comparing `iotPervasiveServiceSDK-0.0.2/LICENSE` & `iotPervasiveServiceSDK-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/PKG-INFO` & `iotPervasiveServiceSDK-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotPervasiveServiceSDK
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author: HFC
 Author-email: 2898534520@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/config.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/config.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/applicationContext.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/applicationContext.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/eventInvoker.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/eventInvoker.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/exception/serviceException.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/exception/serviceException.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/proxyLoader.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/proxyLoader.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/loader/serversLoader.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/loader/serversLoader.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/core/scheduleService.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/core/scheduleService.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/factory/systemServiceFactory.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/factory/systemServiceFactory.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/model/ujinja/source.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/model/ujinja/source.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/capabilityBean.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/capabilityBean.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/eventBean.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/eventBean.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/pojo/serviceBean.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/pojo/serviceBean.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxy/thingProxy.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxy/thingProxy.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/proxySDK.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/proxySDK.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/router/httpRouter.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/router/httpRouter.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/router/mqttRouter.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/router/mqttRouter.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/systemService/mqttService.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/systemService/mqttService.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/systemService/updateService.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/systemService/updateService.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/fileUtils.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/fileUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/logutil.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/logutil.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/netUtils.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/tarGzUtils.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/tarGzUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/taskUtils.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/taskUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK/utils/templateUtils.py` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK/utils/templateUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/PKG-INFO` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotPervasiveServiceSDK
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author: HFC
 Author-email: 2898534520@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `iotPervasiveServiceSDK-0.0.2/iotPervasiveServiceSDK.egg-info/SOURCES.txt` & `iotPervasiveServiceSDK-0.0.3/iotPervasiveServiceSDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.2/setup.py` & `iotPervasiveServiceSDK-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="iotPervasiveServiceSDK", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",    #包版本号，便于维护版本
+    version="0.0.3",    #包版本号，便于维护版本
     author="HFC",    #作者，可以写自己的姓名
     author_email="2898534520@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # Make sure to include 'where' argument
     zip_safe=False,  # Disable zip-safe mode for easier debugging
```

