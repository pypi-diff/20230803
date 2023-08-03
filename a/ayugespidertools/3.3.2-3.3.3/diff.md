# Comparing `tmp/ayugespidertools-3.3.2.tar.gz` & `tmp/ayugespidertools-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.3.2.tar", max compression
+gzip compressed data, was "ayugespidertools-3.3.3.tar", max compression
```

## Comparing `ayugespidertools-3.3.2.tar` & `ayugespidertools-3.3.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/LICENSE
--rw-r--r--   0        0        0     9808 2023-07-25 03:00:57.000000 ayugespidertools-3.3.2/README.md
--rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.2/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.2/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      236 2023-07-18 06:44:00.000000 ayugespidertools-3.3.2/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.2/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      503 2023-07-25 06:46:03.000000 ayugespidertools-3.3.2/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3636 2023-07-18 06:55:41.000000 ayugespidertools-3.3.2/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6562 2023-07-18 06:58:54.000000 ayugespidertools-3.3.2/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     5181 2023-07-18 07:01:23.000000 ayugespidertools-3.3.2/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    16320 2023-07-25 07:41:37.000000 ayugespidertools-3.3.2/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    12726 2023-07-18 07:24:16.000000 ayugespidertools-3.3.2/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32637 2023-07-18 07:24:36.000000 ayugespidertools-3.3.2/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     5980 2023-07-18 07:24:56.000000 ayugespidertools-3.3.2/ayugespidertools/common/spiderconf.py
--rw-r--r--   0        0        0     3688 2023-07-18 08:47:02.000000 ayugespidertools-3.3.2/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     3567 2023-07-18 07:26:36.000000 ayugespidertools-3.3.2/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    17832 2023-07-25 09:12:39.000000 ayugespidertools-3.3.2/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3642 2023-07-18 07:30:17.000000 ayugespidertools-3.3.2/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      376 2023-07-25 06:28:48.000000 ayugespidertools-3.3.2/ayugespidertools/config.py
--rw-r--r--   0        0        0     9615 2023-07-18 07:47:21.000000 ayugespidertools-3.3.2/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7568 2023-07-25 07:44:00.000000 ayugespidertools-3.3.2/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     6254 2023-07-18 08:52:39.000000 ayugespidertools-3.3.2/ayugespidertools/items.py
--rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.2/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8458 2023-07-18 07:52:38.000000 ayugespidertools-3.3.2/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.2/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5368 2023-07-18 07:53:41.000000 ayugespidertools-3.3.2/ayugespidertools/oss.py
--rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.2/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.2/ayugespidertools/request.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1340 2023-07-18 07:30:35.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1081 2023-07-18 07:30:49.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 06:57:30.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/headers/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-18 07:31:13.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10391 2023-07-18 07:33:53.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     3747 2023-07-18 07:34:22.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2417 2023-07-18 07:34:34.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/download/__init__.py
--rw-r--r--   0        0        0     2441 2023-07-18 07:34:59.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-18 07:35:17.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2044 2023-07-18 07:36:59.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1171 2023-07-18 07:37:50.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     3093 2023-07-18 07:38:54.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
--rw-r--r--   0        0        0     1769 2023-07-18 07:39:07.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0    11172 2023-07-18 07:40:39.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     3831 2023-07-18 07:40:57.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      326 2023-07-18 07:41:07.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1696 2023-07-18 07:41:25.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2722 2023-07-18 07:41:38.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3589 2023-07-18 07:42:26.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     7252 2023-07-20 09:38:27.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      430 2023-07-18 07:43:50.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.2/ayugespidertools/spiders.py
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     5148 2023-07-18 07:44:41.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.2/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6910 2023-07-18 07:54:34.000000 ayugespidertools-3.3.2/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     2979 2023-07-26 02:48:20.000000 ayugespidertools-3.3.2/pyproject.toml
--rw-r--r--   0        0        0    11436 1970-01-01 00:00:00.000000 ayugespidertools-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.3/LICENSE
+-rw-r--r--   0        0        0     9808 2023-07-25 03:00:57.000000 ayugespidertools-3.3.3/README.md
+-rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.3/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.3/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:44:00.000000 ayugespidertools-3.3.3/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.3/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      503 2023-07-25 06:46:03.000000 ayugespidertools-3.3.3/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3636 2023-07-18 06:55:41.000000 ayugespidertools-3.3.3/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6562 2023-07-18 06:58:54.000000 ayugespidertools-3.3.3/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     5181 2023-07-18 07:01:23.000000 ayugespidertools-3.3.3/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    16320 2023-07-25 07:41:37.000000 ayugespidertools-3.3.3/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    12409 2023-08-03 07:03:39.000000 ayugespidertools-3.3.3/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32637 2023-07-18 07:24:36.000000 ayugespidertools-3.3.3/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     5980 2023-07-18 07:24:56.000000 ayugespidertools-3.3.3/ayugespidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3688 2023-07-18 08:47:02.000000 ayugespidertools-3.3.3/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     3567 2023-07-18 07:26:36.000000 ayugespidertools-3.3.3/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    17760 2023-07-26 06:36:13.000000 ayugespidertools-3.3.3/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3642 2023-07-18 07:30:17.000000 ayugespidertools-3.3.3/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      376 2023-07-25 06:28:48.000000 ayugespidertools-3.3.3/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9615 2023-07-18 07:47:21.000000 ayugespidertools-3.3.3/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7568 2023-07-25 07:44:00.000000 ayugespidertools-3.3.3/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     6254 2023-07-18 08:52:39.000000 ayugespidertools-3.3.3/ayugespidertools/items.py
+-rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.3/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8458 2023-07-18 07:52:38.000000 ayugespidertools-3.3.3/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.3/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5368 2023-07-18 07:53:41.000000 ayugespidertools-3.3.3/ayugespidertools/oss.py
+-rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.3/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.3/ayugespidertools/request.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1340 2023-07-18 07:30:35.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1081 2023-07-18 07:30:49.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 06:57:30.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/headers/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-18 07:31:13.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10391 2023-07-18 07:33:53.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3747 2023-07-18 07:34:22.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2417 2023-07-18 07:34:34.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/download/__init__.py
+-rw-r--r--   0        0        0     2441 2023-07-18 07:34:59.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-18 07:35:17.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2044 2023-07-18 07:36:59.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1171 2023-07-18 07:37:50.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3093 2023-07-18 07:38:54.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     1769 2023-07-18 07:39:07.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0    11172 2023-07-18 07:40:39.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     3831 2023-07-18 07:40:57.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      326 2023-07-18 07:41:07.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1696 2023-07-18 07:41:25.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2722 2023-07-18 07:41:38.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3589 2023-07-18 07:42:26.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7252 2023-07-20 09:38:27.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-18 07:43:50.000000 ayugespidertools-3.3.3/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.3/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.3/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.3/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     5148 2023-07-18 07:44:41.000000 ayugespidertools-3.3.3/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.3/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.3/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.3/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.3/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.3/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6910 2023-07-18 07:54:34.000000 ayugespidertools-3.3.3/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     2996 2023-08-03 06:55:21.000000 ayugespidertools-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 ayugespidertools-3.3.3/PKG-INFO
```

### Comparing `ayugespidertools-3.3.2/LICENSE` & `ayugespidertools-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/README.md` & `ayugespidertools-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.3.3/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/encryption.py` & `ayugespidertools-3.3.3/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/expend.py` & `ayugespidertools-3.3.3/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.3.3/ayugespidertools/common/mongodbpipe.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.3.3/ayugespidertools/common/multiplexing.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.3.3/ayugespidertools/common/mysqlerrhandle.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,20 +179,15 @@
             2). 执行此 sql 可能会报错的信息
         """
         colum_pattern = re.compile(r"Unknown column '(.*?)' in 'field list'")
         text = re.findall(colum_pattern, err_msg)
         colum = text[0]
         notes = note_dic[colum]
 
-        if colum == "url":
-            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` TEXT(500) NULL COMMENT '{notes}';"
-        elif colum in {"create_time", "crawl_time", "update_time"}:
-            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` DATE NULL DEFAULT NULL COMMENT '{notes}';"
-        else:
-            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(190) NULL DEFAULT '' COMMENT '{notes}';"
+        sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(190) NULL DEFAULT '' COMMENT '{notes}';"
         return sql, f"1054: 添加字段 {colum} 已存在"
 
     def deal_1146_error(
         self,
         err_msg: str,
         table_enum: Type[TableEnumTypeVar],
     ) -> (str, str, str):
```

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/params.py` & `ayugespidertools-3.3.3/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/spiderconf.py` & `ayugespidertools-3.3.3/ayugespidertools/common/spiderconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.3.3/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/typevars.py` & `ayugespidertools-3.3.3/ayugespidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/utils.py` & `ayugespidertools-3.3.3/ayugespidertools/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,16 +328,15 @@
 
         return calculate_bezier_point
 
     def _type(self, type, x, length):
         numbers = []
         pin = (x[1] - x[0]) / length
         if type == 0:
-            for i in range(length):
-                numbers.append(i * pin)
+            numbers.extend(i * pin for i in range(length))
             if pin >= 0:
                 numbers = numbers[::-1]
         elif type == 1:
             for i in range(length):
                 numbers.append(1 * ((i * pin) ** 2))
             numbers = numbers[::-1]
         elif type == 2:
@@ -348,16 +347,15 @@
             track = [
                 np.array([0, 0]),
                 np.array([(x[1] - x[0]) * 0.8, (x[1] - x[0]) * 0.6]),
                 np.array([x[1] - x[0], 0]),
             ]
             fun = self._generate_control_points(track)
             numbers = [0]
-            for i in range(1, length):
-                numbers.append(fun(i * pin) + numbers[-1])
+            numbers.extend(fun(i * pin) + numbers[-1] for i in range(1, length))
             if pin >= 0:
                 numbers = numbers[::-1]
         numbers = np.abs(np.array(numbers) - max(numbers))
         normal_numbers = (
             (numbers - numbers[numbers.argmin()])
             / (numbers[numbers.argmax()] - numbers[numbers.argmin()])
         ) * (x[1] - x[0]) + x[0]
@@ -441,16 +439,15 @@
         w = fun["P"]
         fun = fun["equation"]
         if shake_num != 0:
             track_number = round(num * 0.2 / (shake_num + 1))
             num -= num * (shake_num + 1)
 
             x_track_array = self._type(type, [start[0], end[0]], num)
-            for i in x_track_array:
-                s.append([i, fun(i)])
+            s.extend([i, fun(i)] for i in x_track_array)
             dq = yhh / shake_num
             kg = 0
             ends = np.copy(end)
             for i in range(shake_num):
                 if kg == 0:
                     d = np.array(
                         [
@@ -501,10 +498,9 @@
                 shake_num=0,
                 yhh=10,
             )
             s += list(y["trackArray"])
 
         else:
             x_track_array = self._type(type, [start[0], end[0]], num)
-            for i in x_track_array:
-                s.append([i, fun(i)])
+            s.extend([i, fun(i)] for i in x_track_array)
         return {"trackArray": np.array(s), "P": w}
```

### Comparing `ayugespidertools-3.3.2/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.3.3/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/formatdata.py` & `ayugespidertools-3.3.3/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/imgoperation.py` & `ayugespidertools-3.3.3/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/items.py` & `ayugespidertools-3.3.3/ayugespidertools/items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/middlewares.py` & `ayugespidertools-3.3.3/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/mongoclient.py` & `ayugespidertools-3.3.3/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.3.3/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/oss.py` & `ayugespidertools-3.3.3/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/pipelines.py` & `ayugespidertools-3.3.3/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.3.3/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-3.3.3/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.3.3/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.3.3/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/ayugespidertools/verificationcode.py` & `ayugespidertools-3.3.3/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.2/pyproject.toml` & `ayugespidertools-3.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "3.3.2"
+version = "3.3.3"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -35,14 +35,15 @@
 aiomysql = "^0.1.1"
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
 motor = "2.5.1"
 urllib3 = "~1.26.15"
 pika = "~1.3.2"
 kafka-python = "2.0.2"
+pyyaml = "~6.0"
 
 [tool.poetry.scripts]
 ayuge = "ayugespidertools.utils.cmdline:execute"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^23.1.0"
```

### Comparing `ayugespidertools-3.3.2/PKG-INFO` & `ayugespidertools-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 3.3.2
+Version: 3.3.3
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -30,14 +30,15 @@
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: oss2 (>=2.16.0,<3.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pika (>=1.3.2,<1.4.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pymongo (>=3.12.3,<4.0.0)
 Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0)
+Requires-Dist: pyyaml (>=6.0,<6.1)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: urllib3 (>=1.26.15,<1.27.0)
 Project-URL: Documentation, https://ayugespidertools.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/shengchenyang/AyugeSpiderTools
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ayugespidertools Version: 3.3.2 Summary: scrapy
+Metadata-Version: 2.1 Name: ayugespidertools Version: 3.3.3 Summary: scrapy
 æ©å±åºï¼ç¨äºæ©å± Scrapy åè½æ¥è§£æ¾åæã Home-page: https://
 www.ayuge.top/mkdocs-material/ Keywords:
 crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3 Author: ayuge
 Author-email: ayugesheng@gmail.com Maintainer: ayuge Maintainer-email:
 ayugesheng@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -14,17 +14,17 @@
 Dist: itemadapter (>=0.7.0,<0.8.0) Requires-Dist: kafka-python (==2.0.2)
 Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: motor (==2.5.1) Requires-Dist: numpy (>=1.24.3,<1.25.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0) Requires-Dist: oss2
 (>=2.16.0,<3.0.0) Requires-Dist: pandas (>=1.5.0,<2.0.0) Requires-Dist: pika
 (>=1.3.2,<1.4.0) Requires-Dist: pycryptodome (>=3.15.0,<4.0.0) Requires-Dist:
 pymongo (>=3.12.3,<4.0.0) Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0) Requires-
-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: retrying (>=1.3.3,<2.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: urllib3
-(>=1.26.15,<1.27.0) Project-URL: Documentation, https://
+Dist: pyyaml (>=6.0,<6.1) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
+Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: urllib3 (>=1.26.15,<1.27.0) Project-URL: Documentation, https://
 ayugespidertools.readthedocs.io/en/latest/ Project-URL: Repository, https://
 github.com/shengchenyang/AyugeSpiderTools Description-Content-Type: text/
 markdown
                             [ayugespidertools-logo]
 ===============================================================================
 # AyugeSpiderTools ä»ç» [![OSCS Status](https://www.oscs1024.com/platform/
 badge/AyugeSpiderTools.svg?size=small)](https://www.murphysec.com/
```

