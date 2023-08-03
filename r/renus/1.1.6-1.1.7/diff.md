# Comparing `tmp/renus-1.1.6.tar.gz` & `tmp/renus-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.6.tar", last modified: Mon Jul 31 07:19:29 2023, max compression
+gzip compressed data, was "renus-1.1.7.tar", last modified: Thu Aug  3 08:05:03 2023, max compression
```

## Comparing `renus-1.1.6.tar` & `renus-1.1.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.882069 renus-1.1.6/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.6/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-07-31 07:19:29.881067 renus-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.323069 renus-1.1.6/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.6/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.6/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.379068 renus-1.1.6/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.411086 renus-1.1.6/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1849 2023-07-31 07:12:37.000000 renus-1.1.6/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0      932 2023-07-31 07:19:07.000000 renus-1.1.6/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.6/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4262 2023-06-20 08:05:47.000000 renus-1.1.6/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.6/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.428084 renus-1.1.6/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.6/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.442083 renus-1.1.6/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.6/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.463089 renus-1.1.6/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-05-21 06:32:06.000000 renus-1.1.6/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.6/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.512090 renus-1.1.6/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     3760 2023-05-22 06:18:46.000000 renus-1.1.6/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     4148 2023-05-22 06:14:27.000000 renus-1.1.6/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.6/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.529089 renus-1.1.6/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.6/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.824083 renus-1.1.6/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.6/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/config.py
--rw-rw-rw-   0        0        0     2271 2023-06-20 12:25:48.000000 renus-1.1.6/renus/core/cprint.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.6/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.6/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.6/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.6/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/middleware.py
--rw-rw-rw-   0        0        0    15511 2023-07-05 07:28:40.000000 renus-1.1.6/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.6/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.6/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.6/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.6/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1514 2023-06-27 07:00:06.000000 renus-1.1.6/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.860072 renus-1.1.6/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.6/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.6/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.880087 renus-1.1.6/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.6/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.339084 renus-1.1.6/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 07:19:29.882069 renus-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-07-31 07:15:20.000000 renus-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.729343 renus-1.1.7/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-08-03 08:05:03.728344 renus-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.085894 renus-1.1.7/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.7/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.7/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.136597 renus-1.1.7/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.197783 renus-1.1.7/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1849 2023-07-31 07:12:37.000000 renus-1.1.7/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0      932 2023-07-31 07:19:07.000000 renus-1.1.7/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.7/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4262 2023-06-20 08:05:47.000000 renus-1.1.7/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.7/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.219792 renus-1.1.7/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.7/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.229029 renus-1.1.7/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.7/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.243497 renus-1.1.7/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-21 06:32:06.000000 renus-1.1.7/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.7/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.316146 renus-1.1.7/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     3760 2023-05-22 06:18:46.000000 renus-1.1.7/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     4148 2023-05-22 06:14:27.000000 renus-1.1.7/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.7/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.333542 renus-1.1.7/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.7/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.7/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.685549 renus-1.1.7/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.7/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/config.py
+-rw-rw-rw-   0        0        0     2271 2023-06-20 12:25:48.000000 renus-1.1.7/renus/core/cprint.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.7/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.7/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.7/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.7/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    15511 2023-07-05 07:28:40.000000 renus-1.1.7/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.7/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.7/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.7/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.7/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1514 2023-06-27 07:00:06.000000 renus-1.1.7/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.707522 renus-1.1.7/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0    11361 2023-08-03 07:58:34.000000 renus-1.1.7/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.7/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.7/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.727332 renus-1.1.7/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.7/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.7/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:05:03.100755 renus-1.1.7/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-08-03 08:05:02.000000 renus-1.1.7/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2023-08-03 08:05:02.000000 renus-1.1.7/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 08:05:02.000000 renus-1.1.7/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-03 08:05:02.000000 renus-1.1.7/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 08:05:03.729343 renus-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-08-03 08:04:14.000000 renus-1.1.7/setup.py
```

### Comparing `renus-1.1.6/LICENSE` & `renus-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/app.py` & `renus-1.1.7/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/app/controller.temp` & `renus-1.1.7/renus/commands/app/controller.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/app/model.temp` & `renus-1.1.7/renus/commands/app/model.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/app/route.temp` & `renus-1.1.7/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/app/run.py` & `renus-1.1.7/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/backup/run.py` & `renus-1.1.7/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/copy/run.py` & `renus-1.1.7/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/default/run.py` & `renus-1.1.7/renus/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/help.py` & `renus-1.1.7/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/install/build.py` & `renus-1.1.7/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/install/run.py` & `renus-1.1.7/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/install/service.py` & `renus-1.1.7/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/commands/permission/run.py` & `renus-1.1.7/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/cache.py` & `renus-1.1.7/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/concurrency.py` & `renus-1.1.7/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/cprint.py` & `renus-1.1.7/renus/core/cprint.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/crypt.py` & `renus-1.1.7/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/datastructures.py` & `renus-1.1.7/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/exception.py` & `renus-1.1.7/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/formparsers.py` & `renus-1.1.7/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/injection.py` & `renus-1.1.7/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/log.py` & `renus-1.1.7/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/model.py` & `renus-1.1.7/renus/core/model.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/request.py` & `renus-1.1.7/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/response.py` & `renus-1.1.7/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/routing.py` & `renus-1.1.7/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/schedule.py` & `renus-1.1.7/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/serialize.py` & `renus-1.1.7/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/status.py` & `renus-1.1.7/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/validation/rules.py` & `renus-1.1.7/renus/core/validation/rules.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import os
 import re
 
+
 class Default:
     def __init__(self, data):
         self.d = data
 
     def __call__(self, input):
         if input is None:
             return self.d
         return True
 
+
 class Convert:
     def __init__(self, func):
         self.f = func
 
     def __call__(self, input):
         return self.f(input)
 
@@ -355,7 +358,71 @@
         }).select('_id').count()
 
         if (self.count is not None and self.count == count) or (
                 self.minCount is not None and self.minCount <= count) or (
                 self.maxCount is not None and self.maxCount >= count):
             return True
         return ['exists_count_error', [input]]
+
+class FileSize:
+    def __init__(self, max_byte: int = 0, min_byte: int = 0, delete=True, replace:list=None, item_dict:str=None):
+        """
+        @param max_byte: maximum allowed Bytes
+        @param min_byte:minimum allowed Bytes
+        @param delete: delete file if not passed
+        @param replace: replace file path. default is [('storage/img/','storage/'),('storage/','storage/public/')]
+        @param item_dict: if file path in a dict. ex {url:'',meta:''} => item_dict='url'
+        """
+        if replace is None:
+            replace = [('storage/img/','storage/'),('storage/','storage/public/')]
+        self.delete = delete
+        self.maxByte = max_byte
+        self.minByte = min_byte
+        self.replace = replace
+        self.item_dict = item_dict
+
+    def __call__(self, input):
+        if input is None:
+            return True
+        t = type(input)
+        if t is str:
+            input = [input]
+        passed = True
+        if self.maxByte:
+            for item in input:
+                tt = type(item)
+                if tt is dict:
+                    link=item[self.item_dict]
+                else:
+                    link=item
+                for rep in self.replace:
+                    link=link.replace(rep[0],rep[1])
+                state = os.stat(link)
+                if state.st_size <= self.maxByte:
+                    continue
+                passed = ['max_file_size_error', [item,state.st_size,self.maxByte]]
+        if self.minByte:
+            for item in input:
+                tt = type(item)
+                if tt is dict:
+                    link = item[self.item_dict]
+                else:
+                    link = item
+                for rep in self.replace:
+                    link = link.replace(rep[0], rep[1])
+                state = os.stat(link)
+                if state.st_size >= self.minByte:
+                    continue
+                passed = ['min_file_size_error', [item,state.st_size,self.minByte]]
+        if passed is not True and self.delete:
+            for item in input:
+                tt = type(item)
+                if tt is dict:
+                    link = item[self.item_dict]
+                else:
+                    link = item
+                for rep in self.replace:
+                    link = link.replace(rep[0], rep[1])
+
+                os.remove(link)
+
+        return passed
```

### Comparing `renus-1.1.6/renus/core/validation/validate.py` & `renus-1.1.7/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/core/websockets.py` & `renus-1.1.7/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus/util/helper.py` & `renus-1.1.7/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.6/renus.egg-info/SOURCES.txt` & `renus-1.1.7/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

