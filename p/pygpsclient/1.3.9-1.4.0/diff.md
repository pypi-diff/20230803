# Comparing `tmp/PyGPSClient-1.3.9.tar.gz` & `tmp/pygpsclient-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGPSClient-1.3.9.tar", last modified: Fri Sep  2 09:18:28 2022, max compression
+gzip compressed data, was "pygpsclient-1.4.0.tar", last modified: Thu Aug  3 08:03:51 2023, max compression
```

## Comparing `PyGPSClient-1.3.9.tar` & `pygpsclient-1.4.0.tar`

### file list

```diff
@@ -1,73 +1,96 @@
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.797773 PyGPSClient-1.3.9/
--rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/LICENSE
--rw-r--r--   0 stevensmith   (501) staff       (20)       98 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/MANIFEST.in
--rw-r--r--   0 stevensmith   (501) staff       (20)    30893 2022-09-02 09:18:28.797420 PyGPSClient-1.3.9/PKG-INFO
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.694334 PyGPSClient-1.3.9/PyGPSClient.egg-info/
--rw-r--r--   0 stevensmith   (501) staff       (20)    30893 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/PKG-INFO
--rw-r--r--   0 stevensmith   (501) staff       (20)     2314 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/SOURCES.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/dependency_links.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       58 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/entry_points.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       64 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/requires.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       12 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/top_level.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)    29718 2022-08-29 10:34:28.000000 PyGPSClient-1.3.9/README.md
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.724242 PyGPSClient-1.3.9/pygpsclient/
--rw-r--r--   0 stevensmith   (501) staff       (20)      222 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/__init__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      392 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/__main__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      166 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/pygpsclient/_version.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5285 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/about_dialog.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    22362 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/app.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    19942 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/banner_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     6060 2022-07-05 16:13:18.000000 PyGPSClient-1.3.9/pygpsclient/console_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9581 2022-08-06 16:57:08.000000 PyGPSClient-1.3.9/pygpsclient/file_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7940 2022-08-24 17:39:34.000000 PyGPSClient-1.3.9/pygpsclient/globals.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     1431 2022-04-22 07:36:03.000000 PyGPSClient-1.3.9/pygpsclient/gnss_status.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5727 2022-04-29 08:34:24.000000 PyGPSClient-1.3.9/pygpsclient/graphview_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    12956 2022-08-24 17:39:34.000000 PyGPSClient-1.3.9/pygpsclient/helpers.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7732 2022-04-29 08:34:29.000000 PyGPSClient-1.3.9/pygpsclient/map_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     3434 2022-04-29 08:34:32.000000 PyGPSClient-1.3.9/pygpsclient/menu_bar.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    10960 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/nmea_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    24328 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/pygpsclient/ntrip_client_dialog.py
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.796265 PyGPSClient-1.3.9/pygpsclient/resources/
--rw-r--r--   0 stevensmith   (501) staff       (20)     6148 2022-07-06 11:18:44.000000 PyGPSClient-1.3.9/pygpsclient/resources/.DS_Store
--rw-r--r--   0 stevensmith   (501) staff       (20)     9309 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/resources/binary-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      575 2022-08-24 17:39:34.000000 PyGPSClient-1.3.9/pygpsclient/resources/clear-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     9507 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/ethernet-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      946 2022-04-11 07:18:02.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-antenna-6-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      269 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-arrow-12-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      209 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-arrow-80-16.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      844 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-check-mark-8-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      395 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-door-6-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     1037 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-gear-2-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      439 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-location-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     1724 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-location-27-32.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      328 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-media-control-48-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      125 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-media-control-50-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)    10472 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-noclient-10-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     3856 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-notransmit-10-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      442 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-refresh-6-16.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      875 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-time-6-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      860 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-transmit-10-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      276 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-triangle-1-16.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      466 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-warning-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     4286 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/pygpsclient.ico
--rw-r--r--   0 stevensmith   (501) staff       (20)     5424 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/usbport-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)   327167 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/world.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     1315 2022-04-29 08:34:46.000000 PyGPSClient-1.3.9/pygpsclient/rtcm3_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    14416 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/serialconfig_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    30284 2022-08-08 08:16:28.000000 PyGPSClient-1.3.9/pygpsclient/settings_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5341 2022-05-29 08:04:41.000000 PyGPSClient-1.3.9/pygpsclient/skyview_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     4965 2022-05-08 17:41:44.000000 PyGPSClient-1.3.9/pygpsclient/socketconfig_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     3258 2022-05-08 17:41:44.000000 PyGPSClient-1.3.9/pygpsclient/status_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9561 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/stream_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5004 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/pygpsclient/strings.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    16002 2022-08-29 06:50:48.000000 PyGPSClient-1.3.9/pygpsclient/ubx_cfgval_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    10211 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_config_dialog.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    17058 2022-08-27 14:49:03.000000 PyGPSClient-1.3.9/pygpsclient/ubx_dynamic_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9315 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7700 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_info_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9722 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_msgrate_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9353 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_port_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    18202 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_preset_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7262 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_solrate_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-09-02 09:18:28.797893 PyGPSClient-1.3.9/setup.cfg
--rw-r--r--   0 stevensmith   (501) staff       (20)     2634 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-08-03 08:03:51.641400 pygpsclient-1.4.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)      102 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    51220 2023-08-03 08:03:51.641207 pygpsclient-1.4.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    48221 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     3199 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-08-03 08:03:51.641490 pygpsclient-1.4.0/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-08-03 08:03:51.617812 pygpsclient-1.4.0/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-08-03 08:03:51.631230 pygpsclient-1.4.0/src/pygpsclient/
+-rw-r--r--   0 steve      (501) staff       (20)      222 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     2195 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/__main__.py
+-rw-r--r--   0 steve      (501) staff       (20)      166 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     6790 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/about_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    29445 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/app.py
+-rw-r--r--   0 steve      (501) staff       (20)    21437 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/banner_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     6348 2023-07-20 07:55:54.000000 pygpsclient-1.4.0/src/pygpsclient/console_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    12654 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/file_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)    10682 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/globals.py
+-rw-r--r--   0 steve      (501) staff       (20)     1680 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/gnss_status.py
+-rw-r--r--   0 steve      (501) staff       (20)    20790 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/gpx_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)     6193 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/graphview_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    19608 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/helpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    12223 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/map_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3304 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/mapquest.py
+-rw-r--r--   0 steve      (501) staff       (20)     3200 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/menu_bar.py
+-rw-r--r--   0 steve      (501) staff       (20)    13010 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/nmea_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)    25059 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/ntrip_client_dialog.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-08-03 08:03:51.640326 pygpsclient-1.4.0/src/pygpsclient/resources/
+-rw-r--r--   0 steve      (501) staff       (20)     9309 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/binary-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      576 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/blank-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      575 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/clear-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     9507 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/ethernet-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      714 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-antenna-3-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      808 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-antenna-4-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      269 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-arrow-12-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-arrow-80-16.png
+-rw-r--r--   0 steve      (501) staff       (20)      844 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-check-mark-8-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      395 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-door-6-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      305 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-folder-18-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     1037 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-gear-2-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      439 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-location-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     1724 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-location-27-32.png
+-rw-r--r--   0 steve      (501) staff       (20)      331 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-media-control-48-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      125 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-media-control-50-24.png
+-rw-r--r--   0 steve      (501) staff       (20)    10472 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-noclient-10-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     8807 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-record-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      442 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-refresh-6-16.png
+-rw-r--r--   0 steve      (501) staff       (20)      495 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-refresh-lined-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      205 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-save-14-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      119 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-stop-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-time-6-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      860 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-transmit-10-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      326 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-trash-can-filled-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      276 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-triangle-1-16.png
+-rw-r--r--   0 steve      (501) staff       (20)     7751 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-undo-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      466 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-warning-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     4286 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/pygpsclient.ico
+-rw-r--r--   0 steve      (501) staff       (20)     5424 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/usbport-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)   327167 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/resources/world.png
+-rw-r--r--   0 steve      (501) staff       (20)     1226 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/rtcm3_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)     7645 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/scatter_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    15545 2023-07-21 09:05:31.000000 pygpsclient-1.4.0/src/pygpsclient/serialconfig_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    25477 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/serverconfig_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    24294 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/settings_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     5363 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/skyview_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     8085 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/socketconfig_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     9083 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/spartn_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    17677 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/spartn_gnss_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3948 2023-08-02 19:03:37.000000 pygpsclient-1.4.0/src/pygpsclient/spartn_json_config.py
+-rw-r--r--   0 steve      (501) staff       (20)    21798 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/spartn_lband_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    14869 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/spartn_mqtt_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    14885 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/spectrum_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3340 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/status_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     8342 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/stream_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)     6659 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/strings.py
+-rw-r--r--   0 steve      (501) staff       (20)    13034 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/sysmon_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    14971 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_cfgval_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    11121 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_config_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    16847 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_dynamic_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    15641 2023-08-03 08:03:02.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)     7149 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_info_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     9424 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_msgrate_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     9102 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_port_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    17698 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_preset_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    15236 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_recorder_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     6955 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/ubx_solrate_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     2591 2023-07-18 14:52:16.000000 pygpsclient-1.4.0/src/pygpsclient/widgets.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-08-03 08:03:51.632343 pygpsclient-1.4.0/src/pygpsclient.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    51220 2023-08-03 08:03:51.000000 pygpsclient-1.4.0/src/pygpsclient.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     3413 2023-08-03 08:03:51.000000 pygpsclient-1.4.0/src/pygpsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-08-03 08:03:51.000000 pygpsclient-1.4.0/src/pygpsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       58 2023-08-03 08:03:51.000000 pygpsclient-1.4.0/src/pygpsclient.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-08-03 08:03:51.000000 pygpsclient-1.4.0/src/pygpsclient.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       12 2023-08-03 08:03:51.000000 pygpsclient-1.4.0/src/pygpsclient.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-08-03 08:03:51.640667 pygpsclient-1.4.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)    11124 2023-07-25 08:23:38.000000 pygpsclient-1.4.0/tests/test_static.py
```

### Comparing `PyGPSClient-1.3.9/LICENSE` & `pygpsclient-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/about_dialog.py` & `pygpsclient-1.4.0/src/pygpsclient/about_dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,33 +4,39 @@
 Created on 20 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
-from tkinter import Toplevel, Label, Button
 from platform import python_version
+from subprocess import CalledProcessError, run
+from sys import platform
+from tkinter import Button, Label, Toplevel
 from webbrowser import open_new_tab
-from PIL import ImageTk, Image
+
+from PIL import Image, ImageTk
 from pygnssutils import version as PGVERSION
-from pyubx2 import version as UBXVERSION
 from pynmeagps import version as NMEAVERSION
 from pyrtcm import version as RTCMVERSION
+from pyspartn import version as SPARTNVERSION
+from pyubx2 import version as UBXVERSION
+
+from pygpsclient._version import __version__ as VERSION
+from pygpsclient.globals import DLGTABOUT, GITHUB_URL, ICON_APP, ICON_EXIT
 from pygpsclient.helpers import check_latest
-from pygpsclient.globals import ICON_APP, ICON_EXIT, GITHUB_URL
 from pygpsclient.strings import ABOUTTXT, COPYRIGHTTXT, DLGABOUT
-from pygpsclient._version import __version__ as VERSION
 
 LIBVERSIONS = {
     "PyGPSClient": VERSION,
     "pygnssutils": PGVERSION,
     "pyubx2": UBXVERSION,
     "pynmeagps": NMEAVERSION,
     "pyrtcm": RTCMVERSION,
+    "pyspartn": SPARTNVERSION,
 }
 
 
 class AboutDialog:
     """
     About dialog box class
     """
@@ -39,23 +45,24 @@
         """
         Initialise Toplevel dialog
 
         :param Frame app: reference to main tkinter application
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self._dialog = Toplevel()
         self._dialog.title = DLGABOUT
         self._dialog.geometry(
             f"+{self.__master.winfo_rootx() + 50}+{self.__master.winfo_rooty() + 50}"
         )
         self._dialog.attributes("-topmost", "true")
         self._img_icon = ImageTk.PhotoImage(Image.open(ICON_APP))
         self._img_exit = ImageTk.PhotoImage(Image.open(ICON_EXIT))
+        self._updates = []
 
         self._body()
         self._do_layout()
         self._attach_events()
 
     def _body(self):
         """
@@ -74,15 +81,15 @@
         )
         self._lbl_python_version = Label(
             self._dialog,
             text=f"Python: {python_version()}",
             font=self.__app.font_sm,
         )
         self._lbl_lib_versions = []
-        for (nam, ver) in LIBVERSIONS.items():
+        for nam, ver in LIBVERSIONS.items():
             self._lbl_lib_versions.append(
                 Label(
                     self._dialog,
                     text=f"{nam}: {ver}",
                     font=self.__app.font_sm,
                 )
             )
@@ -92,15 +99,14 @@
             width=12,
             font=self.__app.font_sm,
             cursor="hand2",
         )
         self._lbl_copyright = Label(
             self._dialog,
             text=COPYRIGHTTXT,
-            fg="blue",
             font=self.__app.font_sm,
             cursor="hand2",
         )
         self._btn_ok = Button(
             self._dialog,
             image=self._img_exit,
             width=55,
@@ -138,26 +144,67 @@
         self._btn_ok.focus_set()
 
     def _ok_press(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Handle OK button press.
         """
 
+        self.__app.stop_dialog(DLGTABOUT)
         self._dialog.destroy()
 
     def _check_for_update(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Check for updates.
         """
 
+        self._updates = []
         for i, (nam, current) in enumerate(LIBVERSIONS.items()):
             latest = check_latest(nam)
             txt = f"{nam}: {current}"
             if latest == current:
                 col = "green"
             elif latest == "N/A":
                 txt += ". Info not available!"
                 col = "red"
             else:
+                self._updates.append(nam)
                 txt += f". Latest version is {latest}"
                 col = "red"
             self._lbl_lib_versions[i].config(text=txt, fg=col)
+
+        if len(self._updates) > 0:
+            self._btn_checkupdate.config(text="UPDATE", fg="blue")
+            self._btn_checkupdate.bind("<Button>", self._do_update)
+
+    def _do_update(self, *args, **kwargs):  # pylint: disable=unused-argument
+        """
+        Run python update.
+        """
+
+        self._btn_checkupdate.config(text="UPDATING...", fg="blue")
+        self._dialog.update_idletasks()
+        pyc = "python" if platform == "win32" else "python3"
+        cmd = [
+            pyc,
+            "-m",
+            "pip",
+            "install",
+            "--upgrade",
+            "--user",
+            "--force-reinstall",
+        ]
+        for pkg in self._updates:
+            cmd.append(pkg)
+
+        try:
+            run(
+                cmd,
+                check=True,
+                capture_output=True,
+            )
+        except CalledProcessError:
+            self._btn_checkupdate.config(text="UPDATE FAILED", fg="red")
+            self._btn_checkupdate.bind("<Button>", self._check_for_update)
+            return
+
+        self._btn_checkupdate.config(text="RESTART APP", fg="green")
+        self._btn_checkupdate.bind("<Button>", self.__app.on_exit)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/app.py` & `pygpsclient-1.4.0/src/pygpsclient/serverconfig_frame.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,696 +1,772 @@
 """
-PyGPSClient - Main tkinter application class.
+serverconfig_frame.py
 
-Hosts the various GUI widgets and update routines.
-Holds a GNSSStatus object containing the latest
-GNSS receiver readings.
+Socket Server / NTRIP caster configuration panel Frame class.
+Supports two modes of operation - Socket Server and NTRIP Caster.
 
-Created on 12 Sep 2020
+If running in NTRIP Caster mode, two base station modes are available -
+Survey-In and Fixed. The panel provides methods to configure RTK-compatible
+receiver (e.g. ZED-F9P) to operate in either of these base station modes.
+
+Application icons from https://iconmonstr.com/license/.
+
+Created on 23 Jul 2023
 
 :author: semuadmin
-:copyright: SEMU Consulting © 2020
+:copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
+# pylint: disable=unused-argument
 
-# import logging
-from threading import Thread
-from queue import Queue, Empty
-from datetime import datetime, timedelta
-from tkinter import Frame, N, S, E, W, PhotoImage, font
-from serial import SerialException, SerialTimeoutException
-from pyubx2 import (
-    protocol,
-    NMEA_PROTOCOL,
-    UBX_PROTOCOL,
-    RTCM3_PROTOCOL,
-)
-from pygnssutils import GNSSNTRIPClient
-from pygnssutils.socket_server import SocketServer, ClientHandler
-from pygpsclient.strings import (
-    TITLE,
-    MENUHIDESE,
-    MENUSHOWSE,
-    MENUHIDESB,
-    MENUSHOWSB,
-    MENUHIDECON,
-    MENUSHOWCON,
-    MENUHIDEMAP,
-    MENUSHOWMAP,
-    MENUHIDESATS,
-    MENUSHOWSATS,
-    INTROTXTNOPORTS,
-    NOTCONN,
+from tkinter import (
+    DISABLED,
+    NORMAL,
+    Button,
+    Checkbutton,
+    DoubleVar,
+    E,
+    Entry,
+    Frame,
+    IntVar,
+    Label,
+    Spinbox,
+    StringVar,
+    W,
 )
-from pygpsclient.gnss_status import GNSSStatus
-from pygpsclient.about_dialog import AboutDialog
-from pygpsclient.banner_frame import BannerFrame
-from pygpsclient.console_frame import ConsoleFrame
-from pygpsclient.file_handler import FileHandler
+from tkinter.ttk import Progressbar
+
+from PIL import Image, ImageTk
+from pyubx2 import UBXMessage, llh2ecef
+
 from pygpsclient.globals import (
-    ICON_APP,
-    CONNECTED,
     DISCONNECTED,
-    NOPORTS,
-    GUI_UPDATE_INTERVAL,
-    GPX_TRACK_INTERVAL,
-    SOCKSERVER_MAX_CLIENTS,
-    SOCKSERVER_HOST,
+    ICON_CONTRACT,
+    ICON_EXPAND,
+    READONLY,
+    SOCK_NTRIP,
+    SOCKMODES,
+    SOCKSERVER_NTRIP_PORT,
+    SOCKSERVER_PORT,
+)
+from pygpsclient.helpers import (
+    MAXPORT,
+    VALFLOAT,
+    VALINT,
+    VALNONBLANK,
+    val2sphp,
+    valid_entry,
+)
+from pygpsclient.strings import (
+    LBLACCURACY,
+    LBLCONFIGBASE,
+    LBLDURATIONS,
+    LBLSERVERHOST,
+    LBLSERVERMODE,
+    LBLSERVERPORT,
+    LBLSOCKSERVE,
 )
-from pygpsclient.graphview_frame import GraphviewFrame
-from pygpsclient.map_frame import MapviewFrame
-from pygpsclient.menu_bar import MenuBar
-from pygpsclient.stream_handler import StreamHandler
-from pygpsclient.settings_frame import SettingsFrame
-from pygpsclient.skyview_frame import SkyviewFrame
-from pygpsclient.status_frame import StatusFrame
-from pygpsclient.ubx_config_dialog import UBXConfigDialog
-from pygpsclient.ntrip_client_dialog import NTRIPConfigDialog
-from pygpsclient.nmea_handler import NMEAHandler
-from pygpsclient.ubx_handler import UBXHandler
-
 
-# LOGGING = logging.INFO
+TMODE_DISABLED = 0
+TMODE_SVIN = 1
+TMODE_FIXED = 2
+ECEF = 0
+LLH = 1
+BASE_SVIN = "SURVEY IN"
+BASE_FIXED = "FIXED"
+BASE_DISABLED = "DISABLED"
+POS_LLH = "LLH"
+POS_ECEF = "ECEF"
+BASEMODES = (BASE_SVIN, BASE_DISABLED, BASE_FIXED)
+POSMODES = (POS_LLH, POS_ECEF)
+ACCURACIES = (
+    10,
+    5,
+    3,
+    2,
+    1,
+    10000,
+    5000,
+    3000,
+    2000,
+    1000,
+    500,
+    300,
+    200,
+    100,
+    50,
+    30,
+    20,
+)
+DURATIONS = (60, 1200, 600, 300, 240, 180, 120, 90)
+MAXSVIN = 15
 
 
-class App(Frame):  # pylint: disable=too-many-ancestors
+class ServerConfigFrame(Frame):
     """
-    Main PyGPSClient GUI Application Class
+    Server configuration frame class.
     """
 
-    def __init__(self, master, *args, **kwargs):
+    def __init__(self, app, container, *args, **kwargs):
         """
-        Set up main application and add frames
+        Constructor.
 
-        :param tkinter.Tk master: reference to Tk root
+        :param Frame app: reference to main tkinter application
+        :param tkinter.Frame container: reference to container frame
         :param args: optional args to pass to Frame parent class
-        :param kwargs: optional kwargs to pass to Frame parent class
+        :param kwargs: optional kwargs for value ranges, or to pass to Frame parent class
         """
 
-        # logging.basicConfig(
-        #     format="%(asctime)-15s [%(levelname)s] %(funcName)s: %(message)s",
-        #     level=LOGGING,
-        # )
-
-        self.__master = master
-
-        Frame.__init__(self, self.__master, *args, **kwargs)
-
-        self.__master.protocol("WM_DELETE_WINDOW", self.on_exit)
-        self.__master.title(TITLE)
-        self.__master.iconphoto(True, PhotoImage(file=ICON_APP))
-        self.gnss_status = GNSSStatus()  # holds latest GNSS readings
-        self._last_gui_update = datetime.now()
-        self._last_track_update = datetime.now()
-
-        # Set initial widget visibility
-        self._show_settings = True
-        self._show_ubxconfig = False
-        self._show_status = True
-        self._show_console = True
-        self._show_map = True
-        self._show_sats = True
-
-        # Instantiate protocol handler classes
-        self.msgqueue = Queue()
-        self.ntripqueue = Queue()
-        self.socketqueue = Queue()
-        self.file_handler = FileHandler(self)
-        self.stream_handler = StreamHandler(self)
-        self.nmea_handler = NMEAHandler(self)
-        self.ubx_handler = UBXHandler(self)
-        self._conn_status = DISCONNECTED
-        self.ntrip_handler = GNSSNTRIPClient(self, verbosity=0)
-        self.dlg_ubxconfig = None
-        self.dlg_ntripconfig = None
-        self._ubx_config_thread = None
-        self._ntrip_config_thread = None
-        self._socket_thread = None
-        self._socket_server = None
-
-        # Load web map api key if there is one
-        self.api_key = self.file_handler.load_apikey()
+        Frame.__init__(self, container, *args, **kwargs)
 
-        # Load console color tags from file
-        self.colortags = self.file_handler.load_colortags()
+        self.__app = app
+        self._show_advanced = False
+        self._socket_serve = IntVar()
+        self.sock_port = StringVar()
+        self.sock_host = StringVar()
+        self.sock_mode = StringVar()
+        self._sock_clients = StringVar()
+        self._set_basemode = IntVar()
+        self._base_mode = StringVar()
+        self._acclimit = IntVar()
+        self._duration = IntVar()
+        self._pos_mode = StringVar()
+        self._fixedlat = DoubleVar()
+        self._fixedlon = DoubleVar()
+        self._fixedalt = DoubleVar()
+        self._disable_nmea = IntVar()
+        self._img_expand = ImageTk.PhotoImage(Image.open(ICON_EXPAND))
+        self._img_contract = ImageTk.PhotoImage(Image.open(ICON_CONTRACT))
 
         self._body()
         self._do_layout()
         self._attach_events()
-
-        # Initialise widgets
-        self.frm_satview.init_sats()
-        self.frm_graphview.init_graph()
-        self.frm_banner.update_conn_status(DISCONNECTED)
+        self.reset()
 
     def _body(self):
         """
-        Set up frame and widgets
+        Set up widgets.
         """
 
-        # these grid weights are what gives the grid its
-        # 'pack to window size' behaviour
-        self.__master.grid_columnconfigure(0, weight=1)
-        self.__master.grid_columnconfigure(1, weight=2)
-        self.__master.grid_columnconfigure(2, weight=2)
-        self.__master.grid_rowconfigure(0, weight=0)
-        self.__master.grid_rowconfigure(1, weight=2)
-        self.__master.grid_rowconfigure(2, weight=1)
-        self._set_default_fonts()
-
-        self.menu = MenuBar(self)
-        self.frm_status = StatusFrame(self, borderwidth=2, relief="groove")
-        self.frm_banner = BannerFrame(self, borderwidth=2, relief="groove")
-        self.frm_settings = SettingsFrame(self, borderwidth=2, relief="groove")
-        self.frm_console = ConsoleFrame(self, borderwidth=2, relief="groove")
-        self.frm_mapview = MapviewFrame(self, borderwidth=2, relief="groove")
-        self.frm_satview = SkyviewFrame(self, borderwidth=2, relief="groove")
-        self.frm_graphview = GraphviewFrame(self, borderwidth=2, relief="groove")
-
-        self.__master.config(menu=self.menu)
+        self._frm_basic = Frame(self)
+        self._chk_socketserve = Checkbutton(
+            self._frm_basic,
+            text=LBLSOCKSERVE,
+            variable=self._socket_serve,
+            state=DISABLED,
+        )
+        self._lbl_sockmode = Label(
+            self._frm_basic,
+            text=LBLSERVERMODE,
+        )
+        self._spn_sockmode = Spinbox(
+            self._frm_basic,
+            values=SOCKMODES,
+            width=14,
+            state=READONLY,
+            wrap=True,
+            textvariable=self.sock_mode,
+        )
+        self._lbl_sockhost = Label(
+            self._frm_basic,
+            text=LBLSERVERHOST,
+        )
+        self._ent_sockhost = Entry(
+            self._frm_basic,
+            textvariable=self.sock_host,
+            relief="sunken",
+            width=12,
+        )
+        self._lbl_sockport = Label(
+            self._frm_basic,
+            text=LBLSERVERPORT,
+        )
+        self._ent_sockport = Entry(
+            self._frm_basic,
+            textvariable=self.sock_port,
+            relief="sunken",
+            width=6,
+        )
+        self._lbl_clients = Label(self._frm_basic, text="Clients")
+        self._lbl_sockclients = Label(
+            self._frm_basic,
+            textvariable=self._sock_clients,
+        )
+        self._btn_toggle = Button(
+            self._frm_basic,
+            command=self._on_toggle_advanced,
+            image=self._img_expand,
+            width=28,
+            height=22,
+        )
+        self._frm_advanced = Frame(self)
+        self._chk_set_basemode = Checkbutton(
+            self._frm_advanced,
+            text=LBLCONFIGBASE,
+            variable=self._set_basemode,
+        )
+        self._spn_basemode = Spinbox(
+            self._frm_advanced,
+            values=BASEMODES,
+            width=10,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._base_mode,
+        )
+        self._lbl_acclimit = Label(
+            self._frm_advanced,
+            text=LBLACCURACY,
+        )
+        self._spn_acclimit = Spinbox(
+            self._frm_advanced,
+            values=ACCURACIES,
+            width=5,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._acclimit,
+        )
+        self._lbl_duration = Label(
+            self._frm_advanced,
+            text=LBLDURATIONS,
+        )
+        self._chk_disablenmea = Checkbutton(
+            self._frm_advanced,
+            text="Disable NMEA",
+            variable=self._disable_nmea,
+        )
+        self._spn_duration = Spinbox(
+            self._frm_advanced,
+            values=DURATIONS,
+            width=5,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._duration,
+        )
+        self._lbl_elapsed = Label(
+            self._frm_advanced,
+            text="",
+        )
+        self._pgb_elapsed = Progressbar(
+            self._frm_advanced,
+            orient="horizontal",
+            mode="determinate",
+            length=150,
+        )
+        self._spn_posmode = Spinbox(
+            self._frm_advanced,
+            values=POSMODES,
+            width=6,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._pos_mode,
+        )
+        self._lbl_fixedlat = Label(
+            self._frm_advanced,
+            text="Lat",
+        )
+        self._ent_fixedlat = Entry(
+            self._frm_advanced,
+            textvariable=self._fixedlat,
+            relief="sunken",
+            width=18,
+        )
+        self._lbl_fixedlon = Label(
+            self._frm_advanced,
+            text="Lon",
+        )
+        self._ent_fixedlon = Entry(
+            self._frm_advanced,
+            textvariable=self._fixedlon,
+            relief="sunken",
+            width=18,
+        )
+        self._lbl_fixedalt = Label(
+            self._frm_advanced,
+            text="Height (m)",
+        )
+        self._ent_fixedalt = Entry(
+            self._frm_advanced,
+            textvariable=self._fixedalt,
+            relief="sunken",
+            width=18,
+        )
 
     def _do_layout(self):
         """
-        Arrange widgets in main application frame
+        Layout widgets.
         """
 
-        self.frm_banner.grid(
-            column=0, row=0, columnspan=5, padx=2, pady=2, sticky=(N, S, E, W)
+        self._frm_basic.grid(column=0, row=0, columnspan=5, sticky=(W, E))
+        self._chk_socketserve.grid(
+            column=0, row=0, columnspan=2, rowspan=2, padx=2, pady=1, sticky=W
         )
-        self._grid_console()
-        self._grid_sats()
-        self._grid_map()
-        self._grid_status()
-        self._grid_settings()
-
-        if self.frm_settings.serial_settings().status == NOPORTS:
-            self.set_status(INTROTXTNOPORTS, "red")
+        self._lbl_sockmode.grid(column=2, row=0, padx=2, pady=1, sticky=E)
+        self._spn_sockmode.grid(column=3, row=0, padx=2, pady=1, sticky=W)
+        self._lbl_sockhost.grid(column=2, row=1, padx=2, pady=1, sticky=E)
+        self._ent_sockhost.grid(column=3, row=1, padx=2, pady=1, sticky=W)
+        self._lbl_sockport.grid(column=2, row=2, padx=2, pady=1, sticky=E)
+        self._ent_sockport.grid(column=3, row=2, padx=2, pady=1, sticky=W)
+        self._lbl_clients.grid(column=0, row=2, padx=2, pady=1, sticky=E)
+        self._lbl_sockclients.grid(column=1, row=2, padx=2, pady=1, sticky=W)
+        self._btn_toggle.grid_forget()
+        self._frm_advanced.grid_forget()
+        self._chk_set_basemode.grid(
+            column=0, row=0, columnspan=2, padx=2, pady=2, sticky=W
+        )
+        self._spn_basemode.grid(column=2, row=0, columnspan=2, padx=2, pady=2, sticky=W)
 
     def _attach_events(self):
         """
-        Bind events to main application
+        Bind events to variables.
         """
 
-        self.__master.bind("<<stream_read>>", self.on_read)
-        self.__master.bind("<<gnss_eof>>", self.stream_handler.on_eof)
-        self.__master.bind("<<ntrip_read>>", self.on_ntrip_read)
-        self.__master.bind_all("<Control-q>", self.on_exit)
+        tracemode = ("write", "unset")
+        self._socket_serve.trace_add(tracemode, self._on_socket_serve)
+        self.sock_mode.trace_add(tracemode, self._on_sockmode)
+        self._base_mode.trace_add(tracemode, self._on_basemode)
+        self._pos_mode.trace_add(tracemode, self._on_posmode)
 
-    def _set_default_fonts(self):
+    def reset(self):
         """
-        Set default fonts for entire application
+        Reset settings to defaults.
         """
-        # pylint: disable=attribute-defined-outside-init
 
-        self.font_vsm = font.Font(size=8)
-        self.font_sm = font.Font(size=10)
-        self.font_md = font.Font(size=12)
-        self.font_md2 = font.Font(size=14)
-        self.font_lg = font.Font(size=18)
+        self._base_mode.set(BASE_SVIN)
+        self._pos_mode.set(POS_LLH)
+        self._disable_nmea.set(1)
+        self.clients = 0
 
-    def toggle_settings(self):
+    def set_status(self, status: int):
         """
-        Toggle Settings Frame on or off
-        """
-
-        self._show_settings = not self._show_settings
-        self._grid_settings()
+        Set connection status, which determines whether controls
+        are enabled or not: 0=DISCONNECTED, 1=CONNECTED
 
-    def _grid_settings(self):
-        """
-        Set grid position of Settings Frame
+        :param int status: status (0,1)
         """
 
-        if self._show_settings:
-            self.frm_settings.grid(
-                column=4, row=1, rowspan=2, padx=2, pady=2, sticky=(N, W, E)
-            )
-            self.menu.view_menu.entryconfig(0, label=MENUHIDESE)
-        else:
-            self.frm_settings.grid_forget()
-            self.menu.view_menu.entryconfig(0, label=MENUSHOWSE)
-
-    def toggle_status(self):
-        """
-        Toggle Status Bar on or off
-        """
-
-        self._show_status = not self._show_status
-        self._grid_status()
-
-    def _grid_status(self):
-        """
-        Position Status Bar in grid
-        """
-
-        if self._show_status:
-            self.frm_status.grid(
-                column=0, row=3, columnspan=5, padx=2, pady=2, sticky=(W, E)
-            )
-            self.menu.view_menu.entryconfig(1, label=MENUHIDESB)
+        if status == DISCONNECTED:
+            self._chk_socketserve.configure(state=DISABLED)
+            self._socket_serve.set(0)
+            self.clients = 0
         else:
-            self.frm_status.grid_forget()
-            self.menu.view_menu.entryconfig(1, label=MENUSHOWSB)
+            self._chk_socketserve.configure(state=NORMAL)
 
-    def toggle_console(self):
+    def _on_socket_serve(self, var, index, mode):
         """
-        Toggle Console frame on or off
+        Action when socket_serve variable is updated.
+        Start or stop socket server.
         """
 
-        self._show_console = not self._show_console
-        self._grid_console()
-        self._grid_sats()
-        self._grid_map()
-
-    def _grid_console(self):
-        """
-        Position Console Frame in grid
-        """
-
-        if self._show_console:
-            self.frm_console.grid(
-                column=0, row=1, columnspan=4, padx=2, pady=2, sticky=(N, S, E, W)
-            )
-            self.menu.view_menu.entryconfig(2, label=MENUHIDECON)
-        else:
-            self.frm_console.grid_forget()
-            self.menu.view_menu.entryconfig(2, label=MENUSHOWCON)
+        if self._socket_serve.get():
+            # validate entries
+            valid = True
+            valid = valid & valid_entry(self._ent_sockhost, VALNONBLANK)
+            valid = valid & valid_entry(self._ent_sockport, VALINT, 1, MAXPORT)
+            valid = valid & valid_entry(self._ent_fixedlat, VALFLOAT)
+            valid = valid & valid_entry(self._ent_fixedlon, VALFLOAT)
+            valid = valid & valid_entry(self._ent_fixedalt, VALFLOAT)
+            if valid:
+                self.__app.set_status("", "blue")
+            else:
+                self.__app.set_status("ERROR - invalid entry", "red")
+                self._socket_serve.set(0)
+                return
+            # start server
+            self.__app.start_sockserver_thread()
+            self.__app.stream_handler.sock_serve = True
+        else:  # stop server
+            self.__app.stop_sockserver_thread()
+            self.__app.stream_handler.sock_serve = False
+            self.clients = 0
+
+        # set visibility of various fields depending on server status
+        for wid in (
+            self._ent_sockhost,
+            self._ent_sockport,
+            self._spn_sockmode,
+            self._chk_set_basemode,
+            self._spn_basemode,
+            self._lbl_acclimit,
+            self._spn_acclimit,
+            self._lbl_duration,
+            self._spn_duration,
+            self._chk_disablenmea,
+            self._spn_posmode,
+            self._lbl_fixedlat,
+            self._ent_fixedlat,
+            self._lbl_fixedlon,
+            self._ent_fixedlon,
+            self._lbl_fixedalt,
+            self._ent_fixedalt,
+        ):
+            if self._socket_serve.get():
+                state = DISABLED
+            else:
+                state = READONLY if isinstance(wid, Spinbox) else NORMAL
+            wid.config(state=state)
+        self._lbl_elapsed.config(text="")
+
+        # configure receiver as base station if in NTRIP Caster mode
+        # and 'Configure Base' option is checked.
+        if (
+            self._socket_serve.get()
+            and self.sock_mode.get() == SOCK_NTRIP
+            and self._set_basemode.get()
+        ):
+            self._config_rcvr()
 
-    def toggle_sats(self):
+    def _on_toggle_advanced(self):
         """
-        Toggle Satview and Graphview frames on or off
+        Toggle advanced socket settings panel on or off
+        if server mode is "NTRIP Caster".
         """
 
-        self._show_sats = not self._show_sats
-        self._grid_sats()
-        self._grid_map()
+        if self.sock_mode.get() != SOCK_NTRIP:
+            return
+        self._show_advanced = not self._show_advanced
+        self._set_advanced()
 
-    def _grid_sats(self):
+    def _set_advanced(self):
         """
-        Position Satview and Graphview Frames in grid
+        Set visibility of advanced socket server settings panel.
         """
 
-        if self._show_sats:
-            self.frm_satview.grid(column=0, row=2, padx=2, pady=2, sticky=(N, S, E, W))
-            self.frm_graphview.grid(
-                column=1, row=2, padx=2, pady=2, sticky=(N, S, E, W)
-            )
-            self.menu.view_menu.entryconfig(4, label=MENUHIDESATS)
+        if self._show_advanced:
+            self._frm_advanced.grid(column=0, row=1, columnspan=5, sticky=(W, E))
+            self._btn_toggle.config(image=self._img_contract)
         else:
-            self.frm_satview.grid_forget()
-            self.frm_graphview.grid_forget()
-            self.menu.view_menu.entryconfig(4, label=MENUSHOWSATS)
+            self._frm_advanced.grid_forget()
+            self._btn_toggle.config(image=self._img_expand)
 
-    def toggle_map(self):
+    def _on_sockmode(self, var, index, mode):
         """
-        Toggle Map Frame on or off
+        Action when sock_mode variable is updated.
+        Set default port and expand button depending on socket server mode.
         """
 
-        self._show_map = not self._show_map
-        self._grid_map()
-
-    def _grid_map(self):
-        """
-        Position Map Frame in grid
-        """
-
-        if self._show_map:
-            self.frm_mapview.grid(column=2, row=2, padx=2, pady=2, sticky=(N, S, E, W))
-            self.menu.view_menu.entryconfig(3, label=MENUHIDEMAP)
+        if self.sock_mode.get() == SOCK_NTRIP:
+            self.sock_port.set(SOCKSERVER_NTRIP_PORT)
+            self._btn_toggle.grid(column=4, row=0, sticky=E)
+            self._show_advanced = True
         else:
-            self.frm_mapview.grid_forget()
-            self.menu.view_menu.entryconfig(3, label=MENUSHOWMAP)
-
-    @property
-    def conn_status(self) -> int:
-        """
-        Getter for connection status.
-
-        :param int status: connection status e.g. 1 = CONNECTED
-        """
-
-        return self._conn_status
-
-    @conn_status.setter
-    def conn_status(self, status: int):
-        """
-        Setter for connection status.
-
-        :param int status: connection status e.g. 1 = CONNECTED
-        """
-
-        self._conn_status = status
-        self.frm_banner.update_conn_status(status)
-        self.frm_settings.enable_controls(status)
-        if status == DISCONNECTED:
-            self.set_connection(NOTCONN, "red")
-            self.set_status("", "blue")
-
-    def set_connection(self, message, color="blue"):
-        """
-        Sets connection description in status bar.
-
-        :param str message: message to be displayed in connection label
-        :param str color: rgb color string
-
-        """
-
-        self.frm_status.set_connection(message, color)
-
-    def set_status(self, message, color="black"):
-        """
-        Sets text of status bar
-
-        :param str message: message to be displayed in status label
-        :param str color: rgb color string
-
-        """
-
-        self.frm_status.set_status(message, color)
-
-    def about(self):
-        """
-        Open About dialog
-        """
-
-        AboutDialog(self)
-
-    def ubxconfig(self):
-        """
-        Start UBX Config dialog thread
-        """
-
-        if self._ubx_config_thread is None:
-            self._ubx_config_thread = Thread(
-                target=self._ubxconfig_thread, daemon=False
+            self.sock_port.set(SOCKSERVER_PORT)
+            self._btn_toggle.grid_forget()
+            self._show_advanced = False
+        self._set_advanced()
+
+    def _on_basemode(self, var, index, mode):
+        """
+        Action when base_mode is updated.
+        Set field visibility depending on base mode.
+        """
+
+        if self._base_mode.get() == BASE_SVIN:
+            self._lbl_acclimit.grid(column=0, row=1, padx=2, pady=1, sticky=E)
+            self._spn_acclimit.grid(column=1, row=1, padx=2, pady=1, sticky=W)
+            self._chk_disablenmea.grid(column=2, row=1, padx=2, pady=1, sticky=W)
+            self._lbl_duration.grid(column=0, row=2, padx=2, pady=1, sticky=E)
+            self._spn_duration.grid(column=1, row=2, padx=2, pady=1, sticky=W)
+            self._lbl_elapsed.grid(
+                column=2, row=2, columnspan=2, padx=2, pady=1, sticky=W
             )
-            self._ubx_config_thread.start()
-
-    def _ubxconfig_thread(self):
-        """
-        THREADED PROCESS UBX Configuration Dialog
-        """
-
-        self.dlg_ubxconfig = UBXConfigDialog(self)
-
-    def stop_ubxconfig_thread(self):
-        """
-        Stop UBX Configuration dialog thread.
-        """
-
-        if self._ubx_config_thread is not None:
-            self._ubx_config_thread = None
-            self.dlg_ubxconfig = None
-
-    def ntripconfig(self):
-        """
-        Start NTRIP Config dialog thread
-        """
-
-        if self._ntrip_config_thread is None:
-            self._ntrip_config_thread = Thread(
-                target=self._ntripconfig_thread, daemon=False
+            self._pgb_elapsed.grid_forget()
+            self._spn_posmode.grid_forget()
+            self._lbl_fixedlat.grid_forget()
+            self._ent_fixedlat.grid_forget()
+            self._lbl_fixedlon.grid_forget()
+            self._ent_fixedlon.grid_forget()
+            self._lbl_fixedalt.grid_forget()
+            self._ent_fixedalt.grid_forget()
+        elif self._base_mode.get() == BASE_FIXED:
+            self._lbl_acclimit.grid(column=0, row=1, padx=2, pady=1, sticky=E)
+            self._spn_acclimit.grid(column=1, row=1, padx=2, pady=1, sticky=W)
+            self._chk_disablenmea.grid(column=2, row=1, padx=2, pady=1, sticky=W)
+            self._spn_posmode.grid(column=0, row=2, rowspan=3, padx=2, pady=1, sticky=E)
+            self._lbl_fixedlat.grid(column=1, row=2, padx=2, pady=1, sticky=E)
+            self._ent_fixedlat.grid(
+                column=2, row=2, columnspan=3, padx=2, pady=1, sticky=W
             )
-            self._ntrip_config_thread.start()
-
-    def _ntripconfig_thread(self):
-        """
-        THREADED PROCESS NTRIP Configuration Dialog
-        """
-
-        self.dlg_ntripconfig = NTRIPConfigDialog(self)
-
-    def stop_ntripconfig_thread(self):
-        """
-        Stop UBX Configuration dialog thread.
-        """
-
-        if self._ntrip_config_thread is not None:
-            self._ntrip_config_thread = None
-            self.dlg_ntripconfig = None
-
-    def start_sockserver_thread(self):
-        """
-        Start socket server thread.
-        """
-
-        port = self.frm_settings.server_port
-        ntripmode = self.frm_settings.server_mode
-        self._socket_thread = Thread(
-            target=self._sockserver_thread,
-            args=(
-                ntripmode,
-                SOCKSERVER_HOST,
-                port,
-                SOCKSERVER_MAX_CLIENTS,
-                self.socketqueue,
-            ),
-            daemon=True,
+            self._lbl_fixedlon.grid(column=1, row=3, padx=2, pady=1, sticky=E)
+            self._ent_fixedlon.grid(
+                column=2, row=3, columnspan=3, padx=2, pady=1, sticky=W
+            )
+            self._lbl_fixedalt.grid(column=1, row=4, padx=2, pady=1, sticky=E)
+            self._ent_fixedalt.grid(
+                column=2, row=4, columnspan=3, padx=2, pady=1, sticky=W
+            )
+            self._lbl_duration.grid_forget()
+            self._spn_duration.grid_forget()
+            self._pgb_elapsed.grid_forget()
+            self._lbl_elapsed.grid_forget()
+            self._set_coords(self._pos_mode.get())
+        else:  # Disabled
+            self._chk_disablenmea.grid(column=0, row=1, padx=2, pady=1, sticky=W)
+            self._lbl_acclimit.grid_forget()
+            self._spn_acclimit.grid_forget()
+            self._spn_posmode.grid_forget()
+            self._lbl_fixedlat.grid_forget()
+            self._ent_fixedlat.grid_forget()
+            self._lbl_fixedlon.grid_forget()
+            self._ent_fixedlon.grid_forget()
+            self._lbl_fixedalt.grid_forget()
+            self._ent_fixedalt.grid_forget()
+            self._lbl_duration.grid_forget()
+            self._spn_duration.grid_forget()
+            self._pgb_elapsed.grid_forget()
+            self._lbl_elapsed.grid_forget()
+
+    def _on_posmode(self, var, index, mode):
+        """
+        Action when pos_mode variable is updated.
+        Set fixed reference labels depending on position mode (ECEF or LLH)
+        """
+
+        lbls = (
+            ("Lat", "Lon", "Height (m)")
+            if self._pos_mode.get() == POS_LLH
+            else ("X (m)", "Y (m)", "Z (m)")
         )
-        self._socket_thread.start()
-        self.frm_banner.update_transmit_status(0)
+        self._lbl_fixedlat.config(text=lbls[0])
+        self._lbl_fixedlon.config(text=lbls[1])
+        self._lbl_fixedalt.config(text=lbls[2])
+        self._set_coords(self._pos_mode.get())
 
-    def stop_sockserver_thread(self):
-        """
-        Stop socket server thread.
+    def _set_coords(self, posmode: str):
         """
+        Set current coordinates in LLH or ECEF format.
 
-        self.frm_banner.update_transmit_status(-1)
-        if self._socket_server is not None:
-            self._socket_server.shutdown()
-
-    def _sockserver_thread(
-        self, ntripmode: int, host: str, port: int, maxclients: int, socketqueue: Queue
-    ):
-        """
-        THREADED
-        Socket Server thread.
-
-        :param int ntripmode: 0 = open socket server, 1 = NTRIP server
-        :param str host: socket host name (0.0.0.0)
-        :param int port: socket port (50010)
-        :param int maxclients: max num of clients (5)
-        :param Queue socketqueue: socket server read queue
+        :param str posmode: position mode (LLH or ECEF)
         """
 
+        _, lat, lon, alt, _ = self.__app.get_coordinates()
         try:
-            with SocketServer(
-                self, ntripmode, maxclients, socketqueue, (host, port), ClientHandler
-            ) as self._socket_server:
-                self._socket_server.serve_forever()
-        except OSError as err:
-            self.set_status(f"Error starting socket server {err}", "red")
-
-    def update_clients(self, clients: int):
-        """
-        Update number of connected clients in settings panel.
-
-        :param int clients: no of connected clients
-        """
-
-        self.frm_settings.clients = clients
+            if posmode == POS_ECEF:
+                lat, lon, alt = llh2ecef(lat, lon, alt)
+        except TypeError:  # e.g. no NMEA fix
+            lat = lon = alt = 0.0
+        self._fixedlat.set(lat)
+        self._fixedlon.set(lon)
+        self._fixedalt.set(alt)
 
     @property
-    def appmaster(self) -> object:
+    def clients(self) -> int:
         """
-        Getter for application master (Tk).
+        Getter for number of socket clients.
         """
 
-        return self.__master
+        return self._sock_clients.get()
 
-    def get_master(self):
+    @clients.setter
+    def clients(self, clients: int):
         """
-        Getter for application master (Tk)
-
-        :return: reference to application master (Tk)
-        """
-
-        return self.__master
+        Setter for number of socket clients.
 
-    def on_exit(self, *args, **kwargs):  # pylint: disable=unused-argument
-        """
-        Kill any running processes and quit application
+        :param int clients: no of clients connected
         """
 
-        self.file_handler.close_logfile()
-        self.file_handler.close_trackfile()
-        self.stop_sockserver_thread()
-        self.stream_handler.stop_read_thread()
-        self.stop_ubxconfig_thread()
-        self.stop_ntripconfig_thread()
-        self.__master.destroy()
+        self._sock_clients.set(clients)
+        if self._socket_serve.get() == 1:
+            self.__app.frm_banner.update_transmit_status(clients)
 
-    def on_read(self, event):  # pylint: disable=unused-argument
+    def _config_rcvr(self):
         """
-        EVENT TRIGGERED
-        Action on <<stream_read>> event - read any data on the message queue.
-
-        :param event event: read event
+        Configure receiver as Base Station if in NTRIP caster mode.
         """
 
-        try:
-            raw_data, parsed_data = self.msgqueue.get(False)
-            if raw_data is not None and parsed_data is not None:
-                self.process_data(raw_data, parsed_data)
-        except Empty:
-            pass
-
-    def on_ntrip_read(self, event):  # pylint: disable=unused-argument
-        """
-        EVENT TRIGGERED
-        Action on <<ntrip_read>> event - read data from NTRIP queue.
-        If it's RTCM3 data, send to connected receiver and display on console.
-        If it's NMEA, just display on console.
-
-        :param event event: read event
-        """
+        # set base station timing mode
+        if self._base_mode.get() == BASE_SVIN:
+            msg = self._config_svin(self._acclimit.get(), self._duration.get())
+        elif self._base_mode.get() == BASE_FIXED:
+            msg = self._config_fixed(
+                self._acclimit.get(),
+                self._fixedlat.get(),
+                self._fixedlon.get(),
+                self._fixedalt.get(),
+            )
+        else:  # DISABLED
+            msg = self._config_disable()
+        self.__app.gnss_outqueue.put(msg.serialize())
+
+        # set RTCM and UBX NAV-SVIN message output rate
+        rate = 0 if self._base_mode.get() == BASE_DISABLED else 1
+        for port in ("USB", "UART1"):
+            msg = self._config_msg_rates(rate, port)
+            self.__app.gnss_outqueue.put(msg.serialize())
+            msg = self._config_nmea(self._disable_nmea.get(), port)
+            self.__app.gnss_outqueue.put(msg.serialize())
+
+    def _config_msg_rates(self, rate: int, port_type: str) -> UBXMessage:
+        """
+        Configure RTCM3 and UBX NAV-SVIN message rates.
+
+        :param int rate: message rate (0 = off)
+        :param str port_type: port that rcvr is connected on
+        """
+
+        layers = 1  # 1 = RAM, 2 = BBR, 4 = Flash (can be OR'd)
+        transaction = 0
+        cfg_data = []
+        for rtcm_type in (
+            "1005",
+            "1077",
+            "1087",
+            "1097",
+            "1127",
+            "1230",
+            "4072_0",
+            "4072_1",
+        ):
+            cfg = f"CFG_MSGOUT_RTCM_3X_TYPE{rtcm_type}_{port_type}"
+            cfg_data.append([cfg, rate])
 
-        try:
-            raw_data, parsed_data = self.ntripqueue.get(False)
-            if raw_data is not None and parsed_data is not None:
-                if protocol(raw_data) == RTCM3_PROTOCOL:
-                    if self.conn_status == CONNECTED:
-                        self.stream_handler.serial_write(raw_data)
-                    self.process_data(raw_data, parsed_data, "NTRIP>>")
-                else:  # e.g. NMEA GGA sentence sent to NTRIP server
-                    self.process_data(raw_data, parsed_data, "NTRIP<<")
-        except Empty:
-            pass
-        except (SerialException, SerialTimeoutException) as err:
-            self.set_status(f"Error sending to device {err}", "red")
+        # NAV-SVIN only output in SURVEY-IN mode
+        rate = rate if self._base_mode.get() == BASE_SVIN else 0
+        cfg = f"CFG_MSGOUT_UBX_NAV_SVIN_{port_type}"
+        cfg_data.append([cfg, rate])
+
+        return UBXMessage.config_set(layers, transaction, cfg_data)
+
+    def _config_disable(self):
+        """
+        Disable base station mode.
+        """
+
+        layers = 1
+        transaction = 0
+        cfg_data = [
+            ("CFG_TMODE_MODE", TMODE_DISABLED),
+        ]
+
+        return UBXMessage.config_set(layers, transaction, cfg_data)
+
+    def _config_svin(self, acc_limit: int, svin_min_dur: int) -> UBXMessage:
+        """
+        Configure Survey-In mode with specied accuracy limit.
+
+        :param int acc_limit: accuracy limit in cm
+        :param int svin_min_dur: survey minimimum duration
+        """
+
+        layers = 1
+        transaction = 0
+        acc_limit = int(acc_limit * 100)  # convert to 0.1 mm
+        cfg_data = [
+            ("CFG_TMODE_MODE", TMODE_SVIN),
+            ("CFG_TMODE_SVIN_ACC_LIMIT", acc_limit),
+            ("CFG_TMODE_SVIN_MIN_DUR", svin_min_dur),
+        ]
+
+        return UBXMessage.config_set(layers, transaction, cfg_data)
+
+    def _config_fixed(
+        self, acc_limit: int, lat: float, lon: float, height: float
+    ) -> UBXMessage:
+        """
+        Configure Fixed mode with specified coordinates.
+
+        :param int acc_limit: accuracy limit in cm
+        :param float lat: lat or X in m
+        :param float lat: lon or Y in m
+        :param float lat: height or Z in m
+        """
+
+        layers = 1
+        transaction = 0
+        acc_limit = int(acc_limit * 100)  # convert to 0.1 mm
+        if self._pos_mode.get() == POS_LLH:
+            lat_sp, lat_hp = val2sphp(lat, 1e-7)
+            lon_sp, lon_hp = val2sphp(lon, 1e-7)
+            height_sp, height_hp = val2sphp(height, 0.01)
+            cfg_data = [
+                ("CFG_TMODE_MODE", TMODE_FIXED),
+                ("CFG_TMODE_POS_TYPE", LLH),
+                ("CFG_TMODE_FIXED_POS_ACC", acc_limit),
+                ("CFG_TMODE_LAT", lat_sp),
+                ("CFG_TMODE_LAT_HP", lat_hp),
+                ("CFG_TMODE_LON", lon_sp),
+                ("CFG_TMODE_LON_HP", lon_hp),
+                ("CFG_TMODE_HEIGHT", height_sp),
+                ("CFG_TMODE_HEIGHT_HP", height_hp),
+            ]
+        else:  # ECEF
+            x_sp, x_hp = val2sphp(lat, 0.01)
+            y_sp, y_hp = val2sphp(lon, 0.01)
+            z_sp, z_hp = val2sphp(height, 0.01)
+            cfg_data = [
+                ("CFG_TMODE_MODE", TMODE_FIXED),
+                ("CFG_TMODE_POS_TYPE", ECEF),
+                ("CFG_TMODE_FIXED_POS_ACC", acc_limit),
+                ("CFG_TMODE_ECEF_X", x_sp),
+                ("CFG_TMODE_ECEF_X_HP", x_hp),
+                ("CFG_TMODE_ECEF_Y", y_sp),
+                ("CFG_TMODE_ECEF_Y_HP", y_hp),
+                ("CFG_TMODE_ECEF_Z", z_sp),
+                ("CFG_TMODE_ECEF_Z_HP", z_hp),
+            ]
+
+        return UBXMessage.config_set(layers, transaction, cfg_data)
+
+    def _config_nmea(self, state: int, port_type: str) -> UBXMessage:
+        """
+        Disable NMEA messages at port level and use minimum UBX instead.
+
+        :param int state: 1 = disable NMEA, 0 = enable NMEA
+        :param str port_type: port that rcvr is connected on
+        """
+
+        nmea_state = 0 if state else 1
+        layers = 1
+        transaction = 0
+        cfg_data = []
+        cfg_data.append((f"CFG_{port_type}OUTPROT_NMEA", nmea_state))
+        cfg_data.append((f"CFG_{port_type}OUTPROT_UBX", 1))
+        cfg_data.append((f"CFG_MSGOUT_UBX_NAV_PVT_{port_type}", state))
+        cfg_data.append((f"CFG_MSGOUT_UBX_NAV_SAT_{port_type}", state * 4))
+
+        return UBXMessage.config_set(layers, transaction, cfg_data)
+
+    def svin_countdown(self, ela: int, valid: bool, active: bool):
+        """
+        Display countdown of remaining survey-in duration.
+
+        :param int ela: elapsed time
+        :param bool valid: SVIN validity status
+        :param bool active: SVIN active status
+        """
+
+        if self._base_mode.get() == BASE_SVIN and active and not valid:
+            self._lbl_elapsed.grid_forget()
+            self._pgb_elapsed.grid(
+                column=2, row=2, columnspan=2, padx=2, pady=1, sticky=W
+            )
+            dur = self._duration.get()
+            self._pgb_elapsed["value"] = 100 * (dur - ela) / dur
+        elif self._base_mode.get() == BASE_SVIN and valid:
+            self._pgb_elapsed.grid_forget()
+            self._lbl_elapsed.grid(
+                column=2, row=2, columnspan=2, padx=2, pady=1, sticky=W
+            )
+            self._lbl_elapsed.config(text="SVIN Valid")
+        else:
+            self._lbl_elapsed.grid_forget()
+            self._pgb_elapsed.grid_forget()
 
-    def update_ntrip_status(self, status: bool, msg: tuple = None):
+    @property
+    def socketserving(self) -> bool:
         """
-        Update NTRIP configuration dialog connection status.
+        Getter for socket serve flag.
 
-        :param bool status: connected to NTRIP server yes/no
-        :param tuple msg: tuple of (message, color)
+        :return: server running True/False
+        :rtype: bool
         """
 
-        if self.dlg_ntripconfig is not None:
-            self.dlg_ntripconfig.set_controls(status, msg)
+        return self._socket_serve.get()
 
-    def get_coordinates(self) -> tuple:
+    @socketserving.setter
+    def socketserving(self, state: bool):
         """
-        Get current coordinates.
+        Setter for socket serve flag.
 
-        :return: tuple (conn_status, lat, lon, alt, sep)
-        :rtype: tuple
+        :param bool state: server running True/False
         """
 
-        return (
-            self._conn_status,
-            self.gnss_status.lat,
-            self.gnss_status.lon,
-            self.gnss_status.alt,
-            self.gnss_status.sep,
-        )
-
-    def process_data(self, raw_data: bytes, parsed_data: object, marker: str = ""):
-        """
-        Update the various GUI widgets, GPX track and log file
-        with the latest data. Parsed data tagged with a 'marker' is
-        written to the console for information but not processed further.
-
-        :param bytes raw_data: raw message data
-        :param object parsed data: NMEAMessage, UBXMessage or RTCMMessage
-        :param str marker: string prepended to console entries e.g. "NTRIP>>"
-        """
-
-        protfilter = self.frm_settings.protocol
-        msgprot = protocol(raw_data)
-        if isinstance(parsed_data, str):
-            marker = "WARNING  "
-
-        if msgprot == UBX_PROTOCOL and msgprot & protfilter:
-            if marker == "":
-                self.ubx_handler.process_data(raw_data, parsed_data)
-            else:
-                parsed_data = marker + str(parsed_data)
-        elif msgprot == NMEA_PROTOCOL and msgprot & protfilter:
-            if marker == "":
-                self.nmea_handler.process_data(raw_data, parsed_data)
-            else:
-                parsed_data = marker + str(parsed_data)
-        elif msgprot == RTCM3_PROTOCOL and msgprot & protfilter:
-            if marker != "":
-                parsed_data = marker + str(parsed_data)
-        else:
-            return
-
-        self.frm_console.update_console(raw_data, parsed_data)
-
-        if datetime.now() > self._last_gui_update + timedelta(
-            seconds=GUI_UPDATE_INTERVAL
-        ):
-            self.frm_banner.update_banner()
-            self.frm_mapview.update_map()
-            self.frm_satview.update_sats()
-            self.frm_graphview.update_graph()
-            self._last_gui_update = datetime.now()
-
-        # update GPX track file if enabled
-        if self.frm_settings.record_track:
-            self._update_gpx_track()
-
-        # update log file if enabled
-        if self.frm_settings.datalogging:
-            self.file_handler.write_logfile(raw_data, parsed_data)
-
-    def _update_gpx_track(self):
-        """
-        Update GPX track with latest valid position readings.
-        """
-
-        # must have valid coords
-        if self.gnss_status.lat == "" or self.gnss_status.lon == "":
-            return
-
-        if datetime.now() > self._last_track_update + timedelta(
-            seconds=GPX_TRACK_INTERVAL
-        ):
-            today = datetime.now()
-            gpstime = self.gnss_status.utc
-            trktime = datetime(
-                today.year,
-                today.month,
-                today.day,
-                gpstime.hour,
-                gpstime.minute,
-                gpstime.second,
-                gpstime.microsecond,
-            )
-            time = f"{trktime.isoformat()}Z"
-            if self.gnss_status.diff_corr:
-                fix = "dgps"
-            elif self.gnss_status.fix == "3D":
-                fix = "3d"
-            elif self.gnss_status.fix == "2D":
-                fix = "2d"
-            else:
-                fix = "none"
-            diff_age = self.gnss_status.diff_age
-            diff_station = self.gnss_status.diff_station
-            if diff_age in [None, "", 0] or diff_station in [None, "", 0]:
-                self.file_handler.add_trackpoint(
-                    self.gnss_status.lat,
-                    self.gnss_status.lon,
-                    ele=self.gnss_status.alt,
-                    time=time,
-                    fix=fix,
-                    sat=self.gnss_status.sip,
-                    pdop=self.gnss_status.pdop,
-                )
-            else:
-                self.file_handler.add_trackpoint(
-                    self.gnss_status.lat,
-                    self.gnss_status.lon,
-                    ele=self.gnss_status.alt,
-                    time=time,
-                    fix=fix,
-                    sat=self.gnss_status.sip,
-                    pdop=self.gnss_status.pdop,
-                    ageofdgpsdata=diff_age,
-                    dgpsid=diff_station,
-                )
-
-            self._last_track_update = datetime.now()
+        return self._socket_serve.set(state)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/banner_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/banner_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,49 +5,51 @@
 
 Created on 13 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 from platform import system
-from tkinter import Frame, Label, Button, StringVar, font, N, S, W, E, SUNKEN
-from PIL import ImageTk, Image
+from tkinter import SUNKEN, Button, E, Frame, Label, N, S, StringVar, W, font
+
+from PIL import Image, ImageTk
+from pynmeagps.nmeahelpers import latlon2dmm, latlon2dms, llh2ecef
 from pyubx2 import dop2str
-from pygnssutils.helpers import latlon2dms, latlon2dmm
+
 from pygpsclient.globals import (
+    BGCOL,
+    CONNECTED,
+    CONNECTED_FILE,
+    CONNECTED_NTRIP,
+    CONNECTED_SOCKET,
+    CONNECTED_SPARTNIP,
+    CONNECTED_SPARTNLB,
     DMM,
     DMS,
-    UMK,
-    UI,
-    UIK,
+    ECEF,
+    FGCOL,
+    ICON_BLANK,
     ICON_CONN,
-    ICON_SERIAL,
-    ICON_SOCKET,
+    ICON_CONTRACT,
     ICON_DISCONN,
-    ICON_LOGREAD,
     ICON_EXPAND,
-    ICON_CONTRACT,
-    ICON_TRANSMIT,
-    ICON_NOTRANSMIT,
+    ICON_LOGREAD,
     ICON_NOCLIENT,
-    CONNECTED,
-    CONNECTED_SOCKET,
-    CONNECTED_FILE,
-    BGCOL,
-    FGCOL,
-)
-from pygpsclient.helpers import (
-    m2ft,
-    ms2mph,
-    ms2kmph,
-    ms2knots,
+    ICON_NTRIPCONFIG,
+    ICON_SERIAL,
+    ICON_SOCKET,
+    ICON_SPARTNCONFIG,
+    ICON_TRANSMIT,
+    UI,
+    UIK,
+    UMK,
 )
+from pygpsclient.helpers import m2ft, ms2kmph, ms2knots, ms2mph
 
 DGPSYES = "YES"
 DGPSNO = "N/A"
 
 
 class BannerFrame(Frame):
     """
@@ -60,15 +62,15 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         self._time = StringVar()
         self._lat = StringVar()
         self._lon = StringVar()
         self._alt = StringVar()
         self._speed = StringVar()
@@ -93,16 +95,18 @@
         self._img_serial = ImageTk.PhotoImage(Image.open(ICON_SERIAL))
         self._img_socket = ImageTk.PhotoImage(Image.open(ICON_SOCKET))
         self._img_file = ImageTk.PhotoImage(Image.open(ICON_LOGREAD))
         self._img_disconn = ImageTk.PhotoImage(Image.open(ICON_DISCONN))
         self._img_expand = ImageTk.PhotoImage(Image.open(ICON_EXPAND))
         self._img_contract = ImageTk.PhotoImage(Image.open(ICON_CONTRACT))
         self._img_transmit = ImageTk.PhotoImage(Image.open(ICON_TRANSMIT))
-        self._img_notransmit = ImageTk.PhotoImage(Image.open(ICON_NOTRANSMIT))
         self._img_noclient = ImageTk.PhotoImage(Image.open(ICON_NOCLIENT))
+        self._img_ntrip = ImageTk.PhotoImage(Image.open(ICON_NTRIPCONFIG))
+        self._img_spartn = ImageTk.PhotoImage(Image.open(ICON_SPARTNCONFIG))
+        self._img_blank = ImageTk.PhotoImage(Image.open(ICON_BLANK))
 
         self.width, self.height = self.get_size()
 
         self._body()
         self._do_layout()
         self._attach_events()
 
@@ -167,23 +171,23 @@
             bg=self._bgcol,
             fg=self._fgcol,
             anchor=N,
         )
 
         self.option_add("*Font", self.__app.font_lg)
         self._lbl_status_preset = Label(
-            self._frm_connect, bg=self._bgcol, image=self._img_conn, fg="blue"
+            self._frm_connect, bg=self._bgcol, image=self._img_conn
+        )
+        self._lbl_rtk_preset = Label(
+            self._frm_connect, bg=self._bgcol, image=self._img_blank
         )
         self._lbl_transmit_preset = Label(
-            self._frm_connect,
-            bg=self._bgcol,
-            image=self._img_notransmit,
-            text="0",
-            fg="grey",
+            self._frm_connect, bg=self._bgcol, image=self._img_blank
         )
+
         self._lbl_time = Label(
             self._frm_basic, textvariable=self._time, bg=self._bgcol, fg="cyan"
         )
         self._lbl_lat = Label(
             self._frm_basic, textvariable=self._lat, bg=self._bgcol, fg="orange"
         )
         self._lbl_lon = Label(
@@ -262,16 +266,17 @@
         )
 
     def _do_layout(self):
         """
         Position widgets in frame.
         """
 
-        self._lbl_status_preset.grid(column=0, row=0, padx=8, pady=3, sticky=W)
-        self._lbl_transmit_preset.grid(column=1, row=0, padx=8, pady=3, sticky=W)
+        self._lbl_status_preset.grid(column=0, row=0, padx=2, pady=3, sticky=W)
+        self._lbl_rtk_preset.grid(column=1, row=0, padx=2, pady=3, sticky=W)
+        self._lbl_transmit_preset.grid(column=2, row=0, padx=2, pady=3, sticky=W)
         self._lbl_ltime.grid(column=1, row=0, pady=3, sticky=W)
         self._lbl_time.grid(column=2, row=0, pady=3, sticky=W)
         self._lbl_llat.grid(column=3, row=0, pady=3, sticky=W)
         self._lbl_lat.grid(column=4, row=0, pady=3, sticky=W)
         self._lbl_llon.grid(column=5, row=0, pady=3, sticky=W)
         self._lbl_lon.grid(column=6, row=0, pady=3, sticky=W)
         self._lbl_lalt.grid(column=7, row=0, pady=3, sticky=W)
@@ -307,19 +312,19 @@
         """
         Toggle advanced banner frame on or off.
         """
 
         self._frm_connect.grid(
             column=0, row=0, rowspan=2, pady=3, ipadx=3, ipady=3, sticky=(N, W)
         )
-        self._frm_basic.grid(column=1, row=0, pady=3, sticky=(W))
+        self._frm_basic.grid(column=1, row=0, pady=3, sticky=W)
         self._frm_toggle.grid(column=5, row=0, rowspan=2, pady=3, sticky=(N, E))
         self._show_advanced = not self._show_advanced
         if self._show_advanced:
-            self._frm_advanced.grid(column=1, row=1, pady=3, sticky=(W))
+            self._frm_advanced.grid(column=1, row=1, pady=3, sticky=W)
             self._btn_toggle.config(image=self._img_contract)
         else:
             self._frm_advanced.grid_forget()
             self._btn_toggle.config(image=self._img_expand)
 
     def _attach_events(self):
         """
@@ -340,38 +345,53 @@
         elif status == CONNECTED_SOCKET:
             self._lbl_status_preset.configure(image=self._img_socket)
         elif status == CONNECTED_FILE:
             self._lbl_status_preset.configure(image=self._img_file)
         else:
             self._lbl_status_preset.configure(image=self._img_disconn)
 
+    def update_rtk_status(self, rtk: int = 0):
+        """
+        Update RTK status icon.
+
+        :param int rtk: rtk transmit status (none = 0, ntrip = 1, spartn = 2/4)
+        """
+
+        if rtk == CONNECTED_NTRIP:
+            self._lbl_rtk_preset.configure(image=self._img_ntrip)
+        elif rtk in (CONNECTED_SPARTNIP, CONNECTED_SPARTNLB):
+            self._lbl_rtk_preset.configure(image=self._img_spartn)
+        else:
+            self._lbl_rtk_preset.configure(image=self._img_blank)
+
     def update_transmit_status(self, transmit: int = 1):
         """
-        Update socket server status icon
+        Update socket server status icon.
 
         :param int transmit: socket server transmit status (-1, 0, 1)
         """
 
         if transmit > 0:
             self._lbl_transmit_preset.configure(image=self._img_transmit)
         elif transmit == 0:
             self._lbl_transmit_preset.configure(image=self._img_noclient)
         else:
-            self._lbl_transmit_preset.configure(image=self._img_notransmit)
+            self._lbl_transmit_preset.configure(image=self._img_blank)
 
-    def update_banner(self):
+    def update_frame(self):
         """
         Sets text of banner from GNSSStatus object.
         """
 
-        disp_format = self.__app.frm_settings.format
-        units = self.__app.frm_settings.units
+        settings = self.__app.frm_settings.config
+        deg_format = settings["degreesformat"]
+        units = settings["units"]
 
         self._update_time()
-        self._update_pos(disp_format, units)
+        self._update_pos(deg_format, units)
         self._update_track(units)
         self._update_fix()
         self._update_siv()
         self._update_dop(units)
         self._update_dgps()
 
     def _update_time(self):
@@ -381,42 +401,54 @@
 
         tim = self.__app.gnss_status.utc
         if tim in (None, ""):
             self._time.set("N/A")
         else:
             self._time.set(tim)
 
-    def _update_pos(self, disp_format, units):
+    def _update_pos(self, deg_format, units):
         """
         Update position
 
-        :param str disp_format: degrees display format as string (DMS, DMM, DDD)
+        :param str disp_format: position display format as string (DMS, DMM, DDD, ECEF)
         :param str units: distance units as string (UMM, UMK, UI, UIK)
         """
 
         lat = self.__app.gnss_status.lat
         lon = self.__app.gnss_status.lon
+        alt = self.__app.gnss_status.alt  # hMSL
+        self._lbl_llat.config(text="lat:")
+        self._lbl_llon.config(text="lon:")
+        self._lbl_lalt.config(text="alt:")
+        alt_u = "m"
+
         if isinstance(lat, (int, float)) and isinstance(lon, (int, float)):
-            if disp_format == DMS:
-                lat, lon = latlon2dms((lat, lon))
-            elif disp_format == DMM:
-                lat, lon = latlon2dmm((lat, lon))
+            if deg_format == ECEF and isinstance(alt, (int, float)):
+                lat, lon, alt = llh2ecef(lat, lon, alt)
+                if units in (UI, UIK):
+                    lat, lon = (m2ft(x) for x in (lat, lon))
+                self._lbl_llat.config(text="X:")
+                self._lbl_llon.config(text="Y:")
+                self._lbl_lalt.config(text="Z:")
+            elif deg_format == DMS:
+                lat, lon = latlon2dms(lat, lon)
+            elif deg_format == DMM:
+                lat, lon = latlon2dmm(lat, lon)
             self._lat.set(f"{lat:<15}")
             self._lon.set(f"{lon:<15}")
         else:
             self._lat.set("N/A            ")
             self._lon.set("N/A            ")
 
-        alt = self.__app.gnss_status.alt
-        alt_u = "m"
         if isinstance(alt, (int, float)):
             if units in (UI, UIK):
                 alt = m2ft(alt)
                 alt_u = "ft"
-            self._alt.set(f"{alt:.3f}")
+            fmt = "<15" if deg_format == ECEF else ".3f"
+            self._alt.set(f"{alt:{fmt}}")
             self._alt_u.set(f"{alt_u:<2}")
         else:
             self._alt.set("N/A  ")
             self._alt_u.set("  ")
 
     def _update_track(self, units):
         """
@@ -458,41 +490,44 @@
             self._lbl_fix.config(fg="green2")
         elif fix in ("2D", "DR"):
             self._lbl_fix.config(fg="orange")
         else:
             self._lbl_fix.config(fg="red")
         self._fix.set(fix)
 
-    def _update_siv(self, **kwargs):
+    def _update_siv(self):
         """
         Update siv and sip
         """
 
         self._siv.set(f"{self.__app.gnss_status.siv:02d}")
         self._sip.set(f"{self.__app.gnss_status.sip:02d}")
 
-    def _update_dop(self, units, **kwargs):
+    def _update_dop(self, units):
         """
         Update precision and accuracy
 
         :param str units: distance units as string (UMM, UMK, UI, UIK)
         """
 
         pdop = self.__app.gnss_status.pdop
         self._dop.set(f"{pdop:.2f} {dop2str(pdop):<9}")
         self._hvdop.set(
-            f"hdop {self.__app.gnss_status.hdop:.2f}\nvdop {self.__app.gnss_status.vdop:.2f}"
+            f"hdop {self.__app.gnss_status.hdop:.2f}\n"
+            + f"vdop {self.__app.gnss_status.vdop:.2f}"
         )
         if units in (UI, UIK):
             self._hvacc.set(
-                f"hacc {m2ft(self.__app.gnss_status.hacc):.3f}\nvacc {m2ft(self.__app.gnss_status.vacc):.3f}"
+                f"hacc {m2ft(self.__app.gnss_status.hacc):.3f}\n"
+                + f"vacc {m2ft(self.__app.gnss_status.vacc):.3f}"
             )
         else:
             self._hvacc.set(
-                f"hacc {self.__app.gnss_status.hacc:.3f}\nvacc {self.__app.gnss_status.vacc:.3f}"
+                f"hacc {self.__app.gnss_status.hacc:.3f}\n"
+                + f"vacc {self.__app.gnss_status.vacc:.3f}"
             )
 
     def _update_dgps(self):
         """
         Update DGPS status.
         """
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/console_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/console_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,20 @@
 
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
-from tkinter import Frame, Text, Scrollbar, S, E, W, END, HORIZONTAL, VERTICAL, N
+from tkinter import END, HORIZONTAL, VERTICAL, E, Frame, N, S, Scrollbar, Text, W
+
 from pyubx2 import hextable
-from pygpsclient.globals import (
-    BGCOL,
-    FGCOL,
-    FORMATS,
-    FONT_TEXT,
-    FONT_FIXED,
-)
+
+from pygpsclient.globals import BGCOL, FGCOL, FONT_FIXED, FONT_TEXT, FORMATS
 
 
 class ConsoleFrame(Frame):
     """
     Console frame class.
     """
 
@@ -33,15 +28,15 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         self.width, self.height = self.get_size()
         self._body()
         self._do_layout()
         self._attach_events()
@@ -64,14 +59,15 @@
         self.txt_console = Text(
             self,
             bg=self._console_bg,
             fg=self._console_fg,
             yscrollcommand=self.sblogv.set,
             xscrollcommand=self.sblogh.set,
             wrap="none",
+            height=20,
         )
         self.sblogh.config(command=self.txt_console.xview)
         self.sblogv.config(command=self.txt_console.yview)
         # Making the textbox read only and fixed width font
         self.txt_console.configure(font=FONT_FIXED, state="disabled")
 
     def _do_layout(self):
@@ -86,59 +82,66 @@
     def _attach_events(self):
         """
         Bind events to frame
         """
 
         self.bind("<Configure>", self._on_resize)
 
-    def update_console(self, raw_data, parsed_data):
+    def update_console(self, raw_data: bytes, parsed_data: object, marker: str = ""):
         """
         Print the latest data stream to the console in raw (NMEA) or
         parsed (key,value pair) format.
 
         'maxlines' defines the maximum number of scrollable lines that are
         retained in the text box on a FIFO basis.
 
-        :param str data: data from input stream
+        :param bytes raw_data: raw data from input stream
+        :param object parsed_data: parsed data from input stream
+        :param str marker: information string to prepend to parsed data display
 
         """
 
+        settings = self.__app.frm_settings.config
+        cfm = settings["consoleformat"]
         self._halt = ""
         self.txt_console.configure(font=FONT_FIXED)
-        if self.__app.frm_settings.display_format == FORMATS[1]:  # binary
+        if cfm == FORMATS[1]:  # binary
             data = str(raw_data).strip("\n")
-        elif self.__app.frm_settings.display_format == FORMATS[2]:  # hex string
+        elif cfm == FORMATS[2]:  # hex string
             data = str(raw_data.hex())
-        elif self.__app.frm_settings.display_format == FORMATS[3]:  # hex tabular
+        elif cfm == FORMATS[3]:  # hex tabular
             data = hextable(raw_data)
+        elif cfm == FORMATS[4]:  # parsed + hex tabular
+            data = f"{marker}{parsed_data}\n{hextable(raw_data)}"
         else:
             self.txt_console.configure(font=FONT_TEXT)
-            data = str(parsed_data)
+            data = f"{marker}{parsed_data}"
 
         con = self.txt_console
         con.configure(state="normal")
         con.insert(END, data + "\n")
 
         # format of this list of tuples is (tag, highlight color)
-        if self.__app.frm_settings.colortagging:
-            self._tag_line(data, self.__app.colortags)
+        if settings["colortag"]:
+            colortags = self.__app.app_config.get("colortags", [])
+            self._tag_line(data, colortags)
             if self._halt != "":
                 self.__app.stream_handler.stop_read_thread()
                 self.__app.set_status(f"Halted on user tag match: {self._halt}", "red")
 
         idx = float(con.index("end"))  # Lazy but it works
-        if idx > self.__app.frm_settings.maxlines:
+        if idx > settings["maxlines"]:
             # Remember these tcl indices look like floats but they're not!
             # ("1.0:, "2.0") signifies "from the first character in
             # line 1 (inclusive) to the first character in line 2 (exclusive)"
             # i.e. delete the first line
             con.delete("1.0", "2.0")
 
         # con.update_idletasks()
-        if self.__app.frm_settings.autoscroll:
+        if settings["autoscroll"]:
             con.see("end")
         con.configure(state="disabled")
 
     def _tag_line(self, line, tags):
         """
         Highlights any occurrence of tags in line - each tag
         must be a tuple of (search term, highlight color)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/gnss_status.py` & `pygpsclient-1.4.0/src/pygpsclient/gnss_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,23 +23,26 @@
         """
         Constructor.
         """
 
         self.utc = datetime.utcnow().time().replace(microsecond=0)  # UTC time
         self.lat = 0.0  # latitude as decimal
         self.lon = 0.0  # longitude as decimal
-        self.alt = 0.0  # elevation m
+        self.alt = 0.0  # height above sea level m
         self.speed = 0.0  # speed m/s
         self.track = 0.0  # track degrees
         self.fix = "NO FIX"  # fix type e.g. "3D"
         self.siv = 0  # satellites in view
         self.sip = 0  # satellites in position solution
         self.pdop = 0.0  # dilution of precision DOP
         self.hdop = 0.0  # horizontal DOP
         self.vdop = 0.0  # vertical DOP
         self.hacc = 0.0  # horizontal accuracy m
         self.vacc = 0.0  # vertical accuracy m
-        self.sep = 0.0  # separation from ellipsoid m, used to synthesise GGA sentences
+        self.sep = 0.0  # separation from ellipsoid (height - hMSL) m
         self.diff_corr = 0  # DGPS correction status True/False
         self.diff_age = 0  # DGPS correction age seconds
         self.diff_station = "N/A"  # DGPS station id
         self.gsv_data = []  # list of satellite tuples (gnssId, svid, elev, azim, cno)
+        self.spectrum_data = []  # list of spectrum data (spec, spn, res, ctr, pga)
+        self.sysmon_data = {}  # dict of system monitor data (cpu and memory load, etc.)
+        self.comms_data = {}  # dict of comms port utilisation (tx and rx loads)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/graphview_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/graphview_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 Created on 14 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
-from tkinter import Frame, Canvas, font, BOTH, YES
-from pygpsclient.globals import WIDGETU2, BGCOL, FGCOL, MAX_SNR, GNSS_LIST
+from tkinter import BOTH, YES, Canvas, Frame, font
+
+from pygpsclient.globals import BGCOL, FGCOL, GNSS_LIST, MAX_SNR, WIDGETU2
 from pygpsclient.helpers import snr2col
 
 # Relative offsets of graph axes and legend
 AXIS_XL = 19
 AXIS_XR = 10
 AXIS_Y = 22
 OL_WID = 2
@@ -36,22 +36,23 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         def_w, def_h = WIDGETU2
         self.width = kwargs.get("width", def_w)
         self.height = kwargs.get("height", def_h)
         self._body()
+        self._attach_events()
 
         self.bind("<Configure>", self._on_resize)
 
     def _body(self):
         """
         Set up frame and widgets.
         """
@@ -59,14 +60,32 @@
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)
         self.can_graphview = Canvas(
             self, width=self.width, height=self.height, bg=BGCOL
         )
         self.can_graphview.pack(fill=BOTH, expand=YES)
 
+    def _attach_events(self):
+        """
+        Bind events to frame.
+        """
+
+        self.can_graphview.bind("<Double-Button-1>", self._on_legend)
+
+    def _on_legend(self, event):  # pylint: disable=unused-argument
+        """
+        On double-click - toggle legend on/off.
+
+        :param event: event
+        """
+
+        self.__app.frm_settings.show_legend.set(
+            not self.__app.frm_settings.show_legend.get()
+        )
+
     def init_graph(self):
         """
         Initialise graph view
         """
 
         w, h = self.width, self.height
         resize_font = font.Font(size=min(int(h / 25), 10))
@@ -84,25 +103,25 @@
                 y,
                 text=str(MAX_SNR - (i * 10)),
                 angle=90,
                 fill=FGCOL,
                 font=resize_font,
             )
 
-        if self.__app.frm_settings.show_legend:
+        if self.__app.frm_settings.config["legend"]:
             self._draw_legend()
 
     def _draw_legend(self):
         """
         Draw GNSS color code legend
         """
 
-        w = self.width / 9
+        w = self.width / 10
         h = self.height / 15
-        resize_font = font.Font(size=min(int(self.height / 25), 10))
+        resize_font = font.Font(size=min(int(self.height / 30), 10))
 
         for i, (_, (gnssName, gnssCol)) in enumerate(GNSS_LIST.items()):
             x = LEG_XOFF + w * i
             self.can_graphview.create_rectangle(
                 x,
                 LEG_YOFF,
                 x + w - LEG_GAP,
@@ -115,15 +134,15 @@
                 (x + x + w - LEG_GAP) / 2,
                 LEG_YOFF + h / 2,
                 text=gnssName,
                 fill=FGCOL,
                 font=resize_font,
             )
 
-    def update_graph(self):
+    def update_frame(self):
         """
         Plot satellites' signal-to-noise ratio (cno).
         Automatically adjust y axis according to number of satellites in view.
         """
 
         data = self.__app.gnss_status.gsv_data
         siv = len(self.__app.gnss_status.gsv_data)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/map_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_solrate_frame.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,258 +1,218 @@
 """
-Mapview frame class for PyGPSClient application.
+UBX Configuration frame for CFG-RATE commands
 
-This handles a frame containing a location map downloaded via a MapQuest API.
-
-NOTE: The free MapQuest API key is subject to a limit of 15,000
-transactions / month, or roughly 500 / day, so the map updates are only
-run periodically (once a minute). This utility is NOT intended to be used for
-real time navigation.
-
-Created on 13 Sep 2020
+Created on 19 Feb 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
-from io import BytesIO
-from time import time
-from tkinter import Frame, Canvas, font, NW, N, S, E, W
-from http.client import responses
-from PIL import ImageTk, Image
-from requests import get, RequestException, ConnectionError as ConnError, ConnectTimeout
-
-from pygpsclient.globals import (
-    WIDGETU2,
-    MAPURL,
-    MAP_UPDATE_INTERVAL,
-    IMG_WORLD,
-    ICON_POS,
-    BGCOL,
-)
-from pygpsclient.strings import (
-    NOWEBMAPFIX,
-    NOWEBMAPCONN,
-    NOWEBMAPHTTP,
-    NOWEBMAPKEY,
+from tkinter import Button, E, Frame, IntVar, Label, Spinbox, StringVar, W
+
+from PIL import Image, ImageTk
+from pyubx2 import POLL, SET, UBXMessage
+
+from .globals import (
+    CONNECTED,
+    ICON_CONFIRMED,
+    ICON_PENDING,
+    ICON_SEND,
+    ICON_WARNING,
+    READONLY,
+    UBX_CFGRATE,
 )
+from .strings import LBLCFGRATE
+
+TIMEREFS = {
+    0: "UTC",
+    1: "GPS",
+    2: "GLO",
+    3: "BEI",
+    4: "GAL",
+}
 
 
-class MapviewFrame(Frame):
+class UBX_RATE_Frame(Frame):
     """
-    Map frame class.
+    UBX Navigation Solution Rate configuration command panel.
     """
 
-    def __init__(self, app, *args, **kwargs):
+    def __init__(self, app, container, *args, **kwargs):
         """
         Constructor.
 
         :param Frame app: reference to main tkinter application
+        :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
+        self.__container = container
 
-        Frame.__init__(self, self.__master, *args, **kwargs)
+        Frame.__init__(self, self.__container.container, *args, **kwargs)
 
-        def_w, def_h = WIDGETU2
-        self.width = kwargs.get("width", def_w)
-        self.height = kwargs.get("height", def_h)
-        self._img = None
-        self._marker = None
-        self._last_map_update = 0
-        self._body()
+        self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
+        self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
+        self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
+        self._img_warn = ImageTk.PhotoImage(Image.open(ICON_WARNING))
+        self._measint = IntVar()
+        self._navrate = IntVar()
+        self._timeref = StringVar()
 
-        self.bind("<Configure>", self._on_resize)
+        self._body()
+        self._do_layout()
+        self._attach_events()
 
     def _body(self):
         """
         Set up frame and widgets.
         """
 
-        self.grid_columnconfigure(0, weight=1)
-        self.grid_rowconfigure(0, weight=1)
-        self.can_mapview = Canvas(self, width=self.width, height=self.height, bg=BGCOL)
-        self.can_mapview.grid(column=0, row=0, sticky=(N, S, E, W))
-
-    def update_map(self):
-        """
-        Draw map and mark current known position and horizontal accuracy (where available).
-        """
-
-        lat = self.__app.gnss_status.lat
-        lon = self.__app.gnss_status.lon
-        hacc = self.__app.gnss_status.hacc
-
-        if self.__app.frm_settings.webmap:
-            static = False
-        else:
-            static = True
-
-        # if no valid position, display warning message
-        # fix = kwargs.get("fix", 0)
-        if (
-            lat in (None, "")
-            or lon in (None, "")
-            or (lat == 0 and lon == 0)
-            # or fix in (0, 5)  # no fix or time only
-        ):
-            self.reset_map_refresh()
-            self._disp_error(NOWEBMAPFIX)
-            return
-
-        if static:
-            self._draw_static_map(lat, lon)
-        else:
-            if hacc is None or hacc == "":
-                hacc = 0
-            self._draw_web_map(lat, lon, hacc)
-
-    def _draw_static_map(self, lat: float, lon: float):
-        """
-        Draw fixed scale Mercator world map
-
-        :param float lat: latitude
-        :param float lon: longitude
-        """
-
-        OFFSET_X = 0
-        OFFSET_Y = 0
-
-        w, h = self.width, self.height
-        self.can_mapview.delete("all")
-        self._img = ImageTk.PhotoImage(
-            Image.open(IMG_WORLD).resize((w, h), Image.ANTIALIAS)
+        self._lbl_cfg_rate = Label(self, text=LBLCFGRATE, anchor="w")
+        self._lbl_ubx_measint = Label(self, text="Solution Interval (ms)")
+        self._spn_ubx_measint = Spinbox(
+            self,
+            values=(25, 50, 100, 200, 500, 1000, 2000, 5000, 10000),
+            width=6,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._measint,
+        )
+        self._lbl_ubx_navrate = Label(self, text="Measurement Ratio")
+        self._spn_ubx_navrate = Spinbox(
+            self,
+            from_=1,
+            to=127,
+            width=4,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._navrate,
+        )
+        self._lbl_ubx_timeref = Label(self, text="Time Reference")
+        self._spn_ubx_timeref = Spinbox(
+            self,
+            values=list(TIMEREFS.values()),
+            width=5,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._timeref,
+        )
+        self._lbl_send_command = Label(self, image=self._img_pending)
+        self._btn_send_command = Button(
+            self,
+            image=self._img_send,
+            width=50,
+            command=self._on_send_rate,
+            font=self.__app.font_md,
         )
-        self._marker = ImageTk.PhotoImage(Image.open(ICON_POS))
-        self.can_mapview.create_image(0, 0, image=self._img, anchor=NW)
-        x = (w / 2) + int((lon * (w / 360))) + OFFSET_X
-        y = (h / 2) - int((lat * (h / 180))) + OFFSET_Y
-        self.can_mapview.create_image(x, y, image=self._marker, anchor=S)
 
-    def _draw_web_map(self, lat: float, lon: float, hacc: float):
+    def _do_layout(self):
         """
-        Draw scalable web map via MapQuest API
-
-        :param float lat: latitude
-        :param float lon: longitude
-        :param float hacc: horizontal accuracy
+        Layout widgets.
         """
 
-        sc = "NO CONNECTION"
-        msg = ""
-
-        apikey = self.__app.api_key
-        if apikey == "":
-            self._disp_error(NOWEBMAPKEY)
-            return
-
-        now = time()
-        if now - self._last_map_update < MAP_UPDATE_INTERVAL:
-            self._draw_countdown(
-                (-360 / MAP_UPDATE_INTERVAL) * (now - self._last_map_update)
-            )
-            return
-        self._last_map_update = now
-
-        url = self._format_url(apikey, lat, lon, hacc)
-
-        try:
-            response = get(url)
-            sc = responses[response.status_code]  # get descriptive HTTP status
-            response.raise_for_status()  # raise Exception on HTTP error
-            if sc == "OK":
-                img_data = response.content
-                self._img = ImageTk.PhotoImage(Image.open(BytesIO(img_data)))
-                self.can_mapview.delete("all")
-                self.can_mapview.create_image(0, 0, image=self._img, anchor=NW)
-                self.can_mapview.update_idletasks()
-                return
-        except (ConnError, ConnectTimeout):
-            msg = NOWEBMAPCONN
-        except RequestException:
-            msg = NOWEBMAPHTTP.format(sc)
+        self._lbl_cfg_rate.grid(column=0, row=0, columnspan=6, padx=3, sticky=(W, E))
+        self._lbl_ubx_measint.grid(
+            column=0, row=1, columnspan=2, rowspan=1, padx=3, pady=3, sticky=W
+        )
+        self._spn_ubx_measint.grid(column=2, row=1, columnspan=1, rowspan=1, sticky=W)
+        self._lbl_ubx_navrate.grid(
+            column=0, row=2, columnspan=2, rowspan=1, padx=3, pady=3, sticky=W
+        )
+        self._spn_ubx_navrate.grid(column=2, row=2, columnspan=2, rowspan=1, sticky=W)
+        self._lbl_ubx_timeref.grid(
+            column=0, row=3, columnspan=2, rowspan=1, padx=3, pady=3, sticky=W
+        )
+        self._spn_ubx_timeref.grid(column=2, row=3, columnspan=2, rowspan=1, sticky=W)
+        self._btn_send_command.grid(
+            column=4, row=1, rowspan=3, ipadx=3, ipady=3, sticky=E
+        )
+        self._lbl_send_command.grid(
+            column=5, row=1, rowspan=3, ipadx=3, ipady=3, sticky=E
+        )
 
-        self._disp_error(msg)
+        (cols, rows) = self.grid_size()
+        for i in range(cols):
+            self.grid_columnconfigure(i, weight=1)
+        for i in range(rows):
+            self.grid_rowconfigure(i, weight=1)
+        self.option_add("*Font", self.__app.font_sm)
 
-    def _draw_countdown(self, wait):
+    def _attach_events(self):
         """
-        Draw clock icon indicating time until next scheduled map refresh.
-
-        :param int wait: wait time in seconds
+        Bind events to widget.
         """
 
-        self.can_mapview.create_oval((5, 5, 20, 20), fill="#616161", outline="")
-        self.can_mapview.create_arc(
-            (5, 5, 20, 20), start=90, extent=wait, fill="#ffffff", outline=""
-        )
+        # click mouse button to refresh information
+        self.bind("<Button>", self._do_poll_rate)
 
-    def _format_url(self, apikey: str, lat: float, lon: float, hacc: float):
+    def reset(self):
         """
-        Formats URL for web map download.
-
-        :param str apikey: MapQuest API key
-        :param float lat: latitude
-        :param float lon: longitude
-        :param float hacc: horizontal accuracy
-        :return: formatted MapQuest URL
-        :rtype: str
+        Reset panel to initial settings.
         """
 
-        w, h = self.width, self.height
-        radius = str(hacc / 1000)  # km
-
-        return MAPURL.format(
-            apikey, lat, lon, self.__app.frm_settings.mapzoom, radius, lat, lon, w, h
-        )
+        if self.__app.conn_status == CONNECTED:
+            self._do_poll_rate()
 
-    def _disp_error(self, msg):
+    def update_status(self, msg: UBXMessage):
         """
-        Display error message in webmap widget.
+        Update pending confirmation status.
 
-        :param str msg: error message
+        :param UBXMessage msg: UBX config message
         """
 
-        w, h = self.width, self.height
-        resize_font = font.Font(size=min(int(w / 20), 14))
+        if msg.identity == "CFG-RATE":
+            self._measint.set(msg.measRate)
+            self._navrate.set(msg.navRate)
+            self._timeref.set(TIMEREFS[msg.timeRef])
+            self._lbl_send_command.config(image=self._img_confirmed)
+            self.__container.set_status("CFG-RATE GET message received", "green")
 
-        self.can_mapview.delete("all")
-        self.can_mapview.create_text(
-            w / 2,
-            h / 2 - (w / 20),
-            text=msg,
-            fill="orange",
-            font=resize_font,
-        )
+        elif msg.identity == "ACK-NAK":
+            self.__container.set_status("CFG-RATE POLL message rejected", "red")
+            self._lbl_send_command.config(image=self._img_warn)
 
-    def reset_map_refresh(self):
+    def _on_send_rate(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
-        Reset map refresh counter to zero
+        Handle Send rate config button press.
         """
 
-        self._last_map_update = 0
-
-    def _on_resize(self, event):  # pylint: disable=unused-argument
-        """
-        Resize frame
+        tref = 0
+        for key, val in TIMEREFS.items():
+            if val == self._timeref.get():
+                tref = key
+                break
 
-        :param event event: resize event
-        """
+        msg = UBXMessage(
+            "CFG",
+            "CFG-RATE",
+            SET,
+            measRate=self._measint.get(),
+            navRate=self._navrate.get(),
+            timeRef=tref,
+        )
+        self.__container.send_command(msg)
+        self._lbl_send_command.config(image=self._img_pending)
+        self.__container.set_status(
+            "CFG-RATE SET message sent",
+        )
+        self.__container.set_pending(UBX_CFGRATE, ("ACK-ACK", "ACK-NAK"))
 
-        self.width, self.height = self.get_size()
+        self._do_poll_rate()
 
-    def get_size(self):
+    def _do_poll_rate(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
-        Get current canvas size.
-
-        :return: window size (width, height)
-        :rtype: tuple
+        Poll RATE message configuration.
         """
 
-        self.update_idletasks()  # Make sure we know about any resizing
-        width = self.can_mapview.winfo_width()
-        height = self.can_mapview.winfo_height()
-        return (width, height)
+        msg = UBXMessage("CFG", "CFG-RATE", POLL)
+        self.__container.send_command(msg)
+        self._lbl_send_command.config(image=self._img_pending)
+        self.__container.set_status(
+            "CFG-RATE POLL message sent",
+        )
+        for msgid in ("CFG-RATE", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGRATE)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/nmea_handler.py` & `pygpsclient-1.4.0/src/pygpsclient/nmea_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """
-NMEA Protocol handler - handles all incoming standard and proprietary NMEA sentences
+nmea_handler.py
 
-Uses pynmea2 library for parsing
+NMEA Protocol handler - handles all incoming standard and
+proprietary NMEA sentences.
+
+Parses individual NMEA sentences (using pynmeagps library)
+and adds selected attribute values to the app.gnss_status
+data dictionary. This dictionary is then used to periodically
+update the various user-selectable widgets.
 
 Created on 30 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 from time import time
+
 from pynmeagps import NMEAMessage
+
 from pygpsclient.globals import SAT_EXPIRY
-from pygpsclient.helpers import knots2ms, kmph2ms, fix2desc
+from pygpsclient.helpers import fix2desc, kmph2ms, knots2ms, svid2gnssid
 
 
 class NMEAHandler:
     """
     NMEA handler class.
     """
 
@@ -26,15 +33,15 @@
         """
         Constructor.
 
         :param Frame app: reference to main tkinter application
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
         self._raw_data = None
         self._parsed_data = None
         self.gsv_data = (
             []
         )  # Holds array of current satellites in view from NMEA GSV sentences
         self.gsv_log = {}  # Holds cumulative log of all satellites seen
@@ -67,14 +74,17 @@
             elif parsed_data.msgID == "GSV":  # GPS Satellites in View
                 self._process_GSV(parsed_data)
             elif parsed_data.msgID == "ZDA":  # ZDA Time
                 self._process_ZDA(parsed_data)
             # proprietary GPS Lat/Lon & Acc
             elif parsed_data.msgID == "UBX" and parsed_data.msgId == "00":
                 self._process_UBX00(parsed_data)
+            # proprietary GPS Lat/Lon & Acc
+            elif parsed_data.msgID == "UBX" and parsed_data.msgId == "03":
+                self._process_UBX03(parsed_data)
 
         except ValueError:
             pass
 
     def _process_RMC(self, data: NMEAMessage):
         """
         Process RMC sentence - Recommended minimum data for GPS.
@@ -175,64 +185,67 @@
         Modern receivers can send multiple batches corresponding to different
         GNSS constellations (GPS 1-32, SBAS 33-64, GLONASS 65-96 etc.).
 
         :param pynmeagps.NMEAMessage data: parsed GSV sentence
         """
         # pylint: disable=consider-using-dict-items
 
-        show_unused = self.__app.frm_settings.show_unused
+        settings = self.__app.frm_settings.config
+        show_unused = settings["unusedsat"]
         self.gsv_data = []
         gsv_dict = {}
         now = time()
         if data.talker == "GA":
             gnss = 2  # Galileo
         elif data.talker == "GB":
             gnss = 3  # Beidou (only available in MMEA 4.11)
         elif data.talker == "GL":
             gnss = 6  # GLONASS
+        elif data.talker == "GI":
+            gnss = 7  # NAVIC
         else:
             gnss = 0  # GPS, SBAS, QZSS
 
         try:
             if data.svid_01 != "":
                 svid = data.svid_01
-                key = str(gnss) + "-" + str(svid)
+                key = f"{gnss}-{svid}"
                 gsv_dict[key] = (
                     gnss,
                     svid,
                     data.elv_01,
                     data.az_01,
                     str(data.cno_01),
                     now,
                 )
             if data.svid_02 != "":
                 svid = data.svid_02
-                key = str(gnss) + "-" + str(svid)
+                key = f"{gnss}-{svid}"
                 gsv_dict[key] = (
                     gnss,
                     svid,
                     data.elv_02,
                     data.az_02,
                     str(data.cno_02),
                     now,
                 )
             if data.svid_03 != "":
                 svid = data.svid_03
-                key = str(gnss) + "-" + str(svid)
+                key = f"{gnss}-{svid}"
                 gsv_dict[key] = (
                     gnss,
                     svid,
                     data.elv_03,
                     data.az_03,
                     str(data.cno_03),
                     now,
                 )
             if data.svid_04 != "":
                 svid = data.svid_04
-                key = str(gnss) + "-" + str(svid)
+                key = f"{gnss}-{svid}"
                 gsv_dict[key] = (
                     gnss,
                     svid,
                     data.elv_04,
                     data.az_04,
                     str(data.cno_04),
                     now,
@@ -274,23 +287,67 @@
         :param pynmeagps.NMEAMessage data: parsed ZDA sentence
         """
 
         self.__app.gnss_status.utc = data.time
 
     def _process_UBX00(self, data: NMEAMessage):
         """
-        Process UXB00 sentence - GPS Vector track and Speed over the Ground.
+        Process UXB00 sentence - Lat/Long position data.
 
         :param pynmeagps.NMEAMessage data: parsed UBX,00 sentence
         """
 
         self.__app.gnss_status.lat = data.lat
         self.__app.gnss_status.lon = data.lon
         # self.__app.gnss_status.alt = data.altRef height above datum, not SL
         self.__app.gnss_status.speed = data.SOG
         self.__app.gnss_status.track = data.COG
-        self.__app.gnss_status.pdop = data.PDOP
         self.__app.gnss_status.hdop = data.HDOP
         self.__app.gnss_status.vdop = data.VDOP
         self.__app.gnss_status.hacc = data.hAcc
         self.__app.gnss_status.vacc = data.vAcc
         self.__app.gnss_status.sip = data.numSVs
+
+    def _process_UBX03(self, data: NMEAMessage):
+        """
+        Process UXB03 sentence - NMEA Satellite Status.
+
+        NB: this message appears to use the legacy NMEA 2.n
+        SVID numbering scheme. This may conflict with GSV
+        satellite data if both message types are enabled.
+
+        :param pynmeagps.NMEAMessage data: parsed UBX,03 sentence
+        """
+        # pylint: disable=consider-using-dict-items
+
+        settings = self.__app.frm_settings.config
+        show_unused = settings["unusedsat"]
+        self.gsv_data = []
+        gsv_dict = {}
+        now = time()
+        for i in range(data.numSv):
+            # status = getattr(data, f"status_{i+1:02}")
+            # if status == "U" or show_unused:
+            svid = getattr(data, f"svid_{i+1:02}")
+            gnss = svid2gnssid(svid)
+            key = f"{gnss}-{svid}"
+            gsv_dict[key] = (
+                gnss,
+                svid,
+                getattr(data, f"azi_{i+1:02}"),
+                getattr(data, f"ele_{i+1:02}"),
+                str(getattr(data, f"cno_{i+1:02}")),
+                now,
+            )
+
+        for key in gsv_dict:
+            self.gsv_log[key] = gsv_dict[key]
+
+        for key in self.gsv_log:
+            gnssId, svid, elev, azim, snr, lastupdate = self.gsv_log[key]
+            if snr in ("", "0", 0) and not show_unused:  # omit unused sats
+                continue
+            if now - lastupdate < SAT_EXPIRY:  # expire passed sats
+                self.gsv_data.append((gnssId, svid, elev, azim, snr))
+
+        self.__app.gnss_status.siv = len(self.gsv_data)
+        self.__app.gnss_status.gsv_data = self.gsv_data
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ntrip_client_dialog.py` & `pygpsclient-1.4.0/src/pygpsclient/ntrip_client_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,81 +9,78 @@
 
 Created on 2 Apr 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
+from socket import AF_INET, AF_INET6
 from tkinter import (
-    ttk,
-    Toplevel,
-    Frame,
+    DISABLED,
+    END,
+    HORIZONTAL,
+    NORMAL,
+    VERTICAL,
     Button,
-    Label,
+    E,
     Entry,
-    Spinbox,
-    Listbox,
-    Scrollbar,
-    Radiobutton,
-    StringVar,
+    Frame,
     IntVar,
+    Label,
+    Listbox,
     N,
+    Radiobutton,
     S,
-    E,
-    W,
-    NORMAL,
-    DISABLED,
-    END,
-    VERTICAL,
-    HORIZONTAL,
+    Scrollbar,
+    Spinbox,
+    StringVar,
     TclError,
+    Toplevel,
+    W,
+    ttk,
 )
-from PIL import ImageTk, Image
+
+from PIL import Image, ImageTk
 from pygnssutils import NOGGA
 from pygnssutils.helpers import find_mp_distance
+
 from pygpsclient.globals import (
-    ICON_EXIT,
+    CONNECTED_NTRIP,
+    DISCONNECTED,
+    DLGTNTRIP,
+    GGA_INTERVALS,
     ICON_CONN,
     ICON_DISCONN,
-    UBX_MONVER,
-    UBX_MONHW,
+    ICON_EXIT,
+    POPUP_TRANSIENT,
+    READONLY,
+    UBX_CFGMSG,
     UBX_CFGPRT,
     UBX_CFGRATE,
-    UBX_CFGMSG,
     UBX_CFGVAL,
+    UBX_MONHW,
+    UBX_MONVER,
     UBX_PRESET,
-    ENTCOL,
-    READONLY,
-    POPUP_TRANSIENT,
     UI,
     UIK,
-    GGA_INTERVALS,
 )
+from pygpsclient.helpers import MAXALT, MAXPORT, VALFLOAT, VALINT, VALURL, valid_entry
 from pygpsclient.strings import (
     DLGNTRIPCONFIG,
-    LBLNTRIPSERVER,
-    LBLNTRIPPORT,
-    LBLNTRIPVERSION,
+    LBLGGAFIXED,
+    LBLGGALIVE,
+    LBLNTRIPGGAINT,
     LBLNTRIPMOUNT,
-    LBLNTRIPUSER,
+    LBLNTRIPPORT,
     LBLNTRIPPWD,
-    LBLNTRIPGGAINT,
+    LBLNTRIPSERVER,
     LBLNTRIPSTR,
-    LBLGGALIVE,
-    LBLGGAFIXED,
-)
-from pygpsclient.helpers import (
-    valid_entry,
-    VALINT,
-    VALFLOAT,
-    VALURL,
-    MAXPORT,
-    MAXALT,
+    LBLNTRIPUSER,
+    LBLNTRIPVERSION,
 )
 
 NTRIP_VERSIONS = ("2.0", "1.0")
 KM2MILES = 0.6213712
 
 
 class NTRIPConfigDialog(Toplevel):
@@ -97,15 +94,15 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to parent class (not currently used)
         :param kwargs: optional kwargs to pass to parent class (not currently used)
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         Toplevel.__init__(self, app)
         if POPUP_TRANSIENT:
             self.transient(self.__app)
         self.resizable(True, True)  # allow for MacOS resize glitches
         self.title(DLGNTRIPCONFIG)  # pylint: disable=E1102
         self.protocol("WM_DELETE_WINDOW", self.on_exit)
         self._img_exit = ImageTk.PhotoImage(Image.open(ICON_EXIT))
@@ -122,14 +119,15 @@
             UBX_CFGRATE: (),
         }
         self._status = StringVar()
         self._status_cfgmsg = StringVar()
         self._ntrip_version = StringVar()
         self._ntrip_server = StringVar()
         self._ntrip_port = StringVar()
+        self._ntrip_ipprot = StringVar()
         self._ntrip_mountpoint = StringVar()
         self._ntrip_mpdist = StringVar()
         self._ntrip_user = StringVar()
         self._ntrip_password = StringVar()
         self._ntrip_gga_interval = StringVar()
         self._ntrip_gga_mode = IntVar()
         self._ntrip_gga_lat = StringVar()
@@ -166,47 +164,51 @@
         )
 
         # NTRIP client configuration options
         self._lbl_server = Label(self._frm_container, text=LBLNTRIPSERVER)
         self._ent_server = Entry(
             self._frm_container,
             textvariable=self._ntrip_server,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=50,
         )
         self._lbl_port = Label(self._frm_container, text=LBLNTRIPPORT)
         self._ent_port = Entry(
             self._frm_container,
             textvariable=self._ntrip_port,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=6,
         )
+        self._spn_ipprot = Spinbox(
+            self._frm_container,
+            values=("IPv4", "IPv6"),
+            textvariable=self._ntrip_ipprot,
+            width=6,
+            wrap=True,
+            state=NORMAL,
+        )
         self._lbl_mountpoint = Label(self._frm_container, text=LBLNTRIPMOUNT)
         self._ent_mountpoint = Entry(
             self._frm_container,
             textvariable=self._ntrip_mountpoint,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=20,
         )
         self._lbl_mpdist = Label(
             self._frm_container,
             textvariable=self._ntrip_mpdist,
             width=30,
             anchor="w",
         )
         self._lbl_sourcetable = Label(self._frm_container, text=LBLNTRIPSTR)
         self._lbx_sourcetable = Listbox(
             self._frm_container,
-            bg=ENTCOL,
             height=4,
             relief="sunken",
             width=55,
         )
         self._scr_sourcetablev = Scrollbar(self._frm_container, orient=VERTICAL)
         self._scr_sourcetableh = Scrollbar(self._frm_container, orient=HORIZONTAL)
         self._lbx_sourcetable.config(yscrollcommand=self._scr_sourcetablev.set)
@@ -215,44 +217,40 @@
         self._scr_sourcetableh.config(command=self._lbx_sourcetable.xview)
 
         self._lbl_ntripversion = Label(self._frm_container, text=LBLNTRIPVERSION)
         self._spn_ntripversion = Spinbox(
             self._frm_container,
             values=(NTRIP_VERSIONS),
             width=4,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._ntrip_version,
             state=READONLY,
         )
         self._lbl_user = Label(self._frm_container, text=LBLNTRIPUSER)
         self._ent_user = Entry(
             self._frm_container,
             textvariable=self._ntrip_user,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=50,
         )
         self._lbl_password = Label(self._frm_container, text=LBLNTRIPPWD)
         self._ent_password = Entry(
             self._frm_container,
             textvariable=self._ntrip_password,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=20,
             show="*",
         )
         self._lbl_ntripggaint = Label(self._frm_container, text=LBLNTRIPGGAINT)
         self._spn_ntripggaint = Spinbox(
             self._frm_container,
             values=(GGA_INTERVALS),
             width=5,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._ntrip_gga_interval,
             state=READONLY,
         )
         self._rad_ggalive = Radiobutton(
             self._frm_container, text=LBLGGALIVE, variable=self._ntrip_gga_mode, value=0
         )
@@ -262,42 +260,38 @@
             variable=self._ntrip_gga_mode,
             value=1,
         )
         self._lbl_lat = Label(self._frm_container, text="Ref Latitude")
         self._ent_lat = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_lat,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
         self._lbl_lon = Label(self._frm_container, text="Ref Longitude")
         self._ent_lon = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_lon,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
         self._lbl_alt = Label(self._frm_container, text="Ref Elevation m")
         self._ent_alt = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_alt,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
         self._lbl_sep = Label(self._frm_container, text="Ref Separation m")
         self._ent_sep = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_sep,
-            bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
 
         self._btn_connect = Button(
             self._frm_container,
@@ -336,14 +330,15 @@
         )
 
         # body of grid
         self._lbl_server.grid(column=0, row=0, padx=3, pady=3, sticky=W)
         self._ent_server.grid(column=1, row=0, columnspan=2, padx=3, pady=3, sticky=W)
         self._lbl_port.grid(column=0, row=1, padx=3, pady=3, sticky=W)
         self._ent_port.grid(column=1, row=1, padx=3, pady=3, sticky=W)
+        self._spn_ipprot.grid(column=2, row=1, padx=3, pady=3, sticky=W)
         self._lbl_mountpoint.grid(column=0, row=2, padx=3, pady=3, sticky=W)
         self._ent_mountpoint.grid(column=1, row=2, padx=3, pady=3, sticky=W)
         self._lbl_mpdist.grid(column=2, row=2, padx=3, pady=3, sticky=W)
         self._lbl_sourcetable.grid(column=0, row=3, padx=3, pady=3, sticky=W)
         self._lbx_sourcetable.grid(
             column=1, row=3, columnspan=2, rowspan=4, padx=3, pady=3, sticky=W
         )
@@ -384,15 +379,15 @@
         row = 22
         col = 0
         (colsp, rowsp) = self._frm_container.grid_size()
         self._frm_status.grid(column=col, row=row, columnspan=colsp, sticky=(W, E))
         self._lbl_status.grid(
             column=0, row=0, columnspan=colsp - 1, ipadx=3, ipady=3, sticky=(W, E)
         )
-        self._btn_exit.grid(column=colsp - 1, row=0, ipadx=3, ipady=3, sticky=(E))
+        self._btn_exit.grid(column=colsp - 1, row=0, ipadx=3, ipady=3, sticky=E)
 
         for frm in (self._frm_container, self._frm_status):
             for i in range(colsp):
                 frm.grid_columnconfigure(i, weight=1)
             for i in range(rowsp):
                 frm.grid_rowconfigure(i, weight=1)
 
@@ -410,52 +405,58 @@
         """
         Reset configuration widgets.
         """
 
         self._get_settings()
         self.set_controls(self._connected)
 
-    def set_controls(self, connected: bool, msg: tuple = None):
+    def set_controls(self, connected: bool, msgt: tuple = None):
         """
         Enable or disable controls depending on connection status.
 
         :param bool status: connection status (True/False)
-        :param tuple msg: optional status message tuple (text, color)
+        :param tuple msgt: tuple of (message, color)
         """
 
         try:
-
             self._settings = self.__app.ntrip_handler.settings
             self._connected = connected
-            if msg is None:
+            if msgt is None:
                 server = self._settings["server"]
                 port = self._settings["port"]
-                mountpoint = "/" + self._settings["mountpoint"]
+                mp = self._settings["mountpoint"]
+                if mp is None:
+                    mp = ""
+                mountpoint = "/" + mp
                 if mountpoint == "/":
                     mountpoint = " - retrieving sourcetable..."
                 msg = (
-                    (f"Connected to {server}:{port}{mountpoint}", "green")
+                    f"Connected to {server}:{port}{mountpoint}"
                     if self._connected
-                    else ("Disconnected", "blue")
+                    else "Disconnected"
                 )
-            txt, col = msg
-            self.set_status(txt, col)
+            if msgt is None:
+                self.set_status(msg, "blue")
+            else:
+                msg, col = msgt
+                self.set_status(msg, col)
 
             self._btn_disconnect.config(state=(NORMAL if connected else DISABLED))
 
             for ctl in (
                 self._spn_ntripversion,
                 self._spn_ntripggaint,
             ):
                 ctl.config(state=(DISABLED if connected else READONLY))
 
             for ctl in (
                 self._btn_connect,
                 self._ent_server,
                 self._ent_port,
+                self._spn_ipprot,
                 self._ent_mountpoint,
                 self._ent_user,
                 self._ent_password,
                 self._ent_lat,
                 self._ent_lon,
                 self._ent_alt,
                 self._ent_sep,
@@ -475,24 +476,25 @@
                     self._settings["sourcetable"],
                     self._settings["mountpoint"],
                 )
                 self.set_mp_dist(mindist, mpname)
         except TclError:  # fudge during thread termination
             pass
 
-    def set_status(self, message: str, color: str = "blue"):
+    def set_status(self, message: str, color: str = ""):
         """
         Set status message.
 
         :param str message: message to be displayed
-        :param str color: rgb color of text (blue)
+        :param str color: rgb color of text
         """
 
-        message = (message[:80] + "..") if len(message) > 80 else message
-        self._lbl_status.config(fg=color)
+        message = f"{message[:78]}.." if len(message) > 80 else message
+        if color != "":
+            self._lbl_status.config(fg=color)
         self._status.set(" " + message)
 
     def _on_select_mp(self, event):
         """
         Mountpoint has been selected from listbox; set
         mountpoint and distance from live or reference
         coordinates (if available).
@@ -517,16 +519,15 @@
             pass
 
     def on_exit(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Handle Exit button press.
         """
 
-        # self.__master.update_idletasks()
-        self.__app.stop_ntripconfig_thread()
+        self.__app.stop_dialog(DLGTNTRIP)
         self.destroy()
 
     def get_size(self):
         """
         Get current frame size.
 
         :return: window size (width, height)
@@ -539,20 +540,22 @@
     def _get_settings(self):
         """
         Get settings from NTRIP handler.
         """
 
         self._connected = self.__app.ntrip_handler.connected
         self._settings = self.__app.ntrip_handler.settings
+        ipprot = self._settings.get("ipprot", AF_INET)
+        self._ntrip_ipprot.set("IPv6" if ipprot == AF_INET6 else "IPv4")
         self._ntrip_server.set(self._settings["server"])
         self._ntrip_port.set(self._settings["port"])
         self._ntrip_mountpoint.set(self._settings["mountpoint"])
         self._ntrip_version.set(self._settings["version"])
-        self._ntrip_user.set(self._settings["user"])
-        self._ntrip_password.set(self._settings["password"])
+        self._ntrip_user.set(self._settings["ntripuser"])
+        self._ntrip_password.set(self._settings["ntrippassword"])
         ggaint = self._settings["ggainterval"]
         self._ntrip_gga_interval.set("None" if ggaint == NOGGA else ggaint)
         self._ntrip_gga_mode.set(self._settings["ggamode"])
         self._ntrip_gga_lat.set(self._settings["reflat"])
         self._ntrip_gga_lon.set(self._settings["reflon"])
         self._ntrip_gga_alt.set(self._settings["refalt"])
         self._ntrip_gga_sep.set(self._settings["refsep"])
@@ -564,20 +567,23 @@
         self.set_mp_dist(mindist, mpname)
 
     def _set_settings(self):
         """
         Set settings for NTRIP handler.
         """
 
+        self._settings["ipprot"] = (
+            AF_INET6 if self._ntrip_ipprot.get() == "IPv6" else AF_INET
+        )
         self._settings["server"] = self._ntrip_server.get()
         self._settings["port"] = self._ntrip_port.get()
         self._settings["mountpoint"] = self._ntrip_mountpoint.get()
         self._settings["version"] = self._ntrip_version.get()
-        self._settings["user"] = self._ntrip_user.get()
-        self._settings["password"] = self._ntrip_password.get()
+        self._settings["ntripuser"] = self._ntrip_user.get()
+        self._settings["ntrippassword"] = self._ntrip_password.get()
         self._settings["ggainterval"] = (
             NOGGA
             if self._ntrip_gga_interval.get() == "None"
             else self._ntrip_gga_interval.get()
         )
         self._settings["ggamode"] = self._ntrip_gga_mode.get()
         self._settings["reflat"] = self._ntrip_gga_lat.get()
@@ -603,38 +609,41 @@
         Connect to NTRIP Server. NTRIP handler will invoke set_controls()
         with connection status in due course.
         """
 
         if self._valid_settings():
             self._set_settings()
             self.__app.ntrip_handler.run(
+                ipprot="IPv6" if self._settings["ipprot"] == AF_INET6 else "IPv4",
                 server=self._settings["server"],
                 port=self._settings["port"],
                 mountpoint=self._settings["mountpoint"],
                 version=self._settings["version"],
-                user=self._settings["user"],
-                password=self._settings["password"],
+                ntripuser=self._settings["ntripuser"],
+                ntrippassword=self._settings["ntrippassword"],
                 ggainterval=self._settings["ggainterval"],
                 ggamode=self._settings["ggamode"],
                 reflat=self._settings["reflat"],
                 reflon=self._settings["reflon"],
                 refalt=self._settings["refalt"],
                 refsep=self._settings["refsep"],
-                output=self.__app.ntripqueue,
+                output=self.__app.ntrip_inqueue,
             )
             self.set_controls(True)
+            self.__app.rtk_conn_status = CONNECTED_NTRIP
 
     def _disconnect(self):
         """
         Disconnect from NTRIP Server. NTRIP handler will invoke set_controls()
         with connection status in due course.
         """
 
         self.__app.ntrip_handler.stop()
         self.set_controls(False)
+        self.__app.rtk_conn_status = DISCONNECTED
 
     def _valid_settings(self) -> bool:
         """
         Validate settings.
 
         :return: valid True/False
         :rtype: bool
@@ -657,20 +666,21 @@
     def set_mp_dist(self, dist: float, name: str = ""):
         """
         Set mountpoint distance label.
 
         :param float dist: distance to mountpoint km
         """
 
+        settings = self.__app.frm_settings.config
         if name in (None, ""):
             return
         dist_l = "Distance n/a"
         dist_u = "km"
         if isinstance(dist, float):
-            units = self.__app.frm_settings.units
+            units = settings["units"]
             if units in (UI, UIK):
                 dist *= KM2MILES
                 dist_u = "miles"
             dist_l = f"Distance {dist:,.1f} {dist_u}"
 
         self._ntrip_mountpoint.set(name)
         self._ntrip_mpdist.set(dist_l)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/binary-1-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/binary-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/clear-1-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/clear-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/ethernet-1-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/ethernet-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-check-mark-8-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-check-mark-8-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-gear-2-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-gear-2-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-location-27-32.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-location-27-32.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-noclient-10-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-noclient-10-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-time-6-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-time-6-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-transmit-10-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/iconmonstr-transmit-10-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/pygpsclient.ico` & `pygpsclient-1.4.0/src/pygpsclient/resources/pygpsclient.ico`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/usbport-1-24.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/usbport-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/resources/world.png` & `pygpsclient-1.4.0/src/pygpsclient/resources/world.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.9/pygpsclient/rtcm3_handler.py` & `pygpsclient-1.4.0/src/pygpsclient/rtcm3_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
-RTCM3 Protocol handler - handles all incoming RTCM3 messages
+rtcm3_handler.py
 
-THIS IS JUST A STUB FOR NOW AS THERE'S CURRENTLY NO NEED
-TO PROCESS RTCM3 DATA TO UPDATE THE GUI
+RTCM Protocol handler - handles all incoming RTCM messages.
 
-Uses pyrtcm library for parsing
+Parses individual RTCM3 sentences (using pyrtcm library).
 
 Created on 10 Apr 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 
 class RTCM3Handler:
     """
     RTCM3 handler class.
     """
 
@@ -24,15 +22,15 @@
         """
         Constructor.
 
         :param Frame app: reference to main tkinter application
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
         self._raw_data = None
         self._parsed_data = None
 
     def process_data(self, raw_data: bytes, parsed_data: object):
         """
         Process relevant RTCM message types
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/serialconfig_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/serialconfig_frame.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,52 +11,55 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
 from tkinter import (
+    DISABLED,
+    HORIZONTAL,
+    LEFT,
+    NORMAL,
+    VERTICAL,
+    Button,
+    Checkbutton,
+    DoubleVar,
+    E,
     Frame,
+    IntVar,
+    Label,
     Listbox,
+    N,
+    S,
     Scrollbar,
     Spinbox,
-    Checkbutton,
-    Button,
-    Label,
-    IntVar,
-    DoubleVar,
     StringVar,
-    N,
-    S,
-    E,
     W,
-    LEFT,
-    VERTICAL,
-    HORIZONTAL,
-    NORMAL,
-    DISABLED,
 )
-from PIL import ImageTk, Image
+
+from PIL import Image, ImageTk
+from serial import PARITY_EVEN, PARITY_MARK, PARITY_NONE, PARITY_ODD, PARITY_SPACE
 from serial.tools.list_ports import comports
-from serial import PARITY_NONE, PARITY_EVEN, PARITY_ODD, PARITY_MARK, PARITY_SPACE
-from pygpsclient.globals import ICON_REFRESH, ICON_EXPAND, ICON_CONTRACT
+
+from pygpsclient.globals import ICON_CONTRACT, ICON_EXPAND, ICON_REFRESH, MSGMODES
+from pygpsclient.strings import LBLUDPORT
 
 ADVOFF = "\u25bc"
 ADVON = "\u25b2"
 READONLY = "readonly"
 PARITIES = {
     "None": PARITY_NONE,
     "Even": PARITY_EVEN,
     "Odd": PARITY_ODD,
     "Mark": PARITY_MARK,
     "Space": PARITY_SPACE,
 }
 # These ranges can be overridden via keyword arguments:
 # (the default value will be the first in the range)
-BPSRATE_RNG = (9600, 19200, 38400, 57600, 115200, 4800)
+BPSRATE_RNG = (9600, 19200, 38400, 57600, 115200, 1000000, 4800)
 DATABITS_RNG = (8, 5, 6, 7)
 STOPBITS_RNG = (1, 1.5, 2)
 PARITY_RNG = list(PARITIES.keys())
 TIMEOUT_RNG = ("None", "0", "1", "2", "5", "10", "20")
 BGCOL = "azure"
 DISCONNECTED = 0
 CONNECTED = 1
@@ -74,21 +77,22 @@
         Constructor.
 
         :param tkinter.Frame container: reference to container frame
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs for value ranges, or to pass to Frame parent class
         """
 
+        self._userport = kwargs.pop("userport", "")  # user-defined port
         self._bpsrate_rng = kwargs.pop("bpsrates", BPSRATE_RNG)
         self._databits_rng = kwargs.pop("databits", DATABITS_RNG)
         self._stopbits_rng = kwargs.pop("stopbits", STOPBITS_RNG)
         self._parity_rng = kwargs.pop("parities", PARITY_RNG)
         self._timeout_rng = kwargs.pop("timeouts", TIMEOUT_RNG)
+        self._msgmode_rng = kwargs.pop("msgmodes", ())
         self._preselect = kwargs.pop("preselect", ())
-        self._readonlybg = kwargs.pop("readonlybackground", BGCOL)
 
         Frame.__init__(self, container, *args, **kwargs)
 
         self._show_advanced = False
         self._status = DISCONNECTED
         self._ports = ()
         self._port = StringVar()
@@ -96,14 +100,15 @@
         self._bpsrate = IntVar()
         self._databits = IntVar()
         self._stopbits = DoubleVar()
         self._parity = StringVar()
         self._rtscts = IntVar()
         self._xonxoff = IntVar()
         self._timeout = StringVar()
+        self._msgmode = StringVar()
         self._img_refresh = ImageTk.PhotoImage(Image.open(ICON_REFRESH))
         self._img_expand = ImageTk.PhotoImage(Image.open(ICON_EXPAND))
         self._img_contract = ImageTk.PhotoImage(Image.open(ICON_CONTRACT))
 
         self._body()
         self._do_layout()
         self._get_ports()
@@ -117,15 +122,14 @@
 
         self._frm_basic = Frame(self)
         self._lbl_port = Label(self._frm_basic, text="Serial\nPort  ")
         self._lbx_port = Listbox(
             self._frm_basic,
             border=2,
             relief="sunken",
-            bg=self._readonlybg,
             width=32,
             height=5,
             justify=LEFT,
             exportselection=False,
         )
         self._scr_portv = Scrollbar(self._frm_basic, orient=VERTICAL)
         self._scr_porth = Scrollbar(self._frm_basic, orient=HORIZONTAL)
@@ -135,15 +139,14 @@
         self._scr_porth.config(command=self._lbx_port.xview)
         self._lbl_bpsrate = Label(self._frm_basic, text="Rate bps")
         self._spn_bpsrate = Spinbox(
             self._frm_basic,
             values=self._bpsrate_rng,
             width=8,
             state=READONLY,
-            readonlybackground=self._readonlybg,
             wrap=True,
             textvariable=self._bpsrate,
         )
         self._btn_refresh = Button(
             self._frm_basic,
             command=self._on_refresh,
             image=self._img_refresh,
@@ -161,35 +164,32 @@
         self._frm_advanced = Frame(self)
         self._lbl_databits = Label(self._frm_advanced, text="Data Bits")
         self._spn_databits = Spinbox(
             self._frm_advanced,
             values=self._databits_rng,
             width=3,
             state=READONLY,
-            readonlybackground=self._readonlybg,
             wrap=True,
             textvariable=self._databits,
         )
         self._lbl_stopbits = Label(self._frm_advanced, text="Stop Bits")
         self._spn_stopbits = Spinbox(
             self._frm_advanced,
             values=self._stopbits_rng,
             width=3,
             state=READONLY,
-            readonlybackground=self._readonlybg,
             wrap=True,
             textvariable=self._stopbits,
         )
         self._lbl_parity = Label(self._frm_advanced, text="Parity")
         self._spn_parity = Spinbox(
             self._frm_advanced,
             values=self._parity_rng,
             width=6,
             state=READONLY,
-            readonlybackground=self._readonlybg,
             wrap=True,
             textvariable=self._parity,
         )
         self._chk_rts = Checkbutton(
             self._frm_advanced, text="RTS/CTS", variable=self._rtscts
         )
         self._chk_xon = Checkbutton(
@@ -197,89 +197,107 @@
         )
         self._lbl_timeout = Label(self._frm_advanced, text="Timeout (s)")
         self._spn_timeout = Spinbox(
             self._frm_advanced,
             values=self._timeout_rng,
             width=4,
             state=READONLY,
-            readonlybackground=self._readonlybg,
             wrap=True,
             textvariable=self._timeout,
         )
+        self._lbl_msgmode = Label(self._frm_advanced, text="Msg Mode")
+        self._spn_msgmode = Spinbox(
+            self._frm_advanced,
+            values=self._msgmode_rng,
+            width=4,
+            state=READONLY,
+            wrap=True,
+            textvariable=self._msgmode,
+        )
 
     def _do_layout(self):
         """
         Layout widgets.
         """
 
         self._frm_basic.grid(column=0, row=0, columnspan=4, sticky=(W, E))
-        self._lbl_port.grid(column=0, row=0, sticky=(W))
+        self._lbl_port.grid(column=0, row=0, sticky=W)
         self._lbx_port.grid(
             column=1, row=0, columnspan=2, sticky=(W, E), padx=3, pady=2
         )
         self._scr_portv.grid(column=3, row=0, sticky=(N, S))
         self._scr_porth.grid(column=1, row=1, columnspan=2, sticky=(E, W))
-        self._lbl_bpsrate.grid(column=0, row=2, sticky=(W))
-        self._spn_bpsrate.grid(column=1, row=2, sticky=(W), padx=3, pady=2)
-        self._btn_refresh.grid(column=2, row=2, sticky=(E))
-        self._btn_toggle.grid(column=3, row=2, sticky=(E))
+        self._lbl_bpsrate.grid(column=0, row=2, sticky=W)
+        self._spn_bpsrate.grid(column=1, row=2, sticky=W, padx=3, pady=2)
+        self._btn_refresh.grid(column=2, row=2, sticky=E)
+        self._btn_toggle.grid(column=3, row=2, sticky=E)
 
         self._frm_advanced.grid_forget()
-        self._lbl_databits.grid(column=0, row=0, sticky=(W))
-        self._spn_databits.grid(column=1, row=0, sticky=(W), padx=3, pady=2)
-        self._lbl_stopbits.grid(column=2, row=0, sticky=(W))
-        self._spn_stopbits.grid(column=3, row=0, sticky=(W), padx=3, pady=2)
-        self._lbl_parity.grid(column=0, row=1, sticky=(W))
-        self._spn_parity.grid(column=1, row=1, sticky=(W), padx=3, pady=2)
-        self._chk_rts.grid(column=2, row=1, sticky=(W))
-        self._chk_xon.grid(column=3, row=1, sticky=(W), padx=3, pady=2)
-        self._lbl_timeout.grid(column=0, row=2, sticky=(W))
-        self._spn_timeout.grid(column=1, row=2, sticky=(W), padx=3, pady=2)
+        self._lbl_databits.grid(column=0, row=0, sticky=W)
+        self._spn_databits.grid(column=1, row=0, sticky=W, padx=3, pady=2)
+        self._lbl_stopbits.grid(column=2, row=0, sticky=W)
+        self._spn_stopbits.grid(column=3, row=0, sticky=W, padx=3, pady=2)
+        self._lbl_parity.grid(column=0, row=1, sticky=W)
+        self._spn_parity.grid(column=1, row=1, sticky=W, padx=3, pady=2)
+        self._chk_rts.grid(column=2, row=1, sticky=W)
+        self._chk_xon.grid(column=3, row=1, sticky=W, padx=3, pady=2)
+        self._lbl_timeout.grid(column=0, row=2, sticky=W)
+        self._spn_timeout.grid(column=1, row=2, sticky=W, padx=3, pady=2)
+        if len(self._msgmode_rng) > 0:
+            self._lbl_msgmode.grid(column=2, row=2, sticky=W)
+            self._spn_msgmode.grid(column=3, row=2, sticky=W, padx=3, pady=2)
 
     def _attach_events(self):
         """
         Bind events to widgets.
         """
 
         self._lbx_port.bind("<<ListboxSelect>>", self._on_select_port)
 
     def _get_ports(self):
         """
         Populate list of available serial ports using pyserial comports tool.
 
+        User-defined serial port can be passed as command line keyword argument,
+        in which case this takes precedence.
+
         Attempt to automatically select a serial device matching
         a list of 'preselect' devices (only works on platforms
         which parse UART device desc or HWID e.g. Posix).
         """
 
         self._ports = sorted(comports())
         init_idx = 0
+        recognised = False
+        if self._userport != "":
+            self._ports.insert(0, (self._userport, LBLUDPORT, None))
 
-        port = ""
-        desc = ""
         if len(self._ports) > 0:
-            # default selection to first port
-            (port, desc, _) = self._ports[0]
+            # default to first item in list
+            port, desc, _ = self._ports[0]
+            if desc == "":
+                desc = "device"
             self._port.set(port)
             self._port_desc.set(desc)
             for idx, (port, desc, _) in enumerate(self._ports):
                 self._lbx_port.insert(idx, port + ": " + desc)
-                for dev in self._preselect:
-                    if dev in desc:
-                        # update selection to recognised GNSS device
-                        init_idx = idx
-                        self._port.set(port)
-                        self._port_desc.set(desc)
-
-                        break
+                # default selection to recognised GNSS device if possible
+                if not recognised:
+                    for dev in self._preselect:
+                        if dev in desc:
+                            init_idx = idx
+                            self._port.set(port)
+                            self._port_desc.set(desc)
+                            recognised = True
+                            break
             self.set_status(DISCONNECTED)
+            self._lbx_port.activate(init_idx)
+            self._lbx_port.selection_set(first=init_idx)
         else:
             self.set_status(NOPORTS)
-        self._lbx_port.activate(init_idx)
-        self._lbx_port.selection_set(first=init_idx)
 
     def _on_select_port(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Get selected port from listbox and set global variable.
         """
 
         idx = self._lbx_port.curselection()
@@ -333,22 +351,24 @@
             self._lbl_databits,
             self._lbl_stopbits,
             self._lbl_parity,
             self._lbl_timeout,
             self._chk_rts,
             self._chk_xon,
             self._lbx_port,
+            self._lbl_msgmode,
         ):
             widget.configure(state=(NORMAL if status == DISCONNECTED else DISABLED))
         for widget in (
             self._spn_bpsrate,
             self._spn_databits,
             self._spn_stopbits,
             self._spn_parity,
             self._spn_timeout,
+            self._spn_msgmode,
         ):
             widget.configure(state=(READONLY if status == DISCONNECTED else DISABLED))
 
     def reset(self):
         """
         Reset settings to defaults (first value in range).
         """
@@ -356,14 +376,15 @@
         self._bpsrate.set(self._bpsrate_rng[0])
         self._databits.set(self._databits_rng[0])
         self._stopbits.set(self._stopbits_rng[0])
         self._parity.set(self._parity_rng[0])
         self._rtscts.set(False)
         self._xonxoff.set(False)
         self._timeout.set(self._timeout_rng[0])
+        self._msgmode.set("GET")
 
     @property
     def status(self) -> int:
         """
         Getter for status flag: 0=DISCONNECTED, 1=CONNECTED,
         2=CONNECTED_FILE, 3=NOPORTS.
 
@@ -469,7 +490,19 @@
         :return: selected timeout
         :rtype: float (or None)
         """
 
         if self._timeout.get() == "None":
             return None
         return float(self._timeout.get())
+
+    @property
+    def msgmode(self) -> int:
+        """
+        Return message parsing mode
+        Default is GET i.e. input from receiver.
+
+        :return: message mode 0 = POLL 1 = SET, 2 = POLL
+        :rtype: int
+        """
+
+        return MSGMODES[self._msgmode.get()]
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/settings_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/settings_frame.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,100 @@
 """
+settings_frame.py
+
 Settings frame class for PyGPSClient application.
 
 This handles the settings/configuration panel. It references
-the common SerialConfigFrame utility class for serial port settings.
+the SerialConfigFrame class for serial port settings
+and the SocketConfigFrame class for socket settings.
 
 Exposes the various settings as properties.
 
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name, unnecessary-lambda, too-many-instance-attributes
+# pylint: disable=unnecessary-lambda
 
+from os import getenv
 from tkinter import (
-    ttk,
-    Frame,
+    DISABLED,
+    NORMAL,
     Button,
+    Checkbutton,
+    E,
+    Frame,
+    IntVar,
     Label,
-    Entry,
     Spinbox,
-    Scale,
-    Checkbutton,
     StringVar,
-    IntVar,
-    N,
-    S,
-    E,
     W,
-    NORMAL,
-    DISABLED,
-    HORIZONTAL,
+    ttk,
 )
 
-from PIL import ImageTk, Image
 import pyubx2.ubxtypes_core as ubt
-from pygpsclient.serialconfig_frame import SerialConfigFrame
-from pygpsclient.socketconfig_frame import SocketConfigFrame
+from PIL import Image, ImageTk
+
 from pygpsclient.globals import (
-    ENTCOL,
-    DDD,
-    DMM,
-    DMS,
-    UMM,
-    UMK,
-    UI,
-    UIK,
-    READONLY,
+    BADCOL,
+    BPSRATES,
     CONNECTED,
-    CONNECTED_SOCKET,
     CONNECTED_FILE,
+    CONNECTED_SOCKET,
+    DDD,
     DISCONNECTED,
-    NOPORTS,
+    DLGTNTRIP,
+    DLGTSPARTN,
+    DLGTUBX,
+    DMM,
+    DMS,
+    ECEF,
+    FORMATS,
+    GNSS_EOF_EVENT,
+    GNSS_ERR_EVENT,
+    GNSS_EVENT,
     ICON_CONN,
+    ICON_DISCONN,
+    ICON_EXIT,
+    ICON_LOGREAD,
+    ICON_NTRIPCONFIG,
     ICON_SERIAL,
     ICON_SOCKET,
-    ICON_DISCONN,
+    ICON_SPARTNCONFIG,
     ICON_UBXCONFIG,
-    ICON_NTRIPCONFIG,
-    ICON_LOGREAD,
     KNOWNGPS,
-    BPSRATES,
-    FORMATS,
+    MSGMODES,
+    NOPORTS,
+    READONLY,
     SOCKMODES,
-    TAG_COLORS,
+    SOCKSERVER_HOST,
     SOCKSERVER_PORT,
-    SOCKSERVER_NTRIP_PORT,
-    SOCKSERVER_MAX_CLIENTS,
+    TIMEOUTS,
+    UI,
+    UIK,
+    UMK,
+    UMM,
 )
-from pygpsclient.helpers import valid_entry, VALINT, VALURL, MAXPORT
+from pygpsclient.helpers import MAXPORT, VALINT, VALURL, valid_entry
+from pygpsclient.serialconfig_frame import SerialConfigFrame
+from pygpsclient.serverconfig_frame import ServerConfigFrame
+from pygpsclient.socketconfig_frame import SocketConfigFrame
 from pygpsclient.strings import (
-    LBLUBXCONFIG,
-    LBLNTRIPCONFIG,
-    LBLPROTDISP,
+    CONFIGERR,
     LBLDATADISP,
     LBLDATALOG,
-    LBLTRACKRECORD,
-    LBLSHOWUNUSED,
-    LBLLEGEND,
-    LBLSOCKSERVE,
-    LBLSERVERPORT,
     LBLDEGFORMAT,
-    LBLSERVERMODE,
-)
-
-TIMEOUTS = (
-    "0.1",
-    "0.2",
-    "1",
-    "2",
-    "5",
-    "10",
-    "20",
-    "None",
-    "0",
+    LBLNTRIPCONFIG,
+    LBLPROTDISP,
+    LBLSHOWUNUSED,
+    LBLSPARTNCONFIG,
+    LBLTRACKRECORD,
+    LBLUBXCONFIG,
 )
 
 
 class SettingsFrame(Frame):
     """
     Settings frame class.
     """
@@ -109,47 +105,45 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         Frame.__init__(self, self.__master, *args, **kwargs)
 
+        self.infilepath = None
+        self.outfilepath = None
         self._prot_nmea = IntVar()
         self._prot_ubx = IntVar()
         self._prot_rtcm3 = IntVar()
         self._autoscroll = IntVar()
         self._maxlines = IntVar()
-        self._webmap = IntVar()
-        self._mapzoom = IntVar()
+        self.maptype = StringVar()
+        self.mapzoom = IntVar()
         self._units = StringVar()
-        self._format = StringVar()
+        self._degrees_format = StringVar()
+        self._console_format = StringVar()
         self._datalog = IntVar()
         self._logformat = StringVar()
         self._record_track = IntVar()
         self._show_unusedsat = IntVar()
-        self._show_legend = IntVar()
-        self._colortags = IntVar()
-        self._socket_serve = IntVar()
-        self._sock_port = StringVar()
-        self._sock_mode = StringVar()
-        self._sock_clients = StringVar()
+        self.show_legend = IntVar()
+        self._colortag = IntVar()
         self._validsettings = True
-        self._in_filepath = None
-        self._logpath = None
         self._trackpath = None
-        self._display_format = StringVar()
         self._img_conn = ImageTk.PhotoImage(Image.open(ICON_CONN))
         self._img_serial = ImageTk.PhotoImage(Image.open(ICON_SERIAL))
         self._img_socket = ImageTk.PhotoImage(Image.open(ICON_SOCKET))
         self._img_disconn = ImageTk.PhotoImage(Image.open(ICON_DISCONN))
+        self._img_exit = ImageTk.PhotoImage(Image.open(ICON_EXIT))
         self._img_ubxconfig = ImageTk.PhotoImage(Image.open(ICON_UBXCONFIG))
         self._img_ntripconfig = ImageTk.PhotoImage(Image.open(ICON_NTRIPCONFIG))
+        self._img_spartnconfig = ImageTk.PhotoImage(Image.open(ICON_SPARTNCONFIG))
         self._img_dataread = ImageTk.PhotoImage(Image.open(ICON_LOGREAD))
 
         self._body()
         self._do_layout()
         self._reset()
 
     def _body(self):
@@ -160,56 +154,70 @@
         for i in range(4):
             self.grid_columnconfigure(i, weight=1)
         self.grid_rowconfigure(0, weight=1)
 
         self.option_add("*Font", self.__app.font_sm)
 
         # serial port configuration panel
-        self._frm_serial = SerialConfigFrame(
-            self, preselect=KNOWNGPS, timeouts=TIMEOUTS, bpsrates=BPSRATES
+        userport = self.__app.app_config.get("userport", "")
+        self.frm_serial = SerialConfigFrame(
+            self,
+            preselect=KNOWNGPS,
+            timeouts=TIMEOUTS,
+            bpsrates=BPSRATES,
+            msgmodes=list(MSGMODES.keys()),
+            userport=userport,  # user-defined serial port
         )
 
         # socket configuration panel
-        self._frm_socket = SocketConfigFrame(self)
+        self.frm_socket = SocketConfigFrame(self)
 
         # connection buttons
         self._frm_buttons = Frame(self)
         self._btn_connect = Button(
             self._frm_buttons,
             width=45,
             height=35,
             image=self._img_serial,
-            command=lambda: self._on_serial_stream(),
+            command=lambda: self._on_connect(CONNECTED),
         )
         self._lbl_connect = Label(self._frm_buttons, text="USB/UART")
         self._btn_connect_socket = Button(
             self._frm_buttons,
             width=45,
             height=35,
             image=self._img_socket,
-            command=lambda: self._on_socket_stream(),
+            command=lambda: self._on_connect(CONNECTED_SOCKET),
         )
         self._lbl_connect_socket = Label(self._frm_buttons, text="TCP/UDP")
         self._btn_connect_file = Button(
             self._frm_buttons,
             width=45,
             height=35,
             image=self._img_dataread,
-            command=lambda: self._on_file_stream(),
+            command=lambda: self._on_connect(CONNECTED_FILE),
         )
         self._lbl_connect_file = Label(self._frm_buttons, text="FILE")
         self._btn_disconnect = Button(
             self._frm_buttons,
             width=45,
             height=35,
             image=self._img_disconn,
-            command=lambda: self._on_disconnect(),
+            command=lambda: self._on_connect(DISCONNECTED),
             state=DISABLED,
         )
         self._lbl_disconnect = Label(self._frm_buttons, text="STOP")
+        self._btn_exit = Button(
+            self._frm_buttons,
+            width=45,
+            height=35,
+            image=self._img_exit,
+            command=lambda: self.__app.quit(),
+        )
+
         self._lbl_status_preset = Label(
             self._frm_buttons, font=self.__app.font_md2, text=""
         )
 
         # Other configuration options
         self._frm_options = Frame(self)
         self._lbl_protocol = Label(self._frm_options, text=LBLPROTDISP)
@@ -230,432 +238,343 @@
         )
         self._lbl_consoledisplay = Label(self._frm_options, text=LBLDATADISP)
         self._spn_conformat = Spinbox(
             self._frm_options,
             values=FORMATS,
             width=10,
             state=READONLY,
-            readonlybackground=ENTCOL,
             wrap=True,
-            textvariable=self._display_format,
+            textvariable=self._console_format,
         )
         self._chk_tags = Checkbutton(
             self._frm_options,
             text="Tags",
-            variable=self._colortags,
+            variable=self._colortag,
         )
         self._lbl_format = Label(self._frm_options, text=LBLDEGFORMAT)
         self._spn_format = Spinbox(
             self._frm_options,
-            values=(DDD, DMS, DMM),
+            values=(DDD, DMS, DMM, ECEF),
             width=6,
             state=READONLY,
-            readonlybackground=ENTCOL,
             wrap=True,
-            textvariable=self._format,
+            textvariable=self._degrees_format,
         )
         self._lbl_units = Label(self._frm_options, text="Units")
         self._spn_units = Spinbox(
             self._frm_options,
             values=(UMM, UIK, UI, UMK),
             width=13,
             state=READONLY,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._units,
         )
         self._chk_scroll = Checkbutton(
             self._frm_options, text="Autoscroll", variable=self._autoscroll
         )
         self._spn_maxlines = Spinbox(
             self._frm_options,
             values=("100", "200", "500", "1000", "2000"),
             width=6,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._maxlines,
             state=READONLY,
         )
-        self._chk_webmap = Checkbutton(
+        self._lbl_maptype = Label(self._frm_options, text="Map Type")
+        self.spn_maptype = Spinbox(
             self._frm_options,
-            text="Web Map",
-            variable=self._webmap,
-            command=lambda: self._on_webmap(),
-        )
-        self._lbl_mapzoom = Label(self._frm_options, text="Zoom")
-        self._scl_mapzoom = Scale(
-            self._frm_options,
-            from_=1,
-            to=20,
-            orient=HORIZONTAL,
-            relief="sunken",
-            bg=ENTCOL,
-            variable=self._mapzoom,
+            values=("world", "map", "sat"),
+            width=6,
+            wrap=True,
+            textvariable=self.maptype,
+            state=READONLY,
         )
         self._chk_unusedsat = Checkbutton(
             self._frm_options, text=LBLSHOWUNUSED, variable=self._show_unusedsat
         )
-        self._chk_legend = Checkbutton(
-            self._frm_options, text=LBLLEGEND, variable=self._show_legend
-        )
         self._chk_datalog = Checkbutton(
             self._frm_options,
             text=LBLDATALOG,
             variable=self._datalog,
             command=lambda: self._on_data_log(),
         )
         self._spn_datalog = Spinbox(
             self._frm_options,
             values=(FORMATS),
             width=20,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._logformat,
             state=READONLY,
         )
         self._chk_recordtrack = Checkbutton(
             self._frm_options,
             text=LBLTRACKRECORD,
             variable=self._record_track,
             command=lambda: self._on_record_track(),
         )
         # socket server configuration
-        self._chk_socketserve = Checkbutton(
-            self._frm_options,
-            text=LBLSOCKSERVE,
-            variable=self._socket_serve,
-            command=lambda: self._on_socket_serve(),
-            state=DISABLED,
-        )
-        self._lbl_sockmode = Label(
-            self._frm_options,
-            text=LBLSERVERMODE,
-            state=DISABLED,
-        )
-        self._spn_sockmode = Spinbox(
-            self._frm_options,
-            values=SOCKMODES,
-            width=18,
-            state=DISABLED,
-            readonlybackground=ENTCOL,
-            wrap=True,
-            textvariable=self._sock_mode,
-            command=lambda: self._on_sockmode(),
-        )
-        self._lbl_sockport = Label(
-            self._frm_options,
-            text=LBLSERVERPORT,
-            state=DISABLED,
-        )
-        self._ent_sockport = Entry(
+        self.frm_server = ServerConfigFrame(self.__app, self._frm_options)
+        # configuration panel buttons
+        self._lbl_ubxconfig = Label(
             self._frm_options,
-            textvariable=self._sock_port,
-            bg=ENTCOL,
-            relief="sunken",
-            width=6,
-            state=DISABLED,
+            text=LBLUBXCONFIG,
         )
-        self._lbl_sockclients = Label(
-            self._frm_options,
-            textvariable=self._sock_clients,
-            state=DISABLED,
-        )
-        # configuration panel buttons
-        self._lbl_ubxconfig = Label(self._frm_options, text=LBLUBXCONFIG)
         self._btn_ubxconfig = Button(
             self._frm_options,
             width=45,
-            height=35,
-            text="UBX",
             image=self._img_ubxconfig,
             command=lambda: self._on_ubx_config(),
-            state=NORMAL,
         )
-        self._lbl_ntripconfig = Label(self._frm_options, text=LBLNTRIPCONFIG)
+        self._lbl_ntripconfig = Label(
+            self._frm_options,
+            text=LBLNTRIPCONFIG,
+        )
         self._btn_ntripconfig = Button(
             self._frm_options,
             width=45,
-            height=35,
-            text="NTRIP",
             image=self._img_ntripconfig,
             command=lambda: self._on_ntrip_config(),
-            state=NORMAL,
+        )
+        self._lbl_spartnconfig = Label(
+            self._frm_options,
+            text=LBLSPARTNCONFIG,
+        )
+        self._btn_spartnconfig = Button(
+            self._frm_options,
+            width=45,
+            image=self._img_spartnconfig,
+            command=lambda: self._on_spartn_config(),
         )
 
     def _do_layout(self):
         """
         Position widgets in frame.
         """
 
-        self._frm_serial.grid(
+        self.frm_serial.grid(
             column=0, row=1, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
         ttk.Separator(self).grid(
             column=0, row=2, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
 
-        self._frm_socket.grid(
+        self.frm_socket.grid(
             column=0, row=3, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
         ttk.Separator(self).grid(
             column=0, row=4, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
 
         self._frm_buttons.grid(column=0, row=5, columnspan=4, sticky=(W, E))
         self._btn_connect.grid(column=0, row=0, padx=2, pady=1)
         self._btn_connect_socket.grid(column=1, row=0, padx=2, pady=1)
         self._btn_connect_file.grid(column=2, row=0, padx=2, pady=1)
         self._btn_disconnect.grid(column=3, row=0, padx=2, pady=1)
+        self._btn_exit.grid(column=4, row=0, padx=2, pady=1)
         self._lbl_connect.grid(column=0, row=1, padx=1, pady=1, sticky=(W, E))
         self._lbl_connect_socket.grid(column=1, row=1, padx=1, pady=1, sticky=(W, E))
         self._lbl_connect_file.grid(column=2, row=1, padx=1, pady=1, sticky=(W, E))
         self._lbl_disconnect.grid(column=3, row=1, padx=1, pady=1, sticky=(W, E))
 
         ttk.Separator(self).grid(
             column=0, row=7, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
 
-        self._frm_options.grid(column=0, row=8, columnspan=4, sticky=(W, E))
-        self._lbl_protocol.grid(column=0, row=0, padx=2, pady=2, sticky=(W))
-        self._chk_nmea.grid(column=1, row=0, padx=0, pady=0, sticky=(W))
-        self._chk_ubx.grid(column=2, row=0, padx=0, pady=0, sticky=(W))
-        self._chk_rtcm.grid(column=3, row=0, padx=0, pady=0, sticky=(W))
-        self._lbl_consoledisplay.grid(column=0, row=1, padx=2, pady=2, sticky=(W))
+        self._frm_options.grid(column=0, row=8, columnspan=5, sticky=(W, E))
+        self._lbl_protocol.grid(column=0, row=0, padx=2, pady=2, sticky=W)
+        self._chk_nmea.grid(column=1, row=0, padx=0, pady=0, sticky=W)
+        self._chk_ubx.grid(column=2, row=0, padx=0, pady=0, sticky=W)
+        self._chk_rtcm.grid(column=3, row=0, padx=0, pady=0, sticky=W)
+        self._lbl_consoledisplay.grid(column=0, row=1, padx=2, pady=2, sticky=W)
         self._spn_conformat.grid(
-            column=1, row=1, columnspan=2, padx=1, pady=2, sticky=(W)
+            column=1, row=1, columnspan=2, padx=1, pady=2, sticky=W
         )
-        self._chk_tags.grid(column=3, row=1, padx=1, pady=2, sticky=(W))
-        self._lbl_format.grid(column=0, row=2, padx=2, pady=2, sticky=(W))
-        self._spn_format.grid(column=1, row=2, padx=2, pady=2, sticky=(W))
-        self._lbl_units.grid(column=0, row=3, padx=2, pady=2, sticky=(W))
-        self._spn_units.grid(column=1, row=3, columnspan=3, padx=2, pady=2, sticky=(W))
-        self._chk_scroll.grid(column=0, row=4, padx=2, pady=2, sticky=(W))
-        self._spn_maxlines.grid(
-            column=1, row=4, columnspan=3, padx=2, pady=2, sticky=(W)
-        )
-        self._chk_webmap.grid(column=0, row=5, padx=2, pady=2, sticky=(W))
-        self._lbl_mapzoom.grid(column=1, row=5, sticky=(E))
-        self._scl_mapzoom.grid(column=2, row=5, columnspan=2, sticky=(W))
+        self._chk_tags.grid(column=3, row=1, padx=1, pady=2, sticky=W)
+        self._lbl_format.grid(column=0, row=2, padx=2, pady=2, sticky=W)
+        self._spn_format.grid(column=1, row=2, padx=2, pady=2, sticky=W)
+        self._lbl_units.grid(column=0, row=3, padx=2, pady=2, sticky=W)
+        self._spn_units.grid(column=1, row=3, columnspan=3, padx=2, pady=2, sticky=W)
+        self._chk_scroll.grid(column=0, row=4, padx=2, pady=2, sticky=W)
+        self._spn_maxlines.grid(column=1, row=4, columnspan=3, padx=2, pady=2, sticky=W)
+        self._lbl_maptype.grid(column=0, row=5, padx=2, pady=2, sticky=W)
+        self.spn_maptype.grid(column=1, row=5, padx=2, pady=2, sticky=W)
         self._chk_unusedsat.grid(
-            column=0, row=6, columnspan=2, padx=2, pady=2, sticky=(W)
-        )
-        self._chk_legend.grid(column=2, row=6, columnspan=2, padx=2, pady=2, sticky=(W))
-        self._chk_datalog.grid(column=0, row=7, padx=2, pady=2, sticky=(W))
-        self._spn_datalog.grid(
-            column=1, row=7, columnspan=3, padx=2, pady=2, sticky=(W)
+            column=0, row=6, columnspan=2, padx=2, pady=2, sticky=W
         )
+        self._chk_datalog.grid(column=0, row=7, padx=2, pady=2, sticky=W)
+        self._spn_datalog.grid(column=1, row=7, columnspan=3, padx=2, pady=2, sticky=W)
         self._chk_recordtrack.grid(
-            column=0, row=8, columnspan=2, padx=2, pady=2, sticky=(W)
+            column=0, row=8, columnspan=2, padx=2, pady=2, sticky=W
         )
-        self._chk_socketserve.grid(
-            column=0, row=9, rowspan=2, padx=2, pady=2, sticky=(N, S, W)
+        ttk.Separator(self._frm_options).grid(
+            column=0, row=9, columnspan=4, padx=2, pady=2, sticky=(W, E)
+        )
+        self.frm_server.grid(
+            column=0, row=10, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
-        self._lbl_sockmode.grid(column=1, row=9, padx=2, pady=2, sticky=(E))
-        self._spn_sockmode.grid(
-            column=2, row=9, columnspan=2, padx=2, pady=2, sticky=(W)
-        )
-        self._lbl_sockport.grid(column=1, row=10, padx=2, pady=2, sticky=(E))
-        self._ent_sockport.grid(column=2, row=10, padx=2, pady=2, sticky=(W))
-        self._lbl_sockclients.grid(column=3, row=10, padx=2, pady=2, sticky=(W))
         ttk.Separator(self._frm_options).grid(
             column=0, row=11, columnspan=4, padx=2, pady=2, sticky=(W, E)
         )
-        self._lbl_ubxconfig.grid(column=0, row=12, padx=2, pady=2, sticky=(E))
-        self._btn_ubxconfig.grid(column=1, row=12, padx=2, pady=2, sticky=(W))
-        self._lbl_ntripconfig.grid(column=2, row=12, padx=2, pady=2, sticky=(E))
-        self._btn_ntripconfig.grid(column=3, row=12, padx=2, pady=2, sticky=(W))
+        self._btn_ubxconfig.grid(column=0, row=13)
+        self._lbl_ubxconfig.grid(column=0, row=14)
+        self._btn_ntripconfig.grid(column=1, row=13)
+        self._lbl_ntripconfig.grid(column=1, row=14)
+        self._btn_spartnconfig.grid(column=2, row=13)
+        self._lbl_spartnconfig.grid(column=2, row=14)
+
+    def _on_connect(self, conntype: int):
+        """
+        Start or stop connection (serial, socket or file).
+
+        :param int conntype: connection type
+        """
+
+        conndict = {
+            "read_event": GNSS_EVENT,
+            "eof_event": GNSS_EOF_EVENT,
+            "error_event": GNSS_ERR_EVENT,
+            "inqueue": self.__app.gnss_inqueue,
+            "outqueue": self.__app.gnss_outqueue,
+            "socket_inqueue": self.__app.socket_inqueue,
+            "conntype": conntype,
+            "msgmode": self.frm_serial.msgmode,
+        }
+
+        self.frm_server.set_status(conntype)
+        if conntype == CONNECTED:
+            frm = self.frm_serial
+            if frm.status == NOPORTS:
+                return
+            connstr = f"{frm.port}:{frm.port_desc} @ {frm.bpsrate}"
+            conndict = dict(conndict, **{"serial_settings": frm})
+        elif conntype == CONNECTED_SOCKET:
+            frm = self.frm_socket
+            valid = True
+            valid = valid & valid_entry(frm.ent_server, VALURL)
+            valid = valid & valid_entry(frm.ent_port, VALINT, 1, MAXPORT)
+            if not valid:
+                self.__app.set_status("ERROR - invalid settings", "red")
+                return
+            connstr = f"{frm.server}:{frm.port}"
+            conndict = dict(conndict, **{"socket_settings": frm})
+        elif conntype == CONNECTED_FILE:
+            self.infilepath = self.__app.file_handler.open_infile()
+            if self.infilepath is None:
+                return
+            connstr = f"{self.infilepath}"
+            conndict = dict(conndict, **{"in_filepath": self.infilepath})
+        elif conntype == DISCONNECTED:
+            if self.__app.conn_status != DISCONNECTED:
+                self.__app.conn_status = DISCONNECTED
+                self.__app.stream_handler.stop_read_thread()
+                return
+        else:
+            return
+
+        self.__app.set_connection(connstr, "green")
+        self.__app.set_status("")
+        self.__app.conn_status = conntype
+        self._reset_frames()
+        self.__app.stream_handler.start_read_thread(self.__app, conndict)
 
     def _on_ubx_config(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Open UBX configuration dialog panel.
         """
 
-        self.__app.ubxconfig()
+        self.__app.start_dialog(DLGTUBX)
 
     def _on_ntrip_config(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Open NTRIP Client configuration dialog panel.
         """
 
-        self.__app.ntripconfig()
+        self.__app.start_dialog(DLGTNTRIP)
+
+    def _on_spartn_config(self, *args, **kwargs):  # pylint: disable=unused-argument
+        """
+        Open SPARTN Client configuration dialog panel.
+        """
+
+        self.__app.start_dialog(DLGTSPARTN)
 
-    def _on_webmap(self):
+    def _on_webmap(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Reset webmap refresh timer
         """
 
         self.__app.frm_mapview.reset_map_refresh()
 
     def _on_data_log(self):
         """
         Start or stop data logger
         """
 
         if self._datalog.get() == 1:
-            self._logpath = self.__app.file_handler.set_logfile_path()
-            if self._logpath is not None:
-                self.__app.set_status("Data logging enabled: " + self._logpath, "green")
+            self.outfilepath = self.__app.file_handler.set_logfile_path()
+            if self.outfilepath is not None:
+                self.__app.set_status("Data logging enabled: " + self.outfilepath)
                 self.__app.file_handler.open_logfile()
             else:
                 self._datalog.set(False)
         else:
-            self._logpath = None
+            self.outfilepath = None
             self._datalog.set(False)
             self.__app.file_handler.close_logfile()
-            self.__app.set_status("Data logging disabled", "blue")
+            self.__app.set_status("Data logging disabled")
 
     def _on_record_track(self):
         """
         Start or stop track recorder
         """
 
         if self._record_track.get() == 1:
             self._trackpath = self.__app.file_handler.set_trackfile_path()
             if self._trackpath is not None:
-                self.__app.set_status(
-                    "Track recording enabled: " + self._trackpath, "green"
-                )
+                self.__app.set_status("Track recording enabled: " + self._trackpath)
                 self.__app.file_handler.open_trackfile()
             else:
                 self._record_track.set(False)
         else:
             self._trackpath = None
             self._record_track.set(False)
             self.__app.file_handler.close_trackfile()
-            self.__app.set_status("Track recording disabled", "blue")
-
-    def _on_serial_stream(self):
-
-        if self.serial_settings().status == NOPORTS:
-            return
+            self.__app.set_status("Track recording disabled")
 
-        self.__app.set_connection(
-            (
-                f"{self.serial_settings().port}:{self.serial_settings().port_desc} "
-                + f"@ {self.serial_settings().bpsrate}"
-            ),
-            "green",
-        )
-        self.__app.set_status("")
-        self.__app.conn_status = CONNECTED
-        self.__app.stream_handler.start_read_thread(CONNECTED)
-
-    def _on_socket_stream(self):
-        """
-        Start socket streamer if settings are valid
-        """
-
-        valid = True
-        valid = valid & valid_entry(self._frm_socket.ent_server, VALURL)
-        valid = valid & valid_entry(self._frm_socket.ent_port, VALINT, 1, MAXPORT)
-        if valid:
-            self.__app.set_connection(
-                f"{self.socket_settings().server}:{self.socket_settings().port}",
-                "green",
-            )
-            self.__app.set_status("")
-            self.__app.conn_status = CONNECTED_SOCKET
-            self.__app.stream_handler.start_read_thread(CONNECTED_SOCKET)
-        else:
-            self.__app.set_status("ERROR - invalid settings", "red")
-
-    def _on_file_stream(self):
-        """
-        Start data file streamer if file selected
-        """
-
-        self._in_filepath = self.__app.file_handler.open_infile()
-        if self._in_filepath is not None:
-            self.__app.set_connection(f"{self._in_filepath}", "blue")
-            self.__app.set_status("")
-            self.__app.conn_status = CONNECTED_FILE
-            self.__app.stream_handler.start_read_thread(CONNECTED_FILE)
-
-    def _on_socket_serve(self):
-        """
-        Start or stop socket server.
-        """
-
-        if not valid_entry(self._ent_sockport, VALINT, 1, MAXPORT):
-            self.__app.set_status("ERROR - invalid port", "red")
-            self._socket_serve.set(0)
-            return
-
-        if self._socket_serve.get() == 1:
-            self.__app.start_sockserver_thread()
-            self._ent_sockport.config(state=DISABLED)
-            self._spn_sockmode.config(state=DISABLED)
-            self.__app.stream_handler.sock_serve = True
-        else:
-            self.__app.stop_sockserver_thread()
-            self._ent_sockport.config(state=NORMAL)
-            self._spn_sockmode.config(state=READONLY)
-            self.__app.stream_handler.sock_serve = False
-            self.clients = 0
-
-    def _on_sockmode(self):
-        """
-        Set default port depending on socket server mode.
-        """
-
-        if self._sock_mode.get() == SOCKMODES[1]:  # NTRIP Server
-            self._sock_port.set(SOCKSERVER_NTRIP_PORT)
-        else:
-            self._sock_port.set(SOCKSERVER_PORT)
-
-    def _on_disconnect(self):
+    def _reset(self):
         """
-        Disconnect from stream.
+        Reset settings to defaults.
         """
 
-        if self.__app.conn_status in (CONNECTED, CONNECTED_FILE, CONNECTED_SOCKET):
-            self.__app.stream_handler.stop_read_thread()
-            self.__app.stop_sockserver_thread()
-            self._socket_serve.set(0)
-            self.clients = 0
+        self.config = {}
+        self.clients = 0
 
-    def _reset(self):
+    def _reset_frames(self):
         """
-        Reset settings to defaults.
+        Reset frames.
         """
 
-        self._prot_nmea.set(1)
-        self._prot_ubx.set(1)
-        self._prot_rtcm3.set(1)
-        self._format.set(DDD)
-        self._units.set(UMM)
-        self._autoscroll.set(1)
-        self._maxlines.set(300)
-        self._display_format.set(FORMATS[0])  # Parsed
-        self._webmap.set(False)
-        self._mapzoom.set(10)
-        self._show_legend.set(True)
-        self._show_unusedsat.set(False)
-        self._datalog.set(False)
-        self._record_track.set(False)
-        self._logformat.set(FORMATS[1])  # Binary
-        self._colortags.set(TAG_COLORS)
-        self._socket_serve.set(0)
-        self._sock_port.set(SOCKSERVER_PORT)
-        self._sock_mode.set(SOCKMODES[0])  # open
-        self.clients = 0
+        self.__app.frm_mapview.reset_map_refresh()
+        self.__app.frm_spectrumview.reset()
+        self.__app.reset_gnssstatus()
 
     def enable_controls(self, status: int):
         """
         Public method to enable and disable those controls
         which depend on connection status.
 
         :param int status: connection status as integer
                (0=Disconnected, 1=Connected to serial,
                2=Connected to file, 3=No serial ports available)
 
         """
 
-        self._frm_serial.set_status(status)
-        self._frm_socket.set_status(status)
+        self.frm_serial.set_status(status)
+        self.frm_socket.set_status(status)
+        self.frm_server.set_status(status)
 
         self._btn_connect.config(
             state=(
                 DISABLED
                 if status in (CONNECTED, CONNECTED_SOCKET, CONNECTED_FILE, NOPORTS)
                 else NORMAL
             )
@@ -679,313 +598,99 @@
         self._spn_datalog.config(
             state=(
                 DISABLED
                 if status in (CONNECTED, CONNECTED_SOCKET, CONNECTED_FILE)
                 else READONLY
             )
         )
-        for ctl in (
-            self._chk_socketserve,
-            self._ent_sockport,
-            self._lbl_sockport,
-            self._lbl_sockmode,
-            self._lbl_sockclients,
-        ):
-            ctl.config(
-                state=(
-                    NORMAL
-                    if status in (CONNECTED, CONNECTED_SOCKET, CONNECTED_FILE)
-                    else DISABLED
-                )
-            )
-        self._spn_sockmode.config(
-            state=(
-                READONLY
-                if status in (CONNECTED, CONNECTED_SOCKET, CONNECTED_FILE)
-                else DISABLED
-            )
-        )
 
     def get_size(self) -> tuple:
         """
         Get current frame size.
 
         :return: (width, height)
         :rtype: tuple
 
         """
 
         self.update_idletasks()  # Make sure we know about any resizing
         return (self.winfo_width(), self.winfo_height())
 
-    def serial_settings(self) -> Frame:
-        """
-        Return reference to common serial configuration panel
-
-        :return: reference to serial form
-        :rtype: Frame
-        """
-
-        return self._frm_serial
-
-    def socket_settings(self) -> Frame:
-        """
-        Return reference to common socket configuration panel
-
-        :return: reference to socket form
-        :rtype: Frame
-        """
-
-        return self._frm_socket
-
     @property
-    def protocol(self) -> int:
+    def config(self) -> dict:
         """
-        Getter for displayed protocols
+        Getter for configuration settings to save as file.
 
-        :return: protocol displayed (1=NMEA, 2=UBX, 4=RTMC3, 7=ALL)
-        :rtype: int
+        :return: settings as dictionary
+        :rtype: dict
         """
 
-        return (
+        protocol = (
             (ubt.NMEA_PROTOCOL * self._prot_nmea.get())
             + (ubt.UBX_PROTOCOL * self._prot_ubx.get())
             + (ubt.RTCM3_PROTOCOL * self._prot_rtcm3.get())
         )
+        sockmode = 1 if self.frm_server.sock_mode.get() == SOCKMODES[1] else 0
 
-    @property
-    def display_format(self) -> int:
-        """
-        Getter for console display format
-
-        :return: display format (0 - parsed, 1 = binary, 2 = hex)
-        :rtype: int
-        """
-
-        return self._display_format.get()
-
-    @property
-    def autoscroll(self) -> int:
-        """
-        Getter for autoscroll flag
-
-        :return: scroll setting (0 = no scroll, 1 = auto)
-        :rtype: int
-        """
-
-        return self._autoscroll.get()
-
-    @property
-    def maxlines(self) -> int:
-        """
-        Getter for max console display lines
-
-        :return: max lines in console display (default=300)
-        :rtype: int
-        """
-
-        return self._maxlines.get()
-
-    @property
-    def webmap(self) -> int:
-        """
-        Getter for webmap flag
-
-        :return: map type (0 = static map, 1 = dynamic web map)
-        :rtype: int
-        """
-
-        return self._webmap.get()
-
-    @property
-    def mapzoom(self) -> int:
-        """
-        Getter for webmap zoom level
-
-        :return: webmap zoom level (1-20)
-        :rtype: int
-        """
-
-        return self._mapzoom.get()
-
-    @property
-    def units(self) -> str:
-        """
-        Getter for display units
-
-        :return: "UMM" = metric m/s, "UMK" = metric kmph,
-                 "UI" = imperial mph, "UIK" = imperial knots
-        :rtype: str
-        """
-
-        return self._units.get()
-
-    @property
-    def format(self) -> str:
-        """
-        Getter for degrees format
-
-        :return: "DD.D" = decimal degrees, "DM.M" = degrees, decimal minutes,
-                 "D.M.S" = degrees, minutes, seconds
-        :rtype: str
-        """
-
-        return self._format.get()
-
-    @property
-    def colortagging(self) -> bool:
-        """
-        Getter for colortags boolean
-
-        :return: colortag on/off
-        :rtype: bool
-        """
-
-        return self._colortags.get()
-
-    @property
-    def infilepath(self) -> str:
-        """
-        Getter for input file path
-
-        :return: input file path
-        :rtype: str
-        """
-
-        return self._in_filepath
-
-    @property
-    def outfilepath(self) -> str:
-        """
-        Getter for output file path
-
-        :return: output file path
-        :rtype: str
-        """
-
-        return self._logpath
-
-    @property
-    def datalogging(self) -> int:
-        """
-        Getter for datalogging flag
-
-        :return: 0 = no log, 1 = record datalog
-        :rtype: int
-        """
-
-        return self._datalog.get()
-
-    @property
-    def logformat(self) -> str:
-        """
-        Getter for datalogging format
-
-        :return: "Parsed", "Binary", "Hex", "Hextable"
-        :rtype: str
-        """
-
-        return self._logformat.get()
-
-    @property
-    def record_track(self) -> int:
-        """
-        Getter for record track flag
-
-        :return: 0 = no track, 1 = record track
-        :rtype: int
-        """
-
-        return self._record_track.get()
-
-    @property
-    def show_unused(self) -> int:
-        """
-        Getter for zero signal flag
-
-        :return: 0 = exclude, 1 = include
-        :rtype: int
-        """
-
-        return self._show_unusedsat.get()
-
-    @property
-    def show_legend(self) -> int:
-        """
-        Getter for graph legend flag
-
-        :return: 0 = hide, 1 = show
-        :rtype: int
-        """
-
-        return self._show_legend.get()
-
-    @property
-    def server_state(self) -> int:
-        """
-        Getter for socket server run status.
-
-        :return: status 0 = off, 1 = on
-        :rtype: int
-        """
-
-        return self._socket_serve.get()
-
-    @server_state.setter
-    def server_state(self, status: int):
-        """
-        Setter for server run status.
-
-        :param int status: 0 = off, 1 = on
-        """
-
-        self._socket_serve.set(status)
-
-    @property
-    def server_port(self) -> int:
-        """
-        Getter for socket server port
-
-        :return: port
-        :rtype: int
-        """
-
-        return int(self._sock_port.get())
-
-    @property
-    def server_mode(self) -> int:
-        """
-        Getter for socket server mode
-
-        :return: 0 = open socket server, 1 = NTRIP server
-        :rtype: int
-        """
-
-        if self._sock_mode.get() == SOCKMODES[1]:  # "NTRIP SERVER"
-            return 1
-        return 0
-
-    @property
-    def clients(self) -> int:
-        """
-        Getter for number of socket clients.
-        """
-
-        return self._sock_clients.get()
-
-    @clients.setter
-    def clients(self, clients: int):
-        """
-        Setter for number of socket clients.
-
-        :param int clients: no of clients connected
-        """
-
-        self._sock_clients.set(f"Clients {clients}")
-        if clients >= SOCKSERVER_MAX_CLIENTS:
-            self._lbl_sockclients.config(fg="red")
-        elif clients == 0:
-            self._lbl_sockclients.config(fg="black")
-        else:
-            self._lbl_sockclients.config(fg="green")
-        if self._socket_serve.get() == 1:
-            self.__app.frm_banner.update_transmit_status(clients)
+        config = {
+            "protocol": protocol,
+            "nmeaprot": self._prot_nmea.get(),
+            "ubxprot": self._prot_ubx.get(),
+            "rtcmprot": self._prot_rtcm3.get(),
+            "degreesformat": self._degrees_format.get(),
+            "colortag": self._colortag.get(),
+            "units": self._units.get(),
+            "autoscroll": self._autoscroll.get(),
+            "maxlines": self._maxlines.get(),
+            "consoleformat": self._console_format.get(),
+            "maptype": self.maptype.get(),
+            "mapzoom": self.mapzoom.get(),
+            "legend": self.show_legend.get(),
+            "unusedsat": self._show_unusedsat.get(),
+            "logformat": self._logformat.get(),
+            "datalog": self._datalog.get(),
+            "recordtrack": self._record_track.get(),
+            "sockserver": self.frm_server.socketserving,
+            "sockhost": self.frm_server.sock_host.get(),
+            "sockport": self.frm_server.sock_port.get(),
+            "sockmode": sockmode,
+        }
+        return config
+
+    @config.setter
+    def config(self, config: dict):
+        """
+        Setter for configuration loaded from file.
+
+        :param dict config: configuration
+        """
+
+        try:
+            self._prot_nmea.set(config.get("nmeaprot", 1))
+            self._prot_ubx.set(config.get("ubxprot", 1))
+            self._prot_rtcm3.set(config.get("rtcmprot", 1))
+            self._degrees_format.set(config.get("degreesformat", DDD))
+            self._colortag.set(config.get("colortag", 0))
+            self._units.set(config.get("units", UMM))
+            self._autoscroll.set(config.get("autoscroll", 1))
+            self._maxlines.set(config.get("maxlines", 200))
+            self._console_format.set(config.get("consoleformat", FORMATS[0]))
+            self.maptype.set(config.get("maptype", "world"))
+            self.mapzoom.set(config.get("mapzoom", 10))
+            self.show_legend.set(config.get("legend", 1))
+            self._show_unusedsat.set(config.get("unusedsat", 1))
+            self._logformat.set(config.get("logformat", FORMATS[1]))  # Binary
+            # don't persist datalog or gpx track settings...
+            # self._datalog.set(config.get("datalog", 0))
+            # self._record_track.set(config.get("recordtrack", 0))
+            self.frm_server.socketserving = config.get("sockserver", 0)
+            self.frm_server.sock_host.set(
+                config.get(
+                    "sockhost", getenv("PYGPSCLIENT_BINDADDRESS", SOCKSERVER_HOST)
+                )
+            )
+            self.frm_server.sock_port.set(config.get("sockport", SOCKSERVER_PORT))
+            self.frm_server.sock_mode.set(
+                SOCKMODES[1] if config.get("sockmode", 0) == 1 else SOCKMODES[0]
+            )
+        except KeyError as err:
+            self.__app.set_status(f"{CONFIGERR} - {err}", BADCOL)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/skyview_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/skyview_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 Created on 13 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
-from tkinter import Frame, Canvas, font, BOTH, YES
 from operator import itemgetter
-from pygpsclient.globals import WIDGETU1, BGCOL, FGCOL, GNSS_LIST
-from pygpsclient.helpers import snr2col, cel2cart
+from tkinter import BOTH, YES, Canvas, Frame, font
+
+from pygpsclient.globals import BGCOL, FGCOL, GNSS_LIST, WIDGETU1
+from pygpsclient.helpers import cel2cart, col2contrast, snr2col
 
 OL_WID = 2
 
 
 def _create_circle(self, x, y, r, **kwargs):
     """
     Helper method to simplify drawing circles on canvas
@@ -45,15 +45,15 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         def_w, def_h = WIDGETU1
         self.width = kwargs.get("width", def_w)
         self.height = kwargs.get("height", def_h)
         self.bg_col = BGCOL
@@ -76,16 +76,16 @@
 
     def init_sats(self):
         """
         Initialise satellite view
         """
 
         w, h = self.width, self.height
-        axis_r = w / 15
-        resize_font = font.Font(size=min(int(w / 25), 10))
+        axis_r = h / 18
+        resize_font = font.Font(size=min(int(w / 25), 8))
         self.can_satview.delete("all")
         maxr = min((h / 2), (w / 2)) - (axis_r * 2)
         for r in (0.2, 0.4, 0.6, 0.8, 1):
             self.can_satview.create_circle(
                 w / 2, h / 2, maxr * r, outline=self.fg_col, width=1
             )
         self.can_satview.create_line(w / 2, 0, w / 2, h, fill=self.fg_col)
@@ -99,24 +99,24 @@
         self.can_satview.create_text(
             w / 2, axis_r, text="0\u00b0 N", fill=self.fg_col, font=resize_font
         )
         self.can_satview.create_text(
             w / 2, h - axis_r, text="180\u00b0 S", fill=self.fg_col, font=resize_font
         )
 
-    def update_sats(self):
+    def update_frame(self):
         """
         Plot satellites' elevation and azimuth position.
         """
 
         data = self.__app.gnss_status.gsv_data
         w, h = self.width, self.height
-        axis_r = w / 15
+        axis_r = h / 18
         maxr = min((h / 2), (w / 2)) - (axis_r * 2)
-        resize_font = font.Font(size=min(int(maxr / 10), 10))
+        resize_font = font.Font(size=min(int(maxr / 10), 8))
         self.init_sats()
 
         for d in sorted(data, key=itemgetter(4)):  # sort by ascending snr
             try:
                 gnssId, prn, ele, azi, snr = d
                 ele = int(ele)
                 azi = (int(azi) - 90) % 360  # adjust so north is upwards
@@ -125,27 +125,28 @@
                 y = y * maxr
                 if snr == "":
                     snr = 0
                 else:
                     snr = int(snr)
                 (_, ol_col) = GNSS_LIST[gnssId]
                 prn = f"{int(prn):02}"
+                bg_col = snr2col(snr)
                 self.can_satview.create_circle(
                     x + (w / 2),
                     y + (h / 2),
                     (maxr / 10),
                     outline=ol_col,
-                    fill=snr2col(snr),
+                    fill=bg_col,
                     width=OL_WID,
                 )
                 self.can_satview.create_text(
                     x + (w / 2),
                     y + (h / 2),
                     text=prn,
-                    fill=self.fg_col,
+                    fill=col2contrast(bg_col),
                     font=resize_font,
                 )
             except ValueError:
                 pass
 
         self.can_satview.update_idletasks()
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/socketconfig_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/socketconfig_frame.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+socketconfig_frame.py
+
 Generic socket configuration Frame subclass
 for use in tkinter applications which require a
 socket configuration facility.
 
 Exposes the socket settings as properties.
 
 Application icons from https://iconmonstr.com/license/.
@@ -11,34 +13,36 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 
 from tkinter import (
-    Frame,
+    DISABLED,
+    NORMAL,
+    Button,
+    E,
     Entry,
-    Spinbox,
+    Frame,
     Label,
+    Spinbox,
     StringVar,
-    E,
     W,
-    NORMAL,
-    DISABLED,
 )
-from pygpsclient.globals import DEFAULT_SERVER, DEFAULT_PORT
+
+from PIL import Image, ImageTk
+
+from pygpsclient.globals import DEFAULT_PORT, DEFAULT_SERVER, ICON_CONTRACT, ICON_EXPAND
 
 ADVOFF = "\u25bc"
 ADVON = "\u25b2"
 READONLY = "readonly"
-ENTCOL = "azure"
-BGCOL = "azure"
 DISCONNECTED = 0
 CONNECTED = 1
-PROTOCOLS = ["TCP", "UDP"]
+PROTOCOLS = ["TCP IPv4", "UDP IPv6", "UDP IPv4", "TCP IPv6"]
 
 
 class SocketConfigFrame(Frame):
     """
     Socket configuration frame class.
     """
 
@@ -47,23 +51,25 @@
         Constructor.
 
         :param tkinter.Frame container: reference to container frame
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs for value ranges, or to pass to Frame parent class
         """
 
-        self._readonlybg = kwargs.pop("readonlybackground", BGCOL)
-
         Frame.__init__(self, container, *args, **kwargs)
 
         self._show_advanced = False
         self._status = DISCONNECTED
         self._server = StringVar()
         self._port = StringVar()
         self._protocol = StringVar()
+        self._flowinfo = StringVar()
+        self._scopeid = StringVar()
+        self._img_expand = ImageTk.PhotoImage(Image.open(ICON_EXPAND))
+        self._img_contract = ImageTk.PhotoImage(Image.open(ICON_CONTRACT))
 
         self._body()
         self._do_layout()
         self.reset()
 
     def _body(self):
         """
@@ -71,82 +77,149 @@
         """
 
         self._frm_basic = Frame(self)
         self._lbl_server = Label(self._frm_basic, text="Server")
         self.ent_server = Entry(
             self._frm_basic,
             textvariable=self._server,
-            bg=ENTCOL,
             relief="sunken",
             width=32,
         )
 
         self._lbl_port = Label(self._frm_basic, text="Port")
         self.ent_port = Entry(
             self._frm_basic,
             textvariable=self._port,
-            bg=ENTCOL,
             relief="sunken",
             width=6,
         )
         self._lbl_protocol = Label(self._frm_basic, text="Protocol")
         self._spn_protocol = Spinbox(
             self._frm_basic,
             textvariable=self._protocol,
             values=PROTOCOLS,
             width=12,
             state=READONLY,
-            readonlybackground=self._readonlybg,
             wrap=True,
+            command=self._on_change_protocol,
+        )
+        self._btn_toggle = Button(
+            self._frm_basic,
+            command=self._on_toggle_advanced,
+            image=self._img_expand,
+            width=28,
+            height=22,
+        )
+        self._frm_advanced = Frame(self)
+        self._lbl_flowinfo = Label(self._frm_advanced, text="Flow Info")
+        self.ent_flowinfo = Entry(
+            self._frm_advanced,
+            textvariable=self._flowinfo,
+            relief="sunken",
+            width=6,
+            state=DISABLED,
+        )
+
+        self._lbl_scopeid = Label(self._frm_advanced, text="Scope ID")
+        self.ent_scopeid = Entry(
+            self._frm_advanced,
+            textvariable=self._scopeid,
+            relief="sunken",
+            width=6,
+            state=DISABLED,
         )
 
     def _do_layout(self):
         """
         Layout widgets.
         """
 
         self._frm_basic.grid(column=0, row=0, columnspan=4, sticky=(W, E))
-        self._lbl_server.grid(column=0, row=0, padx=2, pady=2, sticky=(W))
+        self._lbl_server.grid(column=0, row=0, padx=2, pady=2, sticky=W)
         self.ent_server.grid(
             column=1, row=0, padx=2, pady=2, columnspan=4, sticky=(W, E)
         )
-        self._lbl_port.grid(column=0, row=1, padx=2, pady=2, sticky=(W))
-        self.ent_port.grid(column=1, row=1, padx=2, pady=2, sticky=(W))
-        self._lbl_protocol.grid(column=3, row=1, padx=2, pady=2, sticky=(W))
-        self._spn_protocol.grid(column=4, row=1, padx=2, pady=2, sticky=(W))
+        self._lbl_port.grid(column=0, row=1, padx=2, pady=2, sticky=W)
+        self.ent_port.grid(column=1, row=1, padx=2, pady=2, sticky=W)
+        self._lbl_protocol.grid(column=3, row=1, padx=2, pady=2, sticky=W)
+        self._spn_protocol.grid(column=4, row=1, padx=2, pady=2, sticky=W)
+        self._btn_toggle.grid(column=5, row=1, padx=2, pady=2, sticky=W)
+        self._frm_advanced.grid_forget()
+        self._lbl_flowinfo.grid(column=0, row=0, padx=2, pady=2, sticky=W)
+        self.ent_flowinfo.grid(column=1, row=0, padx=2, pady=2, sticky=W)
+        self._lbl_scopeid.grid(column=2, row=0, padx=2, pady=2, sticky=W)
+        self.ent_scopeid.grid(column=3, row=0, padx=2, pady=2, sticky=W)
 
     def reset(self):
         """
         Reset settings to defaults (first value in range).
         """
 
         self._server.set(DEFAULT_SERVER)
         self._port.set(DEFAULT_PORT)
         self._protocol.set(PROTOCOLS[0])
+        self._flowinfo.set(0)
+        self._scopeid.set(0)
 
     def set_status(self, status: int = DISCONNECTED):
         """
         Set connection status, which determines whether controls
         are enabled or not: 0=DISCONNECTED, 1=CONNECTED
 
         :param int status: status (0,1)
         """
 
         self._status = status
         for widget in (
             self._lbl_server,
             self._lbl_port,
             self._lbl_protocol,
+            self._lbl_flowinfo,
+            self._lbl_scopeid,
             self.ent_server,
             self.ent_port,
+            self.ent_flowinfo,
+            self.ent_scopeid,
         ):
             widget.configure(state=(NORMAL if status == DISCONNECTED else DISABLED))
         for widget in (self._spn_protocol,):
             widget.configure(state=(READONLY if status == DISCONNECTED else DISABLED))
 
+    def _on_change_protocol(self):
+        """
+        Toggle fields only used for IPv6.
+        """
+
+        for widget in (
+            self._lbl_flowinfo,
+            self._lbl_scopeid,
+            self.ent_flowinfo,
+            self.ent_scopeid,
+        ):
+            widget.configure(
+                state=(
+                    NORMAL
+                    if self._protocol.get() in ("TCP IPv6", "UDP IPv6")
+                    else DISABLED
+                )
+            )
+
+    def _on_toggle_advanced(self):
+        """
+        Toggle advanced socket settings panel on or off.
+        """
+
+        self._show_advanced = not self._show_advanced
+        if self._show_advanced:
+            self._frm_advanced.grid(column=0, row=1, columnspan=4, sticky=(W, E))
+            self._btn_toggle.config(image=self._img_contract)
+        else:
+            self._frm_advanced.grid_forget()
+            self._btn_toggle.config(image=self._img_expand)
+
     @property
     def status(self) -> int:
         """
         Getter for status flag: 0=DISCONNECTED, 1=CONNECTED
 
         :return: status flag (0,1)
         :rtype: int
@@ -176,14 +249,42 @@
 
         try:
             return int(self._port.get())
         except ValueError:
             return 0
 
     @property
+    def flowinfo(self) -> int:
+        """
+        Getter for flowinfo.
+
+        :return: IPv6 flowinfo
+        :rtype: int
+        """
+
+        try:
+            return int(self._flowinfo.get())
+        except ValueError:
+            return 0
+
+    @property
+    def scopeid(self) -> int:
+        """
+        Getter for scopeid.
+
+        :return: IPv6 scopeid
+        :rtype: int
+        """
+
+        try:
+            return int(self._scopeid.get())
+        except ValueError:
+            return 0
+
+    @property
     def protocol(self) -> str:
         """
         Getter for protocol.
 
         :return: selected protocol
         :rtype: str
         """
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/status_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/status_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
+status_frane.py
+
 Status Bar frame class for PyGPSClient application.
 
 This handles the status bar notifications at the foot of the window.
 
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
-from tkinter import ttk, Frame, Label, StringVar, N, S, W, E, VERTICAL
+from tkinter import VERTICAL, E, Frame, Label, N, S, StringVar, W, ttk
 
 
 class StatusFrame(Frame):
     """
     Status bar frame class.
     """
 
@@ -24,15 +26,15 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         self._status = StringVar()
         self._connection = StringVar()
         self.width, self.height = self.get_size()
         self._body()
 
@@ -49,40 +51,42 @@
 
         self._lbl_connection = Label(self, textvariable=self._connection, anchor=W)
         self._lbl_status_preset = Label(self, textvariable=self._status, anchor=W)
         self._lbl_connection.grid(column=0, row=0, sticky=(W, E))
         ttk.Separator(self, orient=VERTICAL).grid(column=1, row=0, sticky=(N, S))
         self._lbl_status_preset.grid(column=2, row=0, sticky=(W, E))
 
-    def set_connection(self, connection: str, color="blue"):
+    def set_connection(self, connection: str, color: str = ""):
         """
         Sets connection description in status bar.
 
         :param str connection: description of connection
         :param str color: rgb color string (default=blue)
 
         """
 
         if len(connection) > 100:
             connection = "..." + connection[-100:]
-        self._lbl_connection.config(fg=color)
+        if color != "":
+            self._lbl_connection.config(fg=color)
         self._connection.set("  " + connection)
 
-    def set_status(self, message, color="blue"):
+    def set_status(self, message, color: str = ""):
         """
         Sets message in status bar.
 
         :param str message: message to be displayed in status bar
         :param str color: rgb color string (default=blue)
 
         """
 
-        if len(message) > 80:
-            message = "..." + message[-80:]
-        self._lbl_status_preset.config(fg=color)
+        if len(message) > 100:
+            message = "..." + message[-100:]
+        if color != "":
+            self._lbl_status_preset.config(fg=color)
         self._status.set("  " + message)
 
     def clear_status(self):
         """
         Clears status bar.
         """
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/stream_handler.py` & `pygpsclient-1.4.0/src/pygpsclient/stream_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,61 @@
 """
-StreamHandler class for PyGPSClient application
+stream_handler.py
 
-This handles all the stream i/o, threaded read process and direction to
-the appropriate protocol handler
+StreamHandler class for PyGPSClient application.
+
+This handles all the serial stream i/o. It uses the pyubx2.UBXReader
+class to read and parse incoming data from the receiver. It places
+this data on an input message queue and generates a <<read-event>>
+which triggers the main App class to process the data.
+
+It also reads any command and poll messages placed on an output
+message queue and sends these to the receiver.
+
+The StreamHandler class is used by two PyGPSClient 'caller' objects:
+
+- SettingsFrame - i/o with the main GNSS receiver.
+- SpartnLbandDialog - i/o with a SPARTN L-Band receiver, when the
+SPARTN Client is active.
+
+The caller object can implement a 'set_status()' method to
+display any status messages output by StreamHandler.
 
 Created on 16 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
 import socket
-from io import BufferedReader
-from threading import Thread, Event
-from queue import Queue
 from datetime import datetime, timedelta
-from serial import Serial, SerialException, SerialTimeoutException
+from queue import Empty
+from threading import Event, Thread
+
+from pynmeagps import NMEAMessageError, NMEAParseError
+from pyrtcm import RTCMMessageError, RTCMParseError
 from pyubx2 import (
-    UBXReader,
-    UBXMessageError,
-    UBXParseError,
     ERR_IGNORE,
-    UBX_PROTOCOL,
     NMEA_PROTOCOL,
     RTCM3_PROTOCOL,
+    UBX_PROTOCOL,
+    UBXMessageError,
+    UBXParseError,
+    UBXReader,
 )
-from pynmeagps import NMEAMessageError, NMEAParseError
-from pyrtcm import RTCMMessageError, RTCMParseError
+from serial import Serial, SerialException, SerialTimeoutException
+
 from pygpsclient.globals import (
     CONNECTED,
     CONNECTED_FILE,
     CONNECTED_SOCKET,
-    DISCONNECTED,
-    FILEREAD_INTERVAL,
     DEFAULT_BUFSIZE,
+    FILEREAD_INTERVAL,
 )
-from pygpsclient.strings import ENDOFFILE
 
 
 class StreamHandler:
     """
     Stream handler class.
     """
 
@@ -49,263 +64,195 @@
         Constructor.
 
         :param Frame app: reference to main tkinter application
 
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
-        self._serial_object = None
-        self._serial_buffer = None
         self._stream_thread = None
         self._stopevent = Event()
-        self._sockserve_event = Event()
 
-    @property
-    def serial(self):
-        """
-        Getter for serial object
-        """
-
-        return self._serial_object
-
-    @property
-    def sock_serve(self) -> bool:
-        """
-        Getter for socket serve event status.
-
-        :return: socket server status (True/False)
-        :rtype: bool
-        """
-
-        return self._sockserve_event.is_set()
-
-    @sock_serve.setter
-    def sock_serve(self, status: bool):
-        """
-        Setter for socket serve event status.
-
-        :param bool status: sock serve status
-        """
-
-        if status:
-            self._sockserve_event.set()
-        else:
-            self._sockserve_event.clear()
-
-    def serial_write(self, data: bytes):
-        """
-        Write binary data to serial port.
-
-        :param bytes data: data to write to stream
-        """
-
-        if self.__app.conn_status == CONNECTED and self._serial_object is not None:
-            try:
-                self._serial_object.write(data)
-            except (SerialException, SerialTimeoutException) as err:
-                self.__app.set_status(f"Error writing to serial port {err}", "red")
-
-    def start_read_thread(self, mode: int):
+    def start_read_thread(self, caller: object, settings: dict):
         """
         Start the stream read thread.
 
-        :param int mode: connection mode
+        :param caller owner: calling object
+        :param dict settings: settings dictionary
         """
 
         self._stopevent.clear()
-        self.__app.frm_mapview.reset_map_refresh()
         self._stream_thread = Thread(
             target=self._read_thread,
             args=(
+                caller,
                 self._stopevent,
-                self._sockserve_event,
-                self.__app.msgqueue,
-                self.__app.socketqueue,
-                mode,
+                settings,
             ),
             daemon=True,
         )
         self._stream_thread.start()
-        self.__app.set_status("Connected", "blue")
 
     def stop_read_thread(self):
         """
         Stop serial reader thread.
         """
 
         self._stopevent.set()
         self._stream_thread = None
-        self.__app.conn_status = DISCONNECTED
 
     def _read_thread(
         self,
+        caller,
         stopevent: Event,
-        sockserve_event: Event,
-        msgqueue: Queue,
-        socketqueue: Queue,
-        mode: int,
+        settings: dict,
     ):
         """
         THREADED PROCESS
-
         Connects to selected data stream and starts read loop.
 
+        :param caller owner: calling object
         :param Event stopevent: thread stop event
-        :param Event sockserve_event: socket serving event
-        :param Queue msgqueue: message queue
-        :param Queue socketqueue: socket server message queue
-        :param int mode: connection mode
+        :param dict settings: settings dictionary
         """
 
-        connstr = ""
+        conntype = settings["conntype"]
         try:
-
-            if mode == CONNECTED:
-
-                ser = self.__app.frm_settings.serial_settings()
-                connstr = f"{ser.port}:{ser.port_desc} @ {str(ser.bpsrate)}"
-
+            if conntype == CONNECTED:
+                ser = settings["serial_settings"]
                 with Serial(
                     ser.port,
                     ser.bpsrate,
                     bytesize=ser.databits,
                     stopbits=ser.stopbits,
                     parity=ser.parity,
                     xonxoff=ser.xonxoff,
                     rtscts=ser.rtscts,
                     timeout=ser.timeout,
-                ) as self._serial_object:
-                    stream = BufferedReader(self._serial_object)
+                ) as stream:
                     self._readloop(
                         stopevent,
-                        sockserve_event,
-                        msgqueue,
-                        socketqueue,
                         stream,
-                        mode,
+                        settings,
                     )
 
-            elif mode == CONNECTED_FILE:
-
-                in_filepath = self.__app.frm_settings.infilepath
-                connstr = f"{in_filepath}"
-                with open(in_filepath, "rb") as self._serial_object:
-                    stream = BufferedReader(self._serial_object)
+            elif conntype == CONNECTED_FILE:
+                in_filepath = settings["in_filepath"]
+                with open(in_filepath, "rb") as stream:
                     self._readloop(
                         stopevent,
-                        sockserve_event,
-                        msgqueue,
-                        socketqueue,
                         stream,
-                        mode,
+                        settings,
                     )
 
-            elif mode == CONNECTED_SOCKET:
-
-                soc = self.__app.frm_settings.socket_settings()
+            elif conntype == CONNECTED_SOCKET:
+                soc = settings["socket_settings"]
                 server = soc.server
                 port = soc.port
-                connstr = f"{server}:{port}"
-                if soc.protocol == "UDP":
+                flowinfo = soc.flowinfo
+                scopeid = soc.scopeid
+                if soc.protocol[-4:] == "IPv6":
+                    afam = socket.AF_INET6
+                    conn = (server, port, flowinfo, scopeid)
+                else:  # IPv4
+                    afam = socket.AF_INET
+                    conn = (server, port)
+                if soc.protocol[:3] == "UDP":
                     socktype = socket.SOCK_DGRAM
                 else:  # TCP
                     socktype = socket.SOCK_STREAM
-                with socket.socket(socket.AF_INET, socktype) as stream:
-                    stream.connect((server, port))
+                with socket.socket(afam, socktype) as stream:
+                    stream.connect(conn)
                     self._readloop(
-                        stopevent, sockserve_event, msgqueue, socketqueue, stream, mode
+                        stopevent,
+                        stream,
+                        settings,
                     )
 
         except (EOFError, TimeoutError):
-            self.__master.event_generate("<<gnss_eof>>")
+            stopevent.set()
+            self.__master.event_generate(settings["eof_event"])
         except (
             IOError,
             SerialException,
             SerialTimeoutException,
             OSError,
             AttributeError,
             socket.gaierror,
         ) as err:
             if not stopevent.is_set():
                 stopevent.set()
-                self.__app.conn_status = DISCONNECTED
-                self.__app.set_connection(connstr, "red")
-                self.__app.set_status(f"Error in stream read {err}", "red")
+                self.__master.event_generate(settings["error_event"])
+                if hasattr(caller, "set_status"):
+                    caller.set_status(str(err), "red")
 
     def _readloop(
         self,
         stopevent: Event,
-        sockserve_event: Event,
-        msgqueue: Queue,
-        socketqueue: Queue,
         stream: object,
-        mode: int,
+        settings: dict,
     ):
         """
+        THREADED PROCESS
         Read stream continously until stop event or stream error.
 
         File streams use a small delay between reads to
         prevent thrashing.
 
         :param Event stopevent: thread stop event
-        :param Event sockserve_event: socket serving event
-        :param Queue msgqueue: message queue
-        :param Queue socketqueue: socket server message queue
-        :param object stream: data stream
-        :param int mode: connection mode
+        :param object stream: serial data stream
+        :param dict settings: settings dictionary
         """
 
+        conntype = settings["conntype"]
         ubr = UBXReader(
             stream,
             protfilter=NMEA_PROTOCOL | UBX_PROTOCOL | RTCM3_PROTOCOL,
             quitonerror=ERR_IGNORE,
             bufsize=DEFAULT_BUFSIZE,
+            msgmode=settings["msgmode"],
         )
 
         raw_data = None
         parsed_data = None
         lastread = datetime.now()
         while not stopevent.is_set():
             try:
-
-                if mode in (CONNECTED, CONNECTED_SOCKET) or (
-                    mode == CONNECTED_FILE
+                if conntype in (CONNECTED, CONNECTED_SOCKET) or (
+                    conntype == CONNECTED_FILE
                     and datetime.now() > lastread + timedelta(seconds=FILEREAD_INTERVAL)
                 ):
                     raw_data, parsed_data = ubr.read()
                     if raw_data is not None:
-                        msgqueue.put((raw_data, parsed_data))
-                        self.__master.event_generate("<<stream_read>>")
-                        if sockserve_event.is_set():
-                            socketqueue.put(raw_data)
+                        settings["inqueue"].put((raw_data, parsed_data))
+                        self.__master.event_generate(settings["read_event"])
                     else:
-                        if mode == CONNECTED_FILE:
+                        if conntype == CONNECTED_FILE:
                             raise EOFError
-                    if mode == CONNECTED_FILE:
+                    if conntype == CONNECTED_FILE:
                         lastread = datetime.now()
+                        self.__master.update_idletasks()
+
+                    # write any queued output data to serial stream
+                    if conntype in (CONNECTED, CONNECTED_SOCKET):
+                        try:
+                            while not settings["outqueue"].empty():
+                                data = settings["outqueue"].get(False)
+                                if data is not None:
+                                    ubr.datastream.write(data)
+                                settings["outqueue"].task_done()
+                        except Empty:
+                            pass
 
             except (
                 UBXMessageError,
                 UBXParseError,
                 NMEAMessageError,
                 NMEAParseError,
                 RTCMMessageError,
                 RTCMParseError,
             ) as err:
                 parsed_data = f"Error parsing data stream {err}"
-                msgqueue.put((raw_data, parsed_data))
-                self.__master.event_generate("<<stream_read>>")
+                settings["inqueue"].put((raw_data, parsed_data))
+                self.__master.event_generate(settings["read_event"])
                 continue
-
-    def on_eof(self, event):  # pylint: disable=unused-argument
-        """
-        EVENT TRIGGERED
-        Action on end of file
-
-        :param event event: <<gnss_eof>> event
-        """
-
-        self.stop_read_thread()
-        self.__app.frm_settings.server_state = 0  # turn off socket server
-        self.__app.set_status(ENDOFFILE, "blue")
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/strings.py` & `pygpsclient-1.4.0/src/pygpsclient/strings.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,133 +15,168 @@
 
 INTROTXT = "Welcome to PyGPSClient!"
 INTROTXTNOPORTS = "Welcome to PyGPSClient!"
 
 HELPTXT = "Help..About - display About dialog."
 
 ABOUTTXT = (
-    "PyGPSClient is a free, open-source NMEA, UBX & RTCM3 GNSS/GPS client "
+    "PyGPSClient is a free, open-source GNSS/GPS diagnostic and configuration "
     + "application written entirely in Python and tkinter. "
+    + "It supports NMEA, UBX, RTCM3, NTRIP & SPARTN protocols. "
     + "Instructions and source code are available on GitHub at the link below."
 )
+NA = "N/A"
+
+MAPAPIURL = "https://developer.mapquest.com/user/login/sign-up"
 
 # Message text
-SETINITTXT = "Settings initialised"
-VALERROR = "ERROR! Please correct highlighted entries"
-SAVEERROR = "ERROR! File could not be saved to specified directory"
-OPENFILEERROR = "ERROR! File could not be opened"
 BADJSONERROR = "ERROR! Invalid metadata file"
-NMEAVALERROR = "Value error in NMEA message: {}"
-SEROPENERROR = "Error opening serial port {}"
+CONFIGBAD = "{} command rejected"
+CONFIGERR = "Invalid configuration data"
+CONFIGOK = "{} command accepted"
+CONFIGRXM = "{} polled, {} key(s) loaded"
+CONFIGTITLE = "Config File"
+ENDOFFILE = "End of file reached"
 FILEOPENERROR = "Error opening file {}"
+LOADCONFIGBAD = "Configuration not loaded"
+LOADCONFIGOK = "Configuration loaded"
+MQTTCONN = "Connecting to MQTT server {}..."
+NMEAVALERROR = "Value error in NMEA message: {}"
+NOTCONN = "Not connected"
 NOWEBMAP = "Unable to display map."
-NOWEBMAPKEY = NOWEBMAP + "\n\nMQAPIKEY not found or invalid."
-NOWEBMAPHTTP = NOWEBMAP + "\n\nBad HTTP response: {}.\nCheck MQAPIKEY."
-NOWEBMAPFIX = NOWEBMAP + "\n\nNo satellite fix."
-NOWEBMAPCONN = NOWEBMAP + "\n\nCheck internet connection."
-SAVETITLE = "Select Directory"
+NOWEBMAPCONN = NOWEBMAP + "\nCheck internet connection."
+NOWEBMAPFIX = NOWEBMAP + "\nNo satellite fix."
+NOWEBMAPHTTP = NOWEBMAP + "\nBad HTTP response: {}.\nCheck MQAPIKEY.\n"
+NOWEBMAPKEY = NOWEBMAP + f"\nMQAPIKEY not found or invalid.\n\n{MAPAPIURL}"
+NULLSEND = "Nothing to send"
+OPENFILEERROR = "ERROR! File could not be opened"
 READTITLE = "Select File"
-WAITNMEADATA = "Waiting for data..."
-WAITUBXDATA = "Waiting for data..."
-ENDOFFILE = "End of file reached"
+SAVECONFIGBAD = "Configuration not saved"
+SAVECONFIGOK = "Configuration saved OK"
+SAVEERROR = "ERROR! File could not be saved to specified directory"
+SAVETITLE = "Select Directory"
+SEROPENERROR = "Error opening serial port {}"
+SETINITTXT = "Settings initialised"
 STOPDATA = "Serial reader process stopped"
-NOTCONN = "Not connected"
 UBXPOLL = "Polling current UBX configuration..."
+VALERROR = "ERROR! Please correct highlighted entries"
+VERCHECK = "Newer version of PyGPSClient available: {}"
+WAITNMEADATA = "Waiting for data..."
+WAITUBXDATA = "Waiting for data..."
 
 # Menu text
+MENUABOUT = "About"
+MENUCAN = "Cancel"
+MENUEXIT = "Exit"
 MENUFILE = "File"
-MENUVIEW = "View"
+MENUHELP = "Help"
+MENULOAD = "Load Configuration"
 MENUOPTION = "Options"
-MENUSAVE = "Save Settings"
-MENULOAD = "Load Settings"
-MENUEXIT = "Exit"
-MENUCAN = "Cancel"
+MENURESET = "Reset Layout"
 MENURST = "Reset"
-MENUHIDESE = "Hide Settings"
-MENUSHOWSE = "Show Settings"
-MENUHIDEUBX = "Hide UBX Config"
-MENUSHOWUBX = "Show UBX Config"
-MENUHIDESB = "Hide Status Bar"
-MENUSHOWSB = "Show Status Bar"
-MENUHIDECON = "Hide Console"
-MENUSHOWCON = "Show Console"
-MENUHIDEMAP = "Hide Map"
-MENUSHOWMAP = "Show Map"
-MENUHIDESATS = "Hide Satellites"
-MENUSHOWSATS = "Show Satellites"
-MENUUBXCONFIG = "UBX Configuration Dialog"
-MENUNTRIPCONFIG = "NTRIP Configuration Dialog"
-MENUHOWTO = "How To"
-MENUABOUT = "About"
-MENUHELP = "Help"
+MENUSAVE = "Save Configuration"
+MENUVIEW = "View"
+
 
 # Button text
-BTNPLOT = "PLOT"
-BTNSAVE = "Save"
 BTNCAN = "Cancel"
+BTNPLOT = "PLOT"
 BTNRST = "Reset"
+BTNSAVE = "Save"
 
 # Label text
-LBLPROTDISP = "Protocols Shown"
-LBLDATADISP = "Console Display"
-LBLUBXCONFIG = "UBX\nConfig"
-LBLNTRIPCONFIG = "NTRIP\nClient"
-LBLNTRIPGGAINT = "GGA Interval s"
-LBLCTL = "Controls"
-LBLSET = "Settings"
+LBLACCURACY = "Accuracy (cm)"
+LBLCFGGENERIC = "CFG-* Generic Configuration"
+LBLCFGMSG = "CFG-MSG Message Rate Configuration"
 LBLCFGPRT = "CFG-PRT Protocol Configuration"
 LBLCFGRATE = "CFG-RATE Navigation Solution Rate Configuration"
-LBLCFGMSG = "CFG-MSG Message Rate Configuration"
-LBLPRESET = "Preset UBX Configuration Commands"
+LBLCFGRECORD = "CFG Configuration Load/Save/Record"
+LBLCONFIGBASE = "Configure Base Station"
+LBLCTL = "Controls"
+LBLDATADISP = "Console Display"
 LBLDATALOG = "DataLogging"
-LBLSTREAM = "Stream\nfrom file"
-LBLTRACKRECORD = "GPX Track"
-LBLLEGEND = "Show Legend"
-LBLSHOWUNUSED = "Show Unused Satellites"
-LBLNTRIPSERVER = "Server"
-LBLNTRIPPORT = "Port"
-LBLNTRIPVERSION = "Version"
+LBLDEGFORMAT = "Position Format"
+LBLDURATIONS = "Duration (s)"
+LBLGGAFIXED = "Fixed Reference"
+LBLGGALIVE = "Receiver"
+LBLJSONLOAD = "Load Keys From JSON"
+LBLNTRIPCONFIG = "NTRIP Client"
+LBLNTRIPGGAINT = "GGA Interval s"
 LBLNTRIPMOUNT = "Mountpoint"
-LBLNTRIPUSER = "User"
+LBLNTRIPPORT = "Port"
 LBLNTRIPPWD = "Password"
+LBLNTRIPSERVER = "Server"
 LBLNTRIPSTR = "Sourcetable"
-LBLSOCKSERVE = "Socket Server /\nNTRIP Caster   "  # padded to align
-LBLSERVERPORT = "Port"
-LBLDEGFORMAT = "Degrees Format"
+LBLNTRIPUSER = "User"
+LBLNTRIPVERSION = "Version"
+LBLPRESET = "Preset UBX Configuration Commands"
+LBLPROTDISP = "Protocols Shown"
+LBLSERVERHOST = "Host"
 LBLSERVERMODE = "Mode"
-LBLCFGDYN = "CFG-* Other Configuration"
-LBLGGALIVE = "Receiver"
-LBLGGAFIXED = "Fixed Reference"
+LBLSERVERPORT = "Port"
+LBLSET = "Settings"
+LBLSHOWUNUSED = "Show Unused Satellites"
+LBLSOCKSERVE = "Socket Server /\nNTRIP Caster   "  # padded to align
+LBLSPARTNCONFIG = "SPARTN Client"
+LBLSPARTNGN = "GNSS RECEIVER CONFIGURATION (F9*)"
+LBLSPARTNIP = "IP CORRECTION CONFIGURATION (MQTT)"
+LBLSPARTNLB = "L-BAND CORRECTION CONFIGURATION (D9*)"
+LBLSPTNCURR = "CURRENT SPARTN KEY:"
+LBLSPTNDAT = "Valid from YYYYMMDD"
+LBLSPTNFP = "Configure receiver"
+LBLSPTNKEY = "Key as hexadecimal"
+LBLSPTNNEXT = "NEXT SPARTN KEY:"
+LBLSPTNNMEA = "Disable NMEA"
+LBLSPTNUPLOAD = "Upload keys"
+LBLSTREAM = "Stream\nfrom file"
+LBLTRACKRECORD = "GPX Track"
+LBLUBXCONFIG = "UBX Config"
+LBLUDPORT = "USER-DEFINED PORT"
 
 # Dialog text
-DLGUBXCONFIG = "UBX Configuration"
-DLGNTRIPCONFIG = "NTRIP Client Configuration"
 DLGABOUT = "PyGPSClient"
+DLGENABLEMONSPAN = "Enable or poll MON-SPAN message"
+DLGENABLEMONSYS = "Enable or poll MON-SYS/COMMS messages"
+DLGGPXERROR = "GPX PARSING ERROR!"
+DLGGPXLOAD = "LOADING GPX TRACK ..."
+DLGGPXNULL = "NO TRACKPOINTS IN GPX FILE!"
+DLGGPXPROMPT = "CLICK FOLDER ICON TO LOAD GPX FILE"
+DLGGPXVIEWER = "GPX Track Viewer"
 DLGHOWTO = "How To Use PyGPSCLient"
+DLGJSONERR = "ERROR! {}"
+DLGJSONOK = "Keys loaded from {}"
+DLGNOMONSPAN = "This receiver does not appear to\nsupport the MON-SPAN messages"
+DLGNOMONSYS = "This receiver does not appear to support\nthe MON-SYS/COMMS messages"
+DLGNTRIPCONFIG = "NTRIP Client Configuration"
 DLGRESET = "Confirm Reset"
-DLGSAVE = "Confirm Save"
 DLGRESETCONFIRM = (
     "Are you sure you want to reset the\ncurrent configuration to the\nfactory default?"
 )
+DLGSAVE = "Confirm Save"
 DLGSAVECONFIRM = "Are you sure you want to save\nthe current configuration?"
+DLGSPARTNCONFIG = "SPARTN Client Configuration"
+DLGSPARTNWARN = "WARNING! Disconnect from {} client before using {} client"
+DLGUBXCONFIG = "UBX Configuration"
+DLGWAITMONSPAN = "Waiting for MON-SPAN message..."
+DLGWAITMONSYS = "Waiting for MON-SYS/COMMS messages..."
 
 # UBX Preset Command Descriptions
-PSTRESET = "CFG-CFG - RESTORE FACTORY DEFAULTS"
-PSTSAVE = "CFG-CFG - SAVE CURRENT CONFIGURATION"
-PSTMINNMEAON = "CFG-MSG - Turn ON minimum NMEA msgs"
-PSTALLNMEAON = "CFG-MSG - Turn ON all NMEA msgs"
-PSTALLNMEAOFF = "CFG-MSG - Turn OFF all NMEA msgs"
-PSTMINUBXON = "CFG-MSG - Turn ON minimum UBX NAV msgs"
-PSTALLUBXON = "CFG-MSG - Turn ON all UBX NAV msgs"
-PSTALLUBXOFF = "CFG-MSG - Turn OFF all UBX NAV msgs"
-PSTALLINFON = "CFG-INF - Turn ON all INF msgs"
 PSTALLINFOFF = "CFG-INF - Turn OFF all non-error INF msgs"
-PSTALLLOGON = "CFG-MSG - Turn ON all LOG msgs"
+PSTALLINFON = "CFG-INF - Turn ON all INF msgs"
 PSTALLLOGOFF = "CFG-MSG - Turn OFF all LOG msgs"
-PSTALLMONON = "CFG-MSG - Turn ON all MON msgs"
+PSTALLLOGON = "CFG-MSG - Turn ON all LOG msgs"
 PSTALLMONOFF = "CFG-MSG - Turn OFF all MON msgs"
-PSTALLRXMON = "CFG-MSG - Turn ON all RXM msgs"
+PSTALLMONON = "CFG-MSG - Turn ON all MON msgs"
+PSTALLNMEAOFF = "CFG-MSG - Turn OFF all NMEA msgs"
+PSTALLNMEAON = "CFG-MSG - Turn ON all NMEA msgs"
 PSTALLRXMOFF = "CFG-MSG - Turn OFF all RXM msgs"
-PSTPOLLPORT = "CFG-PRT - Poll Port config"
-PSTPOLLINFO = "CFG-INF - Poll Info message config"
+PSTALLRXMON = "CFG-MSG - Turn ON all RXM msgs"
+PSTALLUBXOFF = "CFG-MSG - Turn OFF all UBX NAV msgs"
+PSTALLUBXON = "CFG-MSG - Turn ON all UBX NAV msgs"
+PSTMINNMEAON = "CFG-MSG - Turn ON minimum NMEA msgs"
+PSTMINUBXON = "CFG-MSG - Turn ON minimum UBX NAV msgs"
 PSTPOLLALLCFG = "CFG-xxx - Poll All Configuration Messages"
 PSTPOLLALLNAV = "NAV(2)-xxx - Poll All Navigation Messages"
+PSTPOLLINFO = "CFG-INF - Poll Info message config"
+PSTPOLLPORT = "CFG-PRT - Poll Port config"
+PSTRESET = "CFG-CFG - RESTORE FACTORY DEFAULTS"
+PSTSAVE = "CFG-CFG - Save configuration to non-volatile memory"
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_cfgval_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_cfgval_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,94 +3,49 @@
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 from tkinter import (
-    Frame,
-    Radiobutton,
-    Listbox,
-    Spinbox,
-    Scrollbar,
+    HORIZONTAL,
+    LEFT,
+    NORMAL,
+    VERTICAL,
     Button,
-    Label,
-    StringVar,
-    IntVar,
+    E,
     Entry,
+    Frame,
+    IntVar,
+    Label,
+    Listbox,
     N,
+    Radiobutton,
     S,
-    E,
+    Scrollbar,
+    Spinbox,
+    StringVar,
     W,
-    LEFT,
-    VERTICAL,
-    HORIZONTAL,
-    NORMAL,
 )
-from PIL import ImageTk, Image
-from pyubx2 import UBXMessage, UBX_CONFIG_DATABASE
-from pyubx2.ubxhelpers import atttyp, attsiz, cfgname2key
+
+from PIL import Image, ImageTk
+from pyubx2 import UBX_CONFIG_DATABASE, UBXMessage
+from pyubx2.ubxhelpers import attsiz, atttyp, cfgname2key
+
 from pygpsclient.globals import (
-    ENTCOL,
-    ERRCOL,
-    INFCOL,
+    ICON_CONFIRMED,
+    ICON_PENDING,
     ICON_SEND,
     ICON_WARNING,
-    ICON_PENDING,
-    ICON_CONFIRMED,
     READONLY,
     UBX_CFGVAL,
 )
 
-UBX_CONFIG_CATEGORIES = [
-    "CFG_ANA",
-    "CFG_BATCH",
-    "CFG_BDS",
-    "CFG_GEOFENCE",
-    "CFG_HW_ANT",
-    "CFG_HW_RF",
-    "CFG_I2C",
-    "CFG_INFMSG",
-    "CFG_ITFM",
-    "CFG_LOGFILTER",
-    "CFG_MOT",
-    "CFG_MSGOUT_NMEA",
-    "CFG_MSGOUT_PUBX",
-    "CFG_MSGOUT_RTCM",
-    "CFG_MSGOUT_UBX",
-    "CFG_NAV2",
-    "CFG_NAVHPG",
-    "CFG_NAVSPG",
-    "CFG_NMEA",
-    "CFG_ODO",
-    "CFG_PM",
-    "CFG_PMP",
-    "CFG_QZSS",
-    "CFG_RATE",
-    "CFG_RINV",
-    "CFG_RTCM",
-    "CFG_SBAS",
-    "CFG_SEC",
-    "CFG_SFCORE",
-    "CFG_SFIMU",
-    "CFG_SFODO",
-    "CFG_SIGNAL",
-    "CFG_SPARTN",
-    "CFG_SPI",
-    "CFG_TMODE",
-    "CFG_TP",
-    "CFG_TXREADY",
-    "CFG_UART1",
-    "CFG_UART2",
-    "CFG_USB",
-]
-
 VALSET = 0
 VALDEL = 1
 VALGET = 2
 ATTDICT = {
     "U": "unsigned int",
     "I": "signed int",
     "R": "float",
@@ -113,15 +68,15 @@
         :param Frame app: reference to main tkinter application
         :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self.__container = container
 
         Frame.__init__(self, self.__container.container, *args, **kwargs)
 
         self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
         self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
         self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
@@ -149,15 +104,14 @@
             self, text="CFG-VALSET/DEL/GET Configuration Interface", anchor="w"
         )
         self._lbl_cat = Label(self, text="Category", anchor="w")
         self._lbx_cat = Listbox(
             self,
             border=2,
             relief="sunken",
-            bg=ENTCOL,
             height=5,
             justify=LEFT,
             exportselection=False,
         )
         self._scr_catv = Scrollbar(self, orient=VERTICAL)
         self._scr_cath = Scrollbar(self, orient=HORIZONTAL)
         self._lbx_cat.config(yscrollcommand=self._scr_catv.set)
@@ -165,15 +119,14 @@
         self._scr_catv.config(command=self._lbx_cat.yview)
         self._scr_cath.config(command=self._lbx_cat.xview)
         self._lbl_parm = Label(self, text="Keyname", anchor="w")
         self._lbx_parm = Listbox(
             self,
             border=2,
             relief="sunken",
-            bg=ENTCOL,
             height=5,
             justify=LEFT,
             exportselection=False,
         )
         self._scr_parmv = Scrollbar(self, orient=VERTICAL)
         self._scr_parmh = Scrollbar(self, orient=HORIZONTAL)
         self._lbx_parm.config(yscrollcommand=self._scr_parmv.set)
@@ -190,47 +143,39 @@
         self._rad_cfgget = Radiobutton(
             self, text="CFG-VALGET", variable=self._cfgmode, value=2
         )
         self._lbl_key = Label(self, text="KeyID")
         self._lbl_keyid = Label(
             self,
             textvariable=self._cfgkeyid,
-            bg=ENTCOL,
             width=10,
-            fg=INFCOL,
             border=1,
             relief="sunken",
         )
         self._lbl_type = Label(self, text="Type")
         self._lbl_att = Label(
             self,
             textvariable=self._cfgatt,
-            bg=ENTCOL,
             width=5,
-            fg=INFCOL,
             border=1,
             relief="sunken",
         )
         self._lbl_layer = Label(self, text="Layer")
         self._spn_layer = Spinbox(
             self,
             textvariable=self._cfglayer,
             values=("RAM", "BBR", "FLASH", "DEFAULT"),
-            bg=ENTCOL,
             wrap=True,
             width=8,
             state=READONLY,
-            readonlybackground=ENTCOL,
         )
         self._lbl_val = Label(self, text="Value")
         self._ent_val = Entry(
             self,
             textvariable=self._cfgval,
-            readonlybackground=ENTCOL,
-            fg=INFCOL,
             state=READONLY,
             relief="sunken",
         )
 
         self._lbl_send_command = Label(self)
         self._btn_send_command = Button(
             self,
@@ -251,33 +196,33 @@
         self._scr_cath.grid(column=0, row=7, sticky=(W, E))
         self._lbl_parm.grid(column=1, row=1, columnspan=4, padx=3, sticky=(W, E))
         self._lbx_parm.grid(
             column=1, row=2, columnspan=4, rowspan=5, padx=3, pady=3, sticky=(W, E)
         )
         self._scr_parmv.grid(column=4, row=2, rowspan=5, sticky=(N, S, E))
         self._scr_parmh.grid(column=1, row=7, columnspan=4, sticky=(W, E))
-        self._rad_cfgget.grid(column=0, row=8, padx=3, pady=0, sticky=(W))
-        self._rad_cfgset.grid(column=0, row=9, padx=3, pady=0, sticky=(W))
-        self._rad_cfgdel.grid(column=0, row=10, padx=3, pady=0, sticky=(W))
-        self._lbl_key.grid(column=1, row=8, padx=3, pady=0, sticky=(E))
-        self._lbl_keyid.grid(column=2, row=8, padx=3, pady=0, sticky=(W))
-        self._lbl_type.grid(column=3, row=8, padx=3, pady=0, sticky=(E))
-        self._lbl_att.grid(column=4, row=8, padx=3, pady=0, sticky=(W))
-        self._lbl_layer.grid(column=1, row=9, padx=3, pady=0, sticky=(E))
-        self._spn_layer.grid(column=2, row=9, padx=3, pady=0, sticky=(W))
-        self._lbl_val.grid(column=1, row=10, padx=3, pady=0, sticky=(E))
+        self._rad_cfgget.grid(column=0, row=8, padx=3, pady=0, sticky=W)
+        self._rad_cfgset.grid(column=0, row=9, padx=3, pady=0, sticky=W)
+        self._rad_cfgdel.grid(column=0, row=10, padx=3, pady=0, sticky=W)
+        self._lbl_key.grid(column=1, row=8, padx=3, pady=0, sticky=E)
+        self._lbl_keyid.grid(column=2, row=8, padx=3, pady=0, sticky=W)
+        self._lbl_type.grid(column=3, row=8, padx=3, pady=0, sticky=E)
+        self._lbl_att.grid(column=4, row=8, padx=3, pady=0, sticky=W)
+        self._lbl_layer.grid(column=1, row=9, padx=3, pady=0, sticky=E)
+        self._spn_layer.grid(column=2, row=9, padx=3, pady=0, sticky=W)
+        self._lbl_val.grid(column=1, row=10, padx=3, pady=0, sticky=E)
         self._ent_val.grid(
             column=2, row=10, columnspan=3, padx=3, pady=0, sticky=(W, E)
         )
 
         self._btn_send_command.grid(
-            column=3, row=12, rowspan=2, ipadx=3, ipady=3, sticky=(E)
+            column=3, row=12, rowspan=2, ipadx=3, ipady=3, sticky=E
         )
         self._lbl_send_command.grid(
-            column=4, row=13, rowspan=2, ipadx=3, ipady=3, sticky=(E)
+            column=4, row=13, rowspan=2, ipadx=3, ipady=3, sticky=E
         )
 
         (cols, rows) = self.grid_size()
         for i in range(cols):
             self.grid_columnconfigure(i, weight=1)
         for i in range(rows):
             self.grid_rowconfigure(i, weight=1)
@@ -290,30 +235,39 @@
 
         self._lbx_cat.bind("<<ListboxSelect>>", self._on_select_cat)
         self._lbx_parm.bind("<<ListboxSelect>>", self._on_select_parm)
         self._cfgmode.trace_add("write", self._on_select_mode)
 
     def reset(self):
         """
-        Reset panel.
+        Reset panel with sorted list of unique UBX Config Database key categories.
         """
 
-        for i, cat in enumerate(UBX_CONFIG_CATEGORIES):
+        cdb_cats = []
+        for cdb in UBX_CONFIG_DATABASE:
+            cdbs = cdb.split("_", maxsplit=3)
+            cdbp = f"{cdbs[0]}_{cdbs[1]}"
+            if cdbs[1] == "MSGOUT":  # subdivide large MSGOUT category
+                cdbp += f"_{cdbs[2]}"
+            if cdbp not in cdb_cats:
+                cdb_cats.append(cdbp)
+
+        for i, cat in enumerate(cdb_cats):
             self._lbx_cat.insert(i, cat)
         self._cfgmode.set(2)
 
     def _on_select_mode(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Mode has been selected.
         """
 
         if self._cfgmode.get() == VALSET:
-            self._ent_val.config(state=NORMAL, bg=ENTCOL, fg="Black")
+            self._ent_val.config(state=NORMAL)
         else:
-            self._ent_val.config(state=READONLY, readonlybackground=ENTCOL, fg=INFCOL)
+            self._ent_val.config(state=READONLY)
 
     def _on_select_cat(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Configuration category has been selected.
         """
 
         idx = self._lbx_cat.curselection()
@@ -397,22 +351,22 @@
                 (self._cfgval_keyname, val),
             ]
         except ValueError:
             valid_entry = False
 
         if valid_entry:
             msg = UBXMessage.config_set(layers, transaction, cfgData)
-            self.__app.stream_handler.serial_write(msg.serialize())
-            self._ent_val.configure(bg=ENTCOL)
+            self.__container.send_command(msg)
             self._lbl_send_command.config(image=self._img_pending)
-            self.__container.set_status("CFG-VALSET SET message sent", "blue")
+            self.__container.set_status(
+                "CFG-VALSET SET message sent",
+            )
             for msgid in ("ACK-ACK", "ACK-NAK"):
                 self.__container.set_pending(msgid, UBX_CFGVAL)
         else:
-            self._ent_val.configure(bg=ERRCOL)
             self._lbl_send_command.config(image=self._img_warn)
             typ = ATTDICT[att]
             self.__container.set_status(
                 (
                     "INVALID ENTRY - must conform to parameter "
                     f"type {att} ({typ}) and size {atts} bytes"
                 ),
@@ -434,18 +388,17 @@
         else:
             layers = 1
         transaction = 0
         key = [
             self._cfgval_keyname,
         ]
         msg = UBXMessage.config_del(layers, transaction, key)
-        self.__app.stream_handler.serial_write(msg.serialize())
-        self._ent_val.configure(bg=ENTCOL)
+        self.__container.send_command(msg)
         self._lbl_send_command.config(image=self._img_pending)
-        self.__container.set_status("CFG-VALDEL SET message sent", "blue")
+        self.__container.set_status("CFG-VALDEL SET message sent")
         for msgid in ("ACK-ACK", "ACK-NAK"):
             self.__container.set_pending(msgid, UBX_CFGVAL)
 
     def _do_valget(self):
         """
         Send a CFG-VALGET message.
         """
@@ -460,18 +413,17 @@
         else:
             layers = 0
         transaction = 0
         keys = [
             self._cfgval_keyname,
         ]
         msg = UBXMessage.config_poll(layers, transaction, keys)
-        self.__app.stream_handler.serial_write(msg.serialize())
-        self._ent_val.configure(bg=ENTCOL)
+        self.__container.send_command(msg)
         self._lbl_send_command.config(image=self._img_pending)
-        self.__container.set_status("CFG-VALGET POLL message sent", "blue")
+        self.__container.set_status("CFG-VALGET POLL message sent")
         for msgid in ("CFG-VALGET", "ACK-ACK", "ACK-NAK"):
             self.__container.set_pending(msgid, UBX_CFGVAL)
 
     def update_status(self, msg: UBXMessage):  # pylint: disable=unused-argument
         """
         Update pending confirmation status.
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_config_dialog.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_config_dialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,51 +14,45 @@
 
 Created on 19 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
-from tkinter import (
-    Toplevel,
-    Frame,
-    Button,
-    Label,
-    StringVar,
-    N,
-    S,
-    E,
-    W,
-)
-from PIL import ImageTk, Image
+from tkinter import Button, E, Frame, Label, N, S, StringVar, Toplevel, W
+
+from PIL import Image, ImageTk
 from pyubx2 import UBXMessage
+
 from pygpsclient.globals import (
+    CONNECTED,
+    CONNECTED_SOCKET,
+    DLGTUBX,
+    ENABLE_CFG_OTHER,
     ICON_EXIT,
-    UBX_MONVER,
-    UBX_MONHW,
+    POPUP_TRANSIENT,
+    UBX_CFGMSG,
+    UBX_CFGOTHER,
     UBX_CFGPRT,
     UBX_CFGRATE,
-    UBX_CFGMSG,
     UBX_CFGVAL,
-    UBX_CFGOTHER,
+    UBX_MONHW,
+    UBX_MONVER,
     UBX_PRESET,
-    CONNECTED,
-    ENABLE_CFG_OTHER,
 )
 from pygpsclient.strings import DLGUBXCONFIG
-from pygpsclient.globals import POPUP_TRANSIENT
+from pygpsclient.ubx_cfgval_frame import UBX_CFGVAL_Frame
+from pygpsclient.ubx_dynamic_frame import UBX_Dynamic_Frame
 from pygpsclient.ubx_info_frame import UBX_INFO_Frame
-from pygpsclient.ubx_port_frame import UBX_PORT_Frame
 from pygpsclient.ubx_msgrate_frame import UBX_MSGRATE_Frame
+from pygpsclient.ubx_port_frame import UBX_PORT_Frame
 from pygpsclient.ubx_preset_frame import UBX_PRESET_Frame
-from pygpsclient.ubx_cfgval_frame import UBX_CFGVAL_Frame
+from pygpsclient.ubx_recorder_frame import UBX_Recorder_Frame
 from pygpsclient.ubx_solrate_frame import UBX_RATE_Frame
-from pygpsclient.ubx_dynamic_frame import UBX_Dynamic_Frame
 
 
 class UBXConfigDialog(Toplevel):
     """,
     UBXConfigDialog class.
     """
 
@@ -68,26 +62,27 @@
 
         :param Frame app: reference to main tkinter application
         :param args: optional args to pass to parent class (not currently used)
         :param kwargs: optional kwargs to pass to parent class (not currently used)
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         Toplevel.__init__(self, app)
         if POPUP_TRANSIENT:
             self.transient(self.__app)
         self.resizable(True, True)  # allow for MacOS resize glitches
         self.title(DLGUBXCONFIG)  # pylint: disable=E1102
         self.protocol("WM_DELETE_WINDOW", self.on_exit)
         self._img_exit = ImageTk.PhotoImage(Image.open(ICON_EXIT))
         self._cfg_msg_command = None
         self._pending_confs = {}
         self._status = StringVar()
         self._status_cfgmsg = StringVar()
+        self._recordmode = False
 
         self._body()
         self._do_layout()
         self._reset()
 
     def _body(self):
         """
@@ -107,14 +102,17 @@
             command=self.on_exit,
             font=self.__app.font_md,
         )
         # add configuration widgets
         self._frm_device_info = UBX_INFO_Frame(
             self.__app, self, borderwidth=2, relief="groove"
         )
+        self._frm_recorder = UBX_Recorder_Frame(
+            self.__app, self, borderwidth=2, relief="groove"
+        )
         self._frm_config_port = UBX_PORT_Frame(
             self.__app, self, borderwidth=2, relief="groove"
         )
         self._frm_config_rate = UBX_RATE_Frame(
             self.__app, self, borderwidth=2, relief="groove"
         )
         self._frm_config_msg = UBX_MSGRATE_Frame(
@@ -149,14 +147,15 @@
             ipadx=5,
             ipady=5,
             sticky=(N, S, W, E),
         )
         # left column of grid
         for frm in (
             self._frm_device_info,
+            self._frm_recorder,
             self._frm_config_port,
             self._frm_config_rate,
             self._frm_config_msg,
         ):
             (colsp, rowsp) = frm.grid_size()
             frm.grid(
                 column=col,
@@ -200,15 +199,15 @@
         col = 0
         row = maxrow
         (colsp, rowsp) = self._frm_container.grid_size()
         self._frm_status.grid(column=col, row=row, columnspan=colsp, sticky=(W, E))
         self._lbl_status.grid(
             column=0, row=0, columnspan=colsp - 1, ipadx=3, ipady=3, sticky=(W, E)
         )
-        self._btn_exit.grid(column=colsp - 1, row=0, ipadx=3, ipady=3, sticky=(E))
+        self._btn_exit.grid(column=colsp - 1, row=0, ipadx=3, ipady=3, sticky=E)
 
         for frm in (self._frm_container, self._frm_status):
             for i in range(colsp):
                 frm.grid_columnconfigure(i, weight=1)
             for i in range(rowsp):
                 frm.grid_rowconfigure(i, weight=1)
 
@@ -220,15 +219,15 @@
         Reset configuration widgets.
         """
 
         self._frm_config_rate.reset()
         self._frm_config_port.reset()
         self._frm_config_dynamic.reset()
         self._frm_device_info.reset()
-        if self.__app.conn_status != CONNECTED:
+        if self.__app.conn_status not in (CONNECTED, CONNECTED_SOCKET):
             self.set_status("Device not connected", "red")
 
     def set_pending(self, msgid: int, ubxfrm: int):
         """
         Set pending confirmation flag for UBX configuration frame to
         signify that it's waiting for a confirmation message.
 
@@ -265,33 +264,33 @@
                 self._frm_config_dynamic.update_status(msg)
 
             # reset all confirmation flags for this frame
             for msgid in (msg.identity, "ACK-ACK", "ACK-NAK"):
                 if self._pending_confs.get(msgid, None) == ubxfrm:
                     self._pending_confs.pop(msgid)
 
-    def set_status(self, message: str, color: str = "blue"):
+    def set_status(self, message: str, color: str = ""):
         """
         Set status message.
 
         :param str message: message to be displayed
         :param str color: rgb color of text (blue)
         """
 
         message = (message[:120] + "..") if len(message) > 120 else message
-        self._lbl_status.config(fg=color)
+        if color != "":
+            self._lbl_status.config(fg=color)
         self._status.set("  " + message)
 
     def on_exit(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Handle Exit button press.
         """
 
-        # self.__master.update_idletasks()
-        self.__app.stop_ubxconfig_thread()
+        self.__app.stop_dialog(DLGTUBX)
         self.destroy()
 
     def get_size(self):
         """
         Get current frame size.
 
         :return: window size (width, height)
@@ -307,7 +306,38 @@
         Getter for container frame.
 
         :return: reference to container frame
         :rtype: tkinter.Frame
         """
 
         return self._frm_container
+
+    @property
+    def recordmode(self) -> bool:
+        """
+        Getter for recording status.
+
+        :return: recording yes/no
+        :rtype: bool
+        """
+
+        return self._recordmode
+
+    @recordmode.setter
+    def recordmode(self, recordmode: bool):
+        """
+        Setter for record mode.
+
+        :param bool recordmode: recording yes/no
+        """
+
+        self._recordmode = recordmode
+
+    def send_command(self, msg: UBXMessage):
+        """
+        Send command to receiver and record to memory
+        if in 'record' mode.
+        """
+
+        self.__app.gnss_outqueue.put(msg.serialize())
+        if self.recordmode:
+            self._frm_recorder.update_record(msg)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_dynamic_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_dynamic_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,64 +15,64 @@
 
 Created on 17 Aug 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name, too-many-instance-attributes, too-many-ancestors
 
 from tkinter import (
-    Frame,
+    END,
+    LEFT,
+    VERTICAL,
+    Button,
     Canvas,
-    Listbox,
-    Scrollbar,
+    E,
     Entry,
-    Button,
+    Frame,
     Label,
-    StringVar,
-    LEFT,
-    VERTICAL,
+    Listbox,
     N,
     S,
-    E,
+    Scrollbar,
+    StringVar,
     W,
-    END,
 )
-from PIL import ImageTk, Image
+
+from PIL import Image, ImageTk
 from pyubx2 import (
-    UBXMessage,
     POLL,
     SET,
-    UBX_PAYLOADS_SET,
     UBX_PAYLOADS_POLL,
-    atttyp,
+    UBX_PAYLOADS_SET,
     X1,
     X2,
     X4,
     X6,
     X8,
     X24,
+    UBXMessage,
+    atttyp,
 )
+
 from .globals import (
-    ENTCOL,
-    ICON_SEND,
-    ICON_WARNING,
-    ICON_PENDING,
     ICON_CONFIRMED,
+    ICON_PENDING,
+    ICON_SEND,
     ICON_UNKNOWN,
+    ICON_WARNING,
     UBX_CFGOTHER,
 )
-from .strings import LBLCFGDYN
 from .helpers import stringvar2val
+from .strings import LBLCFGGENERIC
 
 # dimensions of scrollable attribute window
 SCROLLX = 300
 SCROLLY = 300
-# following CFG types exluded from selection...
+# following CFG types excluded from selection...
 CFG_EXCLUDED = (
     "CFG-DAT-NUM",  # deprecated
     "CFG-GEOFENCE",  # 'variable by size' groups not yet implemented - use pyubx2
     "CFG-MSG",  # handled via existing CFG-MSG panel
     "CFG-NMEAv0",  # deprecated
     "CFG-NMEAvX",  # deprecated
     "CFG-PRT",  # handled via existing CFG-PRT panel
@@ -95,15 +95,15 @@
         :param Frame app: reference to main tkinter application
         :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self.__container = container
 
         Frame.__init__(self, self.__container.container, *args, **kwargs)
 
         self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
         self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
         self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
@@ -118,21 +118,20 @@
         self.reset()
 
     def _body(self):
         """
         Set up frame and widgets.
         """
 
-        self._lbl_cfg_dyn = Label(self, text=LBLCFGDYN, anchor="w")
+        self._lbl_cfg_dyn = Label(self, text=LBLCFGGENERIC, anchor="w")
         self._lbx_cfg_cmd = Listbox(
             self,
             border=2,
             relief="sunken",
-            bg=ENTCOL,
-            height=6,
+            height=11,
             justify=LEFT,
             exportselection=False,
         )
         self._scr_cfg_cmd = Scrollbar(
             self, orient=VERTICAL, command=self._lbx_cfg_cmd.yview
         )
         self._lbx_cfg_cmd.config(yscrollcommand=self._scr_cfg_cmd.set)
@@ -167,18 +166,18 @@
 
         self._lbl_cfg_dyn.grid(column=0, row=0, columnspan=4, padx=3, sticky=(W, E))
         self._lbx_cfg_cmd.grid(
             column=0, row=1, columnspan=2, rowspan=6, padx=3, pady=3, sticky=(W, E)
         )
         self._scr_cfg_cmd.grid(column=1, row=1, rowspan=6, sticky=(N, S, E))
         self._btn_send_command.grid(
-            column=3, row=1, rowspan=3, ipadx=3, ipady=3, sticky=(W)
+            column=3, row=1, rowspan=3, ipadx=3, ipady=3, sticky=W
         )
         self._lbl_send_command.grid(
-            column=3, row=4, rowspan=3, ipadx=3, ipady=3, sticky=(W)
+            column=3, row=4, rowspan=3, ipadx=3, ipady=3, sticky=W
         )
         self._lbl_command.grid(column=0, row=7, columnspan=4, padx=3, sticky=(W, E))
         self._frm_container.grid(
             column=0, row=8, columnspan=4, rowspan=15, padx=3, sticky=(N, S, W, E)
         )
         self._can_container.grid(
             column=0, row=0, columnspan=3, rowspan=15, padx=3, sticky=(N, S, W, E)
@@ -291,15 +290,14 @@
         :param int row: current row in frame
         :param int index: grouped item index
         :return: last row used
         :rtype: int
         """
 
         for nam, att in pdict.items():  # process each attribute in dict
-
             if isinstance(att, tuple):  # repeating group or bitfield
                 numr, attd = att
                 if numr in (
                     X1,
                     X2,
                     X4,
                     X6,
@@ -344,28 +342,28 @@
             # if numr == "None":
             #     self._cfg_atts[nam] = (StringVar(), U1)
             #     Label(self._frm_attrs, text="Group Size:").grid(
             #         column=0, row=row, sticky=(E)
             #     )
             #     Entry(
             #         self._frm_attrs,
-            #         readonlybackground=ENTCOL,
+            #
             #         textvariable=self._cfg_atts[nam],
             #         relief="sunken",
-            #         bg=ENTCOL,
+            #
             #     ).grid(column=1, row=row, sticky=(W))
             #     Label(self._frm_attrs, text=U1).grid(column=2, row=row, sticky=(W))
             #     row += 1
             #     otherwise add label indicating the integer or existing attribute
             #     which represents the group size
             # else:
             Label(self._frm_attrs, text="Group Size:").grid(
                 column=0, row=row, sticky=(E)
             )
-            Label(self._frm_attrs, text=numr).grid(column=1, row=row, sticky=(W))
+            Label(self._frm_attrs, text=numr).grid(column=1, row=row, sticky=W)
             row += 1
 
         row = self._add_widgets(msg, attd, row, index)
 
         return row
 
     def _add_widgets_single(
@@ -405,50 +403,49 @@
             if nam == "bdsTalkerId":  # fudge for default CFG-NMEA bdsTalkerId
                 if mval == b"\x00\x00":
                     mval = ""
             if atttyp(att) == "X":
                 mval = hex(int.from_bytes(mval, "big"))
             self._cfg_atts[nam][0].set(mval)
 
-        Label(self._frm_attrs, text=nam).grid(column=0, row=row, sticky=(E))
+        Label(self._frm_attrs, text=nam).grid(column=0, row=row, sticky=E)
         Entry(
             self._frm_attrs,
-            readonlybackground=ENTCOL,
             textvariable=self._cfg_atts[nam][0],
             relief="sunken",
-            bg=ENTCOL,
-        ).grid(column=1, row=row, sticky=(W))
-        Label(self._frm_attrs, text=att).grid(column=2, row=row, sticky=(W))
+        ).grid(column=1, row=row, sticky=W)
+        Label(self._frm_attrs, text=att).grid(column=2, row=row, sticky=W)
         row += 1
 
         return row
 
     def _on_send_cfg(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Populate CFG SET message from Entry fields on panel and send to device.
         """
 
         nam = ""
         ent = StringVar().set("")
         try:
-
             # create dict of attribute keyword arguments from
             # Entry field string variables
             vals = {}
-            for (nam, (ent, att)) in self._cfg_atts.items():
+            for nam, (ent, att) in self._cfg_atts.items():
                 val = ent.get()
                 vals[nam] = stringvar2val(val, att)
 
             # create UBXMessage using these keyword arguments
             msg = UBXMessage("CFG", self._cfg_id, SET, **vals)
 
             # send message, update status and await response
-            self.__app.stream_handler.serial_write(msg.serialize())
+            self.__container.send_command(msg)
             self._lbl_send_command.config(image=self._img_pending)
-            self.__container.set_status(f"{self._cfg_id} SET message sent", "blue")
+            self.__container.set_status(
+                f"{self._cfg_id} SET message sent",
+            )
             for msgid in ("ACK-ACK", "ACK-NAK"):
                 self.__container.set_pending(msgid, UBX_CFGOTHER)
 
         except ValueError as err:
             self.__container.set_status(
                 f"INVALID! {nam}, {att}: {err}",
                 "red",
@@ -457,15 +454,19 @@
     def _do_poll_cfg(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Send CFG POLL request (if supported).
         """
 
         if self._cfg_id in UBX_PAYLOADS_POLL:  # CFG is POLLable
             msg = UBXMessage("CFG", self._cfg_id, POLL)
-            self.__app.stream_handler.serial_write(msg.serialize())
-            self.__container.set_status(f"{self._cfg_id} POLL message sent", "blue")
+            self.__container.send_command(msg)
+            self.__container.set_status(
+                f"{self._cfg_id} POLL message sent",
+            )
             self._lbl_send_command.config(image=self._img_pending)
             for msgid in (self._cfg_id, "ACK-NAK"):
                 self.__container.set_pending(msgid, UBX_CFGOTHER)
         else:  # CFG cannot be POLLed
-            self.__container.set_status(f"{self._cfg_id} No POLL available", "blue")
+            self.__container.set_status(
+                f"{self._cfg_id} No POLL available",
+            )
             self._lbl_send_command.config(image=self._img_unknown)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_handler.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
-UBX Protocol handler
+ubx_handler.py
 
-Uses pyubx2 library for parsing
+UBX Protocol handler - handles all incoming UBX messages
+
+Parses individual UBX messages (using pyubx2 library)
+and adds selected attribute values to the app.gnss_status
+data dictionary. This dictionary is then used to periodically
+update the various user-selectable widget panels.
 
 Created on 30 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 from pyubx2 import UBXMessage, itow2utc
-from pygpsclient.globals import GLONASS_NMEA
-from pygpsclient.helpers import svid2gnssid, fix2desc, corrage2int
+
+from pygpsclient.globals import DLGTSPARTN, DLGTUBX, GLONASS_NMEA
+from pygpsclient.helpers import corrage2int, fix2desc, svid2gnssid
+from pygpsclient.widgets import WDGSPECTRUM, WDGSYSMON
 
 
 class UBXHandler:
     """
     UBXHandler class
     """
 
@@ -25,16 +31,17 @@
         """
         Constructor.
 
         :param Frame app: reference to main tkinter application
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
 
+        self._cdb = 0
         self._raw_data = None
         self._parsed_data = None
         self.gsv_data = (
             []
         )  # Holds array of current satellites in view from NMEA GSV or UBX NAV-SVINFO sentences
 
     def process_data(self, raw_data: bytes, parsed_data: object):
@@ -45,61 +52,149 @@
         :param UBXMessage parsed_data: parsed data
         """
 
         if raw_data is None:
             return
 
         if parsed_data.identity[0:3] in ("ACK", "CFG"):
-            self._update_ubxconfig(parsed_data)
+            self._process_ACK(parsed_data)
         elif parsed_data.identity in ("MON-VER", "MON-HW"):
-            self._update_ubxconfig(parsed_data)
+            self._process_MONVER(parsed_data)
         elif parsed_data.identity in ("NAV-POSLLH", "NAV-HPPOSLLH"):
             self._process_NAV_POSLLH(parsed_data)
         elif parsed_data.identity in ("NAV-PVT", "NAV2-PVT"):
             self._process_NAV_PVT(parsed_data)
+        elif parsed_data.identity == "NAV-PVAT":
+            self._process_NAV_PVAT(parsed_data)
         elif parsed_data.identity == "NAV-VELNED":
             self._process_NAV_VELNED(parsed_data)
         elif parsed_data.identity in ("NAV-SAT", "NAV2-SAT"):
             self._process_NAV_SAT(parsed_data)
         elif parsed_data.identity in ("NAV-STATUS", "NAV2-STATUS)"):
             self._process_NAV_STATUS(parsed_data)
+        elif parsed_data.identity == "NAV-SVIN":
+            self._process_NAV_SVIN(parsed_data)
         elif parsed_data.identity == "NAV-SVINFO":
             self._process_NAV_SVINFO(parsed_data)
         elif parsed_data.identity == "NAV-SOL":
             self._process_NAV_SOL(parsed_data)
         elif parsed_data.identity in ("NAV-DOP", "NAV2-DOP"):
             self._process_NAV_DOP(parsed_data)
         elif parsed_data.identity == "HNR-PVT":
             self._process_HNR_PVT(parsed_data)
         elif parsed_data.identity == "RXM-RTCM":
             self._process_RXM_RTCM(parsed_data)
+        elif parsed_data.identity == "MON-SPAN":
+            self._process_MON_SPAN(parsed_data)
+        elif parsed_data.identity == "MON-SYS":
+            self._process_MON_SYS(parsed_data)
+        elif parsed_data.identity == "MON-COMMS":
+            self._process_MON_COMMS(parsed_data)
+        elif parsed_data.identity == "RXM-SPARTN-KEY":
+            self._process_RXM_SPARTN_KEY(parsed_data)
 
-    def _update_ubxconfig(self, msg: UBXMessage):
+    def _process_ACK(self, msg: UBXMessage):
         """
-        Update UBX Config dialog status.
+        Process ACK-ACK & ACK-NAK sentences and CFG poll responses.
 
         :param UBXMessage msg: UBX config message
         """
 
-        if self.__app.dlg_ubxconfig is not None:
-            self.__app.dlg_ubxconfig.update_pending(msg)
+        if self.__app.dialog(DLGTUBX) is not None:
+            self.__app.dialog(DLGTUBX).update_pending(msg)
+
+        # if SPARTN config dialog is open, send CFG & ACKs there
+        if self.__app.dialog(DLGTSPARTN) is not None:
+            self.__app.dialog(DLGTSPARTN).update_pending(msg)
+
+        # if Spectrumview or Sysmon widgets are active, send ACKSs there
+        if msg.identity in ("ACK-ACK", "ACK-NAK"):
+            wdgs = self.__app.widgets
+            for wdg in (WDGSYSMON, WDGSPECTRUM):
+                if wdgs[wdg]["visible"]:
+                    if msg.clsID == 6 and msg.msgID == 1:  # CFG-MSG
+                        getattr(self.__app, wdgs[wdg]["frm"]).update_pending(msg)
+
+    def _process_MONVER(self, msg: UBXMessage):
+        """
+        Process MON-VER & MON-HW sentences.
+
+        :param UBXMessage msg: UBX config message
+        """
+
+        if self.__app.dialog(DLGTUBX) is not None:
+            self.__app.dialog(DLGTUBX).update_pending(msg)
+
+    def _process_MON_SYS(self, data: UBXMessage):
+        """
+        Process MON-SYS sentences - System Monitor Information.
+
+        :param UBXMessage data: MON-SYS parsed message
+        """
+
+        sysdata = {}
+        sysdata["bootType"] = data.bootType
+        sysdata["cpuLoad"] = data.cpuLoad
+        sysdata["cpuLoadMax"] = data.cpuLoadMax
+        sysdata["memUsage"] = data.memUsage
+        sysdata["memUsageMax"] = data.memUsageMax
+        sysdata["ioUsage"] = data.ioUsage
+        sysdata["ioUsageMax"] = data.ioUsageMax
+        sysdata["runTime"] = data.runTime
+        sysdata["noticeCount"] = data.noticeCount
+        sysdata["warnCount"] = data.warnCount
+        sysdata["errorCount"] = data.errorCount
+        sysdata["tempValue"] = data.tempValue
+        self.__app.gnss_status.sysmon_data = sysdata
+
+    def _process_MON_COMMS(self, data: UBXMessage):
+        """
+        Process MON-COMMS sentences - Comms Port Information.
+
+        :param UBXMessage data: MON-COMMS parsed message
+        """
+
+        commsdata = {}
+        for i in range(1, data.nPorts + 1):
+            idx = f"_{i:02}"
+            pid = getattr(data, "portId" + idx)
+            tx = getattr(data, "txUsage" + idx)
+            txmax = getattr(data, "txPeakUsage" + idx)
+            txbytes = getattr(data, "txBytes" + idx)
+            txpending = getattr(data, "txPending" + idx)
+            rx = getattr(data, "rxUsage" + idx)
+            rxmax = getattr(data, "rxPeakUsage" + idx)
+            rxbytes = getattr(data, "rxBytes" + idx)
+            rxpending = getattr(data, "rxPending" + idx)
+            commsdata[pid] = (
+                tx,
+                txmax,
+                txbytes,
+                txpending,
+                rx,
+                rxmax,
+                rxbytes,
+                rxpending,
+            )
+        self.__app.gnss_status.comms_data = commsdata
 
     def _process_NAV_POSLLH(self, data: UBXMessage):
         """
         Process NAV-(HP)POSLLH sentence - Latitude, Longitude, Height.
 
         :param UBXMessage data: NAV-(HP)POSLLH parsed message
         """
 
         self.__app.gnss_status.utc = itow2utc(data.iTOW)  # datetime.time
         self.__app.gnss_status.lat = data.lat
         self.__app.gnss_status.lon = data.lon
         self.__app.gnss_status.alt = data.hMSL / 1000  # meters
         self.__app.gnss_status.hacc = data.hAcc / 1000  # meters
         self.__app.gnss_status.vacc = data.vAcc / 1000  # meters
+        self.__app.gnss_status.sep = (data.height - data.hMSL) / 1000  # meters
 
     def _process_NAV_PVT(self, data: UBXMessage):
         """
         Process NAV-PVT sentence -  Navigation position velocity time solution.
 
         :param UBXMessage data: NAV-PVT parsed message
         """
@@ -110,19 +205,38 @@
         self.__app.gnss_status.alt = data.hMSL / 1000  # meters
         self.__app.gnss_status.hacc = data.hAcc / 1000  # meters
         self.__app.gnss_status.vacc = data.vAcc / 1000  # meters
         self.__app.gnss_status.pdop = data.pDOP
         self.__app.gnss_status.sip = data.numSV
         self.__app.gnss_status.speed = data.gSpeed / 1000  # m/s
         self.__app.gnss_status.track = data.headMot
+        self.__app.gnss_status.sep = (data.height - data.hMSL) / 1000  # meters
         self.__app.gnss_status.fix = fix2desc("NAV-PVT", data.fixType)
+        if data.carrSoln > 0:
+            self.__app.gnss_status.fix = fix2desc("NAV-PVT", data.carrSoln + 5)
+
         self.__app.gnss_status.diff_corr = data.difSoln
         if data.lastCorrectionAge != 0:
             self.__app.gnss_status.diff_age = corrage2int(data.lastCorrectionAge)
 
+    def _process_NAV_PVAT(self, data: UBXMessage):
+        """
+        Process NAV-PVAT sentence -  Navigation position velocity attitude time solution.
+
+        :param UBXMessage data: NAV-PVT parsed message
+        """
+
+        self.__app.gnss_status.utc = itow2utc(data.iTOW)  # datetime.time
+        self.__app.gnss_status.lat = data.lat
+        self.__app.gnss_status.lon = data.lon
+        self.__app.gnss_status.alt = data.hMSL / 1000  # meters
+        self.__app.gnss_status.speed = data.gSpeed / 1000  # m/s
+        self.__app.gnss_status.sip = data.numSV
+        self.__app.gnss_status.sep = (data.height - data.hMSL) / 1000  # meters
+
     def _process_NAV_VELNED(self, data: UBXMessage):
         """
         Process NAV-VELNED sentence - Velocity Solution in North East Down format.
 
         :param UBXMessage data: NAV-VELNED parsed message
         """
 
@@ -137,28 +251,30 @@
         this uses the NMEA SVID numbering range for GLONASS satellites
         (65 - 96) rather than the Slot ID (1-24) by default.
         To change this, set the GLONASS_NMEA flag in globals.py to False.
 
         :param UBXMessage data: NAV-SAT parsed message
         """
 
+        settings = self.__app.frm_settings.config
+        show_unused = settings["unusedsat"]
         self.gsv_data = []
         num_siv = int(data.numSvs)
 
         for i in range(num_siv):
             idx = f"_{i+1:02d}"
             gnssId = getattr(data, "gnssId" + idx)
             svid = getattr(data, "svId" + idx)
             # use NMEA GLONASS numbering (65-96) rather than slotID (1-24)
             if gnssId == 6 and svid < 25 and svid != 255 and GLONASS_NMEA:
                 svid += 64
             elev = getattr(data, "elev" + idx)
             azim = getattr(data, "azim" + idx)
             cno = getattr(data, "cno" + idx)
-            if cno == 0 and not self.__app.frm_settings.show_unused:  # omit unused sats
+            if cno == 0 and not show_unused:  # omit unused sats
                 continue
             self.gsv_data.append((gnssId, svid, elev, azim, cno))
 
         self.__app.gnss_status.siv = len(self.gsv_data)
         self.__app.gnss_status.gsv_data = self.gsv_data
 
     def _process_NAV_STATUS(self, data: UBXMessage):
@@ -167,35 +283,48 @@
 
         :param UBXMessage data: NAV-STATUS parsed message
         """
 
         self.__app.gnss_status.diff_corr = data.diffSoln
         # self.__app.gnss_status.diff_age = "<60"
         self.__app.gnss_status.fix = fix2desc("NAV-STATUS", data.gpsFix)
+        if data.carrSoln > 0:
+            self.__app.gnss_status.fix = fix2desc("NAV-STATUS", data.carrSoln + 5)
+
+    def _process_NAV_SVIN(self, data: UBXMessage):
+        """
+        Process NAV-SVIN sentences - Survey In Status.
+
+        :param UBXMessage data: NAV-SVIN parsed message
+        """
+
+        self.__app.svin_countdown(data.dur, data.valid, data.active)
 
     def _process_NAV_SVINFO(self, data: UBXMessage):
         """
         Process NAV-SVINFO sentences - Space Vehicle Information.
 
         NB: Since UBX Gen8 this message is deprecated in favour of NAV-SAT
 
         :param UBXMessage data: NAV-SVINFO parsed message
         """
 
+        settings = self.__app.frm_settings.config
+        show_unused = settings["unusedsat"]
         self.gsv_data = []
         num_siv = int(data.numCh)
 
         for i in range(num_siv):
             idx = f"_{i+1:02d}"
             svid = getattr(data, "svid" + idx)
             gnssId = svid2gnssid(svid)  # derive gnssId from svid
             elev = getattr(data, "elev" + idx)
             azim = getattr(data, "azim" + idx)
             cno = getattr(data, "cno" + idx)
-            if cno == 0 and not self.__app.frm_settings.show_unused:  # omit unused sats
+            if cno == 0 and not show_unused:  # omit unused sats
                 continue
             self.gsv_data.append((gnssId, svid, elev, azim, cno))
 
         self.__app.gnss_status.gsv_data = self.gsv_data
 
     def _process_NAV_SOL(self, data: UBXMessage):
         """
@@ -231,18 +360,50 @@
         self.__app.gnss_status.lon = data.lon
         self.__app.gnss_status.alt = data.hMSL / 1000  # meters
         self.__app.gnss_status.hacc = data.hAcc / 1000  # meters
         self.__app.gnss_status.vacc = data.vAcc / 1000  # meters
         self.__app.gnss_status.speed = data.gSpeed / 1000  # m/s
         self.__app.gnss_status.track = data.headMot
         self.__app.gnss_status.fix = fix2desc("HNR-PVT", data.gpsFix)
-        self.__app.gnss_status.diff_corr = data.diffSoln
+        self.__app.gnss_status.diff_corr = data.DiffSoln
+        if data.DiffSoln > 0:
+            self.__app.gnss_status.fix = fix2desc("HNR-PVT", 6)
 
     def _process_RXM_RTCM(self, data: UBXMessage):
         """
         Process RXM-RTCM sentences - Status Information.
 
         :param UBXMessage data: RXM-RTCM parsed message
         """
 
         self.__app.gnss_status.diff_corr = data.msgUsed >= 1
         self.__app.gnss_status.diff_station = data.refStation
+
+    def _process_MON_SPAN(self, data: UBXMessage):
+        """
+        Process MON-SPAN sentences - Spectrum Information.
+
+        :param UBXMessage data: MON-SPAN parsed message
+        """
+
+        numrf = data.numRfBlocks
+        rfbs = []
+        for i in range(1, numrf + 1):
+            idx = f"_{i:02}"
+            spec = getattr(data, "spectrum" + idx)
+            spn = getattr(data, "span" + idx)
+            res = getattr(data, "res" + idx)
+            ctr = getattr(data, "center" + idx)
+            pga = getattr(data, "pga" + idx)
+            rfbs.append((spec, spn, res, ctr, pga))
+
+        self.__app.gnss_status.spectrum_data = rfbs
+
+    def _process_RXM_SPARTN_KEY(self, data: UBXMessage):
+        """
+        Process RXM-SPARTN_KEY sentences - poll response.
+
+        :param UBXMessage data: RXM-SPARTN_KEY poll response message
+        """
+
+        if self.__app.dialog(DLGTSPARTN) is not None:
+            self.__app.dialog(DLGTSPARTN).update_pending(data)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_info_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_info_frame.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,37 +3,33 @@
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
-from tkinter import (
-    Frame,
-    Label,
-    StringVar,
-    W,
-)
-from PIL import ImageTk, Image
-from pyubx2 import UBXMessage, POLL
+from tkinter import Frame, Label, W
+
+from PIL import Image, ImageTk
+from pyubx2 import POLL, UBXMessage
+
 from pygpsclient.globals import (
-    INFCOL,
+    CONNECTED,
+    ICON_CONFIRMED,
+    ICON_PENDING,
     ICON_SEND,
     ICON_WARNING,
-    ICON_PENDING,
-    ICON_CONFIRMED,
-    ANTPOWER,
-    ANTSTATUS,
-    UBX_MONVER,
     UBX_MONHW,
-    CONNECTED,
+    UBX_MONVER,
 )
 
+ANTSTATUS = ("INIT", "DONTKNOW", "OK", "SHORT", "OPEN")
+ANTPOWER = ("OFF", "ON", "DONTKNOW")
+
 
 class UBX_INFO_Frame(Frame):
     """
     UBX hardware & firmware information panel.
     """
 
     def __init__(self, app, container, *args, **kwargs):
@@ -43,74 +39,67 @@
         :param Frame app: reference to main tkinter application
         :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self.__container = container
 
         Frame.__init__(self, self.__container.container, *args, **kwargs)
 
         self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
         self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
         self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
         self._img_warn = ImageTk.PhotoImage(Image.open(ICON_WARNING))
-        self._sw_version = StringVar()
-        self._hw_version = StringVar()
-        self._fw_version = StringVar()
-        self._ant_status = StringVar()
-        self._ant_power = StringVar()
-        self._protocol = StringVar()
-        self._gnss_supported = StringVar()
 
         self._body()
         self._do_layout()
         self._attach_events()
 
     def _body(self):
         """
         Set up frame and widgets.
         """
 
         self._lbl_swverl = Label(self, text="Software")
-        self._lbl_swver = Label(self, textvariable=self._sw_version, fg=INFCOL)
+        self._lbl_swver = Label(self)
         self._lbl_hwverl = Label(self, text="Hardware")
-        self._lbl_hwver = Label(self, textvariable=self._hw_version, fg=INFCOL)
+        self._lbl_hwver = Label(self)
         self._lbl_fwverl = Label(self, text="Firmware")
-        self._lbl_fwver = Label(self, textvariable=self._fw_version, fg=INFCOL)
+        self._lbl_fwver = Label(self)
         self._lbl_romverl = Label(self, text="Protocol")
-        self._lbl_romver = Label(self, textvariable=self._protocol, fg=INFCOL)
+        self._lbl_romver = Label(self)
         self._lbl_gnssl = Label(self, text="GNSS/AS")
-        self._lbl_gnss = Label(self, textvariable=self._gnss_supported, fg=INFCOL)
+        self._lbl_gnss = Label(self)
         self._lbl_ant_statusl = Label(self, text="Ant. Status")
-        self._lbl_ant_status = Label(self, textvariable=self._ant_status, fg=INFCOL)
+        self._lbl_ant_status = Label(self)
         self._lbl_ant_powerl = Label(self, text="Ant. Power")
-        self._lbl_ant_power = Label(self, textvariable=self._ant_power, fg=INFCOL)
+        self._lbl_ant_power = Label(self)
 
     def _do_layout(self):
         """
         Layout widgets.
         """
 
-        self._lbl_swverl.grid(column=0, row=0, padx=2, sticky=(W))
-        self._lbl_swver.grid(column=1, row=0, columnspan=2, padx=2, sticky=(W))
-        self._lbl_hwverl.grid(column=3, row=0, padx=2, sticky=(W))
-        self._lbl_hwver.grid(column=4, row=0, columnspan=2, padx=2, sticky=(W))
-        self._lbl_fwverl.grid(column=0, row=1, padx=2, sticky=(W))
-        self._lbl_fwver.grid(column=1, row=1, columnspan=2, padx=2, sticky=(W))
-        self._lbl_romverl.grid(column=3, row=1, padx=2, sticky=(W))
-        self._lbl_romver.grid(column=4, row=1, columnspan=2, padx=2, sticky=(W))
-        self._lbl_gnssl.grid(column=0, row=2, columnspan=1, padx=2, sticky=(W))
-        self._lbl_gnss.grid(column=1, row=2, columnspan=4, padx=2, sticky=(W))
-        self._lbl_ant_statusl.grid(column=0, row=3, columnspan=1, padx=2, sticky=(W))
-        self._lbl_ant_status.grid(column=1, row=3, columnspan=2, padx=2, sticky=(W))
-        self._lbl_ant_powerl.grid(column=3, row=3, columnspan=1, padx=2, sticky=(W))
-        self._lbl_ant_power.grid(column=4, row=3, columnspan=2, padx=2, sticky=(W))
+        self._lbl_swverl.grid(column=0, row=0, padx=2, sticky=W)
+        self._lbl_swver.grid(column=1, row=0, columnspan=2, padx=2, sticky=W)
+        self._lbl_hwverl.grid(column=3, row=0, padx=2, sticky=W)
+        self._lbl_hwver.grid(column=4, row=0, columnspan=2, padx=2, sticky=W)
+        self._lbl_fwverl.grid(column=0, row=1, padx=2, sticky=W)
+        self._lbl_fwver.grid(column=1, row=1, columnspan=2, padx=2, sticky=W)
+        self._lbl_romverl.grid(column=3, row=1, padx=2, sticky=W)
+        self._lbl_romver.grid(column=4, row=1, columnspan=2, padx=2, sticky=W)
+        self._lbl_gnssl.grid(column=0, row=2, columnspan=1, padx=2, sticky=W)
+        self._lbl_gnss.grid(column=1, row=2, columnspan=4, padx=2, sticky=W)
+        self._lbl_ant_statusl.grid(column=0, row=3, columnspan=1, padx=2, sticky=W)
+        self._lbl_ant_status.grid(column=1, row=3, columnspan=2, padx=2, sticky=W)
+        self._lbl_ant_powerl.grid(column=3, row=3, columnspan=1, padx=2, sticky=W)
+        self._lbl_ant_power.grid(column=4, row=3, columnspan=2, padx=2, sticky=W)
 
         (cols, rows) = self.grid_size()
         for i in range(cols):
             self.grid_columnconfigure(i, weight=1)
         for i in range(rows):
             self.grid_rowconfigure(i, weight=1)
         self.option_add("*Font", self.__app.font_sm)
@@ -136,15 +125,14 @@
         Update pending confirmation status.
 
         :param UBXMessage msg: UBX config message
         """
 
         # MON-VER information (for firmware version)
         if msg.identity == "MON-VER":
-
             exts = []
             fw_version = b"n/a"
             protocol = b"n/a"
             gnss_supported = b""
             model = b""
             sw_version = getattr(msg, "swVersion", b"n/a")
             sw_version = sw_version.replace(b"\x00", b"")
@@ -167,34 +155,35 @@
                 if b"MOD=" in exts[i]:
                     model = exts[i].replace(b"MOD=", b"")
                     hw_version = model + b" " + hw_version
                 for gnss in (b"GPS", b"GLO", b"GAL", b"BDS", b"SBAS", b"IMES", b"QZSS"):
                     if gnss in exts[i]:
                         gnss_supported = gnss_supported + gnss + b" "
 
-            self._sw_version.set(sw_version)
-            self._hw_version.set(hw_version)
-            self._fw_version.set(fw_version)
-            self._protocol.set(protocol)
-            self._gnss_supported.set(gnss_supported)
+            self._lbl_swver.config(text=sw_version)
+            self._lbl_hwver.config(text=hw_version)
+            self._lbl_fwver.config(text=fw_version)
+            self._lbl_romver.config(text=protocol)
+            self._lbl_gnss.config(text=gnss_supported)
 
         # MON-HW information (for antenna status)
         if msg.identity == "MON-HW":
-
             ant_status = getattr(msg, "aStatus", 1)
             ant_power = getattr(msg, "aPower", 2)
-            self._ant_status.set(ANTSTATUS[ant_status])
-            self._ant_power.set(ANTPOWER[ant_power])
+            self._lbl_ant_status.config(text=ANTSTATUS[ant_status])
+            self._lbl_ant_power.config(text=ANTPOWER[ant_power])
 
         self.__container.set_status(f"{msg.identity} GET message received", "green")
 
     def _do_poll_ver(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Poll MON-VER & MON-HW
         """
 
         for msgtype in ("MON-VER", "MON-HW"):
             msg = UBXMessage(msgtype[0:3], msgtype, POLL)
-            self.__app.stream_handler.serial.write(msg.serialize())
-            self.__container.set_status(f"{msgtype} POLL message sent", "blue")
+            self.__app.gnss_outqueue.put(msg.serialize())
+            self.__container.set_status(
+                f"{msgtype} POLL message sent",
+            )
         self.__container.set_pending("MON-VER", UBX_MONVER)
         self.__container.set_pending("MON-HW", UBX_MONHW)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_msgrate_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_msgrate_frame.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 
 Created on 22 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 from tkinter import (
-    Frame,
-    Listbox,
-    Spinbox,
-    Scrollbar,
+    LEFT,
+    VERTICAL,
     Button,
-    Label,
+    E,
+    Frame,
     IntVar,
+    Label,
+    Listbox,
     N,
     S,
-    E,
+    Scrollbar,
+    Spinbox,
     W,
-    LEFT,
-    VERTICAL,
-)
-from PIL import ImageTk, Image
-from pyubx2 import (
-    UBXMessage,
-    POLL,
-    SET,
-    UBX_MSGIDS,
 )
-from pyubx2.ubxhelpers import key_from_val, msgclass2bytes
+
+from PIL import Image, ImageTk
+from pyubx2 import POLL, SET, UBX_MSGIDS, UBXMessage
+from pyubx2.ubxhelpers import key_from_val
+
 from pygpsclient.globals import (
-    ENTCOL,
+    ICON_CONFIRMED,
+    ICON_PENDING,
     ICON_SEND,
     ICON_WARNING,
-    ICON_PENDING,
-    ICON_CONFIRMED,
     READONLY,
     UBX_CFGMSG,
 )
 from pygpsclient.strings import LBLCFGMSG
 
 
 class UBX_MSGRATE_Frame(Frame):
@@ -58,15 +53,15 @@
         :param Frame app: reference to main tkinter application
         :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self.__container = container
 
         Frame.__init__(self, self.__container.container, *args, **kwargs)
 
         self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
         self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
         self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
@@ -90,15 +85,14 @@
 
         MAX_RATE = 0xFF
         self._lbl_cfg_msg = Label(self, text=LBLCFGMSG, anchor="w")
         self._lbx_cfg_msg = Listbox(
             self,
             border=2,
             relief="sunken",
-            bg=ENTCOL,
             height=9,
             justify=LEFT,
             exportselection=False,
         )
         self._scr_cfg_msg = Scrollbar(self, orient=VERTICAL)
         self._lbx_cfg_msg.config(yscrollcommand=self._scr_cfg_msg.set)
         self._scr_cfg_msg.config(command=self._lbx_cfg_msg.yview)
@@ -106,55 +100,50 @@
         self._spn_ddc = Spinbox(
             self,
             width=3,
             from_=0,
             to=MAX_RATE,
             textvariable=self._ddc_rate,
             state=READONLY,
-            readonlybackground=ENTCOL,
         )
         self._lbl_uart1 = Label(self, text="UART1")
         self._spn_uart1 = Spinbox(
             self,
             width=3,
             from_=0,
             to=MAX_RATE,
             textvariable=self._uart1_rate,
             state=READONLY,
-            readonlybackground=ENTCOL,
         )
         self._lbl_uart2 = Label(self, text="UART2")
         self._spn_uart2 = Spinbox(
             self,
             width=3,
             from_=0,
             to=MAX_RATE,
             textvariable=self._uart2_rate,
             state=READONLY,
-            readonlybackground=ENTCOL,
         )
         self._lbl_usb = Label(self, text="USB")
         self._spn_usb = Spinbox(
             self,
             width=3,
             from_=0,
             to=MAX_RATE,
             textvariable=self._usb_rate,
             state=READONLY,
-            readonlybackground=ENTCOL,
         )
         self._lbl_spi = Label(self, text="SPI")
         self._spn_spi = Spinbox(
             self,
             width=3,
             from_=0,
             to=MAX_RATE,
             textvariable=self._spi_rate,
             state=READONLY,
-            readonlybackground=ENTCOL,
         )
         self._lbl_send_command = Label(self)
         self._btn_send_command = Button(
             self,
             image=self._img_send,
             width=50,
             fg="green",
@@ -168,29 +157,29 @@
         """
 
         self._lbl_cfg_msg.grid(column=0, row=0, columnspan=6, padx=3, sticky=(W, E))
         self._lbx_cfg_msg.grid(
             column=0, row=1, columnspan=2, rowspan=11, padx=3, pady=3, sticky=(W, E)
         )
         self._scr_cfg_msg.grid(column=1, row=1, rowspan=11, sticky=(N, S, E))
-        self._lbl_ddc.grid(column=2, row=1, rowspan=2, padx=0, pady=1, sticky=(E))
-        self._spn_ddc.grid(column=3, row=1, rowspan=2, padx=0, pady=0, sticky=(W))
-        self._lbl_uart1.grid(column=2, row=3, rowspan=2, padx=0, pady=1, sticky=(E))
-        self._spn_uart1.grid(column=3, row=3, rowspan=2, padx=0, pady=0, sticky=(W))
-        self._lbl_uart2.grid(column=2, row=5, rowspan=2, padx=0, pady=1, sticky=(E))
-        self._spn_uart2.grid(column=3, row=5, rowspan=2, padx=0, pady=0, sticky=(W))
-        self._lbl_usb.grid(column=2, row=7, rowspan=2, padx=0, pady=1, sticky=(E))
-        self._spn_usb.grid(column=3, row=7, rowspan=2, padx=0, pady=0, sticky=(W))
-        self._lbl_spi.grid(column=2, row=9, rowspan=2, padx=0, pady=1, sticky=(E))
-        self._spn_spi.grid(column=3, row=9, rowspan=2, padx=0, pady=0, sticky=(W))
+        self._lbl_ddc.grid(column=2, row=1, rowspan=2, padx=0, pady=1, sticky=E)
+        self._spn_ddc.grid(column=3, row=1, rowspan=2, padx=0, pady=0, sticky=W)
+        self._lbl_uart1.grid(column=2, row=3, rowspan=2, padx=0, pady=1, sticky=E)
+        self._spn_uart1.grid(column=3, row=3, rowspan=2, padx=0, pady=0, sticky=W)
+        self._lbl_uart2.grid(column=2, row=5, rowspan=2, padx=0, pady=1, sticky=E)
+        self._spn_uart2.grid(column=3, row=5, rowspan=2, padx=0, pady=0, sticky=W)
+        self._lbl_usb.grid(column=2, row=7, rowspan=2, padx=0, pady=1, sticky=E)
+        self._spn_usb.grid(column=3, row=7, rowspan=2, padx=0, pady=0, sticky=W)
+        self._lbl_spi.grid(column=2, row=9, rowspan=2, padx=0, pady=1, sticky=E)
+        self._spn_spi.grid(column=3, row=9, rowspan=2, padx=0, pady=0, sticky=W)
         self._btn_send_command.grid(
-            column=4, row=1, rowspan=11, ipadx=3, ipady=3, sticky=(E)
+            column=4, row=1, rowspan=11, ipadx=3, ipady=3, sticky=E
         )
         self._lbl_send_command.grid(
-            column=5, row=1, rowspan=11, ipadx=3, ipady=3, sticky=(E)
+            column=5, row=1, rowspan=11, ipadx=3, ipady=3, sticky=E
         )
 
         (cols, rows) = self.grid_size()
         for i in range(cols):
             self.grid_columnconfigure(i, weight=1)
         for i in range(rows):
             self.grid_rowconfigure(i, weight=1)
@@ -218,15 +207,14 @@
         """
         Update pending confirmation status.
 
         :param UBXMessage msg: UBX config message
         """
 
         if msg.identity == "CFG-MSG":
-
             self.__container.set_status("CFG-MSG GET message received", "green")
             self._ddc_rate.set(msg.rateDDC)
             self._uart1_rate.set(msg.rateUART1)
             self._uart2_rate.set(msg.rateUART2)
             self._usb_rate.set(msg.rateUSB)
             self._spi_rate.set(msg.rateSPI)
             self._lbl_send_command.config(image=self._img_confirmed)
@@ -240,54 +228,58 @@
         CFG-MSG command has been selected.
         """
 
         idx = self._lbx_cfg_msg.curselection()
         self._cfg_msg_command = self._lbx_cfg_msg.get(idx)
 
         # poll selected message configuration to get current message rates
-        msg = key_from_val(UBX_MSGIDS, self._cfg_msg_command)
-        self._do_poll_msg(msg)
+        msgtyp = key_from_val(UBX_MSGIDS, self._cfg_msg_command)
+        self._do_poll_msg(msgtyp)
 
     def _on_send_cfg_msg(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         CFG-MSG command send button has been clicked.
         """
 
-        msg = key_from_val(UBX_MSGIDS, self._cfg_msg_command)
-        msgClass = int.from_bytes(msg[0:1], "little", signed=False)
-        msgID = int.from_bytes(msg[1:2], "little", signed=False)
+        msgtyp = key_from_val(UBX_MSGIDS, self._cfg_msg_command)
+        msgClass = int.from_bytes(msgtyp[0:1], "little", signed=False)
+        msgID = int.from_bytes(msgtyp[1:2], "little", signed=False)
         rateDDC = int(self._ddc_rate.get())
         rateUART1 = int(self._uart1_rate.get())
         rateUART2 = int(self._uart2_rate.get())
         rateUSB = int(self._usb_rate.get())
         rateSPI = int(self._spi_rate.get())
-        data = UBXMessage(
+        msg = UBXMessage(
             "CFG",
             "CFG-MSG",
             SET,
             msgClass=msgClass,
             msgID=msgID,
             rateDDC=rateDDC,
             rateUART1=rateUART1,
             rateUART2=rateUART2,
             rateUSB=rateUSB,
             rateSPI=rateSPI,
         )
-        self.__app.stream_handler.serial_write(data.serialize())
+        self.__container.send_command(msg)
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-MSG SET message sent", "green")
         for msgid in ("ACK-ACK", "ACK-NAK"):
             self.__container.set_pending(msgid, UBX_CFGMSG)
 
-        self._do_poll_msg(msg)
+        self._do_poll_msg(msgtyp)
 
-    def _do_poll_msg(self, msg):
+    def _do_poll_msg(self, msgtyp: bytes):
         """
         Poll message rate.
+
+        :param bytes msgtyp: payload of msgClass, msgID
         """
 
-        data = UBXMessage("CFG", "CFG-MSG", POLL, payload=msg)  # poll for a response
-        self.__app.stream_handler.serial_write(data.serialize())
+        msg = UBXMessage("CFG", "CFG-MSG", POLL, payload=msgtyp)
+        self.__container.send_command(msg)
         self._lbl_send_command.config(image=self._img_pending)
-        self.__container.set_status("CFG-MSG POLL message sent", "blue")
+        self.__container.set_status(
+            "CFG-MSG POLL message sent",
+        )
         for msgid in ("CFG-MSG", "ACK-NAK"):
             self.__container.set_pending(msgid, UBX_CFGMSG)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_port_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_port_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,30 @@
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name, too-many-instance-attributes, too-many-ancestors
 
-from tkinter import (
-    Frame,
-    Checkbutton,
-    Spinbox,
-    Button,
-    Label,
-    StringVar,
-    IntVar,
-    E,
-    W,
-)
-from PIL import ImageTk, Image
-from pyubx2 import (
-    UBXMessage,
-    POLL,
-    SET,
-)
+from tkinter import Button, Checkbutton, E, Frame, IntVar, Label, Spinbox, StringVar, W
+
+from PIL import Image, ImageTk
+from pyubx2 import POLL, SET, UBXMessage
+
 from .globals import (
-    ENTCOL,
+    BPSRATES,
+    CONNECTED,
+    ICON_CONFIRMED,
+    ICON_PENDING,
     ICON_SEND,
     ICON_WARNING,
-    ICON_PENDING,
-    ICON_CONFIRMED,
     PORTIDS,
-    BPSRATES,
     READONLY,
     UBX_CFGPRT,
-    CONNECTED,
 )
 from .strings import LBLCFGPRT
 
 
 class UBX_PORT_Frame(Frame):
     """
     UBX Port and Protocol configuration command panel.
@@ -53,15 +39,15 @@
         :param Frame app: reference to main tkinter application
         :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self.__container = container
 
         Frame.__init__(self, self.__container.container, *args, **kwargs)
 
         self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
         self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
         self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
@@ -90,26 +76,24 @@
         self._lbl_cfg_port = Label(self, text=LBLCFGPRT, anchor="w")
         self._lbl_ubx_portid = Label(self, text="Port ID")
         self._spn_ubx_portid = Spinbox(
             self,
             values=PORTIDS,
             width=8,
             state=READONLY,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._portid,
             command=lambda: self._on_select_portid(),  # pylint: disable=unnecessary-lambda
         )
         self._lbl_ubx_bpsrate = Label(self, text="Rate bps")
         self._spn_ubx_bpsrate = Spinbox(
             self,
             values=(BPSRATES),
             width=6,
             state=READONLY,
-            readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._bpsrate,
         )
         self._lbl_inprot = Label(self, text="Input")
         self._chk_inprot_nmea = Checkbutton(
             self, text="NMEA", variable=self._inprot_nmea
         )
@@ -142,35 +126,35 @@
     def _do_layout(self):
         """
         Layout widgets.
         """
 
         self._lbl_cfg_port.grid(column=0, row=0, columnspan=6, padx=3, sticky=(W, E))
         self._lbl_ubx_portid.grid(
-            column=0, row=1, columnspan=1, rowspan=2, padx=3, sticky=(W)
+            column=0, row=1, columnspan=1, rowspan=2, padx=3, sticky=W
         )
-        self._spn_ubx_portid.grid(column=1, row=1, columnspan=1, rowspan=2, sticky=(W))
+        self._spn_ubx_portid.grid(column=1, row=1, columnspan=1, rowspan=2, sticky=W)
         self._lbl_ubx_bpsrate.grid(
-            column=2, row=1, columnspan=1, rowspan=2, padx=3, sticky=(W)
+            column=2, row=1, columnspan=1, rowspan=2, padx=3, sticky=W
         )
-        self._spn_ubx_bpsrate.grid(column=3, row=1, columnspan=2, rowspan=2, sticky=(W))
-        self._lbl_inprot.grid(column=0, row=3, padx=3, sticky=(W))
-        self._chk_inprot_nmea.grid(column=1, row=3, sticky=(W))
-        self._chk_inprot_ubx.grid(column=2, row=3, sticky=(W))
-        self._chk_inprot_rtcm2.grid(column=3, row=3, sticky=(W))
-        self._chk_inprot_rtcm3.grid(column=4, row=3, sticky=(W))
-        self._lbl_outprot.grid(column=0, row=4, padx=3, sticky=(W))
-        self._chk_outprot_nmea.grid(column=1, row=4, sticky=(W))
-        self._chk_outprot_ubx.grid(column=2, row=4, sticky=(W))
-        self._chk_outprot_rtcm3.grid(column=3, row=4, sticky=(W))
+        self._spn_ubx_bpsrate.grid(column=3, row=1, columnspan=2, rowspan=2, sticky=W)
+        self._lbl_inprot.grid(column=0, row=3, padx=3, sticky=W)
+        self._chk_inprot_nmea.grid(column=1, row=3, sticky=W)
+        self._chk_inprot_ubx.grid(column=2, row=3, sticky=W)
+        self._chk_inprot_rtcm2.grid(column=3, row=3, sticky=W)
+        self._chk_inprot_rtcm3.grid(column=4, row=3, sticky=W)
+        self._lbl_outprot.grid(column=0, row=4, padx=3, sticky=W)
+        self._chk_outprot_nmea.grid(column=1, row=4, sticky=W)
+        self._chk_outprot_ubx.grid(column=2, row=4, sticky=W)
+        self._chk_outprot_rtcm3.grid(column=3, row=4, sticky=W)
         self._btn_send_command.grid(
-            column=4, row=1, rowspan=2, ipadx=3, ipady=3, sticky=(E)
+            column=4, row=1, rowspan=2, ipadx=3, ipady=3, sticky=E
         )
         self._lbl_send_command.grid(
-            column=5, row=1, rowspan=2, ipadx=3, ipady=3, sticky=(E)
+            column=5, row=1, rowspan=2, ipadx=3, ipady=3, sticky=E
         )
 
         (cols, rows) = self.grid_size()
         for i in range(cols):
             self.grid_columnconfigure(i, weight=1)
         for i in range(rows):
             self.grid_rowconfigure(i, weight=1)
@@ -249,26 +233,31 @@
             inNMEA=inNMEA,
             inRTCM=inRTCM,
             inRTCM3=inRTCM3,
             outUBX=outUBX,
             outNMEA=outNMEA,
             outRTCM3=outRTCM3,
         )
-        self.__app.stream_handler.serial_write(msg.serialize())
+        self.__container.send_command(msg)
         self._lbl_send_command.config(image=self._img_pending)
-        self.__container.set_status("CFG-PRT SET message sent", "blue")
-        self.__container.set_pending(UBX_CFGPRT, ("ACK-ACK", "ACK-NAK"))
+        self.__container.set_status(
+            "CFG-PRT SET message sent",
+        )
+        for msgid in ("ACK-NAK", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGPRT)
 
         self._do_poll_prt()
 
     def _do_poll_prt(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Poll PRT message configuration.
         """
 
         portID = int(self._portid.get()[0:1])
         msg = UBXMessage("CFG", "CFG-PRT", POLL, portID=portID)
-        self.__app.stream_handler.serial_write(msg.serialize())
+        self.__container.send_command(msg)
         self._lbl_send_command.config(image=self._img_pending)
-        self.__container.set_status("CFG-PRT POLL message sent", "blue")
+        self.__container.set_status(
+            "CFG-PRT POLL message sent",
+        )
         for msgid in ("CFG-PRT", "ACK-NAK"):
             self.__container.set_pending(msgid, UBX_CFGPRT)
```

### Comparing `PyGPSClient-1.3.9/pygpsclient/ubx_preset_frame.py` & `pygpsclient-1.4.0/src/pygpsclient/ubx_preset_frame.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,73 +3,67 @@
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name, too-many-instance-attributes, too-many-ancestors
 
 from tkinter import (
-    Frame,
-    Listbox,
-    Scrollbar,
+    HORIZONTAL,
+    LEFT,
+    VERTICAL,
     Button,
+    E,
+    Frame,
     Label,
+    Listbox,
     N,
     S,
-    E,
+    Scrollbar,
     W,
-    LEFT,
-    VERTICAL,
-    HORIZONTAL,
-)
-from PIL import ImageTk, Image
-from pyubx2 import (
-    UBXMessage,
-    POLL,
-    SET,
-    UBX_MSGIDS,
-    UBX_PAYLOADS_POLL,
 )
-from .globals import (
-    ENTCOL,
+
+from PIL import Image, ImageTk
+from pyubx2 import POLL, SET, UBX_MSGIDS, UBX_PAYLOADS_POLL, UBXMessage
+
+from pygpsclient.globals import (
+    ICON_CONFIRMED,
+    ICON_PENDING,
     ICON_SEND,
     ICON_WARNING,
-    ICON_PENDING,
-    ICON_CONFIRMED,
     UBX_PRESET,
 )
-from .helpers import ConfirmBox
-from .strings import (
-    LBLPRESET,
+from pygpsclient.helpers import ConfirmBox, setubxrate
+from pygpsclient.strings import (
     DLGRESET,
-    DLGSAVE,
     DLGRESETCONFIRM,
+    DLGSAVE,
     DLGSAVECONFIRM,
-    PSTRESET,
-    PSTSAVE,
-    PSTMINNMEAON,
-    PSTALLNMEAON,
-    PSTALLNMEAOFF,
-    PSTMINUBXON,
-    PSTALLUBXON,
-    PSTALLUBXOFF,
-    PSTALLINFON,
+    LBLPRESET,
     PSTALLINFOFF,
-    PSTALLLOGON,
+    PSTALLINFON,
     PSTALLLOGOFF,
-    PSTALLMONON,
+    PSTALLLOGON,
     PSTALLMONOFF,
-    PSTALLRXMON,
+    PSTALLMONON,
+    PSTALLNMEAOFF,
+    PSTALLNMEAON,
     PSTALLRXMOFF,
-    PSTPOLLPORT,
-    PSTPOLLINFO,
+    PSTALLRXMON,
+    PSTALLUBXOFF,
+    PSTALLUBXON,
+    PSTMINNMEAON,
+    PSTMINUBXON,
     PSTPOLLALLCFG,
     PSTPOLLALLNAV,
+    PSTPOLLINFO,
+    PSTPOLLPORT,
+    PSTRESET,
+    PSTSAVE,
 )
 
 PRESET_COMMMANDS = [
     PSTRESET,
     PSTSAVE,
     PSTMINNMEAON,
     PSTALLNMEAON,
@@ -86,14 +80,17 @@
     PSTALLRXMON,
     PSTALLRXMOFF,
     PSTPOLLPORT,
     PSTPOLLINFO,
     PSTPOLLALLCFG,
     PSTPOLLALLNAV,
 ]
+CANCELLED = 0
+CONFIRMED = 1
+NOMINAL = 2
 
 
 class UBX_PRESET_Frame(Frame):
     """
     UBX Preset and User-defined configuration command panel.
     """
 
@@ -104,24 +101,25 @@
         :param Frame app: reference to main tkinter application
         :param Frame container: reference to container frame (config-dialog)
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
         self.__app = app  # Reference to main application class
-        self.__master = self.__app.get_master()  # Reference to root class (Tk)
+        self.__master = self.__app.appmaster  # Reference to root class (Tk)
         self.__container = container
 
         Frame.__init__(self, self.__container.container, *args, **kwargs)
 
         self._img_send = ImageTk.PhotoImage(Image.open(ICON_SEND))
         self._img_pending = ImageTk.PhotoImage(Image.open(ICON_PENDING))
         self._img_confirmed = ImageTk.PhotoImage(Image.open(ICON_CONFIRMED))
         self._img_warn = ImageTk.PhotoImage(Image.open(ICON_WARNING))
         self._preset_command = None
+        self._configfile = None
         self._body()
         self._do_layout()
         self._attach_events()
         self.reset()
 
     def _body(self):
         """
@@ -129,17 +127,16 @@
         """
 
         self._lbl_presets = Label(self, text=LBLPRESET, anchor="w")
         self._lbx_preset = Listbox(
             self,
             border=2,
             relief="sunken",
-            bg=ENTCOL,
-            height=7,
-            width=30,
+            height=11,
+            width=34,
             justify=LEFT,
             exportselection=False,
         )
         self._scr_presetv = Scrollbar(self, orient=VERTICAL)
         self._scr_preseth = Scrollbar(self, orient=HORIZONTAL)
         self._lbx_preset.config(yscrollcommand=self._scr_presetv.set)
         self._lbx_preset.config(xscrollcommand=self._scr_preseth.set)
@@ -156,18 +153,18 @@
     def _do_layout(self):
         """
         Layout widgets.
         """
 
         self._lbl_presets.grid(column=0, row=0, columnspan=6, padx=3, sticky=(W, E))
         self._lbx_preset.grid(
-            column=0, row=1, columnspan=3, rowspan=8, padx=3, pady=3, sticky=(W, E)
+            column=0, row=1, columnspan=3, rowspan=12, padx=3, pady=3, sticky=(W, E)
         )
-        self._scr_presetv.grid(column=2, row=1, rowspan=8, sticky=(N, S, E))
-        self._scr_preseth.grid(column=0, row=9, columnspan=3, sticky=(W, E))
+        self._scr_presetv.grid(column=2, row=1, rowspan=12, sticky=(N, S, E))
+        self._scr_preseth.grid(column=0, row=13, columnspan=3, sticky=(W, E))
         self._btn_send_command.grid(
             column=3, row=1, rowspan=6, ipadx=3, ipady=3, sticky=(E)
         )
         self._lbl_send_command.grid(
             column=4, row=1, rowspan=6, ipadx=3, ipady=3, sticky=(E)
         )
 
@@ -187,15 +184,15 @@
 
     def reset(self):
         """
         Reset panel.
         """
 
         # Load user-defined presets if there are any
-        self._userpresets = self.__app.file_handler.load_user_presets()
+        self._userpresets = self.__app.app_config.get("ubxpresets", [])
 
         idx = 0
         for pst in PRESET_COMMMANDS:
             self._lbx_preset.insert(idx, pst)
             idx += 1
 
         for upst in self._userpresets:
@@ -211,22 +208,21 @@
         self._preset_command = self._lbx_preset.get(idx)
 
     def _on_send_preset(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Preset command send button has been clicked.
         """
 
-        confirmed = True
+        status = CONFIRMED
         confids = ("MON-VER", "ACK-ACK")
         try:
-
             if self._preset_command == PSTRESET:
-                confirmed = self._do_factory_reset()
+                status = self._do_factory_reset()
             elif self._preset_command == PSTSAVE:
-                confirmed = self._do_save_config()
+                status = self._do_store_config()
             elif self._preset_command == PSTMINNMEAON:
                 self._do_set_minnmea()
             elif self._preset_command == PSTALLNMEAON:
                 self._do_set_allnmea(1)
             elif self._preset_command == PSTALLNMEAOFF:
                 self._do_set_allnmea(0)
             elif self._preset_command == PSTMINUBXON:
@@ -259,21 +255,29 @@
                 self._do_poll_all_CFG()
             elif self._preset_command == PSTPOLLALLNAV:
                 self._do_poll_all_NAV()
             else:
                 confids = ("MON-VER", "ACK-ACK", "ACK-NAK")
                 self._do_user_defined(self._preset_command)
 
-            if confirmed:
+            if status == CONFIRMED:
                 self._lbl_send_command.config(image=self._img_pending)
-                self.__container.set_status("Command(s) sent", "blue")
+                self.__container.set_status(
+                    "Command(s) sent",
+                )
                 for msgid in confids:
                     self.__container.set_pending(msgid, UBX_PRESET)
-            else:
-                self.__container.set_status("Command(s) cancelled", "blue")
+            elif status == CANCELLED:
+                self.__container.set_status(
+                    "Command(s) cancelled",
+                )
+            elif status == NOMINAL:
+                self.__container.set_status(
+                    "Command(s) sent, no results",
+                )
 
         except Exception as err:  # pylint: disable=broad-except
             self.__container.set_status(f"Error {err}", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
     def _do_poll_all_CFG(self):
         """
@@ -284,43 +288,43 @@
             if msgtype[0:3] == "CFG" and msgtype not in (
                 "CFG-INF",
                 "CFG-MSG",
                 "CFG-PRT-IO",
                 "CFG-TP5-TPX",
             ):
                 msg = UBXMessage("CFG", msgtype, POLL)
-                self.__app.stream_handler.serial_write(msg.serialize())
+                self.__container.send_command(msg)
 
     def _do_poll_all_NAV(self):
         """
         Poll all NAV/NAV2 message configurations.
         """
 
         for msgtype in UBX_PAYLOADS_POLL:
             if msgtype[0:3] == "NAV":
                 msg = UBXMessage(msgtype.split("-")[0], msgtype, POLL)
-                self.__app.stream_handler.serial_write(msg.serialize())
+                self.__container.send_command(msg)
 
     def _do_poll_prt(self):
         """
         Poll PRT message configuration for each port.
         """
 
         for portID in range(5):
             msg = UBXMessage("CFG", "CFG-PRT", POLL, portID=portID)
-            self.__app.stream_handler.serial_write(msg.serialize())
+            self.__container.send_command(msg)
 
     def _do_poll_inf(self):
         """
         Poll INF message configuration.
         """
 
         for protid in (0, 1):  # UBX & NMEA
             msg = UBXMessage("CFG", "CFG-INF", POLL, protocolID=protid)
-            self.__app.stream_handler.serial_write(msg.serialize())
+            self.__container.send_command(msg)
 
     def _do_set_inf(self, onoff: int):
         """
         Turn on device information messages INF.
 
         :param int onoff: on/off boolean
         """
@@ -344,15 +348,15 @@
                 + infMsgMaskUART1
                 + infMsgMaskUART2
                 + infMsgMaskUSB
                 + infMsgMaskSPI
                 + reserved2
             )
             msg = UBXMessage("CFG", "CFG-INF", SET, payload=payload)
-            self.__app.stream_handler.serial_write(msg.serialize())
+            self.__container.send_command(msg)
             self._do_poll_inf()  # poll results
 
     def _do_set_log(self, msgrate: int):
         """
         Turn on all device logging messages LOG.
 
         :param int msgrate: message rate (i.e. every nth position solution)
@@ -398,24 +402,22 @@
                 else:
                     self._do_cfgmsg(msgtype, 0)
             if msgtype[0:1] == b"\xf1":  # proprietary NMEA
                 self._do_cfgmsg(msgtype, 0)
 
     def _do_set_minNAV(self):
         """
-        Turn on minimum set of UBX-NAV messages (PVT & SVINFO).
+        Turn on minimum set of UBX-NAV messages (DOP, PVT, & SAT).
         """
 
         for msgtype in UBX_MSGIDS:
             if msgtype[0:1] == b"\x01":  # UBX-NAV
                 if msgtype == b"\x01\x07":  # NAV-PVT
                     self._do_cfgmsg(msgtype, 1)
-                #                 elif msgtype == b"\x01\x30":  # NAV-SVINFO (deprecated)
-                #                     self._do_cfgmsg(msgtype, 4)
-                elif msgtype == b"\x01\x35":  # NAV-SAT
+                elif msgtype in (b"\x01\x04", b"\x01\x35"):  # NAV-DOP, NAV-SAT
                     self._do_cfgmsg(msgtype, 4)
                 else:
                     self._do_cfgmsg(msgtype, 0)
 
     def _do_set_allnmea(self, msgrate):
         """
         Turn on all NMEA messages.
@@ -438,36 +440,21 @@
             if msgtype[0:1] == b"\x01":
                 self._do_cfgmsg(msgtype, msgrate)
 
     def _do_cfgmsg(self, msgtype: str, msgrate: int):
         """
         Set rate for specified message type via CFG-MSG.
 
-        NB A rate of n means 'for every nth position solution',
-        so values > 1 mean the message is sent less often.
-
         :param str msgtype: type of config message
         :param int msgrate: message rate (i.e. every nth position solution)
         """
 
         msgClass = int.from_bytes(msgtype[0:1], "little", signed=False)
         msgID = int.from_bytes(msgtype[1:2], "little", signed=False)
-        msg = UBXMessage(
-            "CFG",
-            "CFG-MSG",
-            SET,
-            msgClass=msgClass,
-            msgID=msgID,
-            rateDDC=msgrate,
-            rateUART1=msgrate,
-            rateUART2=msgrate,
-            rateUSB=msgrate,
-            rateSPI=msgrate,
-        )
-        self.__app.stream_handler.serial_write(msg.serialize())
+        setubxrate(self.__app, msgClass, msgID, msgrate)
 
     def _do_factory_reset(self) -> bool:
         """
         Restore to factory defaults stored in battery-backed RAM
         but display confirmation message box first.
 
         :return: boolean signifying whether OK was pressed
@@ -482,22 +469,22 @@
                 clearMask=b"\x1f\x1f\x00\x00",
                 # saveMask=b"\x1f\x1f\x00\x00",
                 loadMask=b"\x1f\x1f\x00\x00",
                 devBBR=1,
                 devFlash=1,
                 devEEPROM=1,
             )
-            self.__app.stream_handler.serial_write(msg.serialize())
-            return True
+            self.__container.send_command(msg)
+            return CONFIRMED
 
-        return False
+        return CANCELLED
 
-    def _do_save_config(self) -> bool:
+    def _do_store_config(self) -> bool:
         """
-        Save current configuration to persistent storage
+        Store current configuration in persistent storage
         but display confirmation message box first.
 
         :return: boolean signifying whether OK was pressed
         :rtype: bool
         """
 
         if ConfirmBox(self, DLGSAVE, DLGSAVECONFIRM).show():
@@ -508,18 +495,18 @@
                 # clearMask=b"\x01\x00\x00\x00",
                 saveMask=b"\x1f\x1f\x00\x00",
                 # loadMask=b"\x01\x00\x00\x00",
                 devBBR=1,
                 devFlash=1,
                 devEEPROM=1,
             )
-            self.__app.stream_handler.serial_write(msg.serialize())
-            return True
+            self.__container.send_command(msg)
+            return CONFIRMED
 
-        return False
+        return CANCELLED
 
     def _do_user_defined(self, command: str):
         """
         Parse and send user-defined command(s).
 
         This could result in any number of errors if the
         uxbpresets file contains garbage, so there's a broad
@@ -536,15 +523,15 @@
                 payload = seg[i + 2].strip()
                 mode = int(seg[i + 3].rstrip("\r\n"))
                 if payload != "":
                     payload = bytes(bytearray.fromhex(payload))
                     msg = UBXMessage(ubx_class, ubx_id, mode, payload=payload)
                 else:
                     msg = UBXMessage(ubx_class, ubx_id, mode)
-                self.__app.stream_handler.serial_write(msg.serialize())
+                self.__container.send_command(msg)
         except Exception as err:  # pylint: disable=broad-except
             self.__app.set_status(f"Error {err}", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
     def update_status(self, msg: UBXMessage):
         """
         Update pending confirmation status.
```

