# Comparing `tmp/micrologai-1.3.6.tar.gz` & `tmp/micrologai-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrologai-1.3.6.tar", last modified: Thu Aug  3 07:36:40 2023, max compression
+gzip compressed data, was "micrologai-1.3.7.tar", last modified: Thu Aug  3 08:03:16 2023, max compression
```

## Comparing `micrologai-1.3.6.tar` & `micrologai-1.3.7.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.885345 micrologai-1.3.6/
--rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.6/LICENSE
--rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.6/MANIFEST.in
--rw-r--r--   0 laffra     (501) staff       (20)    46802 2023-08-03 07:36:40.892168 micrologai-1.3.6/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)    11162 2023-07-31 16:21:51.000000 micrologai-1.3.6/README.md
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.006170 micrologai-1.3.6/dashboard/
--rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.6/dashboard/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    12401 2023-07-27 20:00:40.000000 micrologai-1.3.6/dashboard/canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.6/dashboard/colors.py
--rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.6/dashboard/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     8571 2023-07-27 07:37:34.000000 micrologai-1.3.6/dashboard/design.py
--rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.6/dashboard/dialog.py
--rw-r--r--   0 laffra     (501) staff       (20)    14005 2023-08-02 14:24:49.000000 micrologai-1.3.6/dashboard/main.py
--rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.6/dashboard/markdown.py
--rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.6/dashboard/profiler.py
--rw-r--r--   0 laffra     (501) staff       (20)     2233 2023-07-31 16:28:15.000000 micrologai-1.3.6/dashboard/tips.py
--rw-r--r--   0 laffra     (501) staff       (20)     4396 2023-07-30 20:29:02.000000 micrologai-1.3.6/dashboard/treeview.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.052437 micrologai-1.3.6/dashboard/views/
--rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.6/dashboard/views/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    15841 2023-08-01 09:55:10.000000 micrologai-1.3.6/dashboard/views/call.py
--rw-r--r--   0 laffra     (501) staff       (20)     5222 2023-07-29 10:41:01.000000 micrologai-1.3.6/dashboard/views/marker.py
--rw-r--r--   0 laffra     (501) staff       (20)     4416 2023-07-26 13:59:52.000000 micrologai-1.3.6/dashboard/views/status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.6/dashboard/views/timeline.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.178133 micrologai-1.3.6/examples/
--rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.6/examples/binaryTrees.py
--rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.6/examples/books.json
--rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.6/examples/bookstore.py
--rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.6/examples/dataframes.py
--rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.6/examples/example.py
--rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.6/examples/files.py
--rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.6/examples/go.py
--rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.6/examples/helloworld.py
--rw-r--r--   0 laffra     (501) staff       (20)     1361 2023-08-01 08:23:56.000000 micrologai-1.3.6/examples/memory.py
--rw-r--r--   0 laffra     (501) staff       (20)      970 2023-07-29 20:25:44.000000 micrologai-1.3.6/examples/modules.py
--rwxr-xr-x   0 laffra     (501) staff       (20)      729 2023-08-01 08:27:55.000000 micrologai-1.3.6/examples/runall.sh
--rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.6/examples/startstop.py
--rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.6/examples/threads.py
--rw-r--r--   0 laffra     (501) staff       (20)    94019 2023-07-31 09:16:43.000000 micrologai-1.3.6/examples/treemap.ipynb
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.253772 micrologai-1.3.6/microlog/
--rw-r--r--   0 laffra     (501) staff       (20)     1018 2023-08-02 12:29:58.000000 micrologai-1.3.6/microlog/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)     2821 2023-08-02 12:29:03.000000 micrologai-1.3.6/microlog/api.py
--rw-r--r--   0 laffra     (501) staff       (20)      873 2023-08-02 11:46:19.000000 micrologai-1.3.6/microlog/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.6/microlog/explain.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.485539 micrologai-1.3.6/microlog/images/
--rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.6/microlog/images/anomaly.png
--rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.6/microlog/images/apple-touch-icon.png
--rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.6/microlog/images/chatgpt.png
--rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.6/microlog/images/design-go.png
--rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.6/microlog/images/dialog.png
--rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.6/microlog/images/error-log.png
--rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.6/microlog/images/favicon-16x16.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.6/microlog/images/favicon-32x32.png
--rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.6/microlog/images/fd-leak.png
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.731935 micrologai-1.3.6/microlog/images/icons/
--rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.6/microlog/images/icons/asyncio.png
--rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.6/microlog/images/icons/dataclasses.png
--rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.6/microlog/images/icons/email.png
--rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.6/microlog/images/icons/google.png
--rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.6/microlog/images/icons/guppy.png
--rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.6/microlog/images/icons/http.png
--rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.6/microlog/images/icons/jupyter.png
--rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.6/microlog/images/icons/matplotlib.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.6/microlog/images/icons/microlog.png
--rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.6/microlog/images/icons/networkx.png
--rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.6/microlog/images/icons/numpy.png
--rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.6/microlog/images/icons/pandas.png
--rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.6/microlog/images/icons/pyparsing.png
--rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.6/microlog/images/icons/pytest.png
--rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.6/microlog/images/icons/python.png
--rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.6/microlog/images/icons/re.png
--rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.6/microlog/images/icons/squarify.png
--rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.6/microlog/images/icons/ssl.png
--rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.6/microlog/images/icons/tornado.png
--rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.6/microlog/images/icons/urllib.png
--rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.6/microlog/images/icons/wsgi.png
--rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.6/microlog/images/icons/zmq.png
--rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.6/microlog/images/log.png
--rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.6/microlog/images/logo-bing.png
--rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.6/microlog/images/logo-brave.png
--rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.6/microlog/images/logo-duckduckgo.png
--rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.6/microlog/images/logo-google.png
--rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.6/microlog/images/logo-hackernews.png
--rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.6/microlog/images/logo-sourcegraph.png
--rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.6/microlog/images/logo-stackoverflow.png
--rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.6/microlog/images/logo-twitter.png
--rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.6/microlog/images/markdown.png
--rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.6/microlog/images/memory-leak.png
--rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.6/microlog/images/overview.png
--rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.6/microlog/images/spinner.png
--rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.6/microlog/images/status.png
--rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.6/microlog/images/tips.png
--rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.6/microlog/images/zoomedin.png
--rw-r--r--   0 laffra     (501) staff       (20)     5518 2023-08-03 07:34:38.000000 micrologai-1.3.6/microlog/log.py
--rw-r--r--   0 laffra     (501) staff       (20)     9741 2023-07-28 08:12:21.000000 micrologai-1.3.6/microlog/models.py
--rw-r--r--   0 laffra     (501) staff       (20)     6190 2023-07-31 18:51:32.000000 micrologai-1.3.6/microlog/server.py
--rw-r--r--   0 laffra     (501) staff       (20)      595 2023-07-30 16:11:01.000000 micrologai-1.3.6/microlog/sitecustomize.py
--rw-r--r--   0 laffra     (501) staff       (20)    19661 2023-08-02 12:14:02.000000 micrologai-1.3.6/microlog/tracer.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.801051 micrologai-1.3.6/micrologai.egg-info/
--rw-r--r--   0 laffra     (501) staff       (20)    46802 2023-08-03 07:36:39.000000 micrologai-1.3.6/micrologai.egg-info/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)     2801 2023-08-03 07:36:39.000000 micrologai-1.3.6/micrologai.egg-info/SOURCES.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-08-03 07:36:39.000000 micrologai-1.3.6/micrologai.egg-info/dependency_links.txt
--rw-r--r--   0 laffra     (501) staff       (20)       48 2023-08-03 07:36:39.000000 micrologai-1.3.6/micrologai.egg-info/entry_points.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-30 10:03:22.000000 micrologai-1.3.6/micrologai.egg-info/not-zip-safe
--rw-r--r--   0 laffra     (501) staff       (20)       41 2023-08-03 07:36:39.000000 micrologai-1.3.6/micrologai.egg-info/requires.txt
--rw-r--r--   0 laffra     (501) staff       (20)       19 2023-08-03 07:36:39.000000 micrologai-1.3.6/micrologai.egg-info/top_level.txt
--rw-r--r--   0 laffra     (501) staff       (20)      893 2023-08-01 15:35:25.000000 micrologai-1.3.6/pyproject.toml
--rw-r--r--   0 laffra     (501) staff       (20)       79 2023-08-03 07:36:40.906944 micrologai-1.3.6/setup.cfg
--rw-r--r--   0 laffra     (501) staff       (20)     1765 2023-08-01 15:35:25.000000 micrologai-1.3.6/setup.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 07:36:40.880194 micrologai-1.3.6/tests/
--rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.6/tests/test_call_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.6/tests/test_canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.6/tests/test_log.py
--rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.6/tests/test_marker_view.py
--rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.6/tests/test_print.py
--rw-r--r--   0 laffra     (501) staff       (20)      740 2023-07-30 08:56:08.000000 micrologai-1.3.6/tests/test_status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.6/tests/test_status_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.6/tests/test_tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:16.543926 micrologai-1.3.7/
+-rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.7/LICENSE
+-rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.7/MANIFEST.in
+-rw-r--r--   0 laffra     (501) staff       (20)    46802 2023-08-03 08:03:16.551498 micrologai-1.3.7/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)    11162 2023-07-31 16:21:51.000000 micrologai-1.3.7/README.md
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:15.176016 micrologai-1.3.7/dashboard/
+-rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.7/dashboard/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    12401 2023-07-27 20:00:40.000000 micrologai-1.3.7/dashboard/canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.7/dashboard/colors.py
+-rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.7/dashboard/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     8571 2023-07-27 07:37:34.000000 micrologai-1.3.7/dashboard/design.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.7/dashboard/dialog.py
+-rw-r--r--   0 laffra     (501) staff       (20)    14005 2023-08-02 14:24:49.000000 micrologai-1.3.7/dashboard/main.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.7/dashboard/markdown.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.7/dashboard/profiler.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2233 2023-07-31 16:28:15.000000 micrologai-1.3.7/dashboard/tips.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4396 2023-07-30 20:29:02.000000 micrologai-1.3.7/dashboard/treeview.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:15.220759 micrologai-1.3.7/dashboard/views/
+-rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.7/dashboard/views/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    15841 2023-08-01 09:55:10.000000 micrologai-1.3.7/dashboard/views/call.py
+-rw-r--r--   0 laffra     (501) staff       (20)     5222 2023-07-29 10:41:01.000000 micrologai-1.3.7/dashboard/views/marker.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4416 2023-07-26 13:59:52.000000 micrologai-1.3.7/dashboard/views/status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.7/dashboard/views/timeline.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:15.367153 micrologai-1.3.7/examples/
+-rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.7/examples/binaryTrees.py
+-rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.7/examples/books.json
+-rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.7/examples/bookstore.py
+-rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.7/examples/dataframes.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.7/examples/example.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.7/examples/files.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.7/examples/go.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.7/examples/helloworld.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1361 2023-08-01 08:23:56.000000 micrologai-1.3.7/examples/memory.py
+-rw-r--r--   0 laffra     (501) staff       (20)      970 2023-07-29 20:25:44.000000 micrologai-1.3.7/examples/modules.py
+-rwxr-xr-x   0 laffra     (501) staff       (20)      729 2023-08-01 08:27:55.000000 micrologai-1.3.7/examples/runall.sh
+-rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.7/examples/startstop.py
+-rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.7/examples/threads.py
+-rw-r--r--   0 laffra     (501) staff       (20)    94019 2023-08-03 07:47:45.000000 micrologai-1.3.7/examples/treemap.ipynb
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:15.480217 micrologai-1.3.7/microlog/
+-rw-r--r--   0 laffra     (501) staff       (20)      339 2023-08-03 08:02:57.000000 micrologai-1.3.7/microlog/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2821 2023-08-02 12:29:03.000000 micrologai-1.3.7/microlog/api.py
+-rw-r--r--   0 laffra     (501) staff       (20)      873 2023-08-02 11:46:19.000000 micrologai-1.3.7/microlog/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.7/microlog/explain.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:15.988866 micrologai-1.3.7/microlog/images/
+-rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.7/microlog/images/anomaly.png
+-rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.7/microlog/images/apple-touch-icon.png
+-rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.7/microlog/images/chatgpt.png
+-rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.7/microlog/images/design-go.png
+-rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.7/microlog/images/dialog.png
+-rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.7/microlog/images/error-log.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.7/microlog/images/favicon-16x16.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.7/microlog/images/favicon-32x32.png
+-rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.7/microlog/images/fd-leak.png
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:16.297051 micrologai-1.3.7/microlog/images/icons/
+-rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.7/microlog/images/icons/asyncio.png
+-rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.7/microlog/images/icons/dataclasses.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.7/microlog/images/icons/email.png
+-rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.7/microlog/images/icons/google.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.7/microlog/images/icons/guppy.png
+-rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.7/microlog/images/icons/http.png
+-rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.7/microlog/images/icons/jupyter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.7/microlog/images/icons/matplotlib.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.7/microlog/images/icons/microlog.png
+-rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.7/microlog/images/icons/networkx.png
+-rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.7/microlog/images/icons/numpy.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.7/microlog/images/icons/pandas.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.7/microlog/images/icons/pyparsing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.7/microlog/images/icons/pytest.png
+-rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.7/microlog/images/icons/python.png
+-rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.7/microlog/images/icons/re.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.7/microlog/images/icons/squarify.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.7/microlog/images/icons/ssl.png
+-rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.7/microlog/images/icons/tornado.png
+-rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.7/microlog/images/icons/urllib.png
+-rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.7/microlog/images/icons/wsgi.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.7/microlog/images/icons/zmq.png
+-rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.7/microlog/images/log.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.7/microlog/images/logo-bing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.7/microlog/images/logo-brave.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.7/microlog/images/logo-duckduckgo.png
+-rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.7/microlog/images/logo-google.png
+-rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.7/microlog/images/logo-hackernews.png
+-rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.7/microlog/images/logo-sourcegraph.png
+-rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.7/microlog/images/logo-stackoverflow.png
+-rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.7/microlog/images/logo-twitter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.7/microlog/images/markdown.png
+-rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.7/microlog/images/memory-leak.png
+-rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.7/microlog/images/overview.png
+-rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.7/microlog/images/spinner.png
+-rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.7/microlog/images/status.png
+-rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.7/microlog/images/tips.png
+-rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.7/microlog/images/zoomedin.png
+-rw-r--r--   0 laffra     (501) staff       (20)     5518 2023-08-03 07:34:38.000000 micrologai-1.3.7/microlog/log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     9741 2023-07-28 08:12:21.000000 micrologai-1.3.7/microlog/models.py
+-rw-r--r--   0 laffra     (501) staff       (20)      942 2023-08-03 08:02:13.000000 micrologai-1.3.7/microlog/pyscript.py
+-rw-r--r--   0 laffra     (501) staff       (20)     6190 2023-07-31 18:51:32.000000 micrologai-1.3.7/microlog/server.py
+-rw-r--r--   0 laffra     (501) staff       (20)      595 2023-07-30 16:11:01.000000 micrologai-1.3.7/microlog/sitecustomize.py
+-rw-r--r--   0 laffra     (501) staff       (20)    19661 2023-08-02 12:14:02.000000 micrologai-1.3.7/microlog/tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:16.410889 micrologai-1.3.7/micrologai.egg-info/
+-rw-r--r--   0 laffra     (501) staff       (20)    46802 2023-08-03 08:03:14.000000 micrologai-1.3.7/micrologai.egg-info/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)     2822 2023-08-03 08:03:14.000000 micrologai-1.3.7/micrologai.egg-info/SOURCES.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-08-03 08:03:14.000000 micrologai-1.3.7/micrologai.egg-info/dependency_links.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       48 2023-08-03 08:03:14.000000 micrologai-1.3.7/micrologai.egg-info/entry_points.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-30 10:03:22.000000 micrologai-1.3.7/micrologai.egg-info/not-zip-safe
+-rw-r--r--   0 laffra     (501) staff       (20)       41 2023-08-03 08:03:14.000000 micrologai-1.3.7/micrologai.egg-info/requires.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       19 2023-08-03 08:03:14.000000 micrologai-1.3.7/micrologai.egg-info/top_level.txt
+-rw-r--r--   0 laffra     (501) staff       (20)      893 2023-08-03 08:02:57.000000 micrologai-1.3.7/pyproject.toml
+-rw-r--r--   0 laffra     (501) staff       (20)       79 2023-08-03 08:03:16.562939 micrologai-1.3.7/setup.cfg
+-rw-r--r--   0 laffra     (501) staff       (20)     1765 2023-08-03 08:02:57.000000 micrologai-1.3.7/setup.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-03 08:03:16.536137 micrologai-1.3.7/tests/
+-rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.7/tests/test_call_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.7/tests/test_canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.7/tests/test_log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.7/tests/test_marker_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.7/tests/test_print.py
+-rw-r--r--   0 laffra     (501) staff       (20)      740 2023-07-30 08:56:08.000000 micrologai-1.3.7/tests/test_status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.7/tests/test_status_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.7/tests/test_tracer.py
```

### Comparing `micrologai-1.3.6/LICENSE` & `micrologai-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/PKG-INFO` & `micrologai-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.6
+Version: 1.3.7
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
```

### Comparing `micrologai-1.3.6/README.md` & `micrologai-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/canvas.py` & `micrologai-1.3.7/dashboard/canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/colors.py` & `micrologai-1.3.7/dashboard/colors.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/config.py` & `micrologai-1.3.7/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/design.py` & `micrologai-1.3.7/dashboard/design.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/dialog.py` & `micrologai-1.3.7/dashboard/dialog.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/main.py` & `micrologai-1.3.7/dashboard/main.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/markdown.py` & `micrologai-1.3.7/dashboard/markdown.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/profiler.py` & `micrologai-1.3.7/dashboard/profiler.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/tips.py` & `micrologai-1.3.7/dashboard/tips.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/treeview.py` & `micrologai-1.3.7/dashboard/treeview.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/views/__init__.py` & `micrologai-1.3.7/dashboard/views/__init__.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/views/call.py` & `micrologai-1.3.7/dashboard/views/call.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/views/marker.py` & `micrologai-1.3.7/dashboard/views/marker.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/views/status.py` & `micrologai-1.3.7/dashboard/views/status.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/dashboard/views/timeline.py` & `micrologai-1.3.7/dashboard/views/timeline.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/binaryTrees.py` & `micrologai-1.3.7/examples/binaryTrees.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/books.json` & `micrologai-1.3.7/examples/books.json`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/bookstore.py` & `micrologai-1.3.7/examples/bookstore.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/dataframes.py` & `micrologai-1.3.7/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/example.py` & `micrologai-1.3.7/examples/example.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/files.py` & `micrologai-1.3.7/examples/files.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/go.py` & `micrologai-1.3.7/examples/go.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/helloworld.py` & `micrologai-1.3.7/examples/helloworld.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/memory.py` & `micrologai-1.3.7/examples/memory.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/modules.py` & `micrologai-1.3.7/examples/modules.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/runall.sh` & `micrologai-1.3.7/examples/runall.sh`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/startstop.py` & `micrologai-1.3.7/examples/startstop.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/threads.py` & `micrologai-1.3.7/examples/threads.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/examples/treemap.ipynb` & `micrologai-1.3.7/examples/treemap.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.-1.-1'}}"}*

```diff
@@ -220,14 +220,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.-1.-1"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `micrologai-1.3.6/microlog/api.py` & `micrologai-1.3.7/microlog/api.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/config.py` & `micrologai-1.3.7/microlog/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/explain.py` & `micrologai-1.3.7/microlog/explain.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/anomaly.png` & `micrologai-1.3.7/microlog/images/anomaly.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/apple-touch-icon.png` & `micrologai-1.3.7/microlog/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/chatgpt.png` & `micrologai-1.3.7/microlog/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/design-go.png` & `micrologai-1.3.7/microlog/images/design-go.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/dialog.png` & `micrologai-1.3.7/microlog/images/dialog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/error-log.png` & `micrologai-1.3.7/microlog/images/error-log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/favicon-32x32.png` & `micrologai-1.3.7/microlog/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/fd-leak.png` & `micrologai-1.3.7/microlog/images/fd-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/asyncio.png` & `micrologai-1.3.7/microlog/images/icons/asyncio.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/dataclasses.png` & `micrologai-1.3.7/microlog/images/icons/dataclasses.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/email.png` & `micrologai-1.3.7/microlog/images/icons/email.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/google.png` & `micrologai-1.3.7/microlog/images/icons/google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/guppy.png` & `micrologai-1.3.7/microlog/images/icons/guppy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/http.png` & `micrologai-1.3.7/microlog/images/icons/http.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/jupyter.png` & `micrologai-1.3.7/microlog/images/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/matplotlib.png` & `micrologai-1.3.7/microlog/images/icons/matplotlib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/microlog.png` & `micrologai-1.3.7/microlog/images/icons/microlog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/networkx.png` & `micrologai-1.3.7/microlog/images/icons/networkx.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/numpy.png` & `micrologai-1.3.7/microlog/images/icons/numpy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/pandas.png` & `micrologai-1.3.7/microlog/images/icons/pandas.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/pyparsing.png` & `micrologai-1.3.7/microlog/images/icons/pyparsing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/pytest.png` & `micrologai-1.3.7/microlog/images/icons/pytest.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/python.png` & `micrologai-1.3.7/microlog/images/icons/python.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/re.png` & `micrologai-1.3.7/microlog/images/icons/re.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/squarify.png` & `micrologai-1.3.7/microlog/images/icons/squarify.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/ssl.png` & `micrologai-1.3.7/microlog/images/icons/ssl.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/tornado.png` & `micrologai-1.3.7/microlog/images/icons/tornado.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/urllib.png` & `micrologai-1.3.7/microlog/images/icons/urllib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/wsgi.png` & `micrologai-1.3.7/microlog/images/icons/wsgi.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/icons/zmq.png` & `micrologai-1.3.7/microlog/images/icons/zmq.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/log.png` & `micrologai-1.3.7/microlog/images/log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-bing.png` & `micrologai-1.3.7/microlog/images/logo-bing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-brave.png` & `micrologai-1.3.7/microlog/images/logo-brave.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-duckduckgo.png` & `micrologai-1.3.7/microlog/images/logo-duckduckgo.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-google.png` & `micrologai-1.3.7/microlog/images/logo-google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-hackernews.png` & `micrologai-1.3.7/microlog/images/logo-hackernews.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-sourcegraph.png` & `micrologai-1.3.7/microlog/images/logo-sourcegraph.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-stackoverflow.png` & `micrologai-1.3.7/microlog/images/logo-stackoverflow.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/logo-twitter.png` & `micrologai-1.3.7/microlog/images/logo-twitter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/markdown.png` & `micrologai-1.3.7/microlog/images/markdown.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/memory-leak.png` & `micrologai-1.3.7/microlog/images/memory-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/overview.png` & `micrologai-1.3.7/microlog/images/overview.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/status.png` & `micrologai-1.3.7/microlog/images/status.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/tips.png` & `micrologai-1.3.7/microlog/images/tips.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/images/zoomedin.png` & `micrologai-1.3.7/microlog/images/zoomedin.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/log.py` & `micrologai-1.3.7/microlog/log.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/models.py` & `micrologai-1.3.7/microlog/models.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/server.py` & `micrologai-1.3.7/microlog/server.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/sitecustomize.py` & `micrologai-1.3.7/microlog/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/microlog/tracer.py` & `micrologai-1.3.7/microlog/tracer.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/micrologai.egg-info/PKG-INFO` & `micrologai-1.3.7/micrologai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.6
+Version: 1.3.7
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
```

### Comparing `micrologai-1.3.6/micrologai.egg-info/SOURCES.txt` & `micrologai-1.3.7/micrologai.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 examples/treemap.ipynb
 microlog/__init__.py
 microlog/api.py
 microlog/config.py
 microlog/explain.py
 microlog/log.py
 microlog/models.py
+microlog/pyscript.py
 microlog/server.py
 microlog/sitecustomize.py
 microlog/tracer.py
 microlog/images/anomaly.png
 microlog/images/apple-touch-icon.png
 microlog/images/chatgpt.png
 microlog/images/design-go.png
```

### Comparing `micrologai-1.3.6/pyproject.toml` & `micrologai-1.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micrologai"
-version = "1.3.6"
+version = "1.3.7"
 description = "A continuous profiler and logger for Python written entirely in Python"
 readme = "README.md"
 authors = [{ name = "Chris Laffra", email = "chris@chrislaffra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `micrologai-1.3.6/setup.py` & `micrologai-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='Microlog',
     description='A continuous profiler and logger for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="1.3.6",
+    version="1.3.7",
     zip_safe=False,
     author='Chris Laffra',
     author_email='laffra@gmail.com',
     url='https://www.chrislaffra.org/',
     packages=setuptools.find_packages(include=[
         'microlog',
         'dashboard',
```

### Comparing `micrologai-1.3.6/tests/test_call_view.py` & `micrologai-1.3.7/tests/test_call_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/tests/test_canvas.py` & `micrologai-1.3.7/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/tests/test_marker_view.py` & `micrologai-1.3.7/tests/test_marker_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/tests/test_print.py` & `micrologai-1.3.7/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/tests/test_status.py` & `micrologai-1.3.7/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/tests/test_status_view.py` & `micrologai-1.3.7/tests/test_status_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.6/tests/test_tracer.py` & `micrologai-1.3.7/tests/test_tracer.py`

 * *Files identical despite different names*

