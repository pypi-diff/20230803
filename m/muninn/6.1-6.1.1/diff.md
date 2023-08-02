# Comparing `tmp/muninn-6.1.tar.gz` & `tmp/muninn-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muninn-6.1.tar", last modified: Mon Jul 24 14:43:23 2023, max compression
+gzip compressed data, was "dist/muninn-6.1.1.tar", last modified: Wed Aug  2 22:02:11 2023, max compression
```

## Comparing `muninn-6.1.tar` & `muninn-6.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/
--rw-r--r--   0 sander     (501) staff       (20)      878 2023-07-24 14:43:23.000000 muninn-6.1/PKG-INFO
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/test/
--rw-r--r--   0 sander     (501) staff       (20)    72234 2023-07-21 09:55:52.000000 muninn-6.1/test/test.py
--rw-r--r--   0 sander     (501) staff       (20)     4076 2022-08-16 07:53:04.000000 muninn-6.1/test/product_type.py.template
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/test/data/
--rw-r--r--   0 sander     (501) staff       (20)     1015 2022-03-17 08:49:39.000000 muninn-6.1/test/data/pi.txt
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/test/data/multi/
--rw-r--r--   0 sander     (501) staff       (20)      229 2022-03-17 08:49:39.000000 muninn-6.1/test/data/multi/2.txt
--rw-r--r--   0 sander     (501) staff       (20)      209 2022-03-17 08:49:39.000000 muninn-6.1/test/data/multi/1.txt
--rw-r--r--   0 sander     (501) staff       (20)     1508 2022-03-23 13:34:50.000000 muninn-6.1/test/data/README
--rwxr-xr-x   0 sander     (501) staff       (20)       75 2022-03-31 07:35:25.000000 muninn-6.1/test/coverage.sh
--rw-r--r--   0 sander     (501) staff       (20)    26029 2023-07-24 14:30:27.000000 muninn-6.1/CHANGES
--rw-r--r--   0 sander     (501) staff       (20)      229 2022-06-07 12:48:22.000000 muninn-6.1/MANIFEST.in
--rw-r--r--   0 sander     (501) staff       (20)     1593 2022-10-28 15:16:38.000000 muninn-6.1/DEVELOPER.md
--rw-r--r--   0 sander     (501) staff       (20)     1180 2023-01-10 15:30:19.000000 muninn-6.1/README.md
--rw-r--r--   0 sander     (501) staff       (20)     2835 2023-07-24 14:33:23.000000 muninn-6.1/setup.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/database/
--rw-r--r--   0 sander     (501) staff       (20)    42950 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/postgresql.py
--rw-r--r--   0 sander     (501) staff       (20)     7471 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/blobgeometry.py
--rw-r--r--   0 sander     (501) staff       (20)       54 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)     6928 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/ewkb.py
--rw-r--r--   0 sander     (501) staff       (20)    40989 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/sqlite.py
--rw-r--r--   0 sander     (501) staff       (20)    32428 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/sql.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/tools/
--rw-r--r--   0 sander     (501) staff       (20)     4516 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/update.py
--rw-r--r--   0 sander     (501) staff       (20)     6891 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/ingest.py
--rw-r--r--   0 sander     (501) staff       (20)     2157 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/pull.py
--rw-r--r--   0 sander     (501) staff       (20)     2014 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/destroy.py
--rw-r--r--   0 sander     (501) staff       (20)     1468 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/untag.py
--rw-r--r--   0 sander     (501) staff       (20)     1797 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/remove.py
--rw-r--r--   0 sander     (501) staff       (20)     4897 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/attach.py
--rw-r--r--   0 sander     (501) staff       (20)       54 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)     2743 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/export.py
--rw-r--r--   0 sander     (501) staff       (20)     2945 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/hash.py
--rw-r--r--   0 sander     (501) staff       (20)     9571 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/summary.py
--rw-r--r--   0 sander     (501) staff       (20)     4646 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/utils.py
--rw-r--r--   0 sander     (501) staff       (20)     2040 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/retrieve.py
--rw-r--r--   0 sander     (501) staff       (20)    10134 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/search.py
--rw-r--r--   0 sander     (501) staff       (20)      977 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/list_tags.py
--rw-r--r--   0 sander     (501) staff       (20)     1625 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/strip.py
--rw-r--r--   0 sander     (501) staff       (20)     1455 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/info.py
--rw-r--r--   0 sander     (501) staff       (20)     1388 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/prepare.py
--rw-r--r--   0 sander     (501) staff       (20)     1214 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/tag.py
--rw-r--r--   0 sander     (501) staff       (20)     2898 2023-07-24 14:34:27.000000 muninn-6.1/muninn/config.py
--rw-r--r--   0 sander     (501) staff       (20)    10760 2023-07-24 14:34:27.000000 muninn-6.1/muninn/remote.py
--rw-r--r--   0 sander     (501) staff       (20)    10771 2023-07-24 14:34:27.000000 muninn-6.1/muninn/util.py
--rw-r--r--   0 sander     (501) staff       (20)     2281 2023-07-24 14:34:27.000000 muninn-6.1/muninn/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)     1807 2023-07-24 14:34:27.000000 muninn-6.1/muninn/core.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/storage/
--rw-r--r--   0 sander     (501) staff       (20)        0 2022-03-17 08:49:39.000000 muninn-6.1/muninn/storage/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)    11566 2023-07-18 12:06:32.000000 muninn-6.1/muninn/storage/fs.py
--rw-r--r--   0 sander     (501) staff       (20)     8008 2023-07-18 12:06:32.000000 muninn-6.1/muninn/storage/swift.py
--rw-r--r--   0 sander     (501) staff       (20)    11064 2023-07-18 12:06:32.000000 muninn-6.1/muninn/storage/s3.py
--rw-r--r--   0 sander     (501) staff       (20)     2524 2023-07-24 07:50:10.000000 muninn-6.1/muninn/storage/base.py
--rw-r--r--   0 sander     (501) staff       (20)     1206 2023-07-24 14:34:27.000000 muninn-6.1/muninn/visitor.py
--rw-r--r--   0 sander     (501) staff       (20)      273 2023-07-24 14:34:27.000000 muninn-6.1/muninn/extension.py
--rw-r--r--   0 sander     (501) staff       (20)     7040 2023-07-24 14:34:27.000000 muninn-6.1/muninn/geometry.py
--rw-r--r--   0 sander     (501) staff       (20)    31474 2023-07-24 14:34:27.000000 muninn-6.1/muninn/language.py
--rw-r--r--   0 sander     (501) staff       (20)    77997 2023-07-24 14:34:27.000000 muninn-6.1/muninn/archive.py
--rw-r--r--   0 sander     (501) staff       (20)      342 2023-07-24 14:34:27.000000 muninn-6.1/muninn/exceptions.py
--rw-r--r--   0 sander     (501) staff       (20)     1010 2023-07-24 14:34:27.000000 muninn-6.1/muninn/enum.py
--rw-r--r--   0 sander     (501) staff       (20)     1446 2022-03-17 08:49:39.000000 muninn-6.1/muninn/_compat.py
--rw-r--r--   0 sander     (501) staff       (20)     3749 2023-07-24 14:34:27.000000 muninn-6.1/muninn/function.py
--rw-r--r--   0 sander     (501) staff       (20)     1685 2023-07-24 14:34:27.000000 muninn-6.1/muninn/struct.py
--rw-r--r--   0 sander     (501) staff       (20)     6499 2023-07-24 14:34:27.000000 muninn-6.1/muninn/schema.py
--rw-r--r--   0 sander     (501) staff       (20)       38 2023-07-24 14:43:23.000000 muninn-6.1/setup.cfg
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/
--rw-r--r--   0 sander     (501) staff       (20)      878 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)     1340 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/SOURCES.txt
--rw-r--r--   0 sander     (501) staff       (20)      710 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/entry_points.txt
--rw-r--r--   0 sander     (501) staff       (20)        7 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/top_level.txt
--rw-r--r--   0 sander     (501) staff       (20)        1 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/dependency_links.txt
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/
+-rw-r--r--   0 sander     (501) staff       (20)      880 2023-08-02 22:02:11.000000 muninn-6.1.1/PKG-INFO
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/test/
+-rw-r--r--   0 sander     (501) staff       (20)    73176 2023-08-02 18:51:17.000000 muninn-6.1.1/test/test.py
+-rw-r--r--   0 sander     (501) staff       (20)     4076 2022-10-11 08:21:58.000000 muninn-6.1.1/test/product_type.py.template
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/test/data/
+-rw-r--r--   0 sander     (501) staff       (20)     1015 2022-03-09 18:31:40.000000 muninn-6.1.1/test/data/pi.txt
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/test/data/multi/
+-rw-r--r--   0 sander     (501) staff       (20)      229 2022-03-09 18:31:40.000000 muninn-6.1.1/test/data/multi/2.txt
+-rw-r--r--   0 sander     (501) staff       (20)      209 2022-03-09 18:31:40.000000 muninn-6.1.1/test/data/multi/1.txt
+-rw-r--r--   0 sander     (501) staff       (20)     1508 2022-03-28 10:47:50.000000 muninn-6.1.1/test/data/README
+-rwxr-xr-x   0 sander     (501) staff       (20)       75 2022-03-29 16:03:36.000000 muninn-6.1.1/test/coverage.sh
+-rw-r--r--   0 sander     (501) staff       (20)    26133 2023-08-02 18:51:17.000000 muninn-6.1.1/CHANGES
+-rw-r--r--   0 sander     (501) staff       (20)      229 2022-06-24 11:15:53.000000 muninn-6.1.1/MANIFEST.in
+-rw-r--r--   0 sander     (501) staff       (20)     1593 2022-11-24 12:38:40.000000 muninn-6.1.1/DEVELOPER.md
+-rw-r--r--   0 sander     (501) staff       (20)     1180 2023-02-08 17:38:59.000000 muninn-6.1.1/README.md
+-rw-r--r--   0 sander     (501) staff       (20)     2837 2023-08-02 18:51:17.000000 muninn-6.1.1/setup.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn/
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn/database/
+-rw-r--r--   0 sander     (501) staff       (20)    42950 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/database/postgresql.py
+-rw-r--r--   0 sander     (501) staff       (20)     7471 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/database/blobgeometry.py
+-rw-r--r--   0 sander     (501) staff       (20)       54 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/database/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)     6928 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/database/ewkb.py
+-rw-r--r--   0 sander     (501) staff       (20)    40989 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/database/sqlite.py
+-rw-r--r--   0 sander     (501) staff       (20)    32428 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/database/sql.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn/tools/
+-rw-r--r--   0 sander     (501) staff       (20)     4516 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/update.py
+-rw-r--r--   0 sander     (501) staff       (20)     6891 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/ingest.py
+-rw-r--r--   0 sander     (501) staff       (20)     2157 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/pull.py
+-rw-r--r--   0 sander     (501) staff       (20)     2014 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/destroy.py
+-rw-r--r--   0 sander     (501) staff       (20)     1468 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/untag.py
+-rw-r--r--   0 sander     (501) staff       (20)     1797 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/remove.py
+-rw-r--r--   0 sander     (501) staff       (20)     4897 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/attach.py
+-rw-r--r--   0 sander     (501) staff       (20)       54 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)     2743 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/export.py
+-rw-r--r--   0 sander     (501) staff       (20)     2945 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/hash.py
+-rw-r--r--   0 sander     (501) staff       (20)     9571 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/summary.py
+-rw-r--r--   0 sander     (501) staff       (20)     4646 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/utils.py
+-rw-r--r--   0 sander     (501) staff       (20)     2040 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/retrieve.py
+-rw-r--r--   0 sander     (501) staff       (20)    10134 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/search.py
+-rw-r--r--   0 sander     (501) staff       (20)      977 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/list_tags.py
+-rw-r--r--   0 sander     (501) staff       (20)     1625 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/strip.py
+-rw-r--r--   0 sander     (501) staff       (20)     1455 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/info.py
+-rw-r--r--   0 sander     (501) staff       (20)     1388 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/prepare.py
+-rw-r--r--   0 sander     (501) staff       (20)     1214 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/tools/tag.py
+-rw-r--r--   0 sander     (501) staff       (20)     2898 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/config.py
+-rw-r--r--   0 sander     (501) staff       (20)    10760 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/remote.py
+-rw-r--r--   0 sander     (501) staff       (20)    10771 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/util.py
+-rw-r--r--   0 sander     (501) staff       (20)     2283 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)     1807 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/core.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn/storage/
+-rw-r--r--   0 sander     (501) staff       (20)        0 2022-03-09 18:31:40.000000 muninn-6.1.1/muninn/storage/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)    11566 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/storage/fs.py
+-rw-r--r--   0 sander     (501) staff       (20)     8056 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/storage/swift.py
+-rw-r--r--   0 sander     (501) staff       (20)    11112 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/storage/s3.py
+-rw-r--r--   0 sander     (501) staff       (20)     2524 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/storage/base.py
+-rw-r--r--   0 sander     (501) staff       (20)     1206 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/visitor.py
+-rw-r--r--   0 sander     (501) staff       (20)      273 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/extension.py
+-rw-r--r--   0 sander     (501) staff       (20)     7040 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/geometry.py
+-rw-r--r--   0 sander     (501) staff       (20)    31474 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/language.py
+-rw-r--r--   0 sander     (501) staff       (20)    78102 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/archive.py
+-rw-r--r--   0 sander     (501) staff       (20)      342 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/exceptions.py
+-rw-r--r--   0 sander     (501) staff       (20)     1010 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/enum.py
+-rw-r--r--   0 sander     (501) staff       (20)     1446 2022-03-09 18:31:40.000000 muninn-6.1.1/muninn/_compat.py
+-rw-r--r--   0 sander     (501) staff       (20)     3749 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/function.py
+-rw-r--r--   0 sander     (501) staff       (20)     1685 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/struct.py
+-rw-r--r--   0 sander     (501) staff       (20)     6499 2023-08-02 18:51:17.000000 muninn-6.1.1/muninn/schema.py
+-rw-r--r--   0 sander     (501) staff       (20)       38 2023-08-02 22:02:11.000000 muninn-6.1.1/setup.cfg
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn.egg-info/
+-rw-r--r--   0 sander     (501) staff       (20)      880 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn.egg-info/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)     1340 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn.egg-info/SOURCES.txt
+-rw-r--r--   0 sander     (501) staff       (20)      710 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn.egg-info/entry_points.txt
+-rw-r--r--   0 sander     (501) staff       (20)        7 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn.egg-info/top_level.txt
+-rw-r--r--   0 sander     (501) staff       (20)        1 2023-08-02 22:02:11.000000 muninn-6.1.1/muninn.egg-info/dependency_links.txt
```

### Comparing `muninn-6.1/PKG-INFO` & `muninn-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: muninn
-Version: 6.1
+Version: 6.1.1
 Summary: Data product catalogue and archive system
 Home-page: https://github.com/stcorp/muninn
 Author: S[&]T
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `muninn-6.1/test/test.py` & `muninn-6.1.1/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
         ctx = multiprocessing.get_context('forkserver')
         ctx.set_forkserver_preload(['subprocess'])
         manager = ctx.Manager()
     except AttributeError:
         ctx = multiprocessing
         manager = multiprocessing.Manager()
 
+
 def do_popen(cmd, return_dict, join):
     proc = subprocess.Popen(
             cmd,
             shell=True,
             stdout=subprocess.PIPE if join or not PY3 else subprocess.DEVNULL,
             stderr=subprocess.PIPE if join or not PY3 else subprocess.DEVNULL,
     )
@@ -223,14 +224,15 @@
     return request.param
 
 
 @pytest.fixture(params=[s for s in STORAGE_BACKENDS if s != 'none'])
 def storage(request):
     return request.param
 
+
 @pytest.fixture(params=[s for s in STORAGE_BACKENDS if s == 'none'])
 def storage_pure(request):
     return request.param
 
 
 @pytest.fixture(params=ARCHIVE_PATHS)
 def archive_path(request):
@@ -304,14 +306,15 @@
 
 
 @pytest.fixture
 def archive(database, storage, use_enclosing_directory, archive_path):
     for a in _archive(database, storage, use_enclosing_directory, archive_path):
         yield a
 
+
 @pytest.fixture
 def archive_pure(database, storage_pure, use_enclosing_directory, archive_path):
     for a in _archive(database, storage_pure, use_enclosing_directory, archive_path):
         yield a
 
 
 @pytest.fixture(params=REMOTE_BACKENDS, scope='session')
@@ -851,15 +854,15 @@
                 plugin.cascade_rule = cascade_rule
 
                 uuid_a = archive.ingest(['data/a.txt']).core.uuid
                 uuid_b = archive.ingest(['data/b.txt']).core.uuid
                 uuid_c = archive.ingest(['data/c.txt']).core.uuid
                 uuid_pi = archive.ingest(['data/pi.txt']).core.uuid
 
-                time.sleep(2) # grace period # TODO use >= 0 in sql instead of > 0?
+                time.sleep(2)  # grace period # TODO use >= 0 in sql instead of > 0?
 
                 archive.link(uuid_pi, [uuid_pi])  # TODO otherwise no source, so deleted?
 
                 archive.link(uuid_b, [uuid_a])
                 archive.link(uuid_c, [uuid_b])
 
                 # also remove derived products b and c
@@ -935,76 +938,96 @@
 
         # error
         with muninn.util.TemporaryDirectory() as tmp_path:
             with pytest.raises(muninn.exceptions.Error) as excinfo:
                 archive.retrieve(uuid.uuid4())
             assert 'No product found' in str(excinfo)
 
-
     def test_retrieve_multi_file(self, archive):
-        if archive._params['use_enclosing_directory'] is True:
+        if archive._params['use_enclosing_directory']:
             props = self._ingest_multi_file(archive)
 
             # copy (query)
             with muninn.util.TemporaryDirectory() as tmp_path:
                 result = archive.retrieve(target_path=tmp_path)
 
-                for name in ('1.txt', '2.txt'):
+                for name in ('1.txt', '2.txt', 'emptyfile'):
                     path = os.path.join(tmp_path, name)
                     assert os.path.isfile(path)
                     assert os.path.getsize(path) == os.path.getsize('data/multi/%s' % name)
+                for name in ('dir', 'emptydir'):
+                    path = os.path.join(tmp_path, name)
+                    assert os.path.isdir(path)
 
                 assert len(result) == 1
+                assert len(result[0]) == 5
                 assert os.path.join(tmp_path, '1.txt') in result[0]
                 assert os.path.join(tmp_path, '2.txt') in result[0]
+                assert os.path.join(tmp_path, 'dir') in result[0]
+                assert os.path.join(tmp_path, 'emptydir') in result[0]
+                assert os.path.join(tmp_path, 'emptyfile') in result[0]
 
             # copy (uuid)
             with muninn.util.TemporaryDirectory() as tmp_path:
                 result = archive.retrieve(props.core.uuid, target_path=tmp_path)
 
+                assert len(result) == 5
                 assert os.path.join(tmp_path, '1.txt') in result
                 assert os.path.join(tmp_path, '2.txt') in result
+                assert os.path.join(tmp_path, 'dir') in result
+                assert os.path.join(tmp_path, 'emptydir') in result
+                assert os.path.join(tmp_path, 'emptyfile') in result
 
             # copy to '.'
             archive.retrieve(target_path='.')
-            for name in ('1.txt', '2.txt'):
+            for name in ('1.txt', '2.txt', 'emptyfile'):
                 assert os.path.isfile(name)
                 assert os.path.getsize(name) == os.path.getsize('data/multi/%s' % name)
+            for name in ('dir', 'emptydir'):
+                assert os.path.isdir(name)
 
             # symlink
             if archive._params['storage'] == 'fs':
                 with muninn.util.TemporaryDirectory() as tmp_path:
                     archive.retrieve(target_path=tmp_path, use_symlinks=True)
 
-                    for name in ('1.txt', '2.txt'):
+                    for name in ('1.txt', '2.txt', 'dir', 'emptydir', 'emptyfile'):
                         path = os.path.join(tmp_path, name)
                         assert os.path.islink(path)
 
                         target_path = os.path.join(
                             archive._checker.root,
                             archive._params['archive_path'],
                             'multi',
                             name
                         )
 
                         target_path = os.path.realpath(target_path)
 
-                        assert os.path.isfile(target_path)
+                        if name.endswith('dir'):
+                            assert os.path.isdir(target_path)
+                        else:
+                            assert os.path.isfile(target_path)
                         assert os.readlink(path) == target_path
             else:
                 with pytest.raises(muninn.exceptions.Error) as excinfo:
                     with muninn.util.TemporaryDirectory() as tmp_path:
                         archive.retrieve(target_path=tmp_path, use_symlinks=True)
                 assert 'storage backend does not support symlinks' in str(excinfo)
 
     def test_retrieve_dir(self, archive):  # TODO fs: symlink/intra
         self._ingest_dir(archive)
 
         with muninn.util.TemporaryDirectory() as tmp_path:
-            archive.retrieve(target_path=tmp_path)
+            result = archive.retrieve(target_path=tmp_path)
+
+            if archive._params['use_enclosing_directory']:
+                assert result == [[os.path.join(tmp_path, 'dir')]]
+            else:
+                assert result == [os.path.join(tmp_path, 'dir')]
 
             for name in ('dir/pi.txt', 'dir/multi/1.txt', 'dir/multi/2.txt'):
                 path = os.path.join(tmp_path, name)
 
                 assert os.path.isfile(path)
                 assert os.path.getsize(path) == os.path.getsize(os.path.join('data', name))
 
@@ -1177,23 +1200,23 @@
         finally:
             plugin.hash_type = 'md5'
 
     def test_update_properties(self, archive):
         product = self._ingest_file(archive)
 
         for create_namespaces in (True, False):
-            props = muninn.Struct({'mynamespace': {'myjson': {'bla': 14, 'mylist': [1,2,3]}}})
+            props = muninn.Struct({'mynamespace': {'myjson': {'bla': 14, 'mylist': [1, 2, 3]}}})
             archive.update_properties(props, product.core.uuid, create_namespaces)
 
             props = archive.retrieve_properties(uuid=product.core.uuid, namespaces=['mynamespace'])
             myjson = props.mynamespace.myjson
 
             assert isinstance(myjson, dict)
             assert myjson['bla'] == 14
-            assert myjson['mylist'] == [1,2,3]
+            assert myjson['mylist'] == [1, 2, 3]
 
     def test_verify_hash(self, archive):
         product = self._ingest_file(archive)
 
         # normal case: hash contains prefix
         failed = archive.verify_hash()
         assert len(failed) == 0
@@ -1271,16 +1294,15 @@
 
         # having
         for having in ('archive_date.min', 'core.archive_date.min'):
             data, headers = archive.summary(group_by=['core.product_name'],
                                             aggregates=['core.archive_date.min', 'core.archive_date.max'],
                                             where='size > 0',
                                             order_by=['core.product_name'],
-                                            having='%s >= 2020-02-02 and count >= 1' % having,
-                                           )
+                                            having='%s >= 2020-02-02 and count >= 1' % having)
             assert len(data) == 2
 
     def test_broken_plugin(self, archive):
         product = self._ingest_file(archive)
         product.core.product_type = 'broken'
         archive.update_properties(product)
 
@@ -1328,25 +1350,25 @@
         assert len(archive_pure.search()) == 0
 
     def test_retrieve(self, archive_pure):
         properties = archive_pure.ingest(
             ['data/a.txt'],
         )
         with muninn.util.TemporaryDirectory() as tmp_path:
-            archive_pure.retrieve(target_path=tmp_path)
+            result = archive_pure.retrieve(target_path=tmp_path)
+            assert result == [os.path.join(tmp_path, 'a.txt')]
             assert os.listdir(tmp_path) == ['a.txt']
 
-    def test_retrieve_multi(self, archive_pure):
-        if archive_pure._params['use_enclosing_directory']:  # TODO fix archive to accept?
-            properties = archive_pure.ingest(
-                ['data/dir/multi/1.txt', 'data/dir/multi/2.txt'],  # TODO does this cause other files under multi to be included?
-            )
-            with muninn.util.TemporaryDirectory() as tmp_path:
-                archive_pure.retrieve(target_path=tmp_path)
-                assert set(os.listdir(os.path.join(tmp_path, 'multi'))) == set(['1.txt', '2.txt'])
+    def test_retrieve_dir(self, archive_pure):
+        properties = archive_pure.ingest(
+            ['data/dir'],
+        )
+        with muninn.util.TemporaryDirectory() as tmp_path:
+            result = archive_pure.retrieve(target_path=tmp_path)
+            assert result == [os.path.join(tmp_path, 'dir')]
 
     def test_rebuild_properties(self, archive_pure):
         properties = archive_pure.ingest(
             ['data/a.txt'],
         )
         archive_pure.rebuild_properties(properties.core.uuid)  # TODO just pass properties?
 
@@ -1389,14 +1411,15 @@
             s = archive_pure.attach(None)
         assert '"attach" operation not available for storage=none' in str(excinfo)
 
         with pytest.raises(muninn.exceptions.Error) as excinfo:
             s = archive_pure.strip()
         assert '"strip" operation not available for storage=none' in str(excinfo)
 
+
 class TestQuery:
     def _prep_data(self, archive):
         self.uuid_a = archive.ingest(['data/a.txt']).core.uuid
         self.uuid_b = archive.ingest(['data/b.txt']).core.uuid
         self.uuid_c = archive.ingest(['data/c.txt']).core.uuid
 
         archive.update_properties(muninn.Struct({'mynamespace': {'hello': 'hohoho'}}), self.uuid_a, True)
@@ -1660,15 +1683,15 @@
             assert len(s) == 0
 
     def test_alt_number_bases(self, archive):
         self._prep_data(archive)
         s = archive.search('size == %s' % hex(1015))
         assert len(s) == 3
 
-        s = archive.search('size == 0o1767') # py2/3 compat
+        s = archive.search('size == 0o1767')  # py2/3 compat
         assert len(s) == 3
 
         s = archive.search('size == %s' % bin(1015))
         assert len(s) == 3
 
         s = archive.search('size == %s' % hex(1014))
         assert len(s) == 0
@@ -1696,14 +1719,15 @@
             s = archive.search('size in [] xyz')
         assert 'extra characters after expression' in str(excinfo)
 
         with pytest.raises(muninn.exceptions.Error) as excinfo:
             s = archive.search('covers(core.footprint, POINT (1.0, 3.0))')
         assert 'char 34: expected one of: INTEGER, REAL, got ","' in str(excinfo)
 
+
 class TestTools:  # TODO more result checking, preferrably using tools
     def _run(self, tool, args='', action='', archive='my_arch', should_fail=False):
         python_path = 'PYTHONPATH=%s:.:$PYTHONPATH' % PARENT_DIR
         cmd = '%s python%s ../muninn/tools/%s.py %s %s %s 2>&1' % \
               (python_path, '3' if PY3 else '', tool, action, archive, args)
 
         returncode, output, errs = safe_popen(cmd, join=True)
@@ -1718,15 +1742,15 @@
         else:
             assert returncode == 0
             assert not errs
         return output.decode().splitlines()
 
     def test_search(self, archive):
         output = self._run('search', '""')
-        assert len(output) == 2 # header
+        assert len(output) == 2  # header
         output = self._run('ingest', 'data/pi.txt')
         output = self._run('search', '"" -p \\*')
         assert len(output) == 3
         output = self._run('search', '"" -c')
         assert output == ['1']
         output = self._run('search', '"" --uuid')
         assert len(output) == 1
```

### Comparing `muninn-6.1/test/product_type.py.template` & `muninn-6.1.1/test/product_type.py.template`

 * *Files identical despite different names*

### Comparing `muninn-6.1/test/data/pi.txt` & `muninn-6.1.1/test/data/pi.txt`

 * *Files identical despite different names*

### Comparing `muninn-6.1/test/data/README` & `muninn-6.1.1/test/data/README`

 * *Files identical despite different names*

### Comparing `muninn-6.1/CHANGES` & `muninn-6.1.1/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+6.1.1 2023-08-02
+~~~~~~~~~~~~~~~~
+
+* Fixed several issues with the return value of Archive.retrieve().
+
 6.1 2023-07-24
 ~~~~~~~~~~~~~~
 
 * The S3 bucket prefix is now created as a 'directory object' so its existence
   can be explicitly checked.
 
 * muninn-pull for http/https will now retry once in case of a timeout error.
@@ -19,15 +24,15 @@
 
 * Fixed issue where muninn-summary could not group by core.physical_name or
   core.archive_path.
 
 * Fixed issue where muninn was incorrectly using subdirectories in the
   temporary directory if the 'tempdir' archive configuration option was set.
 
-* Fixed issue where archive.retrieve() and archive.export() were returning a
+* Fixed issue where Archive.retrieve() and Archive.export() were returning a
   list if a single properties Struct was given as parameter and
   `use_enclosing_directory` was not set. Additionally, each entry for a
   product where `use_enclosing_directory` _is_ set will now always be a list.
 
 6.0.1 2022-11-17
 ~~~~~~~~~~~~~~~~
 
@@ -91,16 +96,16 @@
      ALTER TABLE table ALTER COLUMN property SET DATA TYPE TEXT COLLATE "C"
 
 * Removed support for all deprecated archive configuration options.
 
 5.4 2022-02-22
 ~~~~~~~~~~~~~~
 
-* Added muninn-attach/archive.attach() which acts as the inverse of
-  muninn-strip/archive.strip().
+* Added muninn-attach/Archive.attach() which acts as the inverse of
+  muninn-strip/Archive.strip().
 
 * Fixed grand_type -> grant_type keyword typo for oauth2 entries in auth_file.
 
 * Allow explicit setting of region for S3 backend.
 
 * Added (optional) 'paths' argument to plugin export methods.
 
@@ -192,15 +197,15 @@
 * Changed `muninn-update -a <action>` command to `munnin-update <action>`.
 
 * Changed `muninn-ingest -c` command to mean 'catalogue only'.
 
 * Added basic 'in' and 'not in' operators (so that e.g. the following works:
  `physical_name not in ["a", "b"]`)
 
-* Namespace records can now be removed with archive.update_properties() by
+* Namespace records can now be removed with Archive.update_properties() by
   passing: `Struct({'mynamespace': None})`
 
 5.0 2020-07-30
 ~~~~~~~~~~~~~~
 
 * Added a storage backend framework, including S3 and Swift backends.
```

### Comparing `muninn-6.1/DEVELOPER.md` & `muninn-6.1.1/DEVELOPER.md`

 * *Files identical despite different names*

### Comparing `muninn-6.1/README.md` & `muninn-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `muninn-6.1/setup.py` & `muninn-6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     sys.exit("Python 2.7 (or newer) or 3.6 (or newer) is required to use this package.")
 
 
 requirements = []
 
 setup(
     name="muninn",
-    version="6.1",
+    version="6.1.1",
     description="Data product catalogue and archive system",
     url="https://github.com/stcorp/muninn",
     author="S[&]T",
     license="BSD",
     packages=["muninn", "muninn.tools", "muninn.database", "muninn.storage"],
     entry_points={"console_scripts": [
         "muninn-attach = muninn.tools.attach:main",
```

### Comparing `muninn-6.1/muninn/database/postgresql.py` & `muninn-6.1.1/muninn/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/database/blobgeometry.py` & `muninn-6.1.1/muninn/database/blobgeometry.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/database/ewkb.py` & `muninn-6.1.1/muninn/database/ewkb.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/database/sqlite.py` & `muninn-6.1.1/muninn/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/database/sql.py` & `muninn-6.1.1/muninn/database/sql.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/update.py` & `muninn-6.1.1/muninn/tools/update.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/ingest.py` & `muninn-6.1.1/muninn/tools/ingest.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/pull.py` & `muninn-6.1.1/muninn/tools/pull.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/destroy.py` & `muninn-6.1.1/muninn/tools/destroy.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/untag.py` & `muninn-6.1.1/muninn/tools/untag.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/remove.py` & `muninn-6.1.1/muninn/tools/remove.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/attach.py` & `muninn-6.1.1/muninn/tools/attach.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/export.py` & `muninn-6.1.1/muninn/tools/export.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/hash.py` & `muninn-6.1.1/muninn/tools/hash.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/summary.py` & `muninn-6.1.1/muninn/tools/summary.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/utils.py` & `muninn-6.1.1/muninn/tools/utils.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/retrieve.py` & `muninn-6.1.1/muninn/tools/retrieve.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/search.py` & `muninn-6.1.1/muninn/tools/search.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/list_tags.py` & `muninn-6.1.1/muninn/tools/list_tags.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/strip.py` & `muninn-6.1.1/muninn/tools/strip.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/info.py` & `muninn-6.1.1/muninn/tools/info.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/prepare.py` & `muninn-6.1.1/muninn/tools/prepare.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/tools/tag.py` & `muninn-6.1.1/muninn/tools/tag.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/config.py` & `muninn-6.1.1/muninn/config.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/remote.py` & `muninn-6.1.1/muninn/remote.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/util.py` & `muninn-6.1.1/muninn/util.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/__init__.py` & `muninn-6.1.1/muninn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
-__version__ = "6.1"
+__version__ = "6.1.1"
 __copyright__ = "Copyright (C) 2014-2023 S[&]T, The Netherlands."
 
 __all__ = ["Error", "InternalError", "Struct", "Archive", "open", "config_path"]
 
 import os as _os
 
 from muninn.archive import Archive
```

### Comparing `muninn-6.1/muninn/core.py` & `muninn-6.1.1/muninn/core.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/storage/fs.py` & `muninn-6.1.1/muninn/storage/fs.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/storage/swift.py` & `muninn-6.1.1/muninn/storage/swift.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,24 +156,25 @@
             raise Error("no data for product '%s' (%s)" % (product.core.product_name, product.core.uuid))
 
         for key in keys:
             rel_path = os.path.relpath(key, archive_path)
             if use_enclosing_directory:
                 rel_path = '/'.join(rel_path.split('/')[1:])
             target = os.path.normpath(os.path.join(target_path, rel_path))
+            if os.path.dirname(rel_path) == '':
+                paths.append(target)
             if key.endswith('/'):
                 util.make_path(target)
             else:
                 dirname = os.path.dirname(target)
                 if dirname != '':
                     util.make_path(dirname)
                 binary = self._conn.get_object(self.container, key)[1]
                 with open(target, 'wb') as f:
                     f.write(binary)
-                paths.append(target)
 
         return paths
 
     def delete(self, product_path, properties):
         for key in self._object_keys(product_path):
             self._conn.delete_object(self.container, key)
```

### Comparing `muninn-6.1/muninn/storage/s3.py` & `muninn-6.1.1/muninn/storage/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,24 +225,25 @@
             raise Error("no data for product '%s' (%s)" % (product.core.product_name, product.core.uuid))
 
         for obj in objs:
             rel_path = os.path.relpath(obj.key, self._prefix + archive_path)
             if use_enclosing_directory:
                 rel_path = '/'.join(rel_path.split('/')[1:])
             target = os.path.normpath(os.path.join(target_path, rel_path))
+            if os.path.dirname(rel_path) == '':
+                paths.append(target)
 
             if obj.key.endswith('/'):
                 util.make_path(target)
             else:
                 dirname = os.path.dirname(target)
                 if dirname != '':
                     util.make_path(dirname)
                 self._resource.Object(self.bucket, obj.key).download_file(target, ExtraArgs=self._download_args,
                                                                           Config=self._transfer_config)
-                paths.append(target)
 
         return paths
 
     def delete(self, product_path, properties):
         prefix = self._prefix + product_path
         for obj in self._resource.Bucket(self.bucket).objects.filter(Prefix=prefix):
             obj.delete()
```

### Comparing `muninn-6.1/muninn/storage/base.py` & `muninn-6.1.1/muninn/storage/base.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/visitor.py` & `muninn-6.1.1/muninn/visitor.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/geometry.py` & `muninn-6.1.1/muninn/geometry.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/language.py` & `muninn-6.1.1/muninn/language.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/archive.py` & `muninn-6.1.1/muninn/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,19 +523,22 @@
             paths = self._storage.get(product, target_path, use_enclosing_directory, use_symlinks)
 
             if verify_hash and 'hash' in product.core and not self._verify_hash(product, paths):
                 raise Error("retrieved product '%s' (%s) has incorrect hash" %
                             (product.core.product_name, product.core.uuid))
 
             if not use_enclosing_directory:
-                paths = paths[0]
+                if len(paths) == 1:
+                    paths = paths[0]
 
         elif 'remote_url' in product.core:
             retrieve_files = remote.retrieve_function(self, product, verify_hash)
             paths = retrieve_files(target_path)
+            if len(paths) == 1:
+                paths = paths[0]
 
         else:
             raise Error("product '%s' (%s) not available" % (product.core.product_name, product.core.uuid))
 
         return paths
 
     def _run_hooks(self, hook_name, properties, reverse=False, paths=None):
```

### Comparing `muninn-6.1/muninn/enum.py` & `muninn-6.1.1/muninn/enum.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/_compat.py` & `muninn-6.1.1/muninn/_compat.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/function.py` & `muninn-6.1.1/muninn/function.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/struct.py` & `muninn-6.1.1/muninn/struct.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn/schema.py` & `muninn-6.1.1/muninn/schema.py`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn.egg-info/PKG-INFO` & `muninn-6.1.1/muninn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: muninn
-Version: 6.1
+Version: 6.1.1
 Summary: Data product catalogue and archive system
 Home-page: https://github.com/stcorp/muninn
 Author: S[&]T
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `muninn-6.1/muninn.egg-info/SOURCES.txt` & `muninn-6.1.1/muninn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muninn-6.1/muninn.egg-info/entry_points.txt` & `muninn-6.1.1/muninn.egg-info/entry_points.txt`

 * *Files identical despite different names*

