# Comparing `tmp/selenium_driverless-1.2.4.tar.gz` & `tmp/selenium_driverless-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.2.4.tar", last modified: Wed Jul 26 16:36:10 2023, max compression
+gzip compressed data, was "selenium_driverless-1.2.5.tar", last modified: Thu Aug  3 07:26:26 2023, max compression
```

## Comparing `selenium_driverless-1.2.4.tar` & `selenium_driverless-1.2.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.796627 selenium_driverless-1.2.4/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.4/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3870 2023-07-26 16:36:10.796627 selenium_driverless-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2554 2023-07-26 16:22:00.000000 selenium_driverless-1.2.4/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.4/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-26 16:36:10.797628 selenium_driverless-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2122 2023-07-26 16:30:17.000000 selenium_driverless-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.683036 selenium_driverless-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.692944 selenium_driverless-1.2.4/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-26 16:35:45.000000 selenium_driverless-1.2.4/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.702585 selenium_driverless-1.2.4/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.4/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.709537 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/
--rw-rw-rw-   0        0        0     1176 2023-07-26 16:14:27.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/__init__.py
--rw-rw-rw-   0        0        0    16611 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/asyncio.py
--rw-rw-rw-   0        0        0     1361 2023-07-26 16:14:27.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/base.py
--rw-rw-rw-   0        0        0     7313 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/browser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.778508 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/
--rw-rw-rw-   0        0        0      798 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/__init__.py
--rw-rw-rw-   0        0        0    23896 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/accessibility.py
--rw-rw-rw-   0        0        0    11602 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/animation.py
--rw-rw-rw-   0        0        0    52280 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/audits.py
--rw-rw-rw-   0        0        0     6066 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/background_service.py
--rw-rw-rw-   0        0        0    21594 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/browser.py
--rw-rw-rw-   0        0        0     8567 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/cache_storage.py
--rw-rw-rw-   0        0        0     4435 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/cast.py
--rw-rw-rw-   0        0        0     2882 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/console.py
--rw-rw-rw-   0        0        0    66950 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/css.py
--rw-rw-rw-   0        0        0     4086 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/database.py
--rw-rw-rw-   0        0        0    52264 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/debugger.py
--rw-rw-rw-   0        0        0     3373 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/device_access.py
--rw-rw-rw-   0        0        0     1154 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/device_orientation.py
--rw-rw-rw-   0        0        0    63790 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom.py
--rw-rw-rw-   0        0        0     9800 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_debugger.py
--rw-rw-rw-   0        0        0    40830 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_snapshot.py
--rw-rw-rw-   0        0        0     5935 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_storage.py
--rw-rw-rw-   0        0        0    26766 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/emulation.py
--rw-rw-rw-   0        0        0     1230 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/event_breakpoints.py
--rw-rw-rw-   0        0        0     5466 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/fed_cm.py
--rw-rw-rw-   0        0        0    20431 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/fetch.py
--rw-rw-rw-   0        0        0     4985 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/headless_experimental.py
--rw-rw-rw-   0        0        0    14046 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/heap_profiler.py
--rw-rw-rw-   0        0        0    15583 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/indexed_db.py
--rw-rw-rw-   0        0        0    28365 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/input_.py
--rw-rw-rw-   0        0        0     1712 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/inspector.py
--rw-rw-rw-   0        0        0     2995 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/io.py
--rw-rw-rw-   0        0        0    15942 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/layer_tree.py
--rw-rw-rw-   0        0        0     5784 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/log.py
--rw-rw-rw-   0        0        0     7923 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/media.py
--rw-rw-rw-   0        0        0     7010 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/memory.py
--rw-rw-rw-   0        0        0   135424 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/network.py
--rw-rw-rw-   0        0        0    56704 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/overlay.py
--rw-rw-rw-   0        0        0   109903 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/page.py
--rw-rw-rw-   0        0        0     3080 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/performance.py
--rw-rw-rw-   0        0        0     7184 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/performance_timeline.py
--rw-rw-rw-   0        0        0    15687 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/preload.py
--rw-rw-rw-   0        0        0    13542 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/profiler.py
--rw-rw-rw-   0        0        0    61736 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/runtime.py
--rw-rw-rw-   0        0        0     1143 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/schema.py
--rw-rw-rw-   0        0        0    18042 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/security.py
--rw-rw-rw-   0        0        0    11603 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/service_worker.py
--rw-rw-rw-   0        0        0    36250 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/storage.py
--rw-rw-rw-   0        0        0    12090 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/system_info.py
--rw-rw-rw-   0        0        0    24638 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/target.py
--rw-rw-rw-   0        0        0     1526 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/tethering.py
--rw-rw-rw-   0        0        0    14160 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/tracing.py
--rw-rw-rw-   0        0        0      455 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/util.py
--rw-rw-rw-   0        0        0    18058 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/web_audio.py
--rw-rw-rw-   0        0        0    16287 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/web_authn.py
--rw-rw-rw-   0        0        0     2426 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/exceptions.py
--rw-rw-rw-   0        0        0    13427 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.782577 selenium_driverless-1.2.4/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.788628 selenium_driverless-1.2.4/src/selenium_driverless/sync/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/__init__.py
--rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/alert.py
--rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/executor.py
--rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/switch_to.py
--rw-rw-rw-   0        0        0     1374 2023-07-26 16:34:36.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/webdriver.py
--rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/webelement.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.791627 selenium_driverless-1.2.4/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.4/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.4/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.4/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.793627 selenium_driverless-1.2.4/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.4/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.4/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    45692 2023-07-26 15:56:46.000000 selenium_driverless-1.2.4/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.701063 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3870 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3718 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.794627 selenium_driverless-1.2.4/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.4/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.721497 selenium_driverless-1.2.5/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.5/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4408 2023-08-03 07:26:26.721497 selenium_driverless-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3092 2023-08-03 07:24:52.000000 selenium_driverless-1.2.5/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.5/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-08-03 07:26:26.723591 selenium_driverless-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2122 2023-07-26 16:30:17.000000 selenium_driverless-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.626665 selenium_driverless-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.634879 selenium_driverless-1.2.5/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-08-03 07:25:58.000000 selenium_driverless-1.2.5/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.640387 selenium_driverless-1.2.5/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.5/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.645388 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/
+-rw-rw-rw-   0        0        0     1176 2023-07-26 16:14:27.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/asyncio.py
+-rw-rw-rw-   0        0        0     1361 2023-07-26 16:14:27.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/base.py
+-rw-rw-rw-   0        0        0     7313 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/browser.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.698395 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/
+-rw-rw-rw-   0        0        0      798 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/__init__.py
+-rw-rw-rw-   0        0        0    23896 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11602 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/animation.py
+-rw-rw-rw-   0        0        0    52280 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/audits.py
+-rw-rw-rw-   0        0        0     6066 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/background_service.py
+-rw-rw-rw-   0        0        0    21594 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/browser.py
+-rw-rw-rw-   0        0        0     8567 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4435 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/cast.py
+-rw-rw-rw-   0        0        0     2882 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/console.py
+-rw-rw-rw-   0        0        0    66950 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/css.py
+-rw-rw-rw-   0        0        0     4086 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/database.py
+-rw-rw-rw-   0        0        0    52264 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3373 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1154 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    63790 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom.py
+-rw-rw-rw-   0        0        0     9800 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    40830 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5935 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    26766 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1230 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     5466 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    20431 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/fetch.py
+-rw-rw-rw-   0        0        0     4985 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14046 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    15583 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    28365 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/input_.py
+-rw-rw-rw-   0        0        0     1712 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/inspector.py
+-rw-rw-rw-   0        0        0     2995 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/io.py
+-rw-rw-rw-   0        0        0    15942 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     5784 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/log.py
+-rw-rw-rw-   0        0        0     7923 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/media.py
+-rw-rw-rw-   0        0        0     7010 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/memory.py
+-rw-rw-rw-   0        0        0   135424 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/network.py
+-rw-rw-rw-   0        0        0    56704 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/overlay.py
+-rw-rw-rw-   0        0        0   109903 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/page.py
+-rw-rw-rw-   0        0        0     3080 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/performance.py
+-rw-rw-rw-   0        0        0     7184 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    15687 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/preload.py
+-rw-rw-rw-   0        0        0    13542 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/profiler.py
+-rw-rw-rw-   0        0        0    61736 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1143 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/schema.py
+-rw-rw-rw-   0        0        0    18042 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/security.py
+-rw-rw-rw-   0        0        0    11603 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    36250 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/storage.py
+-rw-rw-rw-   0        0        0    12090 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/system_info.py
+-rw-rw-rw-   0        0        0    24638 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/target.py
+-rw-rw-rw-   0        0        0     1526 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14160 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/util.py
+-rw-rw-rw-   0        0        0    18058 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    16287 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/web_authn.py
+-rw-rw-rw-   0        0        0     2426 2023-07-26 16:21:09.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/exceptions.py
+-rw-rw-rw-   0        0        0    13427 2023-07-26 16:21:08.000000 selenium_driverless-1.2.5/src/selenium_driverless/pycdp/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.703495 selenium_driverless-1.2.5/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.5/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.5/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.5/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5933 2023-08-03 07:11:26.000000 selenium_driverless-1.2.5/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.711497 selenium_driverless-1.2.5/src/selenium_driverless/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.5/src/selenium_driverless/sync/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.5/src/selenium_driverless/sync/alert.py
+-rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.5/src/selenium_driverless/sync/executor.py
+-rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.5/src/selenium_driverless/sync/switch_to.py
+-rw-rw-rw-   0        0        0     1374 2023-07-26 16:34:36.000000 selenium_driverless-1.2.5/src/selenium_driverless/sync/webdriver.py
+-rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.5/src/selenium_driverless/sync/webelement.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.715498 selenium_driverless-1.2.5/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.5/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.5/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.5/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.718503 selenium_driverless-1.2.5/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.5/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.5/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    45694 2023-08-03 07:13:00.000000 selenium_driverless-1.2.5/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.640387 selenium_driverless-1.2.5/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     4408 2023-08-03 07:26:26.000000 selenium_driverless-1.2.5/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3718 2023-08-03 07:26:26.000000 selenium_driverless-1.2.5/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:26:26.000000 selenium_driverless-1.2.5/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-08-03 07:26:26.000000 selenium_driverless-1.2.5/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 07:26:26.000000 selenium_driverless-1.2.5/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.720497 selenium_driverless-1.2.5/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.5/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.2.4/LICENSE.md` & `selenium_driverless-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/PKG-INFO` & `selenium_driverless-1.2.5/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium_driverless
-Version: 1.2.4
+Name: selenium-driverless
+Version: 1.2.5
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -87,16 +87,23 @@
     source = driver.page_source
     print(title)
 ```
 
 ## Help
 
 Please feel free to open an issue or fork!
+note: please check the todo's below at first!
 
 ## Todo
+- implementations
+  - [ ] [`WebDriverWait`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7)
+  - [ ] [`EC`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7) (expected-conditions)
+  - [ ] [`driver.switch_to.frame`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7)
+  - [ ] [`ActionChains`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/5)
+      - [ ] [`TouchActions`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/5)
 - protocoll
   - [ ] add cdp event handler
 - [x] sync
   - [ ] move sync to threaded for allowing event_handlers
 - [ ] remove pycdp dependency -_-
 
 ## Deprecated
```

### Comparing `selenium_driverless-1.2.4/README.md` & `selenium_driverless-1.2.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -57,16 +57,23 @@
     source = driver.page_source
     print(title)
 ```
 
 ## Help
 
 Please feel free to open an issue or fork!
+note: please check the todo's below at first!
 
 ## Todo
+- implementations
+  - [ ] [`WebDriverWait`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7)
+  - [ ] [`EC`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7) (expected-conditions)
+  - [ ] [`driver.switch_to.frame`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7)
+  - [ ] [`ActionChains`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/5)
+      - [ ] [`TouchActions`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/5)
 - protocoll
   - [ ] add cdp event handler
 - [x] sync
   - [ ] move sync to threaded for allowing event_handlers
 - [ ] remove pycdp dependency -_-
 
 ## Deprecated
```

### Comparing `selenium_driverless-1.2.4/build_upload.md` & `selenium_driverless-1.2.5/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/setup.py` & `selenium_driverless-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/__init__.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/asyncio.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/asyncio.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/base.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/base.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/browser.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/browser.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/__init__.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/accessibility.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/animation.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/audits.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/background_service.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/browser.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/cache_storage.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/cast.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/console.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/console.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/css.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/css.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/database.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/database.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/debugger.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/device_access.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/device_orientation.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_debugger.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_snapshot.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_storage.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/emulation.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/event_breakpoints.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/fed_cm.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/fetch.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/headless_experimental.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/heap_profiler.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/indexed_db.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/input_.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/inspector.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/io.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/io.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/layer_tree.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/log.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/log.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/media.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/media.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/memory.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/network.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/network.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/overlay.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/page.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/page.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/performance.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/performance_timeline.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/preload.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/profiler.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/runtime.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/schema.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/security.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/security.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/service_worker.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/storage.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/system_info.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/target.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/tethering.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/tracing.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/web_audio.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/web_authn.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/exceptions.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/exceptions.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/pycdp/utils.py` & `selenium_driverless-1.2.5/src/selenium_driverless/pycdp/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.2.5/src/selenium_driverless/scripts/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.2.5/src/selenium_driverless/scripts/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.2.5/src/selenium_driverless/scripts/switch_to.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """Returns the element with focus, or BODY if nothing has focus.
 
         :Usage:
             ::
 
                 element = driver.switch_to.active_element
         """
-        raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
+        raise NotImplementedError('You might use driver.switch_to.target(driver.targets[0]["targetId"])')
 
     @property
     async def alert(self) -> Alert:
         """Switches focus to an alert on the page.
 
         :Usage:
             ::
@@ -69,15 +69,15 @@
         """Switch focus to the default frame.
 
         :Usage:
             ::
 
                 driver.switch_to.default_content()
         """
-        raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
+        raise NotImplementedError('You might use driver.switch_to.target(driver.targets[0]["targetId"])')
 
     async def frame(self, frame_reference: Union[str, int, WebElement]) -> None:
         """Switches focus to the specified frame, by index, name, or
         webelement.
 
         :Args:
          - frame_reference: The name of the window to switch to, an integer representing the index,
@@ -95,45 +95,49 @@
                 frame_reference = await self._driver.find_element(By.ID, frame_reference)
             except NoSuchElementException:
                 try:
                     frame_reference = await self._driver.find_element(By.NAME, frame_reference)
                 except NoSuchElementException:
                     raise NoSuchFrameException(frame_reference)
 
-        raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
+        raise NotImplementedError('You might use driver.switch_to.target(driver.targets[0]["targetId"])')
 
     async def target(self, target_id):
         from selenium_driverless.types import RemoteObject
+        from selenium_driverless.pycdp.cdp.target import TargetID
+
         self._driver.session.close()
         # noinspection PyProtectedMember
-        self._driver.session = await self._driver._conn.connect_session(target_id)
+        self._driver.session = await self._driver._conn.connect_session(TargetID(target_id))
         self._driver._global_this = await RemoteObject(driver=self, js="globalThis", check_existence=False)
         await self._driver.execute_cdp_cmd("Target.activateTarget",
-                                           {"targetId": await self._driver.current_window_handle})
+                                           {"targetId": self._driver.current_window_handle})
         return self._driver.session
 
     async def new_window(self, type_hint: Optional[str] = "tab", url="") -> None:
         """Switches to a new top-level browsing context.
 
         The type hint can be one of "tab" or "window". If not specified the
         browser will automatically select it.
 
         :Usage:
             ::
 
                 driver.switch_to.new_window('tab')
         """
-        new_window = False
         new_tab = False
         if type_hint == "window":
-            new_window = True
-        if type_hint == "tab":
-            new_window = True
+            new_tab = True
+        elif type_hint == "tab":
+            pass
+        else:
+            raise ValueError("type hint needs to be 'window' or 'tab'")
         args = {"url": url, "newWindow": new_tab, "forTab": new_tab}
-        target_id = await self._driver.execute_cdp_cmd("Target.createTarget", args)
+        target = await self._driver.execute_cdp_cmd("Target.createTarget", args)
+        target_id = target["targetId"]
         await self.target(target_id)
         return target_id
 
     async def parent_frame(self) -> None:
         """Switches focus to the parent context. If the current context is the
         top level browsing context, the context remains unchanged.
```

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/sync/alert.py` & `selenium_driverless-1.2.5/src/selenium_driverless/sync/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/sync/executor.py` & `selenium_driverless-1.2.5/src/selenium_driverless/sync/executor.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/sync/switch_to.py` & `selenium_driverless-1.2.5/src/selenium_driverless/sync/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/sync/webdriver.py` & `selenium_driverless-1.2.5/src/selenium_driverless/sync/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/sync/webelement.py` & `selenium_driverless-1.2.5/src/selenium_driverless/sync/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.2.5/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/types/by.py` & `selenium_driverless-1.2.5/src/selenium_driverless/types/by.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/types/webelement.py` & `selenium_driverless-1.2.5/src/selenium_driverless/types/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.2.5/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.2.5/src/selenium_driverless/webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
         :Usage:
             ::
 
                 driver.window_handles
         """
         tabs = []
         for target in await self.targets:
-            if target.type_ == "page":
+            if target["type"] == "page":
                 tabs.append(target.target_id)
         return tabs
 
     async def set_window_state(self, state):
         states = ["normal", "minimized", "maximized", "fullscreen"]
         if state not in states:
             raise ValueError(f"expected one of {states}, but got: {state}")
```

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium-driverless
-Version: 1.2.4
+Name: selenium_driverless
+Version: 1.2.5
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -87,16 +87,23 @@
     source = driver.page_source
     print(title)
 ```
 
 ## Help
 
 Please feel free to open an issue or fork!
+note: please check the todo's below at first!
 
 ## Todo
+- implementations
+  - [ ] [`WebDriverWait`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7)
+  - [ ] [`EC`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7) (expected-conditions)
+  - [ ] [`driver.switch_to.frame`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/7)
+  - [ ] [`ActionChains`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/5)
+      - [ ] [`TouchActions`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/5)
 - protocoll
   - [ ] add cdp event handler
 - [x] sync
   - [ ] move sync to threaded for allowing event_handlers
 - [ ] remove pycdp dependency -_-
 
 ## Deprecated
```

### Comparing `selenium_driverless-1.2.4/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.2.5/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.4/tests/test_driverless.py` & `selenium_driverless-1.2.5/tests/test_driverless.py`

 * *Files identical despite different names*

