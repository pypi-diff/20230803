# Comparing `tmp/jet-bridge-base-1.7.9.tar.gz` & `tmp/jet-bridge-base-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jet-bridge-base-1.7.9.tar", last modified: Thu Mar 16 07:39:01 2023, max compression
+gzip compressed data, was "dist/jet-bridge-base-1.8.2.tar", last modified: Thu Aug  3 11:16:09 2023, max compression
```

## Comparing `jet-bridge-base-1.7.9.tar` & `jet-bridge-base-1.8.2.tar`

### file list

```diff
@@ -1,453 +1,596 @@
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/
--rw-r--r--   0 f1nal      (501) staff       (20)    10529 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)     1099 2021-08-25 15:07:30.000000 jet-bridge-base-1.7.9/LICENSE
--rw-r--r--   0 f1nal      (501) staff       (20)       70 2021-08-25 15:07:30.000000 jet-bridge-base-1.7.9/MANIFEST.in
--rw-r--r--   0 f1nal      (501) staff       (20)    10243 2021-08-25 15:07:30.000000 jet-bridge-base-1.7.9/README.md
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/
--rw-r--r--   0 f1nal      (501) staff       (20)    10529 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-25 17:46:26.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/not-zip-safe
--rw-r--r--   0 f1nal      (501) staff       (20)    21662 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/SOURCES.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       94 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/requires.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       16 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/top_level.txt
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base.egg-info/dependency_links.txt
--rw-r--r--   0 f1nal      (501) staff       (20)     1148 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/setup.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/setup.cfg
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/
--rw-r--r--   0 f1nal      (501) staff       (20)     2993 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/filter_class.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4642 2023-03-10 03:57:06.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model_group.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1387 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model_segment.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)      746 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/lookups.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     3983 2023-03-10 03:57:19.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_group.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      942 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/lookups.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2704 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_class.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1441 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_m2m.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1984 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1470 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_m2m.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      521 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      486 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/float_filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1657 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_search.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      480 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/wkt_filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1865 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_relation.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1454 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3728 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_group.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1471 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      512 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/char_filter.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1909 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_segment.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      509 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/wkt_filter.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      533 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1661 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_search.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5988 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      496 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/lookups.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1834 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_relation.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1888 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_segment.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      483 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/char_filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1246 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/order_by.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2738 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_class.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1891 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      492 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1203 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/order_by.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      985 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3529 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      186 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      504 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1018 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      209 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      529 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/integer_filter.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      500 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/integer_filter.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      168 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/integer_filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1002 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model.py
--rw-r--r--   0 f1nal      (501) staff       (20)      720 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model_aggregate.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1479 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model_m2m.py
--rw-r--r--   0 f1nal      (501) staff       (20)      787 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/order_by.py
--rw-r--r--   0 f1nal      (501) staff       (20)      154 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/float_filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1107 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model_search.py
--rw-r--r--   0 f1nal      (501) staff       (20)      173 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/datetime_filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1572 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/model_relation.py
--rw-r--r--   0 f1nal      (501) staff       (20)      151 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/char_filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)     7316 2023-03-16 02:52:34.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)      148 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/wkt_filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4684 2023-03-15 17:06:44.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/filter_for_dbfield.py
--rw-r--r--   0 f1nal      (501) staff       (20)      160 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/filters/boolean_filter.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1021 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/store.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1893 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/configuration.py
--rw-r--r--   0 f1nal      (501) staff       (20)    19551 2023-03-03 07:41:36.000000 jet-bridge-base-1.7.9/jet_bridge_base/db.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2296 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/settings.pyc
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/
--rw-r--r--   0 f1nal      (501) staff       (20)     3668 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/page_number.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     3841 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/page_number.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      731 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/pagination.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3883 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/page_number.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/pagination.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      189 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      212 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      228 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/paginators/pagination.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/
--rw-r--r--   0 f1nal      (501) staff       (20)      109 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/optional_json.py
--rw-r--r--   0 f1nal      (501) staff       (20)      359 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/not_found.py
--rw-r--r--   0 f1nal      (501) staff       (20)      276 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/redirect.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      701 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/redirect.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      975 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      425 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/optional_json.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      801 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/not_found.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      726 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/template.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      732 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/redirect.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      757 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/template.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      926 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/base.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      822 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/json.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      188 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      787 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/json.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      454 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/optional_json.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      211 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      369 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/template.py
--rw-r--r--   0 f1nal      (501) staff       (20)      433 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/json.py
--rw-r--r--   0 f1nal      (501) staff       (20)      582 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/responses/base.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5172 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/request.py
--rw-r--r--   0 f1nal      (501) staff       (20)       56 2023-03-16 02:56:11.000000 jet-bridge-base-1.7.9/jet_bridge_base/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/
--rw-r--r--   0 f1nal      (501) staff       (20)     1247 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/mixin.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2535 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/strategy.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      970 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/storage.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1869 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/mixin.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3342 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/strategy.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1332 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/pipeline.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1915 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/mixin.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1025 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      990 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      192 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      215 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      584 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/utils.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1297 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/pipeline.py
--rw-r--r--   0 f1nal      (501) staff       (20)      322 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/external_auth/storage.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1527 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/encoders.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/
--rw-r--r--   0 f1nal      (501) staff       (20)      875 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/crypt.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1749 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/async_exec.py
--rw-r--r--   0 f1nal      (501) staff       (20)    38305 2023-03-16 02:46:24.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/graphql.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3854 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/backend.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5155 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/db_types.py
--rw-r--r--   0 f1nal      (501) staff       (20)      419 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/relations.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1775 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/async_exec.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      383 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/classes.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2060 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/exceptions.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    25906 2023-03-05 03:12:36.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/graphql.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1149 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/crypt.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3214 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/queryset.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      779 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/gql.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      851 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/utc.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1280 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/type_codes.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1866 2023-03-14 16:20:56.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_model.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1472 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_model.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2676 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/common.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2126 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/common.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1172 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/crypt.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1724 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/async_exec.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4560 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/db_types.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2506 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/db_types.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2127 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1953 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/siblings.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1729 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_database.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      954 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/http.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    19184 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/graphql.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3218 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/backend.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1786 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_database.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3240 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/queryset.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      820 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/gql.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1315 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/type_codes.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1996 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/siblings.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      184 2022-11-13 10:25:55.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      507 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/classes.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      972 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/http.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3217 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/backend.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      611 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/relations.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1876 2023-03-14 14:31:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/track_model.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2790 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/common.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2054 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/siblings.py
--rw-r--r--   0 f1nal      (501) staff       (20)      786 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/http.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1464 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/type_codes.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1308 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/track_database.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3329 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/queryset.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1945 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/exceptions.py
--rw-r--r--   0 f1nal      (501) staff       (20)      359 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/utc.py
--rw-r--r--   0 f1nal      (501) staff       (20)      215 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/classes.py
--rw-r--r--   0 f1nal      (501) staff       (20)      276 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/utils/gql.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/
--rw-r--r--   0 f1nal      (501) staff       (20)      722 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/model_relation_override.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      802 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/data_types.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      520 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/column.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      262 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/base.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1092 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/model_relation_override.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      515 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/table.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      233 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      289 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      779 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/data_types.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      517 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/data_types.py
--rw-r--r--   0 f1nal      (501) staff       (20)      118 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/table.py
--rw-r--r--   0 f1nal      (501) staff       (20)       83 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/base.py
--rw-r--r--   0 f1nal      (501) staff       (20)      125 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/models/column.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     3029 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/media_cache.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1632 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/encoders.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2786 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/status.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      644 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/messages.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2320 2022-11-13 04:37:30.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      611 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/messages.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1025 2022-11-13 04:37:30.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4587 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/request.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1615 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/store.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    13863 2023-03-05 03:12:34.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/db.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     9075 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/db.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1666 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/encoders.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2151 2023-03-14 14:05:43.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/sentry.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4327 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/configuration.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      650 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/router.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2717 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/status.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2351 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4515 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/configuration.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2856 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/reflect.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3095 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/media_cache.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4366 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/permissions.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3957 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/ssh_tunnel.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      248 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      678 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/router.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1017 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/logger.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4576 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/request.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6011 2023-03-14 14:27:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/permissions.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      258 2022-11-13 04:37:30.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2847 2023-02-16 15:32:23.000000 jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/reflect.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      613 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/logger.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/
--rw-r--r--   0 f1nal      (501) staff       (20)      415 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/missing_argument_error.py
--rw-r--r--   0 f1nal      (501) staff       (20)      250 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/validation_error.py
--rw-r--r--   0 f1nal      (501) staff       (20)      239 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/not_found.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      991 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/api.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      865 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/request_error.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      619 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      633 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      601 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/not_found.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      851 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      566 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/sql.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      595 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/sql.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      882 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      572 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/not_found.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      830 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/request_error.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      604 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      590 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      189 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      952 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/api.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      212 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      263 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/permission_denied.py
--rw-r--r--   0 f1nal      (501) staff       (20)      418 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/request_error.py
--rw-r--r--   0 f1nal      (501) staff       (20)      659 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/api.py
--rw-r--r--   0 f1nal      (501) staff       (20)      239 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/exceptions/sql.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/
--rw-r--r--   0 f1nal      (501) staff       (20)      563 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/model_group.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4873 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/relationship_override.py
--rw-r--r--   0 f1nal      (501) staff       (20)      475 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/message.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2142 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/reset_order.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      843 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_group.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6119 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/serializer.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     7099 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6348 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/serializer.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1087 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    12260 2023-03-10 04:29:29.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/sql.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    12048 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/sql.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      878 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_group.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      815 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/message.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      848 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/message.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3450 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1118 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1810 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reorder.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2454 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reset_order.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1963 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/table.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3353 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2443 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reset_order.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1954 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_description.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1842 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/table.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3991 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/relationship_override.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      190 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     7156 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1352 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_description.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1835 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reorder.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      213 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      369 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/model.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2272 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/model_description.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2509 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/reorder.py
--rw-r--r--   0 f1nal      (501) staff       (20)     6209 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/serializer.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1501 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/table.py
--rw-r--r--   0 f1nal      (501) staff       (20)    13587 2023-03-10 04:28:54.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/sql.py
--rw-r--r--   0 f1nal      (501) staff       (20)     9804 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/proxy_request.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4399 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/serializers/model_serializer.py
--rw-r--r--   0 f1nal      (501) staff       (20)      336 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/messages.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2163 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/media_cache.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2128 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)     7307 2023-03-14 14:27:19.000000 jet-bridge-base-1.7.9/jet_bridge_base/permissions.py
--rw-r--r--   0 f1nal      (501) staff       (20)      276 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/__init__.pyc
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/templates/
--rw-r--r--   0 f1nal      (501) staff       (20)       86 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/templates/403.html
--rw-r--r--   0 f1nal      (501) staff       (20)    91691 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/templates/500.debug.html
--rw-r--r--   0 f1nal      (501) staff       (20)       27 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/templates/500.html
--rw-r--r--   0 f1nal      (501) staff       (20)       83 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/templates/404.html
--rw-r--r--   0 f1nal      (501) staff       (20)      736 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/templates/external_auth_complete.html
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/
--rw-r--r--   0 f1nal      (501) staff       (20)     3469 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/field.py
--rw-r--r--   0 f1nal      (501) staff       (20)      206 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/raw.py
--rw-r--r--   0 f1nal      (501) staff       (20)      528 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/float.py
--rw-r--r--   0 f1nal      (501) staff       (20)      509 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/sql_params.py
--rw-r--r--   0 f1nal      (501) staff       (20)      570 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/char.py
--rw-r--r--   0 f1nal      (501) staff       (20)      470 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      931 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/float.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      688 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/raw.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      714 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/raw.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1003 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/datetime.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1069 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/sql_params.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3803 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/field.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1079 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/char.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1007 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/array.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1015 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/boolean.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      968 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/array.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      970 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/boolean.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1042 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/datetime.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1041 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/char.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      984 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/integer.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1238 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/json.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1073 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/wkt.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1118 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/wkt.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      939 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/integer.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3818 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/field.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      754 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1202 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/json.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1101 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/sql_params.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      714 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      681 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/boolean.py
--rw-r--r--   0 f1nal      (501) staff       (20)      530 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/integer.py
--rw-r--r--   0 f1nal      (501) staff       (20)      643 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/wkt.py
--rw-r--r--   0 f1nal      (501) staff       (20)      542 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/array.py
--rw-r--r--   0 f1nal      (501) staff       (20)      642 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/datetime.py
--rw-r--r--   0 f1nal      (501) staff       (20)      729 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/fields/json.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/
--rw-r--r--   0 f1nal      (501) staff       (20)     1289 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/check_token.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1244 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/check_token.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1197 2022-11-13 10:25:55.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/check_token.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      187 2022-11-13 10:25:55.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      210 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      293 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/router.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4104 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/ssh_tunnel.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1828 2023-03-14 14:05:40.000000 jet-bridge-base-1.7.9/jet_bridge_base/sentry.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/
--rw-r--r--   0 f1nal      (501) staff       (20)     6199 2023-03-03 08:35:13.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/graphql.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1704 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/register.py
--rw-r--r--   0 f1nal      (501) staff       (20)      753 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/reload.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/
--rw-r--r--   0 f1nal      (501) staff       (20)     1473 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/update.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1388 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/list.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1196 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/create.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1451 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/destroy.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1718 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1881 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/update.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1503 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/create.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      839 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/model.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1910 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/update.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1360 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/list.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      870 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/model.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1335 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/list.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      851 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      818 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1468 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/create.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1689 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      191 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      214 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      676 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/model.py
--rw-r--r--   0 f1nal      (501) staff       (20)      464 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/retrieve.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1394 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/login.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2219 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1411 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/login.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      198 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2216 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      221 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2128 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/complete.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1098 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/login.py
--rw-r--r--   0 f1nal      (501) staff       (20)      568 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/message.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1773 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/register.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1946 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/image_resize.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1110 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/file_upload.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1156 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/reload.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      808 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/api.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1156 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/proxy_request.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1734 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/register.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4119 2023-02-23 13:41:18.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/status.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     7654 2023-03-10 04:25:41.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5025 2023-03-05 03:12:36.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/graphql.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1476 2023-03-10 04:30:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/sql.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1531 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/sql.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      918 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/message.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      951 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/message.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6990 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     8488 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table_column.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1145 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/file_upload.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1123 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/reload.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3733 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     7205 2023-02-23 14:08:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model_description.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1871 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/image_resize.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      798 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/trigger_exception.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    10010 2023-02-23 13:41:18.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table_column.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2654 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/graphql.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3461 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      184 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      861 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/api.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1148 2022-11-13 10:25:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/proxy_request.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4431 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model_description.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1100 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      419 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/trigger_exception.py
--rw-r--r--   0 f1nal      (501) staff       (20)     9170 2023-03-10 04:14:38.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/model.py
--rw-r--r--   0 f1nal      (501) staff       (20)      541 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/api.py
--rw-r--r--   0 f1nal      (501) staff       (20)    12973 2023-02-23 13:41:13.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/table_column.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2212 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/image_resize.py
--rw-r--r--   0 f1nal      (501) staff       (20)    12033 2023-02-23 14:08:22.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/model_description.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3313 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/table.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1307 2023-03-10 04:29:50.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/sql.py
--rw-r--r--   0 f1nal      (501) staff       (20)      739 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/proxy_request.py
--rw-r--r--   0 f1nal      (501) staff       (20)      742 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/model_description_relationship_override.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:01.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     4157 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/generic_api.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6072 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/api.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4085 2023-02-16 15:32:26.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/generic_api.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      189 2022-11-13 10:25:57.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6172 2023-02-16 15:32:25.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/api.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      212 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6230 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/api.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3857 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/base/generic_api.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5448 2023-02-22 07:15:34.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/status.py
--rw-r--r--   0 f1nal      (501) staff       (20)      962 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/views/file_upload.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3857 2023-02-14 16:01:58.000000 jet-bridge-base-1.7.9/jet_bridge_base/reflect.py
--rw-r--r--   0 f1nal      (501) staff       (20)     1914 2022-11-13 04:32:28.000000 jet-bridge-base-1.7.9/jet_bridge_base/status.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/
+-rw-r--r--   0 f1nal      (501) staff       (20)    10529 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)     1099 2021-08-25 15:07:30.000000 jet-bridge-base-1.8.2/LICENSE
+-rw-r--r--   0 f1nal      (501) staff       (20)       70 2021-08-25 15:07:30.000000 jet-bridge-base-1.8.2/MANIFEST.in
+-rw-r--r--   0 f1nal      (501) staff       (20)    10243 2021-08-25 15:07:30.000000 jet-bridge-base-1.8.2/README.md
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/
+-rw-r--r--   0 f1nal      (501) staff       (20)    10529 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-25 17:46:26.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/not-zip-safe
+-rw-r--r--   0 f1nal      (501) staff       (20)    30269 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/SOURCES.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)      105 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/requires.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       16 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/top_level.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base.egg-info/dependency_links.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)     1170 2023-07-27 06:34:55.000000 jet-bridge-base-1.8.2/setup.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/setup.cfg
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/
+-rw-r--r--   0 f1nal      (501) staff       (20)     2993 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/filter_class.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4642 2023-03-10 03:57:06.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model_group.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1387 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model_segment.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      746 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/lookups.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3983 2023-03-10 03:57:19.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_group.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2706 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_class.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      942 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/lookups.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      946 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/lookups.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2704 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_class.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3985 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_group.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1441 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_m2m.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1996 2023-03-22 12:09:11.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1470 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_m2m.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2000 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      521 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1445 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_m2m.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      486 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/float_filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      490 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/float_filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1657 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_search.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1458 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      480 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/wkt_filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1865 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_relation.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      484 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/wkt_filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1454 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3728 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_group.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1471 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      512 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/char_filter.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1909 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_segment.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      509 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/wkt_filter.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6939 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1665 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_search.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      533 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1661 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_search.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6932 2023-03-23 02:45:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      496 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/lookups.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1892 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_segment.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1834 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_relation.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1838 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_relation.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1888 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_segment.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      483 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/char_filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1246 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/order_by.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      487 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/char_filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      496 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2738 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_class.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1891 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      492 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1203 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/order_by.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      985 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      989 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3529 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1207 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/order_by.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      186 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      508 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      504 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      190 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      504 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/integer_filter.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1018 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      209 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      529 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/integer_filter.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      500 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/integer_filter.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      168 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/integer_filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1002 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      720 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model_aggregate.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1479 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model_m2m.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      787 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/order_by.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      154 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/float_filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1107 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model_search.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      173 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/datetime_filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1572 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/model_relation.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      151 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/char_filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     7235 2023-03-22 12:19:23.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      148 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/wkt_filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4684 2023-03-22 12:09:02.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/filter_for_dbfield.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      160 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/filters/boolean_filter.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1021 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/store.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1893 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/configuration.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    21446 2023-07-27 19:10:45.000000 jet-bridge-base-1.8.2/jet_bridge_base/db.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2296 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/settings.pyc
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3668 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/page_number.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3841 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/page_number.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3845 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/page_number.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      731 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/pagination.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3883 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/page_number.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      712 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/pagination.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/pagination.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      189 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      193 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      212 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      228 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/paginators/pagination.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/
+-rw-r--r--   0 f1nal      (501) staff       (20)      109 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/optional_json.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      359 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/not_found.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      276 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/redirect.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      701 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/redirect.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      705 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/redirect.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      975 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      429 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/optional_json.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      425 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/optional_json.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      801 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/not_found.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      726 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/template.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      732 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/redirect.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      757 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/template.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      730 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/template.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      930 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      926 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/base.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      822 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/json.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      188 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      787 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/json.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      454 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/optional_json.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      791 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/json.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      192 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      211 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      369 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/template.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      433 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/json.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      582 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/responses/base.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     6384 2023-08-02 09:09:35.000000 jet-bridge-base-1.8.2/jet_bridge_base/request.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       56 2023-08-03 09:34:59.000000 jet-bridge-base-1.8.2/jet_bridge_base/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1247 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/mixin.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2535 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/strategy.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      970 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/storage.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1873 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/mixin.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1869 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/mixin.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3342 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/strategy.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1332 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/pipeline.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1915 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/mixin.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1025 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      990 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      994 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      192 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      196 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      215 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      584 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/utils.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1297 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/pipeline.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      322 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/external_auth/storage.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1527 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/encoders.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/
+-rw-r--r--   0 f1nal      (501) staff       (20)      875 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/crypt.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1749 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/async_exec.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    39581 2023-07-27 07:35:59.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/graphql.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3854 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/backend.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     5155 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/db_types.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      419 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/relations.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1775 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/async_exec.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      383 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/classes.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2060 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/exceptions.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2066 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/exceptions.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    26460 2023-07-27 07:36:01.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/graphql.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      783 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/gql.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3206 2023-04-20 15:20:02.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/queryset.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1143 2023-04-20 15:20:02.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/crypt.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1149 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/crypt.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3214 2023-02-16 15:32:23.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/queryset.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      779 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/gql.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    25900 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/graphql.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      851 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/utc.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1280 2023-04-21 03:04:16.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/type_codes.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1866 2023-03-14 16:20:56.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_model.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1472 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_model.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2680 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/common.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2979 2023-07-27 07:00:31.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/common.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2126 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1870 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_model.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1284 2023-04-20 15:30:04.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/type_codes.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1728 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/async_exec.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1172 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/crypt.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1724 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/async_exec.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4560 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/db_types.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2506 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/db_types.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4564 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/db_types.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1957 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/siblings.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2127 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1953 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/siblings.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2071 2023-04-10 14:18:31.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_database.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      565 2023-07-27 06:51:07.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/process.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2075 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_database.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      954 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/http.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    19184 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/graphql.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      958 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/http.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3218 2023-02-16 15:32:23.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/backend.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1786 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_database.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3218 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/backend.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3240 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/queryset.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      820 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/gql.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1315 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/type_codes.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1996 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/siblings.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      184 2022-11-13 10:25:55.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      511 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/classes.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      507 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/classes.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      972 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/http.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      188 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3217 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/backend.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      615 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/relations.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      611 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/relations.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1876 2023-03-14 14:31:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/track_model.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3023 2023-07-27 07:00:30.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/common.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2054 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/siblings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      786 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/http.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1464 2023-04-20 15:30:04.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/type_codes.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1645 2023-04-05 12:12:31.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/track_database.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3329 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/queryset.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1945 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/exceptions.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      266 2023-07-27 06:50:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/process.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      359 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/utc.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      215 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/classes.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      276 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/utils/gql.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/
+-rw-r--r--   0 f1nal      (501) staff       (20)      722 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/model_relation_override.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      802 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/data_types.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      520 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/column.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      266 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      262 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/base.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1092 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/model_relation_override.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1096 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/model_relation_override.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      515 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/table.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      233 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      237 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      783 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/data_types.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      289 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      779 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/data_types.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      517 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/data_types.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      118 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/table.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       83 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/base.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      125 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/models/column.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      426 2023-07-25 14:45:54.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/automap.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3018 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/media_cache.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3029 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/media_cache.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1632 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/encoders.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2786 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/status.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2790 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/status.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1631 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/encoders.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      644 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/messages.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2320 2022-11-13 04:37:30.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4586 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/request.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      615 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/messages.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      611 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/messages.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1025 2022-11-13 04:37:30.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4995 2023-07-27 19:20:38.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/request.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1615 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/store.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    14952 2023-07-27 19:20:37.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/db.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    14010 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/db.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1619 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/store.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     9075 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/db.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1666 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/encoders.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2151 2023-03-14 14:05:43.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/sentry.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      654 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/router.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4327 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/configuration.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      650 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/router.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2155 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/sentry.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2717 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/status.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2470 2023-07-27 17:16:40.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2402 2023-04-20 15:12:02.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4515 2023-02-16 15:32:23.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/configuration.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4519 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/configuration.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2856 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/reflect.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3095 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/media_cache.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4366 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/permissions.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3961 2023-04-20 15:20:02.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/ssh_tunnel.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3957 2023-02-16 15:32:23.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/ssh_tunnel.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      248 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      678 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/router.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1021 2023-04-20 15:12:02.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/logger.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1017 2023-02-16 15:32:23.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/logger.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      253 2023-04-20 15:30:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3184 2023-04-20 15:30:04.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/reflect.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4576 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/request.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6011 2023-07-27 06:38:36.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/permissions.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      258 2022-11-13 04:37:30.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5985 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/permissions.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3441 2023-07-27 07:54:55.000000 jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/reflect.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      613 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/logger.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/
+-rw-r--r--   0 f1nal      (501) staff       (20)      415 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/missing_argument_error.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      250 2023-04-27 08:17:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/validation_error.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      239 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/not_found.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      991 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      865 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/request_error.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      619 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      633 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      601 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/not_found.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      570 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/sql.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      855 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      851 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      566 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/sql.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      595 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/sql.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      882 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      572 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/not_found.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      834 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/request_error.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      830 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/request_error.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      576 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/not_found.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      594 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      604 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      608 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      590 2023-04-27 08:17:31.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      189 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      956 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/api.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      952 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/api.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      193 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      212 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      263 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/permission_denied.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      418 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/request_error.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      659 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/api.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      239 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/exceptions/sql.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/
+-rw-r--r--   0 f1nal      (501) staff       (20)      563 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/model_group.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4873 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/relationship_override.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      475 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/message.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2142 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/reset_order.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      843 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_group.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      847 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_group.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6119 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/serializer.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6342 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/serializer.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7099 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6348 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/serializer.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1091 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1087 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    12261 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/sql.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    12418 2023-08-02 08:34:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/sql.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    12048 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/sql.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      878 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_group.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      815 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/message.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      819 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/message.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      848 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/message.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3450 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1118 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1814 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reorder.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1810 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reorder.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2454 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reset_order.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3454 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1963 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/table.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3353 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1967 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/table.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1958 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_description.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2443 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reset_order.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2447 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reset_order.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1973 2023-07-26 15:25:40.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_description.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1842 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/table.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3995 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/relationship_override.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3991 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/relationship_override.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      190 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7158 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7156 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1352 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_description.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1835 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reorder.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      194 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      213 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      369 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/model.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2309 2023-07-17 14:41:18.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/model_description.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2509 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/reorder.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     6209 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/serializer.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1501 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/table.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    13967 2023-07-28 09:45:20.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/sql.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     9804 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/proxy_request.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4399 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/serializers/model_serializer.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      336 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/messages.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2163 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/media_cache.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2249 2023-07-27 17:16:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     7285 2023-07-27 06:38:35.000000 jet-bridge-base-1.8.2/jet_bridge_base/permissions.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      276 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/__init__.pyc
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/templates/
+-rw-r--r--   0 f1nal      (501) staff       (20)       86 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/templates/403.html
+-rw-r--r--   0 f1nal      (501) staff       (20)    91691 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/templates/500.debug.html
+-rw-r--r--   0 f1nal      (501) staff       (20)       27 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/templates/500.html
+-rw-r--r--   0 f1nal      (501) staff       (20)       83 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/templates/404.html
+-rw-r--r--   0 f1nal      (501) staff       (20)      736 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/templates/external_auth_complete.html
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3469 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/field.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      206 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/raw.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      528 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/float.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      509 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/sql_params.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      570 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/char.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      470 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      935 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/float.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      931 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/float.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      688 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/raw.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      692 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/raw.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      714 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/raw.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1003 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/datetime.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1069 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/sql_params.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1073 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/sql_params.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1007 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/datetime.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3803 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/field.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3803 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/field.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1079 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/char.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1007 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/array.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      972 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/array.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1019 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/boolean.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1015 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/boolean.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      968 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/array.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      970 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/boolean.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1042 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/datetime.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1045 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/char.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1041 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/char.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      984 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/integer.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1238 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/json.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1073 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/wkt.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1118 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/wkt.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1077 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/wkt.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      943 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/integer.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      939 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/integer.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3818 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/field.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      754 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1202 2023-02-16 15:32:25.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/json.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1206 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/json.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      758 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1101 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/sql_params.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      714 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      681 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/boolean.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      530 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/integer.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      798 2023-08-03 08:56:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/wkt.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      542 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/array.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      642 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/datetime.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      729 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/fields/json.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1289 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/check_token.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:08.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1244 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/check_token.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1201 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/check_token.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1197 2022-11-13 10:25:55.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/check_token.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      187 2022-11-13 10:25:55.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      191 2023-04-20 15:15:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      210 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      293 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/router.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4104 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/ssh_tunnel.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1828 2023-03-14 14:05:40.000000 jet-bridge-base-1.8.2/jet_bridge_base/sentry.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      273 2023-07-17 18:57:44.000000 jet-bridge-base-1.8.2/jet_bridge_base/automap.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/
+-rw-r--r--   0 f1nal      (501) staff       (20)     7837 2023-07-27 07:48:55.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/graphql.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1704 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/register.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      753 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/reload.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1473 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/update.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1388 2023-06-26 12:22:04.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/list.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1196 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/create.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1451 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/destroy.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1718 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1881 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/update.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1885 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/update.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1503 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/create.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      843 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      839 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1910 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/update.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1360 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/list.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      870 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1339 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/list.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1335 2023-06-26 16:01:13.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/list.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      851 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      822 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      818 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1693 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1472 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/create.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1468 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/create.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1689 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      191 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      195 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      214 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      676 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/model.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      464 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/retrieve.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1370 2023-04-27 08:20:21.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/discover_connection.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     2223 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1394 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/login.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2219 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1411 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/login.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1415 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/login.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      198 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      202 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2216 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      221 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2128 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/complete.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1098 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/login.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      568 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/message.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1773 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/register.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1946 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/image_resize.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1110 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/file_upload.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1114 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/file_upload.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1156 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/reload.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      808 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1736 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/register.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1156 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/proxy_request.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1630 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/discover_connection.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1626 2023-04-27 08:36:06.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/discover_connection.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1734 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/register.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7658 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4811 2023-07-27 07:58:46.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/status.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4123 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/status.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7654 2023-07-28 07:35:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6114 2023-07-27 07:48:56.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/graphql.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1484 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/sql.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1476 2023-03-10 04:30:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/sql.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1531 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/sql.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5129 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/graphql.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      918 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/message.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      922 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/message.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      951 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/message.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6990 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     8488 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table_column.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1145 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/file_upload.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1123 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/reload.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3733 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3737 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1127 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/reload.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7207 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     7268 2023-07-26 15:25:40.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1871 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/image_resize.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      798 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/trigger_exception.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      802 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/trigger_exception.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1875 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/image_resize.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    10014 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table_column.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    10010 2023-02-23 13:41:18.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table_column.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2027 2023-04-20 15:30:06.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/discover_table.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2654 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/graphql.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3461 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2158 2023-07-26 15:25:39.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/discover_table.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      184 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      865 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/api.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1152 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/proxy_request.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      861 2023-07-28 07:35:03.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/api.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1148 2022-11-13 10:25:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/proxy_request.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4431 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      188 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1104 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1100 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      419 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/trigger_exception.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     9170 2023-07-28 07:35:07.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/model.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      541 2023-07-28 07:35:01.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/api.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    13195 2023-08-03 09:18:53.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/table_column.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2212 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/image_resize.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2116 2023-07-17 14:41:18.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/discover_table.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    12365 2023-08-03 09:27:20.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/model_description.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3313 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/table.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1307 2023-03-10 04:29:50.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/sql.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      739 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/proxy_request.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      742 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/model_description_relationship_override.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:09.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     4157 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/generic_api.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6072 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4085 2023-02-16 15:32:26.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/generic_api.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4089 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/generic_api.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      189 2022-11-13 10:25:57.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6235 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/api.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6243 2023-07-28 07:29:00.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/api.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      193 2023-04-20 15:28:47.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      212 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6377 2023-07-28 07:28:53.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/api.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3857 2023-02-14 16:01:58.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/base/generic_api.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     6904 2023-07-27 07:58:44.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/status.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      962 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/views/file_upload.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4635 2023-07-27 07:54:54.000000 jet-bridge-base-1.8.2/jet_bridge_base/reflect.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     1914 2022-11-13 04:32:28.000000 jet-bridge-base-1.8.2/jet_bridge_base/status.py
```

### Comparing `jet-bridge-base-1.7.9/PKG-INFO` & `jet-bridge-base-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-bridge-base
-Version: 1.7.9
+Version: 1.8.2
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-bridge-base
 Author: Denis Kildishev
 Author-email: support@jetadmin.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jet-bridge-base-1.7.9/LICENSE` & `jet-bridge-base-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/README.md` & `jet-bridge-base-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base.egg-info/PKG-INFO` & `jet-bridge-base-1.8.2/jet_bridge_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-bridge-base
-Version: 1.7.9
+Version: 1.8.2
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-bridge-base
 Author: Denis Kildishev
 Author-email: support@jetadmin.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base.egg-info/SOURCES.txt` & `jet-bridge-base-1.8.2/jet_bridge_base.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 jet_bridge_base/__init__.py
 jet_bridge_base/__init__.pyc
+jet_bridge_base/automap.py
 jet_bridge_base/configuration.py
 jet_bridge_base/db.py
 jet_bridge_base/encoders.py
 jet_bridge_base/logger.py
 jet_bridge_base/media_cache.py
 jet_bridge_base/messages.py
 jet_bridge_base/permissions.py
@@ -24,121 +25,163 @@
 jet_bridge_base.egg-info/SOURCES.txt
 jet_bridge_base.egg-info/dependency_links.txt
 jet_bridge_base.egg-info/not-zip-safe
 jet_bridge_base.egg-info/requires.txt
 jet_bridge_base.egg-info/top_level.txt
 jet_bridge_base/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/__pycache__/__init__.cpython-37.pyc
+jet_bridge_base/__pycache__/automap.cpython-36.pyc
 jet_bridge_base/__pycache__/configuration.cpython-310.pyc
 jet_bridge_base/__pycache__/configuration.cpython-36.pyc
+jet_bridge_base/__pycache__/configuration.cpython-37.pyc
 jet_bridge_base/__pycache__/db.cpython-310.pyc
 jet_bridge_base/__pycache__/db.cpython-36.pyc
+jet_bridge_base/__pycache__/db.cpython-37.pyc
 jet_bridge_base/__pycache__/encoders.cpython-310.pyc
 jet_bridge_base/__pycache__/encoders.cpython-36.pyc
+jet_bridge_base/__pycache__/encoders.cpython-37.pyc
 jet_bridge_base/__pycache__/logger.cpython-310.pyc
 jet_bridge_base/__pycache__/logger.cpython-36.pyc
+jet_bridge_base/__pycache__/logger.cpython-37.pyc
 jet_bridge_base/__pycache__/media_cache.cpython-310.pyc
 jet_bridge_base/__pycache__/media_cache.cpython-36.pyc
+jet_bridge_base/__pycache__/media_cache.cpython-37.pyc
 jet_bridge_base/__pycache__/messages.cpython-310.pyc
 jet_bridge_base/__pycache__/messages.cpython-36.pyc
+jet_bridge_base/__pycache__/messages.cpython-37.pyc
 jet_bridge_base/__pycache__/permissions.cpython-310.pyc
 jet_bridge_base/__pycache__/permissions.cpython-36.pyc
+jet_bridge_base/__pycache__/permissions.cpython-37.pyc
 jet_bridge_base/__pycache__/reflect.cpython-310.pyc
 jet_bridge_base/__pycache__/reflect.cpython-36.pyc
+jet_bridge_base/__pycache__/reflect.cpython-37.pyc
 jet_bridge_base/__pycache__/request.cpython-310.pyc
 jet_bridge_base/__pycache__/request.cpython-36.pyc
+jet_bridge_base/__pycache__/request.cpython-37.pyc
 jet_bridge_base/__pycache__/router.cpython-310.pyc
 jet_bridge_base/__pycache__/router.cpython-36.pyc
+jet_bridge_base/__pycache__/router.cpython-37.pyc
 jet_bridge_base/__pycache__/sentry.cpython-36.pyc
+jet_bridge_base/__pycache__/sentry.cpython-37.pyc
 jet_bridge_base/__pycache__/settings.cpython-310.pyc
 jet_bridge_base/__pycache__/settings.cpython-36.pyc
+jet_bridge_base/__pycache__/settings.cpython-37.pyc
 jet_bridge_base/__pycache__/ssh_tunnel.cpython-36.pyc
+jet_bridge_base/__pycache__/ssh_tunnel.cpython-37.pyc
 jet_bridge_base/__pycache__/status.cpython-310.pyc
 jet_bridge_base/__pycache__/status.cpython-36.pyc
+jet_bridge_base/__pycache__/status.cpython-37.pyc
 jet_bridge_base/__pycache__/store.cpython-36.pyc
+jet_bridge_base/__pycache__/store.cpython-37.pyc
 jet_bridge_base/commands/__init__.py
 jet_bridge_base/commands/check_token.py
 jet_bridge_base/commands/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/commands/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/commands/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/commands/__pycache__/check_token.cpython-310.pyc
 jet_bridge_base/commands/__pycache__/check_token.cpython-36.pyc
+jet_bridge_base/commands/__pycache__/check_token.cpython-37.pyc
 jet_bridge_base/exceptions/__init__.py
 jet_bridge_base/exceptions/api.py
 jet_bridge_base/exceptions/missing_argument_error.py
 jet_bridge_base/exceptions/not_found.py
 jet_bridge_base/exceptions/permission_denied.py
 jet_bridge_base/exceptions/request_error.py
 jet_bridge_base/exceptions/sql.py
 jet_bridge_base/exceptions/validation_error.py
 jet_bridge_base/exceptions/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/api.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/api.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/api.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/not_found.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/not_found.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/not_found.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/request_error.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/request_error.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/request_error.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/sql.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/sql.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/sql.cpython-37.pyc
 jet_bridge_base/exceptions/__pycache__/validation_error.cpython-310.pyc
 jet_bridge_base/exceptions/__pycache__/validation_error.cpython-36.pyc
+jet_bridge_base/exceptions/__pycache__/validation_error.cpython-37.pyc
 jet_bridge_base/external_auth/__init__.py
 jet_bridge_base/external_auth/mixin.py
 jet_bridge_base/external_auth/pipeline.py
 jet_bridge_base/external_auth/storage.py
 jet_bridge_base/external_auth/strategy.py
 jet_bridge_base/external_auth/utils.py
 jet_bridge_base/external_auth/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/external_auth/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/external_auth/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/external_auth/__pycache__/mixin.cpython-310.pyc
 jet_bridge_base/external_auth/__pycache__/mixin.cpython-36.pyc
+jet_bridge_base/external_auth/__pycache__/mixin.cpython-37.pyc
 jet_bridge_base/external_auth/__pycache__/pipeline.cpython-310.pyc
 jet_bridge_base/external_auth/__pycache__/storage.cpython-310.pyc
 jet_bridge_base/external_auth/__pycache__/strategy.cpython-310.pyc
 jet_bridge_base/external_auth/__pycache__/utils.cpython-310.pyc
 jet_bridge_base/external_auth/__pycache__/utils.cpython-36.pyc
+jet_bridge_base/external_auth/__pycache__/utils.cpython-37.pyc
 jet_bridge_base/fields/__init__.py
 jet_bridge_base/fields/array.py
 jet_bridge_base/fields/boolean.py
 jet_bridge_base/fields/char.py
 jet_bridge_base/fields/datetime.py
 jet_bridge_base/fields/field.py
 jet_bridge_base/fields/float.py
 jet_bridge_base/fields/integer.py
 jet_bridge_base/fields/json.py
 jet_bridge_base/fields/raw.py
 jet_bridge_base/fields/sql_params.py
 jet_bridge_base/fields/wkt.py
 jet_bridge_base/fields/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/array.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/array.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/array.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/boolean.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/boolean.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/boolean.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/char.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/char.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/char.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/datetime.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/datetime.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/datetime.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/field.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/field.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/field.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/float.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/float.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/integer.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/integer.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/integer.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/json.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/json.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/json.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/raw.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/raw.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/raw.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/sql_params.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/sql_params.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/sql_params.cpython-37.pyc
 jet_bridge_base/fields/__pycache__/wkt.cpython-310.pyc
 jet_bridge_base/fields/__pycache__/wkt.cpython-36.pyc
+jet_bridge_base/fields/__pycache__/wkt.cpython-37.pyc
 jet_bridge_base/filters/__init__.py
 jet_bridge_base/filters/boolean_filter.py
 jet_bridge_base/filters/char_filter.py
 jet_bridge_base/filters/datetime_filter.py
 jet_bridge_base/filters/filter.py
 jet_bridge_base/filters/filter_class.py
 jet_bridge_base/filters/filter_for_dbfield.py
@@ -152,92 +195,124 @@
 jet_bridge_base/filters/model_relation.py
 jet_bridge_base/filters/model_search.py
 jet_bridge_base/filters/model_segment.py
 jet_bridge_base/filters/order_by.py
 jet_bridge_base/filters/wkt_filter.py
 jet_bridge_base/filters/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/boolean_filter.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/boolean_filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/boolean_filter.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/char_filter.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/char_filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/char_filter.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/datetime_filter.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/datetime_filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/datetime_filter.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/filter.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/filter.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/filter_class.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/filter_class.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/filter_class.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/float_filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/float_filter.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/integer_filter.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/integer_filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/integer_filter.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/lookups.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/lookups.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/lookups.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model_aggregate.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model_aggregate.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model_aggregate.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model_group.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model_group.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model_group.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model_m2m.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model_m2m.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model_m2m.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model_relation.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model_relation.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model_relation.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model_search.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model_search.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model_search.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/model_segment.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/model_segment.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/model_segment.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/order_by.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/order_by.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/order_by.cpython-37.pyc
 jet_bridge_base/filters/__pycache__/wkt_filter.cpython-310.pyc
 jet_bridge_base/filters/__pycache__/wkt_filter.cpython-36.pyc
+jet_bridge_base/filters/__pycache__/wkt_filter.cpython-37.pyc
 jet_bridge_base/models/__init__.py
 jet_bridge_base/models/base.py
 jet_bridge_base/models/column.py
 jet_bridge_base/models/data_types.py
 jet_bridge_base/models/model_relation_override.py
 jet_bridge_base/models/table.py
 jet_bridge_base/models/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/models/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/models/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/models/__pycache__/base.cpython-36.pyc
+jet_bridge_base/models/__pycache__/base.cpython-37.pyc
 jet_bridge_base/models/__pycache__/column.cpython-310.pyc
 jet_bridge_base/models/__pycache__/data_types.cpython-310.pyc
 jet_bridge_base/models/__pycache__/data_types.cpython-36.pyc
+jet_bridge_base/models/__pycache__/data_types.cpython-37.pyc
 jet_bridge_base/models/__pycache__/model_relation_override.cpython-36.pyc
+jet_bridge_base/models/__pycache__/model_relation_override.cpython-37.pyc
 jet_bridge_base/models/__pycache__/table.cpython-310.pyc
 jet_bridge_base/paginators/__init__.py
 jet_bridge_base/paginators/page_number.py
 jet_bridge_base/paginators/pagination.py
 jet_bridge_base/paginators/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/paginators/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/paginators/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/paginators/__pycache__/page_number.cpython-310.pyc
 jet_bridge_base/paginators/__pycache__/page_number.cpython-36.pyc
+jet_bridge_base/paginators/__pycache__/page_number.cpython-37.pyc
 jet_bridge_base/paginators/__pycache__/pagination.cpython-310.pyc
 jet_bridge_base/paginators/__pycache__/pagination.cpython-36.pyc
+jet_bridge_base/paginators/__pycache__/pagination.cpython-37.pyc
 jet_bridge_base/responses/__init__.py
 jet_bridge_base/responses/base.py
 jet_bridge_base/responses/json.py
 jet_bridge_base/responses/not_found.py
 jet_bridge_base/responses/optional_json.py
 jet_bridge_base/responses/redirect.py
 jet_bridge_base/responses/template.py
 jet_bridge_base/responses/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/responses/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/responses/__pycache__/base.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/base.cpython-36.pyc
+jet_bridge_base/responses/__pycache__/base.cpython-37.pyc
 jet_bridge_base/responses/__pycache__/json.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/json.cpython-36.pyc
+jet_bridge_base/responses/__pycache__/json.cpython-37.pyc
 jet_bridge_base/responses/__pycache__/not_found.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/optional_json.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/optional_json.cpython-36.pyc
+jet_bridge_base/responses/__pycache__/optional_json.cpython-37.pyc
 jet_bridge_base/responses/__pycache__/redirect.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/redirect.cpython-36.pyc
+jet_bridge_base/responses/__pycache__/redirect.cpython-37.pyc
 jet_bridge_base/responses/__pycache__/template.cpython-310.pyc
 jet_bridge_base/responses/__pycache__/template.cpython-36.pyc
+jet_bridge_base/responses/__pycache__/template.cpython-37.pyc
 jet_bridge_base/serializers/__init__.py
 jet_bridge_base/serializers/message.py
 jet_bridge_base/serializers/model.py
 jet_bridge_base/serializers/model_description.py
 jet_bridge_base/serializers/model_group.py
 jet_bridge_base/serializers/model_serializer.py
 jet_bridge_base/serializers/proxy_request.py
@@ -245,37 +320,50 @@
 jet_bridge_base/serializers/reorder.py
 jet_bridge_base/serializers/reset_order.py
 jet_bridge_base/serializers/serializer.py
 jet_bridge_base/serializers/sql.py
 jet_bridge_base/serializers/table.py
 jet_bridge_base/serializers/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/message.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/message.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/message.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/model.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/model.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/model.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/model_description.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/model_description.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/model_description.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/model_group.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/model_group.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/model_group.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/model_serializer.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/model_serializer.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/model_serializer.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/proxy_request.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/proxy_request.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/proxy_request.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/relationship_override.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/relationship_override.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/reorder.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/reorder.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/reorder.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/reset_order.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/reset_order.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/reset_order.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/serializer.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/serializer.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/serializer.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/sql.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/sql.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/sql.cpython-37.pyc
 jet_bridge_base/serializers/__pycache__/table.cpython-310.pyc
 jet_bridge_base/serializers/__pycache__/table.cpython-36.pyc
+jet_bridge_base/serializers/__pycache__/table.cpython-37.pyc
 jet_bridge_base/templates/403.html
 jet_bridge_base/templates/404.html
 jet_bridge_base/templates/500.debug.html
 jet_bridge_base/templates/500.html
 jet_bridge_base/templates/external_auth_complete.html
 jet_bridge_base/utils/__init__.py
 jet_bridge_base/utils/async_exec.py
@@ -284,57 +372,78 @@
 jet_bridge_base/utils/common.py
 jet_bridge_base/utils/crypt.py
 jet_bridge_base/utils/db_types.py
 jet_bridge_base/utils/exceptions.py
 jet_bridge_base/utils/gql.py
 jet_bridge_base/utils/graphql.py
 jet_bridge_base/utils/http.py
+jet_bridge_base/utils/process.py
 jet_bridge_base/utils/queryset.py
 jet_bridge_base/utils/relations.py
 jet_bridge_base/utils/siblings.py
 jet_bridge_base/utils/track_database.py
 jet_bridge_base/utils/track_model.py
 jet_bridge_base/utils/type_codes.py
 jet_bridge_base/utils/utc.py
 jet_bridge_base/utils/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/async_exec.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/async_exec.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/async_exec.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/backend.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/backend.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/backend.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/classes.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/classes.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/classes.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/common.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/common.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/common.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/crypt.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/crypt.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/crypt.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/db_types.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/db_types.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/db_types.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/exceptions.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/exceptions.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/exceptions.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/gql.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/gql.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/gql.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/graphql.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/graphql.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/graphql.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/http.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/http.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/http.cpython-37.pyc
+jet_bridge_base/utils/__pycache__/process.cpython-36.pyc
 jet_bridge_base/utils/__pycache__/queryset.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/queryset.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/queryset.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/relations.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/relations.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/siblings.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/siblings.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/siblings.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/track_database.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/track_database.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/track_database.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/track_model.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/track_model.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/track_model.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/type_codes.cpython-310.pyc
 jet_bridge_base/utils/__pycache__/type_codes.cpython-36.pyc
+jet_bridge_base/utils/__pycache__/type_codes.cpython-37.pyc
 jet_bridge_base/utils/__pycache__/utc.cpython-310.pyc
 jet_bridge_base/views/__init__.py
 jet_bridge_base/views/api.py
+jet_bridge_base/views/discover_connection.py
+jet_bridge_base/views/discover_table.py
 jet_bridge_base/views/file_upload.py
 jet_bridge_base/views/graphql.py
 jet_bridge_base/views/image_resize.py
 jet_bridge_base/views/message.py
 jet_bridge_base/views/model.py
 jet_bridge_base/views/model_description.py
 jet_bridge_base/views/model_description_relationship_override.py
@@ -344,75 +453,109 @@
 jet_bridge_base/views/sql.py
 jet_bridge_base/views/status.py
 jet_bridge_base/views/table.py
 jet_bridge_base/views/table_column.py
 jet_bridge_base/views/trigger_exception.py
 jet_bridge_base/views/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/views/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/views/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/views/__pycache__/api.cpython-310.pyc
 jet_bridge_base/views/__pycache__/api.cpython-36.pyc
+jet_bridge_base/views/__pycache__/api.cpython-37.pyc
+jet_bridge_base/views/__pycache__/discover_connection.cpython-36.pyc
+jet_bridge_base/views/__pycache__/discover_connection.cpython-37.pyc
+jet_bridge_base/views/__pycache__/discover_table.cpython-36.pyc
+jet_bridge_base/views/__pycache__/discover_table.cpython-37.pyc
 jet_bridge_base/views/__pycache__/file_upload.cpython-310.pyc
 jet_bridge_base/views/__pycache__/file_upload.cpython-36.pyc
+jet_bridge_base/views/__pycache__/file_upload.cpython-37.pyc
 jet_bridge_base/views/__pycache__/graphql.cpython-310.pyc
 jet_bridge_base/views/__pycache__/graphql.cpython-36.pyc
+jet_bridge_base/views/__pycache__/graphql.cpython-37.pyc
 jet_bridge_base/views/__pycache__/image_resize.cpython-310.pyc
 jet_bridge_base/views/__pycache__/image_resize.cpython-36.pyc
+jet_bridge_base/views/__pycache__/image_resize.cpython-37.pyc
 jet_bridge_base/views/__pycache__/message.cpython-310.pyc
 jet_bridge_base/views/__pycache__/message.cpython-36.pyc
+jet_bridge_base/views/__pycache__/message.cpython-37.pyc
 jet_bridge_base/views/__pycache__/model.cpython-310.pyc
 jet_bridge_base/views/__pycache__/model.cpython-36.pyc
+jet_bridge_base/views/__pycache__/model.cpython-37.pyc
 jet_bridge_base/views/__pycache__/model_description.cpython-310.pyc
 jet_bridge_base/views/__pycache__/model_description.cpython-36.pyc
+jet_bridge_base/views/__pycache__/model_description.cpython-37.pyc
 jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-36.pyc
+jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-37.pyc
 jet_bridge_base/views/__pycache__/proxy_request.cpython-310.pyc
 jet_bridge_base/views/__pycache__/proxy_request.cpython-36.pyc
+jet_bridge_base/views/__pycache__/proxy_request.cpython-37.pyc
 jet_bridge_base/views/__pycache__/register.cpython-310.pyc
 jet_bridge_base/views/__pycache__/register.cpython-36.pyc
+jet_bridge_base/views/__pycache__/register.cpython-37.pyc
 jet_bridge_base/views/__pycache__/reload.cpython-310.pyc
 jet_bridge_base/views/__pycache__/reload.cpython-36.pyc
+jet_bridge_base/views/__pycache__/reload.cpython-37.pyc
 jet_bridge_base/views/__pycache__/sql.cpython-310.pyc
 jet_bridge_base/views/__pycache__/sql.cpython-36.pyc
+jet_bridge_base/views/__pycache__/sql.cpython-37.pyc
 jet_bridge_base/views/__pycache__/status.cpython-36.pyc
+jet_bridge_base/views/__pycache__/status.cpython-37.pyc
 jet_bridge_base/views/__pycache__/table.cpython-310.pyc
 jet_bridge_base/views/__pycache__/table.cpython-36.pyc
+jet_bridge_base/views/__pycache__/table.cpython-37.pyc
 jet_bridge_base/views/__pycache__/table_column.cpython-310.pyc
 jet_bridge_base/views/__pycache__/table_column.cpython-36.pyc
+jet_bridge_base/views/__pycache__/table_column.cpython-37.pyc
 jet_bridge_base/views/__pycache__/trigger_exception.cpython-36.pyc
+jet_bridge_base/views/__pycache__/trigger_exception.cpython-37.pyc
 jet_bridge_base/views/base/__init__.py
 jet_bridge_base/views/base/api.py
 jet_bridge_base/views/base/generic_api.py
 jet_bridge_base/views/base/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/views/base/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/views/base/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/views/base/__pycache__/api.cpython-310.pyc
 jet_bridge_base/views/base/__pycache__/api.cpython-36.pyc
+jet_bridge_base/views/base/__pycache__/api.cpython-37.pyc
 jet_bridge_base/views/base/__pycache__/generic_api.cpython-310.pyc
 jet_bridge_base/views/base/__pycache__/generic_api.cpython-36.pyc
+jet_bridge_base/views/base/__pycache__/generic_api.cpython-37.pyc
 jet_bridge_base/views/external_auth/__init__.py
 jet_bridge_base/views/external_auth/complete.py
 jet_bridge_base/views/external_auth/login.py
 jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/views/external_auth/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/views/external_auth/__pycache__/complete.cpython-310.pyc
 jet_bridge_base/views/external_auth/__pycache__/complete.cpython-36.pyc
+jet_bridge_base/views/external_auth/__pycache__/complete.cpython-37.pyc
 jet_bridge_base/views/external_auth/__pycache__/login.cpython-310.pyc
 jet_bridge_base/views/external_auth/__pycache__/login.cpython-36.pyc
+jet_bridge_base/views/external_auth/__pycache__/login.cpython-37.pyc
 jet_bridge_base/views/mixins/__init__.py
 jet_bridge_base/views/mixins/create.py
 jet_bridge_base/views/mixins/destroy.py
 jet_bridge_base/views/mixins/list.py
 jet_bridge_base/views/mixins/model.py
 jet_bridge_base/views/mixins/retrieve.py
 jet_bridge_base/views/mixins/update.py
 jet_bridge_base/views/mixins/__pycache__/__init__.cpython-310.pyc
 jet_bridge_base/views/mixins/__pycache__/__init__.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/__init__.cpython-37.pyc
 jet_bridge_base/views/mixins/__pycache__/create.cpython-310.pyc
 jet_bridge_base/views/mixins/__pycache__/create.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/create.cpython-37.pyc
 jet_bridge_base/views/mixins/__pycache__/destroy.cpython-310.pyc
 jet_bridge_base/views/mixins/__pycache__/destroy.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/destroy.cpython-37.pyc
 jet_bridge_base/views/mixins/__pycache__/list.cpython-310.pyc
 jet_bridge_base/views/mixins/__pycache__/list.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/list.cpython-37.pyc
 jet_bridge_base/views/mixins/__pycache__/model.cpython-310.pyc
 jet_bridge_base/views/mixins/__pycache__/model.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/model.cpython-37.pyc
 jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-310.pyc
 jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-37.pyc
 jet_bridge_base/views/mixins/__pycache__/update.cpython-310.pyc
-jet_bridge_base/views/mixins/__pycache__/update.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/update.cpython-36.pyc
+jet_bridge_base/views/mixins/__pycache__/update.cpython-37.pyc
```

### Comparing `jet-bridge-base-1.7.9/setup.py` & `jet-bridge-base-1.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     except TypeError:
         file = open(path)
     return file.read()
 
 
 def get_install_requires():
     install_requires = [
-        'sqlalchemy',
+        'sqlalchemy<2.0',
         'six',
         'requests',
         'Pillow',
         'dateparser',
+        'psutil',
         'social-auth-core',
         'prompt_toolkit==2.0.9',
         'graphene<3.0',
     ]
 
     try:
         from collections import OrderedDict
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/filter_class.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/filter_class.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model_group.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model_group.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model_segment.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model_segment.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/lookups.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/lookups.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_group.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_group.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/lookups.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/lookups.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_class.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_class.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_m2m.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_m2m.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 330d 0d0a 76b0 eb63 2912 0000 e300 0000  3...v..c).......
+00000000: 330d 0d0a deef 1a64 4c12 0000 e300 0000  3......dL.......
 00000010: 0000 0000 0000 0000 001e 0000 0040 0000  .............@..
-00000020: 0073 2602 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000020: 0073 2e02 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6406 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 0100 6400 6408 6c0e  d.l.m.Z...d.d.l.
 00000080: 6d0f 5a0f 0100 6505 6a10 6505 6a11 6505  m.Z...e.j.e.j.e.
 00000090: 6a12 6505 6a13 6505 6a14 6505 6a15 6505  j.e.j.e.j.e.j.e.
@@ -12,113 +12,114 @@
 000000b0: 6a10 6505 6a11 6505 6a12 6505 6a13 6505  j.e.j.e.j.e.j.e.
 000000c0: 6a14 6505 6a15 6505 6a16 6505 6a17 6505  j.e.j.e.j.e.j.e.
 000000d0: 6a18 6709 5a1a 6505 6a10 6505 6a15 6505  j.g.Z.e.j.e.j.e.
 000000e0: 6a16 6505 6a1b 6505 6a1c 6505 6a17 6505  j.e.j.e.j.e.j.e.
 000000f0: 6a18 6707 5a1d 6505 6a10 6505 6a15 6505  j.g.Z.e.j.e.j.e.
 00000100: 6a16 6505 6a1b 6505 6a1c 6505 6a17 6505  j.e.j.e.j.e.j.e.
 00000110: 6a18 6707 5a1e 6505 6a10 6505 6a16 6505  j.g.Z.e.j.e.j.e.
-00000120: 6a17 6505 6a18 6704 5a1f 6505 6a20 6505  j.e.j.g.Z.e.j e.
-00000130: 6a17 6505 6a18 6703 5a21 6505 6a22 6701  j.e.j.g.Z!e.j"g.
-00000140: 5a23 6503 6a24 6509 651d 6409 9c02 6503  Z#e.j$e.e.d...e.
-00000150: 6a25 6509 651d 6409 9c02 6503 6a26 6509  j%e.e.d...e.j&e.
-00000160: 651e 6409 9c02 6503 6a27 6507 651f 6409  e.d...e.j'e.e.d.
-00000170: 9c02 6503 6a28 650f 6519 6409 9c02 6503  ..e.j(e.e.d...e.
-00000180: 6a29 650f 6519 6409 9c02 6503 6a2a 650f  j)e.e.d...e.j*e.
-00000190: 6519 6409 9c02 6503 6a2b 650f 6519 6409  e.d...e.j+e.e.d.
-000001a0: 9c02 6503 6a2c 6501 6519 6409 9c02 6503  ..e.j,e.e.d...e.
-000001b0: 6a2d 650b 651a 6409 9c02 6503 6a2e 650b  j-e.e.d...e.j.e.
-000001c0: 651a 6409 9c02 6503 6a2f 650b 651a 6409  e.d...e.j/e.e.d.
-000001d0: 9c02 6503 6a30 6509 6521 6409 9c02 6503  ..e.j0e.e!d...e.
-000001e0: 6a31 6509 6521 6409 9c02 690e 5a32 6532  j1e.e!d...i.Z2e2
-000001f0: 6503 6a24 1900 5a33 7930 6400 640a 6c34  e.j$..Z3y0d.d.l4
-00000200: 6d35 5a35 0100 650d 6523 6409 9c02 6532  m5Z5..e.e#d...e2
-00000210: 6535 6a36 3c00 650d 6523 6409 9c02 6532  e5j6<.e.e#d...e2
-00000220: 6535 6a37 3c00 5700 6e16 0400 6538 6b0a  e5j7<.W.n...e8k.
-00000230: 9002 7218 0100 0100 0100 5900 6e02 5800  ..r.......Y.n.X.
-00000240: 640b 640c 8400 5a39 640d 5300 290e e900  d.d...Z9d.S.)...
-00000250: 0000 0029 01da 0b46 6c6f 6174 4669 6c74  ...)...FloatFilt
-00000260: 6572 2901 da08 7371 6c74 7970 6573 2901  er)...sqltypes).
-00000270: da07 6c6f 6f6b 7570 7329 01da 0d42 6f6f  ..lookups)...Boo
-00000280: 6c65 616e 4669 6c74 6572 2901 da0a 4368  leanFilter)...Ch
-00000290: 6172 4669 6c74 6572 2901 da0e 4461 7465  arFilter)...Date
-000002a0: 5469 6d65 4669 6c74 6572 2901 da09 574b  TimeFilter)...WK
-000002b0: 5446 696c 7465 7229 01da 0d49 6e74 6567  TFilter)...Integ
-000002c0: 6572 4669 6c74 6572 2902 da0c 6669 6c74  erFilter)...filt
-000002d0: 6572 5f63 6c61 7373 7204 0000 0029 01da  er_classr....)..
-000002e0: 0574 7970 6573 6301 0000 0000 0000 0003  .typesc.........
-000002f0: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
-00000300: 7822 7400 6a01 8300 4400 5d16 5c02 7d01  x"t.j...D.].\.}.
-00000310: 7d02 7402 7c00 7c01 8302 720a 7c02 5300  }.t.|.|...r.|.S.
-00000320: 710a 5700 7403 5300 2901 4e29 04da 1246  q.W.t.S.).N)...F
-00000330: 494c 5445 525f 464f 525f 4442 4649 454c  ILTER_FOR_DBFIEL
-00000340: 44da 0569 7465 6d73 da0a 6973 696e 7374  D..items..isinst
-00000350: 616e 6365 da1a 4649 4c54 4552 5f46 4f52  ance..FILTER_FOR
-00000360: 5f44 4246 4945 4c44 5f44 4546 4155 4c54  _DBFIELD_DEFAULT
-00000370: 2903 da05 7661 6c75 65da 0964 6174 615f  )...value..data_
-00000380: 7479 7065 5a0b 6669 6c74 6572 5f64 6174  typeZ.filter_dat
-00000390: 61a9 0072 1200 0000 fa71 2f55 7365 7273  a..r.....q/Users
-000003a0: 2f66 316e 616c 2f44 726f 7062 6f78 2f70  /f1nal/Dropbox/p
-000003b0: 7974 686f 6e2f 6a65 742d 6272 6964 6765  ython/jet-bridge
-000003c0: 2f73 7263 2f70 6163 6b61 6765 732f 6a65  /src/packages/je
-000003d0: 745f 6272 6964 6765 5f62 6173 652f 6a65  t_bridge_base/je
-000003e0: 745f 6272 6964 6765 5f62 6173 652f 6669  t_bridge_base/fi
-000003f0: 6c74 6572 732f 6669 6c74 6572 5f66 6f72  lters/filter_for
-00000400: 5f64 6266 6965 6c64 2e70 79da 1466 696c  _dbfield.py..fil
-00000410: 7465 725f 666f 725f 6461 7461 5f74 7970  ter_for_data_typ
-00000420: 6576 0000 0073 0800 0000 0001 1201 0a01  ev...s..........
-00000430: 0801 7214 0000 004e 293a 5a24 6a65 745f  ..r....N):Z$jet_
-00000440: 6272 6964 6765 5f62 6173 652e 6669 6c74  bridge_base.filt
-00000450: 6572 732e 666c 6f61 745f 6669 6c74 6572  ers.float_filter
-00000460: 7202 0000 005a 0e73 716c 616c 6368 656d  r....Z.sqlalchem
-00000470: 792e 7371 6c72 0300 0000 da17 6a65 745f  y.sqlr......jet_
-00000480: 6272 6964 6765 5f62 6173 652e 6669 6c74  bridge_base.filt
-00000490: 6572 7372 0400 0000 5a26 6a65 745f 6272  ersr....Z&jet_br
-000004a0: 6964 6765 5f62 6173 652e 6669 6c74 6572  idge_base.filter
-000004b0: 732e 626f 6f6c 6561 6e5f 6669 6c74 6572  s.boolean_filter
-000004c0: 7205 0000 005a 236a 6574 5f62 7269 6467  r....Z#jet_bridg
-000004d0: 655f 6261 7365 2e66 696c 7465 7273 2e63  e_base.filters.c
-000004e0: 6861 725f 6669 6c74 6572 7206 0000 005a  har_filterr....Z
-000004f0: 276a 6574 5f62 7269 6467 655f 6261 7365  'jet_bridge_base
-00000500: 2e66 696c 7465 7273 2e64 6174 6574 696d  .filters.datetim
-00000510: 655f 6669 6c74 6572 7207 0000 005a 226a  e_filterr....Z"j
-00000520: 6574 5f62 7269 6467 655f 6261 7365 2e66  et_bridge_base.f
-00000530: 696c 7465 7273 2e77 6b74 5f66 696c 7465  ilters.wkt_filte
-00000540: 7272 0800 0000 5a26 6a65 745f 6272 6964  rr....Z&jet_brid
-00000550: 6765 5f62 6173 652e 6669 6c74 6572 732e  ge_base.filters.
-00000560: 696e 7465 6765 725f 6669 6c74 6572 7209  integer_filterr.
-00000570: 0000 00da 0545 5841 4354 da02 4754 da03  .....EXACT..GT..
-00000580: 4754 45da 024c 54da 034c 5445 da09 4943  GTE..LT..LTE..IC
-00000590: 4f4e 5441 494e 53da 0249 4eda 0749 535f  ONTAINS..IN..IS_
-000005a0: 4e55 4c4c da08 4953 5f45 4d50 5459 5a0e  NULL..IS_EMPTYZ.
-000005b0: 6e75 6d62 6572 5f6c 6f6f 6b75 7073 5a10  number_lookupsZ.
-000005c0: 6461 7465 7469 6d65 5f6c 6f6f 6b75 7073  datetime_lookups
-000005d0: da0b 5354 4152 5453 5f57 4954 48da 0945  ..STARTS_WITH..E
-000005e0: 4e44 535f 5749 5448 5a0c 7465 7874 5f6c  NDS_WITHZ.text_l
-000005f0: 6f6f 6b75 7073 5a0e 7365 6c65 6374 5f6c  ookupsZ.select_l
-00000600: 6f6f 6b75 7073 5a0f 626f 6f6c 6561 6e5f  ookupsZ.boolean_
-00000610: 6c6f 6f6b 7570 73da 0e4a 534f 4e5f 4943  lookups..JSON_IC
-00000620: 4f4e 5441 494e 535a 0c6a 736f 6e5f 6c6f  ONTAINSZ.json_lo
-00000630: 6f6b 7570 73da 0943 4f56 4552 4544 4259  okups..COVEREDBY
-00000640: 5a11 6765 6f67 7261 7068 795f 6c6f 6f6b  Z.geography_look
-00000650: 7570 73da 0756 4152 4348 4152 da04 5445  ups..VARCHAR..TE
-00000660: 5854 da04 456e 756d da07 426f 6f6c 6561  XT..Enum..Boolea
-00000670: 6eda 0749 6e74 6567 6572 da0c 536d 616c  n..Integer..Smal
-00000680: 6c49 6e74 6567 6572 da0a 4269 6749 6e74  lInteger..BigInt
-00000690: 6567 6572 da07 4e75 6d65 7269 63da 0546  eger..Numeric..F
-000006a0: 6c6f 6174 da04 4461 7465 da08 4461 7465  loat..Date..Date
-000006b0: 5469 6d65 da09 5449 4d45 5354 414d 50da  Time..TIMESTAMP.
-000006c0: 044a 534f 4eda 0541 5252 4159 720c 0000  .JSON..ARRAYr...
-000006d0: 0072 0f00 0000 5a0b 6765 6f61 6c63 6865  .r....Z.geoalche
-000006e0: 6d79 3272 0b00 0000 5a08 4765 6f6d 6574  my2r....Z.Geomet
-000006f0: 7279 5a09 4765 6f67 7261 7068 79da 0b49  ryZ.Geography..I
-00000700: 6d70 6f72 7445 7272 6f72 7214 0000 0072  mportErrorr....r
-00000710: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000720: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000730: 0073 8a00 0000 0c01 0c02 0c01 0c01 0c01  .s..............
-00000740: 0c01 0c01 0c03 0401 0401 0401 0401 0401  ................
-00000750: 0401 0401 0401 0804 0401 0401 0401 0401  ................
-00000760: 0401 0401 0401 0401 0804 0401 0401 0401  ................
-00000770: 0401 0401 0401 0804 0401 0401 0401 0401  ................
-00000780: 0401 0401 0804 0401 0401 0401 0804 0401  ................
-00000790: 0401 0804 0804 0c01 0c01 0c01 0c01 0c01  ................
-000007a0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000007b0: 1016 0a02 0201 0c01 1001 1401 1001 0603  ................
+00000120: 6a17 6505 6a18 6704 5a1f 6505 6a10 6505  j.e.j.g.Z.e.j.e.
+00000130: 6a16 6505 6a20 6505 6a17 6505 6a18 6705  j.e.j e.j.e.j.g.
+00000140: 5a21 6505 6a22 6701 5a23 6503 6a24 6509  Z!e.j"g.Z#e.j$e.
+00000150: 651d 6409 9c02 6503 6a25 6509 651d 6409  e.d...e.j%e.e.d.
+00000160: 9c02 6503 6a26 6509 651e 6409 9c02 6503  ..e.j&e.e.d...e.
+00000170: 6a27 6507 651f 6409 9c02 6503 6a28 650f  j'e.e.d...e.j(e.
+00000180: 6519 6409 9c02 6503 6a29 650f 6519 6409  e.d...e.j)e.e.d.
+00000190: 9c02 6503 6a2a 650f 6519 6409 9c02 6503  ..e.j*e.e.d...e.
+000001a0: 6a2b 650f 6519 6409 9c02 6503 6a2c 6501  j+e.e.d...e.j,e.
+000001b0: 6519 6409 9c02 6503 6a2d 650b 651a 6409  e.d...e.j-e.e.d.
+000001c0: 9c02 6503 6a2e 650b 651a 6409 9c02 6503  ..e.j.e.e.d...e.
+000001d0: 6a2f 650b 651a 6409 9c02 6503 6a30 6509  j/e.e.d...e.j0e.
+000001e0: 6521 6409 9c02 6503 6a31 6509 6521 6409  e!d...e.j1e.e!d.
+000001f0: 9c02 690e 5a32 6532 6503 6a24 1900 5a33  ..i.Z2e2e.j$..Z3
+00000200: 7930 6400 640a 6c34 6d35 5a35 0100 650d  y0d.d.l4m5Z5..e.
+00000210: 6523 6409 9c02 6532 6535 6a36 3c00 650d  e#d...e2e5j6<.e.
+00000220: 6523 6409 9c02 6532 6535 6a37 3c00 5700  e#d...e2e5j7<.W.
+00000230: 6e16 0400 6538 6b0a 9002 7220 0100 0100  n...e8k...r ....
+00000240: 0100 5900 6e02 5800 640b 640c 8400 5a39  ..Y.n.X.d.d...Z9
+00000250: 640d 5300 290e e900 0000 0029 01da 0b46  d.S.)......)...F
+00000260: 6c6f 6174 4669 6c74 6572 2901 da08 7371  loatFilter)...sq
+00000270: 6c74 7970 6573 2901 da07 6c6f 6f6b 7570  ltypes)...lookup
+00000280: 7329 01da 0d42 6f6f 6c65 616e 4669 6c74  s)...BooleanFilt
+00000290: 6572 2901 da0a 4368 6172 4669 6c74 6572  er)...CharFilter
+000002a0: 2901 da0e 4461 7465 5469 6d65 4669 6c74  )...DateTimeFilt
+000002b0: 6572 2901 da09 574b 5446 696c 7465 7229  er)...WKTFilter)
+000002c0: 01da 0d49 6e74 6567 6572 4669 6c74 6572  ...IntegerFilter
+000002d0: 2902 da0c 6669 6c74 6572 5f63 6c61 7373  )...filter_class
+000002e0: 7204 0000 0029 01da 0574 7970 6573 6301  r....)...typesc.
+000002f0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000300: 0000 0073 2800 0000 7822 7400 6a01 8300  ...s(...x"t.j...
+00000310: 4400 5d16 5c02 7d01 7d02 7402 7c00 7c01  D.].\.}.}.t.|.|.
+00000320: 8302 720a 7c02 5300 710a 5700 7403 5300  ..r.|.S.q.W.t.S.
+00000330: 2901 4e29 04da 1246 494c 5445 525f 464f  ).N)...FILTER_FO
+00000340: 525f 4442 4649 454c 44da 0569 7465 6d73  R_DBFIELD..items
+00000350: da0a 6973 696e 7374 616e 6365 da1a 4649  ..isinstance..FI
+00000360: 4c54 4552 5f46 4f52 5f44 4246 4945 4c44  LTER_FOR_DBFIELD
+00000370: 5f44 4546 4155 4c54 2903 da05 7661 6c75  _DEFAULT)...valu
+00000380: 65da 0964 6174 615f 7479 7065 5a0b 6669  e..data_typeZ.fi
+00000390: 6c74 6572 5f64 6174 61a9 0072 1200 0000  lter_data..r....
+000003a0: fa71 2f55 7365 7273 2f66 316e 616c 2f44  .q/Users/f1nal/D
+000003b0: 726f 7062 6f78 2f70 7974 686f 6e2f 6a65  ropbox/python/je
+000003c0: 742d 6272 6964 6765 2f73 7263 2f70 6163  t-bridge/src/pac
+000003d0: 6b61 6765 732f 6a65 745f 6272 6964 6765  kages/jet_bridge
+000003e0: 5f62 6173 652f 6a65 745f 6272 6964 6765  _base/jet_bridge
+000003f0: 5f62 6173 652f 6669 6c74 6572 732f 6669  _base/filters/fi
+00000400: 6c74 6572 5f66 6f72 5f64 6266 6965 6c64  lter_for_dbfield
+00000410: 2e70 79da 1466 696c 7465 725f 666f 725f  .py..filter_for_
+00000420: 6461 7461 5f74 7970 6578 0000 0073 0800  data_typex...s..
+00000430: 0000 0001 1201 0a01 0801 7214 0000 004e  ..........r....N
+00000440: 293a 5a24 6a65 745f 6272 6964 6765 5f62  ):Z$jet_bridge_b
+00000450: 6173 652e 6669 6c74 6572 732e 666c 6f61  ase.filters.floa
+00000460: 745f 6669 6c74 6572 7202 0000 005a 0e73  t_filterr....Z.s
+00000470: 716c 616c 6368 656d 792e 7371 6c72 0300  qlalchemy.sqlr..
+00000480: 0000 da17 6a65 745f 6272 6964 6765 5f62  ....jet_bridge_b
+00000490: 6173 652e 6669 6c74 6572 7372 0400 0000  ase.filtersr....
+000004a0: 5a26 6a65 745f 6272 6964 6765 5f62 6173  Z&jet_bridge_bas
+000004b0: 652e 6669 6c74 6572 732e 626f 6f6c 6561  e.filters.boolea
+000004c0: 6e5f 6669 6c74 6572 7205 0000 005a 236a  n_filterr....Z#j
+000004d0: 6574 5f62 7269 6467 655f 6261 7365 2e66  et_bridge_base.f
+000004e0: 696c 7465 7273 2e63 6861 725f 6669 6c74  ilters.char_filt
+000004f0: 6572 7206 0000 005a 276a 6574 5f62 7269  err....Z'jet_bri
+00000500: 6467 655f 6261 7365 2e66 696c 7465 7273  dge_base.filters
+00000510: 2e64 6174 6574 696d 655f 6669 6c74 6572  .datetime_filter
+00000520: 7207 0000 005a 226a 6574 5f62 7269 6467  r....Z"jet_bridg
+00000530: 655f 6261 7365 2e66 696c 7465 7273 2e77  e_base.filters.w
+00000540: 6b74 5f66 696c 7465 7272 0800 0000 5a26  kt_filterr....Z&
+00000550: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+00000560: 6669 6c74 6572 732e 696e 7465 6765 725f  filters.integer_
+00000570: 6669 6c74 6572 7209 0000 00da 0545 5841  filterr......EXA
+00000580: 4354 da02 4754 da03 4754 45da 024c 54da  CT..GT..GTE..LT.
+00000590: 034c 5445 da09 4943 4f4e 5441 494e 53da  .LTE..ICONTAINS.
+000005a0: 0249 4eda 0749 535f 4e55 4c4c da08 4953  .IN..IS_NULL..IS
+000005b0: 5f45 4d50 5459 5a0e 6e75 6d62 6572 5f6c  _EMPTYZ.number_l
+000005c0: 6f6f 6b75 7073 5a10 6461 7465 7469 6d65  ookupsZ.datetime
+000005d0: 5f6c 6f6f 6b75 7073 da0b 5354 4152 5453  _lookups..STARTS
+000005e0: 5f57 4954 48da 0945 4e44 535f 5749 5448  _WITH..ENDS_WITH
+000005f0: 5a0c 7465 7874 5f6c 6f6f 6b75 7073 5a0e  Z.text_lookupsZ.
+00000600: 7365 6c65 6374 5f6c 6f6f 6b75 7073 5a0f  select_lookupsZ.
+00000610: 626f 6f6c 6561 6e5f 6c6f 6f6b 7570 73da  boolean_lookups.
+00000620: 0e4a 534f 4e5f 4943 4f4e 5441 494e 535a  .JSON_ICONTAINSZ
+00000630: 0c6a 736f 6e5f 6c6f 6f6b 7570 73da 0943  .json_lookups..C
+00000640: 4f56 4552 4544 4259 5a11 6765 6f67 7261  OVEREDBYZ.geogra
+00000650: 7068 795f 6c6f 6f6b 7570 73da 0756 4152  phy_lookups..VAR
+00000660: 4348 4152 da04 5445 5854 da04 456e 756d  CHAR..TEXT..Enum
+00000670: da07 426f 6f6c 6561 6eda 0749 6e74 6567  ..Boolean..Integ
+00000680: 6572 da0c 536d 616c 6c49 6e74 6567 6572  er..SmallInteger
+00000690: da0a 4269 6749 6e74 6567 6572 da07 4e75  ..BigInteger..Nu
+000006a0: 6d65 7269 63da 0546 6c6f 6174 da04 4461  meric..Float..Da
+000006b0: 7465 da08 4461 7465 5469 6d65 da09 5449  te..DateTime..TI
+000006c0: 4d45 5354 414d 50da 044a 534f 4eda 0541  MESTAMP..JSON..A
+000006d0: 5252 4159 720c 0000 0072 0f00 0000 5a0b  RRAYr....r....Z.
+000006e0: 6765 6f61 6c63 6865 6d79 3272 0b00 0000  geoalchemy2r....
+000006f0: 5a08 4765 6f6d 6574 7279 5a09 4765 6f67  Z.GeometryZ.Geog
+00000700: 7261 7068 79da 0b49 6d70 6f72 7445 7272  raphy..ImportErr
+00000710: 6f72 7214 0000 0072 1200 0000 7212 0000  orr....r....r...
+00000720: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
+00000730: 6475 6c65 3e01 0000 0073 8e00 0000 0c01  dule>....s......
+00000740: 0c02 0c01 0c01 0c01 0c01 0c01 0c03 0401  ................
+00000750: 0401 0401 0401 0401 0401 0401 0401 0804  ................
+00000760: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000770: 0804 0401 0401 0401 0401 0401 0401 0804  ................
+00000780: 0401 0401 0401 0401 0401 0401 0804 0401  ................
+00000790: 0401 0401 0804 0401 0401 0401 0401 0804  ................
+000007a0: 0804 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000007b0: 0c01 0c01 0c01 0c01 0c01 0c01 1016 0a02  ................
+000007c0: 0201 0c01 1001 1401 1001 0603            ............
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_m2m.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_m2m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/boolean_filter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_search.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_search.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_relation.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_relation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_group.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_group.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/char_filter.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/char_filter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_segment.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_segment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/datetime_filter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_search.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_search.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_relation.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_relation.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_segment.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_segment.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/order_by.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/order_by.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_class.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter_for_dbfield.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/order_by.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/order_by.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/filter.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/filter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/model_aggregate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/__pycache__/integer_filter.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/__pycache__/integer_filter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model_aggregate.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model_aggregate.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model_m2m.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model_m2m.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/order_by.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/order_by.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model_search.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model_search.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/model_relation.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/model_relation.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/filter.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from jet_bridge_base.utils.classes import is_instance_or_subclass
 from jet_bridge_base.utils.queryset import get_session_engine
 from sqlalchemy import Unicode, and_, or_
-from sqlalchemy.dialects.postgresql import JSON, ENUM, JSONB, array
+from sqlalchemy.dialects.postgresql import ENUM, JSONB, array
 from sqlalchemy.sql import sqltypes
 from six import string_types
 
 from jet_bridge_base.fields import field, CharField, BooleanField
 from jet_bridge_base.filters import lookups
 
 EMPTY_VALUES = ([], (), {}, None)
 
 
 def safe_equals(queryset, column, value):
     field_type = column.property.columns[0].type if hasattr(column, 'property') else column.type
 
-    if is_instance_or_subclass(field_type, (JSON, sqltypes.NullType)) or not hasattr(column, 'astext'):
+    if is_instance_or_subclass(field_type, (sqltypes.JSON,)):
         if get_session_engine(queryset.session) == 'postgresql':
             return column.cast(JSONB).op('?')(value)
         else:
             return column.cast(Unicode).ilike('%{}%'.format(value))
     else:
         return column.__eq__(value)
 
 
 def safe_in(queryset, column, value):
     field_type = column.property.columns[0].type if hasattr(column, 'property') else column.type
 
-    if is_instance_or_subclass(field_type, (JSON, sqltypes.NullType)) or not hasattr(column, 'astext'):
+    if is_instance_or_subclass(field_type, (sqltypes.JSON,)):
         if get_session_engine(queryset.session) == 'postgresql':
             return column.cast(JSONB).op('?|')(array(value))
         else:
             operators = list(map(lambda x: column.cast(Unicode).ilike('%{}%'.format(x)), value))
             return or_(*operators)
     else:
         return column.in_(value)
@@ -62,15 +62,15 @@
     else:
         return column.ilike('%{}%'.format(value))
 
 
 def json_icontains(queryset, column, value):
     field_type = column.property.columns[0].type if hasattr(column, 'property') else column.type
 
-    if is_instance_or_subclass(field_type, (JSON, sqltypes.NullType)) or not hasattr(column, 'astext'):
+    if is_instance_or_subclass(field_type, (sqltypes.JSON, sqltypes.NullType)) or not hasattr(column, 'astext'):
         return column.cast(Unicode).ilike('%{}%'.format(value))
     else:
         return column.astext.ilike('%{}%'.format(value))
 
 
 def is_null(queryset, column, value):
     if value:
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/filters/filter_for_dbfield.py` & `jet-bridge-base-1.8.2/jet_bridge_base/filters/filter_for_dbfield.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/store.py` & `jet-bridge-base-1.8.2/jet_bridge_base/store.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/configuration.py` & `jet-bridge-base-1.8.2/jet_bridge_base/configuration.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/db.py` & `jet-bridge-base-1.8.2/jet_bridge_base/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import base64
 import contextlib
 import json
 import threading
 import time
 from datetime import timedelta, datetime
 
+from jet_bridge_base.automap import automap_base
 from jet_bridge_base.reflect import reflect
 from jet_bridge_base.ssh_tunnel import SSHTunnel
 from jet_bridge_base.utils.crypt import get_sha256_hash
+from jet_bridge_base.utils.process import get_memory_usage_human
 from jet_bridge_base.utils.type_codes import fetch_type_code_to_sql_type
 from six import StringIO
 from six.moves.urllib_parse import quote_plus
 
 from sqlalchemy import create_engine, MetaData
-from sqlalchemy.ext.automap import automap_base, generate_relationship
 from sqlalchemy.orm import sessionmaker, scoped_session
 
 from jet_bridge_base.utils.common import get_random_string, merge
 
 try:
     from geoalchemy2 import types
 except ImportError:
@@ -98,23 +99,26 @@
 
             if port:
                 url.append(':')
                 url.append(str(port))
 
             url.append('/')
 
-        url.append(str(conf.get('name')))
+        if conf.get('engine') != 'oracle':
+            url.append(str(conf.get('name')))
 
         if conf.get('extra'):
             url.append('?')
             url.append(str(conf.get('extra')))
         elif conf.get('engine') == 'mysql':
             url.append('?charset=utf8')
         elif conf.get('engine') == 'mssql+pyodbc':
             url.append('?driver=FreeTDS')
+        elif conf.get('engine') == 'oracle':
+            url.append('?service_name={}'.format(url_encode(conf.get('name'))))
 
     return ''.join(url)
 
 
 def get_connection_id(conf):
     return get_sha256_hash(json.dumps([
         conf.get('engine'),
@@ -122,14 +126,17 @@
         conf.get('port'),
         conf.get('name'),
         conf.get('user'),
         conf.get('password'),
         conf.get('only'),
         conf.get('except'),
         conf.get('schema'),
+        conf.get('ssl_ca'),
+        conf.get('ssl_cert'),
+        conf.get('ssl_key'),
         conf.get('ssh_host'),
         conf.get('ssh_port'),
         conf.get('ssh_user'),
         conf.get('ssh_private_key')
     ]))
 
 
@@ -269,22 +276,53 @@
     engine_url = build_engine_url(conf, tunnel)
 
     if not engine_url:
         raise Exception('Database configuration is not set')
 
     if conf.get('engine') == 'sqlite':
         return create_engine(engine_url)
+    elif conf.get('engine') == 'mysql':
+        connect_args = {}
+        ssl = {
+            'ca': conf.get('ssl_ca'),
+            'cert': conf.get('ssl_cert'),
+            'key': conf.get('ssl_key')
+        }
+        ssl_set = dict(list(filter(lambda x: x[1], ssl.items())))
+
+        if len(ssl_set):
+            connect_args['ssl'] = ssl_set
+
+        return create_engine(
+            engine_url,
+            pool_size=conf.get('connections'),
+            pool_pre_ping=True,
+            max_overflow=1,
+            pool_recycle=300,
+            connect_args={
+                'connect_timeout': 5,
+                **connect_args
+            }
+        )
     elif conf.get('engine') == 'bigquery':
         return create_engine(
             engine_url,
             pool_size=conf.get('connections'),
             pool_pre_ping=True,
             max_overflow=1,
             pool_recycle=300
         )
+    elif conf.get('engine') == 'oracle':
+        return create_engine(
+            engine_url,
+            pool_size=conf.get('connections'),
+            pool_pre_ping=True,
+            max_overflow=1,
+            pool_recycle=300
+        )
     else:
         return create_engine(
             engine_url,
             pool_size=conf.get('connections'),
             pool_pre_ping=True,
             max_overflow=1,
             pool_recycle=300,
@@ -319,14 +357,15 @@
 
     existing_connection = wait_pending_connection(connection_id, connection_name)
     if existing_connection:
         return existing_connection
 
     init_start = datetime.now()
 
+    id_short = connection_id[:4]
     connected_condition = threading.Condition()
     pending_connection_id = get_random_string(32)
     pending_connection = {
         'id': pending_connection_id,
         'name': connection_name,
         'project': conf.get('project'),
         'token': conf.get('token'),
@@ -343,43 +382,43 @@
 
         engine = create_connection_engine(conf, tunnel)
         pending_connection['engine'] = engine
 
         Session = scoped_session(sessionmaker(bind=engine))
         session = Session()
 
-        logger.info('Connecting to database "{}"...'.format(connection_name))
+        logger.info('[{}] Connecting to database "{}"...'.format(id_short, connection_name))
 
         connect_start = time.time()
         with session.connection() as connection:
             connect_end = time.time()
             connect_time = round(connect_end - connect_start, 3)
 
-            logger.info('Getting db types for "{}"...'.format(connection_name))
+            logger.info('[{}] Getting db types for "{}"...'.format(id_short, connection_name))
             type_code_to_sql_type = fetch_type_code_to_sql_type(session)
 
-            logger.info('Getting schema for "{}"...'.format(connection_name))
+            logger.info('[{}] Getting schema for "{}"...'.format(id_short, connection_name))
 
             reflect_start = time.time()
 
             metadata = MetaData(schema=schema, bind=connection)
             only = get_connection_only_predicate(conf)
-            reflect(metadata, engine, only=only, pending_connection=pending_connection)
+            reflect(id_short, metadata, engine, only=only, pending_connection=pending_connection, views=True)
 
             reflect_end = time.time()
             reflect_time = round(reflect_end - reflect_start, 3)
 
-            logger.info('Connected to "{}"'.format(connection_name))
+            logger.info('[{}] Connected to "{}" (Mem:{})'.format(id_short, connection_name, get_memory_usage_human()))
 
             MappedBase = automap_base(metadata=metadata)
             load_mapped_base(MappedBase)
 
             for table_name, table in MappedBase.metadata.tables.items():
                 if len(table.primary_key.columns) == 0 and table_name not in MappedBase.classes:
-                    logger.warning('Table "{}" does not have primary key and will be ignored'.format(table_name))
+                    logger.warning('[{}] Table "{}" does not have primary key and will be ignored'.format(id_short, table_name))
 
             connections[connection_id] = {
                 'id': connection_id,
                 'name': connection_name,
                 'engine': engine,
                 'Session': Session,
                 'MappedBase': MappedBase,
@@ -449,14 +488,17 @@
         'user': settings.DATABASE_USER,
         'password': settings.DATABASE_PASSWORD,
         'extra': settings.DATABASE_EXTRA,
         'connections': settings.DATABASE_CONNECTIONS,
         'only': settings.DATABASE_ONLY,
         'except': settings.DATABASE_EXCEPT,
         'schema': settings.DATABASE_SCHEMA,
+        'ssl_ca': settings.DATABASE_SSL_CA,
+        'ssl_cert': settings.DATABASE_SSL_CERT,
+        'ssl_key': settings.DATABASE_SSL_KEY,
         'ssh_host': settings.DATABASE_SSH_HOST,
         'ssh_port': settings.DATABASE_SSH_PORT,
         'ssh_user': settings.DATABASE_SSH_USER,
         'ssh_private_key': settings.DATABASE_SSH_PRIVATE_KEY,
         'project': settings.PROJECT,
         'token': settings.TOKEN
     }
@@ -472,18 +514,21 @@
         'engine': bridge_settings.get('database_engine'),
         'host': bridge_settings.get('database_host'),
         'port': bridge_settings.get('database_port'),
         'name': bridge_settings.get('database_name'),
         'user': bridge_settings.get('database_user'),
         'password': bridge_settings.get('database_password'),
         'extra': bridge_settings.get('database_extra'),
-        'connections': bridge_settings.get('database_connections', 50),
+        'connections': bridge_settings.get('database_connections', settings.DATABASE_CONNECTIONS),
         'only': bridge_settings.get('database_only'),
         'except': bridge_settings.get('database_except'),
         'schema': bridge_settings.get('database_schema'),
+        'ssl_ca': bridge_settings.get('database_ssl_ca'),
+        'ssl_cert': bridge_settings.get('database_ssl_cert'),
+        'ssl_key': bridge_settings.get('database_ssl_key'),
         'ssh_host': bridge_settings.get('database_ssh_host'),
         'ssh_port': bridge_settings.get('database_ssh_port'),
         'ssh_user': bridge_settings.get('database_ssh_user'),
         'ssh_private_key': bridge_settings.get('database_ssh_private_key'),
         'project': bridge_settings.get('project'),
         'token': bridge_settings.get('token'),
     }
@@ -517,14 +562,21 @@
 def create_session(request):
     connection = get_request_connection(request)
     if not connection:
         return
     return connection['Session']()
 
 
+def get_connection_id_short(request):
+    connection = get_request_connection(request)
+    if not connection or 'id' not in connection:
+        return
+    return connection['id'][:4]
+
+
 def get_mapped_base(request):
     connection = get_request_connection(request)
     if not connection:
         return
     return connection['MappedBase']
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/settings.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/settings.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/paginators/page_number.py` & `jet-bridge-base-1.8.2/jet_bridge_base/paginators/page_number.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/page_number.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/page_number.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/pagination.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/pagination.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/page_number.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/page_number.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/paginators/__pycache__/pagination.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/paginators/__pycache__/pagination.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/redirect.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/redirect.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/base.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/not_found.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/not_found.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/template.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/template.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/redirect.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/redirect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/template.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/template.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/base.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/base.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/json.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/json.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/__pycache__/json.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/__pycache__/json.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/responses/base.py` & `jet-bridge-base-1.8.2/jet_bridge_base/responses/base.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/request.py` & `jet-bridge-base-1.8.2/jet_bridge_base/request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import json
+import os
+import tempfile
 from json import JSONDecodeError
 
 from jet_bridge_base.exceptions.request_error import RequestError
 from jet_bridge_base.exceptions.validation_error import ValidationError
+from jet_bridge_base.utils.crypt import get_sha256_hash
 from six import string_types
 
 from jet_bridge_base import settings
 from jet_bridge_base.exceptions.missing_argument_error import MissingArgumentError
 
 _ARG_DEFAULT = object()
 
@@ -151,12 +154,45 @@
             return
 
         from jet_bridge_base.utils.crypt import decrypt
 
         try:
             secret_key = settings.TOKEN.replace('-', '').lower()
             decrypted = decrypt(bridge_settings_encoded, secret_key)
-            self.bridge_settings = json.loads(decrypted)
-            return self.bridge_settings
+
+            self.bridge_settings = {
+                **json.loads(decrypted),
+                'raw': bridge_settings_encoded
+            }
         except Exception:
             return
 
+        database_ssl_ca = self.bridge_settings.get('database_ssl_ca')
+        database_ssl_cert = self.bridge_settings.get('database_ssl_cert')
+        database_ssl_key = self.bridge_settings.get('database_ssl_key')
+
+        temp_dir = os.path.join(tempfile.gettempdir(), 'ssl')
+
+        try:
+            os.makedirs(temp_dir)
+        except OSError:
+            pass
+
+        if database_ssl_ca:
+            self.bridge_settings['database_ssl_ca'] = self.save_file(temp_dir, '{}-ca.pem', database_ssl_ca)
+
+        if database_ssl_cert:
+            self.bridge_settings['database_ssl_cert'] = self.save_file(temp_dir, '{}-cert.pem', database_ssl_cert)
+
+        if database_ssl_key:
+            self.bridge_settings['database_ssl_key'] = self.save_file(temp_dir, '{}-key.pem', database_ssl_key)
+
+        return self.bridge_settings
+
+    def save_file(self, dir_path, name, content):
+        file_hash = get_sha256_hash(content)
+        file_path = os.path.join(dir_path, name.format(file_hash))
+
+        with open(file_path, 'w') as f:
+            f.write(content)
+
+        return f.name
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/mixin.py` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/mixin.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/strategy.py` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/strategy.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/storage.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/storage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/mixin.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/mixin.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/strategy.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/strategy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/pipeline.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/pipeline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/mixin.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/mixin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/utils.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/__pycache__/utils.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/utils.py` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/utils.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/external_auth/pipeline.py` & `jet-bridge-base-1.8.2/jet_bridge_base/external_auth/pipeline.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/encoders.py` & `jet-bridge-base-1.8.2/jet_bridge_base/encoders.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/crypt.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/async_exec.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/async_exec.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/graphql.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/graphql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 import graphene
-from jet_bridge_base.models.model_relation_override import ModelRelationOverrideModel
-from jet_bridge_base.store import store
-from jet_bridge_base.utils.relations import parse_relationship_direction
 from sqlalchemy import inspect, desc, MetaData
 from sqlalchemy.engine import Row
-from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import MANYTOONE, ONETOMANY, aliased
 
+from jet_bridge_base.automap import automap_base
 from jet_bridge_base.db import get_mapped_base, get_engine, load_mapped_base, get_request_connection, get_table_name
 from jet_bridge_base.filters import lookups
 from jet_bridge_base.filters.filter_for_dbfield import filter_for_data_type
 from jet_bridge_base.filters.model_group import get_query_func_by_name
 from jet_bridge_base.filters.model_search import search_queryset
+from jet_bridge_base.models.model_relation_override import ModelRelationOverrideModel
 from jet_bridge_base.serializers.model import get_model_serializer
+from jet_bridge_base.store import store
 from jet_bridge_base.utils.common import get_set_first, any_type_sorter, unique, flatten
 from jet_bridge_base.utils.gql import RawScalar
 from jet_bridge_base.utils.queryset import queryset_count_optimized, apply_default_ordering, get_session_engine
+from jet_bridge_base.utils.relations import parse_relationship_direction
 
 
 class ModelFiltersType(graphene.InputObjectType):
     pass
 
 
 class ModelFiltersFieldType(graphene.InputObjectType):
@@ -109,31 +109,34 @@
         self.model_lookups_types = dict()
         self.model_lookups_field_types = dict()
         self.model_lookups_relationship_types = dict()
         self.model_sort_types = dict()
 
     def get_queryset(self, request, Model, only_columns=None):
         mapper = inspect(Model)
-        pk = mapper.primary_key[0]
+        pks = mapper.primary_key
 
         if only_columns:
-            if not any(map(lambda x: x.name == pk.name, only_columns)):
-                only_columns = [pk, *only_columns]
+            only_columns_name = list(map(lambda x: x.name, only_columns))
+            missing_pks = list(filter(lambda x: x.name not in only_columns_name, pks))
+
+            if len(missing_pks):
+                only_columns = [*missing_pks, *only_columns]
 
             queryset = request.session.query(*only_columns)
         else:
             queryset = request.session.query(Model)
 
         mapper = inspect(Model)
         auto_pk = getattr(mapper.tables[0], '__jet_auto_pk__', False) if len(mapper.tables) else None
         if auto_pk:
             queryset = queryset.filter(mapper.primary_key[0].isnot(None))
 
         if not auto_pk and get_session_engine(request.session) in ['postgresql', 'mysql']:
-            queryset = queryset.group_by(pk)
+            queryset = queryset.group_by(*pks)
 
         return queryset
 
     def get_relationships(self, request, MappedBase, draft):
         result = {}
         relationships_overrides = {}
 
@@ -151,15 +154,15 @@
                         relationships_overrides[override.model] = []
                     relationships_overrides[override.model].append(override)
 
         for Model in MappedBase.classes:
             model_relationships = {}
 
             mapper = inspect(Model)
-            name = mapper.selectable.name
+            name = get_table_name(MappedBase.metadata, mapper.selectable)
 
             model_relationships_overrides = relationships_overrides.get(name, [])
 
             for override in model_relationships_overrides:
                 direction = parse_relationship_direction(override.direction)
                 local_column = getattr(Model, override.local_field, None)
 
@@ -251,24 +254,24 @@
 
     def get_model_columns_by_clean_name(self, MappedBase, mapper):
         table = mapper.tables[0]
         name = get_table_name(MappedBase.metadata, table)
         Model = MappedBase.classes.get(name)
         return dict(map(lambda x: (clean_name(x), getattr(Model, x)), mapper.columns.keys()))
 
-    def get_model_relationships(self, mapper):
-        name = mapper.selectable.name
+    def get_model_relationships(self, MappedBase, mapper):
+        name = get_table_name(MappedBase.metadata, mapper.selectable)
         return self.relationships_by_name.get(name, {}).values()
 
-    def get_model_relationships_by_name(self, mapper):
-        name = mapper.selectable.name
+    def get_model_relationships_by_name(self, MappedBase, mapper):
+        name = get_table_name(MappedBase.metadata, mapper.selectable)
         return self.relationships_by_name.get(name, {})
 
-    def get_model_relationships_by_clean_name(self, mapper):
-        name = mapper.selectable.name
+    def get_model_relationships_by_clean_name(self, MappedBase, mapper):
+        name = get_table_name(MappedBase.metadata, mapper.selectable)
         return self.relationships_by_clean_name.get(name, {})
 
     def filter_queryset(self, MappedBase, queryset, mapper, filters, parent_relations=None, exclude=False):
         parent_relations = parent_relations or []
 
         for filters_item in filters:
             filters_item_dict = dict(filters_item)
@@ -283,15 +286,15 @@
                         parent_relations,
                         exclude=True
                     )
                     continue
 
                 columns_by_clean_name = self.get_model_columns_by_clean_name(MappedBase, mapper)
                 column = columns_by_clean_name.get(filter_name)
-                filter_relationship = self.get_model_relationships_by_clean_name(mapper).get(filter_name)
+                filter_relationship = self.get_model_relationships_by_clean_name(MappedBase, mapper).get(filter_name)
 
                 if filter_relationship is not None:
                     filter_lookups_dict = dict(filter_lookups)
 
                     for lookup_name, lookup_value in filter_lookups_dict.items():
                         if lookup_name == 'relation':
                             relation_mapper = filter_relationship['related_mapper']
@@ -304,15 +307,15 @@
                                 exclude
                             )
                 elif column is not None:
                     filter_lookups_dict = dict(filter_lookups)
 
                     for lookup_name, lookup_value in filter_lookups_dict.items():
                         if lookup_name == 'relation':
-                            for relationship in self.get_model_relationships(mapper):
+                            for relationship in self.get_model_relationships(MappedBase, mapper):
                                 if relationship['direction'] != MANYTOONE or relationship['local_column_name'] != column.name:
                                     continue
 
                                 relation_mapper = relationship['related_mapper']
                                 queryset = self.filter_queryset(
                                     MappedBase,
                                     queryset,
@@ -380,15 +383,15 @@
         result = {}
 
         lookup_item_dict = dict(lookup_item)
 
         for lookup_name, lookup_data in lookup_item_dict.items():
             columns_by_clean_name = self.get_model_columns_by_clean_name(MappedBase, mapper)
             column = columns_by_clean_name.get(lookup_name)
-            relationship = self.get_model_relationships_by_clean_name(mapper).get(lookup_name)
+            relationship = self.get_model_relationships_by_clean_name(MappedBase, mapper).get(lookup_name)
 
             if relationship is not None:
                 lookup_result = {}
                 local_column = relationship['local_column']
                 lookup_values = sorted(unique(flatten(map(lambda x: getattr(x, local_column.name), models))), key=any_type_sorter)
 
                 lookup_result['return'] = lookup_data.get('return', False)
@@ -454,15 +457,15 @@
                 lookup_result['return_list'] = lookup_data.get('returnList', False)
                 lookup_result['Model'] = Model
                 lookup_result['mapper'] = mapper
                 lookup_result['model_values'] = list(map(lambda x: {'instance': x, 'value': getattr(x, column.name)}, models))
                 lookup_result['source_column'] = column.name
 
                 if 'relation' in lookup_data:
-                    for relationship in self.get_model_relationships(mapper):
+                    for relationship in self.get_model_relationships(MappedBase, mapper):
                         if relationship['direction'] != MANYTOONE or relationship['local_column_name'] != column.name:
                             continue
 
                         relation_mapper = relationship['related_mapper']
                         relation_model = relationship['related_model']
                         relation_column = relationship['related_column']
 
@@ -567,45 +570,47 @@
 
         queryset = queryset.limit(limit)
 
         return queryset
 
     def get_model_filters_type(self, MappedBase, mapper, depth=1):
         with_relations = depth <= 4
-        model_name = clean_name(mapper.selectable.name)
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         cls_name = 'Model{}Depth{}NestedFiltersType'.format(model_name, depth) if with_relations \
             else 'Model{}Depth{}FiltersType'.format(model_name, depth)
 
         if cls_name in self.model_filters_types:
             return graphene.List(self.model_filters_types[cls_name])
 
         attrs = {}
 
         for column in mapper.columns:
             column_filters_type = self.get_model_field_filters_type(MappedBase, mapper, column, with_relations, depth)
             attr_name = clean_name(column.name)
             attrs[attr_name] = column_filters_type()
 
         if with_relations:
-            for relationship in self.get_model_relationships(mapper):
+            for relationship in self.get_model_relationships(MappedBase, mapper):
                 if relationship['direction'] != ONETOMANY:
                     continue
 
                 relationship_filters_type = self.get_model_relationship_filters_type(MappedBase, mapper, relationship, with_relations, depth)
                 attr_name = clean_name(relationship['name'])
                 attrs[attr_name] = relationship_filters_type()
 
             attrs['_not_'] = self.get_model_filters_type(MappedBase, mapper, depth + 1)
 
         cls = type(cls_name, (ModelFiltersType,), attrs)
         self.model_filters_types[cls_name] = cls
         return graphene.List(cls)
 
     def get_model_field_filters_type(self, MappedBase, mapper, column, with_relations, depth=1):
-        model_name = clean_name(mapper.selectable.name)
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         column_name = clean_name(column.name)
         cls_name = 'Model{}Column{}Depth{}NestedFiltersType'.format(model_name, column_name, depth) if with_relations \
             else 'Model{}Column{}Depth{}FiltersType'.format(model_name, column_name, depth)
 
         if cls_name in self.model_filters_field_types:
             return self.model_filters_field_types[cls_name]
 
@@ -614,29 +619,30 @@
 
         for lookup in item['lookups']:
             gql_lookup = lookups.gql.get(lookup)
             gql_scalar = lookups.gql_scalar.get(lookup, RawScalar())
             attrs[gql_lookup] = gql_scalar
 
         if with_relations:
-            for relationship in self.get_model_relationships(mapper):
+            for relationship in self.get_model_relationships(MappedBase, mapper):
                 if relationship['direction'] != MANYTOONE or relationship['local_column_name'] != column_name:
                     continue
 
                 relation_mapper = relationship['related_mapper']
                 column_filters_type = self.get_model_filters_type(MappedBase, relation_mapper, depth + 1)
                 attrs['relation'] = column_filters_type
                 break
 
         cls = type(cls_name, (ModelFiltersFieldType,), attrs)
         self.model_filters_field_types[cls_name] = cls
         return cls
 
     def get_model_relationship_filters_type(self, MappedBase, mapper, relationship, with_relations, depth=1):
-        model_name = clean_name(mapper.selectable.name)
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         relationship_key = clean_name(relationship['name'])
         cls_name = 'Model{}Column{}Depth{}NestedRelationshipType'.format(model_name, relationship_key, depth) if with_relations \
             else 'Model{}Column{}Depth{}RelationshipType'.format(model_name, relationship_key, depth)
 
         if cls_name in self.model_filters_relationship_types:
             return self.model_filters_relationship_types[cls_name]
 
@@ -647,71 +653,74 @@
 
         cls = type(cls_name, (ModelFiltersRelationshipType,), attrs)
         self.model_filters_relationship_types[cls_name] = cls
         return cls
 
     def get_model_lookups_type(self, MappedBase, mapper, depth=1):
         with_relations = depth <= 4
-        model_name = clean_name(mapper.selectable.name)
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         cls_name = 'Model{}Depth{}NestedLookupsType'.format(model_name, depth) if with_relations \
             else 'Model{}Depth{}LookupsType'.format(model_name, depth)
 
         if cls_name in self.model_lookups_types:
             return self.model_lookups_types[cls_name]
 
         attrs = {}
 
         for column in mapper.columns:
             column_lookups_type = self.get_model_field_lookups_type(MappedBase, mapper, column, with_relations, depth)
             attr_name = clean_name(column.name)
             attrs[attr_name] = column_lookups_type()
 
         if with_relations:
-            for relationship in self.get_model_relationships(mapper):
+            for relationship in self.get_model_relationships(MappedBase, mapper):
                 if relationship['direction'] != ONETOMANY:
                     continue
 
                 relationship_lookups_type = self.get_model_relationship_lookups_type(MappedBase, mapper, relationship, with_relations, depth)
                 attr_name = clean_name(relationship['name'])
                 attrs[attr_name] = relationship_lookups_type()
 
         cls = type(cls_name, (ModelLookupsType,), attrs)
         self.model_lookups_types[cls_name] = cls
         return cls
 
     def get_model_field_lookups_type(self, MappedBase, mapper, column, with_relations, depth=1):
-        model_name = clean_name(mapper.selectable.name)
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         column_name = clean_name(column.name)
         cls_name = 'Model{}Column{}Depth{}NestedLookupsFieldType'.format(model_name, column_name, depth) if with_relations \
             else 'Model{}Column{}Depth{}LookupsFieldType'.format(model_name, column_name, depth)
 
         if cls_name in self.model_lookups_field_types:
             return self.model_lookups_field_types[cls_name]
 
         attrs = {
             'return': graphene.Boolean(),
             'returnList': graphene.Boolean()
         }
 
         if with_relations:
-            for relationship in self.get_model_relationships(mapper):
+            for relationship in self.get_model_relationships(MappedBase, mapper):
                 if relationship['direction'] != MANYTOONE or relationship['local_column_name'] != column_name:
                     continue
 
                 relation_mapper = relationship['related_mapper']
                 lookups_type = self.get_model_lookups_type(MappedBase, relation_mapper, depth + 1)
                 attrs['relation'] = lookups_type()
                 break
 
         cls = type(cls_name, (ModelLookupsFieldType,), attrs)
         self.model_lookups_field_types[cls_name] = cls
         return cls
 
     def get_model_relationship_lookups_type(self, MappedBase, mapper, relationship, with_relations, depth=1):
-        model_name = clean_name(mapper.selectable.name)
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         relationship_key = clean_name(relationship['name'])
         cls_name = 'Model{}Column{}Depth{}NestedLookupsRelationshipType'.format(model_name, relationship_key, depth) if with_relations \
             else 'Model{}Column{}Depth{}LookupsRelationshipType'.format(model_name, relationship_key, depth)
 
         if cls_name in self.model_lookups_relationship_types:
             return self.model_lookups_relationship_types[cls_name]
 
@@ -722,16 +731,17 @@
         lookups_type = self.get_model_lookups_type(MappedBase, relationship['related_mapper'], depth + 1)
         attrs['relation'] = lookups_type()
 
         cls = type(cls_name, (ModelLookupsRelationshipType,), attrs)
         self.model_lookups_relationship_types[cls_name] = cls
         return cls
 
-    def get_model_sort_type(self, mapper):
-        model_name = clean_name(mapper.selectable.name)
+    def get_model_sort_type(self, MappedBase, mapper):
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        model_name = clean_name(table_name)
         cls_name = 'Model{}SortType'.format(model_name)
 
         if cls_name in self.model_sort_types:
             return graphene.List(self.model_sort_types[cls_name])
 
         attrs = {}
 
@@ -739,16 +749,17 @@
             attr_name = clean_name(column.name)
             attrs[attr_name] = FieldSortType()
 
         cls = type(cls_name, (ModelSortType,), attrs)
         self.model_sort_types[cls_name] = cls
         return graphene.List(cls)
 
-    def get_model_attrs_type(self, mapper):
-        name = clean_name(mapper.selectable.name)
+    def get_model_attrs_type(self, MappedBase, mapper):
+        table_name = get_table_name(MappedBase.metadata, mapper.selectable)
+        name = clean_name(table_name)
         attrs = {}
 
         for column in mapper.columns:
             attr_name = clean_name(column.name)
             attrs[attr_name] = RawScalar()
 
         return type('Model{}RecordAttrsType'.format(name), (ModelAttrsType,), attrs)
@@ -844,35 +855,41 @@
                     elif page is not None:
                         result['pagination']['hasMore'] = page * limit < count
 
             return result
         except Exception as e:
             raise e
 
-    def get_query_type(self, request, draft, before_resolve=None):
+    def get_query_type(self, request, draft, before_resolve=None, on_progress_updated=None):
         MappedBase = get_mapped_base(request)
 
         if len(MappedBase.classes) == 0:
             raise Exception('No tables found')
 
         query_attrs = {}
 
         self.relationships_by_name = self.get_relationships(request, MappedBase, draft)
         self.relationships_by_clean_name = self.clean_relationships_by_name(self.relationships_by_name)
 
+        i = 0
+        total = len(MappedBase.classes)
+
         for Model in MappedBase.classes:
             mapper = inspect(Model)
             table = mapper.tables[0]
             name = get_table_name(MappedBase.metadata, table)
             name = clean_name(name)
 
+            if on_progress_updated:
+                on_progress_updated(name, i, total)
+
             FiltersType = self.get_model_filters_type(MappedBase, mapper)
             LookupsType = self.get_model_lookups_type(MappedBase, mapper)
-            SortType = self.get_model_sort_type(mapper)
-            ModelAttrsType = self.get_model_attrs_type(mapper)
+            SortType = self.get_model_sort_type(MappedBase, mapper)
+            ModelAttrsType = self.get_model_attrs_type(MappedBase, mapper)
             ModelType = type('Model{}ModelType'.format(name), (graphene.ObjectType,), {
                 'attrs': graphene.Field(ModelAttrsType),
                 'allAttrs': graphene.Field(RawScalar),
                 'lookups': graphene.List(RawScalar)
             })
             ModelListType = type('Model{}ModelListType'.format(name), (graphene.ObjectType,), {
                 'data': graphene.List(ModelType),
@@ -905,12 +922,17 @@
                 lookups=graphene.List(LookupsType),
                 sort=SortType,
                 pagination=PaginationType(),
                 search=SearchType()
             )
             query_attrs['resolve_{}'.format(name)] = create_list_resolver(Model, mapper)
 
+            i += 1
+
+        if on_progress_updated:
+            on_progress_updated(None, total, total)
+
         return type('Query', (graphene.ObjectType,), query_attrs)
 
-    def get_schema(self, request, draft, before_resolve=None):
-        Query = self.get_query_type(request, draft, before_resolve)
+    def get_schema(self, request, draft, before_resolve=None, on_progress_updated=None):
+        Query = self.get_query_type(request, draft, before_resolve, on_progress_updated)
         return graphene.Schema(query=Query, auto_camelcase=False)
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/backend.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/backend.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/db_types.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/db_types.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/async_exec.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/async_exec.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/exceptions.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/exceptions.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/graphql.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/graphql.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-00000000: 330d 0d0a 09ac 0164 9795 0000 e300 0000  3......d........
+00000000: 330d 0d0a 5f1e c264 9d9a 0000 e300 0000  3..._..d........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 2402 0000 6400 6401 6c00 5a00 6400  .s$...d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
-00000070: 6406 6c0c 6d0d 5a0d 0100 6400 6407 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 0100 6400 6408 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
-00000090: 6d12 5a12 6d13 5a13 0100 6400 6409 6c14  m.Z.m.Z...d.d.l.
-000000a0: 6d15 5a15 6d16 5a16 6d17 5a17 6d18 5a18  m.Z.m.Z.m.Z.m.Z.
+00000040: 6d04 5a04 6d05 5a05 0100 6400 6403 6c06  m.Z.m.Z...d.d.l.
+00000050: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000060: 6d0a 5a0a 6d0b 5a0b 0100 6400 6405 6c0c  m.Z.m.Z...d.d.l.
+00000070: 6d0d 5a0d 0100 6400 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000080: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
+00000090: 0100 6400 6407 6c14 6d15 5a15 0100 6400  ..d.d.l.m.Z...d.
+000000a0: 6408 6c16 6d17 5a17 0100 6400 6409 6c18  d.l.m.Z...d.d.l.
 000000b0: 6d19 5a19 0100 6400 640a 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
 000000c0: 0100 6400 640b 6c1c 6d1d 5a1d 0100 6400  ..d.d.l.m.Z...d.
 000000d0: 640c 6c1e 6d1f 5a1f 0100 6400 640d 6c20  d.l.m.Z...d.d.l 
 000000e0: 6d21 5a21 0100 6400 640e 6c22 6d23 5a23  m!Z!..d.d.l"m#Z#
-000000f0: 0100 6400 640f 6c24 6d25 5a25 6d26 5a26  ..d.d.l$m%Z%m&Z&
-00000100: 6d27 5a27 6d28 5a28 0100 6400 6410 6c29  m'Z'm(Z(..d.d.l)
-00000110: 6d2a 5a2a 0100 6400 6411 6c2b 6d2c 5a2c  m*Z*..d.d.l+m,Z,
-00000120: 6d2d 5a2d 6d2e 5a2e 0100 4700 6412 6413  m-Z-m.Z...G.d.d.
+000000f0: 6d24 5a24 6d25 5a25 6d26 5a26 0100 6400  m$Z$m%Z%m&Z&..d.
+00000100: 640f 6c27 6d28 5a28 0100 6400 6410 6c29  d.l'm(Z(..d.d.l)
+00000110: 6d2a 5a2a 6d2b 5a2b 6d2c 5a2c 0100 6400  m*Z*m+Z+m,Z,..d.
+00000120: 6411 6c2d 6d2e 5a2e 0100 4700 6412 6413  d.l-m.Z...G.d.d.
 00000130: 8400 6413 6501 6a2f 8303 5a30 4700 6414  ..d.e.j/..Z0G.d.
 00000140: 6415 8400 6415 6501 6a2f 8303 5a31 4700  d...d.e.j/..Z1G.
 00000150: 6416 6417 8400 6417 6501 6a2f 8303 5a32  d.d...d.e.j/..Z2
 00000160: 4700 6418 6419 8400 6419 6501 6a2f 8303  G.d.d...d.e.j/..
 00000170: 5a33 4700 641a 641b 8400 641b 6501 6a2f  Z3G.d.d...d.e.j/
 00000180: 8303 5a34 4700 641c 641d 8400 641d 6501  ..Z4G.d.d...d.e.
 00000190: 6a2f 8303 5a35 4700 641e 641f 8400 641f  j/..Z5G.d.d...d.
@@ -31,45 +31,45 @@
 000001e0: 6426 6427 8400 6427 6501 6a2f 8303 5a3b  d&d'..d'e.j/..Z;
 000001f0: 4700 6428 6429 8400 6429 6501 6a3c 8303  G.d(d)..d)e.j<..
 00000200: 5a3d 4700 642a 642b 8400 642b 6501 6a2f  Z=G.d*d+..d+e.j/
 00000210: 8303 5a3e 4700 642c 642d 8400 642d 6501  ..Z>G.d,d-..d-e.
 00000220: 6a37 8303 5a3f 642e 642f 8400 5a40 6430  j7..Z?d.d/..Z@d0
 00000230: 6431 8400 5a41 4700 6432 6433 8400 6433  d1..ZAG.d2d3..d3
 00000240: 6542 8303 5a43 6401 5300 2934 e900 0000  eB..ZCd.S.)4....
-00000250: 004e 2901 da1a 4d6f 6465 6c52 656c 6174  .N)...ModelRelat
-00000260: 696f 6e4f 7665 7272 6964 654d 6f64 656c  ionOverrideModel
-00000270: 2901 da05 7374 6f72 6529 01da 1c70 6172  )...store)...par
-00000280: 7365 5f72 656c 6174 696f 6e73 6869 705f  se_relationship_
-00000290: 6469 7265 6374 696f 6e29 03da 0769 6e73  direction)...ins
-000002a0: 7065 6374 da04 6465 7363 da08 4d65 7461  pect..desc..Meta
-000002b0: 4461 7461 2901 da03 526f 7729 01da 0c61  Data)...Row)...a
-000002c0: 7574 6f6d 6170 5f62 6173 6529 03da 094d  utomap_base)...M
-000002d0: 414e 5954 4f4f 4e45 da09 4f4e 4554 4f4d  ANYTOONE..ONETOM
-000002e0: 414e 59da 0761 6c69 6173 6564 2905 da0f  ANY..aliased)...
-000002f0: 6765 745f 6d61 7070 6564 5f62 6173 65da  get_mapped_base.
-00000300: 0a67 6574 5f65 6e67 696e 65da 106c 6f61  .get_engine..loa
-00000310: 645f 6d61 7070 6564 5f62 6173 65da 1667  d_mapped_base..g
-00000320: 6574 5f72 6571 7565 7374 5f63 6f6e 6e65  et_request_conne
-00000330: 6374 696f 6eda 0e67 6574 5f74 6162 6c65  ction..get_table
-00000340: 5f6e 616d 6529 01da 076c 6f6f 6b75 7073  _name)...lookups
-00000350: 2901 da14 6669 6c74 6572 5f66 6f72 5f64  )...filter_for_d
-00000360: 6174 615f 7479 7065 2901 da16 6765 745f  ata_type)...get_
-00000370: 7175 6572 795f 6675 6e63 5f62 795f 6e61  query_func_by_na
-00000380: 6d65 2901 da0f 7365 6172 6368 5f71 7565  me)...search_que
-00000390: 7279 7365 7429 01da 1467 6574 5f6d 6f64  ryset)...get_mod
-000003a0: 656c 5f73 6572 6961 6c69 7a65 7229 04da  el_serializer)..
-000003b0: 0d67 6574 5f73 6574 5f66 6972 7374 da0f  .get_set_first..
-000003c0: 616e 795f 7479 7065 5f73 6f72 7465 72da  any_type_sorter.
-000003d0: 0675 6e69 7175 65da 0766 6c61 7474 656e  .unique..flatten
-000003e0: 2901 da09 5261 7753 6361 6c61 7229 03da  )...RawScalar)..
-000003f0: 1871 7565 7279 7365 745f 636f 756e 745f  .queryset_count_
-00000400: 6f70 7469 6d69 7a65 64da 1661 7070 6c79  optimized..apply
-00000410: 5f64 6566 6175 6c74 5f6f 7264 6572 696e  _default_orderin
-00000420: 67da 1267 6574 5f73 6573 7369 6f6e 5f65  g..get_session_e
-00000430: 6e67 696e 6563 0000 0000 0000 0000 0000  nginec..........
+00000250: 004e 2903 da07 696e 7370 6563 74da 0464  .N)...inspect..d
+00000260: 6573 63da 084d 6574 6144 6174 6129 01da  esc..MetaData)..
+00000270: 0352 6f77 2903 da09 4d41 4e59 544f 4f4e  .Row)...MANYTOON
+00000280: 45da 094f 4e45 544f 4d41 4e59 da07 616c  E..ONETOMANY..al
+00000290: 6961 7365 6429 01da 0c61 7574 6f6d 6170  iased)...automap
+000002a0: 5f62 6173 6529 05da 0f67 6574 5f6d 6170  _base)...get_map
+000002b0: 7065 645f 6261 7365 da0a 6765 745f 656e  ped_base..get_en
+000002c0: 6769 6e65 da10 6c6f 6164 5f6d 6170 7065  gine..load_mappe
+000002d0: 645f 6261 7365 da16 6765 745f 7265 7175  d_base..get_requ
+000002e0: 6573 745f 636f 6e6e 6563 7469 6f6e da0e  est_connection..
+000002f0: 6765 745f 7461 626c 655f 6e61 6d65 2901  get_table_name).
+00000300: da07 6c6f 6f6b 7570 7329 01da 1466 696c  ..lookups)...fil
+00000310: 7465 725f 666f 725f 6461 7461 5f74 7970  ter_for_data_typ
+00000320: 6529 01da 1667 6574 5f71 7565 7279 5f66  e)...get_query_f
+00000330: 756e 635f 6279 5f6e 616d 6529 01da 0f73  unc_by_name)...s
+00000340: 6561 7263 685f 7175 6572 7973 6574 2901  earch_queryset).
+00000350: da1a 4d6f 6465 6c52 656c 6174 696f 6e4f  ..ModelRelationO
+00000360: 7665 7272 6964 654d 6f64 656c 2901 da14  verrideModel)...
+00000370: 6765 745f 6d6f 6465 6c5f 7365 7269 616c  get_model_serial
+00000380: 697a 6572 2901 da05 7374 6f72 6529 04da  izer)...store)..
+00000390: 0d67 6574 5f73 6574 5f66 6972 7374 da0f  .get_set_first..
+000003a0: 616e 795f 7479 7065 5f73 6f72 7465 72da  any_type_sorter.
+000003b0: 0675 6e69 7175 65da 0766 6c61 7474 656e  .unique..flatten
+000003c0: 2901 da09 5261 7753 6361 6c61 7229 03da  )...RawScalar)..
+000003d0: 1871 7565 7279 7365 745f 636f 756e 745f  .queryset_count_
+000003e0: 6f70 7469 6d69 7a65 64da 1661 7070 6c79  optimized..apply
+000003f0: 5f64 6566 6175 6c74 5f6f 7264 6572 696e  _default_orderin
+00000400: 67da 1267 6574 5f73 6573 7369 6f6e 5f65  g..get_session_e
+00000410: 6e67 696e 6529 01da 1c70 6172 7365 5f72  ngine)...parse_r
+00000420: 656c 6174 696f 6e73 6869 705f 6469 7265  elationship_dire
+00000430: 6374 696f 6e63 0000 0000 0000 0000 0000  ctionc..........
 00000440: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
 00000450: 005a 0164 005a 0264 0153 0029 02da 104d  .Z.d.Z.d.S.)...M
 00000460: 6f64 656c 4669 6c74 6572 7354 7970 654e  odelFiltersTypeN
 00000470: 2903 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000480: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000490: 6e61 6d65 5f5f a900 7223 0000 0072 2300  name__..r#...r#.
 000004a0: 0000 fa64 2f55 7365 7273 2f66 316e 616c  ...d/Users/f1nal
@@ -273,1348 +273,1382 @@
 00001100: 6f64 656c 5f73 6f72 745f 7479 7065 7329  odel_sort_types)
 00001110: 01da 0473 656c 6672 2300 0000 7223 0000  ...selfr#...r#..
 00001120: 0072 2400 0000 da08 5f5f 696e 6974 5f5f  .r$.....__init__
 00001130: 6700 0000 7312 0000 0000 0108 0108 0108  g...s...........
 00001140: 0108 0108 0108 0108 0108 017a 1f47 7261  ...........z.Gra
 00001150: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
 00001160: 746f 722e 5f5f 696e 6974 5f5f 4e63 0400  tor.__init__Nc..
-00001170: 0000 0000 0000 0700 0000 0500 0000 0300  ................
-00001180: 0000 73b4 0000 0074 007c 0283 017d 047c  ..s....t.|...}.|
-00001190: 046a 0164 0119 0089 007c 0372 4474 0274  .j.d.....|.rDt.t
-000011a0: 0387 0066 0164 0264 0384 087c 0383 0283  ...f.d.d...|....
-000011b0: 0173 3688 0066 017c 0395 027d 037c 016a  .s6..f.|...}.|.j
-000011c0: 046a 057c 038e 007d 056e 0c7c 016a 046a  .j.|...}.n.|.j.j
-000011d0: 057c 0283 017d 0574 007c 0283 017d 0474  .|...}.t.|...}.t
-000011e0: 067c 046a 0783 0172 7474 087c 046a 0764  .|.j...rtt.|.j.d
-000011f0: 0119 0064 0464 0583 036e 0264 007d 067c  ...d.d...n.d.}.|
-00001200: 0672 927c 056a 097c 046a 0164 0119 006a  .r.|.j.|.j.d...j
-00001210: 0a64 0083 0183 017d 057c 060c 0072 b074  .d.....}.|...r.t
-00001220: 0b7c 016a 0483 0164 086b 0672 b07c 056a  .|.j...d.k.r.|.j
-00001230: 0c88 0083 017d 057c 0553 0029 094e 7201  .....}.|.S.).Nr.
-00001240: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
-00001250: 0200 0000 1300 0000 730c 0000 007c 006a  ........s....|.j
-00001260: 0088 006a 006b 0253 0029 014e 2901 7248  ...j.k.S.).N).rH
-00001270: 0000 0029 0172 4b00 0000 2901 da02 706b  ...).rK...)...pk
-00001280: 7223 0000 0072 2400 0000 724c 0000 0077  r#...r$...rL...w
-00001290: 0000 0073 0000 0000 7a35 4772 6170 6851  ...s....z5GraphQ
-000012a0: 4c53 6368 656d 6147 656e 6572 6174 6f72  LSchemaGenerator
-000012b0: 2e67 6574 5f71 7565 7279 7365 742e 3c6c  .get_queryset.<l
-000012c0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3eda  ocals>.<lambda>.
-000012d0: 0f5f 5f6a 6574 5f61 7574 6f5f 706b 5f5f  .__jet_auto_pk__
-000012e0: 46da 0a70 6f73 7467 7265 7371 6cda 056d  F..postgresql..m
-000012f0: 7973 716c 2902 7261 0000 0072 6200 0000  ysql).ra...rb...
-00001300: 290d 7205 0000 00da 0b70 7269 6d61 7279  ).r......primary
-00001310: 5f6b 6579 da03 616e 7972 4d00 0000 da07  _key..anyrM.....
-00001320: 7365 7373 696f 6e72 3800 0000 da03 6c65  sessionr8.....le
-00001330: 6eda 0674 6162 6c65 73da 0767 6574 6174  n..tables..getat
-00001340: 7472 da06 6669 6c74 6572 da05 6973 6e6f  tr..filter..isno
-00001350: 7472 1e00 0000 da08 6772 6f75 705f 6279  tr......group_by
-00001360: 2907 725d 0000 00da 0772 6571 7565 7374  ).r].....request
-00001370: da05 4d6f 6465 6cda 0c6f 6e6c 795f 636f  ..Model..only_co
-00001380: 6c75 6d6e 73da 066d 6170 7065 72da 0871  lumns..mapper..q
-00001390: 7565 7279 7365 745a 0761 7574 6f5f 706b  uerysetZ.auto_pk
-000013a0: 7223 0000 0029 0172 5f00 0000 7224 0000  r#...).r_...r$..
-000013b0: 00da 0c67 6574 5f71 7565 7279 7365 7472  ...get_querysetr
-000013c0: 0000 0073 1c00 0000 0001 0801 0a02 0401  ...s............
-000013d0: 1601 0a02 0e02 0c02 0801 2001 0401 1602  .......... .....
-000013e0: 1401 0a02 7a23 4772 6170 6851 4c53 6368  ....z#GraphQLSch
-000013f0: 656d 6147 656e 6572 6174 6f72 2e67 6574  emaGenerator.get
-00001400: 5f71 7565 7279 7365 7463 0400 0000 0000  _querysetc......
-00001410: 0000 1d00 0000 1200 0000 4300 0000 73d0  ..........C...s.
-00001420: 0200 0069 007d 0469 007d 0574 006a 0183  ...i.}.i.}.t.j..
-00001430: 0072 8274 027c 0183 017d 0674 006a 0383  .r.t.|...}.t.j..
-00001440: 008f 5c7d 077c 076a 0474 0583 016a 0674  ..\}.|.j.t...j.t
-00001450: 056a 077c 0664 0119 006b 027c 037c 036b  .j.|.d...k.|.|.k
-00001460: 0283 026a 0883 007d 0878 307c 0844 005d  ...j...}.x0|.D.]
-00001470: 287d 097c 096a 097c 056b 0772 6467 007c  (}.|.j.|.k.rdg.|
-00001480: 057c 096a 093c 007c 057c 096a 0919 006a  .|.j.<.|.|.j...j
-00001490: 0a7c 0983 0101 0071 4c57 0057 0064 0051  .|.....qLW.W.d.Q
-000014a0: 0052 0058 0090 0278 467c 026a 0b44 0090  .R.X...xF|.j.D..
-000014b0: 025d 3a7d 0a69 007d 0b74 0c7c 0a83 017d  .]:}.i.}.t.|...}
-000014c0: 0c7c 0c6a 0d6a 0e7d 0d7c 056a 0f7c 0d67  .|.j.j.}.|.j.|.g
-000014d0: 0083 027d 0e78 f87c 0e44 005d f07d 0974  ...}.x.|.D.].}.t
-000014e0: 107c 096a 1183 017d 0f74 127c 0a7c 096a  .|.j...}.t.|.|.j
-000014f0: 1364 0083 037d 107c 1064 006b 0872 de71  .d...}.|.d.k.r.q
-00001500: b87c 096a 147d 117c 026a 0b6a 0f7c 1183  .|.j.}.|.j.j.|..
-00001510: 017d 127c 120c 006f fc64 027c 116b 0690  .}.|...o.d.|.k..
-00001520: 0172 5c7c 116a 1564 0264 0383 025c 027d  .r\|.j.d.d...\.}
-00001530: 137d 1474 167c 0183 017d 157c 026a 176a  .}.t.|...}.|.j.j
-00001540: 187d 1674 197c 137c 1664 048d 027d 177c  .}.t.|.|.d...}.|
-00001550: 176a 1a7c 157c 137c 1467 0164 058d 0301  .j.|.|.|.g.d....
-00001560: 0074 1b7c 1764 068d 017d 1874 1c7c 1883  .t.|.d...}.t.|..
-00001570: 0101 007c 186a 0b6a 0f7c 1483 017d 127c  ...|.j.j.|...}.|
-00001580: 1290 0173 6471 b874 0c7c 1283 017d 1974  ...sdq.t.|...}.t
-00001590: 127c 127c 096a 1d64 0083 037d 1a7c 1a64  .|.|.j.d...}.|.d
-000015a0: 006b 0890 0172 8671 b87c 096a 0e7c 0f7c  .k...r.q.|.j.|.|
-000015b0: 107c 096a 137c 127c 197c 1a7c 096a 1d64  .|.j.|.|.|.|.j.d
-000015c0: 079c 087c 0b7c 096a 0e3c 0071 b857 0090  ...|.|.j.<.q.W..
-000015d0: 0178 107c 0c6a 1e6a 1f83 0044 0090 015d  .x.|.j.j...D...]
-000015e0: 007d 1b74 207c 1b6a 2183 017d 1074 207c  .}.t |.j!..}.t |
-000015f0: 1b6a 2283 017d 1c7c 1b6a 1174 236b 0290  .j"..}.|.j.t#k..
-00001600: 0272 487c 1b6a 246a 2564 0819 007d 1474  .rH|.j$j%d...}.t
-00001610: 267c 026a 177c 1483 027d 117c 026a 0b6a  &|.j.|...}.|.j.j
-00001620: 0f7c 1183 017d 127c 1b6a 277c 1b6a 117c  .|...}.|.j'|.j.|
-00001630: 107c 1064 006b 0990 0272 1e7c 106a 0e6e  .|.d.k...r.|.j.n
-00001640: 0264 007c 127c 1b6a 247c 1c7c 1c64 006b  .d.|.|.j$|.|.d.k
-00001650: 0990 0272 387c 1c6a 0e6e 0264 0064 079c  ...r8|.j.n.d.d..
-00001660: 087c 0b7c 1b6a 273c 006e 727c 1b6a 1174  .|.|.j'<.nr|.j.t
-00001670: 286b 0290 0172 ba7c 1b6a 246a 2564 0819  (k...r.|.j$j%d..
-00001680: 007d 1474 267c 026a 177c 1483 027d 117c  .}.t&|.j.|...}.|
-00001690: 026a 0b6a 0f7c 1183 017d 127c 1b6a 277c  .j.j.|...}.|.j'|
-000016a0: 1b6a 117c 107c 1064 006b 0990 0272 927c  .j.|.|.d.k...r.|
-000016b0: 106a 0e6e 0264 007c 127c 1b6a 247c 1c7c  .j.n.d.|.|.j$|.|
-000016c0: 1c64 006b 0990 0272 ac7c 1c6a 0e6e 0264  .d.k...r.|.j.n.d
-000016d0: 0064 079c 087c 0b7c 1b6a 273c 0090 0171  .d...|.|.j'<...q
-000016e0: ba57 007c 0b7c 047c 0d3c 0071 8c57 007c  .W.|.|.|.<.q.W.|
-000016f0: 0453 0029 094e da02 6964 da01 2e72 4a00  .S.).N..id...rJ.
-00001700: 0000 2902 da06 7363 6865 6d61 da04 6269  ..)...schema..bi
-00001710: 6e64 2903 7275 0000 0072 7400 0000 da04  nd).ru...rt.....
-00001720: 6f6e 6c79 2901 da08 6d65 7461 6461 7461  only)...metadata
-00001730: 2908 7248 0000 00da 0964 6972 6563 7469  ).rH.....directi
-00001740: 6f6e da0c 6c6f 6361 6c5f 636f 6c75 6d6e  on..local_column
-00001750: da11 6c6f 6361 6c5f 636f 6c75 6d6e 5f6e  ..local_column_n
-00001760: 616d 65da 0d72 656c 6174 6564 5f6d 6f64  ame..related_mod
-00001770: 656c da0e 7265 6c61 7465 645f 6d61 7070  el..related_mapp
-00001780: 6572 da0e 7265 6c61 7465 645f 636f 6c75  er..related_colu
-00001790: 6d6e 5a13 7265 6c61 7465 645f 636f 6c75  mnZ.related_colu
-000017a0: 6d6e 5f6e 616d 6572 0100 0000 2929 7203  mn_namer....))r.
-000017b0: 0000 00da 0569 735f 6f6b 7210 0000 0072  .....is_okr....r
-000017c0: 6500 0000 7238 0000 0072 0200 0000 7269  e...r8...r....ri
-000017d0: 0000 00da 0d63 6f6e 6e65 6374 696f 6e5f  .....connection_
-000017e0: 6964 da03 616c 6cda 056d 6f64 656c da06  id..all..model..
-000017f0: 6170 7065 6e64 da07 636c 6173 7365 7372  append..classesr
-00001800: 0500 0000 da0a 7365 6c65 6374 6162 6c65  ......selectable
-00001810: 7248 0000 00da 0367 6574 7204 0000 0072  rH.....getr....r
-00001820: 7800 0000 7268 0000 00da 0b6c 6f63 616c  x...rh.....local
-00001830: 5f66 6965 6c64 727b 0000 00da 0573 706c  _fieldr{.....spl
-00001840: 6974 720e 0000 0072 7700 0000 7275 0000  itr....rw...ru..
-00001850: 0072 0700 0000 da07 7265 666c 6563 7472  .r......reflectr
-00001860: 0900 0000 720f 0000 00da 0d72 656c 6174  ....r......relat
-00001870: 6564 5f66 6965 6c64 da0d 7265 6c61 7469  ed_field..relati
-00001880: 6f6e 7368 6970 73da 0676 616c 7565 7372  onships..valuesr
-00001890: 1700 0000 da0d 6c6f 6361 6c5f 636f 6c75  ......local_colu
-000018a0: 6d6e 73da 0b72 656d 6f74 655f 7369 6465  mns..remote_side
-000018b0: 720a 0000 0072 6f00 0000 7267 0000 0072  r....ro...rg...r
-000018c0: 1100 0000 da03 6b65 7972 0b00 0000 291d  ......keyr....).
-000018d0: 725d 0000 0072 6c00 0000 da0a 4d61 7070  r]...rl.....Mapp
-000018e0: 6564 4261 7365 da05 6472 6166 74da 0672  edBase..draft..r
-000018f0: 6573 756c 745a 1772 656c 6174 696f 6e73  esultZ.relations
-00001900: 6869 7073 5f6f 7665 7272 6964 6573 da0a  hips_overrides..
-00001910: 636f 6e6e 6563 7469 6f6e 7265 0000 005a  connectionre...Z
-00001920: 096f 7665 7272 6964 6573 da08 6f76 6572  .overrides..over
-00001930: 7269 6465 726d 0000 005a 136d 6f64 656c  riderm...Z.model
-00001940: 5f72 656c 6174 696f 6e73 6869 7073 726f  _relationshipsro
-00001950: 0000 0072 4800 0000 5a1d 6d6f 6465 6c5f  ...rH...Z.model_
-00001960: 7265 6c61 7469 6f6e 7368 6970 735f 6f76  relationships_ov
-00001970: 6572 7269 6465 7372 7800 0000 7279 0000  erridesrx...ry..
-00001980: 005a 0c72 656c 6174 6564 5f6e 616d 6572  .Z.related_namer
-00001990: 7b00 0000 7274 0000 00da 0574 6162 6c65  {...rt.....table
-000019a0: da06 656e 6769 6e65 7275 0000 005a 1072  ..engineru...Z.r
-000019b0: 656c 6174 6564 5f6d 6574 6164 6174 615a  elated_metadataZ
-000019c0: 0c72 656c 6174 6564 5f62 6173 6572 7c00  .related_baser|.
-000019d0: 0000 727d 0000 00da 0c72 656c 6174 696f  ..r}.....relatio
-000019e0: 6e73 6869 70da 0f72 656c 6174 696f 6e5f  nship..relation_
-000019f0: 636f 6c75 6d6e 7223 0000 0072 2300 0000  columnr#...r#...
-00001a00: 7224 0000 00da 1167 6574 5f72 656c 6174  r$.....get_relat
-00001a10: 696f 6e73 6869 7073 8800 0000 7398 0000  ionships....s...
-00001a20: 0000 0104 0104 0208 0108 020a 010a 010c  ................
-00001a30: 010e 030a 010a 010a 011e 0210 0104 0208  ................
-00001a40: 0108 020c 020a 010a 010e 0208 0102 0206  ................
-00001a50: 010c 0210 0110 0108 0108 020c 0112 010a  ................
-00001a60: 0108 020c 0206 0102 0208 010e 020a 0102  ................
-00001a70: 0304 0102 0102 0104 0102 0102 0102 0114  ................
-00001a80: 0314 010a 010a 020c 010c 010c 010c 0304  ................
-00001a90: 0104 0102 0112 0102 0104 0102 0120 020c  ............. ..
-00001aa0: 010c 010c 010c 0304 0104 0102 0112 0102  ................
-00001ab0: 0104 0102 0124 030c 027a 2847 7261 7068  .....$...z(Graph
-00001ac0: 514c 5363 6865 6d61 4765 6e65 7261 746f  QLSchemaGenerato
-00001ad0: 722e 6765 745f 7265 6c61 7469 6f6e 7368  r.get_relationsh
-00001ae0: 6970 7363 0200 0000 0000 0000 0200 0000  ipsc............
-00001af0: 0500 0000 0300 0000 732e 0000 0064 0164  ........s....d.d
-00001b00: 0284 0089 0087 0066 0164 0364 0484 0889  .......f.d.d....
-00001b10: 0174 0074 0187 0166 0164 0564 0684 087c  .t.t...f.d.d...|
-00001b20: 016a 0283 0083 0283 0153 0029 074e 6301  .j.......S.).Nc.
-00001b30: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
-00001b40: 0000 0073 1400 0000 7400 7c00 6401 1900  ...s....t.|.d...
-00001b50: 8301 7c00 6402 1900 6602 5300 2903 4e72  ..|.d...f.S.).Nr
-00001b60: 0100 0000 724a 0000 0029 0172 4900 0000  ....rJ...).rI...
-00001b70: 2901 724b 0000 0072 2300 0000 7223 0000  ).rK...r#...r#..
-00001b80: 0072 2400 0000 da13 6d61 705f 6d6f 6465  .r$.....map_mode
-00001b90: 6c5f 7265 6c61 7469 6f6e 73f4 0000 0073  l_relations....s
-00001ba0: 0200 0000 0001 7a4f 4772 6170 6851 4c53  ......zOGraphQLS
-00001bb0: 6368 656d 6147 656e 6572 6174 6f72 2e63  chemaGenerator.c
-00001bc0: 6c65 616e 5f72 656c 6174 696f 6e73 6869  lean_relationshi
-00001bd0: 7073 5f62 795f 6e61 6d65 2e3c 6c6f 6361  ps_by_name.<loca
-00001be0: 6c73 3e2e 6d61 705f 6d6f 6465 6c5f 7265  ls>.map_model_re
-00001bf0: 6c61 7469 6f6e 7363 0100 0000 0000 0000  lationsc........
-00001c00: 0100 0000 0600 0000 1300 0000 7326 0000  ............s&..
-00001c10: 007c 0064 0119 0074 0074 0187 0066 0164  .|.d...t.t...f.d
-00001c20: 0264 0384 087c 0064 0419 006a 0283 0083  .d...|.d...j....
-00001c30: 0283 0166 0253 0029 054e 7201 0000 0063  ...f.S.).Nr....c
-00001c40: 0100 0000 0000 0000 0100 0000 0200 0000  ................
-00001c50: 1300 0000 7308 0000 0088 007c 0083 0153  ....s......|...S
-00001c60: 0029 014e 7223 0000 0029 01da 0172 2901  .).Nr#...)...r).
-00001c70: 7299 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
-00001c80: 4c00 0000 f800 0000 7300 0000 007a 5847  L.......s....zXG
-00001c90: 7261 7068 514c 5363 6865 6d61 4765 6e65  raphQLSchemaGene
-00001ca0: 7261 746f 722e 636c 6561 6e5f 7265 6c61  rator.clean_rela
-00001cb0: 7469 6f6e 7368 6970 735f 6279 5f6e 616d  tionships_by_nam
-00001cc0: 652e 3c6c 6f63 616c 733e 2e6d 6170 5f6d  e.<locals>.map_m
-00001cd0: 6f64 656c 732e 3c6c 6f63 616c 733e 2e3c  odels.<locals>.<
-00001ce0: 6c61 6d62 6461 3e72 4a00 0000 2903 724f  lambda>rJ...).rO
-00001cf0: 0000 0072 4d00 0000 724e 0000 0029 0172  ...rM...rN...).r
-00001d00: 4b00 0000 2901 7299 0000 0072 2300 0000  K...).r....r#...
-00001d10: 7224 0000 00da 0a6d 6170 5f6d 6f64 656c  r$.....map_model
-00001d20: 73f7 0000 0073 0200 0000 0001 7a46 4772  s....s......zFGr
-00001d30: 6170 6851 4c53 6368 656d 6147 656e 6572  aphQLSchemaGener
-00001d40: 6174 6f72 2e63 6c65 616e 5f72 656c 6174  ator.clean_relat
-00001d50: 696f 6e73 6869 7073 5f62 795f 6e61 6d65  ionships_by_name
-00001d60: 2e3c 6c6f 6361 6c73 3e2e 6d61 705f 6d6f  .<locals>.map_mo
-00001d70: 6465 6c73 6301 0000 0000 0000 0001 0000  delsc...........
-00001d80: 0002 0000 0013 0000 0073 0800 0000 8800  .........s......
-00001d90: 7c00 8301 5300 2901 4e72 2300 0000 2901  |...S.).Nr#...).
-00001da0: 724b 0000 0029 0172 9b00 0000 7223 0000  rK...).r....r#..
-00001db0: 0072 2400 0000 724c 0000 00fa 0000 0073  .r$...rL.......s
-00001dc0: 0000 0000 7a44 4772 6170 6851 4c53 6368  ....zDGraphQLSch
-00001dd0: 656d 6147 656e 6572 6174 6f72 2e63 6c65  emaGenerator.cle
-00001de0: 616e 5f72 656c 6174 696f 6e73 6869 7073  an_relationships
-00001df0: 5f62 795f 6e61 6d65 2e3c 6c6f 6361 6c73  _by_name.<locals
-00001e00: 3e2e 3c6c 616d 6264 613e 2903 724f 0000  >.<lambda>).rO..
-00001e10: 0072 4d00 0000 724e 0000 0029 0272 5d00  .rM...rN...).r].
-00001e20: 0000 728a 0000 0072 2300 0000 2902 7299  ..r....r#...).r.
-00001e30: 0000 0072 9b00 0000 7224 0000 00da 1b63  ...r....r$.....c
-00001e40: 6c65 616e 5f72 656c 6174 696f 6e73 6869  lean_relationshi
-00001e50: 7073 5f62 795f 6e61 6d65 f300 0000 7306  ps_by_name....s.
-00001e60: 0000 0000 0108 030c 037a 3247 7261 7068  .........z2Graph
-00001e70: 514c 5363 6865 6d61 4765 6e65 7261 746f  QLSchemaGenerato
-00001e80: 722e 636c 6561 6e5f 7265 6c61 7469 6f6e  r.clean_relation
-00001e90: 7368 6970 735f 6279 5f6e 616d 6563 0300  ships_by_namec..
-00001ea0: 0000 0000 0000 0500 0000 0500 0000 0300  ................
-00001eb0: 0000 733e 0000 007c 026a 0064 0119 007d  ..s>...|.j.d...}
-00001ec0: 0374 017c 016a 027c 0383 027d 047c 016a  .t.|.j.|...}.|.j
-00001ed0: 036a 047c 0483 0189 0074 0574 0687 0066  .j.|.....t.t...f
-00001ee0: 0164 0264 0384 087c 026a 076a 0883 0083  .d.d...|.j.j....
-00001ef0: 0283 0153 0029 044e 7201 0000 0063 0100  ...S.).Nr....c..
-00001f00: 0000 0000 0000 0100 0000 0400 0000 1300  ................
-00001f10: 0000 7312 0000 0074 007c 0083 0174 0188  ..s....t.|...t..
-00001f20: 007c 0083 0266 0253 0029 014e 2902 7249  .|...f.S.).N).rI
-00001f30: 0000 0072 6800 0000 2901 724b 0000 0029  ...rh...).rK...)
-00001f40: 0172 6d00 0000 7223 0000 0072 2400 0000  .rm...r#...r$...
-00001f50: 724c 0000 0000 0100 0073 0000 0000 7a48  rL.......s....zH
-00001f60: 4772 6170 6851 4c53 6368 656d 6147 656e  GraphQLSchemaGen
-00001f70: 6572 6174 6f72 2e67 6574 5f6d 6f64 656c  erator.get_model
-00001f80: 5f63 6f6c 756d 6e73 5f62 795f 636c 6561  _columns_by_clea
-00001f90: 6e5f 6e61 6d65 2e3c 6c6f 6361 6c73 3e2e  n_name.<locals>.
-00001fa0: 3c6c 616d 6264 613e 2909 7267 0000 0072  <lambda>).rg...r
-00001fb0: 1100 0000 7277 0000 0072 8300 0000 7285  ....rw...r....r.
-00001fc0: 0000 0072 4f00 0000 724d 0000 00da 0763  ...rO...rM.....c
-00001fd0: 6f6c 756d 6e73 da04 6b65 7973 2905 725d  olumns..keys).r]
-00001fe0: 0000 0072 8f00 0000 726f 0000 0072 9400  ...r....ro...r..
-00001ff0: 0000 7248 0000 0072 2300 0000 2901 726d  ..rH...r#...).rm
-00002000: 0000 0072 2400 0000 da1f 6765 745f 6d6f  ...r$.....get_mo
-00002010: 6465 6c5f 636f 6c75 6d6e 735f 6279 5f63  del_columns_by_c
-00002020: 6c65 616e 5f6e 616d 65fc 0000 0073 0800  lean_name....s..
-00002030: 0000 0001 0a01 0c01 0c01 7a36 4772 6170  ..........z6Grap
-00002040: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
-00002050: 6f72 2e67 6574 5f6d 6f64 656c 5f63 6f6c  or.get_model_col
-00002060: 756d 6e73 5f62 795f 636c 6561 6e5f 6e61  umns_by_clean_na
-00002070: 6d65 6302 0000 0000 0000 0003 0000 0003  mec.............
-00002080: 0000 0043 0000 0073 1a00 0000 7c01 6a00  ...C...s....|.j.
-00002090: 6a01 7d02 7c00 6a02 6a03 7c02 6900 8302  j.}.|.j.j.|.i...
-000020a0: 6a04 8300 5300 2901 4e29 0572 8400 0000  j...S.).N).r....
-000020b0: 7248 0000 0072 5400 0000 7285 0000 0072  rH...rT...r....r
-000020c0: 8b00 0000 2903 725d 0000 0072 6f00 0000  ....).r]...ro...
-000020d0: 7248 0000 0072 2300 0000 7223 0000 0072  rH...r#...r#...r
-000020e0: 2400 0000 da17 6765 745f 6d6f 6465 6c5f  $.....get_model_
-000020f0: 7265 6c61 7469 6f6e 7368 6970 7302 0100  relationships...
-00002100: 0073 0400 0000 0001 0801 7a2e 4772 6170  .s........z.Grap
-00002110: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
-00002120: 6f72 2e67 6574 5f6d 6f64 656c 5f72 656c  or.get_model_rel
-00002130: 6174 696f 6e73 6869 7073 6302 0000 0000  ationshipsc.....
-00002140: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00002150: 1600 0000 7c01 6a00 6a01 7d02 7c00 6a02  ....|.j.j.}.|.j.
-00002160: 6a03 7c02 6900 8302 5300 2901 4e29 0472  j.|.i...S.).N).r
-00002170: 8400 0000 7248 0000 0072 5400 0000 7285  ....rH...rT...r.
-00002180: 0000 0029 0372 5d00 0000 726f 0000 0072  ...).r]...ro...r
-00002190: 4800 0000 7223 0000 0072 2300 0000 7224  H...r#...r#...r$
-000021a0: 0000 00da 1f67 6574 5f6d 6f64 656c 5f72  .....get_model_r
-000021b0: 656c 6174 696f 6e73 6869 7073 5f62 795f  elationships_by_
-000021c0: 6e61 6d65 0601 0000 7304 0000 0000 0108  name....s.......
-000021d0: 017a 3647 7261 7068 514c 5363 6865 6d61  .z6GraphQLSchema
-000021e0: 4765 6e65 7261 746f 722e 6765 745f 6d6f  Generator.get_mo
-000021f0: 6465 6c5f 7265 6c61 7469 6f6e 7368 6970  del_relationship
-00002200: 735f 6279 5f6e 616d 6563 0200 0000 0000  s_by_namec......
-00002210: 0000 0300 0000 0300 0000 4300 0000 7316  ..........C...s.
-00002220: 0000 007c 016a 006a 017d 027c 006a 026a  ...|.j.j.}.|.j.j
-00002230: 037c 0269 0083 0253 0029 014e 2904 7284  .|.i...S.).N).r.
-00002240: 0000 0072 4800 0000 7255 0000 0072 8500  ...rH...rU...r..
-00002250: 0000 2903 725d 0000 0072 6f00 0000 7248  ..).r]...ro...rH
-00002260: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00002270: 0000 da25 6765 745f 6d6f 6465 6c5f 7265  ...%get_model_re
-00002280: 6c61 7469 6f6e 7368 6970 735f 6279 5f63  lationships_by_c
-00002290: 6c65 616e 5f6e 616d 650a 0100 0073 0400  lean_name....s..
-000022a0: 0000 0001 0801 7a3c 4772 6170 6851 4c53  ......z<GraphQLS
-000022b0: 6368 656d 6147 656e 6572 6174 6f72 2e67  chemaGenerator.g
-000022c0: 6574 5f6d 6f64 656c 5f72 656c 6174 696f  et_model_relatio
-000022d0: 6e73 6869 7073 5f62 795f 636c 6561 6e5f  nships_by_clean_
-000022e0: 6e61 6d65 4663 0700 0000 0000 0000 1b00  nameFc..........
-000022f0: 0000 0b00 0000 4300 0000 7332 0200 007c  ......C...s2...|
-00002300: 0570 0667 007d 0590 0278 227c 0444 0090  .p.g.}...x"|.D..
-00002310: 025d 187d 0774 007c 0783 017d 0890 0278  .].}.t.|...}...x
-00002320: 087c 086a 0183 0044 0090 015d fa5c 027d  .|.j...D...].\.}
-00002330: 097d 0a7c 0964 016b 0272 547c 006a 027c  .}.|.d.k.rT|.j.|
-00002340: 017c 027c 037c 0a7c 0564 0264 038d 067d  .|.|.|.|.d.d...}
-00002350: 0271 2a7c 006a 037c 017c 0383 027d 0b7c  .q*|.j.|.|...}.|
-00002360: 0b6a 047c 0983 017d 0c7c 006a 057c 0383  .j.|...}.|.j.|..
-00002370: 016a 047c 0983 017d 0d7c 0d64 006b 0972  .j.|...}.|.d.k.r
-00002380: cc74 007c 0a83 017d 0e78 3e7c 0e6a 0183  .t.|...}.x>|.j..
-00002390: 0044 005d 325c 027d 0f7d 107c 0f64 046b  .D.]2\.}.}.|.d.k
-000023a0: 0272 947c 0d64 0519 007d 117c 006a 027c  .r.|.d...}.|.j.|
-000023b0: 017c 027c 117c 107c 057c 0d66 0195 027c  .|.|.|.|.|.f...|
-000023c0: 0683 067d 0271 9457 0071 2a7c 0c64 006b  ...}.q.W.q*|.d.k
-000023d0: 0972 2a74 007c 0a83 017d 0e90 0178 467c  .r*t.|...}...xF|
-000023e0: 0e6a 0183 0044 0090 015d 385c 027d 0f7d  .j...D...]8\.}.}
-000023f0: 107c 0f64 046b 0290 0172 5a78 5a7c 006a  .|.d.k...rZxZ|.j
-00002400: 067c 0383 0144 005d 4c7d 127c 1264 0619  .|...D.]L}.|.d..
-00002410: 0074 076b 0390 0173 087c 1264 0719 007c  .t.k...s.|.d...|
-00002420: 0c6a 086b 0390 0172 2e90 0171 087c 1264  .j.k...r...q.|.d
-00002430: 0519 007d 117c 006a 027c 017c 027c 117c  ...}.|.j.|.|.|.|
-00002440: 107c 057c 1266 0195 027c 0683 067d 0250  .|.|.f...|...}.P
-00002450: 0090 0171 0857 0071 e874 097c 0583 0190  ...q.W.q.t.|....
-00002460: 0172 d264 007d 1378 5c7c 0544 005d 547d  .r.d.}.x\|.D.]T}
-00002470: 1274 0a7c 1264 0819 0083 017d 1474 0b7c  .t.|.d.....}.t.|
-00002480: 147c 1264 0919 006a 0883 027d 157c 1390  .|.d...j...}.|..
-00002490: 0172 a474 0b7c 137c 1264 0a19 006a 0883  .r.t.|.|.d...j..
-000024a0: 026e 067c 1264 0a19 007d 167c 026a 0c7c  .n.|.d...}.|.j.|
-000024b0: 147c 157c 166b 0283 027d 027c 147d 1390  .|.|.k...}.|.}..
-000024c0: 0171 6e57 0074 0b7c 137c 0c6a 0883 027d  .qnW.t.|.|.j...}
-000024d0: 0c74 0d7c 0c6a 0e83 017d 1774 0f6a 106a  .t.|.j...}.t.j.j
-000024e0: 047c 0f83 017d 187c 1764 0b19 007c 0c6a  .|...}.|.d...|.j
-000024f0: 117c 0c7c 1864 0c64 0d8d 047d 197c 196a  .|.|.d.d...}.|.j
-00002500: 127c 1083 017d 1a7c 0690 0272 147c 1a0f  .|...}.|...r.|..
-00002510: 006e 027c 1a7d 1a7c 026a 137c 1a83 017d  .n.|.}.|.j.|...}
-00002520: 0271 e857 0071 2a57 0071 1057 007c 0253  .q.W.q*W.q.W.|.S
-00002530: 0029 0e4e da05 5f6e 6f74 5f54 2901 da07  .).N.._not_T)...
-00002540: 6578 636c 7564 65da 0872 656c 6174 696f  exclude..relatio
-00002550: 6e72 7c00 0000 7278 0000 0072 7a00 0000  nr|...rx...rz...
-00002560: 727b 0000 0072 7d00 0000 7279 0000 005a  r{...r}...ry...Z
-00002570: 0c66 696c 7465 725f 636c 6173 7346 2904  .filter_classF).
-00002580: 7248 0000 00da 0663 6f6c 756d 6eda 066c  rH.....column..l
-00002590: 6f6f 6b75 7072 a400 0000 2914 724f 0000  ookupr....).rO..
-000025a0: 0072 4e00 0000 da0f 6669 6c74 6572 5f71  .rN.....filter_q
-000025b0: 7565 7279 7365 7472 9f00 0000 7285 0000  uerysetr....r...
-000025c0: 0072 a200 0000 72a0 0000 0072 0a00 0000  .r....r....r....
-000025d0: 7248 0000 0072 6600 0000 720c 0000 0072  rH...rf...r....r
-000025e0: 6800 0000 da04 6a6f 696e 7213 0000 00da  h.....joinr.....
-000025f0: 0474 7970 6572 1200 0000 5a06 6279 5f67  .typer....Z.by_g
-00002600: 716c 728e 0000 005a 1567 6574 5f6c 6f6f  qlr....Z.get_loo
-00002610: 6f6b 7570 5f63 7269 7465 7269 6f6e 7269  okup_criterionri
-00002620: 0000 0029 1b72 5d00 0000 728f 0000 0072  ...).r]...r....r
-00002630: 7000 0000 726f 0000 00da 0766 696c 7465  p...ro.....filte
-00002640: 7273 5a10 7061 7265 6e74 5f72 656c 6174  rsZ.parent_relat
-00002650: 696f 6e73 72a4 0000 005a 0c66 696c 7465  ionsr....Z.filte
-00002660: 7273 5f69 7465 6d5a 1166 696c 7465 7273  rs_itemZ.filters
-00002670: 5f69 7465 6d5f 6469 6374 5a0b 6669 6c74  _item_dictZ.filt
-00002680: 6572 5f6e 616d 655a 0e66 696c 7465 725f  er_nameZ.filter_
-00002690: 6c6f 6f6b 7570 73da 1563 6f6c 756d 6e73  lookups..columns
-000026a0: 5f62 795f 636c 6561 6e5f 6e61 6d65 72a6  _by_clean_namer.
-000026b0: 0000 005a 1366 696c 7465 725f 7265 6c61  ...Z.filter_rela
-000026c0: 7469 6f6e 7368 6970 5a13 6669 6c74 6572  tionshipZ.filter
-000026d0: 5f6c 6f6f 6b75 7073 5f64 6963 74da 0b6c  _lookups_dict..l
-000026e0: 6f6f 6b75 705f 6e61 6d65 5a0c 6c6f 6f6b  ookup_nameZ.look
-000026f0: 7570 5f76 616c 7565 da0f 7265 6c61 7469  up_value..relati
-00002700: 6f6e 5f6d 6170 7065 7272 9600 0000 5a12  on_mapperr....Z.
-00002710: 6c61 7374 5f72 656c 6174 6564 5f6d 6f64  last_related_mod
-00002720: 656c 727b 0000 0072 7d00 0000 7279 0000  elr{...r}...ry..
-00002730: 00da 0469 7465 6d72 a700 0000 da08 696e  ...itemr......in
-00002740: 7374 616e 6365 da09 6372 6974 6572 696f  stance..criterio
-00002750: 6e72 2300 0000 7223 0000 0072 2400 0000  nr#...r#...r$...
-00002760: 72a8 0000 000e 0100 0073 8400 0000 0001  r........s......
-00002770: 0802 0e01 0802 1601 0801 0401 0201 0201  ................
-00002780: 0201 0201 0201 0802 0202 0c01 0a01 1002  ................
-00002790: 0801 0802 1201 0801 0801 0401 0201 0201  ................
-000027a0: 0201 0201 0801 0c02 0801 0802 1601 0a01  ................
-000027b0: 1001 1e01 0402 0801 0401 0201 0201 0201  ................
-000027c0: 0201 0801 0602 0a02 0a01 0402 0a01 0c01  ................
-000027d0: 1001 1e01 0401 0201 0a02 0a02 0c02 0a01  ................
-000027e0: 0c01 0601 0401 0201 0201 0802 0a01 1002  ................
-000027f0: 1602 7a26 4772 6170 6851 4c53 6368 656d  ..z&GraphQLSchem
-00002800: 6147 656e 6572 6174 6f72 2e66 696c 7465  aGenerator.filte
-00002810: 725f 7175 6572 7973 6574 6304 0000 0000  r_querysetc.....
-00002820: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
-00002830: 2000 0000 7c03 6400 6b09 721c 7c03 6401   ...|.d.k.r.|.d.
-00002840: 1900 7d04 7400 7c01 7c02 7c04 8303 7d01  ..}.t.|.|.|...}.
-00002850: 7c01 5300 2902 4e72 3800 0000 2901 7215  |.S.).Nr8...).r.
-00002860: 0000 0029 0572 5d00 0000 7270 0000 0072  ...).r]...rp...r
-00002870: 6f00 0000 da06 7365 6172 6368 7238 0000  o.....searchr8..
-00002880: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00002890: 7215 0000 0064 0100 0073 0800 0000 0001  r....d...s......
-000028a0: 0801 0801 0c02 7a26 4772 6170 6851 4c53  ......z&GraphQLS
-000028b0: 6368 656d 6147 656e 6572 6174 6f72 2e73  chemaGenerator.s
-000028c0: 6561 7263 685f 7175 6572 7973 6574 6307  earch_querysetc.
-000028d0: 0000 0000 0000 000a 0000 0008 0000 0043  ...............C
-000028e0: 0000 0073 3400 0000 6700 7d07 782a 7c06  ...s4...g.}.x*|.
-000028f0: 4400 5d22 7d08 7c00 6a00 7c08 7c01 7c02  D.]"}.|.j.|.|.|.
-00002900: 7c03 7c04 7c05 8306 7d09 7c07 6a01 7c09  |.|.|...}.|.j.|.
-00002910: 8301 0100 710a 5700 7c07 5300 2901 4e29  ....q.W.|.S.).N)
-00002920: 02da 1167 6574 5f6d 6f64 656c 735f 6c6f  ...get_models_lo
-00002930: 6f6b 7570 7282 0000 0029 0a72 5d00 0000  okupr....).r]...
-00002940: 726c 0000 0072 8f00 0000 da06 6d6f 6465  rl...r......mode
-00002950: 6c73 726d 0000 0072 6f00 0000 7212 0000  lsrm...ro...r...
-00002960: 0072 9100 0000 da0b 6c6f 6f6b 7570 5f69  .r......lookup_i
-00002970: 7465 6dda 0d6c 6f6f 6b75 705f 7265 7375  tem..lookup_resu
-00002980: 6c74 7223 0000 0072 2300 0000 7224 0000  ltr#...r#...r$..
-00002990: 00da 1267 6574 5f6d 6f64 656c 735f 6c6f  ...get_models_lo
-000029a0: 6f6b 7570 736b 0100 0073 1600 0000 0001  okupsk...s......
-000029b0: 0402 0a01 0401 0201 0201 0201 0201 0201  ................
-000029c0: 0602 0e02 7a29 4772 6170 6851 4c53 6368  ....z)GraphQLSch
-000029d0: 656d 6147 656e 6572 6174 6f72 2e67 6574  emaGenerator.get
-000029e0: 5f6d 6f64 656c 735f 6c6f 6f6b 7570 7363  _models_lookupsc
-000029f0: 0700 0000 0000 0000 1700 0000 0900 0000  ................
-00002a00: 0300 0000 7342 0300 0069 007d 0774 007c  ....sB...i.}.t.|
-00002a10: 0183 017d 0890 0378 2e7c 086a 0183 0044  ...}...x.|.j...D
-00002a20: 0090 035d 205c 027d 097d 0a7c 006a 027c  ...] \.}.}.|.j.|
-00002a30: 037c 0683 027d 0b7c 0b6a 037c 0983 0189  .|...}.|.j.|....
-00002a40: 007c 006a 047c 0683 016a 037c 0983 017d  .|.j.|...j.|...}
-00002a50: 0c7c 0c64 006b 0990 0272 0a69 007d 0d7c  .|.d.k...r.i.}.|
-00002a60: 0c64 0119 0089 0274 0574 0674 0774 0887  .d.....t.t.t.t..
-00002a70: 0266 0164 0264 0384 087c 0483 0283 0183  .f.d.d...|......
-00002a80: 0174 0964 048d 027d 0e7c 0a6a 0364 0564  .t.d...}.|.j.d.d
-00002a90: 0683 027c 0d64 053c 007c 0a6a 0364 0764  ...|.d.<.|.j.d.d
-00002aa0: 0683 027c 0d64 083c 007c 057c 0d64 093c  ...|.d.<.|.|.d.<
-00002ab0: 007c 067c 0d64 0a3c 0074 0a74 0887 0266  .|.|.d.<.t.t...f
-00002ac0: 0164 0b64 0384 087c 0483 0283 017c 0d64  .d.d...|.....|.d
-00002ad0: 0c3c 0088 026a 0b7c 0d64 0d3c 0064 0e7c  .<...j.|.d.<.d.|
-00002ae0: 0a6b 0690 0172 947c 0c64 0f19 007d 0f7c  .k...r.|.d...}.|
-00002af0: 0c64 1019 007d 107c 0c64 1119 007d 1164  .d...}.|.d...}.d
-00002b00: 127c 0a64 0e19 006b 0690 0172 127c 0a64  .|.d...k...r.|.d
-00002b10: 0e19 0064 1219 007d 126e 0c7c 106a 0c64  ...d...}.n.|.j.d
-00002b20: 1319 006a 0b7d 1274 0d7c 0f7c 1264 0083  ...j.}.t.|.|.d..
-00002b30: 037d 137c 1364 006b 0990 0172 9474 0e7c  .}.|.d.k...r.t.|
-00002b40: 0a64 0e19 0064 1419 007c 1383 027d 147c  .d...d...|...}.|
-00002b50: 026a 0f6a 107c 117c 1483 026a 117c 116a  .j.j.|.|...j.|.j
-00002b60: 127c 0e83 0183 016a 137c 1183 017d 1574  .|.....j.|...}.t
-00002b70: 007c 1583 0189 0174 0a74 0887 0187 0266  .|.....t.t.....f
-00002b80: 0264 1564 0384 087c 0483 0283 017c 0d64  .d.d...|.....|.d
-00002b90: 163c 007c 116a 0b7c 0d64 113c 0064 177c  .<.|.j.|.d.<.d.|
-00002ba0: 0a6b 0690 0272 007c 0c64 0f19 007d 0f7c  .k...r.|.d...}.|
-00002bb0: 0c64 1019 007d 107c 0c64 1119 007d 117c  .d...}.|.d...}.|
-00002bc0: 026a 0f6a 107c 0f83 016a 117c 116a 127c  .j.j.|...j.|.j.|
-00002bd0: 0e83 0183 016a 1483 007d 1674 0a7c 1683  .....j...}.t.|..
-00002be0: 017d 167c 006a 157c 0a64 1719 007c 027c  .}.|.j.|.d...|.|
-00002bf0: 037c 167c 0f7c 1083 067c 0d64 183c 007c  .|.|.|...|.d.<.|
-00002c00: 116a 0b7c 0d64 113c 007c 0d7c 077c 093c  .j.|.d.<.|.|.|.<
-00002c10: 0071 1888 0064 006b 0972 1869 007d 0d74  .q...d.k.r.i.}.t
-00002c20: 0574 0674 0774 0887 0066 0164 1964 0384  .t.t.t...f.d.d..
-00002c30: 087c 0483 0283 0183 0174 0964 048d 027d  .|.......t.d...}
-00002c40: 0e7c 0a6a 0364 0564 0683 027c 0d64 053c  .|.j.d.d...|.d.<
-00002c50: 007c 0a6a 0364 0764 0683 027c 0d64 083c  .|.j.d.d...|.d.<
-00002c60: 007c 057c 0d64 093c 007c 067c 0d64 0a3c  .|.|.d.<.|.|.d.<
-00002c70: 0074 0a74 0887 0066 0164 1a64 0384 087c  .t.t...f.d.d...|
-00002c80: 0483 0283 017c 0d64 0c3c 0088 006a 0b7c  .....|.d.<...j.|
-00002c90: 0d64 0d3c 0064 177c 0a6b 0690 0372 3278  .d.<.d.|.k...r2x
-00002ca0: 9a7c 006a 167c 0683 0144 005d 8c7d 0c7c  .|.j.|...D.].}.|
-00002cb0: 0c64 1b19 0074 176b 0390 0273 a27c 0c64  .d...t.k...s.|.d
-00002cc0: 1c19 0088 006a 0b6b 0390 0272 c890 0271  .....j.k...r...q
-00002cd0: a27c 0c64 1019 007d 107c 0c64 0f19 007d  .|.d...}.|.d...}
-00002ce0: 0f7c 0c64 1119 007d 117c 026a 0f6a 107c  .|.d...}.|.j.j.|
-00002cf0: 0f83 016a 117c 116a 127c 0e83 0183 016a  ...j.|.j.|.....j
-00002d00: 1483 007d 1674 0a7c 1683 017d 167c 006a  ...}.t.|...}.|.j
-00002d10: 157c 0a64 1719 007c 027c 037c 167c 0f7c  .|.d...|.|.|.|.|
-00002d20: 1083 067c 0d64 183c 007c 116a 0b7c 0d64  ...|.d.<.|.j.|.d
-00002d30: 113c 0050 0090 0271 a257 007c 0d7c 077c  .<.P...q.W.|.|.|
-00002d40: 093c 0071 1857 007c 0753 0029 1d4e 7279  .<.q.W.|.S.).Nry
-00002d50: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
-00002d60: 0300 0000 1300 0000 730c 0000 0074 007c  ........s....t.|
-00002d70: 0088 006a 0183 0253 0029 014e 2902 7268  ...j...S.).N).rh
-00002d80: 0000 0072 4800 0000 2901 724b 0000 0029  ...rH...).rK...)
-00002d90: 0172 7900 0000 7223 0000 0072 2400 0000  .ry...r#...r$...
-00002da0: 724c 0000 0088 0100 0073 0000 0000 7a3a  rL.......s....z:
-00002db0: 4772 6170 6851 4c53 6368 656d 6147 656e  GraphQLSchemaGen
-00002dc0: 6572 6174 6f72 2e67 6574 5f6d 6f64 656c  erator.get_model
-00002dd0: 735f 6c6f 6f6b 7570 2e3c 6c6f 6361 6c73  s_lookup.<locals
-00002de0: 3e2e 3c6c 616d 6264 613e 2901 728e 0000  >.<lambda>).r...
-00002df0: 00da 0672 6574 7572 6e46 da0a 7265 7475  ...returnF..retu
-00002e00: 726e 4c69 7374 da0b 7265 7475 726e 5f6c  rnList..return_l
-00002e10: 6973 7472 6d00 0000 726f 0000 0063 0100  istrm...ro...c..
-00002e20: 0000 0000 0000 0100 0000 0400 0000 1300  ................
-00002e30: 0000 7312 0000 007c 0074 007c 0088 006a  ..s....|.t.|...j
-00002e40: 0183 0264 019c 0253 0029 024e 2902 72b0  ...d...S.).N).r.
-00002e50: 0000 00da 0576 616c 7565 2902 7268 0000  .....value).rh..
-00002e60: 0072 4800 0000 2901 724b 0000 0029 0172  .rH...).rK...).r
-00002e70: 7900 0000 7223 0000 0072 2400 0000 724c  y...r#...r$...rL
-00002e80: 0000 008e 0100 0073 0000 0000 da0c 6d6f  .......s......mo
-00002e90: 6465 6c5f 7661 6c75 6573 da0d 736f 7572  del_values..sour
-00002ea0: 6365 5f63 6f6c 756d 6eda 0961 6767 7265  ce_column..aggre
-00002eb0: 6761 7465 727b 0000 0072 7c00 0000 727d  gater{...r|...r}
-00002ec0: 0000 0072 4100 0000 7201 0000 0072 4000  ...rA...r....r@.
-00002ed0: 0000 6301 0000 0000 0000 0001 0000 0005  ..c.............
-00002ee0: 0000 0013 0000 0073 1a00 0000 7c00 8800  .......s....|...
-00002ef0: 6a00 7401 7c00 8801 6a02 8302 6401 8302  j.t.|...j...d...
-00002f00: 6402 9c02 5300 2903 4e72 0100 0000 2902  d...S.).Nr....).
-00002f10: 72b0 0000 0072 bb00 0000 2903 7285 0000  r....r....).r...
-00002f20: 0072 6800 0000 7248 0000 0029 0172 4b00  .rh...rH...).rK.
-00002f30: 0000 2902 da0b 6772 6f75 7073 5f64 6963  ..)...groups_dic
-00002f40: 7472 7900 0000 7223 0000 0072 2400 0000  try...r#...r$...
-00002f50: 724c 0000 00a5 0100 0073 0400 0000 0001  rL.......s......
-00002f60: 0201 da11 6167 6772 6567 6174 6564 5f76  ....aggregated_v
-00002f70: 616c 7565 7372 a500 0000 da07 7265 6c61  aluesr......rela
-00002f80: 7465 6463 0100 0000 0000 0000 0100 0000  tedc............
-00002f90: 0300 0000 1300 0000 730c 0000 0074 007c  ........s....t.|
-00002fa0: 0088 006a 0183 0253 0029 014e 2902 7268  ...j...S.).N).rh
-00002fb0: 0000 0072 4800 0000 2901 724b 0000 0029  ...rH...).rK...)
-00002fc0: 0172 a600 0000 7223 0000 0072 2400 0000  .r....r#...r$...
-00002fd0: 724c 0000 00c3 0100 0073 0000 0000 6301  rL.......s....c.
-00002fe0: 0000 0000 0000 0001 0000 0004 0000 0013  ................
-00002ff0: 0000 0073 1200 0000 7c00 7400 7c00 8800  ...s....|.t.|...
-00003000: 6a01 8302 6401 9c02 5300 2902 4e29 0272  j...d...S.).N).r
-00003010: b000 0000 72bb 0000 0029 0272 6800 0000  ....r....).rh...
-00003020: 7248 0000 0029 0172 4b00 0000 2901 72a6  rH...).rK...).r.
-00003030: 0000 0072 2300 0000 7224 0000 0072 4c00  ...r#...r$...rL.
-00003040: 0000 c901 0000 7300 0000 0072 7800 0000  ......s....rx...
-00003050: 727a 0000 0029 1872 4f00 0000 724e 0000  rz...).rO...rN..
-00003060: 0072 9f00 0000 7285 0000 0072 a200 0000  .r....r....r....
-00003070: da06 736f 7274 6564 7219 0000 0072 1a00  ..sortedr....r..
-00003080: 0000 724d 0000 0072 1800 0000 da04 6c69  ..rM...r......li
-00003090: 7374 7248 0000 0072 6300 0000 7268 0000  strH...rc...rh..
-000030a0: 0072 1400 0000 7265 0000 0072 3800 0000  .r....re...r8...
-000030b0: 7269 0000 00da 0369 6e5f 726b 0000 0072  ri.....in_rk...r
-000030c0: 8000 0000 72b3 0000 0072 a000 0000 720a  ....r....r....r.
-000030d0: 0000 0029 1772 5d00 0000 72b5 0000 0072  ...).r]...r....r
-000030e0: 6c00 0000 728f 0000 0072 b400 0000 726d  l...r....r....rm
-000030f0: 0000 0072 6f00 0000 7291 0000 005a 106c  ...ro...r....Z.l
-00003100: 6f6f 6b75 705f 6974 656d 5f64 6963 7472  ookup_item_dictr
-00003110: ad00 0000 da0b 6c6f 6f6b 7570 5f64 6174  ......lookup_dat
-00003120: 6172 ac00 0000 7296 0000 0072 b600 0000  ar....r....r....
-00003130: 5a0d 6c6f 6f6b 7570 5f76 616c 7565 735a  Z.lookup_valuesZ
-00003140: 0e72 656c 6174 696f 6e5f 6d6f 6465 6c72  .relation_modelr
-00003150: ae00 0000 7297 0000 005a 1561 6767 7265  ....r....Z.aggre
-00003160: 6761 7465 5f63 6f6c 756d 6e5f 6e61 6d65  gate_column_name
-00003170: 5a10 6167 6772 6567 6174 655f 636f 6c75  Z.aggregate_colu
-00003180: 6d6e 5a0e 6167 6772 6567 6174 655f 6675  mnZ.aggregate_fu
-00003190: 6e63 da06 6772 6f75 7073 5a0e 7265 6c61  nc..groupsZ.rela
-000031a0: 7465 645f 6d6f 6465 6c73 7223 0000 0029  ted_modelsr#...)
-000031b0: 0372 a600 0000 72bf 0000 0072 7900 0000  .r....r....ry...
-000031c0: 7224 0000 0072 b300 0000 7b01 0000 73a4  r$...r....{...s.
-000031d0: 0000 0000 0104 0208 0216 010c 010a 0110  ................
-000031e0: 020a 0104 0108 0122 0210 0110 0108 0108  ......."........
-000031f0: 011a 010a 020a 0108 0108 0108 020e 010e  ................
-00003200: 020c 020c 010a 0112 0206 0108 010c 0106  ................
-00003210: 0108 0210 030c 010a 020a 0108 0108 0108  ................
-00003220: 0206 0106 0110 0208 0204 0106 0102 0102  ................
-00003230: 0102 0102 010a 020a 020a 0108 0104 0122  ..............."
-00003240: 0210 0110 0108 0108 011a 010a 020a 0110  ................
-00003250: 011e 0104 0208 0108 0108 0206 0106 0110  ................
-00003260: 0208 0204 0106 0102 0102 0102 0102 010a  ................
-00003270: 020a 0108 020c 027a 2847 7261 7068 514c  .......z(GraphQL
-00003280: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
-00003290: 6765 745f 6d6f 6465 6c73 5f6c 6f6f 6b75  get_models_looku
-000032a0: 7063 0300 0000 0000 0000 0700 0000 0600  pc..............
-000032b0: 0000 0300 0000 73fa 0000 0069 007d 0378  ......s....i.}.x
-000032c0: f07c 016a 0083 0044 005d e45c 027d 0489  .|.j...D.].\.}..
-000032d0: 0169 007d 0588 0164 0119 007d 0688 0072  .i.}...d...}...r
-000032e0: 3c74 0174 0287 0066 0164 0264 0384 087c  <t.t...f.d.d...|
-000032f0: 0683 0283 017d 0674 0174 0374 0464 0464  .....}.t.t.t.d.d
-00003300: 0384 007c 0683 0283 0183 0189 0288 0164  ...|...........d
-00003310: 0519 0072 8488 0164 0619 0072 6c88 027c  ...r...d...rl..|
-00003320: 0564 073c 006e 1874 0588 0283 0172 7c88  .d.<.n.t.....r|.
-00003330: 0264 0819 006e 0264 007c 0564 073c 0064  .d...n.d.|.d.<.d
-00003340: 0988 016b 0672 aa7c 006a 0688 0164 0919  ...k.r.|.j...d..
-00003350: 0087 0187 0266 0264 0a64 0384 0883 027c  .....f.d.d.....|
-00003360: 0564 093c 0064 0b88 016b 0672 ea74 0174  .d.<.d...k.r.t.t
-00003370: 0287 0187 0266 0264 0c64 0384 0888 0164  .....f.d.d.....d
-00003380: 0b19 0083 0283 017d 0674 057c 0683 0172  .......}.t.|...r
-00003390: e27c 0664 0819 0064 0719 006e 0264 087c  .|.d...d...n.d.|
-000033a0: 0564 0d3c 007c 057c 037c 043c 0071 0e57  .d.<.|.|.|.<.q.W
-000033b0: 007c 0353 0029 0e4e 72bc 0000 0063 0100  .|.S.).Nr....c..
-000033c0: 0000 0000 0000 0100 0000 0300 0000 1300  ................
-000033d0: 0000 730c 0000 0088 007c 0064 0119 0083  ..s......|.d....
-000033e0: 0153 0029 024e 72b0 0000 0072 2300 0000  .S.).Nr....r#...
-000033f0: 2901 724b 0000 0029 01da 1269 6e73 7461  ).rK...)...insta
-00003400: 6e63 655f 7072 6564 6963 6174 6572 2300  nce_predicater#.
-00003410: 0000 7224 0000 0072 4c00 0000 f301 0000  ..r$...rL.......
-00003420: 7300 0000 007a 3d47 7261 7068 514c 5363  s....z=GraphQLSc
-00003430: 6865 6d61 4765 6e65 7261 746f 722e 6669  hemaGenerator.fi
-00003440: 6c74 6572 5f6c 6f6f 6b75 705f 6d6f 6465  lter_lookup_mode
-00003450: 6c73 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ls.<locals>.<lam
-00003460: 6264 613e 6301 0000 0000 0000 0001 0000  bda>c...........
-00003470: 0002 0000 0053 0000 0073 0800 0000 7c00  .....S...s....|.
-00003480: 6401 1900 5300 2902 4e72 bb00 0000 7223  d...S.).Nr....r#
-00003490: 0000 0029 0172 4b00 0000 7223 0000 0072  ...).rK...r#...r
-000034a0: 2300 0000 7224 0000 0072 4c00 0000 f501  #...r$...rL.....
-000034b0: 0000 7300 0000 0072 b800 0000 72ba 0000  ..s....r....r...
-000034c0: 0072 bb00 0000 7201 0000 0072 c100 0000  .r....r....r....
-000034d0: 6301 0000 0000 0000 0001 0000 0004 0000  c...............
-000034e0: 0013 0000 0073 1400 0000 7400 7c00 8800  .....s....t.|...
-000034f0: 6401 1900 6400 8303 8801 6b06 5300 2902  d...d.....k.S.).
-00003500: 4e72 7d00 0000 2901 7268 0000 0029 0172  Nr}...).rh...).r
-00003510: 4b00 0000 2902 72c5 0000 0072 8b00 0000  K...).r....r....
-00003520: 7223 0000 0072 2400 0000 724c 0000 0000  r#...r$...rL....
-00003530: 0200 0073 0000 0000 72c0 0000 0063 0100  ...s....r....c..
-00003540: 0000 0000 0000 0100 0000 0400 0000 1300  ................
-00003550: 0000 7318 0000 0074 007c 0064 0119 0088  ..s....t.|.d....
-00003560: 0064 0219 0064 0083 0388 016b 0653 0029  .d...d.....k.S.)
-00003570: 034e 72b0 0000 0072 bd00 0000 2901 7268  .Nr....r....).rh
-00003580: 0000 0029 0172 4b00 0000 2902 72c5 0000  ...).rK...).r...
-00003590: 0072 8b00 0000 7223 0000 0072 2400 0000  .r....r#...r$...
-000035a0: 724c 0000 0005 0200 0073 0000 0000 5a0a  rL.......s....Z.
-000035b0: 6167 6772 6567 6174 6564 2907 724e 0000  aggregated).rN..
-000035c0: 0072 c300 0000 7269 0000 0072 1a00 0000  .r....ri...r....
-000035d0: 724d 0000 0072 6600 0000 da14 6669 6c74  rM...rf.....filt
-000035e0: 6572 5f6c 6f6f 6b75 705f 6d6f 6465 6c73  er_lookup_models
-000035f0: 2907 725d 0000 0072 a700 0000 72c7 0000  ).r]...r....r...
-00003600: 0072 9100 0000 72ad 0000 005a 0b69 7465  .r....r....Z.ite
-00003610: 6d5f 7265 7375 6c74 72bc 0000 0072 2300  m_resultr....r#.
-00003620: 0000 2903 72c7 0000 0072 c500 0000 728b  ..).r....r....r.
-00003630: 0000 0072 2400 0000 72c8 0000 00ea 0100  ...r$...r.......
-00003640: 0073 2c00 0000 0001 0402 1201 0402 0802  .s,.............
-00003650: 0401 1602 1602 0801 0801 0a02 1802 0801  ................
-00003660: 0401 0601 1403 0801 0401 0c01 0c02 1c02  ................
-00003670: 0c02 7a2b 4772 6170 6851 4c53 6368 656d  ..z+GraphQLSchem
-00003680: 6147 656e 6572 6174 6f72 2e66 696c 7465  aGenerator.filte
-00003690: 725f 6c6f 6f6b 7570 5f6d 6f64 656c 7363  r_lookup_modelsc
-000036a0: 0500 0000 0000 0000 0800 0000 0300 0000  ................
-000036b0: 4300 0000 733e 0000 007c 046a 0064 0164  C...s>...|.j.d.d
-000036c0: 0283 027d 057c 006a 017c 017c 0283 027d  ...}.|.j.|.|...}
-000036d0: 067c 066a 007c 0383 017d 077c 0764 006b  .|.j.|...}.|.d.k
-000036e0: 0872 2e64 0053 007c 0572 3a74 027c 0783  .r.d.S.|.r:t.|..
-000036f0: 017d 077c 0753 0029 034e 7230 0000 0046  .}.|.S.).Nr0...F
-00003700: 2903 7285 0000 0072 9f00 0000 7206 0000  ).r....r....r...
-00003710: 0029 0872 5d00 0000 728f 0000 0072 6f00  .).r]...r....ro.
-00003720: 0000 7248 0000 00da 076f 7074 696f 6e73  ..rH.....options
-00003730: 7230 0000 0072 ac00 0000 72a6 0000 0072  r0...r....r....r
-00003740: 2300 0000 7223 0000 0072 2400 0000 da14  #...r#...r$.....
-00003750: 6d61 705f 736f 7274 5f6f 7264 6572 5f66  map_sort_order_f
-00003760: 6965 6c64 0e02 0000 7310 0000 0000 010c  ield....s.......
-00003770: 020c 010a 0208 0104 0204 0108 027a 2b47  .............z+G
-00003780: 7261 7068 514c 5363 6865 6d61 4765 6e65  raphQLSchemaGene
-00003790: 7261 746f 722e 6d61 705f 736f 7274 5f6f  rator.map_sort_o
-000037a0: 7264 6572 5f66 6965 6c64 6305 0000 0000  rder_fieldc.....
-000037b0: 0000 000b 0000 0005 0000 0003 0000 0073  ...............s
-000037c0: 8000 0000 784e 7c04 4400 5d46 7d05 7400  ....xN|.D.]F}.t.
-000037d0: 7c05 8301 7d06 7401 8700 8701 8702 6603  |...}.t.......f.
-000037e0: 6401 6402 8408 7c06 6a02 8300 8302 7d07  d.d...|.j.....}.
-000037f0: 7403 6403 6402 8400 7c07 8302 7d07 7404  t.d.d...|...}.t.
-00003800: 7c07 8301 7d07 7c01 6a05 7c07 8e00 7d01  |...}.|.j.|...}.
-00003810: 7106 5700 8801 6a06 6404 1900 7d08 7407  q.W...j.d...}.t.
-00003820: 8800 6a08 7c08 8302 7d09 8800 6a09 6a0a  ..j.|...}...j.j.
-00003830: 7c09 8301 7d0a 740b 7c0a 7c01 8302 7d01  |...}.t.|.|...}.
-00003840: 7c01 5300 2905 4e63 0100 0000 0000 0000  |.S.).Nc........
-00003850: 0100 0000 0600 0000 1300 0000 7318 0000  ............s...
-00003860: 0088 026a 0088 0088 017c 0064 0119 007c  ...j.....|.d...|
-00003870: 0064 0219 0083 0453 0029 034e 7201 0000  .d.....S.).Nr...
-00003880: 0072 4a00 0000 2901 72ca 0000 0029 0172  .rJ...).r....).r
-00003890: 4b00 0000 2903 728f 0000 0072 6f00 0000  K...).r....ro...
-000038a0: 725d 0000 0072 2300 0000 7224 0000 0072  r]...r#...r$...r
-000038b0: 4c00 0000 2002 0000 7300 0000 007a 3647  L... ...s....z6G
-000038c0: 7261 7068 514c 5363 6865 6d61 4765 6e65  raphQLSchemaGene
-000038d0: 7261 746f 722e 736f 7274 5f71 7565 7279  rator.sort_query
-000038e0: 7365 742e 3c6c 6f63 616c 733e 2e3c 6c61  set.<locals>.<la
-000038f0: 6d62 6461 3e63 0100 0000 0000 0000 0100  mbda>c..........
-00003900: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
-00003910: 0064 006b 0953 0029 014e 7223 0000 0029  .d.k.S.).Nr#...)
-00003920: 0172 4b00 0000 7223 0000 0072 2300 0000  .rK...r#...r#...
-00003930: 7224 0000 0072 4c00 0000 2102 0000 7300  r$...rL...!...s.
-00003940: 0000 0072 0100 0000 290c 724f 0000 0072  ...r....).rO...r
-00003950: 4d00 0000 724e 0000 0072 6900 0000 72c3  M...rN...ri...r.
-00003960: 0000 00da 086f 7264 6572 5f62 7972 6700  .....order_byrg.
-00003970: 0000 7211 0000 0072 7700 0000 7283 0000  ..r....rw...r...
-00003980: 0072 8500 0000 721d 0000 0029 0b72 5d00  .r....r....).r].
-00003990: 0000 7270 0000 0072 8f00 0000 726f 0000  ..rp...r....ro..
-000039a0: 00da 0473 6f72 7472 af00 0000 5a09 6974  ...sortr....Z.it
-000039b0: 656d 5f64 6963 7472 cb00 0000 7294 0000  em_dictr....r...
-000039c0: 0072 4800 0000 726d 0000 0072 2300 0000  .rH...rm...r#...
-000039d0: 2903 728f 0000 0072 6f00 0000 725d 0000  ).r....ro...r]..
-000039e0: 0072 2400 0000 da0d 736f 7274 5f71 7565  .r$.....sort_que
-000039f0: 7279 7365 741c 0200 0073 1600 0000 0001  ryset....s......
-00003a00: 0a01 0802 1a01 0e01 0802 0e02 0a01 0c01  ................
-00003a10: 0c01 0a02 7a24 4772 6170 6851 4c53 6368  ....z$GraphQLSch
-00003a20: 656d 6147 656e 6572 6174 6f72 2e73 6f72  emaGenerator.sor
-00003a30: 745f 7175 6572 7973 6574 6302 0000 0000  t_querysetc.....
-00003a40: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00003a50: 0c00 0000 7c01 6a00 6401 6402 8302 5300  ....|.j.d.d...S.
-00003a60: 2903 4e72 3500 0000 e914 0000 0029 0172  ).Nr5........).r
-00003a70: 8500 0000 2902 725d 0000 00da 0a70 6167  ....).r].....pag
-00003a80: 696e 6174 696f 6e72 2300 0000 7223 0000  inationr#...r#..
-00003a90: 0072 2400 0000 da14 6765 745f 7061 6769  .r$.....get_pagi
-00003aa0: 6e61 7469 6f6e 5f6c 696d 6974 2d02 0000  nation_limit-...
-00003ab0: 7302 0000 0000 017a 2b47 7261 7068 514c  s......z+GraphQL
-00003ac0: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
-00003ad0: 6765 745f 7061 6769 6e61 7469 6f6e 5f6c  get_pagination_l
-00003ae0: 696d 6974 6303 0000 0000 0000 0004 0000  imitc...........
-00003af0: 0003 0000 0043 0000 0073 4e00 0000 7c00  .....C...sN...|.
-00003b00: 6a00 7c02 8301 7d03 6401 7c02 6b06 7222  j.|...}.d.|.k.r"
-00003b10: 7c01 6a01 7c02 6401 1900 8301 7d01 6e1e  |.j.|.d.....}.n.
-00003b20: 6402 7c02 6b06 7240 7c01 6a01 7c02 6402  d.|.k.r@|.j.|.d.
-00003b30: 1900 6403 1800 7c03 1400 8301 7d01 7c01  ..d...|.....}.|.
-00003b40: 6a02 7c03 8301 7d01 7c01 5300 2904 4e72  j.|...}.|.S.).Nr
-00003b50: 3400 0000 7233 0000 0072 4a00 0000 2903  4...r3...rJ...).
-00003b60: 72d0 0000 0072 3400 0000 7235 0000 0029  r....r4...r5...)
-00003b70: 0472 5d00 0000 7270 0000 0072 cf00 0000  .r]...rp...r....
-00003b80: 7235 0000 0072 2300 0000 7223 0000 0072  r5...r#...r#...r
-00003b90: 2400 0000 da11 7061 6769 6e61 7465 5f71  $.....paginate_q
-00003ba0: 7565 7279 7365 7430 0200 0073 0e00 0000  ueryset0...s....
-00003bb0: 0001 0a02 0801 1001 0801 1602 0a02 7a28  ..............z(
-00003bc0: 4772 6170 6851 4c53 6368 656d 6147 656e  GraphQLSchemaGen
-00003bd0: 6572 6174 6f72 2e70 6167 696e 6174 655f  erator.paginate_
-00003be0: 7175 6572 7973 6574 724a 0000 0063 0400  querysetrJ...c..
-00003bf0: 0000 0000 0000 0e00 0000 0700 0000 4300  ..............C.
-00003c00: 0000 730a 0100 007c 0364 016b 017d 0474  ..s....|.d.k.}.t
-00003c10: 007c 026a 016a 0283 017d 057c 0472 2464  .|.j.j...}.|.r$d
-00003c20: 026a 037c 057c 0383 026e 0a64 036a 037c  .j.|.|...n.d.j.|
-00003c30: 057c 0383 027d 067c 067c 006a 046b 0672  .|...}.|.|.j.k.r
-00003c40: 4a74 056a 067c 006a 047c 0619 0083 0153  Jt.j.|.j.|.....S
-00003c50: 0069 007d 0778 347c 026a 0744 005d 2a7d  .i.}.x4|.j.D.]*}
-00003c60: 087c 006a 087c 017c 027c 087c 047c 0383  .|.j.|.|.|.|.|..
-00003c70: 057d 0974 007c 086a 0283 017d 0a7c 0983  .}.t.|.j...}.|..
-00003c80: 007c 077c 0a3c 0071 5657 007c 0472 e878  .|.|.<.qVW.|.r.x
-00003c90: 487c 006a 097c 0283 0144 005d 3a7d 0b7c  H|.j.|...D.]:}.|
-00003ca0: 0b64 0419 0074 0a6b 0372 a671 947c 006a  .d...t.k.r.q.|.j
-00003cb0: 0b7c 017c 027c 0b7c 047c 0383 057d 0c74  .|.|.|.|.|...}.t
-00003cc0: 007c 0b64 0519 0083 017d 0a7c 0c83 007c  .|.d.....}.|...|
-00003cd0: 077c 0a3c 0071 9457 007c 006a 0c7c 017c  .|.<.q.W.|.j.|.|
-00003ce0: 027c 0364 0617 0083 037c 0764 073c 0074  .|.d.....|.d.<.t
-00003cf0: 0d7c 0674 0e66 017c 0783 037d 0d7c 0d7c  .|.t.f.|...}.|.|
-00003d00: 006a 047c 063c 0074 056a 067c 0d83 0153  .j.|.<.t.j.|...S
-00003d10: 0029 084e e904 0000 007a 1f4d 6f64 656c  .).N.....z.Model
-00003d20: 7b7d 4465 7074 687b 7d4e 6573 7465 6446  {}Depth{}NestedF
-00003d30: 696c 7465 7273 5479 7065 7a19 4d6f 6465  iltersTypez.Mode
-00003d40: 6c7b 7d44 6570 7468 7b7d 4669 6c74 6572  l{}Depth{}Filter
-00003d50: 7354 7970 6572 7800 0000 7248 0000 0072  sTyperx...rH...r
-00003d60: 4a00 0000 72a3 0000 0029 0f72 4900 0000  J...r....).rI...
-00003d70: 7284 0000 0072 4800 0000 da06 666f 726d  r....rH.....form
-00003d80: 6174 7256 0000 0072 2e00 0000 da04 4c69  atrV...r......Li
-00003d90: 7374 729d 0000 00da 1c67 6574 5f6d 6f64  str......get_mod
-00003da0: 656c 5f66 6965 6c64 5f66 696c 7465 7273  el_field_filters
-00003db0: 5f74 7970 6572 a000 0000 720b 0000 00da  _typer....r.....
-00003dc0: 2367 6574 5f6d 6f64 656c 5f72 656c 6174  #get_model_relat
-00003dd0: 696f 6e73 6869 705f 6669 6c74 6572 735f  ionship_filters_
-00003de0: 7479 7065 da16 6765 745f 6d6f 6465 6c5f  type..get_model_
-00003df0: 6669 6c74 6572 735f 7479 7065 72aa 0000  filters_typer...
-00003e00: 0072 1f00 0000 290e 725d 0000 0072 8f00  .r....).r]...r..
-00003e10: 0000 726f 0000 00da 0564 6570 7468 da0e  ..ro.....depth..
-00003e20: 7769 7468 5f72 656c 6174 696f 6e73 da0a  with_relations..
-00003e30: 6d6f 6465 6c5f 6e61 6d65 da08 636c 735f  model_name..cls_
-00003e40: 6e61 6d65 da05 6174 7472 7372 a600 0000  name..attrsr....
-00003e50: da13 636f 6c75 6d6e 5f66 696c 7465 7273  ..column_filters
-00003e60: 5f74 7970 65da 0961 7474 725f 6e61 6d65  _type..attr_name
-00003e70: 7296 0000 005a 1972 656c 6174 696f 6e73  r....Z.relations
-00003e80: 6869 705f 6669 6c74 6572 735f 7479 7065  hip_filters_type
-00003e90: da03 636c 7372 2300 0000 7223 0000 0072  ..clsr#...r#...r
-00003ea0: 2400 0000 72d7 0000 003c 0200 0073 2c00  $...r....<...s,.
-00003eb0: 0000 0001 0801 0c01 1001 0c02 0a01 1002  ................
-00003ec0: 0402 0c01 1201 0a01 0e02 0401 1001 0c01  ................
-00003ed0: 0202 1201 0c01 0e02 1602 0e01 0a01 7a2d  ..............z-
-00003ee0: 4772 6170 6851 4c53 6368 656d 6147 656e  GraphQLSchemaGen
-00003ef0: 6572 6174 6f72 2e67 6574 5f6d 6f64 656c  erator.get_model
-00003f00: 5f66 696c 7465 7273 5f74 7970 6563 0600  _filters_typec..
-00003f10: 0000 0000 0000 1200 0000 0600 0000 4300  ..............C.
-00003f20: 0000 7300 0100 0074 007c 026a 016a 0283  ..s....t.|.j.j..
-00003f30: 017d 0674 007c 036a 0283 017d 077c 0472  .}.t.|.j...}.|.r
-00003f40: 2864 016a 037c 067c 077c 0583 036e 0c64  (d.j.|.|.|...n.d
-00003f50: 026a 037c 067c 077c 0583 037d 087c 087c  .j.|.|.|...}.|.|
-00003f60: 006a 046b 0672 4a7c 006a 047c 0819 0053  .j.k.rJ|.j.|...S
-00003f70: 0069 007d 0974 057c 036a 0683 017d 0a78  .i.}.t.|.j...}.x
-00003f80: 347c 0a64 0319 0044 005d 287d 0b74 076a  4|.d...D.](}.t.j
-00003f90: 086a 097c 0b83 017d 0c74 076a 0a6a 097c  .j.|...}.t.j.j.|
-00003fa0: 0b74 0b83 0083 027d 0d7c 0d7c 097c 0c3c  .t.....}.|.|.|.<
-00003fb0: 0071 6257 007c 0472 e478 507c 006a 0c7c  .qbW.|.r.xP|.j.|
-00003fc0: 0283 0144 005d 427d 0e7c 0e64 0419 0074  ...D.]B}.|.d...t
-00003fd0: 0d6b 0373 9e7c 0e64 0519 007c 076b 0372  .k.s.|.d...|.k.r
-00003fe0: bc71 9e7c 0e64 0619 007d 0f7c 006a 0e7c  .q.|.d...}.|.j.|
-00003ff0: 017c 0f7c 0564 0717 0083 037d 107c 107c  .|.|.d.....}.|.|
-00004000: 0964 083c 0050 0071 9e57 0074 067c 0874  .d.<.P.q.W.t.|.t
-00004010: 0f66 017c 0983 037d 117c 117c 006a 047c  .f.|...}.|.|.j.|
-00004020: 083c 007c 1153 0029 094e 7a27 4d6f 6465  .<.|.S.).Nz'Mode
-00004030: 6c7b 7d43 6f6c 756d 6e7b 7d44 6570 7468  l{}Column{}Depth
-00004040: 7b7d 4e65 7374 6564 4669 6c74 6572 7354  {}NestedFiltersT
-00004050: 7970 657a 214d 6f64 656c 7b7d 436f 6c75  ypez!Model{}Colu
-00004060: 6d6e 7b7d 4465 7074 687b 7d46 696c 7465  mn{}Depth{}Filte
-00004070: 7273 5479 7065 7212 0000 0072 7800 0000  rsTyper....rx...
-00004080: 727a 0000 0072 7c00 0000 724a 0000 0072  rz...r|...rJ...r
-00004090: a500 0000 2910 7249 0000 0072 8400 0000  ....).rI...r....
-000040a0: 7248 0000 0072 d300 0000 7257 0000 0072  rH...r....rW...r
-000040b0: 1300 0000 72aa 0000 0072 1200 0000 5a03  ....r....r....Z.
-000040c0: 6771 6c72 8500 0000 da0a 6771 6c5f 7363  gqlr......gql_sc
-000040d0: 616c 6172 721b 0000 0072 a000 0000 720a  alarr....r....r.
-000040e0: 0000 0072 d700 0000 7225 0000 0029 1272  ...r....r%...).r
-000040f0: 5d00 0000 728f 0000 0072 6f00 0000 72a6  ]...r....ro...r.
-00004100: 0000 0072 d900 0000 72d8 0000 0072 da00  ...r....r....r..
-00004110: 0000 da0b 636f 6c75 6d6e 5f6e 616d 6572  ....column_namer
-00004120: db00 0000 72dc 0000 0072 af00 0000 72a7  ....r....r....r.
-00004130: 0000 005a 0a67 716c 5f6c 6f6f 6b75 7072  ...Z.gql_lookupr
-00004140: e000 0000 7296 0000 0072 ae00 0000 72dd  ....r....r....r.
-00004150: 0000 0072 df00 0000 7223 0000 0072 2300  ...r....r#...r#.
-00004160: 0000 7224 0000 0072 d500 0000 5b02 0000  ..r$...r....[...
-00004170: 732e 0000 0000 010c 010a 0112 010e 020a  s...............
-00004180: 010a 0204 010a 020e 010c 0110 010c 0204  ................
-00004190: 0110 0118 0102 0208 0112 0108 0106 020e  ................
-000041a0: 010a 017a 3347 7261 7068 514c 5363 6865  ...z3GraphQLSche
-000041b0: 6d61 4765 6e65 7261 746f 722e 6765 745f  maGenerator.get_
-000041c0: 6d6f 6465 6c5f 6669 656c 645f 6669 6c74  model_field_filt
-000041d0: 6572 735f 7479 7065 6306 0000 0000 0000  ers_typec.......
-000041e0: 000c 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
-000041f0: 0000 7400 7c02 6a01 6a02 8301 7d06 7400  ..t.|.j.j...}.t.
-00004200: 7c03 6401 1900 8301 7d07 7c04 722a 6402  |.d.....}.|.r*d.
-00004210: 6a03 7c06 7c07 7c05 8303 6e0c 6403 6a03  j.|.|.|...n.d.j.
-00004220: 7c06 7c07 7c05 8303 7d08 7c08 7c00 6a04  |.|.|...}.|.|.j.
-00004230: 6b06 724c 7c00 6a04 7c08 1900 5300 6900  k.rL|.j.|...S.i.
-00004240: 7d09 7c00 6a05 7c01 7c03 6404 1900 7c05  }.|.j.|.|.d...|.
-00004250: 6405 1700 8303 7d0a 7c0a 7c09 6406 3c00  d.....}.|.|.d.<.
-00004260: 7406 7c08 7407 6601 7c09 8303 7d0b 7c0b  t.|.t.f.|...}.|.
-00004270: 7c00 6a04 7c08 3c00 7c0b 5300 2907 4e72  |.j.|.<.|.S.).Nr
-00004280: 4800 0000 7a2c 4d6f 6465 6c7b 7d43 6f6c  H...z,Model{}Col
-00004290: 756d 6e7b 7d44 6570 7468 7b7d 4e65 7374  umn{}Depth{}Nest
-000042a0: 6564 5265 6c61 7469 6f6e 7368 6970 5479  edRelationshipTy
-000042b0: 7065 7a26 4d6f 6465 6c7b 7d43 6f6c 756d  pez&Model{}Colum
-000042c0: 6e7b 7d44 6570 7468 7b7d 5265 6c61 7469  n{}Depth{}Relati
-000042d0: 6f6e 7368 6970 5479 7065 727c 0000 0072  onshipTyper|...r
-000042e0: 4a00 0000 72a5 0000 0029 0872 4900 0000  J...r....).rI...
-000042f0: 7284 0000 0072 4800 0000 72d3 0000 0072  r....rH...r....r
-00004300: 5800 0000 72d7 0000 0072 aa00 0000 7226  X...r....r....r&
-00004310: 0000 0029 0c72 5d00 0000 728f 0000 0072  ...).r]...r....r
-00004320: 6f00 0000 7296 0000 0072 d900 0000 72d8  o...r....r....r.
-00004330: 0000 0072 da00 0000 da10 7265 6c61 7469  ...r......relati
-00004340: 6f6e 7368 6970 5f6b 6579 72db 0000 0072  onship_keyr....r
-00004350: dc00 0000 da0c 6c6f 6f6b 7570 735f 7479  ......lookups_ty
-00004360: 7065 72df 0000 0072 2300 0000 7223 0000  per....r#...r#..
-00004370: 0072 2400 0000 72d6 0000 007a 0200 0073  .r$...r....z...s
-00004380: 1800 0000 0001 0c01 0c01 1201 0e02 0a01  ................
-00004390: 0a02 0402 1601 0802 0e01 0a01 7a3a 4772  ............z:Gr
-000043a0: 6170 6851 4c53 6368 656d 6147 656e 6572  aphQLSchemaGener
-000043b0: 6174 6f72 2e67 6574 5f6d 6f64 656c 5f72  ator.get_model_r
-000043c0: 656c 6174 696f 6e73 6869 705f 6669 6c74  elationship_filt
-000043d0: 6572 735f 7479 7065 6304 0000 0000 0000  ers_typec.......
-000043e0: 000e 0000 0007 0000 0043 0000 0073 e800  .........C...s..
-000043f0: 0000 7c03 6401 6b01 7d04 7400 7c02 6a01  ..|.d.k.}.t.|.j.
-00004400: 6a02 8301 7d05 7c04 7224 6402 6a03 7c05  j...}.|.r$d.j.|.
-00004410: 7c03 8302 6e0a 6403 6a03 7c05 7c03 8302  |...n.d.j.|.|...
-00004420: 7d06 7c06 7c00 6a04 6b06 7244 7c00 6a04  }.|.|.j.k.rD|.j.
-00004430: 7c06 1900 5300 6900 7d07 7834 7c02 6a05  |...S.i.}.x4|.j.
-00004440: 4400 5d2a 7d08 7c00 6a06 7c01 7c02 7c08  D.]*}.|.j.|.|.|.
-00004450: 7c04 7c03 8305 7d09 7400 7c08 6a02 8301  |.|...}.t.|.j...
-00004460: 7d0a 7c09 8300 7c07 7c0a 3c00 7150 5700  }.|...|.|.<.qPW.
-00004470: 7c04 72cc 7848 7c00 6a07 7c02 8301 4400  |.r.xH|.j.|...D.
-00004480: 5d3a 7d0b 7c0b 6404 1900 7408 6b03 72a0  ]:}.|.d...t.k.r.
-00004490: 718e 7c00 6a09 7c01 7c02 7c0b 7c04 7c03  q.|.j.|.|.|.|.|.
-000044a0: 8305 7d0c 7400 7c0b 6405 1900 8301 7d0a  ..}.t.|.d.....}.
-000044b0: 7c0c 8300 7c07 7c0a 3c00 718e 5700 740a  |...|.|.<.q.W.t.
-000044c0: 7c06 740b 6601 7c07 8303 7d0d 7c0d 7c00  |.t.f.|...}.|.|.
-000044d0: 6a04 7c06 3c00 7c0d 5300 2906 4e72 d200  j.|.<.|.S.).Nr..
-000044e0: 0000 7a1f 4d6f 6465 6c7b 7d44 6570 7468  ..z.Model{}Depth
-000044f0: 7b7d 4e65 7374 6564 4c6f 6f6b 7570 7354  {}NestedLookupsT
-00004500: 7970 657a 194d 6f64 656c 7b7d 4465 7074  ypez.Model{}Dept
-00004510: 687b 7d4c 6f6f 6b75 7073 5479 7065 7278  h{}LookupsTyperx
-00004520: 0000 0072 4800 0000 290c 7249 0000 0072  ...rH...).rI...r
-00004530: 8400 0000 7248 0000 0072 d300 0000 7259  ....rH...r....rY
-00004540: 0000 0072 9d00 0000 da1c 6765 745f 6d6f  ...r......get_mo
-00004550: 6465 6c5f 6669 656c 645f 6c6f 6f6b 7570  del_field_lookup
-00004560: 735f 7479 7065 72a0 0000 0072 0b00 0000  s_typer....r....
-00004570: da23 6765 745f 6d6f 6465 6c5f 7265 6c61  .#get_model_rela
-00004580: 7469 6f6e 7368 6970 5f6c 6f6f 6b75 7073  tionship_lookups
-00004590: 5f74 7970 6572 aa00 0000 7227 0000 0029  _typer....r'...)
-000045a0: 0e72 5d00 0000 728f 0000 0072 6f00 0000  .r]...r....ro...
-000045b0: 72d8 0000 0072 d900 0000 72da 0000 0072  r....r....r....r
-000045c0: db00 0000 72dc 0000 0072 a600 0000 5a13  ....r....r....Z.
-000045d0: 636f 6c75 6d6e 5f6c 6f6f 6b75 7073 5f74  column_lookups_t
-000045e0: 7970 6572 de00 0000 7296 0000 005a 1972  yper....r....Z.r
-000045f0: 656c 6174 696f 6e73 6869 705f 6c6f 6f6b  elationship_look
-00004600: 7570 735f 7479 7065 72df 0000 0072 2300  ups_typer....r#.
-00004610: 0000 7223 0000 0072 2400 0000 da16 6765  ..r#...r$.....ge
-00004620: 745f 6d6f 6465 6c5f 6c6f 6f6b 7570 735f  t_model_lookups_
-00004630: 7479 7065 8c02 0000 732a 0000 0000 0108  type....s*......
-00004640: 010c 0110 010c 020a 010a 0204 020c 0112  ................
-00004650: 010a 010e 0204 0110 010c 0102 0212 010c  ................
-00004660: 010e 020e 010a 017a 2d47 7261 7068 514c  .......z-GraphQL
-00004670: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
-00004680: 6765 745f 6d6f 6465 6c5f 6c6f 6f6b 7570  get_model_lookup
-00004690: 735f 7479 7065 6306 0000 0000 0000 000e  s_typec.........
-000046a0: 0000 0006 0000 0043 0000 0073 d000 0000  .......C...s....
-000046b0: 7400 7c02 6a01 6a02 8301 7d06 7400 7c03  t.|.j.j...}.t.|.
-000046c0: 6a02 8301 7d07 7c04 7228 6401 6a03 7c06  j...}.|.r(d.j.|.
-000046d0: 7c07 7c05 8303 6e0c 6402 6a03 7c06 7c07  |.|...n.d.j.|.|.
-000046e0: 7c05 8303 7d08 7c08 7c00 6a04 6b06 724a  |...}.|.|.j.k.rJ
-000046f0: 7c00 6a04 7c08 1900 5300 7405 6a06 8300  |.j.|...S.t.j...
-00004700: 7405 6a06 8300 6403 9c02 7d09 7c04 72b4  t.j...d...}.|.r.
-00004710: 7852 7c00 6a07 7c02 8301 4400 5d44 7d0a  xR|.j.|...D.]D}.
-00004720: 7c0a 6404 1900 7408 6b03 736c 7c0a 6405  |.d...t.k.sl|.d.
-00004730: 1900 7c07 6b03 728a 716c 7c0a 6406 1900  ..|.k.r.ql|.d...
-00004740: 7d0b 7c00 6a09 7c01 7c0b 7c05 6407 1700  }.|.j.|.|.|.d...
-00004750: 8303 7d0c 7c0c 8300 7c09 6408 3c00 5000  ..}.|...|.d.<.P.
-00004760: 716c 5700 740a 7c08 740b 6601 7c09 8303  qlW.t.|.t.f.|...
-00004770: 7d0d 7c0d 7c00 6a04 7c08 3c00 7c0d 5300  }.|.|.j.|.<.|.S.
-00004780: 2909 4e7a 2c4d 6f64 656c 7b7d 436f 6c75  ).Nz,Model{}Colu
-00004790: 6d6e 7b7d 4465 7074 687b 7d4e 6573 7465  mn{}Depth{}Neste
-000047a0: 644c 6f6f 6b75 7073 4669 656c 6454 7970  dLookupsFieldTyp
-000047b0: 657a 264d 6f64 656c 7b7d 436f 6c75 6d6e  ez&Model{}Column
-000047c0: 7b7d 4465 7074 687b 7d4c 6f6f 6b75 7073  {}Depth{}Lookups
-000047d0: 4669 656c 6454 7970 6529 0272 b800 0000  FieldType).r....
-000047e0: 72b9 0000 0072 7800 0000 727a 0000 0072  r....rx...rz...r
-000047f0: 7c00 0000 724a 0000 0072 a500 0000 290c  |...rJ...r....).
-00004800: 7249 0000 0072 8400 0000 7248 0000 0072  rI...r....rH...r
-00004810: d300 0000 725a 0000 0072 2e00 0000 722f  ....rZ...r....r/
-00004820: 0000 0072 a000 0000 720a 0000 0072 e600  ...r....r....r..
-00004830: 0000 72aa 0000 0072 2800 0000 290e 725d  ..r....r(...).r]
-00004840: 0000 0072 8f00 0000 726f 0000 0072 a600  ...r....ro...r..
-00004850: 0000 72d9 0000 0072 d800 0000 72da 0000  ..r....r....r...
-00004860: 0072 e100 0000 72db 0000 0072 dc00 0000  .r....r....r....
-00004870: 7296 0000 0072 ae00 0000 72e3 0000 0072  r....r....r....r
-00004880: df00 0000 7223 0000 0072 2300 0000 7224  ....r#...r#...r$
-00004890: 0000 0072 e400 0000 a902 0000 7326 0000  ...r........s&..
-000048a0: 0000 010c 010a 0112 010e 020a 010a 0306  ................
-000048b0: 010c 0304 0110 0118 0102 0208 0112 010a  ................
-000048c0: 0106 020e 010a 017a 3347 7261 7068 514c  .......z3GraphQL
-000048d0: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
-000048e0: 6765 745f 6d6f 6465 6c5f 6669 656c 645f  get_model_field_
-000048f0: 6c6f 6f6b 7570 735f 7479 7065 6306 0000  lookups_typec...
-00004900: 0000 0000 000c 0000 0005 0000 0043 0000  .............C..
-00004910: 0073 9200 0000 7400 7c02 6a01 6a02 8301  .s....t.|.j.j...
-00004920: 7d06 7400 7c03 6401 1900 8301 7d07 7c04  }.t.|.d.....}.|.
-00004930: 722a 6402 6a03 7c06 7c07 7c05 8303 6e0c  r*d.j.|.|.|...n.
-00004940: 6403 6a03 7c06 7c07 7c05 8303 7d08 7c08  d.j.|.|.|...}.|.
-00004950: 7c00 6a04 6b06 724c 7c00 6a04 7c08 1900  |.j.k.rL|.j.|...
-00004960: 5300 6404 7405 8300 6901 7d09 7c00 6a06  S.d.t...i.}.|.j.
-00004970: 7c01 7c03 6405 1900 7c05 6406 1700 8303  |.|.d...|.d.....
-00004980: 7d0a 7c0a 8300 7c09 6407 3c00 7407 7c08  }.|...|.d.<.t.|.
-00004990: 7408 6601 7c09 8303 7d0b 7c0b 7c00 6a04  t.f.|...}.|.|.j.
-000049a0: 7c08 3c00 7c0b 5300 2908 4e72 4800 0000  |.<.|.S.).NrH...
-000049b0: 7a33 4d6f 6465 6c7b 7d43 6f6c 756d 6e7b  z3Model{}Column{
-000049c0: 7d44 6570 7468 7b7d 4e65 7374 6564 4c6f  }Depth{}NestedLo
-000049d0: 6f6b 7570 7352 656c 6174 696f 6e73 6869  okupsRelationshi
-000049e0: 7054 7970 657a 2d4d 6f64 656c 7b7d 436f  pTypez-Model{}Co
-000049f0: 6c75 6d6e 7b7d 4465 7074 687b 7d4c 6f6f  lumn{}Depth{}Loo
-00004a00: 6b75 7073 5265 6c61 7469 6f6e 7368 6970  kupsRelationship
-00004a10: 5479 7065 72be 0000 0072 7c00 0000 724a  Typer....r|...rJ
-00004a20: 0000 0072 a500 0000 2909 7249 0000 0072  ...r....).rI...r
-00004a30: 8400 0000 7248 0000 0072 d300 0000 725b  ....rH...r....r[
-00004a40: 0000 0072 3f00 0000 72e6 0000 0072 aa00  ...r?...r....r..
-00004a50: 0000 7229 0000 0029 0c72 5d00 0000 728f  ..r)...).r]...r.
-00004a60: 0000 0072 6f00 0000 7296 0000 0072 d900  ...ro...r....r..
-00004a70: 0000 72d8 0000 0072 da00 0000 72e2 0000  ..r....r....r...
-00004a80: 0072 db00 0000 72dc 0000 0072 e300 0000  .r....r....r....
-00004a90: 72df 0000 0072 2300 0000 7223 0000 0072  r....r#...r#...r
-00004aa0: 2400 0000 72e5 0000 00c5 0200 0073 1800  $...r........s..
-00004ab0: 0000 0001 0c01 0c01 1201 0e02 0a01 0a03  ................
-00004ac0: 0a03 1601 0a02 0e01 0a01 7a3a 4772 6170  ..........z:Grap
-00004ad0: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
-00004ae0: 6f72 2e67 6574 5f6d 6f64 656c 5f72 656c  or.get_model_rel
-00004af0: 6174 696f 6e73 6869 705f 6c6f 6f6b 7570  ationship_lookup
-00004b00: 735f 7479 7065 6302 0000 0000 0000 0008  s_typec.........
-00004b10: 0000 0004 0000 0043 0000 0073 7a00 0000  .......C...sz...
-00004b20: 7400 7c01 6a01 6a02 8301 7d02 6401 6a03  t.|.j.j...}.d.j.
-00004b30: 7c02 8301 7d03 7c03 7c00 6a04 6b06 7230  |...}.|.|.j.k.r0
-00004b40: 7405 6a06 7c00 6a04 7c03 1900 8301 5300  t.j.|.j.|.....S.
-00004b50: 6900 7d04 7822 7c01 6a07 4400 5d18 7d05  i.}.x"|.j.D.].}.
-00004b60: 7400 7c05 6a02 8301 7d06 7408 8300 7c04  t.|.j...}.t...|.
-00004b70: 7c06 3c00 713c 5700 7409 7c03 740a 6601  |.<.q<W.t.|.t.f.
-00004b80: 7c04 8303 7d07 7c07 7c00 6a04 7c03 3c00  |...}.|.|.j.|.<.
-00004b90: 7405 6a06 7c07 8301 5300 2902 4e7a 0f4d  t.j.|...S.).Nz.M
-00004ba0: 6f64 656c 7b7d 536f 7274 5479 7065 290b  odel{}SortType).
-00004bb0: 7249 0000 0072 8400 0000 7248 0000 0072  rI...r....rH...r
-00004bc0: d300 0000 725c 0000 0072 2e00 0000 72d4  ....r\...r....r.
-00004bd0: 0000 0072 9d00 0000 722c 0000 0072 aa00  ...r....r,...r..
-00004be0: 0000 722a 0000 0029 0872 5d00 0000 726f  ..r*...).r]...ro
-00004bf0: 0000 0072 da00 0000 72db 0000 0072 dc00  ...r....r....r..
-00004c00: 0000 72a6 0000 0072 de00 0000 72df 0000  ..r....r....r...
-00004c10: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00004c20: da13 6765 745f 6d6f 6465 6c5f 736f 7274  ..get_model_sort
-00004c30: 5f74 7970 65d9 0200 0073 1600 0000 0001  _type....s......
-00004c40: 0c01 0a02 0a01 1002 0402 0c01 0a01 0e02  ................
-00004c50: 0e01 0a01 7a2a 4772 6170 6851 4c53 6368  ....z*GraphQLSch
-00004c60: 656d 6147 656e 6572 6174 6f72 2e67 6574  emaGenerator.get
-00004c70: 5f6d 6f64 656c 5f73 6f72 745f 7479 7065  _model_sort_type
-00004c80: 6302 0000 0000 0000 0006 0000 0004 0000  c...............
-00004c90: 0043 0000 0073 4800 0000 7400 7c01 6a01  .C...sH...t.|.j.
-00004ca0: 6a02 8301 7d02 6900 7d03 7822 7c01 6a03  j...}.i.}.x"|.j.
-00004cb0: 4400 5d18 7d04 7400 7c04 6a02 8301 7d05  D.].}.t.|.j...}.
-00004cc0: 7404 8300 7c03 7c05 3c00 7118 5700 7405  t...|.|.<.q.W.t.
-00004cd0: 6401 6a06 7c02 8301 7407 6601 7c03 8303  d.j.|...t.f.|...
-00004ce0: 5300 2902 4e7a 164d 6f64 656c 7b7d 5265  S.).Nz.Model{}Re
-00004cf0: 636f 7264 4174 7472 7354 7970 6529 0872  cordAttrsType).r
-00004d00: 4900 0000 7284 0000 0072 4800 0000 729d  I...r....rH...r.
-00004d10: 0000 0072 1b00 0000 72aa 0000 0072 d300  ...r....r....r..
-00004d20: 0000 722b 0000 0029 0672 5d00 0000 726f  ..r+...).r]...ro
-00004d30: 0000 0072 4800 0000 72dc 0000 0072 a600  ...rH...r....r..
-00004d40: 0000 72de 0000 0072 2300 0000 7223 0000  ..r....r#...r#..
-00004d50: 0072 2400 0000 da14 6765 745f 6d6f 6465  .r$.....get_mode
-00004d60: 6c5f 6174 7472 735f 7479 7065 ea02 0000  l_attrs_type....
-00004d70: 730c 0000 0000 010c 0104 020c 010a 010e  s...............
-00004d80: 027a 2b47 7261 7068 514c 5363 6865 6d61  .z+GraphQLSchema
-00004d90: 4765 6e65 7261 746f 722e 6765 745f 6d6f  Generator.get_mo
-00004da0: 6465 6c5f 6174 7472 735f 7479 7065 6303  del_attrs_typec.
-00004db0: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
-00004dc0: 0000 0073 6400 0000 6401 7d03 7c01 6a00  ...sd...d.}.|.j.
-00004dd0: 6401 1900 7d04 7850 7c02 4400 5d48 7d05  d...}.xP|.D.]H}.
-00004de0: 783a 7c04 6a01 6a02 4400 5d2e 7d06 7c06  x:|.j.j.D.].}.|.
-00004df0: 6a03 6a04 7c05 6b02 7222 7c03 7405 7c02  j.j.|.k.r"|.t.|.
-00004e00: 8301 6402 1800 6b02 724a 7c06 6a01 6a02  ..d...k.rJ|.j.j.
-00004e10: 5300 7c06 7d04 5000 7122 5700 7c03 6402  S.|.}.P.q"W.|.d.
-00004e20: 3700 7d03 7114 5700 6400 5300 2903 4e72  7.}.q.W.d.S.).Nr
-00004e30: 0100 0000 724a 0000 0029 06da 0a66 6965  ....rJ...)...fie
-00004e40: 6c64 5f61 7374 73da 0d73 656c 6563 7469  ld_asts..selecti
-00004e50: 6f6e 5f73 6574 da0a 7365 6c65 6374 696f  on_set..selectio
-00004e60: 6e73 7248 0000 0072 bb00 0000 7266 0000  nsrH...r....rf..
-00004e70: 0029 0772 5d00 0000 da04 696e 666f da04  .).r].....info..
-00004e80: 7061 7468 da01 695a 0d63 7572 7265 6e74  path..iZ.current
-00004e90: 5f66 6965 6c64 da09 7061 7468 5f69 7465  _field..path_ite
-00004ea0: 6dda 0973 656c 6563 7469 6f6e 7223 0000  m..selectionr#..
-00004eb0: 0072 2300 0000 7224 0000 00da 0e67 6574  .r#...r$.....get
-00004ec0: 5f73 656c 6563 7469 6f6e 73f4 0200 0073  _selections....s
-00004ed0: 1400 0000 0001 0401 0a02 0a01 0e01 0c01  ................
-00004ee0: 1001 0802 0401 0602 7a25 4772 6170 6851  ........z%GraphQ
-00004ef0: 4c53 6368 656d 6147 656e 6572 6174 6f72  LSchemaGenerator
-00004f00: 2e67 6574 5f73 656c 6563 7469 6f6e 7363  .get_selectionsc
-00004f10: 0a00 0000 0000 0000 1b00 0000 1000 0000  ................
-00004f20: 0300 0000 7350 0200 0090 0279 207c 0570  ....sP.....y |.p
-00004f30: 0a67 007d 057c 0670 1267 007d 067c 0770  .g.}.|.p.g.}.|.p
-00004f40: 1a67 007d 077c 0870 2269 007d 087c 046a  .g.}.|.p"i.}.|.j
-00004f50: 006a 0164 0183 017d 0a88 046a 027c 0464  .j.d...}...j.|.d
-00004f60: 0264 0367 0283 0270 4267 007d 0b74 0374  .d.g...pBg.}.t.t
-00004f70: 0464 0464 0584 007c 0b83 0283 017d 0c88  .d.d...|.....}..
-00004f80: 046a 027c 0464 0267 0183 0270 6667 007d  .j.|.d.g...pfg.}
-00004f90: 0d74 0374 0464 0664 0584 007c 0d83 0283  .t.t.d.d...|....
-00004fa0: 017d 0e74 0574 0487 0066 0164 0764 0584  .}.t.t...f.d.d..
-00004fb0: 0874 0688 0083 0183 0283 0189 0274 077c  .t...........t.|
-00004fc0: 0c83 0172 c464 087c 0e6b 0772 c474 0374  ...r.d.|.k.r.t.t
-00004fd0: 0864 0964 0584 0074 0487 0266 0164 0a64  .d.d...t...f.d.d
-00004fe0: 0584 087c 0c83 0283 0283 016e 0264 007d  ...|.......n.d.}
-00004ff0: 0f88 046a 097c 0a88 007c 0f83 037d 1088  ...j.|...|...}..
-00005000: 046a 0a7c 017c 1088 017c 0583 047d 1088  .j.|.|...|...}..
-00005010: 046a 0b7c 1088 017c 0983 037d 1088 046a  .j.|...|...}...j
-00005020: 0c7c 107c 0188 017c 0783 047d 1074 0388  .|.|...|...}.t..
-00005030: 046a 0d7c 107c 0883 0283 017d 1174 0e88  .j.|.|.....}.t..
-00005040: 0083 0189 0569 0089 0688 046a 0f7c 0a7c  .....i.....j.|.|
-00005050: 017c 1188 0088 017c 0683 0689 0387 0187  .|.....|........
-00005060: 0387 0487 0587 0666 0564 0b64 0c84 087d  .......f.d.d...}
-00005070: 1264 0274 0374 047c 127c 1183 0283 0169  .d.t.t.|.|.....i
-00005080: 017d 1388 046a 027c 0464 0d67 0183 0290  .}...j.|.d.g....
-00005090: 0170 6c67 007d 1474 0374 0464 0e64 0584  .plg.}.t.t.d.d..
-000050a0: 007c 1483 0283 017d 1574 077c 1583 0190  .|.....}.t.|....
-000050b0: 0272 2088 046a 107c 0883 017d 167c 086a  .r ..j.|...}.|.j
-000050c0: 0164 0f83 017d 177c 086a 0164 1083 017d  .d...}.|.j.d...}
-000050d0: 187c 167c 177c 1864 119c 037c 1364 0d3c  .|.|.|.d...|.d.<
-000050e0: 0064 127c 156b 0690 0173 cc64 137c 156b  .d.|.k...s.d.|.k
-000050f0: 0690 0272 2074 117c 0a7c 1083 027d 197c  ...r t.|.|...}.|
-00005100: 197c 1364 0d19 0064 123c 007c 1764 006b  .|.d...d.<.|.d.k
-00005110: 0990 0272 027c 177c 1617 007c 196b 007c  ...r.|.|...|.k.|
-00005120: 1364 0d19 0064 133c 006e 1e7c 1864 006b  .d...d.<.n.|.d.k
-00005130: 0990 0272 207c 187c 1614 007c 196b 007c  ...r |.|...|.k.|
-00005140: 1364 0d19 0064 133c 007c 1353 0004 0074  .d...d.<.|.S...t
-00005150: 126b 0a90 0272 4a01 007d 1a01 007a 0a7c  .k...rJ..}...z.|
-00005160: 1a82 0157 0059 0064 0064 007d 1a7e 1a58  ...W.Y.d.d.}.~.X
-00005170: 006e 0258 0064 0053 0029 144e 726c 0000  .n.X.d.S.).Nrl..
-00005180: 00da 0464 6174 6172 dc00 0000 6301 0000  ...datar....c...
-00005190: 0000 0000 0001 0000 0001 0000 0053 0000  .............S..
-000051a0: 0073 0800 0000 7c00 6a00 6a01 5300 2901  .s....|.j.j.S.).
-000051b0: 4e29 0272 4800 0000 72bb 0000 0029 0172  N).rH...r....).r
-000051c0: 4b00 0000 7223 0000 0072 2300 0000 7224  K...r#...r#...r$
-000051d0: 0000 0072 4c00 0000 0d03 0000 7300 0000  ...rL.......s...
-000051e0: 007a 3b47 7261 7068 514c 5363 6865 6d61  .z;GraphQLSchema
-000051f0: 4765 6e65 7261 746f 722e 7265 736f 6c76  Generator.resolv
-00005200: 655f 6d6f 6465 6c5f 6c69 7374 2e3c 6c6f  e_model_list.<lo
-00005210: 6361 6c73 3e2e 3c6c 616d 6264 613e 6301  cals>.<lambda>c.
-00005220: 0000 0000 0000 0001 0000 0001 0000 0053  ...............S
-00005230: 0000 0073 0800 0000 7c00 6a00 6a01 5300  ...s....|.j.j.S.
-00005240: 2901 4e29 0272 4800 0000 72bb 0000 0029  ).N).rH...r....)
-00005250: 0172 4b00 0000 7223 0000 0072 2300 0000  .rK...r#...r#...
-00005260: 7224 0000 0072 4c00 0000 0f03 0000 7300  r$...rL.......s.
-00005270: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
-00005280: 0400 0000 1300 0000 7312 0000 0074 007c  ........s....t.|
-00005290: 0083 0174 0188 007c 0083 0267 0253 0029  ...t...|...g.S.)
-000052a0: 014e 2902 7249 0000 0072 6800 0000 2901  .N).rI...rh...).
-000052b0: 724b 0000 0029 0172 6d00 0000 7223 0000  rK...).rm...r#..
-000052c0: 0072 2400 0000 724c 0000 0010 0300 0073  .r$...rL.......s
-000052d0: 0000 0000 da08 616c 6c41 7474 7273 6301  ......allAttrsc.
-000052e0: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
-000052f0: 0000 0073 0800 0000 7c00 6400 6b09 5300  ...s....|.d.k.S.
-00005300: 2901 4e72 2300 0000 2901 724b 0000 0072  ).Nr#...).rK...r
-00005310: 2300 0000 7223 0000 0072 2400 0000 724c  #...r#...r$...rL
-00005320: 0000 0011 0300 0073 0000 0000 6301 0000  .......s....c...
-00005330: 0000 0000 0001 0000 0002 0000 0013 0000  ................
-00005340: 0073 0a00 0000 8800 6a00 7c00 8301 5300  .s......j.|...S.
-00005350: 2901 4e29 0172 8500 0000 2901 724b 0000  ).N).r....).rK..
-00005360: 0029 01da 0b6d 6f64 656c 5f61 7474 7273  .)...model_attrs
-00005370: 7223 0000 0072 2400 0000 724c 0000 0011  r#...r$...rL....
-00005380: 0300 0073 0000 0000 6301 0000 0000 0000  ...s....c.......
-00005390: 0004 0000 0007 0000 0013 0000 0073 6600  .............sf.
-000053a0: 0000 7400 8800 7401 8302 7214 7402 8800  ..t...t...r.t...
-000053b0: 8301 7d01 6e18 7402 7403 8700 6601 6401  ..}.n.t.t...f.d.
-000053c0: 6402 8408 8801 6a04 8302 8301 7d01 8804  d.....j.....}...
-000053d0: 7c01 8805 6403 8d02 7d02 7c02 6a05 7d03  |...d...}.|.j.}.
-000053e0: 7406 7c03 8301 7d03 7c03 7c03 7407 7403  t.|...}.|.|.t.t.
-000053f0: 8700 8703 6602 6404 6402 8408 8802 8302  ....f.d.d.......
-00005400: 8301 6405 9c03 5300 2906 4e63 0100 0000  ..d...S.).Nc....
-00005410: 0000 0000 0100 0000 0400 0000 1300 0000  ................
-00005420: 7316 0000 0074 007c 006a 0183 0174 0288  s....t.|.j...t..
-00005430: 007c 006a 0183 0266 0253 0029 014e 2903  .|.j...f.S.).N).
-00005440: 7249 0000 0072 4800 0000 7268 0000 0029  rI...rH...rh...)
-00005450: 0172 4b00 0000 2901 da03 726f 7772 2300  .rK...)...rowr#.
-00005460: 0000 7224 0000 0072 4c00 0000 2503 0000  ..r$...rL...%...
-00005470: 7300 0000 007a 5b47 7261 7068 514c 5363  s....z[GraphQLSc
-00005480: 6865 6d61 4765 6e65 7261 746f 722e 7265  hemaGenerator.re
-00005490: 736f 6c76 655f 6d6f 6465 6c5f 6c69 7374  solve_model_list
-000054a0: 2e3c 6c6f 6361 6c73 3e2e 6d61 705f 7175  .<locals>.map_qu
-000054b0: 6572 7973 6574 5f70 6167 655f 6974 656d  eryset_page_item
-000054c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-000054d0: 613e 2902 72b0 0000 00da 0763 6f6e 7465  a>).r......conte
-000054e0: 7874 6301 0000 0000 0000 0001 0000 0005  xtc.............
-000054f0: 0000 0013 0000 0073 1400 0000 8801 6a00  .......s......j.
-00005500: 7c00 8700 6601 6401 6402 8408 8302 5300  |...f.d.d.....S.
-00005510: 2903 4e63 0100 0000 0000 0000 0100 0000  ).Nc............
-00005520: 0200 0000 1300 0000 7308 0000 007c 0088  ........s....|..
-00005530: 006b 0253 0029 014e 7223 0000 0029 0172  .k.S.).Nr#...).r
-00005540: b000 0000 2901 72f5 0000 0072 2300 0000  ....).r....r#...
-00005550: 7224 0000 0072 4c00 0000 2f03 0000 7300  r$...rL.../...s.
-00005560: 0000 007a 6d47 7261 7068 514c 5363 6865  ...zmGraphQLSche
-00005570: 6d61 4765 6e65 7261 746f 722e 7265 736f  maGenerator.reso
-00005580: 6c76 655f 6d6f 6465 6c5f 6c69 7374 2e3c  lve_model_list.<
-00005590: 6c6f 6361 6c73 3e2e 6d61 705f 7175 6572  locals>.map_quer
-000055a0: 7973 6574 5f70 6167 655f 6974 656d 2e3c  yset_page_item.<
-000055b0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-000055c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-000055d0: 613e 2901 72c8 0000 0029 0172 4b00 0000  a>).r....).rK...
-000055e0: 2902 72f5 0000 0072 5d00 0000 7223 0000  ).r....r]...r#..
-000055f0: 0072 2400 0000 724c 0000 002f 0300 0073  .r$...rL.../...s
-00005600: 0000 0000 2903 72dc 0000 0072 f300 0000  ....).r....r....
-00005610: 7212 0000 0029 08da 0a69 7369 6e73 7461  r....)...isinsta
-00005620: 6e63 6572 0800 0000 724f 0000 0072 4d00  ncer....rO...rM.
-00005630: 0000 729d 0000 005a 1372 6570 7265 7365  ..r....Z.represe
-00005640: 6e74 6174 696f 6e5f 6461 7461 7252 0000  ntation_datarR..
-00005650: 0072 c300 0000 2904 72f5 0000 0072 f200  .r....).r....r..
-00005660: 0000 5a0a 7365 7269 616c 697a 6572 da0a  ..Z.serializer..
-00005670: 7365 7269 616c 697a 6564 2905 726f 0000  serialized).ro..
-00005680: 00da 1571 7565 7279 7365 745f 7061 6765  ...queryset_page
-00005690: 5f6c 6f6f 6b75 7073 725d 0000 00da 1073  _lookupsr].....s
-000056a0: 6572 6961 6c69 7a65 725f 636c 6173 73da  erializer_class.
-000056b0: 1273 6572 6961 6c69 7a65 725f 636f 6e74  .serializer_cont
-000056c0: 6578 7429 0172 f500 0000 7224 0000 00da  ext).r....r$....
-000056d0: 166d 6170 5f71 7565 7279 7365 745f 7061  .map_queryset_pa
-000056e0: 6765 5f69 7465 6d21 0300 0073 1600 0000  ge_item!...s....
-000056f0: 0001 0a01 0a02 1802 0c01 0601 0803 0201  ................
-00005700: 0201 0401 0c01 7a49 4772 6170 6851 4c53  ......zIGraphQLS
-00005710: 6368 656d 6147 656e 6572 6174 6f72 2e72  chemaGenerator.r
-00005720: 6573 6f6c 7665 5f6d 6f64 656c 5f6c 6973  esolve_model_lis
-00005730: 742e 3c6c 6f63 616c 733e 2e6d 6170 5f71  t.<locals>.map_q
-00005740: 7565 7279 7365 745f 7061 6765 5f69 7465  ueryset_page_ite
-00005750: 6d72 cf00 0000 6301 0000 0000 0000 0001  mr....c.........
-00005760: 0000 0001 0000 0053 0000 0073 0800 0000  .......S...s....
-00005770: 7c00 6a00 6a01 5300 2901 4e29 0272 4800  |.j.j.S.).N).rH.
-00005780: 0000 72bb 0000 0029 0172 4b00 0000 7223  ..r....).rK...r#
-00005790: 0000 0072 2300 0000 7224 0000 0072 4c00  ...r#...r$...rL.
-000057a0: 0000 3903 0000 7300 0000 0072 3400 0000  ..9...s....r4...
-000057b0: 7233 0000 0029 0372 3500 0000 7234 0000  r3...).r5...r4..
-000057c0: 0072 3300 0000 723a 0000 0072 4300 0000  .r3...r:...rC...
-000057d0: 2913 72f6 0000 0072 8500 0000 72f1 0000  ).r....r....r...
-000057e0: 0072 c300 0000 724d 0000 0072 4f00 0000  .r....rM...rO...
-000057f0: da03 6469 7272 6600 0000 7269 0000 0072  ..dirrf...ri...r
-00005800: 7100 0000 72a8 0000 0072 1500 0000 72cd  q...r....r....r.
-00005810: 0000 0072 d100 0000 7216 0000 0072 b700  ...r....r....r..
-00005820: 0000 72d0 0000 0072 1c00 0000 da09 4578  ..r....r......Ex
-00005830: 6365 7074 696f 6e29 1b72 5d00 0000 728f  ception).r]...r.
-00005840: 0000 0072 6d00 0000 726f 0000 0072 ec00  ...rm...ro...r..
-00005850: 0000 72ab 0000 0072 1200 0000 72cc 0000  ..r....r....r...
-00005860: 0072 cf00 0000 72b2 0000 0072 6c00 0000  .r....r....rl...
-00005870: 5a10 6669 656c 645f 7365 6c65 6374 696f  Z.field_selectio
-00005880: 6e73 da0b 6669 656c 645f 6e61 6d65 735a  ns..field_namesZ
-00005890: 0f64 6174 615f 7365 6c65 6374 696f 6e73  .data_selections
-000058a0: 5a0a 6461 7461 5f6e 616d 6573 726e 0000  Z.data_namesrn..
-000058b0: 0072 7000 0000 5a0d 7175 6572 7973 6574  .rp...Z.queryset
-000058c0: 5f70 6167 6572 fc00 0000 7291 0000 005a  _pager....r....Z
-000058d0: 1570 6167 696e 6174 696f 6e5f 7365 6c65  .pagination_sele
-000058e0: 6374 696f 6e73 5a10 7061 6769 6e61 7469  ctionsZ.paginati
-000058f0: 6f6e 5f6e 616d 6573 7235 0000 0072 3400  on_namesr5...r4.
-00005900: 0000 7233 0000 0072 3a00 0000 da01 6572  ..r3...r:.....er
-00005910: 2300 0000 2907 726d 0000 0072 6f00 0000  #...).rm...ro...
-00005920: 72f4 0000 0072 f900 0000 725d 0000 0072  r....r....r]...r
-00005930: fa00 0000 72fb 0000 0072 2400 0000 da12  ....r....r$.....
-00005940: 7265 736f 6c76 655f 6d6f 6465 6c5f 6c69  resolve_model_li
-00005950: 7374 0303 0000 7352 0000 0000 0104 0108  st....sR........
-00005960: 0108 0108 0108 020c 0214 0112 0112 0112  ................
-00005970: 011a 0234 020e 0210 010e 0110 0210 0208  ...4............
-00005980: 0104 0214 0214 1412 0314 0112 020a 010a  ................
-00005990: 010a 010a 0302 0102 010c 0314 010a 010c  ................
-000059a0: 020a 0116 010a 0114 0204 0112 017a 2947  .............z)G
-000059b0: 7261 7068 514c 5363 6865 6d61 4765 6e65  raphQLSchemaGene
-000059c0: 7261 746f 722e 7265 736f 6c76 655f 6d6f  rator.resolve_mo
-000059d0: 6465 6c5f 6c69 7374 6304 0000 0000 0000  del_listc.......
-000059e0: 0010 0000 0009 0000 0003 0000 0073 5401  .............sT.
-000059f0: 0000 7400 7c01 8301 8900 7401 8800 6a02  ..t.|.....t...j.
-00005a00: 8301 6401 6b02 721e 7403 6402 8301 8201  ..d.k.r.t.d.....
-00005a10: 6900 7d04 8802 6a04 7c01 8800 7c02 8303  i.}...j.|...|...
-00005a20: 8802 5f05 8802 6a06 8802 6a05 8301 8802  .._...j...j.....
-00005a30: 5f07 9001 7800 8800 6a02 4400 5df6 7d05  _...x...j.D.].}.
-00005a40: 7408 7c05 8301 7d06 7c06 6a09 6401 1900  t.|...}.|.j.d...
-00005a50: 7d07 740a 8800 6a0b 7c07 8302 7d08 740c  }.t...j.|...}.t.
-00005a60: 7c08 8301 7d08 8802 6a0d 8800 7c06 8302  |...}...j...|...
-00005a70: 7d09 8802 6a0e 8800 7c06 8302 7d0a 8802  }...j...|...}...
-00005a80: 6a0f 7c06 8301 7d0b 8802 6a10 7c06 8301  j.|...}...j.|...
-00005a90: 7d0c 7411 6403 6a12 7c08 8301 7413 6a14  }.t.d.j.|...t.j.
-00005aa0: 6601 7413 6a15 7c0c 8301 7413 6a15 7416  f.t.j.|...t.j.t.
-00005ab0: 8301 7413 6a17 7416 8301 6404 9c03 8303  ..t.j.t...d.....
-00005ac0: 7d0d 7411 6405 6a12 7c08 8301 7413 6a14  }.t.d.j.|...t.j.
-00005ad0: 6601 7413 6a17 7c0d 8301 7413 6a15 7418  f.t.j.|...t.j.t.
-00005ae0: 8301 6406 9c02 8303 7d0e 8700 8701 8702  ..d.....}.......
-00005af0: 6603 6407 6408 8408 7d0f 7413 6a15 7c0e  f.d.d...}.t.j.|.
-00005b00: 7c09 7413 6a17 7c0a 8301 7c0b 7419 8300  |.t.j.|...|.t...
-00005b10: 741a 8300 6409 8d06 7c04 7c08 3c00 7c0f  t...d...|.|.<.|.
-00005b20: 7c05 7c06 8302 7c04 640a 6a12 7c08 8301  |.|...|.d.j.|...
-00005b30: 3c00 714a 5700 7411 640b 7413 6a14 6601  <.qJW.t.d.t.j.f.
-00005b40: 7c04 8303 5300 290c 4e72 0100 0000 7a0f  |...S.).Nr....z.
-00005b50: 4e6f 2074 6162 6c65 7320 666f 756e 647a  No tables foundz
-00005b60: 104d 6f64 656c 7b7d 4d6f 6465 6c54 7970  .Model{}ModelTyp
-00005b70: 6529 0372 dc00 0000 72f3 0000 0072 1200  e).r....r....r..
-00005b80: 0000 7a14 4d6f 6465 6c7b 7d4d 6f64 656c  ..z.Model{}Model
-00005b90: 4c69 7374 5479 7065 2902 72f2 0000 0072  ListType).r....r
-00005ba0: cf00 0000 6302 0000 0000 0000 0003 0000  ....c...........
-00005bb0: 0006 0000 0013 0000 0073 1a00 0000 6403  .........s....d.
-00005bc0: 8702 8700 8703 8701 8704 6605 6401 6402  ..........f.d.d.
-00005bd0: 8409 7d02 7c02 5300 2904 4e63 0700 0000  ..}.|.S.).Nc....
-00005be0: 0000 0000 0800 0000 0b00 0000 1300 0000  ................
-00005bf0: 733c 0000 007c 016a 006a 0164 0183 017d  s<...|.j.j.d...}
-00005c00: 0788 0264 006b 0972 2088 027c 0788 0364  ...d.k.r ..|...d
-00005c10: 028d 0201 0088 046a 0288 0088 0188 037c  .......j.......|
-00005c20: 017c 027c 037c 047c 057c 0664 038d 0953  .|.|.|.|.|.d...S
-00005c30: 0029 044e 726c 0000 0029 0272 6c00 0000  .).Nrl...).rl...
-00005c40: 726f 0000 0029 0572 ab00 0000 7212 0000  ro...).r....r...
-00005c50: 0072 cc00 0000 72cf 0000 0072 b200 0000  .r....r....r....
-00005c60: 2903 72f6 0000 0072 8500 0000 7201 0100  ).r....r....r...
-00005c70: 0029 08da 0670 6172 656e 7472 ec00 0000  .)...parentr....
-00005c80: 72ab 0000 0072 1200 0000 72cc 0000 0072  r....r....r....r
-00005c90: cf00 0000 72b2 0000 0072 6c00 0000 2905  ....r....rl...).
-00005ca0: 728f 0000 0072 6d00 0000 da0e 6265 666f  r....rm.....befo
-00005cb0: 7265 5f72 6573 6f6c 7665 726f 0000 0072  re_resolvero...r
-00005cc0: 5d00 0000 7223 0000 0072 2400 0000 da08  ]...r#...r$.....
-00005cd0: 7265 736f 6c76 6572 7303 0000 731a 0000  resolvers...s...
-00005ce0: 0000 010c 0208 010c 0204 0102 0102 0102  ................
-00005cf0: 0102 0102 0102 0102 0102 017a 5547 7261  ...........zUGra
-00005d00: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
-00005d10: 746f 722e 6765 745f 7175 6572 795f 7479  tor.get_query_ty
-00005d20: 7065 2e3c 6c6f 6361 6c73 3e2e 6372 6561  pe.<locals>.crea
-00005d30: 7465 5f6c 6973 745f 7265 736f 6c76 6572  te_list_resolver
-00005d40: 2e3c 6c6f 6361 6c73 3e2e 7265 736f 6c76  .<locals>.resolv
-00005d50: 6572 2905 4e4e 4e4e 4e72 2300 0000 2903  er).NNNNNr#...).
-00005d60: 726d 0000 0072 6f00 0000 7204 0100 0029  rm...ro...r....)
-00005d70: 0372 8f00 0000 7203 0100 0072 5d00 0000  .r....r....r]...
-00005d80: 2902 726d 0000 0072 6f00 0000 7224 0000  ).rm...ro...r$..
-00005d90: 00da 1463 7265 6174 655f 6c69 7374 5f72  ...create_list_r
-00005da0: 6573 6f6c 7665 7272 0300 0073 0400 0000  esolverr...s....
-00005db0: 0001 1611 7a43 4772 6170 6851 4c53 6368  ....zCGraphQLSch
-00005dc0: 656d 6147 656e 6572 6174 6f72 2e67 6574  emaGenerator.get
-00005dd0: 5f71 7565 7279 5f74 7970 652e 3c6c 6f63  _query_type.<loc
-00005de0: 616c 733e 2e63 7265 6174 655f 6c69 7374  als>.create_list
-00005df0: 5f72 6573 6f6c 7665 7229 0572 ab00 0000  _resolver).r....
-00005e00: 7212 0000 0072 cc00 0000 72cf 0000 0072  r....r....r....r
-00005e10: b200 0000 7a0a 7265 736f 6c76 655f 7b7d  ....z.resolve_{}
-00005e20: da05 5175 6572 7929 1b72 0d00 0000 7266  ..Query).r....rf
-00005e30: 0000 0072 8300 0000 72fe 0000 0072 9800  ...r....r....r..
-00005e40: 0000 7254 0000 0072 9c00 0000 7255 0000  ..rT...r....rU..
-00005e50: 0072 0500 0000 7267 0000 0072 1100 0000  .r....rg...r....
-00005e60: 7277 0000 0072 4900 0000 72d7 0000 0072  rw...rI...r....r
-00005e70: e600 0000 72e7 0000 0072 e800 0000 72aa  ....r....r....r.
-00005e80: 0000 0072 d300 0000 722e 0000 00da 0a4f  ...r....r......O
-00005e90: 626a 6563 7454 7970 65da 0546 6965 6c64  bjectType..Field
-00005ea0: 721b 0000 0072 d400 0000 7242 0000 0072  r....r....rB...r
-00005eb0: 3100 0000 7236 0000 0029 1072 5d00 0000  1...r6...).r]...
-00005ec0: 726c 0000 0072 9000 0000 7203 0100 005a  rl...r....r....Z
-00005ed0: 0b71 7565 7279 5f61 7474 7273 726d 0000  .query_attrsrm..
-00005ee0: 0072 6f00 0000 7294 0000 0072 4800 0000  .ro...r....rH...
-00005ef0: 5a0b 4669 6c74 6572 7354 7970 655a 0b4c  Z.FiltersTypeZ.L
-00005f00: 6f6f 6b75 7073 5479 7065 5a08 536f 7274  ookupsTypeZ.Sort
-00005f10: 5479 7065 722b 0000 005a 094d 6f64 656c  Typer+...Z.Model
-00005f20: 5479 7065 5a0d 4d6f 6465 6c4c 6973 7454  TypeZ.ModelListT
-00005f30: 7970 6572 0501 0000 7223 0000 0029 0372  yper....r#...).r
-00005f40: 8f00 0000 7203 0100 0072 5d00 0000 7224  ....r....r]...r$
-00005f50: 0000 00da 0e67 6574 5f71 7565 7279 5f74  .....get_query_t
-00005f60: 7970 6553 0300 0073 4000 0000 0001 0802  ypeS...s@.......
-00005f70: 0e01 0802 0402 1001 0e02 0e01 0801 0a01  ................
-00005f80: 0c01 0802 0c01 0c01 0a01 0a01 1001 0801  ................
-00005f90: 0801 1002 1001 0801 1003 1014 0401 0201  ................
-00005fa0: 0201 0801 0201 0401 0e02 1802 7a25 4772  ............z%Gr
-00005fb0: 6170 6851 4c53 6368 656d 6147 656e 6572  aphQLSchemaGener
-00005fc0: 6174 6f72 2e67 6574 5f71 7565 7279 5f74  ator.get_query_t
-00005fd0: 7970 6563 0400 0000 0000 0000 0500 0000  ypec............
-00005fe0: 0400 0000 4300 0000 731c 0000 007c 006a  ....C...s....|.j
-00005ff0: 007c 017c 027c 0383 037d 0474 016a 027c  .|.|.|...}.t.j.|
-00006000: 0464 0164 028d 0253 0029 034e 4629 0272  .d.d...S.).NF).r
-00006010: 3800 0000 5a0e 6175 746f 5f63 616d 656c  8...Z.auto_camel
-00006020: 6361 7365 2903 7209 0100 0072 2e00 0000  case).r....r....
-00006030: 5a06 5363 6865 6d61 2905 725d 0000 0072  Z.Schema).r]...r
-00006040: 6c00 0000 7290 0000 0072 0301 0000 7206  l...r....r....r.
-00006050: 0100 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00006060: 0000 da0a 6765 745f 7363 6865 6d61 9203  ....get_schema..
-00006070: 0000 7304 0000 0000 010e 017a 2147 7261  ..s........z!Gra
-00006080: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
-00006090: 746f 722e 6765 745f 7363 6865 6d61 2901  tor.get_schema).
-000060a0: 4e29 024e 4629 014e 2901 724a 0000 0029  N).NF).N).rJ...)
-000060b0: 0172 4a00 0000 2901 724a 0000 0029 0172  .rJ...).rJ...).r
-000060c0: 4a00 0000 2901 724a 0000 0029 0172 4a00  J...).rJ...).rJ.
-000060d0: 0000 2905 4e4e 4e4e 4e29 014e 2901 4e29  ..).NNNNN).N).N)
-000060e0: 2072 2000 0000 7221 0000 0072 2200 0000   r ...r!...r"...
-000060f0: 725e 0000 0072 7100 0000 7298 0000 0072  r^...rq...r....r
-00006100: 9c00 0000 729f 0000 0072 a000 0000 72a1  ....r....r....r.
-00006110: 0000 0072 a200 0000 72a8 0000 0072 1500  ...r....r....r..
-00006120: 0000 72b7 0000 0072 b300 0000 72c8 0000  ..r....r....r...
-00006130: 0072 ca00 0000 72cd 0000 0072 d000 0000  .r....r....r....
-00006140: 72d1 0000 0072 d700 0000 72d5 0000 0072  r....r....r....r
-00006150: d600 0000 72e6 0000 0072 e400 0000 72e5  ....r....r....r.
-00006160: 0000 0072 e700 0000 72e8 0000 0072 f100  ...r....r....r..
-00006170: 0000 7201 0100 0072 0901 0000 720a 0100  ..r....r....r...
-00006180: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
-00006190: 7224 0000 0072 5300 0000 6600 0000 733a  r$...rS...f...s:
-000061a0: 0000 0008 0108 0b0a 1608 6b08 0908 0608  ..........k.....
-000061b0: 0408 0408 040a 5608 0708 1008 6f0a 2408  ......V.....o.$.
-000061c0: 0e08 1108 0308 0c0a 1f0a 1f0a 120a 1d0a  ................
-000061d0: 1c0a 1408 1108 0a08 0f0a 500a 3f72 5300  ..........P.?rS.
-000061e0: 0000 2944 7246 0000 0072 2e00 0000 5a2e  ..)DrF...r....Z.
-000061f0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00006200: 6d6f 6465 6c73 2e6d 6f64 656c 5f72 656c  models.model_rel
-00006210: 6174 696f 6e5f 6f76 6572 7269 6465 7202  ation_overrider.
-00006220: 0000 00da 156a 6574 5f62 7269 6467 655f  .....jet_bridge_
-00006230: 6261 7365 2e73 746f 7265 7203 0000 005a  base.storer....Z
-00006240: 1f6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00006250: 2e75 7469 6c73 2e72 656c 6174 696f 6e73  .utils.relations
-00006260: 7204 0000 00da 0a73 716c 616c 6368 656d  r......sqlalchem
-00006270: 7972 0500 0000 7206 0000 0072 0700 0000  yr....r....r....
-00006280: 5a11 7371 6c61 6c63 6865 6d79 2e65 6e67  Z.sqlalchemy.eng
-00006290: 696e 6572 0800 0000 da16 7371 6c61 6c63  iner......sqlalc
-000062a0: 6865 6d79 2e65 7874 2e61 7574 6f6d 6170  hemy.ext.automap
-000062b0: 7209 0000 00da 0e73 716c 616c 6368 656d  r......sqlalchem
-000062c0: 792e 6f72 6d72 0a00 0000 720b 0000 0072  y.ormr....r....r
-000062d0: 0c00 0000 da12 6a65 745f 6272 6964 6765  ......jet_bridge
-000062e0: 5f62 6173 652e 6462 720d 0000 0072 0e00  _base.dbr....r..
-000062f0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00006300: 005a 176a 6574 5f62 7269 6467 655f 6261  .Z.jet_bridge_ba
-00006310: 7365 2e66 696c 7465 7273 7212 0000 005a  se.filtersr....Z
-00006320: 2a6a 6574 5f62 7269 6467 655f 6261 7365  *jet_bridge_base
-00006330: 2e66 696c 7465 7273 2e66 696c 7465 725f  .filters.filter_
-00006340: 666f 725f 6462 6669 656c 6472 1300 0000  for_dbfieldr....
-00006350: 5a23 6a65 745f 6272 6964 6765 5f62 6173  Z#jet_bridge_bas
-00006360: 652e 6669 6c74 6572 732e 6d6f 6465 6c5f  e.filters.model_
-00006370: 6772 6f75 7072 1400 0000 5a24 6a65 745f  groupr....Z$jet_
-00006380: 6272 6964 6765 5f62 6173 652e 6669 6c74  bridge_base.filt
-00006390: 6572 732e 6d6f 6465 6c5f 7365 6172 6368  ers.model_search
-000063a0: 7215 0000 005a 216a 6574 5f62 7269 6467  r....Z!jet_bridg
-000063b0: 655f 6261 7365 2e73 6572 6961 6c69 7a65  e_base.serialize
-000063c0: 7273 2e6d 6f64 656c 7216 0000 00da 1c6a  rs.modelr......j
-000063d0: 6574 5f62 7269 6467 655f 6261 7365 2e75  et_bridge_base.u
-000063e0: 7469 6c73 2e63 6f6d 6d6f 6e72 1700 0000  tils.commonr....
-000063f0: 7218 0000 0072 1900 0000 721a 0000 005a  r....r....r....Z
-00006400: 196a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00006410: 2e75 7469 6c73 2e67 716c 721b 0000 00da  .utils.gqlr.....
-00006420: 1e6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00006430: 2e75 7469 6c73 2e71 7565 7279 7365 7472  .utils.querysetr
-00006440: 1c00 0000 721d 0000 0072 1e00 0000 5a0f  ....r....r....Z.
-00006450: 496e 7075 744f 626a 6563 7454 7970 6572  InputObjectTyper
-00006460: 1f00 0000 7225 0000 0072 2600 0000 7227  ....r%...r&...r'
-00006470: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
-00006480: 0000 7207 0100 0072 2b00 0000 722c 0000  ..r....r+...r,..
-00006490: 0072 3100 0000 7236 0000 00da 0445 6e75  .r1...r6.....Enu
-000064a0: 6d72 3900 0000 723f 0000 0072 4200 0000  mr9...r?...rB...
-000064b0: 7249 0000 0072 5200 0000 da06 6f62 6a65  rI...rR.....obje
-000064c0: 6374 7253 0000 0072 2300 0000 7223 0000  ctrS...r#...r#..
-000064d0: 0072 2300 0000 7224 0000 00da 083c 6d6f  .r#...r$.....<mo
-000064e0: 6475 6c65 3e01 0000 0073 4400 0000 0801  dule>....sD.....
-000064f0: 0801 0c01 0c01 0c01 1401 0c01 0c01 1402  ................
-00006500: 1c01 0c01 0c01 0c01 0c01 0c01 1801 0c01  ................
-00006510: 1403 1204 1204 1204 1204 1204 1204 1204  ................
-00006520: 1204 1204 1206 1204 1208 1205 1208 0808  ................
-00006530: 0805                                     ..
+00001170: 0000 0000 0000 0900 0000 0500 0000 0300  ................
+00001180: 0000 73c8 0000 0074 007c 0283 017d 047c  ..s....t.|...}.|
+00001190: 046a 017d 057c 0372 5874 0274 0364 0164  .j.}.|.rXt.t.d.d
+000011a0: 0284 007c 0383 0283 0189 0074 0274 0487  ...|.......t.t..
+000011b0: 0066 0164 0364 0284 087c 0583 0283 017d  .f.d.d...|.....}
+000011c0: 0674 057c 0683 0172 4a7c 067c 0395 027d  .t.|...rJ|.|...}
+000011d0: 037c 016a 066a 077c 038e 007d 076e 0c7c  .|.j.j.|...}.n.|
+000011e0: 016a 066a 077c 0283 017d 0774 007c 0283  .j.j.|...}.t.|..
+000011f0: 017d 0474 057c 046a 0883 0172 8874 097c  .}.t.|.j...r.t.|
+00001200: 046a 0864 0419 0064 0564 0683 036e 0264  .j.d...d.d...n.d
+00001210: 007d 087c 0872 a67c 076a 047c 046a 0164  .}.|.r.|.j.|.j.d
+00001220: 0419 006a 0a64 0083 0183 017d 077c 080c  ...j.d.....}.|..
+00001230: 0072 c474 0b7c 016a 0683 0164 096b 0672  .r.t.|.j...d.k.r
+00001240: c47c 076a 0c7c 058e 007d 077c 0753 0029  .|.j.|...}.|.S.)
+00001250: 0a4e 6301 0000 0000 0000 0001 0000 0001  .Nc.............
+00001260: 0000 0053 0000 0073 0600 0000 7c00 6a00  ...S...s....|.j.
+00001270: 5300 2901 4e29 0172 4800 0000 2901 724b  S.).N).rH...).rK
+00001280: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00001290: 0000 724c 0000 0077 0000 0073 0000 0000  ..rL...w...s....
+000012a0: 7a35 4772 6170 6851 4c53 6368 656d 6147  z5GraphQLSchemaG
+000012b0: 656e 6572 6174 6f72 2e67 6574 5f71 7565  enerator.get_que
+000012c0: 7279 7365 742e 3c6c 6f63 616c 733e 2e3c  ryset.<locals>.<
+000012d0: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
+000012e0: 0100 0000 0200 0000 1300 0000 730a 0000  ............s...
+000012f0: 007c 006a 0088 006b 0753 0029 014e 2901  .|.j...k.S.).N).
+00001300: 7248 0000 0029 0172 4b00 0000 2901 da11  rH...).rK...)...
+00001310: 6f6e 6c79 5f63 6f6c 756d 6e73 5f6e 616d  only_columns_nam
+00001320: 6572 2300 0000 7224 0000 0072 4c00 0000  er#...r$...rL...
+00001330: 7800 0000 7300 0000 0072 0100 0000 da0f  x...s....r......
+00001340: 5f5f 6a65 745f 6175 746f 5f70 6b5f 5f46  __jet_auto_pk__F
+00001350: da0a 706f 7374 6772 6573 716c da05 6d79  ..postgresql..my
+00001360: 7371 6c29 0272 6100 0000 7262 0000 0029  sql).ra...rb...)
+00001370: 0d72 0200 0000 da0b 7072 696d 6172 795f  .r......primary_
+00001380: 6b65 79da 046c 6973 7472 4d00 0000 da06  key..listrM.....
+00001390: 6669 6c74 6572 da03 6c65 6eda 0773 6573  filter..len..ses
+000013a0: 7369 6f6e 7238 0000 00da 0674 6162 6c65  sionr8.....table
+000013b0: 73da 0767 6574 6174 7472 da05 6973 6e6f  s..getattr..isno
+000013c0: 7472 1d00 0000 da08 6772 6f75 705f 6279  tr......group_by
+000013d0: 2909 725d 0000 00da 0772 6571 7565 7374  ).r].....request
+000013e0: da05 4d6f 6465 6cda 0c6f 6e6c 795f 636f  ..Model..only_co
+000013f0: 6c75 6d6e 73da 066d 6170 7065 72da 0370  lumns..mapper..p
+00001400: 6b73 5a0b 6d69 7373 696e 675f 706b 73da  ksZ.missing_pks.
+00001410: 0871 7565 7279 7365 745a 0761 7574 6f5f  .querysetZ.auto_
+00001420: 706b 7223 0000 0029 0172 5f00 0000 7224  pkr#...).r_...r$
+00001430: 0000 00da 0c67 6574 5f71 7565 7279 7365  .....get_queryse
+00001440: 7472 0000 0073 2000 0000 0001 0801 0602  tr...s .........
+00001450: 0401 1201 1602 0801 0802 0e02 0c02 0801  ................
+00001460: 2001 0401 1602 1401 0a02 7a23 4772 6170   .........z#Grap
+00001470: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
+00001480: 6f72 2e67 6574 5f71 7565 7279 7365 7463  or.get_querysetc
+00001490: 0400 0000 0000 0000 1d00 0000 1200 0000  ................
+000014a0: 4300 0000 73d8 0200 0069 007d 0469 007d  C...s....i.}.i.}
+000014b0: 0574 006a 0183 0072 8274 027c 0183 017d  .t.j...r.t.|...}
+000014c0: 0674 006a 0383 008f 5c7d 077c 076a 0474  .t.j....\}.|.j.t
+000014d0: 0583 016a 0674 056a 077c 0664 0119 006b  ...j.t.j.|.d...k
+000014e0: 027c 037c 036b 0283 026a 0883 007d 0878  .|.|.k...j...}.x
+000014f0: 307c 0844 005d 287d 097c 096a 097c 056b  0|.D.](}.|.j.|.k
+00001500: 0772 6467 007c 057c 096a 093c 007c 057c  .rdg.|.|.j.<.|.|
+00001510: 096a 0919 006a 0a7c 0983 0101 0071 4c57  .j...j.|.....qLW
+00001520: 0057 0064 0051 0052 0058 0090 0278 4e7c  .W.d.Q.R.X...xN|
+00001530: 026a 0b44 0090 025d 427d 0a69 007d 0b74  .j.D...]B}.i.}.t
+00001540: 0c7c 0a83 017d 0c74 0d7c 026a 0e7c 0c6a  .|...}.t.|.j.|.j
+00001550: 0f83 027d 0d7c 056a 107c 0d67 0083 027d  ...}.|.j.|.g...}
+00001560: 0e78 fa7c 0e44 005d f27d 0974 117c 096a  .x.|.D.].}.t.|.j
+00001570: 1283 017d 0f74 137c 0a7c 096a 1464 0083  ...}.t.|.|.j.d..
+00001580: 037d 107c 1064 006b 0872 e471 be7c 096a  .}.|.d.k.r.q.|.j
+00001590: 157d 117c 026a 0b6a 107c 1183 017d 127c  .}.|.j.j.|...}.|
+000015a0: 120c 0090 0172 6464 027c 116b 0690 0172  .....rdd.|.k...r
+000015b0: 647c 116a 1664 0264 0383 025c 027d 137d  d|.j.d.d...\.}.}
+000015c0: 1474 177c 0183 017d 157c 026a 0e6a 187d  .t.|...}.|.j.j.}
+000015d0: 1674 197c 137c 1664 048d 027d 177c 176a  .t.|.|.d...}.|.j
+000015e0: 1a7c 157c 137c 1467 0164 058d 0301 0074  .|.|.|.g.d.....t
+000015f0: 1b7c 1764 068d 017d 1874 1c7c 1883 0101  .|.d...}.t.|....
+00001600: 007c 186a 0b6a 107c 1483 017d 127c 1290  .|.j.j.|...}.|..
+00001610: 0173 6c71 be74 0c7c 1283 017d 1974 137c  .slq.t.|...}.t.|
+00001620: 127c 096a 1d64 0083 037d 1a7c 1a64 006b  .|.j.d...}.|.d.k
+00001630: 0890 0172 8e71 be7c 096a 1e7c 0f7c 107c  ...r.q.|.j.|.|.|
+00001640: 096a 147c 127c 197c 1a7c 096a 1d64 079c  .j.|.|.|.|.j.d..
+00001650: 087c 0b7c 096a 1e3c 0071 be57 0090 0178  .|.|.j.<.q.W...x
+00001660: 107c 0c6a 1f6a 2083 0044 0090 015d 007d  .|.j.j ..D...].}
+00001670: 1b74 217c 1b6a 2283 017d 1074 217c 1b6a  .t!|.j"..}.t!|.j
+00001680: 2383 017d 1c7c 1b6a 1274 246b 0290 0272  #..}.|.j.t$k...r
+00001690: 507c 1b6a 256a 2664 0819 007d 1474 0d7c  P|.j%j&d...}.t.|
+000016a0: 026a 0e7c 1483 027d 117c 026a 0b6a 107c  .j.|...}.|.j.j.|
+000016b0: 1183 017d 127c 1b6a 277c 1b6a 127c 107c  ...}.|.j'|.j.|.|
+000016c0: 1064 006b 0990 0272 267c 106a 1e6e 0264  .d.k...r&|.j.n.d
+000016d0: 007c 127c 1b6a 257c 1c7c 1c64 006b 0990  .|.|.j%|.|.d.k..
+000016e0: 0272 407c 1c6a 1e6e 0264 0064 079c 087c  .r@|.j.n.d.d...|
+000016f0: 0b7c 1b6a 273c 006e 727c 1b6a 1274 286b  .|.j'<.nr|.j.t(k
+00001700: 0290 0172 c27c 1b6a 256a 2664 0819 007d  ...r.|.j%j&d...}
+00001710: 1474 0d7c 026a 0e7c 1483 027d 117c 026a  .t.|.j.|...}.|.j
+00001720: 0b6a 107c 1183 017d 127c 1b6a 277c 1b6a  .j.|...}.|.j'|.j
+00001730: 127c 107c 1064 006b 0990 0272 9a7c 106a  .|.|.d.k...r.|.j
+00001740: 1e6e 0264 007c 127c 1b6a 257c 1c7c 1c64  .n.d.|.|.j%|.|.d
+00001750: 006b 0990 0272 b47c 1c6a 1e6e 0264 0064  .k...r.|.j.n.d.d
+00001760: 079c 087c 0b7c 1b6a 273c 0090 0171 c257  ...|.|.j'<...q.W
+00001770: 007c 0b7c 047c 0d3c 0071 8c57 007c 0453  .|.|.|.<.q.W.|.S
+00001780: 0029 094e da02 6964 da01 2e72 4a00 0000  .).N..id...rJ...
+00001790: 2902 da06 7363 6865 6d61 da04 6269 6e64  )...schema..bind
+000017a0: 2903 7276 0000 0072 7500 0000 da04 6f6e  ).rv...ru.....on
+000017b0: 6c79 2901 da08 6d65 7461 6461 7461 2908  ly)...metadata).
+000017c0: 7248 0000 00da 0964 6972 6563 7469 6f6e  rH.....direction
+000017d0: da0c 6c6f 6361 6c5f 636f 6c75 6d6e da11  ..local_column..
+000017e0: 6c6f 6361 6c5f 636f 6c75 6d6e 5f6e 616d  local_column_nam
+000017f0: 65da 0d72 656c 6174 6564 5f6d 6f64 656c  e..related_model
+00001800: da0e 7265 6c61 7465 645f 6d61 7070 6572  ..related_mapper
+00001810: da0e 7265 6c61 7465 645f 636f 6c75 6d6e  ..related_column
+00001820: 5a13 7265 6c61 7465 645f 636f 6c75 6d6e  Z.related_column
+00001830: 5f6e 616d 6572 0100 0000 2929 7215 0000  _namer....))r...
+00001840: 00da 0569 735f 6f6b 720d 0000 0072 6700  ...is_okr....rg.
+00001850: 0000 7238 0000 0072 1300 0000 7265 0000  ..r8...r....re..
+00001860: 00da 0d63 6f6e 6e65 6374 696f 6e5f 6964  ...connection_id
+00001870: da03 616c 6cda 056d 6f64 656c da06 6170  ..all..model..ap
+00001880: 7065 6e64 da07 636c 6173 7365 7372 0200  pend..classesr..
+00001890: 0000 720e 0000 0072 7800 0000 da0a 7365  ..r....rx.....se
+000018a0: 6c65 6374 6162 6c65 da03 6765 7472 1e00  lectable..getr..
+000018b0: 0000 7279 0000 0072 6900 0000 da0b 6c6f  ..ry...ri.....lo
+000018c0: 6361 6c5f 6669 656c 6472 7c00 0000 da05  cal_fieldr|.....
+000018d0: 7370 6c69 7472 0b00 0000 7276 0000 0072  splitr....rv...r
+000018e0: 0400 0000 da07 7265 666c 6563 7472 0900  ......reflectr..
+000018f0: 0000 720c 0000 00da 0d72 656c 6174 6564  ..r......related
+00001900: 5f66 6965 6c64 7248 0000 00da 0d72 656c  _fieldrH.....rel
+00001910: 6174 696f 6e73 6869 7073 da06 7661 6c75  ationships..valu
+00001920: 6573 7216 0000 00da 0d6c 6f63 616c 5f63  esr......local_c
+00001930: 6f6c 756d 6e73 da0b 7265 6d6f 7465 5f73  olumns..remote_s
+00001940: 6964 6572 0600 0000 726f 0000 0072 6800  ider....ro...rh.
+00001950: 0000 da03 6b65 7972 0700 0000 291d 725d  ....keyr....).r]
+00001960: 0000 0072 6c00 0000 da0a 4d61 7070 6564  ...rl.....Mapped
+00001970: 4261 7365 da05 6472 6166 74da 0672 6573  Base..draft..res
+00001980: 756c 745a 1772 656c 6174 696f 6e73 6869  ultZ.relationshi
+00001990: 7073 5f6f 7665 7272 6964 6573 da0a 636f  ps_overrides..co
+000019a0: 6e6e 6563 7469 6f6e 7267 0000 005a 096f  nnectionrg...Z.o
+000019b0: 7665 7272 6964 6573 da08 6f76 6572 7269  verrides..overri
+000019c0: 6465 726d 0000 005a 136d 6f64 656c 5f72  derm...Z.model_r
+000019d0: 656c 6174 696f 6e73 6869 7073 726f 0000  elationshipsro..
+000019e0: 0072 4800 0000 5a1d 6d6f 6465 6c5f 7265  .rH...Z.model_re
+000019f0: 6c61 7469 6f6e 7368 6970 735f 6f76 6572  lationships_over
+00001a00: 7269 6465 7372 7900 0000 727a 0000 005a  ridesry...rz...Z
+00001a10: 0c72 656c 6174 6564 5f6e 616d 6572 7c00  .related_namer|.
+00001a20: 0000 7275 0000 00da 0574 6162 6c65 da06  ..ru.....table..
+00001a30: 656e 6769 6e65 7276 0000 005a 1072 656c  enginerv...Z.rel
+00001a40: 6174 6564 5f6d 6574 6164 6174 615a 0c72  ated_metadataZ.r
+00001a50: 656c 6174 6564 5f62 6173 6572 7d00 0000  elated_baser}...
+00001a60: 727e 0000 00da 0c72 656c 6174 696f 6e73  r~.....relations
+00001a70: 6869 70da 0f72 656c 6174 696f 6e5f 636f  hip..relation_co
+00001a80: 6c75 6d6e 7223 0000 0072 2300 0000 7224  lumnr#...r#...r$
+00001a90: 0000 00da 1167 6574 5f72 656c 6174 696f  .....get_relatio
+00001aa0: 6e73 6869 7073 8b00 0000 7398 0000 0000  nships....s.....
+00001ab0: 0104 0104 0208 0108 020a 010a 010c 010e  ................
+00001ac0: 030a 010a 010a 011e 0210 0104 0208 010e  ................
+00001ad0: 020c 020a 010a 010e 0208 0102 0206 010c  ................
+00001ae0: 0212 0110 0108 0108 020c 0112 010a 0108  ................
+00001af0: 020c 0206 0102 0208 010e 020a 0102 0304  ................
+00001b00: 0102 0102 0104 0102 0102 0102 0114 0314  ................
+00001b10: 010a 010a 020c 010c 010c 010c 0304 0104  ................
+00001b20: 0102 0112 0102 0104 0102 0120 020c 010c  ........... ....
+00001b30: 010c 010c 0304 0104 0102 0112 0102 0104  ................
+00001b40: 0102 0124 030c 027a 2847 7261 7068 514c  ...$...z(GraphQL
+00001b50: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
+00001b60: 6765 745f 7265 6c61 7469 6f6e 7368 6970  get_relationship
+00001b70: 7363 0200 0000 0000 0000 0200 0000 0500  sc..............
+00001b80: 0000 0300 0000 732e 0000 0064 0164 0284  ......s....d.d..
+00001b90: 0089 0087 0066 0164 0364 0484 0889 0174  .....f.d.d.....t
+00001ba0: 0074 0187 0166 0164 0564 0684 087c 016a  .t...f.d.d...|.j
+00001bb0: 0283 0083 0283 0153 0029 074e 6301 0000  .......S.).Nc...
+00001bc0: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00001bd0: 0073 1400 0000 7400 7c00 6401 1900 8301  .s....t.|.d.....
+00001be0: 7c00 6402 1900 6602 5300 2903 4e72 0100  |.d...f.S.).Nr..
+00001bf0: 0000 724a 0000 0029 0172 4900 0000 2901  ..rJ...).rI...).
+00001c00: 724b 0000 0072 2300 0000 7223 0000 0072  rK...r#...r#...r
+00001c10: 2400 0000 da13 6d61 705f 6d6f 6465 6c5f  $.....map_model_
+00001c20: 7265 6c61 7469 6f6e 73f7 0000 0073 0200  relations....s..
+00001c30: 0000 0001 7a4f 4772 6170 6851 4c53 6368  ....zOGraphQLSch
+00001c40: 656d 6147 656e 6572 6174 6f72 2e63 6c65  emaGenerator.cle
+00001c50: 616e 5f72 656c 6174 696f 6e73 6869 7073  an_relationships
+00001c60: 5f62 795f 6e61 6d65 2e3c 6c6f 6361 6c73  _by_name.<locals
+00001c70: 3e2e 6d61 705f 6d6f 6465 6c5f 7265 6c61  >.map_model_rela
+00001c80: 7469 6f6e 7363 0100 0000 0000 0000 0100  tionsc..........
+00001c90: 0000 0600 0000 1300 0000 7326 0000 007c  ..........s&...|
+00001ca0: 0064 0119 0074 0074 0187 0066 0164 0264  .d...t.t...f.d.d
+00001cb0: 0384 087c 0064 0419 006a 0283 0083 0283  ...|.d...j......
+00001cc0: 0166 0253 0029 054e 7201 0000 0063 0100  .f.S.).Nr....c..
+00001cd0: 0000 0000 0000 0100 0000 0200 0000 1300  ................
+00001ce0: 0000 7308 0000 0088 007c 0083 0153 0029  ..s......|...S.)
+00001cf0: 014e 7223 0000 0029 01da 0172 2901 729a  .Nr#...)...r).r.
+00001d00: 0000 0072 2300 0000 7224 0000 0072 4c00  ...r#...r$...rL.
+00001d10: 0000 fb00 0000 7300 0000 007a 5847 7261  ......s....zXGra
+00001d20: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
+00001d30: 746f 722e 636c 6561 6e5f 7265 6c61 7469  tor.clean_relati
+00001d40: 6f6e 7368 6970 735f 6279 5f6e 616d 652e  onships_by_name.
+00001d50: 3c6c 6f63 616c 733e 2e6d 6170 5f6d 6f64  <locals>.map_mod
+00001d60: 656c 732e 3c6c 6f63 616c 733e 2e3c 6c61  els.<locals>.<la
+00001d70: 6d62 6461 3e72 4a00 0000 2903 724f 0000  mbda>rJ...).rO..
+00001d80: 0072 4d00 0000 724e 0000 0029 0172 4b00  .rM...rN...).rK.
+00001d90: 0000 2901 729a 0000 0072 2300 0000 7224  ..).r....r#...r$
+00001da0: 0000 00da 0a6d 6170 5f6d 6f64 656c 73fa  .....map_models.
+00001db0: 0000 0073 0200 0000 0001 7a46 4772 6170  ...s......zFGrap
+00001dc0: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
+00001dd0: 6f72 2e63 6c65 616e 5f72 656c 6174 696f  or.clean_relatio
+00001de0: 6e73 6869 7073 5f62 795f 6e61 6d65 2e3c  nships_by_name.<
+00001df0: 6c6f 6361 6c73 3e2e 6d61 705f 6d6f 6465  locals>.map_mode
+00001e00: 6c73 6301 0000 0000 0000 0001 0000 0002  lsc.............
+00001e10: 0000 0013 0000 0073 0800 0000 8800 7c00  .......s......|.
+00001e20: 8301 5300 2901 4e72 2300 0000 2901 724b  ..S.).Nr#...).rK
+00001e30: 0000 0029 0172 9c00 0000 7223 0000 0072  ...).r....r#...r
+00001e40: 2400 0000 724c 0000 00fd 0000 0073 0000  $...rL.......s..
+00001e50: 0000 7a44 4772 6170 6851 4c53 6368 656d  ..zDGraphQLSchem
+00001e60: 6147 656e 6572 6174 6f72 2e63 6c65 616e  aGenerator.clean
+00001e70: 5f72 656c 6174 696f 6e73 6869 7073 5f62  _relationships_b
+00001e80: 795f 6e61 6d65 2e3c 6c6f 6361 6c73 3e2e  y_name.<locals>.
+00001e90: 3c6c 616d 6264 613e 2903 724f 0000 0072  <lambda>).rO...r
+00001ea0: 4d00 0000 724e 0000 0029 0272 5d00 0000  M...rN...).r]...
+00001eb0: 728b 0000 0072 2300 0000 2902 729a 0000  r....r#...).r...
+00001ec0: 0072 9c00 0000 7224 0000 00da 1b63 6c65  .r....r$.....cle
+00001ed0: 616e 5f72 656c 6174 696f 6e73 6869 7073  an_relationships
+00001ee0: 5f62 795f 6e61 6d65 f600 0000 7306 0000  _by_name....s...
+00001ef0: 0000 0108 030c 037a 3247 7261 7068 514c  .......z2GraphQL
+00001f00: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
+00001f10: 636c 6561 6e5f 7265 6c61 7469 6f6e 7368  clean_relationsh
+00001f20: 6970 735f 6279 5f6e 616d 6563 0300 0000  ips_by_namec....
+00001f30: 0000 0000 0500 0000 0500 0000 0300 0000  ................
+00001f40: 733e 0000 007c 026a 0064 0119 007d 0374  s>...|.j.d...}.t
+00001f50: 017c 016a 027c 0383 027d 047c 016a 036a  .|.j.|...}.|.j.j
+00001f60: 047c 0483 0189 0074 0574 0687 0066 0164  .|.....t.t...f.d
+00001f70: 0264 0384 087c 026a 076a 0883 0083 0283  .d...|.j.j......
+00001f80: 0153 0029 044e 7201 0000 0063 0100 0000  .S.).Nr....c....
+00001f90: 0000 0000 0100 0000 0400 0000 1300 0000  ................
+00001fa0: 7312 0000 0074 007c 0083 0174 0188 007c  s....t.|...t...|
+00001fb0: 0083 0266 0253 0029 014e 2902 7249 0000  ...f.S.).N).rI..
+00001fc0: 0072 6900 0000 2901 724b 0000 0029 0172  .ri...).rK...).r
+00001fd0: 6d00 0000 7223 0000 0072 2400 0000 724c  m...r#...r$...rL
+00001fe0: 0000 0003 0100 0073 0000 0000 7a48 4772  .......s....zHGr
+00001ff0: 6170 6851 4c53 6368 656d 6147 656e 6572  aphQLSchemaGener
+00002000: 6174 6f72 2e67 6574 5f6d 6f64 656c 5f63  ator.get_model_c
+00002010: 6f6c 756d 6e73 5f62 795f 636c 6561 6e5f  olumns_by_clean_
+00002020: 6e61 6d65 2e3c 6c6f 6361 6c73 3e2e 3c6c  name.<locals>.<l
+00002030: 616d 6264 613e 2909 7268 0000 0072 0e00  ambda>).rh...r..
+00002040: 0000 7278 0000 0072 8400 0000 7286 0000  ..rx...r....r...
+00002050: 0072 4f00 0000 724d 0000 00da 0763 6f6c  .rO...rM.....col
+00002060: 756d 6e73 da04 6b65 7973 2905 725d 0000  umns..keys).r]..
+00002070: 0072 9000 0000 726f 0000 0072 9500 0000  .r....ro...r....
+00002080: 7248 0000 0072 2300 0000 2901 726d 0000  rH...r#...).rm..
+00002090: 0072 2400 0000 da1f 6765 745f 6d6f 6465  .r$.....get_mode
+000020a0: 6c5f 636f 6c75 6d6e 735f 6279 5f63 6c65  l_columns_by_cle
+000020b0: 616e 5f6e 616d 65ff 0000 0073 0800 0000  an_name....s....
+000020c0: 0001 0a01 0c01 0c01 7a36 4772 6170 6851  ........z6GraphQ
+000020d0: 4c53 6368 656d 6147 656e 6572 6174 6f72  LSchemaGenerator
+000020e0: 2e67 6574 5f6d 6f64 656c 5f63 6f6c 756d  .get_model_colum
+000020f0: 6e73 5f62 795f 636c 6561 6e5f 6e61 6d65  ns_by_clean_name
+00002100: 6303 0000 0000 0000 0004 0000 0003 0000  c...............
+00002110: 0043 0000 0073 2000 0000 7400 7c01 6a01  .C...s ...t.|.j.
+00002120: 7c02 6a02 8302 7d03 7c00 6a03 6a04 7c03  |.j...}.|.j.j.|.
+00002130: 6900 8302 6a05 8300 5300 2901 4e29 0672  i...j...S.).N).r
+00002140: 0e00 0000 7278 0000 0072 8500 0000 7254  ....rx...r....rT
+00002150: 0000 0072 8600 0000 728c 0000 0029 0472  ...r....r....).r
+00002160: 5d00 0000 7290 0000 0072 6f00 0000 7248  ]...r....ro...rH
+00002170: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00002180: 0000 da17 6765 745f 6d6f 6465 6c5f 7265  ....get_model_re
+00002190: 6c61 7469 6f6e 7368 6970 7305 0100 0073  lationships....s
+000021a0: 0400 0000 0001 0e01 7a2e 4772 6170 6851  ........z.GraphQ
+000021b0: 4c53 6368 656d 6147 656e 6572 6174 6f72  LSchemaGenerator
+000021c0: 2e67 6574 5f6d 6f64 656c 5f72 656c 6174  .get_model_relat
+000021d0: 696f 6e73 6869 7073 6303 0000 0000 0000  ionshipsc.......
+000021e0: 0004 0000 0003 0000 0043 0000 0073 1c00  .........C...s..
+000021f0: 0000 7400 7c01 6a01 7c02 6a02 8302 7d03  ..t.|.j.|.j...}.
+00002200: 7c00 6a03 6a04 7c03 6900 8302 5300 2901  |.j.j.|.i...S.).
+00002210: 4e29 0572 0e00 0000 7278 0000 0072 8500  N).r....rx...r..
+00002220: 0000 7254 0000 0072 8600 0000 2904 725d  ..rT...r....).r]
+00002230: 0000 0072 9000 0000 726f 0000 0072 4800  ...r....ro...rH.
+00002240: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
+00002250: 00da 1f67 6574 5f6d 6f64 656c 5f72 656c  ...get_model_rel
+00002260: 6174 696f 6e73 6869 7073 5f62 795f 6e61  ationships_by_na
+00002270: 6d65 0901 0000 7304 0000 0000 010e 017a  me....s........z
+00002280: 3647 7261 7068 514c 5363 6865 6d61 4765  6GraphQLSchemaGe
+00002290: 6e65 7261 746f 722e 6765 745f 6d6f 6465  nerator.get_mode
+000022a0: 6c5f 7265 6c61 7469 6f6e 7368 6970 735f  l_relationships_
+000022b0: 6279 5f6e 616d 6563 0300 0000 0000 0000  by_namec........
+000022c0: 0400 0000 0300 0000 4300 0000 731c 0000  ........C...s...
+000022d0: 0074 007c 016a 017c 026a 0283 027d 037c  .t.|.j.|.j...}.|
+000022e0: 006a 036a 047c 0369 0083 0253 0029 014e  .j.j.|.i...S.).N
+000022f0: 2905 720e 0000 0072 7800 0000 7285 0000  ).r....rx...r...
+00002300: 0072 5500 0000 7286 0000 0029 0472 5d00  .rU...r....).r].
+00002310: 0000 7290 0000 0072 6f00 0000 7248 0000  ..r....ro...rH..
+00002320: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00002330: da25 6765 745f 6d6f 6465 6c5f 7265 6c61  .%get_model_rela
+00002340: 7469 6f6e 7368 6970 735f 6279 5f63 6c65  tionships_by_cle
+00002350: 616e 5f6e 616d 650d 0100 0073 0400 0000  an_name....s....
+00002360: 0001 0e01 7a3c 4772 6170 6851 4c53 6368  ....z<GraphQLSch
+00002370: 656d 6147 656e 6572 6174 6f72 2e67 6574  emaGenerator.get
+00002380: 5f6d 6f64 656c 5f72 656c 6174 696f 6e73  _model_relations
+00002390: 6869 7073 5f62 795f 636c 6561 6e5f 6e61  hips_by_clean_na
+000023a0: 6d65 4663 0700 0000 0000 0000 1b00 0000  meFc............
+000023b0: 0b00 0000 4300 0000 7338 0200 007c 0570  ....C...s8...|.p
+000023c0: 0667 007d 0590 0278 287c 0444 0090 025d  .g.}...x(|.D...]
+000023d0: 1e7d 0774 007c 0783 017d 0890 0278 0e7c  .}.t.|...}...x.|
+000023e0: 086a 0183 0044 0090 025d 005c 027d 097d  .j...D...].\.}.}
+000023f0: 0a7c 0964 016b 0272 547c 006a 027c 017c  .|.d.k.rT|.j.|.|
+00002400: 027c 037c 0a7c 0564 0264 038d 067d 0271  .|.|.|.d.d...}.q
+00002410: 2a7c 006a 037c 017c 0383 027d 0b7c 0b6a  *|.j.|.|...}.|.j
+00002420: 047c 0983 017d 0c7c 006a 057c 017c 0383  .|...}.|.j.|.|..
+00002430: 026a 047c 0983 017d 0d7c 0d64 006b 0972  .j.|...}.|.d.k.r
+00002440: ce74 007c 0a83 017d 0e78 3e7c 0e6a 0183  .t.|...}.x>|.j..
+00002450: 0044 005d 325c 027d 0f7d 107c 0f64 046b  .D.]2\.}.}.|.d.k
+00002460: 0272 967c 0d64 0519 007d 117c 006a 027c  .r.|.d...}.|.j.|
+00002470: 017c 027c 117c 107c 057c 0d66 0195 027c  .|.|.|.|.|.f...|
+00002480: 0683 067d 0271 9657 0071 2a7c 0c64 006b  ...}.q.W.q*|.d.k
+00002490: 0972 2a74 007c 0a83 017d 0e90 0178 4a7c  .r*t.|...}...xJ|
+000024a0: 0e6a 0183 0044 0090 015d 3c5c 027d 0f7d  .j...D...]<\.}.}
+000024b0: 107c 0f64 046b 0290 0172 5e78 5c7c 006a  .|.d.k...r^x\|.j
+000024c0: 067c 017c 0383 0244 005d 4c7d 127c 1264  .|.|...D.]L}.|.d
+000024d0: 0619 0074 076b 0390 0173 0c7c 1264 0719  ...t.k...s.|.d..
+000024e0: 007c 0c6a 086b 0390 0172 3290 0171 0c7c  .|.j.k...r2..q.|
+000024f0: 1264 0519 007d 117c 006a 027c 017c 027c  .d...}.|.j.|.|.|
+00002500: 117c 107c 057c 1266 0195 027c 0683 067d  .|.|.|.f...|...}
+00002510: 0250 0090 0171 0c57 0071 ea74 097c 0583  .P...q.W.q.t.|..
+00002520: 0190 0172 d664 007d 1378 5c7c 0544 005d  ...r.d.}.x\|.D.]
+00002530: 547d 1274 0a7c 1264 0819 0083 017d 1474  T}.t.|.d.....}.t
+00002540: 0b7c 147c 1264 0919 006a 0883 027d 157c  .|.|.d...j...}.|
+00002550: 1390 0172 a874 0b7c 137c 1264 0a19 006a  ...r.t.|.|.d...j
+00002560: 0883 026e 067c 1264 0a19 007d 167c 026a  ...n.|.d...}.|.j
+00002570: 0c7c 147c 157c 166b 0283 027d 027c 147d  .|.|.|.k...}.|.}
+00002580: 1390 0171 7257 0074 0b7c 137c 0c6a 0883  ...qrW.t.|.|.j..
+00002590: 027d 0c74 0d7c 0c6a 0e83 017d 1774 0f6a  .}.t.|.j...}.t.j
+000025a0: 106a 047c 0f83 017d 187c 1764 0b19 007c  .j.|...}.|.d...|
+000025b0: 0c6a 117c 0c7c 1864 0c64 0d8d 047d 197c  .j.|.|.d.d...}.|
+000025c0: 196a 127c 027c 1083 027d 1a7c 0690 0272  .j.|.|...}.|...r
+000025d0: 1a7c 1a0f 006e 027c 1a7d 1a7c 026a 137c  .|...n.|.}.|.j.|
+000025e0: 1a83 017d 0271 ea57 0071 2a57 0071 1057  ...}.q.W.q*W.q.W
+000025f0: 007c 0253 0029 0e4e da05 5f6e 6f74 5f54  .|.S.).N.._not_T
+00002600: 2901 da07 6578 636c 7564 65da 0872 656c  )...exclude..rel
+00002610: 6174 696f 6e72 7d00 0000 7279 0000 0072  ationr}...ry...r
+00002620: 7b00 0000 727c 0000 0072 7e00 0000 727a  {...r|...r~...rz
+00002630: 0000 005a 0c66 696c 7465 725f 636c 6173  ...Z.filter_clas
+00002640: 7346 2904 7248 0000 00da 0663 6f6c 756d  sF).rH.....colum
+00002650: 6eda 066c 6f6f 6b75 7072 a500 0000 2914  n..lookupr....).
+00002660: 724f 0000 0072 4e00 0000 da0f 6669 6c74  rO...rN.....filt
+00002670: 6572 5f71 7565 7279 7365 7472 a000 0000  er_querysetr....
+00002680: 7286 0000 0072 a300 0000 72a1 0000 0072  r....r....r....r
+00002690: 0600 0000 7248 0000 0072 6600 0000 7208  ....rH...rf...r.
+000026a0: 0000 0072 6900 0000 da04 6a6f 696e 7210  ...ri.....joinr.
+000026b0: 0000 00da 0474 7970 6572 0f00 0000 5a06  .....typer....Z.
+000026c0: 6279 5f67 716c 728f 0000 005a 1567 6574  by_gqlr....Z.get
+000026d0: 5f6c 6f6f 6f6b 7570 5f63 7269 7465 7269  _loookup_criteri
+000026e0: 6f6e 7265 0000 0029 1b72 5d00 0000 7290  onre...).r]...r.
+000026f0: 0000 0072 7100 0000 726f 0000 00da 0766  ...rq...ro.....f
+00002700: 696c 7465 7273 5a10 7061 7265 6e74 5f72  iltersZ.parent_r
+00002710: 656c 6174 696f 6e73 72a5 0000 005a 0c66  elationsr....Z.f
+00002720: 696c 7465 7273 5f69 7465 6d5a 1166 696c  ilters_itemZ.fil
+00002730: 7465 7273 5f69 7465 6d5f 6469 6374 5a0b  ters_item_dictZ.
+00002740: 6669 6c74 6572 5f6e 616d 655a 0e66 696c  filter_nameZ.fil
+00002750: 7465 725f 6c6f 6f6b 7570 73da 1563 6f6c  ter_lookups..col
+00002760: 756d 6e73 5f62 795f 636c 6561 6e5f 6e61  umns_by_clean_na
+00002770: 6d65 72a7 0000 005a 1366 696c 7465 725f  mer....Z.filter_
+00002780: 7265 6c61 7469 6f6e 7368 6970 5a13 6669  relationshipZ.fi
+00002790: 6c74 6572 5f6c 6f6f 6b75 7073 5f64 6963  lter_lookups_dic
+000027a0: 74da 0b6c 6f6f 6b75 705f 6e61 6d65 5a0c  t..lookup_nameZ.
+000027b0: 6c6f 6f6b 7570 5f76 616c 7565 da0f 7265  lookup_value..re
+000027c0: 6c61 7469 6f6e 5f6d 6170 7065 7272 9700  lation_mapperr..
+000027d0: 0000 5a12 6c61 7374 5f72 656c 6174 6564  ..Z.last_related
+000027e0: 5f6d 6f64 656c 727c 0000 0072 7e00 0000  _modelr|...r~...
+000027f0: 727a 0000 00da 0469 7465 6d72 a800 0000  rz.....itemr....
+00002800: da08 696e 7374 616e 6365 da09 6372 6974  ..instance..crit
+00002810: 6572 696f 6e72 2300 0000 7223 0000 0072  erionr#...r#...r
+00002820: 2400 0000 72a9 0000 0011 0100 0073 8400  $...r........s..
+00002830: 0000 0001 0802 0e01 0802 1601 0801 0401  ................
+00002840: 0201 0201 0201 0201 0201 0802 0202 0c01  ................
+00002850: 0a01 1202 0801 0802 1201 0801 0801 0401  ................
+00002860: 0201 0201 0201 0201 0801 0c02 0801 0802  ................
+00002870: 1601 0a01 1201 1e01 0402 0801 0401 0201  ................
+00002880: 0201 0201 0201 0801 0602 0a02 0a01 0402  ................
+00002890: 0a01 0c01 1001 1e01 0401 0201 0a02 0a02  ................
+000028a0: 0c02 0a01 0c01 0601 0401 0201 0201 0802  ................
+000028b0: 0c01 1002 1602 7a26 4772 6170 6851 4c53  ......z&GraphQLS
+000028c0: 6368 656d 6147 656e 6572 6174 6f72 2e66  chemaGenerator.f
+000028d0: 696c 7465 725f 7175 6572 7973 6574 6304  ilter_querysetc.
+000028e0: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
+000028f0: 0000 0073 2000 0000 7c03 6400 6b09 721c  ...s ...|.d.k.r.
+00002900: 7c03 6401 1900 7d04 7400 7c01 7c02 7c04  |.d...}.t.|.|.|.
+00002910: 8303 7d01 7c01 5300 2902 4e72 3800 0000  ..}.|.S.).Nr8...
+00002920: 2901 7212 0000 0029 0572 5d00 0000 7271  ).r....).r]...rq
+00002930: 0000 0072 6f00 0000 da06 7365 6172 6368  ...ro.....search
+00002940: 7238 0000 0072 2300 0000 7223 0000 0072  r8...r#...r#...r
+00002950: 2400 0000 7212 0000 0067 0100 0073 0800  $...r....g...s..
+00002960: 0000 0001 0801 0801 0c02 7a26 4772 6170  ..........z&Grap
+00002970: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
+00002980: 6f72 2e73 6561 7263 685f 7175 6572 7973  or.search_querys
+00002990: 6574 6307 0000 0000 0000 000a 0000 0008  etc.............
+000029a0: 0000 0043 0000 0073 3400 0000 6700 7d07  ...C...s4...g.}.
+000029b0: 782a 7c06 4400 5d22 7d08 7c00 6a00 7c08  x*|.D.]"}.|.j.|.
+000029c0: 7c01 7c02 7c03 7c04 7c05 8306 7d09 7c07  |.|.|.|.|...}.|.
+000029d0: 6a01 7c09 8301 0100 710a 5700 7c07 5300  j.|.....q.W.|.S.
+000029e0: 2901 4e29 02da 1167 6574 5f6d 6f64 656c  ).N)...get_model
+000029f0: 735f 6c6f 6f6b 7570 7283 0000 0029 0a72  s_lookupr....).r
+00002a00: 5d00 0000 726c 0000 0072 9000 0000 da06  ]...rl...r......
+00002a10: 6d6f 6465 6c73 726d 0000 0072 6f00 0000  modelsrm...ro...
+00002a20: 720f 0000 0072 9200 0000 da0b 6c6f 6f6b  r....r......look
+00002a30: 7570 5f69 7465 6dda 0d6c 6f6f 6b75 705f  up_item..lookup_
+00002a40: 7265 7375 6c74 7223 0000 0072 2300 0000  resultr#...r#...
+00002a50: 7224 0000 00da 1267 6574 5f6d 6f64 656c  r$.....get_model
+00002a60: 735f 6c6f 6f6b 7570 736e 0100 0073 1600  s_lookupsn...s..
+00002a70: 0000 0001 0402 0a01 0401 0201 0201 0201  ................
+00002a80: 0201 0201 0602 0e02 7a29 4772 6170 6851  ........z)GraphQ
+00002a90: 4c53 6368 656d 6147 656e 6572 6174 6f72  LSchemaGenerator
+00002aa0: 2e67 6574 5f6d 6f64 656c 735f 6c6f 6f6b  .get_models_look
+00002ab0: 7570 7363 0700 0000 0000 0000 1700 0000  upsc............
+00002ac0: 0900 0000 0300 0000 7346 0300 0069 007d  ........sF...i.}
+00002ad0: 0774 007c 0183 017d 0890 0378 327c 086a  .t.|...}...x2|.j
+00002ae0: 0183 0044 0090 035d 245c 027d 097d 0a7c  ...D...]$\.}.}.|
+00002af0: 006a 027c 037c 0683 027d 0b7c 0b6a 037c  .j.|.|...}.|.j.|
+00002b00: 0983 0189 007c 006a 047c 037c 0683 026a  .....|.j.|.|...j
+00002b10: 037c 0983 017d 0c7c 0c64 006b 0990 0272  .|...}.|.d.k...r
+00002b20: 0c69 007d 0d7c 0c64 0119 0089 0274 0574  .i.}.|.d.....t.t
+00002b30: 0674 0774 0887 0266 0164 0264 0384 087c  .t.t...f.d.d...|
+00002b40: 0483 0283 0183 0174 0964 048d 027d 0e7c  .......t.d...}.|
+00002b50: 0a6a 0364 0564 0683 027c 0d64 053c 007c  .j.d.d...|.d.<.|
+00002b60: 0a6a 0364 0764 0683 027c 0d64 083c 007c  .j.d.d...|.d.<.|
+00002b70: 057c 0d64 093c 007c 067c 0d64 0a3c 0074  .|.d.<.|.|.d.<.t
+00002b80: 0a74 0887 0266 0164 0b64 0384 087c 0483  .t...f.d.d...|..
+00002b90: 0283 017c 0d64 0c3c 0088 026a 0b7c 0d64  ...|.d.<...j.|.d
+00002ba0: 0d3c 0064 0e7c 0a6b 0690 0172 967c 0c64  .<.d.|.k...r.|.d
+00002bb0: 0f19 007d 0f7c 0c64 1019 007d 107c 0c64  ...}.|.d...}.|.d
+00002bc0: 1119 007d 1164 127c 0a64 0e19 006b 0690  ...}.d.|.d...k..
+00002bd0: 0172 147c 0a64 0e19 0064 1219 007d 126e  .r.|.d...d...}.n
+00002be0: 0c7c 106a 0c64 1319 006a 0b7d 1274 0d7c  .|.j.d...j.}.t.|
+00002bf0: 0f7c 1264 0083 037d 137c 1364 006b 0990  .|.d...}.|.d.k..
+00002c00: 0172 9674 0e7c 0a64 0e19 0064 1419 007c  .r.t.|.d...d...|
+00002c10: 1383 027d 147c 026a 0f6a 107c 117c 1483  ...}.|.j.j.|.|..
+00002c20: 026a 117c 116a 127c 0e83 0183 016a 137c  .j.|.j.|.....j.|
+00002c30: 1183 017d 1574 007c 1583 0189 0174 0a74  ...}.t.|.....t.t
+00002c40: 0887 0187 0266 0264 1564 0384 087c 0483  .....f.d.d...|..
+00002c50: 0283 017c 0d64 163c 007c 116a 0b7c 0d64  ...|.d.<.|.j.|.d
+00002c60: 113c 0064 177c 0a6b 0690 0272 027c 0c64  .<.d.|.k...r.|.d
+00002c70: 0f19 007d 0f7c 0c64 1019 007d 107c 0c64  ...}.|.d...}.|.d
+00002c80: 1119 007d 117c 026a 0f6a 107c 0f83 016a  ...}.|.j.j.|...j
+00002c90: 117c 116a 127c 0e83 0183 016a 1483 007d  .|.j.|.....j...}
+00002ca0: 1674 0a7c 1683 017d 167c 006a 157c 0a64  .t.|...}.|.j.|.d
+00002cb0: 1719 007c 027c 037c 167c 0f7c 1083 067c  ...|.|.|.|.|...|
+00002cc0: 0d64 183c 007c 116a 0b7c 0d64 113c 007c  .d.<.|.j.|.d.<.|
+00002cd0: 0d7c 077c 093c 0071 1888 0064 006b 0972  .|.|.<.q...d.k.r
+00002ce0: 1869 007d 0d74 0574 0674 0774 0887 0066  .i.}.t.t.t.t...f
+00002cf0: 0164 1964 0384 087c 0483 0283 0183 0174  .d.d...|.......t
+00002d00: 0964 048d 027d 0e7c 0a6a 0364 0564 0683  .d...}.|.j.d.d..
+00002d10: 027c 0d64 053c 007c 0a6a 0364 0764 0683  .|.d.<.|.j.d.d..
+00002d20: 027c 0d64 083c 007c 057c 0d64 093c 007c  .|.d.<.|.|.d.<.|
+00002d30: 067c 0d64 0a3c 0074 0a74 0887 0066 0164  .|.d.<.t.t...f.d
+00002d40: 1a64 0384 087c 0483 0283 017c 0d64 0c3c  .d...|.....|.d.<
+00002d50: 0088 006a 0b7c 0d64 0d3c 0064 177c 0a6b  ...j.|.d.<.d.|.k
+00002d60: 0690 0372 3678 9c7c 006a 167c 037c 0683  ...r6x.|.j.|.|..
+00002d70: 0244 005d 8c7d 0c7c 0c64 1b19 0074 176b  .D.].}.|.d...t.k
+00002d80: 0390 0273 a67c 0c64 1c19 0088 006a 0b6b  ...s.|.d.....j.k
+00002d90: 0390 0272 cc90 0271 a67c 0c64 1019 007d  ...r...q.|.d...}
+00002da0: 107c 0c64 0f19 007d 0f7c 0c64 1119 007d  .|.d...}.|.d...}
+00002db0: 117c 026a 0f6a 107c 0f83 016a 117c 116a  .|.j.j.|...j.|.j
+00002dc0: 127c 0e83 0183 016a 1483 007d 1674 0a7c  .|.....j...}.t.|
+00002dd0: 1683 017d 167c 006a 157c 0a64 1719 007c  ...}.|.j.|.d...|
+00002de0: 027c 037c 167c 0f7c 1083 067c 0d64 183c  .|.|.|.|...|.d.<
+00002df0: 007c 116a 0b7c 0d64 113c 0050 0090 0271  .|.j.|.d.<.P...q
+00002e00: a657 007c 0d7c 077c 093c 0071 1857 007c  .W.|.|.|.<.q.W.|
+00002e10: 0753 0029 1d4e 727a 0000 0063 0100 0000  .S.).Nrz...c....
+00002e20: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00002e30: 730c 0000 0074 007c 0088 006a 0183 0253  s....t.|...j...S
+00002e40: 0029 014e 2902 7269 0000 0072 4800 0000  .).N).ri...rH...
+00002e50: 2901 724b 0000 0029 0172 7a00 0000 7223  ).rK...).rz...r#
+00002e60: 0000 0072 2400 0000 724c 0000 008b 0100  ...r$...rL......
+00002e70: 0073 0000 0000 7a3a 4772 6170 6851 4c53  .s....z:GraphQLS
+00002e80: 6368 656d 6147 656e 6572 6174 6f72 2e67  chemaGenerator.g
+00002e90: 6574 5f6d 6f64 656c 735f 6c6f 6f6b 7570  et_models_lookup
+00002ea0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00002eb0: 613e 2901 728f 0000 00da 0672 6574 7572  a>).r......retur
+00002ec0: 6e46 da0a 7265 7475 726e 4c69 7374 da0b  nF..returnList..
+00002ed0: 7265 7475 726e 5f6c 6973 7472 6d00 0000  return_listrm...
+00002ee0: 726f 0000 0063 0100 0000 0000 0000 0100  ro...c..........
+00002ef0: 0000 0400 0000 1300 0000 7312 0000 007c  ..........s....|
+00002f00: 0074 007c 0088 006a 0183 0264 019c 0253  .t.|...j...d...S
+00002f10: 0029 024e 2902 72b1 0000 00da 0576 616c  .).N).r......val
+00002f20: 7565 2902 7269 0000 0072 4800 0000 2901  ue).ri...rH...).
+00002f30: 724b 0000 0029 0172 7a00 0000 7223 0000  rK...).rz...r#..
+00002f40: 0072 2400 0000 724c 0000 0091 0100 0073  .r$...rL.......s
+00002f50: 0000 0000 da0c 6d6f 6465 6c5f 7661 6c75  ......model_valu
+00002f60: 6573 da0d 736f 7572 6365 5f63 6f6c 756d  es..source_colum
+00002f70: 6eda 0961 6767 7265 6761 7465 727c 0000  n..aggregater|..
+00002f80: 0072 7d00 0000 727e 0000 0072 4100 0000  .r}...r~...rA...
+00002f90: 7201 0000 0072 4000 0000 6301 0000 0000  r....r@...c.....
+00002fa0: 0000 0001 0000 0005 0000 0013 0000 0073  ...............s
+00002fb0: 1a00 0000 7c00 8800 6a00 7401 7c00 8801  ....|...j.t.|...
+00002fc0: 6a02 8302 6401 8302 6402 9c02 5300 2903  j...d...d...S.).
+00002fd0: 4e72 0100 0000 2902 72b1 0000 0072 bc00  Nr....).r....r..
+00002fe0: 0000 2903 7286 0000 0072 6900 0000 7248  ..).r....ri...rH
+00002ff0: 0000 0029 0172 4b00 0000 2902 da0b 6772  ...).rK...)...gr
+00003000: 6f75 7073 5f64 6963 7472 7a00 0000 7223  oups_dictrz...r#
+00003010: 0000 0072 2400 0000 724c 0000 00a8 0100  ...r$...rL......
+00003020: 0073 0400 0000 0001 0201 da11 6167 6772  .s..........aggr
+00003030: 6567 6174 6564 5f76 616c 7565 7372 a600  egated_valuesr..
+00003040: 0000 da07 7265 6c61 7465 6463 0100 0000  ....relatedc....
+00003050: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00003060: 730c 0000 0074 007c 0088 006a 0183 0253  s....t.|...j...S
+00003070: 0029 014e 2902 7269 0000 0072 4800 0000  .).N).ri...rH...
+00003080: 2901 724b 0000 0029 0172 a700 0000 7223  ).rK...).r....r#
+00003090: 0000 0072 2400 0000 724c 0000 00c6 0100  ...r$...rL......
+000030a0: 0073 0000 0000 6301 0000 0000 0000 0001  .s....c.........
+000030b0: 0000 0004 0000 0013 0000 0073 1200 0000  ...........s....
+000030c0: 7c00 7400 7c00 8800 6a01 8302 6401 9c02  |.t.|...j...d...
+000030d0: 5300 2902 4e29 0272 b100 0000 72bc 0000  S.).N).r....r...
+000030e0: 0029 0272 6900 0000 7248 0000 0029 0172  .).ri...rH...).r
+000030f0: 4b00 0000 2901 72a7 0000 0072 2300 0000  K...).r....r#...
+00003100: 7224 0000 0072 4c00 0000 cc01 0000 7300  r$...rL.......s.
+00003110: 0000 0072 7900 0000 727b 0000 0029 1872  ...ry...r{...).r
+00003120: 4f00 0000 724e 0000 0072 a000 0000 7286  O...rN...r....r.
+00003130: 0000 0072 a300 0000 da06 736f 7274 6564  ...r......sorted
+00003140: 7218 0000 0072 1900 0000 724d 0000 0072  r....r....rM...r
+00003150: 1700 0000 7264 0000 0072 4800 0000 7263  ....rd...rH...rc
+00003160: 0000 0072 6900 0000 7211 0000 0072 6700  ...ri...r....rg.
+00003170: 0000 7238 0000 0072 6500 0000 da03 696e  ..r8...re.....in
+00003180: 5f72 6b00 0000 7281 0000 0072 b400 0000  _rk...r....r....
+00003190: 72a1 0000 0072 0600 0000 2917 725d 0000  r....r....).r]..
+000031a0: 0072 b600 0000 726c 0000 0072 9000 0000  .r....rl...r....
+000031b0: 72b5 0000 0072 6d00 0000 726f 0000 0072  r....rm...ro...r
+000031c0: 9200 0000 5a10 6c6f 6f6b 7570 5f69 7465  ....Z.lookup_ite
+000031d0: 6d5f 6469 6374 72ae 0000 00da 0b6c 6f6f  m_dictr......loo
+000031e0: 6b75 705f 6461 7461 72ad 0000 0072 9700  kup_datar....r..
+000031f0: 0000 72b7 0000 005a 0d6c 6f6f 6b75 705f  ..r....Z.lookup_
+00003200: 7661 6c75 6573 5a0e 7265 6c61 7469 6f6e  valuesZ.relation
+00003210: 5f6d 6f64 656c 72af 0000 0072 9800 0000  _modelr....r....
+00003220: 5a15 6167 6772 6567 6174 655f 636f 6c75  Z.aggregate_colu
+00003230: 6d6e 5f6e 616d 655a 1061 6767 7265 6761  mn_nameZ.aggrega
+00003240: 7465 5f63 6f6c 756d 6e5a 0e61 6767 7265  te_columnZ.aggre
+00003250: 6761 7465 5f66 756e 63da 0667 726f 7570  gate_func..group
+00003260: 735a 0e72 656c 6174 6564 5f6d 6f64 656c  sZ.related_model
+00003270: 7372 2300 0000 2903 72a7 0000 0072 c000  sr#...).r....r..
+00003280: 0000 727a 0000 0072 2400 0000 72b4 0000  ..rz...r$...r...
+00003290: 007e 0100 0073 a400 0000 0001 0402 0802  .~...s..........
+000032a0: 1601 0c01 0a01 1202 0a01 0401 0801 2202  ..............".
+000032b0: 1001 1001 0801 0801 1a01 0a02 0a01 0801  ................
+000032c0: 0801 0802 0e01 0e02 0c02 0c01 0a01 1202  ................
+000032d0: 0601 0801 0c01 0601 0802 1003 0c01 0a02  ................
+000032e0: 0a01 0801 0801 0802 0601 0601 1002 0802  ................
+000032f0: 0401 0601 0201 0201 0201 0201 0a02 0a02  ................
+00003300: 0a01 0801 0401 2202 1001 1001 0801 0801  ......".........
+00003310: 1a01 0a02 0a01 1201 1e01 0402 0801 0801  ................
+00003320: 0802 0601 0601 1002 0802 0401 0601 0201  ................
+00003330: 0201 0201 0201 0a02 0a01 0802 0c02 7a28  ..............z(
+00003340: 4772 6170 6851 4c53 6368 656d 6147 656e  GraphQLSchemaGen
+00003350: 6572 6174 6f72 2e67 6574 5f6d 6f64 656c  erator.get_model
+00003360: 735f 6c6f 6f6b 7570 6303 0000 0000 0000  s_lookupc.......
+00003370: 0007 0000 0006 0000 0003 0000 0073 fa00  .............s..
+00003380: 0000 6900 7d03 78f0 7c01 6a00 8300 4400  ..i.}.x.|.j...D.
+00003390: 5de4 5c02 7d04 8901 6900 7d05 8801 6401  ].\.}...i.}...d.
+000033a0: 1900 7d06 8800 723c 7401 7402 8700 6601  ..}...r<t.t...f.
+000033b0: 6402 6403 8408 7c06 8302 8301 7d06 7401  d.d...|.....}.t.
+000033c0: 7403 7404 6404 6403 8400 7c06 8302 8301  t.t.d.d...|.....
+000033d0: 8301 8902 8801 6405 1900 7284 8801 6406  ......d...r...d.
+000033e0: 1900 726c 8802 7c05 6407 3c00 6e18 7405  ..rl..|.d.<.n.t.
+000033f0: 8802 8301 727c 8802 6408 1900 6e02 6400  ....r|..d...n.d.
+00003400: 7c05 6407 3c00 6409 8801 6b06 72aa 7c00  |.d.<.d...k.r.|.
+00003410: 6a06 8801 6409 1900 8701 8702 6602 640a  j...d.......f.d.
+00003420: 6403 8408 8302 7c05 6409 3c00 640b 8801  d.....|.d.<.d...
+00003430: 6b06 72ea 7401 7402 8701 8702 6602 640c  k.r.t.t.....f.d.
+00003440: 6403 8408 8801 640b 1900 8302 8301 7d06  d.....d.......}.
+00003450: 7405 7c06 8301 72e2 7c06 6408 1900 6407  t.|...r.|.d...d.
+00003460: 1900 6e02 6408 7c05 640d 3c00 7c05 7c03  ..n.d.|.d.<.|.|.
+00003470: 7c04 3c00 710e 5700 7c03 5300 290e 4e72  |.<.q.W.|.S.).Nr
+00003480: bd00 0000 6301 0000 0000 0000 0001 0000  ....c...........
+00003490: 0003 0000 0013 0000 0073 0c00 0000 8800  .........s......
+000034a0: 7c00 6401 1900 8301 5300 2902 4e72 b100  |.d.....S.).Nr..
+000034b0: 0000 7223 0000 0029 0172 4b00 0000 2901  ..r#...).rK...).
+000034c0: da12 696e 7374 616e 6365 5f70 7265 6469  ..instance_predi
+000034d0: 6361 7465 7223 0000 0072 2400 0000 724c  cater#...r$...rL
+000034e0: 0000 00f6 0100 0073 0000 0000 7a3d 4772  .......s....z=Gr
+000034f0: 6170 6851 4c53 6368 656d 6147 656e 6572  aphQLSchemaGener
+00003500: 6174 6f72 2e66 696c 7465 725f 6c6f 6f6b  ator.filter_look
+00003510: 7570 5f6d 6f64 656c 732e 3c6c 6f63 616c  up_models.<local
+00003520: 733e 2e3c 6c61 6d62 6461 3e63 0100 0000  s>.<lambda>c....
+00003530: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
+00003540: 7308 0000 007c 0064 0119 0053 0029 024e  s....|.d...S.).N
+00003550: 72bc 0000 0072 2300 0000 2901 724b 0000  r....r#...).rK..
+00003560: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00003570: 724c 0000 00f8 0100 0073 0000 0000 72b9  rL.......s....r.
+00003580: 0000 0072 bb00 0000 72bc 0000 0072 0100  ...r....r....r..
+00003590: 0000 72c2 0000 0063 0100 0000 0000 0000  ..r....c........
+000035a0: 0100 0000 0400 0000 1300 0000 7314 0000  ............s...
+000035b0: 0074 007c 0088 0064 0119 0064 0083 0388  .t.|...d...d....
+000035c0: 016b 0653 0029 024e 727e 0000 0029 0172  .k.S.).Nr~...).r
+000035d0: 6900 0000 2901 724b 0000 0029 0272 c500  i...).rK...).r..
+000035e0: 0000 728c 0000 0072 2300 0000 7224 0000  ..r....r#...r$..
+000035f0: 0072 4c00 0000 0302 0000 7300 0000 0072  .rL.......s....r
+00003600: c100 0000 6301 0000 0000 0000 0001 0000  ....c...........
+00003610: 0004 0000 0013 0000 0073 1800 0000 7400  .........s....t.
+00003620: 7c00 6401 1900 8800 6402 1900 6400 8303  |.d.....d...d...
+00003630: 8801 6b06 5300 2903 4e72 b100 0000 72be  ..k.S.).Nr....r.
+00003640: 0000 0029 0172 6900 0000 2901 724b 0000  ...).ri...).rK..
+00003650: 0029 0272 c500 0000 728c 0000 0072 2300  .).r....r....r#.
+00003660: 0000 7224 0000 0072 4c00 0000 0802 0000  ..r$...rL.......
+00003670: 7300 0000 005a 0a61 6767 7265 6761 7465  s....Z.aggregate
+00003680: 6429 0772 4e00 0000 7264 0000 0072 6500  d).rN...rd...re.
+00003690: 0000 7219 0000 0072 4d00 0000 7266 0000  ..r....rM...rf..
+000036a0: 00da 1466 696c 7465 725f 6c6f 6f6b 7570  ...filter_lookup
+000036b0: 5f6d 6f64 656c 7329 0772 5d00 0000 72a8  _models).r]...r.
+000036c0: 0000 0072 c700 0000 7292 0000 0072 ae00  ...r....r....r..
+000036d0: 0000 5a0b 6974 656d 5f72 6573 756c 7472  ..Z.item_resultr
+000036e0: bd00 0000 7223 0000 0029 0372 c700 0000  ....r#...).r....
+000036f0: 72c5 0000 0072 8c00 0000 7224 0000 0072  r....r....r$...r
+00003700: c800 0000 ed01 0000 732c 0000 0000 0104  ........s,......
+00003710: 0212 0104 0208 0204 0116 0216 0208 0108  ................
+00003720: 010a 0218 0208 0104 0106 0114 0308 0104  ................
+00003730: 010c 010c 021c 020c 027a 2b47 7261 7068  .........z+Graph
+00003740: 514c 5363 6865 6d61 4765 6e65 7261 746f  QLSchemaGenerato
+00003750: 722e 6669 6c74 6572 5f6c 6f6f 6b75 705f  r.filter_lookup_
+00003760: 6d6f 6465 6c73 6305 0000 0000 0000 0008  modelsc.........
+00003770: 0000 0003 0000 0043 0000 0073 3e00 0000  .......C...s>...
+00003780: 7c04 6a00 6401 6402 8302 7d05 7c00 6a01  |.j.d.d...}.|.j.
+00003790: 7c01 7c02 8302 7d06 7c06 6a00 7c03 8301  |.|...}.|.j.|...
+000037a0: 7d07 7c07 6400 6b08 722e 6400 5300 7c05  }.|.d.k.r.d.S.|.
+000037b0: 723a 7402 7c07 8301 7d07 7c07 5300 2903  r:t.|...}.|.S.).
+000037c0: 4e72 3000 0000 4629 0372 8600 0000 72a0  Nr0...F).r....r.
+000037d0: 0000 0072 0300 0000 2908 725d 0000 0072  ...r....).r]...r
+000037e0: 9000 0000 726f 0000 0072 4800 0000 da07  ....ro...rH.....
+000037f0: 6f70 7469 6f6e 7372 3000 0000 72ad 0000  optionsr0...r...
+00003800: 0072 a700 0000 7223 0000 0072 2300 0000  .r....r#...r#...
+00003810: 7224 0000 00da 146d 6170 5f73 6f72 745f  r$.....map_sort_
+00003820: 6f72 6465 725f 6669 656c 6411 0200 0073  order_field....s
+00003830: 1000 0000 0001 0c02 0c01 0a02 0801 0402  ................
+00003840: 0401 0802 7a2b 4772 6170 6851 4c53 6368  ....z+GraphQLSch
+00003850: 656d 6147 656e 6572 6174 6f72 2e6d 6170  emaGenerator.map
+00003860: 5f73 6f72 745f 6f72 6465 725f 6669 656c  _sort_order_fiel
+00003870: 6463 0500 0000 0000 0000 0b00 0000 0500  dc..............
+00003880: 0000 0300 0000 7380 0000 0078 4e7c 0444  ......s....xN|.D
+00003890: 005d 467d 0574 007c 0583 017d 0674 0187  .]F}.t.|...}.t..
+000038a0: 0087 0187 0266 0364 0164 0284 087c 066a  .....f.d.d...|.j
+000038b0: 0283 0083 027d 0774 0364 0364 0284 007c  .....}.t.d.d...|
+000038c0: 0783 027d 0774 047c 0783 017d 077c 016a  ...}.t.|...}.|.j
+000038d0: 057c 078e 007d 0171 0657 0088 016a 0664  .|...}.q.W...j.d
+000038e0: 0419 007d 0874 0788 006a 087c 0883 027d  ...}.t...j.|...}
+000038f0: 0988 006a 096a 0a7c 0983 017d 0a74 0b7c  ...j.j.|...}.t.|
+00003900: 0a7c 0183 027d 017c 0153 0029 054e 6301  .|...}.|.S.).Nc.
+00003910: 0000 0000 0000 0001 0000 0006 0000 0013  ................
+00003920: 0000 0073 1800 0000 8802 6a00 8800 8801  ...s......j.....
+00003930: 7c00 6401 1900 7c00 6402 1900 8304 5300  |.d...|.d.....S.
+00003940: 2903 4e72 0100 0000 724a 0000 0029 0172  ).Nr....rJ...).r
+00003950: ca00 0000 2901 724b 0000 0029 0372 9000  ....).rK...).r..
+00003960: 0000 726f 0000 0072 5d00 0000 7223 0000  ..ro...r]...r#..
+00003970: 0072 2400 0000 724c 0000 0023 0200 0073  .r$...rL...#...s
+00003980: 0000 0000 7a36 4772 6170 6851 4c53 6368  ....z6GraphQLSch
+00003990: 656d 6147 656e 6572 6174 6f72 2e73 6f72  emaGenerator.sor
+000039a0: 745f 7175 6572 7973 6574 2e3c 6c6f 6361  t_queryset.<loca
+000039b0: 6c73 3e2e 3c6c 616d 6264 613e 6301 0000  ls>.<lambda>c...
+000039c0: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+000039d0: 0073 0800 0000 7c00 6400 6b09 5300 2901  .s....|.d.k.S.).
+000039e0: 4e72 2300 0000 2901 724b 0000 0072 2300  Nr#...).rK...r#.
+000039f0: 0000 7223 0000 0072 2400 0000 724c 0000  ..r#...r$...rL..
+00003a00: 0024 0200 0073 0000 0000 7201 0000 0029  .$...s....r....)
+00003a10: 0c72 4f00 0000 724d 0000 0072 4e00 0000  .rO...rM...rN...
+00003a20: 7265 0000 0072 6400 0000 da08 6f72 6465  re...rd.....orde
+00003a30: 725f 6279 7268 0000 0072 0e00 0000 7278  r_byrh...r....rx
+00003a40: 0000 0072 8400 0000 7286 0000 0072 1c00  ...r....r....r..
+00003a50: 0000 290b 725d 0000 0072 7100 0000 7290  ..).r]...rq...r.
+00003a60: 0000 0072 6f00 0000 da04 736f 7274 72b0  ...ro.....sortr.
+00003a70: 0000 005a 0969 7465 6d5f 6469 6374 72cb  ...Z.item_dictr.
+00003a80: 0000 0072 9500 0000 7248 0000 0072 6d00  ...r....rH...rm.
+00003a90: 0000 7223 0000 0029 0372 9000 0000 726f  ..r#...).r....ro
+00003aa0: 0000 0072 5d00 0000 7224 0000 00da 0d73  ...r]...r$.....s
+00003ab0: 6f72 745f 7175 6572 7973 6574 1f02 0000  ort_queryset....
+00003ac0: 7316 0000 0000 010a 0108 021a 010e 0108  s...............
+00003ad0: 020e 020a 010c 010c 010a 027a 2447 7261  ...........z$Gra
+00003ae0: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
+00003af0: 746f 722e 736f 7274 5f71 7565 7279 7365  tor.sort_queryse
+00003b00: 7463 0200 0000 0000 0000 0200 0000 0300  tc..............
+00003b10: 0000 4300 0000 730c 0000 007c 016a 0064  ..C...s....|.j.d
+00003b20: 0164 0283 0253 0029 034e 7235 0000 00e9  .d...S.).Nr5....
+00003b30: 1400 0000 2901 7286 0000 0029 0272 5d00  ....).r....).r].
+00003b40: 0000 da0a 7061 6769 6e61 7469 6f6e 7223  ....paginationr#
+00003b50: 0000 0072 2300 0000 7224 0000 00da 1467  ...r#...r$.....g
+00003b60: 6574 5f70 6167 696e 6174 696f 6e5f 6c69  et_pagination_li
+00003b70: 6d69 7430 0200 0073 0200 0000 0001 7a2b  mit0...s......z+
+00003b80: 4772 6170 6851 4c53 6368 656d 6147 656e  GraphQLSchemaGen
+00003b90: 6572 6174 6f72 2e67 6574 5f70 6167 696e  erator.get_pagin
+00003ba0: 6174 696f 6e5f 6c69 6d69 7463 0300 0000  ation_limitc....
+00003bb0: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
+00003bc0: 734e 0000 007c 006a 007c 0283 017d 0364  sN...|.j.|...}.d
+00003bd0: 017c 026b 0672 227c 016a 017c 0264 0119  .|.k.r"|.j.|.d..
+00003be0: 0083 017d 016e 1e64 027c 026b 0672 407c  ...}.n.d.|.k.r@|
+00003bf0: 016a 017c 0264 0219 0064 0318 007c 0314  .j.|.d...d...|..
+00003c00: 0083 017d 017c 016a 027c 0383 017d 017c  ...}.|.j.|...}.|
+00003c10: 0153 0029 044e 7234 0000 0072 3300 0000  .S.).Nr4...r3...
+00003c20: 724a 0000 0029 0372 d000 0000 7234 0000  rJ...).r....r4..
+00003c30: 0072 3500 0000 2904 725d 0000 0072 7100  .r5...).r]...rq.
+00003c40: 0000 72cf 0000 0072 3500 0000 7223 0000  ..r....r5...r#..
+00003c50: 0072 2300 0000 7224 0000 00da 1170 6167  .r#...r$.....pag
+00003c60: 696e 6174 655f 7175 6572 7973 6574 3302  inate_queryset3.
+00003c70: 0000 730e 0000 0000 010a 0208 0110 0108  ..s.............
+00003c80: 0116 020a 027a 2847 7261 7068 514c 5363  .....z(GraphQLSc
+00003c90: 6865 6d61 4765 6e65 7261 746f 722e 7061  hemaGenerator.pa
+00003ca0: 6769 6e61 7465 5f71 7565 7279 7365 7472  ginate_querysetr
+00003cb0: 4a00 0000 6304 0000 0000 0000 000f 0000  J...c...........
+00003cc0: 0007 0000 0043 0000 0073 1601 0000 7c03  .....C...s....|.
+00003cd0: 6401 6b01 7d04 7400 7c01 6a01 7c02 6a02  d.k.}.t.|.j.|.j.
+00003ce0: 8302 7d05 7403 7c05 8301 7d06 7c04 722e  ..}.t.|...}.|.r.
+00003cf0: 6402 6a04 7c06 7c03 8302 6e0a 6403 6a04  d.j.|.|...n.d.j.
+00003d00: 7c06 7c03 8302 7d07 7c07 7c00 6a05 6b06  |.|...}.|.|.j.k.
+00003d10: 7254 7406 6a07 7c00 6a05 7c07 1900 8301  rTt.j.|.j.|.....
+00003d20: 5300 6900 7d08 7834 7c02 6a08 4400 5d2a  S.i.}.x4|.j.D.]*
+00003d30: 7d09 7c00 6a09 7c01 7c02 7c09 7c04 7c03  }.|.j.|.|.|.|.|.
+00003d40: 8305 7d0a 7403 7c09 6a0a 8301 7d0b 7c0a  ..}.t.|.j...}.|.
+00003d50: 8300 7c08 7c0b 3c00 7160 5700 7c04 72f4  ..|.|.<.q`W.|.r.
+00003d60: 784a 7c00 6a0b 7c01 7c02 8302 4400 5d3a  xJ|.j.|.|...D.]:
+00003d70: 7d0c 7c0c 6404 1900 740c 6b03 72b2 71a0  }.|.d...t.k.r.q.
+00003d80: 7c00 6a0d 7c01 7c02 7c0c 7c04 7c03 8305  |.j.|.|.|.|.|...
+00003d90: 7d0d 7403 7c0c 6405 1900 8301 7d0b 7c0d  }.t.|.d.....}.|.
+00003da0: 8300 7c08 7c0b 3c00 71a0 5700 7c00 6a0e  ..|.|.<.q.W.|.j.
+00003db0: 7c01 7c02 7c03 6406 1700 8303 7c08 6407  |.|.|.d.....|.d.
+00003dc0: 3c00 740f 7c07 7410 6601 7c08 8303 7d0e  <.t.|.t.f.|...}.
+00003dd0: 7c0e 7c00 6a05 7c07 3c00 7406 6a07 7c0e  |.|.j.|.<.t.j.|.
+00003de0: 8301 5300 2908 4ee9 0400 0000 7a1f 4d6f  ..S.).N.....z.Mo
+00003df0: 6465 6c7b 7d44 6570 7468 7b7d 4e65 7374  del{}Depth{}Nest
+00003e00: 6564 4669 6c74 6572 7354 7970 657a 194d  edFiltersTypez.M
+00003e10: 6f64 656c 7b7d 4465 7074 687b 7d46 696c  odel{}Depth{}Fil
+00003e20: 7465 7273 5479 7065 7279 0000 0072 4800  tersTypery...rH.
+00003e30: 0000 724a 0000 0072 a400 0000 2911 720e  ..rJ...r....).r.
+00003e40: 0000 0072 7800 0000 7285 0000 0072 4900  ...rx...r....rI.
+00003e50: 0000 da06 666f 726d 6174 7256 0000 0072  ....formatrV...r
+00003e60: 2e00 0000 da04 4c69 7374 729e 0000 00da  ......Listr.....
+00003e70: 1c67 6574 5f6d 6f64 656c 5f66 6965 6c64  .get_model_field
+00003e80: 5f66 696c 7465 7273 5f74 7970 6572 4800  _filters_typerH.
+00003e90: 0000 72a1 0000 0072 0700 0000 da23 6765  ..r....r.....#ge
+00003ea0: 745f 6d6f 6465 6c5f 7265 6c61 7469 6f6e  t_model_relation
+00003eb0: 7368 6970 5f66 696c 7465 7273 5f74 7970  ship_filters_typ
+00003ec0: 65da 1667 6574 5f6d 6f64 656c 5f66 696c  e..get_model_fil
+00003ed0: 7465 7273 5f74 7970 6572 ab00 0000 721f  ters_typer....r.
+00003ee0: 0000 0029 0f72 5d00 0000 7290 0000 0072  ...).r]...r....r
+00003ef0: 6f00 0000 da05 6465 7074 68da 0e77 6974  o.....depth..wit
+00003f00: 685f 7265 6c61 7469 6f6e 73da 0a74 6162  h_relations..tab
+00003f10: 6c65 5f6e 616d 65da 0a6d 6f64 656c 5f6e  le_name..model_n
+00003f20: 616d 65da 0863 6c73 5f6e 616d 65da 0561  ame..cls_name..a
+00003f30: 7474 7273 72a7 0000 00da 1363 6f6c 756d  ttrsr......colum
+00003f40: 6e5f 6669 6c74 6572 735f 7479 7065 da09  n_filters_type..
+00003f50: 6174 7472 5f6e 616d 6572 9700 0000 5a19  attr_namer....Z.
+00003f60: 7265 6c61 7469 6f6e 7368 6970 5f66 696c  relationship_fil
+00003f70: 7465 7273 5f74 7970 65da 0363 6c73 7223  ters_type..clsr#
+00003f80: 0000 0072 2300 0000 7224 0000 0072 d700  ...r#...r$...r..
+00003f90: 0000 3f02 0000 732e 0000 0000 0108 010e  ..?...s.........
+00003fa0: 0108 0110 010c 020a 0110 0204 020c 0112  ................
+00003fb0: 010a 010e 0204 0112 010c 0102 0212 010c  ................
+00003fc0: 010e 0216 020e 010a 017a 2d47 7261 7068  .........z-Graph
+00003fd0: 514c 5363 6865 6d61 4765 6e65 7261 746f  QLSchemaGenerato
+00003fe0: 722e 6765 745f 6d6f 6465 6c5f 6669 6c74  r.get_model_filt
+00003ff0: 6572 735f 7479 7065 6306 0000 0000 0000  ers_typec.......
+00004000: 0013 0000 0006 0000 0043 0000 0073 0c01  .........C...s..
+00004010: 0000 7400 7c01 6a01 7c02 6a02 8302 7d06  ..t.|.j.|.j...}.
+00004020: 7403 7c06 8301 7d07 7403 7c03 6a04 8301  t.|...}.t.|.j...
+00004030: 7d08 7c04 7232 6401 6a05 7c07 7c08 7c05  }.|.r2d.j.|.|.|.
+00004040: 8303 6e0c 6402 6a05 7c07 7c08 7c05 8303  ..n.d.j.|.|.|...
+00004050: 7d09 7c09 7c00 6a06 6b06 7254 7c00 6a06  }.|.|.j.k.rT|.j.
+00004060: 7c09 1900 5300 6900 7d0a 7407 7c03 6a08  |...S.i.}.t.|.j.
+00004070: 8301 7d0b 7834 7c0b 6403 1900 4400 5d28  ..}.x4|.d...D.](
+00004080: 7d0c 7409 6a0a 6a0b 7c0c 8301 7d0d 7409  }.t.j.j.|...}.t.
+00004090: 6a0c 6a0b 7c0c 740d 8300 8302 7d0e 7c0e  j.j.|.t.....}.|.
+000040a0: 7c0a 7c0d 3c00 716c 5700 7c04 72f0 7852  |.|.<.qlW.|.r.xR
+000040b0: 7c00 6a0e 7c01 7c02 8302 4400 5d42 7d0f  |.j.|.|...D.]B}.
+000040c0: 7c0f 6404 1900 740f 6b03 73aa 7c0f 6405  |.d...t.k.s.|.d.
+000040d0: 1900 7c08 6b03 72c8 71aa 7c0f 6406 1900  ..|.k.r.q.|.d...
+000040e0: 7d10 7c00 6a10 7c01 7c10 7c05 6407 1700  }.|.j.|.|.|.d...
+000040f0: 8303 7d11 7c11 7c0a 6408 3c00 5000 71aa  ..}.|.|.d.<.P.q.
+00004100: 5700 7408 7c09 7411 6601 7c0a 8303 7d12  W.t.|.t.f.|...}.
+00004110: 7c12 7c00 6a06 7c09 3c00 7c12 5300 2909  |.|.j.|.<.|.S.).
+00004120: 4e7a 274d 6f64 656c 7b7d 436f 6c75 6d6e  Nz'Model{}Column
+00004130: 7b7d 4465 7074 687b 7d4e 6573 7465 6446  {}Depth{}NestedF
+00004140: 696c 7465 7273 5479 7065 7a21 4d6f 6465  iltersTypez!Mode
+00004150: 6c7b 7d43 6f6c 756d 6e7b 7d44 6570 7468  l{}Column{}Depth
+00004160: 7b7d 4669 6c74 6572 7354 7970 6572 0f00  {}FiltersTyper..
+00004170: 0000 7279 0000 0072 7b00 0000 727d 0000  ..ry...r{...r}..
+00004180: 0072 4a00 0000 72a6 0000 0029 1272 0e00  .rJ...r....).r..
+00004190: 0000 7278 0000 0072 8500 0000 7249 0000  ..rx...r....rI..
+000041a0: 0072 4800 0000 72d3 0000 0072 5700 0000  .rH...r....rW...
+000041b0: 7210 0000 0072 ab00 0000 720f 0000 005a  r....r....r....Z
+000041c0: 0367 716c 7286 0000 00da 0a67 716c 5f73  .gqlr......gql_s
+000041d0: 6361 6c61 7272 1a00 0000 72a1 0000 0072  calarr....r....r
+000041e0: 0600 0000 72d7 0000 0072 2500 0000 2913  ....r....r%...).
+000041f0: 725d 0000 0072 9000 0000 726f 0000 0072  r]...r....ro...r
+00004200: a700 0000 72d9 0000 0072 d800 0000 72da  ....r....r....r.
+00004210: 0000 0072 db00 0000 da0b 636f 6c75 6d6e  ...r......column
+00004220: 5f6e 616d 6572 dc00 0000 72dd 0000 0072  _namer....r....r
+00004230: b000 0000 72a8 0000 005a 0a67 716c 5f6c  ....r....Z.gql_l
+00004240: 6f6f 6b75 7072 e100 0000 7297 0000 0072  ookupr....r....r
+00004250: af00 0000 72de 0000 0072 e000 0000 7223  ....r....r....r#
+00004260: 0000 0072 2300 0000 7224 0000 0072 d500  ...r#...r$...r..
+00004270: 0000 5f02 0000 7330 0000 0000 010e 0108  .._...s0........
+00004280: 010a 0112 010e 020a 010a 0204 010a 020e  ................
+00004290: 010c 0110 010c 0204 0112 0118 0102 0208  ................
+000042a0: 0112 0108 0106 020e 010a 017a 3347 7261  ...........z3Gra
+000042b0: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
+000042c0: 746f 722e 6765 745f 6d6f 6465 6c5f 6669  tor.get_model_fi
+000042d0: 656c 645f 6669 6c74 6572 735f 7479 7065  eld_filters_type
+000042e0: 6306 0000 0000 0000 000d 0000 0005 0000  c...............
+000042f0: 0043 0000 0073 9400 0000 7400 7c01 6a01  .C...s....t.|.j.
+00004300: 7c02 6a02 8302 7d06 7403 7c06 8301 7d07  |.j...}.t.|...}.
+00004310: 7403 7c03 6401 1900 8301 7d08 7c04 7234  t.|.d.....}.|.r4
+00004320: 6402 6a04 7c07 7c08 7c05 8303 6e0c 6403  d.j.|.|.|...n.d.
+00004330: 6a04 7c07 7c08 7c05 8303 7d09 7c09 7c00  j.|.|.|...}.|.|.
+00004340: 6a05 6b06 7256 7c00 6a05 7c09 1900 5300  j.k.rV|.j.|...S.
+00004350: 6900 7d0a 7c00 6a06 7c01 7c03 6404 1900  i.}.|.j.|.|.d...
+00004360: 7c05 6405 1700 8303 7d0b 7c0b 7c0a 6406  |.d.....}.|.|.d.
+00004370: 3c00 7407 7c09 7408 6601 7c0a 8303 7d0c  <.t.|.t.f.|...}.
+00004380: 7c0c 7c00 6a05 7c09 3c00 7c0c 5300 2907  |.|.j.|.<.|.S.).
+00004390: 4e72 4800 0000 7a2c 4d6f 6465 6c7b 7d43  NrH...z,Model{}C
+000043a0: 6f6c 756d 6e7b 7d44 6570 7468 7b7d 4e65  olumn{}Depth{}Ne
+000043b0: 7374 6564 5265 6c61 7469 6f6e 7368 6970  stedRelationship
+000043c0: 5479 7065 7a26 4d6f 6465 6c7b 7d43 6f6c  Typez&Model{}Col
+000043d0: 756d 6e7b 7d44 6570 7468 7b7d 5265 6c61  umn{}Depth{}Rela
+000043e0: 7469 6f6e 7368 6970 5479 7065 727d 0000  tionshipTyper}..
+000043f0: 0072 4a00 0000 72a6 0000 0029 0972 0e00  .rJ...r....).r..
+00004400: 0000 7278 0000 0072 8500 0000 7249 0000  ..rx...r....rI..
+00004410: 0072 d300 0000 7258 0000 0072 d700 0000  .r....rX...r....
+00004420: 72ab 0000 0072 2600 0000 290d 725d 0000  r....r&...).r]..
+00004430: 0072 9000 0000 726f 0000 0072 9700 0000  .r....ro...r....
+00004440: 72d9 0000 0072 d800 0000 72da 0000 0072  r....r....r....r
+00004450: db00 0000 da10 7265 6c61 7469 6f6e 7368  ......relationsh
+00004460: 6970 5f6b 6579 72dc 0000 0072 dd00 0000  ip_keyr....r....
+00004470: da0c 6c6f 6f6b 7570 735f 7479 7065 72e0  ..lookups_typer.
+00004480: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00004490: 0000 72d6 0000 007f 0200 0073 1a00 0000  ..r........s....
+000044a0: 0001 0e01 0801 0c01 1201 0e02 0a01 0a02  ................
+000044b0: 0402 1601 0802 0e01 0a01 7a3a 4772 6170  ..........z:Grap
+000044c0: 6851 4c53 6368 656d 6147 656e 6572 6174  hQLSchemaGenerat
+000044d0: 6f72 2e67 6574 5f6d 6f64 656c 5f72 656c  or.get_model_rel
+000044e0: 6174 696f 6e73 6869 705f 6669 6c74 6572  ationship_filter
+000044f0: 735f 7479 7065 6304 0000 0000 0000 000f  s_typec.........
+00004500: 0000 0007 0000 0043 0000 0073 f400 0000  .......C...s....
+00004510: 7c03 6401 6b01 7d04 7400 7c01 6a01 7c02  |.d.k.}.t.|.j.|.
+00004520: 6a02 8302 7d05 7403 7c05 8301 7d06 7c04  j...}.t.|...}.|.
+00004530: 722e 6402 6a04 7c06 7c03 8302 6e0a 6403  r.d.j.|.|...n.d.
+00004540: 6a04 7c06 7c03 8302 7d07 7c07 7c00 6a05  j.|.|...}.|.|.j.
+00004550: 6b06 724e 7c00 6a05 7c07 1900 5300 6900  k.rN|.j.|...S.i.
+00004560: 7d08 7834 7c02 6a06 4400 5d2a 7d09 7c00  }.x4|.j.D.]*}.|.
+00004570: 6a07 7c01 7c02 7c09 7c04 7c03 8305 7d0a  j.|.|.|.|.|...}.
+00004580: 7403 7c09 6a08 8301 7d0b 7c0a 8300 7c08  t.|.j...}.|...|.
+00004590: 7c0b 3c00 715a 5700 7c04 72d8 784a 7c00  |.<.qZW.|.r.xJ|.
+000045a0: 6a09 7c01 7c02 8302 4400 5d3a 7d0c 7c0c  j.|.|...D.]:}.|.
+000045b0: 6404 1900 740a 6b03 72ac 719a 7c00 6a0b  d...t.k.r.q.|.j.
+000045c0: 7c01 7c02 7c0c 7c04 7c03 8305 7d0d 7403  |.|.|.|.|...}.t.
+000045d0: 7c0c 6405 1900 8301 7d0b 7c0d 8300 7c08  |.d.....}.|...|.
+000045e0: 7c0b 3c00 719a 5700 740c 7c07 740d 6601  |.<.q.W.t.|.t.f.
+000045f0: 7c08 8303 7d0e 7c0e 7c00 6a05 7c07 3c00  |...}.|.|.j.|.<.
+00004600: 7c0e 5300 2906 4e72 d200 0000 7a1f 4d6f  |.S.).Nr....z.Mo
+00004610: 6465 6c7b 7d44 6570 7468 7b7d 4e65 7374  del{}Depth{}Nest
+00004620: 6564 4c6f 6f6b 7570 7354 7970 657a 194d  edLookupsTypez.M
+00004630: 6f64 656c 7b7d 4465 7074 687b 7d4c 6f6f  odel{}Depth{}Loo
+00004640: 6b75 7073 5479 7065 7279 0000 0072 4800  kupsTypery...rH.
+00004650: 0000 290e 720e 0000 0072 7800 0000 7285  ..).r....rx...r.
+00004660: 0000 0072 4900 0000 72d3 0000 0072 5900  ...rI...r....rY.
+00004670: 0000 729e 0000 00da 1c67 6574 5f6d 6f64  ..r......get_mod
+00004680: 656c 5f66 6965 6c64 5f6c 6f6f 6b75 7073  el_field_lookups
+00004690: 5f74 7970 6572 4800 0000 72a1 0000 0072  _typerH...r....r
+000046a0: 0700 0000 da23 6765 745f 6d6f 6465 6c5f  .....#get_model_
+000046b0: 7265 6c61 7469 6f6e 7368 6970 5f6c 6f6f  relationship_loo
+000046c0: 6b75 7073 5f74 7970 6572 ab00 0000 7227  kups_typer....r'
+000046d0: 0000 0029 0f72 5d00 0000 7290 0000 0072  ...).r]...r....r
+000046e0: 6f00 0000 72d8 0000 0072 d900 0000 72da  o...r....r....r.
+000046f0: 0000 0072 db00 0000 72dc 0000 0072 dd00  ...r....r....r..
+00004700: 0000 72a7 0000 005a 1363 6f6c 756d 6e5f  ..r....Z.column_
+00004710: 6c6f 6f6b 7570 735f 7479 7065 72df 0000  lookups_typer...
+00004720: 0072 9700 0000 5a19 7265 6c61 7469 6f6e  .r....Z.relation
+00004730: 7368 6970 5f6c 6f6f 6b75 7073 5f74 7970  ship_lookups_typ
+00004740: 6572 e000 0000 7223 0000 0072 2300 0000  er....r#...r#...
+00004750: 7224 0000 00da 1667 6574 5f6d 6f64 656c  r$.....get_model
+00004760: 5f6c 6f6f 6b75 7073 5f74 7970 6592 0200  _lookups_type...
+00004770: 0073 2c00 0000 0001 0801 0e01 0801 1001  .s,.............
+00004780: 0c02 0a01 0a02 0402 0c01 1201 0a01 0e02  ................
+00004790: 0401 1201 0c01 0202 1201 0c01 0e02 0e01  ................
+000047a0: 0a01 7a2d 4772 6170 6851 4c53 6368 656d  ..z-GraphQLSchem
+000047b0: 6147 656e 6572 6174 6f72 2e67 6574 5f6d  aGenerator.get_m
+000047c0: 6f64 656c 5f6c 6f6f 6b75 7073 5f74 7970  odel_lookups_typ
+000047d0: 6563 0600 0000 0000 0000 0f00 0000 0600  ec..............
+000047e0: 0000 4300 0000 73dc 0000 0074 007c 016a  ..C...s....t.|.j
+000047f0: 017c 026a 0283 027d 0674 037c 0683 017d  .|.j...}.t.|...}
+00004800: 0774 037c 036a 0483 017d 087c 0472 3264  .t.|.j...}.|.r2d
+00004810: 016a 057c 077c 087c 0583 036e 0c64 026a  .j.|.|.|...n.d.j
+00004820: 057c 077c 087c 0583 037d 097c 097c 006a  .|.|.|...}.|.|.j
+00004830: 066b 0672 547c 006a 067c 0919 0053 0074  .k.rT|.j.|...S.t
+00004840: 076a 0883 0074 076a 0883 0064 039c 027d  .j...t.j...d...}
+00004850: 0a7c 0472 c078 547c 006a 097c 017c 0283  .|.r.xT|.j.|.|..
+00004860: 0244 005d 447d 0b7c 0b64 0419 0074 0a6b  .D.]D}.|.d...t.k
+00004870: 0373 787c 0b64 0519 007c 086b 0372 9671  .sx|.d...|.k.r.q
+00004880: 787c 0b64 0619 007d 0c7c 006a 0b7c 017c  x|.d...}.|.j.|.|
+00004890: 0c7c 0564 0717 0083 037d 0d7c 0d83 007c  .|.d.....}.|...|
+000048a0: 0a64 083c 0050 0071 7857 0074 0c7c 0974  .d.<.P.qxW.t.|.t
+000048b0: 0d66 017c 0a83 037d 0e7c 0e7c 006a 067c  .f.|...}.|.|.j.|
+000048c0: 093c 007c 0e53 0029 094e 7a2c 4d6f 6465  .<.|.S.).Nz,Mode
+000048d0: 6c7b 7d43 6f6c 756d 6e7b 7d44 6570 7468  l{}Column{}Depth
+000048e0: 7b7d 4e65 7374 6564 4c6f 6f6b 7570 7346  {}NestedLookupsF
+000048f0: 6965 6c64 5479 7065 7a26 4d6f 6465 6c7b  ieldTypez&Model{
+00004900: 7d43 6f6c 756d 6e7b 7d44 6570 7468 7b7d  }Column{}Depth{}
+00004910: 4c6f 6f6b 7570 7346 6965 6c64 5479 7065  LookupsFieldType
+00004920: 2902 72b9 0000 0072 ba00 0000 7279 0000  ).r....r....ry..
+00004930: 0072 7b00 0000 727d 0000 0072 4a00 0000  .r{...r}...rJ...
+00004940: 72a6 0000 0029 0e72 0e00 0000 7278 0000  r....).r....rx..
+00004950: 0072 8500 0000 7249 0000 0072 4800 0000  .r....rI...rH...
+00004960: 72d3 0000 0072 5a00 0000 722e 0000 0072  r....rZ...r....r
+00004970: 2f00 0000 72a1 0000 0072 0600 0000 72e7  /...r....r....r.
+00004980: 0000 0072 ab00 0000 7228 0000 0029 0f72  ...r....r(...).r
+00004990: 5d00 0000 7290 0000 0072 6f00 0000 72a7  ]...r....ro...r.
+000049a0: 0000 0072 d900 0000 72d8 0000 0072 da00  ...r....r....r..
+000049b0: 0000 72db 0000 0072 e200 0000 72dc 0000  ..r....r....r...
+000049c0: 0072 dd00 0000 7297 0000 0072 af00 0000  .r....r....r....
+000049d0: 72e4 0000 0072 e000 0000 7223 0000 0072  r....r....r#...r
+000049e0: 2300 0000 7224 0000 0072 e500 0000 b002  #...r$...r......
+000049f0: 0000 7328 0000 0000 010e 0108 010a 0112  ..s(............
+00004a00: 010e 020a 010a 0306 010c 0304 0112 0118  ................
+00004a10: 0102 0208 0112 010a 0106 020e 010a 017a  ...............z
+00004a20: 3347 7261 7068 514c 5363 6865 6d61 4765  3GraphQLSchemaGe
+00004a30: 6e65 7261 746f 722e 6765 745f 6d6f 6465  nerator.get_mode
+00004a40: 6c5f 6669 656c 645f 6c6f 6f6b 7570 735f  l_field_lookups_
+00004a50: 7479 7065 6306 0000 0000 0000 000d 0000  typec...........
+00004a60: 0005 0000 0043 0000 0073 9c00 0000 7400  .....C...s....t.
+00004a70: 7c01 6a01 7c02 6a02 8302 7d06 7403 7c06  |.j.|.j...}.t.|.
+00004a80: 8301 7d07 7403 7c03 6401 1900 8301 7d08  ..}.t.|.d.....}.
+00004a90: 7c04 7234 6402 6a04 7c07 7c08 7c05 8303  |.r4d.j.|.|.|...
+00004aa0: 6e0c 6403 6a04 7c07 7c08 7c05 8303 7d09  n.d.j.|.|.|...}.
+00004ab0: 7c09 7c00 6a05 6b06 7256 7c00 6a05 7c09  |.|.j.k.rV|.j.|.
+00004ac0: 1900 5300 6404 7406 8300 6901 7d0a 7c00  ..S.d.t...i.}.|.
+00004ad0: 6a07 7c01 7c03 6405 1900 7c05 6406 1700  j.|.|.d...|.d...
+00004ae0: 8303 7d0b 7c0b 8300 7c0a 6407 3c00 7408  ..}.|...|.d.<.t.
+00004af0: 7c09 7409 6601 7c0a 8303 7d0c 7c0c 7c00  |.t.f.|...}.|.|.
+00004b00: 6a05 7c09 3c00 7c0c 5300 2908 4e72 4800  j.|.<.|.S.).NrH.
+00004b10: 0000 7a33 4d6f 6465 6c7b 7d43 6f6c 756d  ..z3Model{}Colum
+00004b20: 6e7b 7d44 6570 7468 7b7d 4e65 7374 6564  n{}Depth{}Nested
+00004b30: 4c6f 6f6b 7570 7352 656c 6174 696f 6e73  LookupsRelations
+00004b40: 6869 7054 7970 657a 2d4d 6f64 656c 7b7d  hipTypez-Model{}
+00004b50: 436f 6c75 6d6e 7b7d 4465 7074 687b 7d4c  Column{}Depth{}L
+00004b60: 6f6f 6b75 7073 5265 6c61 7469 6f6e 7368  ookupsRelationsh
+00004b70: 6970 5479 7065 72bf 0000 0072 7d00 0000  ipTyper....r}...
+00004b80: 724a 0000 0072 a600 0000 290a 720e 0000  rJ...r....).r...
+00004b90: 0072 7800 0000 7285 0000 0072 4900 0000  .rx...r....rI...
+00004ba0: 72d3 0000 0072 5b00 0000 723f 0000 0072  r....r[...r?...r
+00004bb0: e700 0000 72ab 0000 0072 2900 0000 290d  ....r....r)...).
+00004bc0: 725d 0000 0072 9000 0000 726f 0000 0072  r]...r....ro...r
+00004bd0: 9700 0000 72d9 0000 0072 d800 0000 72da  ....r....r....r.
+00004be0: 0000 0072 db00 0000 72e3 0000 0072 dc00  ...r....r....r..
+00004bf0: 0000 72dd 0000 0072 e400 0000 72e0 0000  ..r....r....r...
+00004c00: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00004c10: 72e6 0000 00cd 0200 0073 1a00 0000 0001  r........s......
+00004c20: 0e01 0801 0c01 1201 0e02 0a01 0a03 0a03  ................
+00004c30: 1601 0a02 0e01 0a01 7a3a 4772 6170 6851  ........z:GraphQ
+00004c40: 4c53 6368 656d 6147 656e 6572 6174 6f72  LSchemaGenerator
+00004c50: 2e67 6574 5f6d 6f64 656c 5f72 656c 6174  .get_model_relat
+00004c60: 696f 6e73 6869 705f 6c6f 6f6b 7570 735f  ionship_lookups_
+00004c70: 7479 7065 6303 0000 0000 0000 000a 0000  typec...........
+00004c80: 0004 0000 0043 0000 0073 8400 0000 7400  .....C...s....t.
+00004c90: 7c01 6a01 7c02 6a02 8302 7d03 7403 7c03  |.j.|.j...}.t.|.
+00004ca0: 8301 7d04 6401 6a04 7c04 8301 7d05 7c05  ..}.d.j.|...}.|.
+00004cb0: 7c00 6a05 6b06 723a 7406 6a07 7c00 6a05  |.j.k.r:t.j.|.j.
+00004cc0: 7c05 1900 8301 5300 6900 7d06 7822 7c02  |.....S.i.}.x"|.
+00004cd0: 6a08 4400 5d18 7d07 7403 7c07 6a09 8301  j.D.].}.t.|.j...
+00004ce0: 7d08 740a 8300 7c06 7c08 3c00 7146 5700  }.t...|.|.<.qFW.
+00004cf0: 740b 7c05 740c 6601 7c06 8303 7d09 7c09  t.|.t.f.|...}.|.
+00004d00: 7c00 6a05 7c05 3c00 7406 6a07 7c09 8301  |.j.|.<.t.j.|...
+00004d10: 5300 2902 4e7a 0f4d 6f64 656c 7b7d 536f  S.).Nz.Model{}So
+00004d20: 7274 5479 7065 290d 720e 0000 0072 7800  rtType).r....rx.
+00004d30: 0000 7285 0000 0072 4900 0000 72d3 0000  ..r....rI...r...
+00004d40: 0072 5c00 0000 722e 0000 0072 d400 0000  .r\...r....r....
+00004d50: 729e 0000 0072 4800 0000 722c 0000 0072  r....rH...r,...r
+00004d60: ab00 0000 722a 0000 0029 0a72 5d00 0000  ....r*...).r]...
+00004d70: 7290 0000 0072 6f00 0000 72da 0000 0072  r....ro...r....r
+00004d80: db00 0000 72dc 0000 0072 dd00 0000 72a7  ....r....r....r.
+00004d90: 0000 0072 df00 0000 72e0 0000 0072 2300  ...r....r....r#.
+00004da0: 0000 7223 0000 0072 2400 0000 da13 6765  ..r#...r$.....ge
+00004db0: 745f 6d6f 6465 6c5f 736f 7274 5f74 7970  t_model_sort_typ
+00004dc0: 65e2 0200 0073 1800 0000 0001 0e01 0801  e....s..........
+00004dd0: 0a02 0a01 1002 0402 0c01 0a01 0e02 0e01  ................
+00004de0: 0a01 7a2a 4772 6170 6851 4c53 6368 656d  ..z*GraphQLSchem
+00004df0: 6147 656e 6572 6174 6f72 2e67 6574 5f6d  aGenerator.get_m
+00004e00: 6f64 656c 5f73 6f72 745f 7479 7065 6303  odel_sort_typec.
+00004e10: 0000 0000 0000 0008 0000 0004 0000 0043  ...............C
+00004e20: 0000 0073 5200 0000 7400 7c01 6a01 7c02  ...sR...t.|.j.|.
+00004e30: 6a02 8302 7d03 7403 7c03 8301 7d04 6900  j...}.t.|...}.i.
+00004e40: 7d05 7822 7c02 6a04 4400 5d18 7d06 7403  }.x"|.j.D.].}.t.
+00004e50: 7c06 6a05 8301 7d07 7406 8300 7c05 7c07  |.j...}.t...|.|.
+00004e60: 3c00 7122 5700 7407 6401 6a08 7c04 8301  <.q"W.t.d.j.|...
+00004e70: 7409 6601 7c05 8303 5300 2902 4e7a 164d  t.f.|...S.).Nz.M
+00004e80: 6f64 656c 7b7d 5265 636f 7264 4174 7472  odel{}RecordAttr
+00004e90: 7354 7970 6529 0a72 0e00 0000 7278 0000  sType).r....rx..
+00004ea0: 0072 8500 0000 7249 0000 0072 9e00 0000  .r....rI...r....
+00004eb0: 7248 0000 0072 1a00 0000 72ab 0000 0072  rH...r....r....r
+00004ec0: d300 0000 722b 0000 0029 0872 5d00 0000  ....r+...).r]...
+00004ed0: 7290 0000 0072 6f00 0000 72da 0000 0072  r....ro...r....r
+00004ee0: 4800 0000 72dd 0000 0072 a700 0000 72df  H...r....r....r.
+00004ef0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00004f00: 0000 da14 6765 745f 6d6f 6465 6c5f 6174  ....get_model_at
+00004f10: 7472 735f 7479 7065 f402 0000 730e 0000  trs_type....s...
+00004f20: 0000 010e 0108 0104 020c 010a 010e 027a  ...............z
+00004f30: 2b47 7261 7068 514c 5363 6865 6d61 4765  +GraphQLSchemaGe
+00004f40: 6e65 7261 746f 722e 6765 745f 6d6f 6465  nerator.get_mode
+00004f50: 6c5f 6174 7472 735f 7479 7065 6303 0000  l_attrs_typec...
+00004f60: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
+00004f70: 0073 6400 0000 6401 7d03 7c01 6a00 6401  .sd...d.}.|.j.d.
+00004f80: 1900 7d04 7850 7c02 4400 5d48 7d05 783a  ..}.xP|.D.]H}.x:
+00004f90: 7c04 6a01 6a02 4400 5d2e 7d06 7c06 6a03  |.j.j.D.].}.|.j.
+00004fa0: 6a04 7c05 6b02 7222 7c03 7405 7c02 8301  j.|.k.r"|.t.|...
+00004fb0: 6402 1800 6b02 724a 7c06 6a01 6a02 5300  d...k.rJ|.j.j.S.
+00004fc0: 7c06 7d04 5000 7122 5700 7c03 6402 3700  |.}.P.q"W.|.d.7.
+00004fd0: 7d03 7114 5700 6400 5300 2903 4e72 0100  }.q.W.d.S.).Nr..
+00004fe0: 0000 724a 0000 0029 06da 0a66 6965 6c64  ..rJ...)...field
+00004ff0: 5f61 7374 73da 0d73 656c 6563 7469 6f6e  _asts..selection
+00005000: 5f73 6574 da0a 7365 6c65 6374 696f 6e73  _set..selections
+00005010: 7248 0000 0072 bc00 0000 7266 0000 0029  rH...r....rf...)
+00005020: 0772 5d00 0000 da04 696e 666f da04 7061  .r].....info..pa
+00005030: 7468 da01 695a 0d63 7572 7265 6e74 5f66  th..iZ.current_f
+00005040: 6965 6c64 da09 7061 7468 5f69 7465 6dda  ield..path_item.
+00005050: 0973 656c 6563 7469 6f6e 7223 0000 0072  .selectionr#...r
+00005060: 2300 0000 7224 0000 00da 0e67 6574 5f73  #...r$.....get_s
+00005070: 656c 6563 7469 6f6e 73ff 0200 0073 1400  elections....s..
+00005080: 0000 0001 0401 0a02 0a01 0e01 0c01 1001  ................
+00005090: 0802 0401 0602 7a25 4772 6170 6851 4c53  ......z%GraphQLS
+000050a0: 6368 656d 6147 656e 6572 6174 6f72 2e67  chemaGenerator.g
+000050b0: 6574 5f73 656c 6563 7469 6f6e 7363 0a00  et_selectionsc..
+000050c0: 0000 0000 0000 1b00 0000 1000 0000 0300  ................
+000050d0: 0000 7350 0200 0090 0279 207c 0570 0a67  ..sP.....y |.p.g
+000050e0: 007d 057c 0670 1267 007d 067c 0770 1a67  .}.|.p.g.}.|.p.g
+000050f0: 007d 077c 0870 2269 007d 087c 046a 006a  .}.|.p"i.}.|.j.j
+00005100: 0164 0183 017d 0a88 046a 027c 0464 0264  .d...}...j.|.d.d
+00005110: 0367 0283 0270 4267 007d 0b74 0374 0464  .g...pBg.}.t.t.d
+00005120: 0464 0584 007c 0b83 0283 017d 0c88 046a  .d...|.....}...j
+00005130: 027c 0464 0267 0183 0270 6667 007d 0d74  .|.d.g...pfg.}.t
+00005140: 0374 0464 0664 0584 007c 0d83 0283 017d  .t.d.d...|.....}
+00005150: 0e74 0574 0487 0066 0164 0764 0584 0874  .t.t...f.d.d...t
+00005160: 0688 0083 0183 0283 0189 0274 077c 0c83  ...........t.|..
+00005170: 0172 c464 087c 0e6b 0772 c474 0374 0864  .r.d.|.k.r.t.t.d
+00005180: 0964 0584 0074 0487 0266 0164 0a64 0584  .d...t...f.d.d..
+00005190: 087c 0c83 0283 0283 016e 0264 007d 0f88  .|.......n.d.}..
+000051a0: 046a 097c 0a88 007c 0f83 037d 1088 046a  .j.|...|...}...j
+000051b0: 0a7c 017c 1088 017c 0583 047d 1088 046a  .|.|...|...}...j
+000051c0: 0b7c 1088 017c 0983 037d 1088 046a 0c7c  .|...|...}...j.|
+000051d0: 107c 0188 017c 0783 047d 1074 0388 046a  .|...|...}.t...j
+000051e0: 0d7c 107c 0883 0283 017d 1174 0e88 0083  .|.|.....}.t....
+000051f0: 0189 0569 0089 0688 046a 0f7c 0a7c 017c  ...i.....j.|.|.|
+00005200: 1188 0088 017c 0683 0689 0387 0187 0387  .....|..........
+00005210: 0487 0587 0666 0564 0b64 0c84 087d 1264  .....f.d.d...}.d
+00005220: 0274 0374 047c 127c 1183 0283 0169 017d  .t.t.|.|.....i.}
+00005230: 1388 046a 027c 0464 0d67 0183 0290 0170  ...j.|.d.g.....p
+00005240: 6c67 007d 1474 0374 0464 0e64 0584 007c  lg.}.t.t.d.d...|
+00005250: 1483 0283 017d 1574 077c 1583 0190 0272  .....}.t.|.....r
+00005260: 2088 046a 107c 0883 017d 167c 086a 0164   ..j.|...}.|.j.d
+00005270: 0f83 017d 177c 086a 0164 1083 017d 187c  ...}.|.j.d...}.|
+00005280: 167c 177c 1864 119c 037c 1364 0d3c 0064  .|.|.d...|.d.<.d
+00005290: 127c 156b 0690 0173 cc64 137c 156b 0690  .|.k...s.d.|.k..
+000052a0: 0272 2074 117c 0a7c 1083 027d 197c 197c  .r t.|.|...}.|.|
+000052b0: 1364 0d19 0064 123c 007c 1764 006b 0990  .d...d.<.|.d.k..
+000052c0: 0272 027c 177c 1617 007c 196b 007c 1364  .r.|.|...|.k.|.d
+000052d0: 0d19 0064 133c 006e 1e7c 1864 006b 0990  ...d.<.n.|.d.k..
+000052e0: 0272 207c 187c 1614 007c 196b 007c 1364  .r |.|...|.k.|.d
+000052f0: 0d19 0064 133c 007c 1353 0004 0074 126b  ...d.<.|.S...t.k
+00005300: 0a90 0272 4a01 007d 1a01 007a 0a7c 1a82  ...rJ..}...z.|..
+00005310: 0157 0059 0064 0064 007d 1a7e 1a58 006e  .W.Y.d.d.}.~.X.n
+00005320: 0258 0064 0053 0029 144e 726c 0000 00da  .X.d.S.).Nrl....
+00005330: 0464 6174 6172 dd00 0000 6301 0000 0000  .datar....c.....
+00005340: 0000 0001 0000 0001 0000 0053 0000 0073  ...........S...s
+00005350: 0800 0000 7c00 6a00 6a01 5300 2901 4e29  ....|.j.j.S.).N)
+00005360: 0272 4800 0000 72bc 0000 0029 0172 4b00  .rH...r....).rK.
+00005370: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
+00005380: 0072 4c00 0000 1803 0000 7300 0000 007a  .rL.......s....z
+00005390: 3b47 7261 7068 514c 5363 6865 6d61 4765  ;GraphQLSchemaGe
+000053a0: 6e65 7261 746f 722e 7265 736f 6c76 655f  nerator.resolve_
+000053b0: 6d6f 6465 6c5f 6c69 7374 2e3c 6c6f 6361  model_list.<loca
+000053c0: 6c73 3e2e 3c6c 616d 6264 613e 6301 0000  ls>.<lambda>c...
+000053d0: 0000 0000 0001 0000 0001 0000 0053 0000  .............S..
+000053e0: 0073 0800 0000 7c00 6a00 6a01 5300 2901  .s....|.j.j.S.).
+000053f0: 4e29 0272 4800 0000 72bc 0000 0029 0172  N).rH...r....).r
+00005400: 4b00 0000 7223 0000 0072 2300 0000 7224  K...r#...r#...r$
+00005410: 0000 0072 4c00 0000 1a03 0000 7300 0000  ...rL.......s...
+00005420: 0063 0100 0000 0000 0000 0100 0000 0400  .c..............
+00005430: 0000 1300 0000 7312 0000 0074 007c 0083  ......s....t.|..
+00005440: 0174 0188 007c 0083 0267 0253 0029 014e  .t...|...g.S.).N
+00005450: 2902 7249 0000 0072 6900 0000 2901 724b  ).rI...ri...).rK
+00005460: 0000 0029 0172 6d00 0000 7223 0000 0072  ...).rm...r#...r
+00005470: 2400 0000 724c 0000 001b 0300 0073 0000  $...rL.......s..
+00005480: 0000 da08 616c 6c41 7474 7273 6301 0000  ....allAttrsc...
+00005490: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+000054a0: 0073 0800 0000 7c00 6400 6b09 5300 2901  .s....|.d.k.S.).
+000054b0: 4e72 2300 0000 2901 724b 0000 0072 2300  Nr#...).rK...r#.
+000054c0: 0000 7223 0000 0072 2400 0000 724c 0000  ..r#...r$...rL..
+000054d0: 001c 0300 0073 0000 0000 6301 0000 0000  .....s....c.....
+000054e0: 0000 0001 0000 0002 0000 0013 0000 0073  ...............s
+000054f0: 0a00 0000 8800 6a00 7c00 8301 5300 2901  ......j.|...S.).
+00005500: 4e29 0172 8600 0000 2901 724b 0000 0029  N).r....).rK...)
+00005510: 01da 0b6d 6f64 656c 5f61 7474 7273 7223  ...model_attrsr#
+00005520: 0000 0072 2400 0000 724c 0000 001c 0300  ...r$...rL......
+00005530: 0073 0000 0000 6301 0000 0000 0000 0004  .s....c.........
+00005540: 0000 0007 0000 0013 0000 0073 6600 0000  ...........sf...
+00005550: 7400 8800 7401 8302 7214 7402 8800 8301  t...t...r.t.....
+00005560: 7d01 6e18 7402 7403 8700 6601 6401 6402  }.n.t.t...f.d.d.
+00005570: 8408 8801 6a04 8302 8301 7d01 8804 7c01  ....j.....}...|.
+00005580: 8805 6403 8d02 7d02 7c02 6a05 7d03 7406  ..d...}.|.j.}.t.
+00005590: 7c03 8301 7d03 7c03 7c03 7407 7403 8700  |...}.|.|.t.t...
+000055a0: 8703 6602 6404 6402 8408 8802 8302 8301  ..f.d.d.........
+000055b0: 6405 9c03 5300 2906 4e63 0100 0000 0000  d...S.).Nc......
+000055c0: 0000 0100 0000 0400 0000 1300 0000 7316  ..............s.
+000055d0: 0000 0074 007c 006a 0183 0174 0288 007c  ...t.|.j...t...|
+000055e0: 006a 0183 0266 0253 0029 014e 2903 7249  .j...f.S.).N).rI
+000055f0: 0000 0072 4800 0000 7269 0000 0029 0172  ...rH...ri...).r
+00005600: 4b00 0000 2901 da03 726f 7772 2300 0000  K...)...rowr#...
+00005610: 7224 0000 0072 4c00 0000 3003 0000 7300  r$...rL...0...s.
+00005620: 0000 007a 5b47 7261 7068 514c 5363 6865  ...z[GraphQLSche
+00005630: 6d61 4765 6e65 7261 746f 722e 7265 736f  maGenerator.reso
+00005640: 6c76 655f 6d6f 6465 6c5f 6c69 7374 2e3c  lve_model_list.<
+00005650: 6c6f 6361 6c73 3e2e 6d61 705f 7175 6572  locals>.map_quer
+00005660: 7973 6574 5f70 6167 655f 6974 656d 2e3c  yset_page_item.<
+00005670: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00005680: 2902 72b1 0000 00da 0763 6f6e 7465 7874  ).r......context
+00005690: 6301 0000 0000 0000 0001 0000 0005 0000  c...............
+000056a0: 0013 0000 0073 1400 0000 8801 6a00 7c00  .....s......j.|.
+000056b0: 8700 6601 6401 6402 8408 8302 5300 2903  ..f.d.d.....S.).
+000056c0: 4e63 0100 0000 0000 0000 0100 0000 0200  Nc..............
+000056d0: 0000 1300 0000 7308 0000 007c 0088 006b  ......s....|...k
+000056e0: 0253 0029 014e 7223 0000 0029 0172 b100  .S.).Nr#...).r..
+000056f0: 0000 2901 72f6 0000 0072 2300 0000 7224  ..).r....r#...r$
+00005700: 0000 0072 4c00 0000 3a03 0000 7300 0000  ...rL...:...s...
+00005710: 007a 6d47 7261 7068 514c 5363 6865 6d61  .zmGraphQLSchema
+00005720: 4765 6e65 7261 746f 722e 7265 736f 6c76  Generator.resolv
+00005730: 655f 6d6f 6465 6c5f 6c69 7374 2e3c 6c6f  e_model_list.<lo
+00005740: 6361 6c73 3e2e 6d61 705f 7175 6572 7973  cals>.map_querys
+00005750: 6574 5f70 6167 655f 6974 656d 2e3c 6c6f  et_page_item.<lo
+00005760: 6361 6c73 3e2e 3c6c 616d 6264 613e 2e3c  cals>.<lambda>.<
+00005770: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00005780: 2901 72c8 0000 0029 0172 4b00 0000 2902  ).r....).rK...).
+00005790: 72f6 0000 0072 5d00 0000 7223 0000 0072  r....r]...r#...r
+000057a0: 2400 0000 724c 0000 003a 0300 0073 0000  $...rL...:...s..
+000057b0: 0000 2903 72dd 0000 0072 f400 0000 720f  ..).r....r....r.
+000057c0: 0000 0029 08da 0a69 7369 6e73 7461 6e63  ...)...isinstanc
+000057d0: 6572 0500 0000 724f 0000 0072 4d00 0000  er....rO...rM...
+000057e0: 729e 0000 005a 1372 6570 7265 7365 6e74  r....Z.represent
+000057f0: 6174 696f 6e5f 6461 7461 7252 0000 0072  ation_datarR...r
+00005800: 6400 0000 2904 72f6 0000 0072 f300 0000  d...).r....r....
+00005810: 5a0a 7365 7269 616c 697a 6572 da0a 7365  Z.serializer..se
+00005820: 7269 616c 697a 6564 2905 726f 0000 00da  rialized).ro....
+00005830: 1571 7565 7279 7365 745f 7061 6765 5f6c  .queryset_page_l
+00005840: 6f6f 6b75 7073 725d 0000 00da 1073 6572  ookupsr].....ser
+00005850: 6961 6c69 7a65 725f 636c 6173 73da 1273  ializer_class..s
+00005860: 6572 6961 6c69 7a65 725f 636f 6e74 6578  erializer_contex
+00005870: 7429 0172 f600 0000 7224 0000 00da 166d  t).r....r$.....m
+00005880: 6170 5f71 7565 7279 7365 745f 7061 6765  ap_queryset_page
+00005890: 5f69 7465 6d2c 0300 0073 1600 0000 0001  _item,...s......
+000058a0: 0a01 0a02 1802 0c01 0601 0803 0201 0201  ................
+000058b0: 0401 0c01 7a49 4772 6170 6851 4c53 6368  ....zIGraphQLSch
+000058c0: 656d 6147 656e 6572 6174 6f72 2e72 6573  emaGenerator.res
+000058d0: 6f6c 7665 5f6d 6f64 656c 5f6c 6973 742e  olve_model_list.
+000058e0: 3c6c 6f63 616c 733e 2e6d 6170 5f71 7565  <locals>.map_que
+000058f0: 7279 7365 745f 7061 6765 5f69 7465 6d72  ryset_page_itemr
+00005900: cf00 0000 6301 0000 0000 0000 0001 0000  ....c...........
+00005910: 0001 0000 0053 0000 0073 0800 0000 7c00  .....S...s....|.
+00005920: 6a00 6a01 5300 2901 4e29 0272 4800 0000  j.j.S.).N).rH...
+00005930: 72bc 0000 0029 0172 4b00 0000 7223 0000  r....).rK...r#..
+00005940: 0072 2300 0000 7224 0000 0072 4c00 0000  .r#...r$...rL...
+00005950: 4403 0000 7300 0000 0072 3400 0000 7233  D...s....r4...r3
+00005960: 0000 0029 0372 3500 0000 7234 0000 0072  ...).r5...r4...r
+00005970: 3300 0000 723a 0000 0072 4300 0000 2913  3...r:...rC...).
+00005980: 72f7 0000 0072 8600 0000 72f2 0000 0072  r....r....r....r
+00005990: 6400 0000 724d 0000 0072 4f00 0000 da03  d...rM...rO.....
+000059a0: 6469 7272 6600 0000 7265 0000 0072 7200  dirrf...re...rr.
+000059b0: 0000 72a9 0000 0072 1200 0000 72cd 0000  ..r....r....r...
+000059c0: 0072 d100 0000 7214 0000 0072 b800 0000  .r....r....r....
+000059d0: 72d0 0000 0072 1b00 0000 da09 4578 6365  r....r......Exce
+000059e0: 7074 696f 6e29 1b72 5d00 0000 7290 0000  ption).r]...r...
+000059f0: 0072 6d00 0000 726f 0000 0072 ed00 0000  .rm...ro...r....
+00005a00: 72ac 0000 0072 0f00 0000 72cc 0000 0072  r....r....r....r
+00005a10: cf00 0000 72b3 0000 0072 6c00 0000 5a10  ....r....rl...Z.
+00005a20: 6669 656c 645f 7365 6c65 6374 696f 6e73  field_selections
+00005a30: da0b 6669 656c 645f 6e61 6d65 735a 0f64  ..field_namesZ.d
+00005a40: 6174 615f 7365 6c65 6374 696f 6e73 5a0a  ata_selectionsZ.
+00005a50: 6461 7461 5f6e 616d 6573 726e 0000 0072  data_namesrn...r
+00005a60: 7100 0000 5a0d 7175 6572 7973 6574 5f70  q...Z.queryset_p
+00005a70: 6167 6572 fd00 0000 7292 0000 005a 1570  ager....r....Z.p
+00005a80: 6167 696e 6174 696f 6e5f 7365 6c65 6374  agination_select
+00005a90: 696f 6e73 5a10 7061 6769 6e61 7469 6f6e  ionsZ.pagination
+00005aa0: 5f6e 616d 6573 7235 0000 0072 3400 0000  _namesr5...r4...
+00005ab0: 7233 0000 0072 3a00 0000 da01 6572 2300  r3...r:.....er#.
+00005ac0: 0000 2907 726d 0000 0072 6f00 0000 72f5  ..).rm...ro...r.
+00005ad0: 0000 0072 fa00 0000 725d 0000 0072 fb00  ...r....r]...r..
+00005ae0: 0000 72fc 0000 0072 2400 0000 da12 7265  ..r....r$.....re
+00005af0: 736f 6c76 655f 6d6f 6465 6c5f 6c69 7374  solve_model_list
+00005b00: 0e03 0000 7352 0000 0000 0104 0108 0108  ....sR..........
+00005b10: 0108 0108 020c 0214 0112 0112 0112 011a  ................
+00005b20: 0234 020e 0210 010e 0110 0210 0208 0104  .4..............
+00005b30: 0214 0214 1412 0314 0112 020a 010a 010a  ................
+00005b40: 010a 0302 0102 010c 0314 010a 010c 020a  ................
+00005b50: 0116 010a 0114 0204 0112 017a 2947 7261  ...........z)Gra
+00005b60: 7068 514c 5363 6865 6d61 4765 6e65 7261  phQLSchemaGenera
+00005b70: 746f 722e 7265 736f 6c76 655f 6d6f 6465  tor.resolve_mode
+00005b80: 6c5f 6c69 7374 6305 0000 0000 0000 0013  l_listc.........
+00005b90: 0000 0009 0000 0003 0000 0073 9201 0000  ...........s....
+00005ba0: 7400 7c01 8301 8900 7401 8800 6a02 8301  t.|.....t...j...
+00005bb0: 6401 6b02 721e 7403 6402 8301 8201 6900  d.k.r.t.d.....i.
+00005bc0: 7d05 8802 6a04 7c01 8800 7c02 8303 8802  }...j.|...|.....
+00005bd0: 5f05 8802 6a06 8802 6a05 8301 8802 5f07  _...j...j....._.
+00005be0: 6401 7d06 7401 8800 6a02 8301 7d07 9001  d.}.t...j...}...
+00005bf0: 781e 8800 6a02 4400 9001 5d12 7d08 7408  x...j.D...].}.t.
+00005c00: 7c08 8301 7d09 7c09 6a09 6401 1900 7d0a  |...}.|.j.d...}.
+00005c10: 740a 8800 6a0b 7c0a 8302 7d0b 740c 7c0b  t...j.|...}.t.|.
+00005c20: 8301 7d0b 7c04 7294 7c04 7c0b 7c06 7c07  ..}.|.r.|.|.|.|.
+00005c30: 8303 0100 8802 6a0d 8800 7c09 8302 7d0c  ......j...|...}.
+00005c40: 8802 6a0e 8800 7c09 8302 7d0d 8802 6a0f  ..j...|...}...j.
+00005c50: 8800 7c09 8302 7d0e 8802 6a10 8800 7c09  ..|...}...j...|.
+00005c60: 8302 7d0f 7411 6403 6a12 7c0b 8301 7413  ..}.t.d.j.|...t.
+00005c70: 6a14 6601 7413 6a15 7c0f 8301 7413 6a15  j.f.t.j.|...t.j.
+00005c80: 7416 8301 7413 6a17 7416 8301 6404 9c03  t...t.j.t...d...
+00005c90: 8303 7d10 7411 6405 6a12 7c0b 8301 7413  ..}.t.d.j.|...t.
+00005ca0: 6a14 6601 7413 6a17 7c10 8301 7413 6a15  j.f.t.j.|...t.j.
+00005cb0: 7418 8301 6406 9c02 8303 7d11 8700 8701  t...d.....}.....
+00005cc0: 8702 6603 6407 6408 8408 7d12 7413 6a15  ..f.d.d...}.t.j.
+00005cd0: 7c11 7c0c 7413 6a17 7c0d 8301 7c0e 7419  |.|.t.j.|...|.t.
+00005ce0: 8300 741a 8300 6409 8d06 7c05 7c0b 3c00  ..t...d...|.|.<.
+00005cf0: 7c12 7c08 7c09 8302 7c05 640a 6a12 7c0b  |.|.|...|.d.j.|.
+00005d00: 8301 3c00 7c06 640b 3700 7d06 7158 5700  ..<.|.d.7.}.qXW.
+00005d10: 7c04 9001 7282 7c04 6400 7c07 7c07 8303  |...r.|.d.|.|...
+00005d20: 0100 7411 640c 7413 6a14 6601 7c05 8303  ..t.d.t.j.f.|...
+00005d30: 5300 290d 4e72 0100 0000 7a0f 4e6f 2074  S.).Nr....z.No t
+00005d40: 6162 6c65 7320 666f 756e 647a 104d 6f64  ables foundz.Mod
+00005d50: 656c 7b7d 4d6f 6465 6c54 7970 6529 0372  el{}ModelType).r
+00005d60: dd00 0000 72f4 0000 0072 0f00 0000 7a14  ....r....r....z.
+00005d70: 4d6f 6465 6c7b 7d4d 6f64 656c 4c69 7374  Model{}ModelList
+00005d80: 5479 7065 2902 72f3 0000 0072 cf00 0000  Type).r....r....
+00005d90: 6302 0000 0000 0000 0003 0000 0006 0000  c...............
+00005da0: 0013 0000 0073 1a00 0000 6403 8702 8700  .....s....d.....
+00005db0: 8703 8701 8704 6605 6401 6402 8409 7d02  ......f.d.d...}.
+00005dc0: 7c02 5300 2904 4e63 0700 0000 0000 0000  |.S.).Nc........
+00005dd0: 0800 0000 0b00 0000 1300 0000 733c 0000  ............s<..
+00005de0: 007c 016a 006a 0164 0183 017d 0788 0264  .|.j.j.d...}...d
+00005df0: 006b 0972 2088 027c 0788 0364 028d 0201  .k.r ..|...d....
+00005e00: 0088 046a 0288 0088 0188 037c 017c 027c  ...j.......|.|.|
+00005e10: 037c 047c 057c 0664 038d 0953 0029 044e  .|.|.|.d...S.).N
+00005e20: 726c 0000 0029 0272 6c00 0000 726f 0000  rl...).rl...ro..
+00005e30: 0029 0572 ac00 0000 720f 0000 0072 cc00  .).r....r....r..
+00005e40: 0000 72cf 0000 0072 b300 0000 2903 72f7  ..r....r....).r.
+00005e50: 0000 0072 8600 0000 7202 0100 0029 08da  ...r....r....)..
+00005e60: 0670 6172 656e 7472 ed00 0000 72ac 0000  .parentr....r...
+00005e70: 0072 0f00 0000 72cc 0000 0072 cf00 0000  .r....r....r....
+00005e80: 72b3 0000 0072 6c00 0000 2905 7290 0000  r....rl...).r...
+00005e90: 0072 6d00 0000 da0e 6265 666f 7265 5f72  .rm.....before_r
+00005ea0: 6573 6f6c 7665 726f 0000 0072 5d00 0000  esolvero...r]...
+00005eb0: 7223 0000 0072 2400 0000 da08 7265 736f  r#...r$.....reso
+00005ec0: 6c76 6572 8403 0000 731a 0000 0000 010c  lver....s.......
+00005ed0: 0208 010c 0204 0102 0102 0102 0102 0102  ................
+00005ee0: 0102 0102 0102 017a 5547 7261 7068 514c  .......zUGraphQL
+00005ef0: 5363 6865 6d61 4765 6e65 7261 746f 722e  SchemaGenerator.
+00005f00: 6765 745f 7175 6572 795f 7479 7065 2e3c  get_query_type.<
+00005f10: 6c6f 6361 6c73 3e2e 6372 6561 7465 5f6c  locals>.create_l
+00005f20: 6973 745f 7265 736f 6c76 6572 2e3c 6c6f  ist_resolver.<lo
+00005f30: 6361 6c73 3e2e 7265 736f 6c76 6572 2905  cals>.resolver).
+00005f40: 4e4e 4e4e 4e72 2300 0000 2903 726d 0000  NNNNNr#...).rm..
+00005f50: 0072 6f00 0000 7205 0100 0029 0372 9000  .ro...r....).r..
+00005f60: 0000 7204 0100 0072 5d00 0000 2902 726d  ..r....r]...).rm
+00005f70: 0000 0072 6f00 0000 7224 0000 00da 1463  ...ro...r$.....c
+00005f80: 7265 6174 655f 6c69 7374 5f72 6573 6f6c  reate_list_resol
+00005f90: 7665 7283 0300 0073 0400 0000 0001 1611  ver....s........
+00005fa0: 7a43 4772 6170 6851 4c53 6368 656d 6147  zCGraphQLSchemaG
+00005fb0: 656e 6572 6174 6f72 2e67 6574 5f71 7565  enerator.get_que
+00005fc0: 7279 5f74 7970 652e 3c6c 6f63 616c 733e  ry_type.<locals>
+00005fd0: 2e63 7265 6174 655f 6c69 7374 5f72 6573  .create_list_res
+00005fe0: 6f6c 7665 7229 0572 ac00 0000 720f 0000  olver).r....r...
+00005ff0: 0072 cc00 0000 72cf 0000 0072 b300 0000  .r....r....r....
+00006000: 7a0a 7265 736f 6c76 655f 7b7d 724a 0000  z.resolve_{}rJ..
+00006010: 00da 0551 7565 7279 291b 720a 0000 0072  ...Query).r....r
+00006020: 6600 0000 7284 0000 0072 ff00 0000 7299  f...r....r....r.
+00006030: 0000 0072 5400 0000 729d 0000 0072 5500  ...rT...r....rU.
+00006040: 0000 7202 0000 0072 6800 0000 720e 0000  ..r....rh...r...
+00006050: 0072 7800 0000 7249 0000 0072 d700 0000  .rx...rI...r....
+00006060: 72e7 0000 0072 e800 0000 72e9 0000 0072  r....r....r....r
+00006070: ab00 0000 72d3 0000 0072 2e00 0000 da0a  ....r....r......
+00006080: 4f62 6a65 6374 5479 7065 da05 4669 656c  ObjectType..Fiel
+00006090: 6472 1a00 0000 72d4 0000 0072 4200 0000  dr....r....rB...
+000060a0: 7231 0000 0072 3600 0000 2913 725d 0000  r1...r6...).r]..
+000060b0: 0072 6c00 0000 7291 0000 0072 0401 0000  .rl...r....r....
+000060c0: da13 6f6e 5f70 726f 6772 6573 735f 7570  ..on_progress_up
+000060d0: 6461 7465 645a 0b71 7565 7279 5f61 7474  datedZ.query_att
+000060e0: 7273 72ef 0000 00da 0574 6f74 616c 726d  rsr......totalrm
+000060f0: 0000 0072 6f00 0000 7295 0000 0072 4800  ...ro...r....rH.
+00006100: 0000 5a0b 4669 6c74 6572 7354 7970 655a  ..Z.FiltersTypeZ
+00006110: 0b4c 6f6f 6b75 7073 5479 7065 5a08 536f  .LookupsTypeZ.So
+00006120: 7274 5479 7065 722b 0000 005a 094d 6f64  rtTyper+...Z.Mod
+00006130: 656c 5479 7065 5a0d 4d6f 6465 6c4c 6973  elTypeZ.ModelLis
+00006140: 7454 7970 6572 0601 0000 7223 0000 0029  tTyper....r#...)
+00006150: 0372 9000 0000 7204 0100 0072 5d00 0000  .r....r....r]...
+00006160: 7224 0000 00da 0e67 6574 5f71 7565 7279  r$.....get_query
+00006170: 5f74 7970 655e 0300 0073 4e00 0000 0001  _type^...sN.....
+00006180: 0802 0e01 0802 0402 1001 0e02 0401 0a02  ................
+00006190: 1001 0801 0a01 0c01 0802 0401 0c02 0c01  ................
+000061a0: 0c01 0c01 0c01 1001 0801 0801 1002 1001  ................
+000061b0: 0801 1003 1014 0401 0201 0201 0801 0201  ................
+000061c0: 0401 0e02 1402 0c02 0601 0c02 7a25 4772  ............z%Gr
+000061d0: 6170 6851 4c53 6368 656d 6147 656e 6572  aphQLSchemaGener
+000061e0: 6174 6f72 2e67 6574 5f71 7565 7279 5f74  ator.get_query_t
+000061f0: 7970 6563 0500 0000 0000 0000 0600 0000  ypec............
+00006200: 0500 0000 4300 0000 731e 0000 007c 006a  ....C...s....|.j
+00006210: 007c 017c 027c 037c 0483 047d 0574 016a  .|.|.|.|...}.t.j
+00006220: 027c 0564 0164 028d 0253 0029 034e 4629  .|.d.d...S.).NF)
+00006230: 0272 3800 0000 5a0e 6175 746f 5f63 616d  .r8...Z.auto_cam
+00006240: 656c 6361 7365 2903 720c 0100 0072 2e00  elcase).r....r..
+00006250: 0000 5a06 5363 6865 6d61 2906 725d 0000  ..Z.Schema).r]..
+00006260: 0072 6c00 0000 7291 0000 0072 0401 0000  .rl...r....r....
+00006270: 720a 0100 0072 0701 0000 7223 0000 0072  r....r....r#...r
+00006280: 2300 0000 7224 0000 00da 0a67 6574 5f73  #...r$.....get_s
+00006290: 6368 656d 61a8 0300 0073 0400 0000 0001  chema....s......
+000062a0: 1001 7a21 4772 6170 6851 4c53 6368 656d  ..z!GraphQLSchem
+000062b0: 6147 656e 6572 6174 6f72 2e67 6574 5f73  aGenerator.get_s
+000062c0: 6368 656d 6129 014e 2902 4e46 2901 4e29  chema).N).NF).N)
+000062d0: 0172 4a00 0000 2901 724a 0000 0029 0172  .rJ...).rJ...).r
+000062e0: 4a00 0000 2901 724a 0000 0029 0172 4a00  J...).rJ...).rJ.
+000062f0: 0000 2901 724a 0000 0029 054e 4e4e 4e4e  ..).rJ...).NNNNN
+00006300: 2902 4e4e 2902 4e4e 2920 7220 0000 0072  ).NN).NN) r ...r
+00006310: 2100 0000 7222 0000 0072 5e00 0000 7272  !...r"...r^...rr
+00006320: 0000 0072 9900 0000 729d 0000 0072 a000  ...r....r....r..
+00006330: 0000 72a1 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+00006340: 0072 a900 0000 7212 0000 0072 b800 0000  .r....r....r....
+00006350: 72b4 0000 0072 c800 0000 72ca 0000 0072  r....r....r....r
+00006360: cd00 0000 72d0 0000 0072 d100 0000 72d7  ....r....r....r.
+00006370: 0000 0072 d500 0000 72d6 0000 0072 e700  ...r....r....r..
+00006380: 0000 72e5 0000 0072 e600 0000 72e8 0000  ..r....r....r...
+00006390: 0072 e900 0000 72f2 0000 0072 0201 0000  .r....r....r....
+000063a0: 720c 0100 0072 0d01 0000 7223 0000 0072  r....r....r#...r
+000063b0: 2300 0000 7223 0000 0072 2400 0000 7253  #...r#...r$...rS
+000063c0: 0000 0066 0000 0073 3a00 0000 0801 080b  ...f...s:.......
+000063d0: 0a19 086b 0809 0806 0804 0804 0804 0a56  ...k...........V
+000063e0: 0807 0810 086f 0a24 080e 0811 0803 080c  .....o.$........
+000063f0: 0a20 0a20 0a13 0a1e 0a1d 0a15 0812 080b  . . ............
+00006400: 080f 0a50 0a4a 7253 0000 0029 4472 4600  ...P.JrS...)DrF.
+00006410: 0000 722e 0000 00da 0a73 716c 616c 6368  ..r......sqlalch
+00006420: 656d 7972 0200 0000 7203 0000 0072 0400  emyr....r....r..
+00006430: 0000 5a11 7371 6c61 6c63 6865 6d79 2e65  ..Z.sqlalchemy.e
+00006440: 6e67 696e 6572 0500 0000 da0e 7371 6c61  nginer......sqla
+00006450: 6c63 6865 6d79 2e6f 726d 7206 0000 0072  lchemy.ormr....r
+00006460: 0700 0000 7208 0000 00da 176a 6574 5f62  ....r......jet_b
+00006470: 7269 6467 655f 6261 7365 2e61 7574 6f6d  ridge_base.autom
+00006480: 6170 7209 0000 00da 126a 6574 5f62 7269  apr......jet_bri
+00006490: 6467 655f 6261 7365 2e64 6272 0a00 0000  dge_base.dbr....
+000064a0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+000064b0: 0e00 0000 5a17 6a65 745f 6272 6964 6765  ....Z.jet_bridge
+000064c0: 5f62 6173 652e 6669 6c74 6572 7372 0f00  _base.filtersr..
+000064d0: 0000 5a2a 6a65 745f 6272 6964 6765 5f62  ..Z*jet_bridge_b
+000064e0: 6173 652e 6669 6c74 6572 732e 6669 6c74  ase.filters.filt
+000064f0: 6572 5f66 6f72 5f64 6266 6965 6c64 7210  er_for_dbfieldr.
+00006500: 0000 005a 236a 6574 5f62 7269 6467 655f  ...Z#jet_bridge_
+00006510: 6261 7365 2e66 696c 7465 7273 2e6d 6f64  base.filters.mod
+00006520: 656c 5f67 726f 7570 7211 0000 005a 246a  el_groupr....Z$j
+00006530: 6574 5f62 7269 6467 655f 6261 7365 2e66  et_bridge_base.f
+00006540: 696c 7465 7273 2e6d 6f64 656c 5f73 6561  ilters.model_sea
+00006550: 7263 6872 1200 0000 5a2e 6a65 745f 6272  rchr....Z.jet_br
+00006560: 6964 6765 5f62 6173 652e 6d6f 6465 6c73  idge_base.models
+00006570: 2e6d 6f64 656c 5f72 656c 6174 696f 6e5f  .model_relation_
+00006580: 6f76 6572 7269 6465 7213 0000 005a 216a  overrider....Z!j
+00006590: 6574 5f62 7269 6467 655f 6261 7365 2e73  et_bridge_base.s
+000065a0: 6572 6961 6c69 7a65 7273 2e6d 6f64 656c  erializers.model
+000065b0: 7214 0000 00da 156a 6574 5f62 7269 6467  r......jet_bridg
+000065c0: 655f 6261 7365 2e73 746f 7265 7215 0000  e_base.storer...
+000065d0: 00da 1c6a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
+000065e0: 7365 2e75 7469 6c73 2e63 6f6d 6d6f 6e72  se.utils.commonr
+000065f0: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+00006600: 0000 005a 196a 6574 5f62 7269 6467 655f  ...Z.jet_bridge_
+00006610: 6261 7365 2e75 7469 6c73 2e67 716c 721a  base.utils.gqlr.
+00006620: 0000 00da 1e6a 6574 5f62 7269 6467 655f  .....jet_bridge_
+00006630: 6261 7365 2e75 7469 6c73 2e71 7565 7279  base.utils.query
+00006640: 7365 7472 1b00 0000 721c 0000 0072 1d00  setr....r....r..
+00006650: 0000 5a1f 6a65 745f 6272 6964 6765 5f62  ..Z.jet_bridge_b
+00006660: 6173 652e 7574 696c 732e 7265 6c61 7469  ase.utils.relati
+00006670: 6f6e 7372 1e00 0000 5a0f 496e 7075 744f  onsr....Z.InputO
+00006680: 626a 6563 7454 7970 6572 1f00 0000 7225  bjectTyper....r%
+00006690: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
+000066a0: 0000 7229 0000 0072 2a00 0000 7208 0100  ..r)...r*...r...
+000066b0: 0072 2b00 0000 722c 0000 0072 3100 0000  .r+...r,...r1...
+000066c0: 7236 0000 00da 0445 6e75 6d72 3900 0000  r6.....Enumr9...
+000066d0: 723f 0000 0072 4200 0000 7249 0000 0072  r?...rB...rI...r
+000066e0: 5200 0000 da06 6f62 6a65 6374 7253 0000  R.....objectrS..
+000066f0: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
+00006700: 7224 0000 00da 083c 6d6f 6475 6c65 3e01  r$.....<module>.
+00006710: 0000 0073 4400 0000 0801 0801 1401 0c01  ...sD...........
+00006720: 1402 0c01 1c01 0c01 0c01 0c01 0c01 0c01  ................
+00006730: 0c01 0c01 1801 0c01 1401 0c03 1204 1204  ................
+00006740: 1204 1204 1204 1204 1204 1204 1204 1206  ................
+00006750: 1204 1208 1205 1208 0808 0805            ............
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/crypt.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/crypt.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/queryset.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/queryset.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/gql.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/gql.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/utc.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/utc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/type_codes.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/type_codes.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 76b0 eb63 b805 0000 e300 0000  3...v..c........
+00000000: 330d 0d0a 7c5a 4164 b805 0000 e300 0000  3...|ZAd........
 00000010: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
 00000020: 0073 2800 0000 6400 6401 6c00 5a00 6400  .s(...d.d.l.Z.d.
 00000030: 6402 6c01 6d02 5a02 0100 6403 6404 8400  d.l.m.Z...d.d...
 00000040: 5a03 6405 6406 8400 5a04 6401 5300 2907  Z.d.d...Z.d.S.).
 00000050: e900 0000 004e 2901 da12 6765 745f 7365  .....N)...get_se
 00000060: 7373 696f 6e5f 656e 6769 6e65 6301 0000  ssion_enginec...
 00000070: 0000 0000 000b 0000 0005 0000 0043 0000  .............C..
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_model.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_model.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/common.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/common.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-00000000: 330d 0d0a 76b0 eb63 e60a 0000 e300 0000  3...v..c........
-00000010: 0000 0000 0000 0000 000b 0000 0040 0000  .............@..
-00000020: 0073 9a00 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 7910  d.l.Z.d.d.l.Z.y.
-00000040: 6501 6a03 8300 5a01 6402 5a04 5700 6e2a  e.j...Z.d.Z.W.n*
-00000050: 0400 6505 6b0a 7252 0100 0100 0100 6400  ..e.k.rR......d.
-00000060: 6401 6c06 5a06 6506 6a07 6403 8301 0100  d.l.Z.e.j.d.....
-00000070: 6404 5a04 5900 6e02 5800 6417 6407 6408  d.Z.Y.n.X.d.d.d.
-00000080: 8401 5a08 6409 640a 8400 5a09 640b 640c  ..Z.d.d...Z.d.d.
-00000090: 8400 5a0a 640d 640e 8400 5a0b 640f 6410  ..Z.d.d...Z.d.d.
-000000a0: 8400 5a0c 6411 6412 8400 5a0d 6413 6414  ..Z.d.d...Z.d.d.
-000000b0: 8400 5a0e 6415 6416 8400 5a0f 6401 5300  ..Z.d.d...Z.d.S.
-000000c0: 2918 e900 0000 004e 547a 6a41 2073 6563  )......NTzjA sec
-000000d0: 7572 6520 7073 6575 646f 2d72 616e 646f  ure pseudo-rando
-000000e0: 6d20 6e75 6d62 6572 2067 656e 6572 6174  m number generat
-000000f0: 6f72 2069 7320 6e6f 7420 6176 6169 6c61  or is not availa
-00000100: 626c 6520 6f6e 2079 6f75 7220 7379 7374  ble on your syst
-00000110: 656d 2e20 4661 6c6c 696e 6720 6261 636b  em. Falling back
-00000120: 2074 6f20 4d65 7273 656e 6e65 2054 7769   to Mersenne Twi
-00000130: 7374 6572 2e46 da3e 6162 6364 6566 6768  ster.F.>abcdefgh
-00000140: 696a 6b6c 6d6e 6f70 7172 7374 7576 7778  ijklmnopqrstuvwx
-00000150: 797a 4142 4344 4546 4748 494a 4b4c 4d4e  yzABCDEFGHIJKLMN
-00000160: 4f50 5152 5354 5556 5758 595a 3031 3233  OPQRSTUVWXYZ0123
-00000170: 3435 3637 3839 da00 6303 0000 0000 0000  456789..c.......
-00000180: 0003 0000 0006 0000 0003 0000 0073 4c00  .............sL.
-00000190: 0000 7400 7330 7401 6a02 7403 6a04 6401  ..t.s0t.j.t.j.d.
-000001a0: 7401 6a05 8300 7406 6a06 8300 7c02 6603  t.j...t.j...|.f.
-000001b0: 1600 6a07 6402 8301 8301 6a08 8300 8301  ..j.d.....j.....
-000001c0: 0100 6403 6a09 8700 6601 6404 6405 8408  ..d.j...f.d.d...
-000001d0: 740a 7c00 8301 4400 8301 8301 5300 2906  t.|...D.....S.).
-000001e0: 7ab4 0a20 2020 2052 6574 7572 6e73 2061  z..    Returns a
-000001f0: 2073 6563 7572 656c 7920 6765 6e65 7261   securely genera
-00000200: 7465 6420 7261 6e64 6f6d 2073 7472 696e  ted random strin
-00000210: 672e 0a0a 2020 2020 5468 6520 6465 6661  g...    The defa
-00000220: 756c 7420 6c65 6e67 7468 206f 6620 3132  ult length of 12
-00000230: 2077 6974 6820 7468 6520 612d 7a2c 2041   with the a-z, A
-00000240: 2d5a 2c20 302d 3920 6368 6172 6163 7465  -Z, 0-9 characte
-00000250: 7220 7365 7420 7265 7475 726e 730a 2020  r set returns.  
-00000260: 2020 6120 3731 2d62 6974 2076 616c 7565    a 71-bit value
-00000270: 2e20 6c6f 675f 3228 2832 362b 3236 2b31  . log_2((26+26+1
-00000280: 3029 5e31 3229 203d 7e20 3731 2062 6974  0)^12) =~ 71 bit
-00000290: 730a 2020 2020 7a06 2573 2573 2573 7a05  s.    z.%s%s%sz.
-000002a0: 7574 662d 3872 0300 0000 6301 0000 0000  utf-8r....c.....
-000002b0: 0000 0002 0000 0003 0000 0033 0000 0073  ...........3...s
-000002c0: 1800 0000 7c00 5d10 7d01 7400 6a01 8800  ....|.].}.t.j...
-000002d0: 8301 5600 0100 7102 6400 5300 2901 4e29  ..V...q.d.S.).N)
-000002e0: 02da 0672 616e 646f 6dda 0663 686f 6963  ...random..choic
-000002f0: 6529 02da 022e 30da 0169 2901 da0d 616c  e)....0..i)...al
-00000300: 6c6f 7765 645f 6368 6172 73a9 00fa 632f  lowed_chars...c/
-00000310: 5573 6572 732f 6631 6e61 6c2f 4472 6f70  Users/f1nal/Drop
-00000320: 626f 782f 7079 7468 6f6e 2f6a 6574 2d62  box/python/jet-b
-00000330: 7269 6467 652f 7372 632f 7061 636b 6167  ridge/src/packag
-00000340: 6573 2f6a 6574 5f62 7269 6467 655f 6261  es/jet_bridge_ba
-00000350: 7365 2f6a 6574 5f62 7269 6467 655f 6261  se/jet_bridge_ba
-00000360: 7365 2f75 7469 6c73 2f63 6f6d 6d6f 6e2e  se/utils/common.
-00000370: 7079 fa09 3c67 656e 6578 7072 3e24 0000  py..<genexpr>$..
-00000380: 0073 0200 0000 0400 7a24 6765 745f 7261  .s......z$get_ra
-00000390: 6e64 6f6d 5f73 7472 696e 672e 3c6c 6f63  ndom_string.<loc
-000003a0: 616c 733e 2e3c 6765 6e65 7870 723e 290b  als>.<genexpr>).
-000003b0: da0f 7573 696e 675f 7379 7372 616e 646f  ..using_sysrando
-000003c0: 6d72 0400 0000 da04 7365 6564 da07 6861  mr......seed..ha
-000003d0: 7368 6c69 62da 0673 6861 3235 36da 0867  shlib..sha256..g
-000003e0: 6574 7374 6174 65da 0474 696d 65da 0665  etstate..time..e
-000003f0: 6e63 6f64 65da 0664 6967 6573 74da 046a  ncode..digest..j
-00000400: 6f69 6eda 0572 616e 6765 2903 da06 6c65  oin..range)...le
-00000410: 6e67 7468 7208 0000 005a 0473 616c 7472  ngthr....Z.saltr
-00000420: 0900 0000 2901 7208 0000 0072 0a00 0000  ....).r....r....
-00000430: da11 6765 745f 7261 6e64 6f6d 5f73 7472  ..get_random_str
-00000440: 696e 670f 0000 0073 1000 0000 0007 0407  ing....s........
-00000450: 0401 0401 0201 0601 0601 1602 7217 0000  ............r...
-00000460: 0063 0200 0000 0000 0000 0400 0000 0400  .c..............
-00000470: 0000 4300 0000 7328 0000 0078 2274 007c  ..C...s(...x"t.|
-00000480: 0083 0144 005d 165c 027d 027d 037c 017c  ...D.].\.}.}.|.|
-00000490: 037c 0283 0272 0a7c 0253 0071 0a57 0064  .|...r.|.S.q.W.d
-000004a0: 0053 0029 014e 2901 da09 656e 756d 6572  .S.).N)...enumer
-000004b0: 6174 6529 04da 046c 6973 74da 0970 7265  ate)...list..pre
-000004c0: 6469 6361 7465 7207 0000 00da 0576 616c  dicater......val
-000004d0: 7565 7209 0000 0072 0900 0000 720a 0000  uer....r....r...
-000004e0: 00da 0a66 696e 645f 696e 6465 7827 0000  ...find_index'..
-000004f0: 0073 0800 0000 0001 1201 0a01 0801 721c  .s............r.
-00000500: 0000 0063 0200 0000 0000 0000 0600 0000  ...c............
-00000510: 0700 0000 0300 0000 73ae 0000 0078 a87c  ........s....x.|
-00000520: 016a 0083 0044 005d 9c5c 027d 027d 037c  .j...D.].\.}.}.|
-00000530: 0264 016b 0272 247c 037c 007c 023c 0071  .d.k.r$|.|.|.<.q
-00000540: 0a74 017c 0374 0283 0272 467c 006a 037c  .t.|.t...rF|.j.|
-00000550: 0269 0083 027d 0474 047c 047c 0383 0201  .i...}.t.|.|....
-00000560: 0071 0a74 017c 0374 0583 0272 9e7c 006a  .q.t.|.t...r.|.j
-00000570: 037c 0267 0083 027d 0478 487c 0344 005d  .|.g...}.xH|.D.]
-00000580: 3689 0074 067c 0487 0066 0164 0264 0384  6..t.|...f.d.d..
-00000590: 0883 027d 057c 0564 006b 0872 8271 627c  ...}.|.d.k.r.qb|
-000005a0: 047c 0519 0001 0074 047c 047c 0519 0088  .|.....t.|.|....
-000005b0: 0083 0201 0071 6257 0071 0a7c 037c 007c  .....qbW.q.|.|.|
-000005c0: 023c 0071 0a57 007c 0053 0029 044e da06  .<.q.W.|.S.).N..
-000005d0: 7061 7261 6d73 6302 0000 0000 0000 0002  paramsc.........
-000005e0: 0000 0003 0000 0013 0000 0073 1000 0000  ...........s....
-000005f0: 7c00 6401 1900 8800 6401 1900 6b02 5300  |.d.....d...k.S.
-00000600: 2902 4e5a 0964 625f 636f 6c75 6d6e 7209  ).NZ.db_columnr.
-00000610: 0000 0029 02da 0178 7207 0000 0029 01da  ...)...xr....)..
-00000620: 0469 7465 6d72 0900 0000 720a 0000 00da  .itemr....r.....
-00000630: 083c 6c61 6d62 6461 3e3b 0000 0073 0000  .<lambda>;...s..
-00000640: 0000 7a17 6d65 7267 652e 3c6c 6f63 616c  ..z.merge.<local
-00000650: 733e 2e3c 6c61 6d62 6461 3e29 07da 0569  s>.<lambda>)...i
-00000660: 7465 6d73 da0a 6973 696e 7374 616e 6365  tems..isinstance
-00000670: da04 6469 6374 da0a 7365 7464 6566 6175  ..dict..setdefau
-00000680: 6c74 da05 6d65 7267 6572 1900 0000 721c  lt..merger....r.
-00000690: 0000 0029 06da 0b64 6573 7469 6e61 7469  ...)...destinati
-000006a0: 6f6e da06 736f 7572 6365 da03 6b65 7972  on..source..keyr
-000006b0: 1b00 0000 da04 6e6f 6465 da05 696e 6465  ......node..inde
-000006c0: 7872 0900 0000 2901 721f 0000 0072 0a00  xr....).r....r..
-000006d0: 0000 7225 0000 0030 0000 0073 2000 0000  ..r%...0...s ...
-000006e0: 0001 1201 0801 0a01 0a01 0c01 0c01 0a01  ................
-000006f0: 0c02 0a01 1201 0801 0201 0801 1402 0c02  ................
-00000700: 7225 0000 0063 0200 0000 0000 0000 0300  r%...c..........
-00000710: 0000 0200 0000 4300 0000 7316 0000 007c  ......C...s....|
-00000720: 006a 0083 007d 027c 026a 017c 0183 0101  .j...}.|.j.|....
-00000730: 007c 0253 0029 014e 2902 da04 636f 7079  .|.S.).N)...copy
-00000740: da06 7570 6461 7465 2903 721e 0000 00da  ..update).r.....
-00000750: 0179 da01 7a72 0900 0000 7209 0000 0072  .y..zr....r....r
-00000760: 0a00 0000 da0f 6d65 7267 655f 7477 6f5f  ......merge_two_
-00000770: 6469 6374 7346 0000 0073 0600 0000 0001  dictsF...s......
-00000780: 0801 0a01 722f 0000 0063 0100 0000 0000  ....r/...c......
-00000790: 0000 0100 0000 0300 0000 4300 0000 730c  ..........C...s.
-000007a0: 0000 0074 0074 017c 0083 0183 0153 0029  ...t.t.|.....S.)
-000007b0: 014e 2902 da04 6e65 7874 da04 6974 6572  .N)...next..iter
-000007c0: 2901 721b 0000 0072 0900 0000 7209 0000  ).r....r....r...
-000007d0: 0072 0a00 0000 da0d 6765 745f 7365 745f  .r......get_set_
-000007e0: 6669 7273 744c 0000 0073 0200 0000 0001  firstL...s......
-000007f0: 7232 0000 0063 0100 0000 0000 0000 0100  r2...c..........
-00000800: 0000 0200 0000 4300 0000 7314 0000 007c  ......C...s....|
-00000810: 0064 006b 0872 0c64 0153 0074 007c 0083  .d.k.r.d.S.t.|..
-00000820: 0153 0029 024e 7203 0000 0029 01da 0373  .S.).Nr....)...s
-00000830: 7472 2901 721b 0000 0072 0900 0000 7209  tr).r....r....r.
-00000840: 0000 0072 0a00 0000 da0f 616e 795f 7479  ...r......any_ty
-00000850: 7065 5f73 6f72 7465 7250 0000 0073 0600  pe_sorterP...s..
-00000860: 0000 0001 0801 0401 7234 0000 0063 0100  ........r4...c..
-00000870: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00000880: 0000 7328 0000 0067 007d 0178 1e7c 0044  ..s(...g.}.x.|.D
-00000890: 005d 167d 027c 027c 016b 0772 0a7c 016a  .].}.|.|.k.r.|.j
-000008a0: 007c 0283 0101 0071 0a57 007c 0153 0029  .|.....q.W.|.S.)
-000008b0: 014e 2901 da06 6170 7065 6e64 2903 da03  .N)...append)...
-000008c0: 6172 72da 0672 6573 756c 7472 1f00 0000  arr..resultr....
-000008d0: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-000008e0: 0675 6e69 7175 6556 0000 0073 0a00 0000  .uniqueV...s....
-000008f0: 0001 0401 0a01 0801 0e01 7238 0000 0063  ..........r8...c
-00000900: 0100 0000 0000 0000 0300 0000 0400 0000  ................
-00000910: 4300 0000 7336 0000 0067 007d 0178 2c7c  C...s6...g.}.x,|
-00000920: 0044 005d 247d 0274 007c 0274 0183 0272  .D.]$}.t.|.t...r
-00000930: 247c 016a 027c 0283 0101 0071 0a7c 016a  $|.j.|.....q.|.j
-00000940: 037c 0283 0101 0071 0a57 007c 0153 0029  .|.....q.W.|.S.)
-00000950: 014e 2904 7222 0000 0072 1900 0000 da06  .N).r"...r......
-00000960: 6578 7465 6e64 7235 0000 0029 0372 3600  extendr5...).r6.
-00000970: 0000 7237 0000 0072 1f00 0000 7209 0000  ..r7...r....r...
-00000980: 0072 0900 0000 720a 0000 00da 0766 6c61  .r....r......fla
-00000990: 7474 656e 5e00 0000 730c 0000 0000 0104  tten^...s.......
-000009a0: 010a 010a 010c 020e 0172 3a00 0000 2902  .........r:...).
-000009b0: 7202 0000 0072 0300 0000 2910 720e 0000  r....r....).r...
-000009c0: 0072 0400 0000 7211 0000 00da 0c53 7973  .r....r......Sys
-000009d0: 7465 6d52 616e 646f 6d72 0c00 0000 da13  temRandomr......
-000009e0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-000009f0: 726f 72da 0877 6172 6e69 6e67 73da 0477  ror..warnings..w
-00000a00: 6172 6e72 1700 0000 721c 0000 0072 2500  arnr....r....r%.
-00000a10: 0000 722f 0000 0072 3200 0000 7234 0000  ..r/...r2...r4..
-00000a20: 0072 3800 0000 723a 0000 0072 0900 0000  .r8...r:...r....
-00000a30: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-00000a40: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
-00000a50: 0000 0801 0801 0802 0201 0801 0801 0e01  ................
-00000a60: 0801 0a02 0a03 0a18 0809 0816 0806 0804  ................
-00000a70: 0806 0808                                ....
+00000000: 420d 0d0a 0000 0000 76b0 eb63 e60a 0000  B.......v..c....
+00000010: e300 0000 0000 0000 0000 0000 0008 0000  ................
+00000020: 0040 0000 0073 9a00 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 5a00 6400 6401 6c01 5a01 6400 6401 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 7910 6501 a003 a100 5a01 6402 5a04  Z.y.e.....Z.d.Z.
+00000050: 5700 6e2a 0400 6505 6b0a 7252 0100 0100  W.n*..e.k.rR....
+00000060: 0100 6400 6401 6c06 5a06 6506 a007 6403  ..d.d.l.Z.e...d.
+00000070: a101 0100 6404 5a04 5900 6e02 5800 6417  ....d.Z.Y.n.X.d.
+00000080: 6407 6408 8401 5a08 6409 640a 8400 5a09  d.d...Z.d.d...Z.
+00000090: 640b 640c 8400 5a0a 640d 640e 8400 5a0b  d.d...Z.d.d...Z.
+000000a0: 640f 6410 8400 5a0c 6411 6412 8400 5a0d  d.d...Z.d.d...Z.
+000000b0: 6413 6414 8400 5a0e 6415 6416 8400 5a0f  d.d...Z.d.d...Z.
+000000c0: 6401 5300 2918 e900 0000 004e 547a 6a41  d.S.)......NTzjA
+000000d0: 2073 6563 7572 6520 7073 6575 646f 2d72   secure pseudo-r
+000000e0: 616e 646f 6d20 6e75 6d62 6572 2067 656e  andom number gen
+000000f0: 6572 6174 6f72 2069 7320 6e6f 7420 6176  erator is not av
+00000100: 6169 6c61 626c 6520 6f6e 2079 6f75 7220  ailable on your 
+00000110: 7379 7374 656d 2e20 4661 6c6c 696e 6720  system. Falling 
+00000120: 6261 636b 2074 6f20 4d65 7273 656e 6e65  back to Mersenne
+00000130: 2054 7769 7374 6572 2e46 da3e 6162 6364   Twister.F.>abcd
+00000140: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
+00000150: 7576 7778 797a 4142 4344 4546 4748 494a  uvwxyzABCDEFGHIJ
+00000160: 4b4c 4d4e 4f50 5152 5354 5556 5758 595a  KLMNOPQRSTUVWXYZ
+00000170: 3031 3233 3435 3637 3839 da00 6303 0000  0123456789..c...
+00000180: 0000 0000 0003 0000 0008 0000 0003 0000  ................
+00000190: 0073 4c00 0000 7400 7330 7401 a002 7403  .sL...t.s0t...t.
+000001a0: a004 6401 7401 a005 a100 7406 a006 a100  ..d.t.....t.....
+000001b0: 7c02 6603 1600 a007 6402 a101 a101 a008  |.f.....d.......
+000001c0: a100 a101 0100 6403 a009 8700 6601 6404  ......d.....f.d.
+000001d0: 6405 8408 740a 7c00 8301 4400 8301 a101  d...t.|...D.....
+000001e0: 5300 2906 7ab4 0a20 2020 2052 6574 7572  S.).z..    Retur
+000001f0: 6e73 2061 2073 6563 7572 656c 7920 6765  ns a securely ge
+00000200: 6e65 7261 7465 6420 7261 6e64 6f6d 2073  nerated random s
+00000210: 7472 696e 672e 0a0a 2020 2020 5468 6520  tring...    The 
+00000220: 6465 6661 756c 7420 6c65 6e67 7468 206f  default length o
+00000230: 6620 3132 2077 6974 6820 7468 6520 612d  f 12 with the a-
+00000240: 7a2c 2041 2d5a 2c20 302d 3920 6368 6172  z, A-Z, 0-9 char
+00000250: 6163 7465 7220 7365 7420 7265 7475 726e  acter set return
+00000260: 730a 2020 2020 6120 3731 2d62 6974 2076  s.    a 71-bit v
+00000270: 616c 7565 2e20 6c6f 675f 3228 2832 362b  alue. log_2((26+
+00000280: 3236 2b31 3029 5e31 3229 203d 7e20 3731  26+10)^12) =~ 71
+00000290: 2062 6974 730a 2020 2020 7a06 2573 2573   bits.    z.%s%s
+000002a0: 2573 7a05 7574 662d 3872 0300 0000 6301  %sz.utf-8r....c.
+000002b0: 0000 0000 0000 0002 0000 0004 0000 0033  ...............3
+000002c0: 0000 0073 1800 0000 7c00 5d10 7d01 7400  ...s....|.].}.t.
+000002d0: a001 8800 a101 5600 0100 7102 6400 5300  ......V...q.d.S.
+000002e0: 2901 4e29 02da 0672 616e 646f 6dda 0663  ).N)...random..c
+000002f0: 686f 6963 6529 02da 022e 30da 0169 2901  hoice)....0..i).
+00000300: da0d 616c 6c6f 7765 645f 6368 6172 73a9  ..allowed_chars.
+00000310: 00fa 632f 5573 6572 732f 6631 6e61 6c2f  ..c/Users/f1nal/
+00000320: 4472 6f70 626f 782f 7079 7468 6f6e 2f6a  Dropbox/python/j
+00000330: 6574 2d62 7269 6467 652f 7372 632f 7061  et-bridge/src/pa
+00000340: 636b 6167 6573 2f6a 6574 5f62 7269 6467  ckages/jet_bridg
+00000350: 655f 6261 7365 2f6a 6574 5f62 7269 6467  e_base/jet_bridg
+00000360: 655f 6261 7365 2f75 7469 6c73 2f63 6f6d  e_base/utils/com
+00000370: 6d6f 6e2e 7079 fa09 3c67 656e 6578 7072  mon.py..<genexpr
+00000380: 3e24 0000 0073 0200 0000 0400 7a24 6765  >$...s......z$ge
+00000390: 745f 7261 6e64 6f6d 5f73 7472 696e 672e  t_random_string.
+000003a0: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+000003b0: 723e 290b da0f 7573 696e 675f 7379 7372  r>)...using_sysr
+000003c0: 616e 646f 6d72 0400 0000 da04 7365 6564  andomr......seed
+000003d0: da07 6861 7368 6c69 62da 0673 6861 3235  ..hashlib..sha25
+000003e0: 36da 0867 6574 7374 6174 65da 0474 696d  6..getstate..tim
+000003f0: 65da 0665 6e63 6f64 65da 0664 6967 6573  e..encode..diges
+00000400: 74da 046a 6f69 6eda 0572 616e 6765 2903  t..join..range).
+00000410: da06 6c65 6e67 7468 7208 0000 005a 0473  ..lengthr....Z.s
+00000420: 616c 7472 0900 0000 2901 7208 0000 0072  altr....).r....r
+00000430: 0a00 0000 da11 6765 745f 7261 6e64 6f6d  ......get_random
+00000440: 5f73 7472 696e 670f 0000 0073 1000 0000  _string....s....
+00000450: 0007 0407 0401 0401 0201 0601 0601 1602  ................
+00000460: 7217 0000 0063 0200 0000 0000 0000 0400  r....c..........
+00000470: 0000 0400 0000 4300 0000 7328 0000 0078  ......C...s(...x
+00000480: 2274 007c 0083 0144 005d 165c 027d 027d  "t.|...D.].\.}.}
+00000490: 037c 017c 037c 0283 0272 0a7c 0253 0071  .|.|.|...r.|.S.q
+000004a0: 0a57 0064 0053 0029 014e 2901 da09 656e  .W.d.S.).N)...en
+000004b0: 756d 6572 6174 6529 04da 046c 6973 74da  umerate)...list.
+000004c0: 0970 7265 6469 6361 7465 7207 0000 00da  .predicater.....
+000004d0: 0576 616c 7565 7209 0000 0072 0900 0000  .valuer....r....
+000004e0: 720a 0000 00da 0a66 696e 645f 696e 6465  r......find_inde
+000004f0: 7827 0000 0073 0800 0000 0001 1201 0a01  x'...s..........
+00000500: 0801 721c 0000 0063 0200 0000 0000 0000  ..r....c........
+00000510: 0600 0000 0700 0000 0300 0000 73ae 0000  ............s...
+00000520: 0078 a87c 01a0 00a1 0044 005d 9c5c 027d  .x.|.....D.].\.}
+00000530: 027d 037c 0264 016b 0272 247c 037c 007c  .}.|.d.k.r$|.|.|
+00000540: 023c 0071 0a74 017c 0374 0283 0272 467c  .<.q.t.|.t...rF|
+00000550: 00a0 037c 0269 00a1 027d 0474 047c 047c  ...|.i...}.t.|.|
+00000560: 0383 0201 0071 0a74 017c 0374 0583 0272  .....q.t.|.t...r
+00000570: 9e7c 00a0 037c 0267 00a1 027d 0478 487c  .|...|.g...}.xH|
+00000580: 0344 005d 3689 0074 067c 0487 0066 0164  .D.]6..t.|...f.d
+00000590: 0264 0384 0883 027d 057c 0564 006b 0872  .d.....}.|.d.k.r
+000005a0: 8271 627c 047c 0519 0001 0074 047c 047c  .qb|.|.....t.|.|
+000005b0: 0519 0088 0083 0201 0071 6257 0071 0a7c  .........qbW.q.|
+000005c0: 037c 007c 023c 0071 0a57 007c 0053 0029  .|.|.<.q.W.|.S.)
+000005d0: 044e da06 7061 7261 6d73 6302 0000 0000  .N..paramsc.....
+000005e0: 0000 0002 0000 0003 0000 0013 0000 0073  ...............s
+000005f0: 1000 0000 7c00 6401 1900 8800 6401 1900  ....|.d.....d...
+00000600: 6b02 5300 2902 4e5a 0964 625f 636f 6c75  k.S.).NZ.db_colu
+00000610: 6d6e 7209 0000 0029 02da 0178 7207 0000  mnr....)...xr...
+00000620: 0029 01da 0469 7465 6d72 0900 0000 720a  .)...itemr....r.
+00000630: 0000 00da 083c 6c61 6d62 6461 3e3b 0000  .....<lambda>;..
+00000640: 00f3 0000 0000 7a17 6d65 7267 652e 3c6c  ......z.merge.<l
+00000650: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00000660: 07da 0569 7465 6d73 da0a 6973 696e 7374  ...items..isinst
+00000670: 616e 6365 da04 6469 6374 da0a 7365 7464  ance..dict..setd
+00000680: 6566 6175 6c74 da05 6d65 7267 6572 1900  efault..merger..
+00000690: 0000 721c 0000 0029 06da 0b64 6573 7469  ..r....)...desti
+000006a0: 6e61 7469 6f6e da06 736f 7572 6365 da03  nation..source..
+000006b0: 6b65 7972 1b00 0000 da04 6e6f 6465 da05  keyr......node..
+000006c0: 696e 6465 7872 0900 0000 2901 721f 0000  indexr....).r...
+000006d0: 0072 0a00 0000 7226 0000 0030 0000 0073  .r....r&...0...s
+000006e0: 2000 0000 0001 1201 0801 0a01 0a01 0c01   ...............
+000006f0: 0c01 0a01 0c02 0a01 1201 0801 0201 0801  ................
+00000700: 1402 0c02 7226 0000 0063 0200 0000 0000  ....r&...c......
+00000710: 0000 0300 0000 0300 0000 4300 0000 7316  ..........C...s.
+00000720: 0000 007c 00a0 00a1 007d 027c 02a0 017c  ...|.....}.|...|
+00000730: 01a1 0101 007c 0253 0029 014e 2902 da04  .....|.S.).N)...
+00000740: 636f 7079 da06 7570 6461 7465 2903 721e  copy..update).r.
+00000750: 0000 00da 0179 da01 7a72 0900 0000 7209  .....y..zr....r.
+00000760: 0000 0072 0a00 0000 da0f 6d65 7267 655f  ...r......merge_
+00000770: 7477 6f5f 6469 6374 7346 0000 0073 0600  two_dictsF...s..
+00000780: 0000 0001 0801 0a01 7230 0000 0063 0100  ........r0...c..
+00000790: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000007a0: 0000 730c 0000 0074 0074 017c 0083 0183  ..s....t.t.|....
+000007b0: 0153 0029 014e 2902 da04 6e65 7874 da04  .S.).N)...next..
+000007c0: 6974 6572 2901 721b 0000 0072 0900 0000  iter).r....r....
+000007d0: 7209 0000 0072 0a00 0000 da0d 6765 745f  r....r......get_
+000007e0: 7365 745f 6669 7273 744c 0000 0073 0200  set_firstL...s..
+000007f0: 0000 0001 7233 0000 0063 0100 0000 0000  ....r3...c......
+00000800: 0000 0100 0000 0200 0000 4300 0000 7314  ..........C...s.
+00000810: 0000 007c 0064 006b 0872 0c64 0153 0074  ...|.d.k.r.d.S.t
+00000820: 007c 0083 0153 0029 024e 7203 0000 0029  .|...S.).Nr....)
+00000830: 01da 0373 7472 2901 721b 0000 0072 0900  ...str).r....r..
+00000840: 0000 7209 0000 0072 0a00 0000 da0f 616e  ..r....r......an
+00000850: 795f 7479 7065 5f73 6f72 7465 7250 0000  y_type_sorterP..
+00000860: 0073 0600 0000 0001 0801 0401 7235 0000  .s..........r5..
+00000870: 0063 0100 0000 0000 0000 0300 0000 0400  .c..............
+00000880: 0000 4300 0000 7328 0000 0067 007d 0178  ..C...s(...g.}.x
+00000890: 1e7c 0044 005d 167d 027c 027c 016b 0772  .|.D.].}.|.|.k.r
+000008a0: 0a7c 01a0 007c 02a1 0101 0071 0a57 007c  .|...|.....q.W.|
+000008b0: 0153 0029 014e 2901 da06 6170 7065 6e64  .S.).N)...append
+000008c0: 2903 da03 6172 72da 0672 6573 756c 7472  )...arr..resultr
+000008d0: 1f00 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+000008e0: 0000 00da 0675 6e69 7175 6556 0000 0073  .....uniqueV...s
+000008f0: 0a00 0000 0001 0401 0a01 0801 0e01 7239  ..............r9
+00000900: 0000 0063 0100 0000 0000 0000 0300 0000  ...c............
+00000910: 0400 0000 4300 0000 7336 0000 0067 007d  ....C...s6...g.}
+00000920: 0178 2c7c 0044 005d 247d 0274 007c 0274  .x,|.D.]$}.t.|.t
+00000930: 0183 0272 247c 01a0 027c 02a1 0101 0071  ...r$|...|.....q
+00000940: 0a7c 01a0 037c 02a1 0101 0071 0a57 007c  .|...|.....q.W.|
+00000950: 0153 0029 014e 2904 7223 0000 0072 1900  .S.).N).r#...r..
+00000960: 0000 da06 6578 7465 6e64 7236 0000 0029  ....extendr6...)
+00000970: 0372 3700 0000 7238 0000 0072 1f00 0000  .r7...r8...r....
+00000980: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
+00000990: 0766 6c61 7474 656e 5e00 0000 730c 0000  .flatten^...s...
+000009a0: 0000 0104 010a 010a 010c 020e 0172 3b00  .............r;.
+000009b0: 0000 2902 7202 0000 0072 0300 0000 2910  ..).r....r....).
+000009c0: 720e 0000 0072 0400 0000 7211 0000 00da  r....r....r.....
+000009d0: 0c53 7973 7465 6d52 616e 646f 6d72 0c00  .SystemRandomr..
+000009e0: 0000 da13 4e6f 7449 6d70 6c65 6d65 6e74  ....NotImplement
+000009f0: 6564 4572 726f 72da 0877 6172 6e69 6e67  edError..warning
+00000a00: 73da 0477 6172 6e72 1700 0000 721c 0000  s..warnr....r...
+00000a10: 0072 2600 0000 7230 0000 0072 3300 0000  .r&...r0...r3...
+00000a20: 7235 0000 0072 3900 0000 723b 0000 0072  r5...r9...r;...r
+00000a30: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00000a40: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000a50: 0073 2200 0000 0801 0801 0802 0201 0801  .s".............
+00000a60: 0801 0e01 0801 0a02 0a03 0a18 0809 0816  ................
+00000a70: 0806 0804 0806 0808                      ........
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/common.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/common.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/crypt.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/crypt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/async_exec.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/async_exec.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/db_types.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/db_types.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/db_types.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/db_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/exceptions.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/siblings.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/siblings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/http.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/http.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/graphql.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/graphql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/backend.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/backend.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/track_database.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/track_database.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/queryset.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/queryset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/gql.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/gql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/type_codes.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/type_codes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/siblings.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/siblings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/http.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/http.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/backend.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/backend.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/__pycache__/relations.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/__pycache__/relations.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/track_model.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/track_model.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/common.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,7 +95,15 @@
     result = []
     for item in arr:
         if isinstance(item, list):
             result.extend(item)
         else:
             result.append(item)
     return result
+
+
+def format_size(num, suffix='B'):
+    for unit in ('', 'Ki', 'Mi', 'Gi', 'Ti', 'Pi', 'Ei', 'Zi'):
+        if abs(num) < 1024.0:
+            return f'{num:3.1f}{unit}{suffix}'
+        num /= 1024.0
+    return f'{num:.1f}Yi{suffix}'
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/siblings.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/siblings.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/http.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/http.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/type_codes.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/type_codes.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/track_database.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/track_database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 from fnmatch import fnmatch
 import requests
 
 from jet_bridge_base import settings
 from jet_bridge_base.db import get_conf
+from jet_bridge_base.sentry import sentry_controller
 from jet_bridge_base.utils.async_exec import as_future
 
 
 def track_database(request):
     if not settings.TRACK_DATABASES_ENDPOINT:
         return
 
     track_databases = list(filter(lambda x: x != '', map(lambda x: x.lower().strip(), settings.TRACK_DATABASES.split(','))))
     conf = get_conf(request)
     hostname = '{}:{}'.format(conf.get('host', ''), conf.get('port', '')).lower()
 
-    if any(map(lambda x: fnmatch(hostname, x), track_databases)):
-        headers = {}
-        data = {
-            'databaseName': conf.get('name', ''),
-            'databaseSchema': conf.get('schema', ''),
-            'databaseHost': conf.get('host', ''),
-            'databasePort': conf.get('port', '')
-        }
+    if not any(map(lambda x: fnmatch(hostname, x), track_databases)):
+        return
+
+    headers = {}
+    data = {
+        'databaseName': conf.get('name', ''),
+        'databaseSchema': conf.get('schema', ''),
+        'databaseHost': conf.get('host', ''),
+        'databasePort': conf.get('port', '')
+    }
 
-        if settings.TRACK_DATABASES_AUTH:
-            headers['Authorization'] = settings.TRACK_DATABASES_AUTH
+    if settings.TRACK_DATABASES_AUTH:
+        headers['Authorization'] = settings.TRACK_DATABASES_AUTH
+
+    try:
+        r = requests.post(settings.TRACK_DATABASES_ENDPOINT, headers=headers, json=data)
+        success = 200 <= r.status_code < 300
 
-        requests.request('POST', settings.TRACK_DATABASES_ENDPOINT, headers=headers, json=data)
+        if not success:
+            error = 'TRACK_DATABASE request error: {} {} {}'.format(r.status_code, r.reason, r.text)
+            sentry_controller.capture_message(error)
+    except Exception as e:
+        sentry_controller.capture_exception(e)
 
 
 def track_database_async(request):
     if not settings.TRACK_DATABASES_ENDPOINT:
         return
 
     try:
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/queryset.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/queryset.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/utils/exceptions.py` & `jet-bridge-base-1.8.2/jet_bridge_base/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/model_relation_override.py` & `jet-bridge-base-1.8.2/jet_bridge_base/models/model_relation_override.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/data_types.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/data_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/column.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/column.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/model_relation_override.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/model_relation_override.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/table.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/__pycache__/data_types.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/models/__pycache__/data_types.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/models/data_types.py` & `jet-bridge-base-1.8.2/jet_bridge_base/models/data_types.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/media_cache.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/media_cache.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/encoders.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/encoders.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/status.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/status.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/messages.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/messages.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/settings.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/messages.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/messages.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/logger.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/request.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/request.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-00000000: 330d 0d0a 76b0 eb63 3414 0000 e300 0000  3...v..c4.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 6a00 0000 6400 6401 6c00 5a00 6400  .sj...d.d.l.Z.d.
-00000030: 6402 6c00 6d01 5a01 0100 6400 6403 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6406 6c08 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 0100 650c 8300 5a0d 4700 6408  m.Z...e...Z.G.d.
-00000080: 6409 8400 6409 650c 8303 5a0e 6401 5300  d...d.e...Z.d.S.
-00000090: 290a e900 0000 004e 2901 da0f 4a53 4f4e  )......N)...JSON
-000000a0: 4465 636f 6465 4572 726f 7229 01da 0c52  DecodeError)...R
-000000b0: 6571 7565 7374 4572 726f 7229 01da 0f56  equestError)...V
-000000c0: 616c 6964 6174 696f 6e45 7272 6f72 2901  alidationError).
-000000d0: da0c 7374 7269 6e67 5f74 7970 6573 2901  ..string_types).
-000000e0: da08 7365 7474 696e 6773 2901 da14 4d69  ..settings)...Mi
-000000f0: 7373 696e 6741 7267 756d 656e 7445 7272  ssingArgumentErr
-00000100: 6f72 6300 0000 0000 0000 0000 0000 000e  orc.............
-00000110: 0000 0040 0000 0073 9e00 0000 6500 5a01  ...@...s....e.Z.
-00000120: 6400 5a02 6401 5a03 6401 5a04 6401 5a05  d.Z.d.Z.d.Z.d.Z.
-00000130: 6401 5a06 6401 5a07 6900 5a08 641b 6402  d.Z.d.Z.i.Z.d.d.
-00000140: 6403 8401 5a09 6404 6405 8400 5a0a 650b  d...Z.d.d...Z.e.
-00000150: 6406 6602 6407 6408 8401 5a0c 641c 6409  d.f.d.d...Z.d.d.
-00000160: 640a 8401 5a0d 650b 6601 640b 640c 8401  d...Z.e.f.d.d...
-00000170: 5a0e 650b 6406 6602 640d 640e 8401 5a0f  Z.e.d.f.d.d...Z.
-00000180: 641d 640f 6410 8401 5a10 6411 6412 8400  d.d.d...Z.d.d...
-00000190: 5a11 6413 6414 8400 5a12 641e 6415 6416  Z.d.d...Z.d.d.d.
-000001a0: 8401 5a13 641f 6417 6418 8401 5a14 6419  ..Z.d.d.d...Z.d.
-000001b0: 641a 8400 5a15 6401 5300 2920 da07 5265  d...Z.d.S.) ..Re
-000001c0: 7175 6573 744e 630f 0000 0000 0000 0014  questNc.........
-000001d0: 0000 0010 0000 0003 0000 0073 1c01 0000  ...........s....
-000001e0: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
-000001f0: 5f02 7c04 7c00 5f03 7c05 7c00 5f04 7c06  _.|.|._.|.|._.|.
-00000200: 7c00 5f05 7c07 702a 6900 7c00 5f06 7c08  |._.|.p*i.|._.|.
-00000210: 7034 6900 7c00 5f07 7c09 7c00 5f08 7c0a  p4i.|._.|.|._.|.
-00000220: 7044 6900 7c00 5f09 7c0b 704e 6900 7c00  pDi.|._.|.pNi.|.
-00000230: 5f0a 7c0c 7c00 5f0b 7c0d 7c00 5f0c 7c0e  _.|.|._.|.|._.|.
-00000240: 7c00 5f0d 7c00 6a07 6a0e 6401 6402 8302  |._.|.j.j.d.d...
-00000250: 7d0f 7c0f 6a0f 6403 8301 72e6 7c00 6a08  }.|.j.d...r.|.j.
-00000260: 7d10 7410 7c10 7411 8302 7398 7c10 6a12  }.t.|.t...s.|.j.
-00000270: 6404 6405 8302 7d10 7918 7c10 72a8 7413  d.d...}.y.|.r.t.
-00000280: 6a14 7c10 8301 6e02 6900 7c00 5f15 5700  j.|...n.i.|._.W.
-00000290: 6e32 0400 7416 6b0a 72e2 0100 7d11 0100  n2..t.k.r...}...
-000002a0: 7a16 7417 7c00 6406 6a18 7c11 8301 8302  z.t.|.d.j.|.....
-000002b0: 8201 5700 5900 6400 6400 7d11 7e11 5800  ..W.Y.d.d.}.~.X.
-000002c0: 6e02 5800 6e32 6407 6408 8400 8900 8700  n.X.n2d.d.......
-000002d0: 6601 6409 640a 8408 7d12 7419 741a 7c12  f.d.d...}.t.t.|.
-000002e0: 7c00 6a09 6a1b 8300 8302 8301 7d13 741c  |.j.j.......}.t.
-000002f0: 7c13 8301 7c00 5f15 6400 5300 290b 4e5a  |...|._.d.S.).NZ
-00000300: 0c43 4f4e 5445 4e54 5f54 5950 45da 007a  .CONTENT_TYPE..z
-00000310: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00000320: 6e7a 0575 7466 2d38 da0d 7375 7272 6f67  nz.utf-8..surrog
-00000330: 6174 6570 6173 737a 1749 6e63 6f72 7265  atepassz.Incorre
-00000340: 6374 204a 534f 4e20 626f 6479 3a20 7b7d  ct JSON body: {}
-00000350: 6301 0000 0000 0000 0001 0000 0009 0000  c...............
-00000360: 0053 0000 0073 2a00 0000 7400 7c00 7401  .S...s*...t.|.t.
-00000370: 8302 7226 790e 7c00 6a02 6401 8301 7d00  ..r&y.|.j.d...}.
-00000380: 5700 6e0c 0100 0100 0100 5900 6e02 5800  W.n.......Y.n.X.
-00000390: 7c00 5300 2902 4e7a 0575 7466 2d38 2903  |.S.).Nz.utf-8).
-000003a0: da0a 6973 696e 7374 616e 6365 da05 6279  ..isinstance..by
-000003b0: 7465 73da 0664 6563 6f64 6529 01da 0576  tes..decode)...v
-000003c0: 616c 7565 a900 720f 0000 00fa 5e2f 5573  alue..r.....^/Us
-000003d0: 6572 732f 6631 6e61 6c2f 4472 6f70 626f  ers/f1nal/Dropbo
-000003e0: 782f 7079 7468 6f6e 2f6a 6574 2d62 7269  x/python/jet-bri
-000003f0: 6467 652f 7372 632f 7061 636b 6167 6573  dge/src/packages
-00000400: 2f6a 6574 5f62 7269 6467 655f 6261 7365  /jet_bridge_base
-00000410: 2f6a 6574 5f62 7269 6467 655f 6261 7365  /jet_bridge_base
-00000420: 2f72 6571 7565 7374 2e70 79da 1362 6f64  /request.py..bod
-00000430: 795f 6172 6775 6d65 6e74 5f76 616c 7565  y_argument_value
-00000440: 4300 0000 730c 0000 0000 010a 0102 010e  C...s...........
-00000450: 0106 0106 017a 2d52 6571 7565 7374 2e5f  .....z-Request._
-00000460: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00000470: 2e62 6f64 795f 6172 6775 6d65 6e74 5f76  .body_argument_v
-00000480: 616c 7565 6301 0000 0000 0000 0003 0000  aluec...........
-00000490: 0004 0000 0013 0000 0073 4e00 0000 7c00  .........sN...|.
-000004a0: 5c02 7d01 7d02 7400 7401 8800 7c02 8302  \.}.}.t.t...|...
-000004b0: 8301 7d02 7402 7c02 8301 6401 6b04 722a  ..}.t.|...d.k.r*
-000004c0: 7c01 7c02 6602 5300 7402 7c02 8301 6401  |.|.f.S.t.|...d.
-000004d0: 6b02 7242 7c01 7c02 6402 1900 6602 5300  k.rB|.|.d...f.S.
-000004e0: 7c01 6400 6602 5300 6400 5300 2903 4ee9  |.d.f.S.d.S.).N.
-000004f0: 0100 0000 7201 0000 0029 03da 046c 6973  ....r....)...lis
-00000500: 74da 036d 6170 da03 6c65 6e29 03da 0469  t..map..len)...i
-00000510: 7465 6dda 036b 6579 da06 7661 6c75 6573  tem..key..values
-00000520: 2901 7211 0000 0072 0f00 0000 7210 0000  ).r....r....r...
-00000530: 00da 086d 6170 5f69 7465 6d4b 0000 0073  ...map_itemK...s
-00000540: 0e00 0000 0001 0801 0e01 0c01 0801 0c01  ................
-00000550: 0c02 7a22 5265 7175 6573 742e 5f5f 696e  ..z"Request.__in
-00000560: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6d61  it__.<locals>.ma
-00000570: 705f 6974 656d 291d da06 6d65 7468 6f64  p_item)...method
-00000580: da08 7072 6f74 6f63 6f6c da04 686f 7374  ..protocol..host
-00000590: da04 7061 7468 da0b 7061 7468 5f6b 7761  ..path..path_kwa
-000005a0: 7267 73da 0375 7269 da0f 7175 6572 795f  rgs..uri..query_
-000005b0: 6172 6775 6d65 6e74 73da 0768 6561 6465  arguments..heade
-000005c0: 7273 da04 626f 6479 da0e 626f 6479 5f61  rs..body..body_a
-000005d0: 7267 756d 656e 7473 da05 6669 6c65 73da  rguments..files.
-000005e0: 106f 7269 6769 6e61 6c5f 7265 7175 6573  .original_reques
-000005f0: 74da 106f 7269 6769 6e61 6c5f 6861 6e64  t..original_hand
-00000600: 6c65 72da 0661 6374 696f 6eda 0367 6574  ler..action..get
-00000610: da0a 7374 6172 7473 7769 7468 720b 0000  ..startswithr...
-00000620: 0072 0500 0000 720d 0000 00da 046a 736f  .r....r......jso
-00000630: 6eda 056c 6f61 6473 da04 6461 7461 da0a  n..loads..data..
-00000640: 5661 6c75 6545 7272 6f72 7203 0000 00da  ValueErrorr.....
-00000650: 0666 6f72 6d61 7472 1300 0000 7214 0000  .formatr....r...
-00000660: 00da 0569 7465 6d73 da04 6469 6374 2914  ...items..dict).
-00000670: da04 7365 6c66 721a 0000 0072 1b00 0000  ..selfr....r....
-00000680: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000690: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-000006a0: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-000006b0: 0000 7226 0000 0072 2700 0000 da0c 636f  ..r&...r'.....co
-000006c0: 6e74 656e 745f 7479 7065 722c 0000 00da  ntent_typer,....
-000006d0: 0165 7219 0000 00da 0674 7570 6c65 7372  .er......tuplesr
-000006e0: 0f00 0000 2901 7211 0000 0072 1000 0000  ....).r....r....
-000006f0: da08 5f5f 696e 6974 5f5f 1700 0000 7336  ..__init__....s6
-00000700: 0000 0000 1106 0106 0106 0106 0106 0106  ................
-00000710: 010a 010a 0106 010a 010a 0106 0106 0106  ................
-00000720: 020e 020a 0106 020a 010c 0102 0118 0110  ................
-00000730: 0124 0208 080c 0a14 017a 1052 6571 7565  .$.......z.Reque
-00000740: 7374 2e5f 5f69 6e69 745f 5f63 0100 0000  st.__init__c....
-00000750: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000760: 7316 0000 007c 006a 0064 0117 007c 006a  s....|.j.d...|.j
-00000770: 0117 007c 006a 0217 0053 0029 024e 7a03  ...|.j...S.).Nz.
-00000780: 3a2f 2f29 0372 1b00 0000 721c 0000 0072  ://).r....r....r
-00000790: 1f00 0000 2901 7231 0000 0072 0f00 0000  ....).r1...r....
-000007a0: 720f 0000 0072 1000 0000 da08 6675 6c6c  r....r......full
-000007b0: 5f75 726c 5800 0000 7302 0000 0000 017a  _urlX...s......z
-000007c0: 1052 6571 7565 7374 2e66 756c 6c5f 7572  .Request.full_ur
-000007d0: 6c54 6304 0000 0000 0000 0004 0000 0005  lTc.............
-000007e0: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
-000007f0: 7c01 7c02 7c00 6a01 7c03 8304 5300 2901  |.|.|.j.|...S.).
-00000800: 4e29 02da 0d5f 6765 745f 6172 6775 6d65  N)..._get_argume
-00000810: 6e74 7220 0000 0029 0472 3100 0000 da04  ntr ...).r1.....
-00000820: 6e61 6d65 da07 6465 6661 756c 74da 0573  name..default..s
-00000830: 7472 6970 720f 0000 0072 0f00 0000 7210  tripr....r....r.
-00000840: 0000 00da 0c67 6574 5f61 7267 756d 656e  .....get_argumen
-00000850: 745b 0000 0073 0200 0000 0001 7a14 5265  t[...s......z.Re
-00000860: 7175 6573 742e 6765 745f 6172 6775 6d65  quest.get_argume
-00000870: 6e74 6303 0000 0000 0000 0003 0000 0004  ntc.............
-00000880: 0000 0043 0000 0073 1000 0000 7c00 6a00  ...C...s....|.j.
-00000890: 7c01 7c00 6a01 7c02 8303 5300 2901 4e29  |.|.j.|...S.).N)
-000008a0: 02da 0e5f 6765 745f 6172 6775 6d65 6e74  ..._get_argument
-000008b0: 7372 2000 0000 2903 7231 0000 0072 3800  sr ...).r1...r8.
-000008c0: 0000 723a 0000 0072 0f00 0000 720f 0000  ..r:...r....r...
-000008d0: 0072 1000 0000 da0d 6765 745f 6172 6775  .r......get_argu
-000008e0: 6d65 6e74 735e 0000 0073 0200 0000 0001  ments^...s......
-000008f0: 7a15 5265 7175 6573 742e 6765 745f 6172  z.Request.get_ar
-00000900: 6775 6d65 6e74 7363 0300 0000 0000 0000  gumentsc........
-00000910: 0500 0000 0200 0000 4300 0000 733a 0000  ........C...s:..
-00000920: 007c 006a 007c 0183 017d 0374 017c 0383  .|.j.|...}.t.|..
-00000930: 0164 016b 0272 1c7c 027d 046e 1a74 017c  .d.k.r.|.}.n.t.|
-00000940: 0383 0164 026b 0272 327c 0364 0119 007d  ...d.k.r2|.d...}
-00000950: 046e 047c 037d 047c 0453 0029 034e 7201  .n.|.}.|.S.).Nr.
-00000960: 0000 0072 1200 0000 2902 723d 0000 0072  ...r....).r=...r
-00000970: 1500 0000 2905 7231 0000 0072 3800 0000  ....).r1...r8...
-00000980: 7239 0000 0072 1800 0000 720e 0000 0072  r9...r....r....r
-00000990: 0f00 0000 720f 0000 0072 1000 0000 da11  ....r....r......
-000009a0: 6765 745f 6172 6775 6d65 6e74 5f73 6166  get_argument_saf
-000009b0: 6561 0000 0073 0e00 0000 0001 0a02 0c01  ea...s..........
-000009c0: 0601 0c01 0a02 0402 7a19 5265 7175 6573  ........z.Reques
-000009d0: 742e 6765 745f 6172 6775 6d65 6e74 5f73  t.get_argument_s
-000009e0: 6166 6563 0400 0000 0000 0000 0400 0000  afec............
-000009f0: 0500 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
-00000a00: 007c 017c 027c 006a 017c 0383 0453 0029  .|.|.|.j.|...S.)
-00000a10: 014e 2902 7237 0000 0072 2300 0000 2904  .N).r7...r#...).
-00000a20: 7231 0000 0072 3800 0000 7239 0000 0072  r1...r8...r9...r
-00000a30: 3a00 0000 720f 0000 0072 0f00 0000 7210  :...r....r....r.
-00000a40: 0000 00da 1167 6574 5f62 6f64 795f 6172  .....get_body_ar
-00000a50: 6775 6d65 6e74 6d00 0000 7302 0000 0000  gumentm...s.....
-00000a60: 017a 1952 6571 7565 7374 2e67 6574 5f62  .z.Request.get_b
-00000a70: 6f64 795f 6172 6775 6d65 6e74 6303 0000  ody_argumentc...
-00000a80: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00000a90: 0073 1000 0000 7c00 6a00 7c01 7c00 6a01  .s....|.j.|.|.j.
-00000aa0: 7c02 8303 5300 2901 4e29 0272 3c00 0000  |...S.).N).r<...
-00000ab0: 7223 0000 0029 0372 3100 0000 7238 0000  r#...).r1...r8..
-00000ac0: 0072 3a00 0000 720f 0000 0072 0f00 0000  .r:...r....r....
-00000ad0: 7210 0000 00da 1267 6574 5f62 6f64 795f  r......get_body_
-00000ae0: 6172 6775 6d65 6e74 7370 0000 0073 0200  argumentsp...s..
-00000af0: 0000 0001 7a1a 5265 7175 6573 742e 6765  ....z.Request.ge
-00000b00: 745f 626f 6479 5f61 7267 756d 656e 7473  t_body_arguments
-00000b10: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-00000b20: 0043 0000 0073 0c00 0000 7c00 6a00 6a01  .C...s....|.j.j.
-00000b30: 6401 8301 5300 2902 4e5a 0958 5f52 4541  d...S.).NZ.X_REA
-00000b40: 4c5f 4950 2902 7221 0000 0072 2800 0000  L_IP).r!...r(...
-00000b50: 2901 7231 0000 0072 0f00 0000 720f 0000  ).r1...r....r...
-00000b60: 0072 1000 0000 da06 6765 745f 6970 7300  .r......get_ips.
-00000b70: 0000 7302 0000 0000 017a 0e52 6571 7565  ..s......z.Reque
-00000b80: 7374 2e67 6574 5f69 7063 0100 0000 0000  st.get_ipc......
-00000b90: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
-00000ba0: 0000 007c 006a 006a 0164 0183 0153 0029  ...|.j.j.d...S.)
-00000bb0: 024e 5a0f 585f 5354 4943 4b5f 5345 5353  .NZ.X_STICK_SESS
-00000bc0: 494f 4e29 0272 2100 0000 7228 0000 0029  ION).r!...r(...)
-00000bd0: 0172 3100 0000 720f 0000 0072 0f00 0000  .r1...r....r....
-00000be0: 7210 0000 00da 1167 6574 5f73 7469 636b  r......get_stick
-00000bf0: 5f73 6573 7369 6f6e 7600 0000 7302 0000  _sessionv...s...
-00000c00: 0000 017a 1952 6571 7565 7374 2e67 6574  ...z.Request.get
-00000c10: 5f73 7469 636b 5f73 6573 7369 6f6e 6305  _stick_sessionc.
-00000c20: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-00000c30: 0000 0073 3000 0000 7c00 6a00 7c01 7c03  ...s0...|.j.|.|.
-00000c40: 7c04 6401 8d03 7d05 7c05 7328 7c02 7401  |.d...}.|.s(|.t.
-00000c50: 6b08 7224 7402 7c01 8301 8201 7c02 5300  k.r$t.|.....|.S.
-00000c60: 7c05 6403 1900 5300 2904 4e29 0172 3a00  |.d...S.).N).r:.
-00000c70: 0000 7212 0000 00e9 ffff ffff 2903 723c  ..r.........).r<
-00000c80: 0000 00da 0c5f 4152 475f 4445 4641 554c  ....._ARG_DEFAUL
-00000c90: 5472 0700 0000 2906 7231 0000 0072 3800  Tr....).r1...r8.
-00000ca0: 0000 7239 0000 00da 0673 6f75 7263 6572  ..r9.....sourcer
-00000cb0: 3a00 0000 da04 6172 6773 720f 0000 0072  :.....argsr....r
-00000cc0: 0f00 0000 7210 0000 0072 3700 0000 7900  ....r....r7...y.
-00000cd0: 0000 730c 0000 0000 0110 0104 0108 0108  ..s.............
-00000ce0: 0104 017a 1552 6571 7565 7374 2e5f 6765  ...z.Request._ge
-00000cf0: 745f 6172 6775 6d65 6e74 6304 0000 0000  t_argumentc.....
-00000d00: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
-00000d10: 4800 0000 6700 7d04 783e 7c02 6a00 7c01  H...g.}.x>|.j.|.
-00000d20: 6700 8302 4400 5d2e 7d05 7401 7c05 7402  g...D.].}.t.|.t.
-00000d30: 8302 722a 7c05 6a03 6401 8301 7d05 7c03  ..r*|.j.d...}.|.
-00000d40: 7236 7c05 6a04 8300 7d05 7c04 6a05 7c05  r6|.j...}.|.j.|.
-00000d50: 8301 0100 7112 5700 7c04 5300 2902 4e7a  ....q.W.|.S.).Nz
-00000d60: 0575 7466 2d38 2906 7228 0000 0072 0b00  .utf-8).r(...r..
-00000d70: 0000 720c 0000 0072 0d00 0000 723a 0000  ..r....r....r:..
-00000d80: 00da 0661 7070 656e 6429 0672 3100 0000  ...append).r1...
-00000d90: 7238 0000 0072 4500 0000 723a 0000 0072  r8...rE...r:...r
-00000da0: 1800 0000 da01 7672 0f00 0000 720f 0000  ......vr....r...
-00000db0: 0072 1000 0000 723c 0000 0081 0000 0073  .r....r<.......s
-00000dc0: 1000 0000 0001 0401 1201 0a01 0a06 0401  ................
-00000dd0: 0801 0e01 7a16 5265 7175 6573 742e 5f67  ....z.Request._g
-00000de0: 6574 5f61 7267 756d 656e 7473 6301 0000  et_argumentsc...
-00000df0: 0000 0000 0005 0000 000b 0000 0043 0000  .............C..
-00000e00: 0073 7400 0000 7c00 6a00 720c 7c00 6a00  .st...|.j.r.|.j.
-00000e10: 5300 7c00 6a01 6a02 6401 8301 7d01 7c01  S.|.j.j.d...}.|.
-00000e20: 7320 6400 5300 6402 6403 6c03 6d04 7d02  s d.S.d.d.l.m.}.
-00000e30: 0100 792e 7405 6a06 6a07 6404 6405 8302  ..y.t.j.j.d.d...
-00000e40: 6a08 8300 7d03 7c02 7c01 7c03 8302 7d04  j...}.|.|.|...}.
-00000e50: 7409 6a0a 7c04 8301 7c00 5f00 7c00 6a00  t.j.|...|._.|.j.
-00000e60: 5300 0400 740b 6b0a 726e 0100 0100 0100  S...t.k.rn......
-00000e70: 6400 5300 5800 6400 5300 2906 4e5a 1158  d.S.X.d.S.).NZ.X
-00000e80: 5f42 5249 4447 455f 5345 5454 494e 4753  _BRIDGE_SETTINGS
-00000e90: 7201 0000 0029 01da 0764 6563 7279 7074  r....)...decrypt
-00000ea0: fa01 2d72 0900 0000 290c da0f 6272 6964  ..-r....)...brid
-00000eb0: 6765 5f73 6574 7469 6e67 7372 2100 0000  ge_settingsr!...
-00000ec0: 7228 0000 00da 1b6a 6574 5f62 7269 6467  r(.....jet_bridg
-00000ed0: 655f 6261 7365 2e75 7469 6c73 2e63 7279  e_base.utils.cry
-00000ee0: 7074 7249 0000 0072 0600 0000 da05 544f  ptrI...r......TO
-00000ef0: 4b45 4eda 0772 6570 6c61 6365 da05 6c6f  KEN..replace..lo
-00000f00: 7765 7272 2a00 0000 722b 0000 00da 0945  werr*...r+.....E
-00000f10: 7863 6570 7469 6f6e 2905 7231 0000 005a  xception).r1...Z
-00000f20: 1762 7269 6467 655f 7365 7474 696e 6773  .bridge_settings
-00000f30: 5f65 6e63 6f64 6564 7249 0000 00da 0a73  _encodedrI.....s
-00000f40: 6563 7265 745f 6b65 795a 0964 6563 7279  ecret_keyZ.decry
-00000f50: 7074 6564 720f 0000 0072 0f00 0000 7210  ptedr....r....r.
-00000f60: 0000 00da 1367 6574 5f62 7269 6467 655f  .....get_bridge_
-00000f70: 7365 7474 696e 6773 9000 0000 731a 0000  settings....s...
-00000f80: 0000 0106 0106 020c 0204 0104 020c 0202  ................
-00000f90: 0112 010a 010c 0106 010e 017a 1b52 6571  ...........z.Req
-00000fa0: 7565 7374 2e67 6574 5f62 7269 6467 655f  uest.get_bridge_
-00000fb0: 7365 7474 696e 6773 290e 4e4e 4e4e 4e4e  settings).NNNNNN
-00000fc0: 4e4e 4e4e 4e4e 4e4e 2901 5429 0154 2901  NNNNNNNN).T).T).
-00000fd0: 5429 0154 2916 da08 5f5f 6e61 6d65 5f5f  T).T)...__name__
-00000fe0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000ff0: 7175 616c 6e61 6d65 5f5f da07 7365 7373  qualname__..sess
-00001000: 696f 6e72 4b00 0000 da07 7072 6f6a 6563  ionrK.....projec
-00001010: 74da 0b65 6e76 6972 6f6e 6d65 6e74 da0e  t..environment..
-00001020: 7265 736f 7572 6365 5f74 6f6b 656e da07  resource_token..
-00001030: 636f 6e74 6578 7472 3500 0000 7236 0000  contextr5...r6..
-00001040: 0072 4400 0000 723b 0000 0072 3d00 0000  .rD...r;...r=...
-00001050: 723e 0000 0072 3f00 0000 7240 0000 0072  r>...r?...r@...r
-00001060: 4100 0000 7242 0000 0072 3700 0000 723c  A...rB...r7...r<
-00001070: 0000 0072 5200 0000 720f 0000 0072 0f00  ...rR...r....r..
-00001080: 0000 720f 0000 0072 1000 0000 7208 0000  ..r....r....r...
-00001090: 000e 0000 0073 3e00 0000 0802 0401 0401  .....s>.........
-000010a0: 0401 0401 0401 0404 0001 0001 0001 0001  ................
-000010b0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-000010c0: 0001 0a32 0803 0e03 0a03 0c0c 0e03 0a03  ...2............
-000010d0: 0803 0803 0a08 0a0f 7208 0000 0029 0f72  ........r....).r
-000010e0: 2a00 0000 7202 0000 00da 286a 6574 5f62  *...r.....(jet_b
-000010f0: 7269 6467 655f 6261 7365 2e65 7863 6570  ridge_base.excep
-00001100: 7469 6f6e 732e 7265 7175 6573 745f 6572  tions.request_er
-00001110: 726f 7272 0300 0000 da2b 6a65 745f 6272  rorr.....+jet_br
-00001120: 6964 6765 5f62 6173 652e 6578 6365 7074  idge_base.except
-00001130: 696f 6e73 2e76 616c 6964 6174 696f 6e5f  ions.validation_
-00001140: 6572 726f 7272 0400 0000 da03 7369 7872  errorr......sixr
-00001150: 0500 0000 da0f 6a65 745f 6272 6964 6765  ......jet_bridge
-00001160: 5f62 6173 6572 0600 0000 da31 6a65 745f  _baser.....1jet_
-00001170: 6272 6964 6765 5f62 6173 652e 6578 6365  bridge_base.exce
-00001180: 7074 696f 6e73 2e6d 6973 7369 6e67 5f61  ptions.missing_a
-00001190: 7267 756d 656e 745f 6572 726f 7272 0700  rgument_errorr..
-000011a0: 0000 da06 6f62 6a65 6374 7244 0000 0072  ....objectrD...r
-000011b0: 0800 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
-000011c0: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
-000011d0: 653e 0100 0000 7310 0000 0008 010c 020c  e>....s.........
-000011e0: 010c 010c 020c 010c 0206 03              ...........
+00000000: 420d 0d0a 0000 0000 76b0 eb63 3414 0000  B.......v..c4...
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 6a00 0000 6400 6401 6c00  .@...sj...d.d.l.
+00000030: 5a00 6400 6402 6c00 6d01 5a01 0100 6400  Z.d.d.l.m.Z...d.
+00000040: 6403 6c02 6d03 5a03 0100 6400 6404 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6406 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6407 6c0a 6d0b 5a0b 0100 650c 8300 5a0d  d.l.m.Z...e...Z.
+00000080: 4700 6408 6409 8400 6409 650c 8303 5a0e  G.d.d...d.e...Z.
+00000090: 6401 5300 290a e900 0000 004e 2901 da0f  d.S.)......N)...
+000000a0: 4a53 4f4e 4465 636f 6465 4572 726f 7229  JSONDecodeError)
+000000b0: 01da 0c52 6571 7565 7374 4572 726f 7229  ...RequestError)
+000000c0: 01da 0f56 616c 6964 6174 696f 6e45 7272  ...ValidationErr
+000000d0: 6f72 2901 da0c 7374 7269 6e67 5f74 7970  or)...string_typ
+000000e0: 6573 2901 da08 7365 7474 696e 6773 2901  es)...settings).
+000000f0: da14 4d69 7373 696e 6741 7267 756d 656e  ..MissingArgumen
+00000100: 7445 7272 6f72 6300 0000 0000 0000 0000  tErrorc.........
+00000110: 0000 000e 0000 0040 0000 0073 9e00 0000  .......@...s....
+00000120: 6500 5a01 6400 5a02 6401 5a03 6401 5a04  e.Z.d.Z.d.Z.d.Z.
+00000130: 6401 5a05 6401 5a06 6401 5a07 6900 5a08  d.Z.d.Z.d.Z.i.Z.
+00000140: 641b 6402 6403 8401 5a09 6404 6405 8400  d.d.d...Z.d.d...
+00000150: 5a0a 650b 6406 6602 6407 6408 8401 5a0c  Z.e.d.f.d.d...Z.
+00000160: 641c 6409 640a 8401 5a0d 650b 6601 640b  d.d.d...Z.e.f.d.
+00000170: 640c 8401 5a0e 650b 6406 6602 640d 640e  d...Z.e.d.f.d.d.
+00000180: 8401 5a0f 641d 640f 6410 8401 5a10 6411  ..Z.d.d.d...Z.d.
+00000190: 6412 8400 5a11 6413 6414 8400 5a12 641e  d...Z.d.d...Z.d.
+000001a0: 6415 6416 8401 5a13 641f 6417 6418 8401  d.d...Z.d.d.d...
+000001b0: 5a14 6419 641a 8400 5a15 6401 5300 2920  Z.d.d...Z.d.S.) 
+000001c0: da07 5265 7175 6573 744e 630f 0000 0000  ..RequestNc.....
+000001d0: 0000 0014 0000 000a 0000 0003 0000 0073  ...............s
+000001e0: 1c01 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
+000001f0: 7c03 7c00 5f02 7c04 7c00 5f03 7c05 7c00  |.|._.|.|._.|.|.
+00000200: 5f04 7c06 7c00 5f05 7c07 702a 6900 7c00  _.|.|._.|.p*i.|.
+00000210: 5f06 7c08 7034 6900 7c00 5f07 7c09 7c00  _.|.p4i.|._.|.|.
+00000220: 5f08 7c0a 7044 6900 7c00 5f09 7c0b 704e  _.|.pDi.|._.|.pN
+00000230: 6900 7c00 5f0a 7c0c 7c00 5f0b 7c0d 7c00  i.|._.|.|._.|.|.
+00000240: 5f0c 7c0e 7c00 5f0d 7c00 6a07 a00e 6401  _.|.|._.|.j...d.
+00000250: 6402 a102 7d0f 7c0f a00f 6403 a101 72e6  d...}.|...d...r.
+00000260: 7c00 6a08 7d10 7410 7c10 7411 8302 7398  |.j.}.t.|.t...s.
+00000270: 7c10 a012 6404 6405 a102 7d10 7918 7c10  |...d.d...}.y.|.
+00000280: 72a8 7413 a014 7c10 a101 6e02 6900 7c00  r.t...|...n.i.|.
+00000290: 5f15 5700 6e32 0400 7416 6b0a 72e2 0100  _.W.n2..t.k.r...
+000002a0: 7d11 0100 7a14 7417 7c00 6406 a018 7c11  }...z.t.|.d...|.
+000002b0: a101 8302 8201 5700 6400 6400 7d11 7e11  ......W.d.d.}.~.
+000002c0: 5800 5900 6e02 5800 6e32 6407 6408 8400  X.Y.n.X.n2d.d...
+000002d0: 8900 8700 6601 6409 640a 8408 7d12 7419  ....f.d.d...}.t.
+000002e0: 741a 7c12 7c00 6a09 a01b a100 8302 8301  t.|.|.j.........
+000002f0: 7d13 741c 7c13 8301 7c00 5f15 6400 5300  }.t.|...|._.d.S.
+00000300: 290b 4e5a 0c43 4f4e 5445 4e54 5f54 5950  ).NZ.CONTENT_TYP
+00000310: 45da 007a 1061 7070 6c69 6361 7469 6f6e  E..z.application
+00000320: 2f6a 736f 6e7a 0575 7466 2d38 da0d 7375  /jsonz.utf-8..su
+00000330: 7272 6f67 6174 6570 6173 737a 1749 6e63  rrogatepassz.Inc
+00000340: 6f72 7265 6374 204a 534f 4e20 626f 6479  orrect JSON body
+00000350: 3a20 7b7d 6301 0000 0000 0000 0001 0000  : {}c...........
+00000360: 0006 0000 0053 0000 0073 2a00 0000 7400  .....S...s*...t.
+00000370: 7c00 7401 8302 7226 790e 7c00 a002 6401  |.t...r&y.|...d.
+00000380: a101 7d00 5700 6e0c 0100 0100 0100 5900  ..}.W.n.......Y.
+00000390: 6e02 5800 7c00 5300 2902 4e7a 0575 7466  n.X.|.S.).Nz.utf
+000003a0: 2d38 2903 da0a 6973 696e 7374 616e 6365  -8)...isinstance
+000003b0: da05 6279 7465 73da 0664 6563 6f64 6529  ..bytes..decode)
+000003c0: 01da 0576 616c 7565 a900 720f 0000 00fa  ...value..r.....
+000003d0: 5e2f 5573 6572 732f 6631 6e61 6c2f 4472  ^/Users/f1nal/Dr
+000003e0: 6f70 626f 782f 7079 7468 6f6e 2f6a 6574  opbox/python/jet
+000003f0: 2d62 7269 6467 652f 7372 632f 7061 636b  -bridge/src/pack
+00000400: 6167 6573 2f6a 6574 5f62 7269 6467 655f  ages/jet_bridge_
+00000410: 6261 7365 2f6a 6574 5f62 7269 6467 655f  base/jet_bridge_
+00000420: 6261 7365 2f72 6571 7565 7374 2e70 79da  base/request.py.
+00000430: 1362 6f64 795f 6172 6775 6d65 6e74 5f76  .body_argument_v
+00000440: 616c 7565 4300 0000 730c 0000 0000 010a  alueC...s.......
+00000450: 0102 010e 0106 0106 017a 2d52 6571 7565  .........z-Reque
+00000460: 7374 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  st.__init__.<loc
+00000470: 616c 733e 2e62 6f64 795f 6172 6775 6d65  als>.body_argume
+00000480: 6e74 5f76 616c 7565 6301 0000 0000 0000  nt_valuec.......
+00000490: 0003 0000 0004 0000 0013 0000 0073 4e00  .............sN.
+000004a0: 0000 7c00 5c02 7d01 7d02 7400 7401 8800  ..|.\.}.}.t.t...
+000004b0: 7c02 8302 8301 7d02 7402 7c02 8301 6401  |.....}.t.|...d.
+000004c0: 6b04 722a 7c01 7c02 6602 5300 7402 7c02  k.r*|.|.f.S.t.|.
+000004d0: 8301 6401 6b02 7242 7c01 7c02 6402 1900  ..d.k.rB|.|.d...
+000004e0: 6602 5300 7c01 6400 6602 5300 6400 5300  f.S.|.d.f.S.d.S.
+000004f0: 2903 4ee9 0100 0000 7201 0000 0029 03da  ).N.....r....)..
+00000500: 046c 6973 74da 036d 6170 da03 6c65 6e29  .list..map..len)
+00000510: 03da 0469 7465 6dda 036b 6579 da06 7661  ...item..key..va
+00000520: 6c75 6573 2901 7211 0000 0072 0f00 0000  lues).r....r....
+00000530: 7210 0000 00da 086d 6170 5f69 7465 6d4b  r......map_itemK
+00000540: 0000 0073 0e00 0000 0001 0801 0e01 0c01  ...s............
+00000550: 0801 0c01 0c02 7a22 5265 7175 6573 742e  ......z"Request.
+00000560: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00000570: 3e2e 6d61 705f 6974 656d 291d da06 6d65  >.map_item)...me
+00000580: 7468 6f64 da08 7072 6f74 6f63 6f6c da04  thod..protocol..
+00000590: 686f 7374 da04 7061 7468 da0b 7061 7468  host..path..path
+000005a0: 5f6b 7761 7267 73da 0375 7269 da0f 7175  _kwargs..uri..qu
+000005b0: 6572 795f 6172 6775 6d65 6e74 73da 0768  ery_arguments..h
+000005c0: 6561 6465 7273 da04 626f 6479 da0e 626f  eaders..body..bo
+000005d0: 6479 5f61 7267 756d 656e 7473 da05 6669  dy_arguments..fi
+000005e0: 6c65 73da 106f 7269 6769 6e61 6c5f 7265  les..original_re
+000005f0: 7175 6573 74da 106f 7269 6769 6e61 6c5f  quest..original_
+00000600: 6861 6e64 6c65 72da 0661 6374 696f 6eda  handler..action.
+00000610: 0367 6574 da0a 7374 6172 7473 7769 7468  .get..startswith
+00000620: 720b 0000 0072 0500 0000 720d 0000 00da  r....r....r.....
+00000630: 046a 736f 6eda 056c 6f61 6473 da04 6461  .json..loads..da
+00000640: 7461 da0a 5661 6c75 6545 7272 6f72 7203  ta..ValueErrorr.
+00000650: 0000 00da 0666 6f72 6d61 7472 1300 0000  .....formatr....
+00000660: 7214 0000 00da 0569 7465 6d73 da04 6469  r......items..di
+00000670: 6374 2914 da04 7365 6c66 721a 0000 0072  ct)...selfr....r
+00000680: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00000690: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+000006a0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+000006b0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+000006c0: da0c 636f 6e74 656e 745f 7479 7065 722c  ..content_typer,
+000006d0: 0000 00da 0165 7219 0000 00da 0674 7570  .....er......tup
+000006e0: 6c65 7372 0f00 0000 2901 7211 0000 0072  lesr....).r....r
+000006f0: 1000 0000 da08 5f5f 696e 6974 5f5f 1700  ......__init__..
+00000700: 0000 7336 0000 0000 1106 0106 0106 0106  ..s6............
+00000710: 0106 0106 010a 010a 0106 010a 010a 0106  ................
+00000720: 0106 0106 020e 020a 0106 020a 010c 0102  ................
+00000730: 0118 0110 0124 0208 080c 0a14 017a 1052  .....$.......z.R
+00000740: 6571 7565 7374 2e5f 5f69 6e69 745f 5f63  equest.__init__c
+00000750: 0100 0000 0000 0000 0100 0000 0200 0000  ................
+00000760: 4300 0000 7316 0000 007c 006a 0064 0117  C...s....|.j.d..
+00000770: 007c 006a 0117 007c 006a 0217 0053 0029  .|.j...|.j...S.)
+00000780: 024e 7a03 3a2f 2f29 0372 1b00 0000 721c  .Nz.://).r....r.
+00000790: 0000 0072 1f00 0000 2901 7231 0000 0072  ...r....).r1...r
+000007a0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+000007b0: 6675 6c6c 5f75 726c 5800 0000 7302 0000  full_urlX...s...
+000007c0: 0000 017a 1052 6571 7565 7374 2e66 756c  ...z.Request.ful
+000007d0: 6c5f 7572 6c54 6304 0000 0000 0000 0004  l_urlTc.........
+000007e0: 0000 0006 0000 0043 0000 0073 1200 0000  .......C...s....
+000007f0: 7c00 a000 7c01 7c02 7c00 6a01 7c03 a104  |...|.|.|.j.|...
+00000800: 5300 2901 4e29 02da 0d5f 6765 745f 6172  S.).N)..._get_ar
+00000810: 6775 6d65 6e74 7220 0000 0029 0472 3100  gumentr ...).r1.
+00000820: 0000 da04 6e61 6d65 da07 6465 6661 756c  ....name..defaul
+00000830: 74da 0573 7472 6970 720f 0000 0072 0f00  t..stripr....r..
+00000840: 0000 7210 0000 00da 0c67 6574 5f61 7267  ..r......get_arg
+00000850: 756d 656e 745b 0000 0073 0200 0000 0001  ument[...s......
+00000860: 7a14 5265 7175 6573 742e 6765 745f 6172  z.Request.get_ar
+00000870: 6775 6d65 6e74 6303 0000 0000 0000 0003  gumentc.........
+00000880: 0000 0005 0000 0043 0000 0073 1000 0000  .......C...s....
+00000890: 7c00 a000 7c01 7c00 6a01 7c02 a103 5300  |...|.|.j.|...S.
+000008a0: 2901 4e29 02da 0e5f 6765 745f 6172 6775  ).N)..._get_argu
+000008b0: 6d65 6e74 7372 2000 0000 2903 7231 0000  mentsr ...).r1..
+000008c0: 0072 3800 0000 723a 0000 0072 0f00 0000  .r8...r:...r....
+000008d0: 720f 0000 0072 1000 0000 da0d 6765 745f  r....r......get_
+000008e0: 6172 6775 6d65 6e74 735e 0000 0073 0200  arguments^...s..
+000008f0: 0000 0001 7a15 5265 7175 6573 742e 6765  ....z.Request.ge
+00000900: 745f 6172 6775 6d65 6e74 7363 0300 0000  t_argumentsc....
+00000910: 0000 0000 0500 0000 0300 0000 4300 0000  ............C...
+00000920: 733a 0000 007c 00a0 007c 01a1 017d 0374  s:...|...|...}.t
+00000930: 017c 0383 0164 016b 0272 1c7c 027d 046e  .|...d.k.r.|.}.n
+00000940: 1a74 017c 0383 0164 026b 0272 327c 0364  .t.|...d.k.r2|.d
+00000950: 0119 007d 046e 047c 037d 047c 0453 0029  ...}.n.|.}.|.S.)
+00000960: 034e 7201 0000 0072 1200 0000 2902 723d  .Nr....r....).r=
+00000970: 0000 0072 1500 0000 2905 7231 0000 0072  ...r....).r1...r
+00000980: 3800 0000 7239 0000 0072 1800 0000 720e  8...r9...r....r.
+00000990: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000009a0: 0000 da11 6765 745f 6172 6775 6d65 6e74  ....get_argument
+000009b0: 5f73 6166 6561 0000 0073 0e00 0000 0001  _safea...s......
+000009c0: 0a02 0c01 0601 0c01 0a02 0402 7a19 5265  ............z.Re
+000009d0: 7175 6573 742e 6765 745f 6172 6775 6d65  quest.get_argume
+000009e0: 6e74 5f73 6166 6563 0400 0000 0000 0000  nt_safec........
+000009f0: 0400 0000 0600 0000 4300 0000 7312 0000  ........C...s...
+00000a00: 007c 00a0 007c 017c 027c 006a 017c 03a1  .|...|.|.|.j.|..
+00000a10: 0453 0029 014e 2902 7237 0000 0072 2300  .S.).N).r7...r#.
+00000a20: 0000 2904 7231 0000 0072 3800 0000 7239  ..).r1...r8...r9
+00000a30: 0000 0072 3a00 0000 720f 0000 0072 0f00  ...r:...r....r..
+00000a40: 0000 7210 0000 00da 1167 6574 5f62 6f64  ..r......get_bod
+00000a50: 795f 6172 6775 6d65 6e74 6d00 0000 7302  y_argumentm...s.
+00000a60: 0000 0000 017a 1952 6571 7565 7374 2e67  .....z.Request.g
+00000a70: 6574 5f62 6f64 795f 6172 6775 6d65 6e74  et_body_argument
+00000a80: 6303 0000 0000 0000 0003 0000 0005 0000  c...............
+00000a90: 0043 0000 0073 1000 0000 7c00 a000 7c01  .C...s....|...|.
+00000aa0: 7c00 6a01 7c02 a103 5300 2901 4e29 0272  |.j.|...S.).N).r
+00000ab0: 3c00 0000 7223 0000 0029 0372 3100 0000  <...r#...).r1...
+00000ac0: 7238 0000 0072 3a00 0000 720f 0000 0072  r8...r:...r....r
+00000ad0: 0f00 0000 7210 0000 00da 1267 6574 5f62  ....r......get_b
+00000ae0: 6f64 795f 6172 6775 6d65 6e74 7370 0000  ody_argumentsp..
+00000af0: 0073 0200 0000 0001 7a1a 5265 7175 6573  .s......z.Reques
+00000b00: 742e 6765 745f 626f 6479 5f61 7267 756d  t.get_body_argum
+00000b10: 656e 7473 6301 0000 0000 0000 0001 0000  entsc...........
+00000b20: 0003 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
+00000b30: 6a00 a001 6401 a101 5300 2902 4e5a 0958  j...d...S.).NZ.X
+00000b40: 5f52 4541 4c5f 4950 2902 7221 0000 0072  _REAL_IP).r!...r
+00000b50: 2800 0000 2901 7231 0000 0072 0f00 0000  (...).r1...r....
+00000b60: 720f 0000 0072 1000 0000 da06 6765 745f  r....r......get_
+00000b70: 6970 7300 0000 7302 0000 0000 017a 0e52  ips...s......z.R
+00000b80: 6571 7565 7374 2e67 6574 5f69 7063 0100  equest.get_ipc..
+00000b90: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000ba0: 0000 730c 0000 007c 006a 00a0 0164 01a1  ..s....|.j...d..
+00000bb0: 0153 0029 024e 5a0f 585f 5354 4943 4b5f  .S.).NZ.X_STICK_
+00000bc0: 5345 5353 494f 4e29 0272 2100 0000 7228  SESSION).r!...r(
+00000bd0: 0000 0029 0172 3100 0000 720f 0000 0072  ...).r1...r....r
+00000be0: 0f00 0000 7210 0000 00da 1167 6574 5f73  ....r......get_s
+00000bf0: 7469 636b 5f73 6573 7369 6f6e 7600 0000  tick_sessionv...
+00000c00: 7302 0000 0000 017a 1952 6571 7565 7374  s......z.Request
+00000c10: 2e67 6574 5f73 7469 636b 5f73 6573 7369  .get_stick_sessi
+00000c20: 6f6e 6305 0000 0000 0000 0006 0000 0005  onc.............
+00000c30: 0000 0043 0000 0073 3000 0000 7c00 6a00  ...C...s0...|.j.
+00000c40: 7c01 7c03 7c04 6401 8d03 7d05 7c05 7328  |.|.|.d...}.|.s(
+00000c50: 7c02 7401 6b08 7224 7402 7c01 8301 8201  |.t.k.r$t.|.....
+00000c60: 7c02 5300 7c05 6402 1900 5300 2903 4e29  |.S.|.d...S.).N)
+00000c70: 0172 3a00 0000 e9ff ffff ff29 0372 3c00  .r:........).r<.
+00000c80: 0000 da0c 5f41 5247 5f44 4546 4155 4c54  ...._ARG_DEFAULT
+00000c90: 7207 0000 0029 0672 3100 0000 7238 0000  r....).r1...r8..
+00000ca0: 0072 3900 0000 da06 736f 7572 6365 723a  .r9.....sourcer:
+00000cb0: 0000 00da 0461 7267 7372 0f00 0000 720f  .....argsr....r.
+00000cc0: 0000 0072 1000 0000 7237 0000 0079 0000  ...r....r7...y..
+00000cd0: 0073 0c00 0000 0001 1001 0401 0801 0801  .s..............
+00000ce0: 0401 7a15 5265 7175 6573 742e 5f67 6574  ..z.Request._get
+00000cf0: 5f61 7267 756d 656e 7463 0400 0000 0000  _argumentc......
+00000d00: 0000 0600 0000 0400 0000 4300 0000 7348  ..........C...sH
+00000d10: 0000 0067 007d 0478 3e7c 02a0 007c 0167  ...g.}.x>|...|.g
+00000d20: 00a1 0244 005d 2e7d 0574 017c 0574 0283  ...D.].}.t.|.t..
+00000d30: 0272 2a7c 05a0 0364 01a1 017d 057c 0372  .r*|...d...}.|.r
+00000d40: 367c 05a0 04a1 007d 057c 04a0 057c 05a1  6|.....}.|...|..
+00000d50: 0101 0071 1257 007c 0453 0029 024e 7a05  ...q.W.|.S.).Nz.
+00000d60: 7574 662d 3829 0672 2800 0000 720b 0000  utf-8).r(...r...
+00000d70: 0072 0c00 0000 720d 0000 0072 3a00 0000  .r....r....r:...
+00000d80: da06 6170 7065 6e64 2906 7231 0000 0072  ..append).r1...r
+00000d90: 3800 0000 7245 0000 0072 3a00 0000 7218  8...rE...r:...r.
+00000da0: 0000 00da 0176 720f 0000 0072 0f00 0000  .....vr....r....
+00000db0: 7210 0000 0072 3c00 0000 8100 0000 7310  r....r<.......s.
+00000dc0: 0000 0000 0104 0112 010a 010a 0604 0108  ................
+00000dd0: 010e 017a 1652 6571 7565 7374 2e5f 6765  ...z.Request._ge
+00000de0: 745f 6172 6775 6d65 6e74 7363 0100 0000  t_argumentsc....
+00000df0: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
+00000e00: 7374 0000 007c 006a 0072 0c7c 006a 0053  st...|.j.r.|.j.S
+00000e10: 007c 006a 01a0 0264 01a1 017d 017c 0173  .|.j...d...}.|.s
+00000e20: 2064 0053 0064 0264 036c 036d 047d 0201   d.S.d.d.l.m.}..
+00000e30: 0079 2e74 056a 06a0 0764 0464 05a1 02a0  .y.t.j...d.d....
+00000e40: 08a1 007d 037c 027c 017c 0383 027d 0474  ...}.|.|.|...}.t
+00000e50: 09a0 0a7c 04a1 017c 005f 007c 006a 0053  ...|...|._.|.j.S
+00000e60: 0004 0074 0b6b 0a72 6e01 0001 0001 0064  ...t.k.rn......d
+00000e70: 0053 0058 0064 0053 0029 064e 5a11 585f  .S.X.d.S.).NZ.X_
+00000e80: 4252 4944 4745 5f53 4554 5449 4e47 5372  BRIDGE_SETTINGSr
+00000e90: 0100 0000 2901 da07 6465 6372 7970 74da  ....)...decrypt.
+00000ea0: 012d 7209 0000 0029 0cda 0f62 7269 6467  .-r....)...bridg
+00000eb0: 655f 7365 7474 696e 6773 7221 0000 0072  e_settingsr!...r
+00000ec0: 2800 0000 da1b 6a65 745f 6272 6964 6765  (.....jet_bridge
+00000ed0: 5f62 6173 652e 7574 696c 732e 6372 7970  _base.utils.cryp
+00000ee0: 7472 4900 0000 7206 0000 00da 0554 4f4b  trI...r......TOK
+00000ef0: 454e da07 7265 706c 6163 65da 056c 6f77  EN..replace..low
+00000f00: 6572 722a 0000 0072 2b00 0000 da09 4578  err*...r+.....Ex
+00000f10: 6365 7074 696f 6e29 0572 3100 0000 5a17  ception).r1...Z.
+00000f20: 6272 6964 6765 5f73 6574 7469 6e67 735f  bridge_settings_
+00000f30: 656e 636f 6465 6472 4900 0000 da0a 7365  encodedrI.....se
+00000f40: 6372 6574 5f6b 6579 5a09 6465 6372 7970  cret_keyZ.decryp
+00000f50: 7465 6472 0f00 0000 720f 0000 0072 1000  tedr....r....r..
+00000f60: 0000 da13 6765 745f 6272 6964 6765 5f73  ....get_bridge_s
+00000f70: 6574 7469 6e67 7390 0000 0073 1a00 0000  ettings....s....
+00000f80: 0001 0601 0602 0c02 0401 0402 0c02 0201  ................
+00000f90: 1201 0a01 0c01 0601 0e01 7a1b 5265 7175  ..........z.Requ
+00000fa0: 6573 742e 6765 745f 6272 6964 6765 5f73  est.get_bridge_s
+00000fb0: 6574 7469 6e67 7329 0e4e 4e4e 4e4e 4e4e  ettings).NNNNNNN
+00000fc0: 4e4e 4e4e 4e4e 4e29 0154 2901 5429 0154  NNNNNNN).T).T).T
+00000fd0: 2901 5429 16da 085f 5f6e 616d 655f 5fda  ).T)...__name__.
+00000fe0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000ff0: 7561 6c6e 616d 655f 5fda 0773 6573 7369  ualname__..sessi
+00001000: 6f6e 724b 0000 00da 0770 726f 6a65 6374  onrK.....project
+00001010: da0b 656e 7669 726f 6e6d 656e 74da 0e72  ..environment..r
+00001020: 6573 6f75 7263 655f 746f 6b65 6eda 0763  esource_token..c
+00001030: 6f6e 7465 7874 7235 0000 0072 3600 0000  ontextr5...r6...
+00001040: 7244 0000 0072 3b00 0000 723d 0000 0072  rD...r;...r=...r
+00001050: 3e00 0000 723f 0000 0072 4000 0000 7241  >...r?...r@...rA
+00001060: 0000 0072 4200 0000 7237 0000 0072 3c00  ...rB...r7...r<.
+00001070: 0000 7252 0000 0072 0f00 0000 720f 0000  ..rR...r....r...
+00001080: 0072 0f00 0000 7210 0000 0072 0800 0000  .r....r....r....
+00001090: 0e00 0000 733e 0000 0008 0204 0104 0104  ....s>..........
+000010a0: 0104 0104 0104 0400 0100 0100 0100 0100  ................
+000010b0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+000010c0: 010a 3208 030e 030a 030c 0c0e 030a 0308  ..2.............
+000010d0: 0308 030a 080a 0f72 0800 0000 290f 722a  .......r....).r*
+000010e0: 0000 0072 0200 0000 da28 6a65 745f 6272  ...r.....(jet_br
+000010f0: 6964 6765 5f62 6173 652e 6578 6365 7074  idge_base.except
+00001100: 696f 6e73 2e72 6571 7565 7374 5f65 7272  ions.request_err
+00001110: 6f72 7203 0000 00da 2b6a 6574 5f62 7269  orr.....+jet_bri
+00001120: 6467 655f 6261 7365 2e65 7863 6570 7469  dge_base.excepti
+00001130: 6f6e 732e 7661 6c69 6461 7469 6f6e 5f65  ons.validation_e
+00001140: 7272 6f72 7204 0000 00da 0373 6978 7205  rrorr......sixr.
+00001150: 0000 00da 0f6a 6574 5f62 7269 6467 655f  .....jet_bridge_
+00001160: 6261 7365 7206 0000 00da 316a 6574 5f62  baser.....1jet_b
+00001170: 7269 6467 655f 6261 7365 2e65 7863 6570  ridge_base.excep
+00001180: 7469 6f6e 732e 6d69 7373 696e 675f 6172  tions.missing_ar
+00001190: 6775 6d65 6e74 5f65 7272 6f72 7207 0000  gument_errorr...
+000011a0: 00da 066f 626a 6563 7472 4400 0000 7208  ...objectrD...r.
+000011b0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+000011c0: 0000 7210 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000011d0: 3e01 0000 0073 1000 0000 0801 0c02 0c01  >....s..........
+000011e0: 0c01 0c02 0c01 0c02 0603                 ..........
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/store.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/store.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/db.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/db.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,867 +1,935 @@
-00000000: 330d 0d0a b0a4 0164 5f4c 0000 e300 0000  3......d_L......
+00000000: 330d 0d0a 35c1 c264 c653 0000 e300 0000  3...5..d.S......
 00000010: 0000 0000 0000 0000 000b 0000 0040 0000  .............@..
-00000020: 0073 1802 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
+00000020: 0073 2802 0000 6400 6401 6c00 5a00 6400  .s(...d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6403 6c07 6d08 5a08 0100 6400 6404 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6406 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
 00000090: 6407 6c0f 6d10 5a10 0100 6400 6408 6c11  d.l.m.Z...d.d.l.
 000000a0: 6d12 5a12 0100 6400 6409 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-000000b0: 6d15 5a15 0100 6400 640a 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000c0: 6d18 5a18 0100 6400 640b 6c19 6d1a 5a1a  m.Z...d.d.l.m.Z.
-000000d0: 6d1b 5a1b 0100 6400 640c 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000e0: 6d1e 5a1e 0100 7910 6400 640d 6c1f 6d20  m.Z...y.d.d.l.m 
-000000f0: 5a20 0100 5700 6e14 0400 6521 6b0a 72e4  Z ..W.n...e!k.r.
-00000100: 0100 0100 0100 5900 6e02 5800 6400 640e  ......Y.n.X.d.d.
-00000110: 6c22 6d23 5a23 0100 6400 640f 6c24 6d25  l"m#Z#..d.d.l$m%
-00000120: 5a25 0100 6900 6126 6900 6127 6410 6411  Z%..i.a&i.a'd.d.
-00000130: 8400 5a28 6451 6412 6413 8401 5a29 6414  ..Z(dQd.d...Z)d.
-00000140: 6415 8400 5a2a 6416 6417 8400 5a2b 6418  d...Z*d.d...Z+d.
-00000150: 6419 8400 5a2c 641a 641b 8400 5a2d 641c  d...Z,d.d...Z-d.
-00000160: 641d 8400 5a2e 641e 641f 8400 5a2f 6420  d...Z.d.d...Z/d 
-00000170: 6421 8400 5a30 6422 6423 8400 5a31 6424  d!..Z0d"d#..Z1d$
-00000180: 6425 8400 5a32 6426 6427 8400 5a33 6428  d%..Z2d&d'..Z3d(
-00000190: 6429 8400 5a34 642a 642b 8400 5a35 642c  d)..Z4d*d+..Z5d,
-000001a0: 642d 8400 5a36 642e 642f 8400 5a37 6430  d-..Z6d.d/..Z7d0
-000001b0: 6431 8400 5a38 6432 6433 8400 5a39 6434  d1..Z8d2d3..Z9d4
-000001c0: 6435 8400 5a3a 6436 6437 8400 5a3b 6438  d5..Z:d6d7..Z;d8
-000001d0: 6439 8400 5a3c 643a 643b 8400 5a3d 643c  d9..Z<d:d;..Z=d<
-000001e0: 643d 8400 5a3e 643e 643f 8400 5a3f 6440  d=..Z>d>d?..Z?d@
-000001f0: 6441 8400 5a40 6501 6a41 6442 6443 8400  dA..Z@e.jAdBdC..
-00000200: 8301 5a42 6452 6444 6445 8401 5a43 6446  ..ZBdRdDdE..ZCdF
-00000210: 6447 8400 5a44 6448 6449 8400 5a45 6453  dG..ZDdHdI..ZEdS
-00000220: 644a 644b 8401 5a46 644c 644d 8400 5a47  dJdK..ZFdLdM..ZG
-00000230: 6454 644f 6450 8401 5a48 6401 5300 2955  dTdOdP..ZHd.S.)U
-00000240: e900 0000 004e 2902 da09 7469 6d65 6465  .....N)...timede
-00000250: 6c74 61da 0864 6174 6574 696d 6529 01da  lta..datetime)..
-00000260: 0772 6566 6c65 6374 2901 da09 5353 4854  .reflect)...SSHT
-00000270: 756e 6e65 6c29 01da 0f67 6574 5f73 6861  unnel)...get_sha
-00000280: 3235 365f 6861 7368 2901 da1b 6665 7463  256_hash)...fetc
-00000290: 685f 7479 7065 5f63 6f64 655f 746f 5f73  h_type_code_to_s
-000002a0: 716c 5f74 7970 6529 01da 0853 7472 696e  ql_type)...Strin
-000002b0: 6749 4f29 01da 0a71 756f 7465 5f70 6c75  gIO)...quote_plu
-000002c0: 7329 02da 0d63 7265 6174 655f 656e 6769  s)...create_engi
-000002d0: 6e65 da08 4d65 7461 4461 7461 2902 da0c  ne..MetaData)...
-000002e0: 6175 746f 6d61 705f 6261 7365 da15 6765  automap_base..ge
-000002f0: 6e65 7261 7465 5f72 656c 6174 696f 6e73  nerate_relations
-00000300: 6869 7029 02da 0c73 6573 7369 6f6e 6d61  hip)...sessionma
-00000310: 6b65 72da 0e73 636f 7065 645f 7365 7373  ker..scoped_sess
-00000320: 696f 6e29 02da 1167 6574 5f72 616e 646f  ion)...get_rando
-00000330: 6d5f 7374 7269 6e67 da05 6d65 7267 6529  m_string..merge)
-00000340: 01da 0574 7970 6573 2901 da08 7365 7474  ...types)...sett
-00000350: 696e 6773 2901 da06 6c6f 6767 6572 6301  ings)...loggerc.
-00000360: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000370: 0000 0073 0800 0000 7400 7c00 8301 5300  ...s....t.|...S.
-00000380: 2901 4e29 0172 0900 0000 2901 da05 7661  ).N).r....)...va
-00000390: 6c75 65a9 0072 1600 0000 fa59 2f55 7365  lue..r.....Y/Use
-000003a0: 7273 2f66 316e 616c 2f44 726f 7062 6f78  rs/f1nal/Dropbox
-000003b0: 2f70 7974 686f 6e2f 6a65 742d 6272 6964  /python/jet-brid
-000003c0: 6765 2f73 7263 2f70 6163 6b61 6765 732f  ge/src/packages/
-000003d0: 6a65 745f 6272 6964 6765 5f62 6173 652f  jet_bridge_base/
-000003e0: 6a65 745f 6272 6964 6765 5f62 6173 652f  jet_bridge_base/
-000003f0: 6462 2e70 79da 0a75 726c 5f65 6e63 6f64  db.py..url_encod
-00000400: 6521 0000 0073 0200 0000 0001 7218 0000  e!...s......r...
-00000410: 0063 0200 0000 0000 0000 0500 0000 0a00  .c..............
-00000420: 0000 4300 0000 7316 0300 007c 006a 0064  ..C...s....|.j.d
-00000430: 0183 010c 0073 187c 006a 0064 0283 010c  .....s.|.j.d....
-00000440: 0072 1c64 0053 0074 017c 006a 0064 0183  .r.d.S.t.|.j.d..
-00000450: 0183 0164 0367 027d 027c 006a 0064 0183  ...d.g.}.|.j.d..
-00000460: 0164 046b 0272 867c 026a 0264 0583 0101  .d.k.r.|.j.d....
-00000470: 007c 026a 0274 017c 006a 0064 0283 0183  .|.j.t.|.j.d....
-00000480: 0183 0101 007c 006a 0064 0683 0172 827c  .....|.j.d...r.|
-00000490: 026a 0264 0783 0101 007c 026a 0274 017c  .j.d.....|.j.t.|
-000004a0: 006a 0064 0683 0183 0183 0101 0090 026e  .j.d...........n
-000004b0: 867c 006a 0064 0183 0164 086b 0290 0172  .|.j.d...d.k...r
-000004c0: 0e7c 026a 0274 017c 006a 0064 0283 0183  .|.j.t.|.j.d....
-000004d0: 0183 0101 0079 5274 036a 047c 006a 0064  .....yRt.j.|.j.d
-000004e0: 0983 0183 0101 007c 026a 0264 0a6a 057c  .......|.j.d.j.|
-000004f0: 006a 0064 0983 0183 0183 0101 007c 006a  .j.d.........|.j
-00000500: 0064 0683 0172 fa7c 026a 0264 0b83 0101  .d...r.|.j.d....
-00000510: 007c 026a 0274 017c 006a 0064 0683 0183  .|.j.t.|.j.d....
-00000520: 0183 0101 0057 006e 0c01 0001 0001 0059  .....W.n.......Y
-00000530: 006e 0258 0090 016e fe7c 006a 0064 0183  .n.X...n.|.j.d..
-00000540: 0164 0c6b 0290 0172 ce7c 026a 0274 0674  .d.k...r.|.j.t.t
-00000550: 017c 006a 0064 0d83 0183 0183 0183 0101  .|.j.d..........
-00000560: 007c 006a 0064 0983 0190 0172 647c 026a  .|.j.d.....rd|.j
-00000570: 0264 0e83 0101 007c 026a 0274 0674 017c  .d.....|.j.t.t.|
-00000580: 006a 0064 0983 0183 0183 0183 0101 007c  .j.d...........|
-00000590: 026a 0264 0f83 0101 007c 026a 0274 017c  .j.d.....|.j.t.|
-000005a0: 006a 0064 1083 0183 0183 0101 007c 026a  .j.d.........|.j
-000005b0: 0264 0583 0101 007c 026a 0274 017c 006a  .d.....|.j.t.|.j
-000005c0: 0064 0283 0183 0183 0101 007c 006a 0064  .d.........|.j.d
-000005d0: 0683 0190 0372 0c7c 026a 0264 0783 0101  .....r.|.j.d....
-000005e0: 007c 026a 0274 017c 006a 0064 0683 0183  .|.j.t.|.j.d....
-000005f0: 0183 0101 0090 016e 3e7c 0190 0172 d864  .......n>|...r.d
-00000600: 116e 087c 006a 0064 1083 017d 037c 0190  .n.|.j.d...}.|..
-00000610: 0172 ee7c 016a 076e 087c 006a 0064 1283  .r.|.j.n.|.j.d..
-00000620: 017d 047c 006a 0064 0d83 0190 0272 5a7c  .}.|.j.d.....rZ|
-00000630: 026a 0274 0674 017c 006a 0064 0d83 0183  .j.t.t.|.j.d....
-00000640: 0183 0183 0101 007c 006a 0064 0983 0190  .......|.j.d....
-00000650: 0272 4a7c 026a 0264 0e83 0101 007c 026a  .rJ|.j.d.....|.j
-00000660: 0274 0674 017c 006a 0064 0983 0183 0183  .t.t.|.j.d......
-00000670: 0183 0101 007c 0390 0272 5a7c 026a 0264  .....|...rZ|.j.d
-00000680: 0f83 0101 007c 0390 0272 967c 026a 0274  .....|...r.|.j.t
-00000690: 017c 0383 0183 0101 007c 0490 0272 8c7c  .|.......|...r.|
-000006a0: 026a 0264 0e83 0101 007c 026a 0274 017c  .j.d.....|.j.t.|
-000006b0: 0483 0183 0101 007c 026a 0264 0583 0101  .......|.j.d....
-000006c0: 007c 026a 0274 017c 006a 0064 0283 0183  .|.j.t.|.j.d....
-000006d0: 0183 0101 007c 006a 0064 0683 0190 0272  .....|.j.d.....r
-000006e0: d67c 026a 0264 0783 0101 007c 026a 0274  .|.j.d.....|.j.t
-000006f0: 017c 006a 0064 0683 0183 0183 0101 006e  .|.j.d.........n
-00000700: 367c 006a 0064 0183 0164 136b 0290 0272  6|.j.d...d.k...r
-00000710: f27c 026a 0264 1483 0101 006e 1a7c 006a  .|.j.d.....n.|.j
-00000720: 0064 0183 0164 156b 0290 0372 0c7c 026a  .d...d.k...r.|.j
-00000730: 0264 1683 0101 0064 176a 087c 0283 0153  .d.....d.j.|...S
-00000740: 0029 184e da06 656e 6769 6e65 da04 6e61  .).N..engine..na
-00000750: 6d65 7a03 3a2f 2fda 0673 716c 6974 65fa  mez.://..sqlite.
-00000760: 012f da05 6578 7472 61fa 013f da08 6269  ./..extra..?..bi
-00000770: 6771 7565 7279 da08 7061 7373 776f 7264  gquery..password
-00000780: 7a16 3f63 7265 6465 6e74 6961 6c73 5f62  z.?credentials_b
-00000790: 6173 6536 343d 7b7d fa01 26da 0973 6e6f  ase64={}..&..sno
-000007a0: 7766 6c61 6b65 da04 7573 6572 fa01 3afa  wflake..user..:.
-000007b0: 0140 da04 686f 7374 7a09 3132 372e 302e  .@..hostz.127.0.
-000007c0: 302e 31da 0470 6f72 745a 056d 7973 716c  0.1..portZ.mysql
-000007d0: 7a0d 3f63 6861 7273 6574 3d75 7466 387a  z.?charset=utf8z
-000007e0: 0c6d 7373 716c 2b70 796f 6462 637a 0f3f  .mssql+pyodbcz.?
-000007f0: 6472 6976 6572 3d46 7265 6554 4453 da00  driver=FreeTDS..
-00000800: 2909 da03 6765 74da 0373 7472 da06 6170  )...get..str..ap
-00000810: 7065 6e64 da06 6261 7365 3634 da09 6236  pend..base64..b6
-00000820: 3464 6563 6f64 65da 0666 6f72 6d61 7472  4decode..formatr
-00000830: 1800 0000 da0f 6c6f 6361 6c5f 6269 6e64  ......local_bind
-00000840: 5f70 6f72 74da 046a 6f69 6e29 05da 0463  _port..join)...c
-00000850: 6f6e 66da 0674 756e 6e65 6cda 0375 726c  onf..tunnel..url
-00000860: 7226 0000 0072 2700 0000 7216 0000 0072  r&...r'...r....r
-00000870: 1600 0000 7217 0000 00da 1062 7569 6c64  ....r......build
-00000880: 5f65 6e67 696e 655f 7572 6c25 0000 0073  _engine_url%...s
-00000890: 7000 0000 0001 1801 0403 0c01 0603 0e01  p...............
-000008a0: 0a01 1402 0a01 0a01 1801 1001 1402 0201  ................
-000008b0: 1001 1602 0a01 0a01 1801 0601 0a01 1001  ................
-000008c0: 1802 0c01 0a01 1802 0a02 1401 0a02 1402  ................
-000008d0: 0c01 0a01 1802 1401 1602 0c01 1802 0c01  ................
-000008e0: 0a01 1802 0601 0a02 0601 0e02 0601 0a01  ................
-000008f0: 0e02 0a02 1402 0c01 0a01 1601 1001 0c01  ................
-00000900: 1001 0a02 7234 0000 0063 0100 0000 0000  ....r4...c......
-00000910: 0000 0100 0000 1000 0000 4300 0000 7376  ..........C...sv
-00000920: 0000 0074 0074 016a 027c 006a 0364 0183  ...t.t.j.|.j.d..
-00000930: 017c 006a 0364 0283 017c 006a 0364 0383  .|.j.d...|.j.d..
-00000940: 017c 006a 0364 0483 017c 006a 0364 0583  .|.j.d...|.j.d..
-00000950: 017c 006a 0364 0683 017c 006a 0364 0783  .|.j.d...|.j.d..
-00000960: 017c 006a 0364 0883 017c 006a 0364 0983  .|.j.d...|.j.d..
-00000970: 017c 006a 0364 0a83 017c 006a 0364 0b83  .|.j.d...|.j.d..
-00000980: 017c 006a 0364 0c83 017c 006a 0364 0d83  .|.j.d...|.j.d..
-00000990: 0167 0d83 0183 0153 0029 0e4e 7219 0000  .g.....S.).Nr...
-000009a0: 0072 2600 0000 7227 0000 0072 1a00 0000  .r&...r'...r....
-000009b0: 7223 0000 0072 2000 0000 da04 6f6e 6c79  r#...r .....only
-000009c0: da06 6578 6365 7074 da06 7363 6865 6d61  ..except..schema
-000009d0: da08 7373 685f 686f 7374 da08 7373 685f  ..ssh_host..ssh_
-000009e0: 706f 7274 da08 7373 685f 7573 6572 da0f  port..ssh_user..
-000009f0: 7373 685f 7072 6976 6174 655f 6b65 7929  ssh_private_key)
-00000a00: 0472 0600 0000 da04 6a73 6f6e da05 6475  .r......json..du
-00000a10: 6d70 7372 2900 0000 2901 7231 0000 0072  mpsr)...).r1...r
-00000a20: 1600 0000 7216 0000 0072 1700 0000 da11  ....r....r......
-00000a30: 6765 745f 636f 6e6e 6563 7469 6f6e 5f69  get_connection_i
-00000a40: 6476 0000 0073 1c00 0000 0001 0601 0801  dv...s..........
-00000a50: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00000a60: 0801 0801 0801 723e 0000 0063 0100 0000  ......r>...c....
-00000a70: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000a80: 731a 0000 0074 006a 017c 006a 0264 0183  s....t.j.|.j.d..
-00000a90: 017c 006a 0264 0283 0167 0283 0153 0029  .|.j.d...g...S.)
-00000aa0: 034e 721d 0000 00da 0b63 6f6e 6e65 6374  .Nr......connect
-00000ab0: 696f 6e73 2903 723c 0000 0072 3d00 0000  ions).r<...r=...
-00000ac0: 7229 0000 0029 0172 3100 0000 7216 0000  r)...).r1...r...
-00000ad0: 0072 1600 0000 7217 0000 00da 1867 6574  .r....r......get
-00000ae0: 5f63 6f6e 6e65 6374 696f 6e5f 7061 7261  _connection_para
-00000af0: 6d73 5f69 6488 0000 0073 0600 0000 0001  ms_id....s......
-00000b00: 0401 0801 7240 0000 0063 0100 0000 0000  ....r@...c......
-00000b10: 0000 0100 0000 0700 0000 0300 0000 731e  ..............s.
-00000b20: 0000 0074 0074 0187 0066 0164 0164 0284  ...t.t...f.d.d..
-00000b30: 0864 0364 0464 0564 0667 0483 0283 0153  .d.d.d.d.g.....S
-00000b40: 0029 074e 6301 0000 0000 0000 0001 0000  .).Nc...........
-00000b50: 0002 0000 0013 0000 0073 0a00 0000 8800  .........s......
-00000b60: 6a00 7c00 8301 5300 2901 4e29 0172 2900  j.|...S.).N).r).
-00000b70: 0000 2901 da01 7829 0172 3100 0000 7216  ..)...x).r1...r.
-00000b80: 0000 0072 1700 0000 da08 3c6c 616d 6264  ...r......<lambd
-00000b90: 613e 9000 0000 7300 0000 007a 2669 735f  a>....s....z&is_
-00000ba0: 7475 6e6e 656c 5f63 6f6e 6e65 6374 696f  tunnel_connectio
-00000bb0: 6e2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  n.<locals>.<lamb
-00000bc0: 6461 3e72 3800 0000 7239 0000 0072 3a00  da>r8...r9...r:.
-00000bd0: 0000 723b 0000 0029 02da 0361 6c6c da03  ..r;...)...all..
-00000be0: 6d61 7029 0172 3100 0000 7216 0000 0029  map).r1...r....)
-00000bf0: 0172 3100 0000 7217 0000 00da 1469 735f  .r1...r......is_
-00000c00: 7475 6e6e 656c 5f63 6f6e 6e65 6374 696f  tunnel_connectio
-00000c10: 6e8f 0000 0073 0200 0000 0001 7245 0000  n....s......rE..
-00000c20: 0063 0100 0000 0000 0000 0400 0000 0a00  .c..............
-00000c30: 0000 0300 0000 73a0 0000 0074 0088 0083  ......s....t....
-00000c40: 0173 0c64 0053 0074 0188 0083 017d 0174  .s.d.S.t.....}.t
-00000c50: 0288 007c 0183 0289 0174 036a 0464 016a  ...|.....t.j.d.j
-00000c60: 0588 0183 0183 0101 0087 0087 0166 0264  .............f.d
-00000c70: 0264 0384 087d 0274 0688 0188 006a 0764  .d...}.t.....j.d
-00000c80: 0483 0188 006a 0764 0583 0188 006a 0764  .....j.d.....j.d
-00000c90: 0683 0188 006a 0764 0783 016a 0864 0864  .....j.d...j.d.d
-00000ca0: 0983 0288 006a 0764 0a83 0188 006a 0764  .....j.d.....j.d
-00000cb0: 0b83 017c 0264 0c8d 087d 037c 036a 0983  ...|.d...}.|.j..
-00000cc0: 0001 0074 036a 0464 0d6a 057c 036a 0a88  ...t.j.d.j.|.j..
-00000cd0: 0183 0283 0101 007c 0353 0029 0e4e 7a2a  .......|.S.).Nz*
-00000ce0: 5374 6172 7469 6e67 2053 5348 2074 756e  Starting SSH tun
-00000cf0: 6e65 6c20 666f 7220 636f 6e6e 6563 7469  nel for connecti
-00000d00: 6f6e 2022 7b7d 222e 2e2e 6300 0000 0000  on "{}"...c.....
-00000d10: 0000 0002 0000 0003 0000 0013 0000 0073  ...............s
-00000d20: 4400 0000 7400 8800 8301 7d00 7401 6a02  D...t.....}.t.j.
-00000d30: 7c00 8301 7d01 7c01 7230 7403 6a04 6401  |...}.|.r0t.j.d.
-00000d40: 6a05 8801 8301 8301 0100 7406 8800 8301  j.........t.....
-00000d50: 0100 6e10 7403 6a04 6402 6a05 8801 8301  ..n.t.j.d.j.....
-00000d60: 8301 0100 6400 5300 2903 4e7a 2f53 5348  ....d.S.).Nz/SSH
-00000d70: 2074 756e 6e65 6c20 6973 2063 6c6f 7365   tunnel is close
-00000d80: 642c 2064 6973 706f 7369 6e67 2063 6f6e  d, disposing con
-00000d90: 6e65 6374 696f 6e20 227b 7d22 7a28 5353  nection "{}"z(SS
-00000da0: 4820 7475 6e6e 656c 2069 7320 636c 6f73  H tunnel is clos
-00000db0: 6564 2066 6f72 2063 6f6e 6e65 6374 696f  ed for connectio
-00000dc0: 6e20 227b 7d22 2907 723e 0000 0072 3f00  n "{}").r>...r?.
-00000dd0: 0000 7229 0000 0072 1400 0000 da04 696e  ..r)...r......in
-00000de0: 666f 722e 0000 00da 1264 6973 706f 7365  for......dispose
-00000df0: 5f63 6f6e 6e65 6374 696f 6e29 02da 0d63  _connection)...c
-00000e00: 6f6e 6e65 6374 696f 6e5f 6964 da0a 636f  onnection_id..co
-00000e10: 6e6e 6563 7469 6f6e 2902 7231 0000 00da  nnection).r1....
-00000e20: 0f63 6f6e 6e65 6374 696f 6e5f 6e61 6d65  .connection_name
-00000e30: 7216 0000 0072 1700 0000 da08 6f6e 5f63  r....r......on_c
-00000e40: 6c6f 7365 c500 0000 730c 0000 0000 0108  lose....s.......
-00000e50: 010a 0204 0110 010a 027a 2767 6574 5f63  .........z'get_c
-00000e60: 6f6e 6e65 6374 696f 6e5f 7475 6e6e 656c  onnection_tunnel
-00000e70: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c6f  .<locals>.on_clo
-00000e80: 7365 7238 0000 0072 3900 0000 723a 0000  ser8...r9...r:..
-00000e90: 0072 3b00 0000 7a02 5c6e da01 0a72 2600  .r;...z.\n...r&.
-00000ea0: 0000 7227 0000 0029 0872 1a00 0000 7238  ..r'...).r....r8
-00000eb0: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
-00000ec0: 0000 5a0b 7265 6d6f 7465 5f68 6f73 745a  ..Z.remote_hostZ
-00000ed0: 0b72 656d 6f74 655f 706f 7274 724b 0000  .remote_portrK..
-00000ee0: 007a 3153 5348 2074 756e 6e65 6c20 7374  .z1SSH tunnel st
-00000ef0: 6172 7465 6420 6f6e 2070 6f72 7420 7b7d  arted on port {}
-00000f00: 2066 6f72 2063 6f6e 6e65 6374 696f 6e20   for connection 
-00000f10: 227b 7d22 290b 7245 0000 00da 1567 6574  "{}").rE.....get
-00000f20: 5f63 6f6e 6e65 6374 696f 6e5f 7363 6865  _connection_sche
-00000f30: 6d61 da13 6765 745f 636f 6e6e 6563 7469  ma..get_connecti
-00000f40: 6f6e 5f6e 616d 6572 1400 0000 7246 0000  on_namer....rF..
-00000f50: 0072 2e00 0000 7205 0000 0072 2900 0000  .r....r....r)...
-00000f60: da07 7265 706c 6163 65da 0573 7461 7274  ..replace..start
-00000f70: 722f 0000 0029 0472 3100 0000 7237 0000  r/...).r1...r7..
-00000f80: 0072 4b00 0000 7232 0000 0072 1600 0000  .rK...r2...r....
-00000f90: 2902 7231 0000 0072 4a00 0000 7217 0000  ).r1...rJ...r...
-00000fa0: 00da 1567 6574 5f63 6f6e 6e65 6374 696f  ...get_connectio
-00000fb0: 6e5f 7475 6e6e 656c 9300 0000 7324 0000  n_tunnel....s$..
-00000fc0: 0000 0108 0104 0208 010a 2b10 020e 0a02  ..........+.....
-00000fd0: 0102 0108 0108 0108 0110 0108 0108 0108  ................
-00000fe0: 0208 0214 0272 5100 0000 6301 0000 0000  .....rQ...c.....
-00000ff0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00001000: 4600 0000 7c00 6a00 6401 8301 7222 7c00  F...|.j.d...r"|.
-00001010: 6a00 6401 8301 6402 6b03 7222 7c00 6a00  j.d...d.k.r"|.j.
-00001020: 6401 8301 6e02 6400 7d01 7c01 0c00 7242  d...n.d.}.|...rB
-00001030: 7c00 6a00 6403 6402 8302 6a01 6404 8301  |.j.d.d...j.d...
-00001040: 7242 6405 7d01 7c01 5300 2906 4e72 3700  rBd.}.|.S.).Nr7.
-00001050: 0000 7228 0000 0072 1900 0000 5a05 6d73  ..r(...r....Z.ms
-00001060: 7371 6c5a 0364 626f 2902 7229 0000 00da  sqlZ.dbo).r)....
-00001070: 0a73 7461 7274 7377 6974 6829 0272 3100  .startswith).r1.
-00001080: 0000 7237 0000 0072 1600 0000 7216 0000  ..r7...r....r...
-00001090: 0072 1700 0000 724d 0000 00e0 0000 0073  .r....rM.......s
-000010a0: 0800 0000 0001 2602 1801 0402 724d 0000  ......&.....rM..
-000010b0: 0063 0200 0000 0000 0000 0500 0000 0600  .c..............
-000010c0: 0000 4300 0000 7372 0000 0064 017d 0274  ..C...sr...d.}.t
-000010d0: 0074 0069 007c 0083 0264 027c 0269 0183  .t.i.|...d.|.i..
-000010e0: 027d 0374 017c 0383 017d 047c 0472 307c  .}.t.|...}.|.r0|
-000010f0: 046a 027c 0264 0383 027d 047c 0172 427c  .j.|.d...}.|.rB|
-00001100: 0464 046a 037c 0183 0137 007d 0474 047c  .d.j.|...7.}.t.|
-00001110: 0083 0172 6e7c 0464 056a 037c 006a 0564  ...rn|.d.j.|.j.d
-00001120: 0683 017c 006a 0564 0783 017c 006a 0564  ...|.j.d...|.j.d
-00001130: 0883 0183 0337 007d 047c 0453 0029 094e  .....7.}.|.S.).N
-00001140: 5a0f 5f5f 4a45 545f 4442 5f50 4153 535f  Z.__JET_DB_PASS_
-00001150: 5f72 2000 0000 7a08 2a2a 2a2a 2a2a 2a2a  _r ...z.********
-00001160: 7a03 3a7b 7d7a 0f20 2876 6961 207b 7d40  z.:{}z. (via {}@
-00001170: 7b7d 3a7b 7d29 723a 0000 0072 3800 0000  {}:{})r:...r8...
-00001180: 7239 0000 0029 0672 1100 0000 7234 0000  r9...).r....r4..
-00001190: 0072 4f00 0000 722e 0000 0072 4500 0000  .rO...r....rE...
-000011a0: 7229 0000 0029 0572 3100 0000 7237 0000  r)...).r1...r7..
-000011b0: 005a 0e70 6173 7377 6f72 645f 746f 6b65  .Z.password_toke
-000011c0: 6e5a 086c 6f67 5f63 6f6e 6672 4a00 0000  nZ.log_confrJ...
-000011d0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-000011e0: 4e00 0000 e900 0000 7314 0000 0000 0104  N.......s.......
-000011f0: 0114 0208 0104 010c 0104 010e 0108 0124  ...............$
-00001200: 0272 4e00 0000 6302 0000 0000 0000 0005  .rN...c.........
-00001210: 0000 000a 0000 0043 0000 0073 8a00 0000  .......C...s....
-00001220: 7c00 7400 6b07 720c 6400 5300 7400 7c00  |.t.k.r.d.S.t.|.
-00001230: 1900 7d02 7401 6a02 6401 6a03 7c01 8301  ..}.t.j.d.j.|...
-00001240: 8301 0100 7c02 6402 1900 7d03 7c03 8f20  ....|.d...}.|.. 
-00001250: 0100 7404 6403 6404 8d01 6a05 8300 7d04  ..t.d.d...j...}.
-00001260: 7c03 6a06 7c04 6405 8d01 0100 5700 6400  |.j.|.d.....W.d.
-00001270: 5100 5200 5800 7c00 7407 6b06 7276 7401  Q.R.X.|.t.k.rvt.
-00001280: 6a02 6406 6a03 7c01 8301 8301 0100 7407  j.d.j.|.......t.
-00001290: 7c00 1900 5300 7401 6a02 6407 6a03 7c01  |...S.t.j.d.j.|.
-000012a0: 8301 8301 0100 6400 5300 2908 4e7a 2357  ......d.S.).Nz#W
-000012b0: 6169 7469 6e67 2064 6174 6162 6173 6520  aiting database 
-000012c0: 636f 6e6e 6563 7469 6f6e 2022 7b7d 222e  connection "{}".
-000012d0: 2e2e da09 636f 6e6e 6563 7465 64e9 0a00  ....connected...
-000012e0: 0000 2901 da07 6d69 6e75 7465 7329 01da  ..)...minutes)..
-000012f0: 0774 696d 656f 7574 7a1e 466f 756e 6420  .timeoutz.Found 
-00001300: 6461 7461 6261 7365 2063 6f6e 6e65 6374  database connect
-00001310: 696f 6e20 227b 7d22 7a22 4e6f 7420 666f  ion "{}"z"Not fo
-00001320: 756e 6420 6461 7461 6261 7365 2063 6f6e  und database con
-00001330: 6e65 6374 696f 6e20 227b 7d22 2908 da13  nection "{}")...
-00001340: 7065 6e64 696e 675f 636f 6e6e 6563 7469  pending_connecti
-00001350: 6f6e 7372 1400 0000 7246 0000 0072 2e00  onsr....rF...r..
-00001360: 0000 7202 0000 00da 0d74 6f74 616c 5f73  ..r......total_s
-00001370: 6563 6f6e 6473 da04 7761 6974 723f 0000  econds..waitr?..
-00001380: 0029 0572 4800 0000 724a 0000 00da 1270  .).rH...rJ.....p
-00001390: 656e 6469 6e67 5f63 6f6e 6e65 6374 696f  ending_connectio
-000013a0: 6eda 1363 6f6e 6e65 6374 6564 5f63 6f6e  n..connected_con
-000013b0: 6469 7469 6f6e 7256 0000 0072 1600 0000  ditionrV...r....
-000013c0: 7216 0000 0072 1700 0000 da17 7761 6974  r....r......wait
-000013d0: 5f70 656e 6469 6e67 5f63 6f6e 6e65 6374  _pending_connect
-000013e0: 696f 6ef8 0000 0073 1800 0000 0001 0801  ion....s........
-000013f0: 0402 0802 1002 0801 0601 0e01 1602 0801  ................
-00001400: 1001 0802 725c 0000 0063 0200 0000 0000  ....r\...c......
-00001410: 0000 0300 0000 0800 0000 4300 0000 7374  ..........C...st
-00001420: 0000 0074 007c 007c 0183 027d 027c 0273  ...t.|.|...}.|.s
-00001430: 1674 0164 0183 0182 017c 006a 0264 0283  .t.d.....|.j.d..
-00001440: 0164 036b 0272 2c74 037c 0283 0153 007c  .d.k.r,t.|...S.|
-00001450: 006a 0264 0283 0164 046b 0272 5274 037c  .j.d...d.k.rRt.|
-00001460: 027c 006a 0264 0583 0164 0664 0764 0864  .|.j.d...d.d.d.d
-00001470: 098d 0553 0074 037c 027c 006a 0264 0583  ...S.t.|.|.j.d..
-00001480: 0164 0664 0764 0864 0a64 0b69 0164 0c8d  .d.d.d.d.d.i.d..
-00001490: 0653 0064 0053 0029 0d4e 7a21 4461 7461  .S.d.S.).Nz!Data
-000014a0: 6261 7365 2063 6f6e 6669 6775 7261 7469  base configurati
-000014b0: 6f6e 2069 7320 6e6f 7420 7365 7472 1900  on is not setr..
-000014c0: 0000 721b 0000 0072 1f00 0000 723f 0000  ..r....r....r?..
-000014d0: 0054 e901 0000 0069 2c01 0000 2904 da09  .T.....i,...)...
-000014e0: 706f 6f6c 5f73 697a 65da 0d70 6f6f 6c5f  pool_size..pool_
-000014f0: 7072 655f 7069 6e67 da0c 6d61 785f 6f76  pre_ping..max_ov
-00001500: 6572 666c 6f77 da0c 706f 6f6c 5f72 6563  erflow..pool_rec
-00001510: 7963 6c65 da0f 636f 6e6e 6563 745f 7469  ycle..connect_ti
-00001520: 6d65 6f75 74e9 0500 0000 2905 725e 0000  meout.....).r^..
-00001530: 0072 5f00 0000 7260 0000 0072 6100 0000  .r_...r`...ra...
-00001540: 5a0c 636f 6e6e 6563 745f 6172 6773 2904  Z.connect_args).
-00001550: 7234 0000 00da 0945 7863 6570 7469 6f6e  r4.....Exception
-00001560: 7229 0000 0072 0a00 0000 2903 7231 0000  r)...r....).r1..
-00001570: 0072 3200 0000 5a0a 656e 6769 6e65 5f75  .r2...Z.engine_u
-00001580: 726c 7216 0000 0072 1600 0000 7217 0000  rlr....r....r...
-00001590: 00da 1863 7265 6174 655f 636f 6e6e 6563  ...create_connec
-000015a0: 7469 6f6e 5f65 6e67 696e 650c 0100 0073  tion_engine....s
-000015b0: 2600 0000 0001 0a02 0401 0802 0e01 0801  &...............
-000015c0: 0e01 0201 0201 0801 0201 0201 0803 0201  ................
-000015d0: 0201 0801 0201 0201 0201 7265 0000 0063  ..........re...c
-000015e0: 0100 0000 0000 0000 0200 0000 0300 0000  ................
-000015f0: 0300 0000 7310 0000 0087 0066 0164 0164  ....s......f.d.d
-00001600: 0284 087d 017c 0153 0029 034e 6302 0000  ...}.|.S.).Nc...
-00001610: 0000 0000 0002 0000 0003 0000 0013 0000  ................
-00001620: 0073 4400 0000 8800 6a00 6401 8301 6400  .sD.....j.d...d.
-00001630: 6b09 7220 7c00 8800 6a00 6401 8301 6b07  k.r |...j.d...k.
-00001640: 7220 6402 5300 8800 6a00 6403 8301 6400  r d.S...j.d...d.
-00001650: 6b09 7240 7c00 8800 6a00 6403 8301 6b06  k.r@|...j.d...k.
-00001660: 7240 6402 5300 6404 5300 2905 4e72 3500  r@d.S.d.S.).Nr5.
-00001670: 0000 4672 3600 0000 5429 0172 2900 0000  ..Fr6...T).r)...
-00001680: 2902 da05 7461 626c 65da 046d 6574 6129  )...table..meta)
-00001690: 0172 3100 0000 7216 0000 0072 1700 0000  .r1...r....r....
-000016a0: 7235 0000 0028 0100 0073 0a00 0000 0001  r5...(...s......
-000016b0: 1c01 0401 1c01 0401 7a2b 6765 745f 636f  ........z+get_co
-000016c0: 6e6e 6563 7469 6f6e 5f6f 6e6c 795f 7072  nnection_only_pr
-000016d0: 6564 6963 6174 652e 3c6c 6f63 616c 733e  edicate.<locals>
-000016e0: 2e6f 6e6c 7972 1600 0000 2902 7231 0000  .onlyr....).r1..
-000016f0: 0072 3500 0000 7216 0000 0029 0172 3100  .r5...r....).r1.
-00001700: 0000 7217 0000 00da 1d67 6574 5f63 6f6e  ..r......get_con
-00001710: 6e65 6374 696f 6e5f 6f6e 6c79 5f70 7265  nection_only_pre
-00001720: 6469 6361 7465 2701 0000 7304 0000 0000  dicate'...s.....
-00001730: 010c 0672 6800 0000 6301 0000 0000 0000  ...rh...c.......
-00001740: 001c 0000 0023 0000 0043 0000 0073 c202  .....#...C...s..
-00001750: 0000 7400 7c00 8301 7d01 7401 7c00 8301  ..t.|...}.t.|...
-00001760: 7d02 7c01 7402 6b06 7238 7402 7c01 1900  }.|.t.k.r8t.|...
-00001770: 6401 1900 7c02 6b02 7230 7402 7c01 1900  d...|.k.r0t.|...
-00001780: 5300 7403 7c00 8301 0100 7404 7c00 8301  S.t.|.....t.|...
-00001790: 7d03 7405 7c00 7c03 8302 7d04 7406 7c01  }.t.|.|...}.t.|.
-000017a0: 7c04 8302 7d05 7c05 725c 7c05 5300 7407  |...}.|.r\|.S.t.
-000017b0: 6a08 8300 7d06 7409 6a0a 8300 7d07 740b  j...}.t.j...}.t.
-000017c0: 6402 8301 7d08 7c08 7c04 7c00 6a0c 6403  d...}.|.|.|.j.d.
-000017d0: 8301 7c00 6a0c 6404 8301 7c06 6a0d 8300  ..|.j.d...|.j...
-000017e0: 7c07 6405 9c06 7d09 7c09 740e 7c01 3c00  |.d...}.|.t.|.<.
-000017f0: 6400 7d0a 9001 7ada 9001 799c 740f 7c00  d.}...z...y.t.|.
-00001800: 8301 7d0a 7c0a 7c09 6406 3c00 7410 7c00  ..}.|.|.d.<.t.|.
-00001810: 7c0a 8302 7d0b 7c0b 7c09 6407 3c00 7411  |...}.|.|.d.<.t.
-00001820: 7412 7c0b 6408 8d01 8301 7d0c 7c0c 8300  t.|.d.....}.|...
-00001830: 7d0d 7413 6a14 6409 6a15 7c04 8301 8301  }.t.j.d.j.|.....
-00001840: 0100 7416 6a16 8300 7d0e 7c0d 6a17 8300  ..t.j...}.|.j...
-00001850: 9001 8f2e 7d0f 7416 6a16 8300 7d10 7418  ....}.t.j...}.t.
-00001860: 7c10 7c0e 1800 640a 8302 7d11 7413 6a14  |.|...d...}.t.j.
-00001870: 640b 6a15 7c04 8301 8301 0100 7419 7c0d  d.j.|.......t.|.
-00001880: 8301 7d12 7413 6a14 640c 6a15 7c04 8301  ..}.t.j.d.j.|...
-00001890: 8301 0100 7416 6a16 8300 7d13 741a 7c03  ....t.j...}.t.|.
-000018a0: 7c0f 640d 8d02 7d14 741b 7c00 8301 7d15  |.d...}.t.|...}.
-000018b0: 741c 7c14 7c0b 7c15 7c09 640e 8d04 0100  t.|.|.|.|.d.....
-000018c0: 7416 6a16 8300 7d16 7418 7c16 7c13 1800  t.j...}.t.|.|...
-000018d0: 640a 8302 7d17 7413 6a14 640f 6a15 7c04  d...}.t.j.d.j.|.
-000018e0: 8301 8301 0100 741d 7c14 6410 8d01 7d18  ......t.|.d...}.
-000018f0: 741e 7c18 8301 0100 7848 7c18 6a1f 6a20  t.|.....xH|.j.j 
-00001900: 6a21 8300 4400 5d38 5c02 7d19 7d1a 7422  j!..D.]8\.}.}.t"
-00001910: 7c1a 6a23 6a24 8301 6411 6b02 9001 72b4  |.j#j$..d.k...r.
-00001920: 7c19 7c18 6a25 6b07 9001 72b4 7413 6a26  |.|.j%k...r.t.j&
-00001930: 6412 6a15 7c19 8301 8301 0100 9001 71b4  d.j.|.........q.
-00001940: 5700 7c01 7c04 7c0b 7c0c 7c18 7c02 7c12  W.|.|.|.|.|.|.|.
-00001950: 7c0a 6900 7409 6a27 8300 7c00 6a0c 6403  |.i.t.j'..|.j.d.
-00001960: 8301 7c00 6a0c 6404 8301 7c06 6a0d 8300  ..|.j.d...|.j...
-00001970: 7c11 7c17 6413 9c0f 7402 7c01 3c00 5700  |.|.d...t.|.<.W.
-00001980: 6400 5100 5200 5800 7c0d 6a28 8300 0100  d.Q.R.X.|.j(....
-00001990: 7402 7c01 1900 5300 0400 7429 6b0a 9002  t.|...S...t)k...
-000019a0: 727a 0100 7d1b 0100 7a18 7c0a 9002 7266  rz..}...z.|...rf
-000019b0: 7c0a 6a28 8300 0100 7c1b 8201 5700 5900  |.j(....|...W.Y.
-000019c0: 6400 6400 7d1b 7e1b 5800 6e02 5800 5700  d.d.}.~.X.n.X.W.
-000019d0: 6400 7c01 740e 6b06 9002 72a4 740e 7c01  d.|.t.k...r.t.|.
-000019e0: 1900 6a0c 6414 8301 7c08 6b02 9002 72a4  ..j.d...|.k...r.
-000019f0: 740e 7c01 3d00 7c07 8f0e 0100 7c07 6a2a  t.|.=.|.....|.j*
-00001a00: 8300 0100 5700 6400 5100 5200 5800 5800  ....W.d.Q.R.X.X.
-00001a10: 6400 5300 2915 4eda 0970 6172 616d 735f  d.S.).N..params_
-00001a20: 6964 e920 0000 00da 0770 726f 6a65 6374  id. .....project
-00001a30: da05 746f 6b65 6e29 06da 0269 6472 1a00  ..token)...idr..
-00001a40: 0000 726b 0000 0072 6c00 0000 da0a 696e  ..rk...rl.....in
-00001a50: 6974 5f73 7461 7274 7253 0000 0072 3200  it_startrS...r2.
-00001a60: 0000 7219 0000 0029 01da 0462 696e 647a  ..r....)...bindz
-00001a70: 1e43 6f6e 6e65 6374 696e 6720 746f 2064  .Connecting to d
-00001a80: 6174 6162 6173 6520 227b 7d22 2e2e 2ee9  atabase "{}"....
-00001a90: 0300 0000 7a1c 4765 7474 696e 6720 6462  ....z.Getting db
-00001aa0: 2074 7970 6573 2066 6f72 2022 7b7d 222e   types for "{}".
-00001ab0: 2e2e 7a1a 4765 7474 696e 6720 7363 6865  ..z.Getting sche
-00001ac0: 6d61 2066 6f72 2022 7b7d 222e 2e2e 2902  ma for "{}"...).
-00001ad0: 7237 0000 0072 6f00 0000 2902 7235 0000  r7...ro...).r5..
-00001ae0: 0072 5a00 0000 7a11 436f 6e6e 6563 7465  .rZ...z.Connecte
-00001af0: 6420 746f 2022 7b7d 2229 01da 086d 6574  d to "{}")...met
-00001b00: 6164 6174 6172 0100 0000 7a38 5461 626c  adatar....z8Tabl
-00001b10: 6520 227b 7d22 2064 6f65 7320 6e6f 7420  e "{}" does not 
-00001b20: 6861 7665 2070 7269 6d61 7279 206b 6579  have primary key
-00001b30: 2061 6e64 2077 696c 6c20 6265 2069 676e   and will be ign
-00001b40: 6f72 6564 290f 726d 0000 0072 1a00 0000  ored).rm...r....
-00001b50: 7219 0000 00da 0753 6573 7369 6f6e da0a  r......Session..
-00001b60: 4d61 7070 6564 4261 7365 7269 0000 00da  MappedBaseri....
-00001b70: 1574 7970 655f 636f 6465 5f74 6f5f 7371  .type_code_to_sq
-00001b80: 6c5f 7479 7065 7232 0000 00da 0563 6163  l_typer2.....cac
-00001b90: 6865 da04 6c6f 636b 726b 0000 0072 6c00  he..lockrk...rl.
-00001ba0: 0000 726e 0000 00da 0c63 6f6e 6e65 6374  ..rn.....connect
-00001bb0: 5f74 696d 65da 0c72 6566 6c65 6374 5f74  _time..reflect_t
-00001bc0: 696d 6572 6d00 0000 292b 723e 0000 0072  imerm...)+r>...r
-00001bd0: 4000 0000 723f 0000 0072 4700 0000 724d  @...r?...rG...rM
-00001be0: 0000 0072 4e00 0000 725c 0000 0072 0300  ...rN...r\...r..
-00001bf0: 0000 da03 6e6f 77da 0974 6872 6561 6469  ....now..threadi
-00001c00: 6e67 da09 436f 6e64 6974 696f 6e72 1000  ng..Conditionr..
-00001c10: 0000 7229 0000 00da 0969 736f 666f 726d  ..r).....isoform
-00001c20: 6174 7257 0000 0072 5100 0000 7265 0000  atrW...rQ...re..
-00001c30: 0072 0f00 0000 720e 0000 0072 1400 0000  .r....r....r....
-00001c40: 7246 0000 0072 2e00 0000 da04 7469 6d65  rF...r......time
-00001c50: 7249 0000 00da 0572 6f75 6e64 7207 0000  rI.....roundr...
-00001c60: 0072 0b00 0000 7268 0000 0072 0400 0000  .r....rh...r....
-00001c70: 720c 0000 00da 106c 6f61 645f 6d61 7070  r......load_mapp
-00001c80: 6564 5f62 6173 6572 7100 0000 5a06 7461  ed_baserq...Z.ta
-00001c90: 626c 6573 da05 6974 656d 73da 036c 656e  bles..items..len
-00001ca0: 5a0b 7072 696d 6172 795f 6b65 79da 0763  Z.primary_key..c
-00001cb0: 6f6c 756d 6e73 da07 636c 6173 7365 73da  olumns..classes.
-00001cc0: 0777 6172 6e69 6e67 da04 4c6f 636b da05  .warning..Lock..
-00001cd0: 636c 6f73 6572 6400 0000 da0a 6e6f 7469  closerd.....noti
-00001ce0: 6679 5f61 6c6c 291c 7231 0000 0072 4800  fy_all).r1...rH.
-00001cf0: 0000 5a14 636f 6e6e 6563 7469 6f6e 5f70  ..Z.connection_p
-00001d00: 6172 616d 735f 6964 7237 0000 0072 4a00  arams_idr7...rJ.
-00001d10: 0000 5a13 6578 6973 7469 6e67 5f63 6f6e  ..Z.existing_con
-00001d20: 6e65 6374 696f 6e72 6e00 0000 725b 0000  nectionrn...r[..
-00001d30: 005a 1570 656e 6469 6e67 5f63 6f6e 6e65  .Z.pending_conne
-00001d40: 6374 696f 6e5f 6964 725a 0000 0072 3200  ction_idrZ...r2.
-00001d50: 0000 7219 0000 0072 7200 0000 da07 7365  ..r....rr.....se
-00001d60: 7373 696f 6e5a 0d63 6f6e 6e65 6374 5f73  ssionZ.connect_s
-00001d70: 7461 7274 7249 0000 005a 0b63 6f6e 6e65  tartrI...Z.conne
-00001d80: 6374 5f65 6e64 7277 0000 0072 7400 0000  ct_endrw...rt...
-00001d90: 5a0d 7265 666c 6563 745f 7374 6172 7472  Z.reflect_startr
-00001da0: 7100 0000 7235 0000 005a 0b72 6566 6c65  q...r5...Z.refle
-00001db0: 6374 5f65 6e64 7278 0000 0072 7300 0000  ct_endrx...rs...
-00001dc0: 5a0a 7461 626c 655f 6e61 6d65 7266 0000  Z.table_namerf..
-00001dd0: 00da 0165 7216 0000 0072 1600 0000 7217  ...er....r....r.
-00001de0: 0000 00da 1063 6f6e 6e65 6374 5f64 6174  .....connect_dat
-00001df0: 6162 6173 6531 0100 0073 9400 0000 0003  abase1...s......
-00001e00: 0801 0802 0801 1001 0802 0802 0801 0a02  ................
-00001e10: 0a01 0401 0402 0802 0801 0802 0201 0201  ................
-00001e20: 0801 0801 0601 0803 0801 0402 0801 0801  ................
-00001e30: 0802 0a01 0802 0e01 0602 1002 0801 0c01  ................
-00001e40: 0801 0e02 1001 0802 1002 0802 0c01 0801  ................
-00001e50: 1002 0801 0e02 1002 0a01 0802 1601 1e01  ................
-00001e60: 1603 0201 0201 0201 0201 0201 0201 0201  ................
-00001e70: 0201 0201 0601 0801 0801 0601 0201 1603  ................
-00001e80: 0802 0801 1201 0601 0802 1a02 1e01 0602  ................
-00001e90: 0601 728a 0000 0063 0100 0000 0000 0000  ..r....c........
-00001ea0: 0100 0000 0b00 0000 4300 0000 7340 0000  ........C...s@..
-00001eb0: 0079 267c 0064 0119 006a 0083 0001 007c  .y&|.d...j.....|
-00001ec0: 006a 0164 0283 0172 247c 0064 0219 006a  .j.d...r$|.d...j
-00001ed0: 0283 0001 0064 0353 0004 0074 036b 0a72  .....d.S...t.k.r
-00001ee0: 3a01 0001 0001 0064 0453 0058 0064 0053  :......d.S.X.d.S
-00001ef0: 0029 054e 7219 0000 0072 3200 0000 5446  .).Nr....r2...TF
-00001f00: 2904 da07 6469 7370 6f73 6572 2900 0000  )...disposer)...
-00001f10: 7286 0000 0072 6400 0000 2901 7249 0000  r....rd...).rI..
-00001f20: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00001f30: da19 6469 7370 6f73 655f 636f 6e6e 6563  ..dispose_connec
-00001f40: 7469 6f6e 5f6f 626a 6563 749e 0100 0073  tion_object....s
-00001f50: 0e00 0000 0001 0201 0c02 0a01 0c02 0401  ................
-00001f60: 0e01 728c 0000 0063 0100 0000 0000 0000  ..r....c........
-00001f70: 0300 0000 0200 0000 4300 0000 732c 0000  ........C...s,..
-00001f80: 0074 007c 0083 017d 0174 016a 027c 0183  .t.|...}.t.j.|..
-00001f90: 017d 027c 0272 2874 037c 0283 0172 2874  .}.|.r(t.|...r(t
-00001fa0: 017c 013d 0064 0153 0064 0253 0029 034e  .|.=.d.S.d.S.).N
-00001fb0: 5446 2904 723e 0000 0072 3f00 0000 7229  TF).r>...r?...r)
-00001fc0: 0000 0072 8c00 0000 2903 7231 0000 0072  ...r....).r1...r
-00001fd0: 4800 0000 7249 0000 0072 1600 0000 7216  H...rI...r....r.
-00001fe0: 0000 0072 1700 0000 7247 0000 00aa 0100  ...r....rG......
-00001ff0: 0073 0c00 0000 0003 0801 0a02 0c01 0601  .s..............
-00002000: 0402 7247 0000 0063 0100 0000 0000 0000  ..rG...c........
-00002010: 0100 0000 0300 0000 4300 0000 730c 0000  ........C...s...
-00002020: 0074 0074 017c 0083 0183 0153 0029 014e  .t.t.|.....S.).N
-00002030: 2902 7247 0000 00da 0867 6574 5f63 6f6e  ).rG.....get_con
-00002040: 6629 01da 0772 6571 7565 7374 7216 0000  f)...requestr...
-00002050: 0072 1600 0000 7217 0000 00da 1a64 6973  .r....r......dis
-00002060: 706f 7365 5f72 6571 7565 7374 5f63 6f6e  pose_request_con
-00002070: 6e65 6374 696f 6eb7 0100 0073 0200 0000  nection....s....
-00002080: 0001 728f 0000 0063 0000 0000 0000 0000  ..r....c........
-00002090: 0000 0000 1200 0000 4300 0000 734a 0000  ........C...sJ..
-000020a0: 0074 006a 0174 006a 0274 006a 0374 006a  .t.j.t.j.t.j.t.j
-000020b0: 0474 006a 0574 006a 0674 006a 0774 006a  .t.j.t.j.t.j.t.j
-000020c0: 0874 006a 0974 006a 0a74 006a 0b74 006a  .t.j.t.j.t.j.t.j
-000020d0: 0c74 006a 0d74 006a 0e74 006a 0f74 006a  .t.j.t.j.t.j.t.j
-000020e0: 1074 006a 1164 019c 1153 0029 024e 2911  .t.j.d...S.).N).
-000020f0: 7219 0000 0072 2600 0000 7227 0000 0072  r....r&...r'...r
-00002100: 1a00 0000 7223 0000 0072 2000 0000 721d  ....r#...r ...r.
-00002110: 0000 0072 3f00 0000 7235 0000 0072 3600  ...r?...r5...r6.
-00002120: 0000 7237 0000 0072 3800 0000 7239 0000  ..r7...r8...r9..
-00002130: 0072 3a00 0000 723b 0000 0072 6b00 0000  .r:...r;...rk...
-00002140: 726c 0000 0029 1272 1300 0000 da0f 4441  rl...).r......DA
-00002150: 5441 4241 5345 5f45 4e47 494e 45da 0d44  TABASE_ENGINE..D
-00002160: 4154 4142 4153 455f 484f 5354 da0d 4441  ATABASE_HOST..DA
-00002170: 5441 4241 5345 5f50 4f52 54da 0d44 4154  TABASE_PORT..DAT
-00002180: 4142 4153 455f 4e41 4d45 da0d 4441 5441  ABASE_NAME..DATA
-00002190: 4241 5345 5f55 5345 52da 1144 4154 4142  BASE_USER..DATAB
-000021a0: 4153 455f 5041 5353 574f 5244 da0e 4441  ASE_PASSWORD..DA
-000021b0: 5441 4241 5345 5f45 5854 5241 da14 4441  TABASE_EXTRA..DA
-000021c0: 5441 4241 5345 5f43 4f4e 4e45 4354 494f  TABASE_CONNECTIO
-000021d0: 4e53 da0d 4441 5441 4241 5345 5f4f 4e4c  NS..DATABASE_ONL
-000021e0: 59da 0f44 4154 4142 4153 455f 4558 4345  Y..DATABASE_EXCE
-000021f0: 5054 da0f 4441 5441 4241 5345 5f53 4348  PT..DATABASE_SCH
-00002200: 454d 41da 1144 4154 4142 4153 455f 5353  EMA..DATABASE_SS
-00002210: 485f 484f 5354 da11 4441 5441 4241 5345  H_HOST..DATABASE
-00002220: 5f53 5348 5f50 4f52 54da 1144 4154 4142  _SSH_PORT..DATAB
-00002230: 4153 455f 5353 485f 5553 4552 da18 4441  ASE_SSH_USER..DA
-00002240: 5441 4241 5345 5f53 5348 5f50 5249 5641  TABASE_SSH_PRIVA
-00002250: 5445 5f4b 4559 da07 5052 4f4a 4543 54da  TE_KEY..PROJECT.
-00002260: 0554 4f4b 454e 7216 0000 0072 1600 0000  .TOKENr....r....
-00002270: 7216 0000 0072 1700 0000 da11 6765 745f  r....r......get_
-00002280: 7365 7474 696e 6773 5f63 6f6e 66bb 0100  settings_conf...
-00002290: 0073 2200 0000 0002 0401 0401 0401 0401  .s".............
-000022a0: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-000022b0: 0401 0401 0401 0401 72a1 0000 0063 0100  ........r....c..
-000022c0: 0000 0000 0000 0200 0000 1200 0000 4300  ..............C.
-000022d0: 0000 73a0 0000 007c 006a 0083 007d 017c  ..s....|.j...}.|
-000022e0: 0173 1064 0053 007c 016a 0164 0183 017c  .s.d.S.|.j.d...|
-000022f0: 016a 0164 0283 017c 016a 0164 0383 017c  .j.d...|.j.d...|
-00002300: 016a 0164 0483 017c 016a 0164 0583 017c  .j.d...|.j.d...|
-00002310: 016a 0164 0683 017c 016a 0164 0783 017c  .j.d...|.j.d...|
-00002320: 016a 0164 0864 0983 027c 016a 0164 0a83  .j.d.d...|.j.d..
-00002330: 017c 016a 0164 0b83 017c 016a 0164 0c83  .|.j.d...|.j.d..
-00002340: 017c 016a 0164 0d83 017c 016a 0164 0e83  .|.j.d...|.j.d..
-00002350: 017c 016a 0164 0f83 017c 016a 0164 1083  .|.j.d...|.j.d..
-00002360: 017c 016a 0164 1183 017c 016a 0164 1283  .|.j.d...|.j.d..
-00002370: 0164 139c 1153 0029 144e da0f 6461 7461  .d...S.).N..data
-00002380: 6261 7365 5f65 6e67 696e 65da 0d64 6174  base_engine..dat
-00002390: 6162 6173 655f 686f 7374 da0d 6461 7461  abase_host..data
-000023a0: 6261 7365 5f70 6f72 74da 0d64 6174 6162  base_port..datab
-000023b0: 6173 655f 6e61 6d65 da0d 6461 7461 6261  ase_name..databa
-000023c0: 7365 5f75 7365 72da 1164 6174 6162 6173  se_user..databas
-000023d0: 655f 7061 7373 776f 7264 da0e 6461 7461  e_password..data
-000023e0: 6261 7365 5f65 7874 7261 5a14 6461 7461  base_extraZ.data
-000023f0: 6261 7365 5f63 6f6e 6e65 6374 696f 6e73  base_connections
-00002400: e932 0000 00da 0d64 6174 6162 6173 655f  .2.....database_
-00002410: 6f6e 6c79 da0f 6461 7461 6261 7365 5f65  only..database_e
-00002420: 7863 6570 74da 0f64 6174 6162 6173 655f  xcept..database_
-00002430: 7363 6865 6d61 da11 6461 7461 6261 7365  schema..database
-00002440: 5f73 7368 5f68 6f73 74da 1164 6174 6162  _ssh_host..datab
-00002450: 6173 655f 7373 685f 706f 7274 da11 6461  ase_ssh_port..da
-00002460: 7461 6261 7365 5f73 7368 5f75 7365 72da  tabase_ssh_user.
-00002470: 1864 6174 6162 6173 655f 7373 685f 7072  .database_ssh_pr
-00002480: 6976 6174 655f 6b65 7972 6b00 0000 726c  ivate_keyrk...rl
-00002490: 0000 0029 1172 1900 0000 7226 0000 0072  ...).r....r&...r
-000024a0: 2700 0000 721a 0000 0072 2300 0000 7220  '...r....r#...r 
-000024b0: 0000 0072 1d00 0000 723f 0000 0072 3500  ...r....r?...r5.
-000024c0: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
-000024d0: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
-000024e0: 726b 0000 0072 6c00 0000 2902 5a13 6765  rk...rl...).Z.ge
-000024f0: 745f 6272 6964 6765 5f73 6574 7469 6e67  t_bridge_setting
-00002500: 7372 2900 0000 2902 728e 0000 005a 0f62  sr)...).r....Z.b
-00002510: 7269 6467 655f 7365 7474 696e 6773 7216  ridge_settingsr.
-00002520: 0000 0072 1600 0000 7217 0000 00da 1067  ...r....r......g
-00002530: 6574 5f72 6571 7565 7374 5f63 6f6e 66d1  et_request_conf.
-00002540: 0100 0073 2800 0000 0001 0802 0401 0403  ...s(...........
-00002550: 0801 0801 0801 0801 0801 0801 0801 0a01  ................
-00002560: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00002570: 72b1 0000 0063 0100 0000 0000 0000 0200  r....c..........
-00002580: 0000 0200 0000 4300 0000 731a 0000 0074  ......C...s....t
-00002590: 007c 0083 017d 017c 0172 107c 0153 0074  .|...}.|.r.|.S.t
-000025a0: 0183 0053 0064 0053 0029 014e 2902 72b1  ...S.d.S.).N).r.
-000025b0: 0000 0072 a100 0000 2902 728e 0000 005a  ...r....).r....Z
-000025c0: 0c72 6571 7565 7374 5f63 6f6e 6672 1600  .request_confr..
-000025d0: 0000 7216 0000 0072 1700 0000 728d 0000  ..r....r....r...
-000025e0: 00ec 0100 0073 0800 0000 0001 0802 0401  .....s..........
-000025f0: 0402 728d 0000 0063 0100 0000 0000 0000  ..r....c........
-00002600: 0300 0000 0200 0000 4300 0000 731a 0000  ........C...s...
-00002610: 0074 007c 0083 017d 0174 017c 0183 017d  .t.|...}.t.|...}
-00002620: 0274 026a 037c 0283 0153 0029 014e 2904  .t.j.|...S.).N).
-00002630: 728d 0000 0072 3e00 0000 723f 0000 0072  r....r>...r?...r
-00002640: 2900 0000 2903 728e 0000 0072 3100 0000  )...).r....r1...
-00002650: 7248 0000 0072 1600 0000 7216 0000 0072  rH...r....r....r
-00002660: 1700 0000 da0e 6765 745f 636f 6e6e 6563  ......get_connec
-00002670: 7469 6f6e f501 0000 7306 0000 0000 0108  tion....s.......
-00002680: 0108 0172 b200 0000 6300 0000 0000 0000  ...r....c.......
-00002690: 0000 0000 0002 0000 0043 0000 0073 1800  .........C...s..
-000026a0: 0000 7400 6a01 6401 6b02 720e 6400 5300  ..t.j.d.k.r.d.S.
-000026b0: 7402 7403 8300 8301 5300 2902 4eda 046e  t.t.....S.).N..n
-000026c0: 6f6e 6529 0472 1300 0000 7290 0000 0072  one).r....r....r
-000026d0: 8a00 0000 72a1 0000 0072 1600 0000 7216  ....r....r....r.
-000026e0: 0000 0072 1600 0000 7217 0000 00da 1e63  ...r....r......c
-000026f0: 6f6e 6e65 6374 5f64 6174 6162 6173 655f  onnect_database_
-00002700: 6672 6f6d 5f73 6574 7469 6e67 73fb 0100  from_settings...
-00002710: 0073 0600 0000 0001 0a01 0401 72b4 0000  .s..........r...
-00002720: 0063 0100 0000 0000 0000 0100 0000 0300  .c..............
-00002730: 0000 4300 0000 730c 0000 0074 0074 017c  ..C...s....t.t.|
-00002740: 0083 0183 0153 0029 014e 2902 728a 0000  .....S.).N).r...
-00002750: 0072 8d00 0000 2901 728e 0000 0072 1600  .r....).r....r..
-00002760: 0000 7216 0000 0072 1700 0000 da16 6765  ..r....r......ge
-00002770: 745f 7265 7175 6573 745f 636f 6e6e 6563  t_request_connec
-00002780: 7469 6f6e 0102 0000 7302 0000 0000 0172  tion....s......r
-00002790: b500 0000 6301 0000 0000 0000 0002 0000  ....c...........
-000027a0: 0002 0000 0043 0000 0073 1a00 0000 7400  .....C...s....t.
-000027b0: 7c00 8301 7d01 7c01 7310 6400 5300 7c01  |...}.|.s.d.S.|.
-000027c0: 6401 1900 8300 5300 2902 4e72 7200 0000  d.....S.).Nrr...
-000027d0: 2901 72b5 0000 0029 0272 8e00 0000 7249  ).r....).r....rI
-000027e0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000027f0: 0000 da0e 6372 6561 7465 5f73 6573 7369  ....create_sessi
-00002800: 6f6e 0502 0000 7308 0000 0000 0108 0104  on....s.........
-00002810: 0104 0172 b600 0000 6301 0000 0000 0000  ...r....c.......
-00002820: 0002 0000 0002 0000 0043 0000 0073 1800  .........C...s..
-00002830: 0000 7400 7c00 8301 7d01 7c01 7310 6400  ..t.|...}.|.s.d.
-00002840: 5300 7c01 6401 1900 5300 2902 4e72 7300  S.|.d...S.).Nrs.
-00002850: 0000 2901 72b5 0000 0029 0272 8e00 0000  ..).r....).r....
-00002860: 7249 0000 0072 1600 0000 7216 0000 0072  rI...r....r....r
-00002870: 1700 0000 da0f 6765 745f 6d61 7070 6564  ......get_mapped
-00002880: 5f62 6173 650c 0200 0073 0800 0000 0001  _base....s......
-00002890: 0801 0401 0401 72b7 0000 0063 0100 0000  ......r....c....
-000028a0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-000028b0: 7318 0000 0074 007c 0083 017d 017c 0173  s....t.|...}.|.s
-000028c0: 1064 0053 007c 0164 0119 0053 0029 024e  .d.S.|.d...S.).N
-000028d0: 7219 0000 0029 0172 b500 0000 2902 728e  r....).r....).r.
-000028e0: 0000 0072 4900 0000 7216 0000 0072 1600  ...rI...r....r..
-000028f0: 0000 7217 0000 00da 0a67 6574 5f65 6e67  ..r......get_eng
-00002900: 696e 6513 0200 0073 0800 0000 0001 0801  ine....s........
-00002910: 0401 0401 72b8 0000 0063 0100 0000 0000  ....r....c......
-00002920: 0000 0200 0000 0200 0000 4300 0000 7318  ..........C...s.
-00002930: 0000 0074 007c 0083 017d 017c 0173 1064  ...t.|...}.|.s.d
-00002940: 0053 007c 0164 0119 0053 0029 024e 7274  .S.|.d...S.).Nrt
-00002950: 0000 0029 0172 b500 0000 2902 728e 0000  ...).r....).r...
-00002960: 0072 4900 0000 7216 0000 0072 1600 0000  .rI...r....r....
-00002970: 7217 0000 00da 1967 6574 5f74 7970 655f  r......get_type_
-00002980: 636f 6465 5f74 6f5f 7371 6c5f 7479 7065  code_to_sql_type
-00002990: 1a02 0000 7308 0000 0000 0108 0104 0104  ....s...........
-000029a0: 0172 b900 0000 6301 0000 0000 0000 0002  .r....c.........
-000029b0: 0000 0009 0000 0063 0000 0073 3400 0000  .......c...s4...
-000029c0: 7400 7c00 8301 7d01 7c01 7312 6900 5600  t.|...}.|.s.i.V.
-000029d0: 0100 7c01 6401 1900 8f10 0100 7c01 6402  ..|.d.......|.d.
-000029e0: 1900 5600 0100 5700 6400 5100 5200 5800  ..V...W.d.Q.R.X.
-000029f0: 6400 5300 2903 4e72 7600 0000 7275 0000  d.S.).Nrv...ru..
-00002a00: 0029 0172 b500 0000 2902 728e 0000 0072  .).r....).r....r
-00002a10: 4900 0000 7216 0000 0072 1600 0000 7217  I...r....r....r.
-00002a20: 0000 00da 1063 6f6e 6e65 6374 696f 6e5f  .....connection_
-00002a30: 6361 6368 6521 0200 0073 0a00 0000 0002  cache!...s......
-00002a40: 0801 0401 0601 0a01 72ba 0000 0063 0300  ........r....c..
-00002a50: 0000 0000 0000 0400 0000 0a00 0000 4300  ..............C.
-00002a60: 0000 7334 0000 0074 007c 0083 017d 037c  ..s4...t.|...}.|
-00002a70: 0373 1064 0053 007c 0364 0119 008f 1201  .s.d.S.|.d......
-00002a80: 007c 0364 0219 006a 017c 017c 0283 0253  .|.d...j.|.|...S
-00002a90: 0051 0052 0058 0064 0053 0029 034e 7276  .Q.R.X.d.S.).Nrv
-00002aa0: 0000 0072 7500 0000 2902 72b5 0000 0072  ...ru...).r....r
-00002ab0: 2900 0000 2904 728e 0000 0072 1a00 0000  )...).r....r....
-00002ac0: da07 6465 6661 756c 7472 4900 0000 7216  ..defaultrI...r.
-00002ad0: 0000 0072 1600 0000 7217 0000 00da 1463  ...r....r......c
-00002ae0: 6f6e 6e65 6374 696f 6e5f 6361 6368 655f  onnection_cache_
-00002af0: 6765 742a 0200 0073 0a00 0000 0001 0801  get*...s........
-00002b00: 0401 0401 0a01 72bc 0000 0063 0300 0000  ......r....c....
-00002b10: 0000 0000 0400 0000 0a00 0000 4300 0000  ............C...
-00002b20: 7334 0000 0074 007c 0083 017d 037c 0373  s4...t.|...}.|.s
-00002b30: 1064 0053 007c 0364 0119 008f 1201 007c  .d.S.|.d.......|
-00002b40: 027c 0364 0219 007c 013c 0057 0064 0051  .|.d...|.<.W.d.Q
-00002b50: 0052 0058 0064 0053 0029 034e 7276 0000  .R.X.d.S.).Nrv..
-00002b60: 0072 7500 0000 2901 72b5 0000 0029 0472  .ru...).r....).r
-00002b70: 8e00 0000 721a 0000 0072 1500 0000 7249  ....r....r....rI
-00002b80: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002b90: 0000 da14 636f 6e6e 6563 7469 6f6e 5f63  ....connection_c
-00002ba0: 6163 6865 5f73 6574 3202 0000 730a 0000  ache_set2...s...
-00002bb0: 0000 0108 0104 0104 010a 0172 bd00 0000  ...........r....
-00002bc0: 6301 0000 0000 0000 0002 0000 0003 0000  c...............
-00002bd0: 0043 0000 0073 1e00 0000 7400 7c00 8301  .C...s....t.|...
-00002be0: 7d01 7401 7c01 6401 8302 0100 7402 7c00  }.t.|.d.....t.|.
-00002bf0: 8301 0100 6400 5300 2902 4e54 2903 72b7  ....d.S.).NT).r.
-00002c00: 0000 0072 7f00 0000 da1d 7265 6c6f 6164  ...r......reload
-00002c10: 5f72 6571 7565 7374 5f67 7261 7068 716c  _request_graphql
-00002c20: 5f73 6368 656d 6129 0272 8e00 0000 7273  _schema).r....rs
-00002c30: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002c40: 0000 da1a 7265 6c6f 6164 5f72 6571 7565  ....reload_reque
-00002c50: 7374 5f6d 6170 7065 645f 6261 7365 3a02  st_mapped_base:.
-00002c60: 0000 7306 0000 0000 0108 010a 0172 bf00  ..s..........r..
-00002c70: 0000 6302 0000 0000 0000 0004 0000 000a  ..c.............
-00002c80: 0000 0043 0000 0073 4600 0000 7400 7c00  ...C...sF...t.|.
-00002c90: 8301 8f34 7d02 7c01 6400 6b08 7224 6400  ...4}.|.d.k.r$d.
-00002ca0: 7c02 6401 3c00 6400 7c02 6402 3c00 6e14  |.d.<.d.|.d.<.n.
-00002cb0: 7c01 722c 6402 6e02 6401 7d03 6400 7c02  |.r,d.n.d.}.d.|.
-00002cc0: 7c03 3c00 5700 6400 5100 5200 5800 6400  |.<.W.d.Q.R.X.d.
-00002cd0: 5300 2903 4e5a 0e67 7261 7068 716c 5f73  S.).NZ.graphql_s
-00002ce0: 6368 656d 615a 1467 7261 7068 716c 5f73  chemaZ.graphql_s
-00002cf0: 6368 656d 615f 6472 6166 7429 0172 ba00  chema_draft).r..
-00002d00: 0000 2904 728e 0000 00da 0564 7261 6674  ..).r......draft
-00002d10: 7275 0000 005a 0a73 6368 656d 615f 6b65  ru...Z.schema_ke
-00002d20: 7972 1600 0000 7216 0000 0072 1700 0000  yr....r....r....
-00002d30: 72be 0000 0040 0200 0073 0c00 0000 0001  r....@...s......
-00002d40: 0a01 0801 0801 0a02 0c01 72be 0000 0063  ..........r....c
-00002d50: 0200 0000 0000 0000 0200 0000 0300 0000  ................
-00002d60: 4300 0000 7330 0000 007c 016a 0072 227c  C...s0...|.j.r"|
-00002d70: 016a 007c 006a 006b 0372 2264 016a 017c  .j.|.j.k.r"d.j.|
-00002d80: 016a 007c 016a 0283 0253 0074 037c 016a  .j.|.j...S.t.|.j
-00002d90: 0283 0153 0064 0053 0029 024e 7a05 7b7d  ...S.d.S.).Nz.{}
-00002da0: 2e7b 7d29 0472 3700 0000 722e 0000 0072  .{}).r7...r....r
-00002db0: 1a00 0000 722a 0000 0029 0272 7100 0000  ....r*...).rq...
-00002dc0: 7266 0000 0072 1600 0000 7216 0000 0072  rf...r....r....r
-00002dd0: 1700 0000 da0e 6765 745f 7461 626c 655f  ......get_table_
-00002de0: 6e61 6d65 4a02 0000 7306 0000 0000 0112  nameJ...s.......
-00002df0: 0110 0272 c100 0000 4663 0200 0000 0000  ...r....Fc......
-00002e00: 0000 0500 0000 0500 0000 0300 0000 7348  ..............sH
-00002e10: 0000 0087 0066 0164 0164 0284 087d 0264  .....f.d.d...}.d
-00002e20: 0364 0484 007d 0364 0564 0684 007d 047c  .d...}.d.d...}.|
-00002e30: 0172 3488 006a 006a 0183 0001 0088 006a  .r4..j.j.......j
-00002e40: 026a 0383 0001 0088 006a 047c 027c 037c  .j.......j.|.|.|
-00002e50: 0464 078d 0301 0064 0053 0029 084e 6303  .d.....d.S.).Nc.
-00002e60: 0000 0000 0000 0003 0000 0003 0000 0013  ................
-00002e70: 0000 0073 0c00 0000 7400 8800 6a01 7c02  ...s....t...j.|.
-00002e80: 8302 5300 2901 4e29 0272 c100 0000 7271  ..S.).N).r....rq
-00002e90: 0000 0029 03da 0462 6173 655a 0974 6162  ...)...baseZ.tab
-00002ea0: 6c65 6e61 6d65 7266 0000 0029 0172 7300  lenamerf...).rs.
-00002eb0: 0000 7216 0000 0072 1700 0000 da13 636c  ..r....r......cl
-00002ec0: 6173 736e 616d 655f 666f 725f 7461 626c  assname_for_tabl
-00002ed0: 6552 0200 0073 0200 0000 0001 7a2d 6c6f  eR...s......z-lo
-00002ee0: 6164 5f6d 6170 7065 645f 6261 7365 2e3c  ad_mapped_base.<
-00002ef0: 6c6f 6361 6c73 3e2e 636c 6173 736e 616d  locals>.classnam
-00002f00: 655f 666f 725f 7461 626c 6563 0400 0000  e_for_tablec....
-00002f10: 0000 0000 0600 0000 0500 0000 5300 0000  ............S...
-00002f20: 7370 0000 0074 007c 036a 0183 0172 147c  sp...t.|.j...r.|
-00002f30: 036a 0164 0119 006e 0264 007d 047c 0472  .j.d...n.d.}.|.r
-00002f40: 3e64 026a 027c 046a 036a 0464 037c 046a  >d.j.|.j.j.d.|.j
-00002f50: 056a 066a 047c 046a 056a 0467 0483 017d  .j.j.|.j.j.g...}
-00002f60: 056e 0a7c 026a 076a 0883 007d 057c 057c  .n.|.j.j...}.|.|
-00002f70: 036a 036a 096b 0672 6c7c 0564 0417 007d  .j.j.k.rl|.d...}
-00002f80: 0574 0a6a 0b64 056a 0c7c 0583 0183 0101  .t.j.d.j.|......
-00002f90: 007c 0553 0029 064e 7201 0000 00da 025f  .|.S.).Nr......_
-00002fa0: 5fda 0274 6fda 095f 7265 6c61 7469 6f6e  _..to.._relation
-00002fb0: 7a26 416c 7265 6164 7920 6465 7465 6374  z&Already detect
-00002fc0: 6564 2063 6f6c 756d 6e20 6e61 6d65 2c20  ed column name, 
-00002fd0: 7573 696e 6720 7b7d 290d 7281 0000 00da  using {}).r.....
-00002fe0: 0865 6c65 6d65 6e74 7372 3000 0000 da06  .elementsr0.....
-00002ff0: 7061 7265 6e74 721a 0000 00da 0663 6f6c  parentr......col
-00003000: 756d 6e72 6600 0000 da08 5f5f 6e61 6d65  umnrf.....__name
-00003010: 5f5f da05 6c6f 7765 7272 8200 0000 7214  __..lowerr....r.
-00003020: 0000 0072 8400 0000 722e 0000 0029 0672  ...r....r....).r
-00003030: c200 0000 da09 6c6f 6361 6c5f 636c 73da  ......local_cls.
-00003040: 0c72 6566 6572 7265 645f 636c 73da 0a63  .referred_cls..c
-00003050: 6f6e 7374 7261 696e 74da 0b66 6f72 6569  onstraint..forei
-00003060: 676e 5f6b 6579 721a 0000 0072 1600 0000  gn_keyr....r....
-00003070: 7216 0000 0072 1700 0000 da1c 6e61 6d65  r....r......name
-00003080: 5f66 6f72 5f73 6361 6c61 725f 7265 6c61  _for_scalar_rela
-00003090: 7469 6f6e 7368 6970 5502 0000 7310 0000  tionshipU...s...
-000030a0: 0000 0118 0104 0122 020a 020c 0108 0110  ......."........
-000030b0: 027a 366c 6f61 645f 6d61 7070 6564 5f62  .z6load_mapped_b
-000030c0: 6173 652e 3c6c 6f63 616c 733e 2e6e 616d  ase.<locals>.nam
-000030d0: 655f 666f 725f 7363 616c 6172 5f72 656c  e_for_scalar_rel
-000030e0: 6174 696f 6e73 6869 7063 0400 0000 0000  ationshipc......
-000030f0: 0000 0600 0000 0500 0000 5300 0000 7370  ..........S...sp
-00003100: 0000 0074 007c 036a 0183 0172 147c 036a  ...t.|.j...r.|.j
-00003110: 0164 0119 006e 0264 007d 047c 0472 3e64  .d...n.d.}.|.r>d
-00003120: 026a 027c 046a 036a 046a 057c 046a 036a  .j.|.j.j.j.|.j.j
-00003130: 0564 037c 046a 066a 0567 0483 017d 056e  .d.|.j.j.g...}.n
-00003140: 0a7c 026a 076a 0883 007d 057c 057c 036a  .|.j.j...}.|.|.j
-00003150: 036a 096b 0672 6c7c 0564 0417 007d 0574  .j.k.rl|.d...}.t
-00003160: 0a6a 0b64 056a 0c7c 0583 0183 0101 007c  .j.d.j.|.......|
-00003170: 0553 0029 064e 7201 0000 0072 c400 0000  .S.).Nr....r....
-00003180: 72c5 0000 0072 c600 0000 7a26 416c 7265  r....r....z&Alre
-00003190: 6164 7920 6465 7465 6374 6564 2063 6f6c  ady detected col
-000031a0: 756d 6e20 6e61 6d65 2c20 7573 696e 6720  umn name, using 
-000031b0: 7b7d 290d 7281 0000 0072 c700 0000 7230  {}).r....r....r0
-000031c0: 0000 0072 c800 0000 7266 0000 0072 1a00  ...r....rf...r..
-000031d0: 0000 72c9 0000 0072 ca00 0000 72cb 0000  ..r....r....r...
-000031e0: 0072 8200 0000 7214 0000 0072 8400 0000  .r....r....r....
-000031f0: 722e 0000 0029 0672 c200 0000 72cc 0000  r....).r....r...
-00003200: 0072 cd00 0000 72ce 0000 0072 cf00 0000  .r....r....r....
-00003210: 721a 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00003220: 1700 0000 da20 6e61 6d65 5f66 6f72 5f63  ..... name_for_c
-00003230: 6f6c 6c65 6374 696f 6e5f 7265 6c61 7469  ollection_relati
-00003240: 6f6e 7368 6970 6202 0000 7310 0000 0000  onshipb...s.....
-00003250: 0118 0104 0122 020a 020c 0108 0110 027a  .....".........z
-00003260: 3a6c 6f61 645f 6d61 7070 6564 5f62 6173  :load_mapped_bas
-00003270: 652e 3c6c 6f63 616c 733e 2e6e 616d 655f  e.<locals>.name_
-00003280: 666f 725f 636f 6c6c 6563 7469 6f6e 5f72  for_collection_r
-00003290: 656c 6174 696f 6e73 6869 7029 0372 c300  elationship).r..
-000032a0: 0000 72d0 0000 0072 d100 0000 2905 da08  ..r....r....)...
-000032b0: 7265 6769 7374 7279 728b 0000 0072 8300  registryr....r..
-000032c0: 0000 da05 636c 6561 72da 0770 7265 7061  ....clear..prepa
-000032d0: 7265 2905 7273 0000 0072 d300 0000 72c3  re).rs...r....r.
-000032e0: 0000 0072 d000 0000 72d1 0000 0072 1600  ...r....r....r..
-000032f0: 0000 2901 7273 0000 0072 1700 0000 727f  ..).rs...r....r.
-00003300: 0000 0051 0200 0073 1400 0000 0001 0c03  ...Q...s........
-00003310: 080d 080d 0401 0a01 0a02 0401 0201 0201  ................
-00003320: 727f 0000 0029 014e 2901 4e29 014e 2901  r....).N).N).N).
-00003330: 4629 4972 2c00 0000 da0a 636f 6e74 6578  F)Ir,.....contex
-00003340: 746c 6962 723c 0000 0072 7a00 0000 727d  tlibr<...rz...r}
-00003350: 0000 0072 0300 0000 7202 0000 005a 176a  ...r....r....Z.j
-00003360: 6574 5f62 7269 6467 655f 6261 7365 2e72  et_bridge_base.r
-00003370: 6566 6c65 6374 7204 0000 005a 1a6a 6574  eflectr....Z.jet
-00003380: 5f62 7269 6467 655f 6261 7365 2e73 7368  _bridge_base.ssh
-00003390: 5f74 756e 6e65 6c72 0500 0000 5a1b 6a65  _tunnelr....Z.je
-000033a0: 745f 6272 6964 6765 5f62 6173 652e 7574  t_bridge_base.ut
-000033b0: 696c 732e 6372 7970 7472 0600 0000 5a20  ils.cryptr....Z 
-000033c0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-000033d0: 7574 696c 732e 7479 7065 5f63 6f64 6573  utils.type_codes
-000033e0: 7207 0000 00da 0373 6978 7208 0000 005a  r......sixr....Z
-000033f0: 1673 6978 2e6d 6f76 6573 2e75 726c 6c69  .six.moves.urlli
-00003400: 625f 7061 7273 6572 0900 0000 5a0a 7371  b_parser....Z.sq
-00003410: 6c61 6c63 6865 6d79 720a 0000 0072 0b00  lalchemyr....r..
-00003420: 0000 5a16 7371 6c61 6c63 6865 6d79 2e65  ..Z.sqlalchemy.e
-00003430: 7874 2e61 7574 6f6d 6170 720c 0000 0072  xt.automapr....r
-00003440: 0d00 0000 5a0e 7371 6c61 6c63 6865 6d79  ....Z.sqlalchemy
-00003450: 2e6f 726d 720e 0000 0072 0f00 0000 da1c  .ormr....r......
-00003460: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00003470: 7574 696c 732e 636f 6d6d 6f6e 7210 0000  utils.commonr...
-00003480: 0072 1100 0000 5a0b 6765 6f61 6c63 6865  .r....Z.geoalche
-00003490: 6d79 3272 1200 0000 da0b 496d 706f 7274  my2r......Import
-000034a0: 4572 726f 72da 0f6a 6574 5f62 7269 6467  Error..jet_bridg
-000034b0: 655f 6261 7365 7213 0000 00da 166a 6574  e_baser......jet
-000034c0: 5f62 7269 6467 655f 6261 7365 2e6c 6f67  _bridge_base.log
-000034d0: 6765 7272 1400 0000 723f 0000 0072 5700  gerr....r?...rW.
-000034e0: 0000 7218 0000 0072 3400 0000 723e 0000  ..r....r4...r>..
-000034f0: 0072 4000 0000 7245 0000 0072 5100 0000  .r@...rE...rQ...
-00003500: 724d 0000 0072 4e00 0000 725c 0000 0072  rM...rN...r\...r
-00003510: 6500 0000 7268 0000 0072 8a00 0000 728c  e...rh...r....r.
-00003520: 0000 0072 4700 0000 728f 0000 0072 a100  ...rG...r....r..
-00003530: 0000 72b1 0000 0072 8d00 0000 72b2 0000  ..r....r....r...
-00003540: 0072 b400 0000 72b5 0000 0072 b600 0000  .r....r....r....
-00003550: 72b7 0000 0072 b800 0000 72b9 0000 00da  r....r....r.....
-00003560: 0e63 6f6e 7465 7874 6d61 6e61 6765 7272  .contextmanagerr
-00003570: ba00 0000 72bc 0000 0072 bd00 0000 72bf  ....r....r....r.
-00003580: 0000 0072 be00 0000 72c1 0000 0072 7f00  ...r....r....r..
-00003590: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000035a0: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000035b0: 0100 0000 736e 0000 0008 0108 0108 0108  ....sn..........
-000035c0: 0108 0110 020c 010c 010c 010c 010c 010c  ................
-000035d0: 0210 0110 0110 0210 0202 0110 010e 0106  ................
-000035e0: 020c 010c 0204 0104 0308 040a 5108 1208  ............Q...
-000035f0: 0708 0408 4d08 0908 0f08 1408 1b08 0a08  ....M...........
-00003600: 6d08 0c08 0d08 0408 1608 1b08 0908 0608  m...............
-00003610: 0608 0408 0708 0708 0708 070e 090a 0808  ................
-00003620: 0808 060a 0a08 07                        .......
+000000b0: 0100 6400 640a 6c15 6d16 5a16 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 640b 6c17 6d18 5a18 6d19 5a19 0100 6400  d.l.m.Z.m.Z...d.
+000000d0: 640c 6c1a 6d1b 5a1b 6d1c 5a1c 0100 6400  d.l.m.Z.m.Z...d.
+000000e0: 640d 6c1d 6d1e 5a1e 6d1f 5a1f 0100 7910  d.l.m.Z.m.Z...y.
+000000f0: 6400 640e 6c20 6d21 5a21 0100 5700 6e14  d.d.l m!Z!..W.n.
+00000100: 0400 6522 6b0a 72ec 0100 0100 0100 5900  ..e"k.r.......Y.
+00000110: 6e02 5800 6400 640f 6c23 6d24 5a24 0100  n.X.d.d.l#m$Z$..
+00000120: 6400 6410 6c25 6d26 5a26 0100 6900 6127  d.d.l%m&Z&..i.a'
+00000130: 6900 6128 6411 6412 8400 5a29 6454 6413  i.a(d.d...Z)dTd.
+00000140: 6414 8401 5a2a 6415 6416 8400 5a2b 6417  d...Z*d.d...Z+d.
+00000150: 6418 8400 5a2c 6419 641a 8400 5a2d 641b  d...Z,d.d...Z-d.
+00000160: 641c 8400 5a2e 641d 641e 8400 5a2f 641f  d...Z.d.d...Z/d.
+00000170: 6420 8400 5a30 6421 6422 8400 5a31 6423  d ..Z0d!d"..Z1d#
+00000180: 6424 8400 5a32 6425 6426 8400 5a33 6427  d$..Z2d%d&..Z3d'
+00000190: 6428 8400 5a34 6429 642a 8400 5a35 642b  d(..Z4d)d*..Z5d+
+000001a0: 642c 8400 5a36 642d 642e 8400 5a37 642f  d,..Z6d-d...Z7d/
+000001b0: 6430 8400 5a38 6431 6432 8400 5a39 6433  d0..Z8d1d2..Z9d3
+000001c0: 6434 8400 5a3a 6435 6436 8400 5a3b 6437  d4..Z:d5d6..Z;d7
+000001d0: 6438 8400 5a3c 6439 643a 8400 5a3d 643b  d8..Z<d9d:..Z=d;
+000001e0: 643c 8400 5a3e 643d 643e 8400 5a3f 643f  d<..Z>d=d>..Z?d?
+000001f0: 6440 8400 5a40 6441 6442 8400 5a41 6443  d@..Z@dAdB..ZAdC
+00000200: 6444 8400 5a42 6501 6a43 6445 6446 8400  dD..ZBe.jCdEdF..
+00000210: 8301 5a44 6455 6447 6448 8401 5a45 6449  ..ZDdUdGdH..ZEdI
+00000220: 644a 8400 5a46 644b 644c 8400 5a47 6456  dJ..ZFdKdL..ZGdV
+00000230: 644d 644e 8401 5a48 644f 6450 8400 5a49  dMdN..ZHdOdP..ZI
+00000240: 6457 6452 6453 8401 5a4a 6401 5300 2958  dWdRdS..ZJd.S.)X
+00000250: e900 0000 004e 2902 da09 7469 6d65 6465  .....N)...timede
+00000260: 6c74 61da 0864 6174 6574 696d 6529 01da  lta..datetime)..
+00000270: 0c61 7574 6f6d 6170 5f62 6173 6529 01da  .automap_base)..
+00000280: 0772 6566 6c65 6374 2901 da09 5353 4854  .reflect)...SSHT
+00000290: 756e 6e65 6c29 01da 0f67 6574 5f73 6861  unnel)...get_sha
+000002a0: 3235 365f 6861 7368 2901 da16 6765 745f  256_hash)...get_
+000002b0: 6d65 6d6f 7279 5f75 7361 6765 5f68 756d  memory_usage_hum
+000002c0: 616e 2901 da1b 6665 7463 685f 7479 7065  an)...fetch_type
+000002d0: 5f63 6f64 655f 746f 5f73 716c 5f74 7970  _code_to_sql_typ
+000002e0: 6529 01da 0853 7472 696e 6749 4f29 01da  e)...StringIO)..
+000002f0: 0a71 756f 7465 5f70 6c75 7329 02da 0d63  .quote_plus)...c
+00000300: 7265 6174 655f 656e 6769 6e65 da08 4d65  reate_engine..Me
+00000310: 7461 4461 7461 2902 da0c 7365 7373 696f  taData)...sessio
+00000320: 6e6d 616b 6572 da0e 7363 6f70 6564 5f73  nmaker..scoped_s
+00000330: 6573 7369 6f6e 2902 da11 6765 745f 7261  ession)...get_ra
+00000340: 6e64 6f6d 5f73 7472 696e 67da 056d 6572  ndom_string..mer
+00000350: 6765 2901 da05 7479 7065 7329 01da 0873  ge)...types)...s
+00000360: 6574 7469 6e67 7329 01da 066c 6f67 6765  ettings)...logge
+00000370: 7263 0100 0000 0000 0000 0100 0000 0200  rc..............
+00000380: 0000 4300 0000 7308 0000 0074 007c 0083  ..C...s....t.|..
+00000390: 0153 0029 014e 2901 720b 0000 0029 01da  .S.).N).r....)..
+000003a0: 0576 616c 7565 a900 7216 0000 00fa 592f  .value..r.....Y/
+000003b0: 5573 6572 732f 6631 6e61 6c2f 4472 6f70  Users/f1nal/Drop
+000003c0: 626f 782f 7079 7468 6f6e 2f6a 6574 2d62  box/python/jet-b
+000003d0: 7269 6467 652f 7372 632f 7061 636b 6167  ridge/src/packag
+000003e0: 6573 2f6a 6574 5f62 7269 6467 655f 6261  es/jet_bridge_ba
+000003f0: 7365 2f6a 6574 5f62 7269 6467 655f 6261  se/jet_bridge_ba
+00000400: 7365 2f64 622e 7079 da0a 7572 6c5f 656e  se/db.py..url_en
+00000410: 636f 6465 2200 0000 7302 0000 0000 0172  code"...s......r
+00000420: 1800 0000 6302 0000 0000 0000 0005 0000  ....c...........
+00000430: 000a 0000 0043 0000 0073 5203 0000 7c00  .....C...sR...|.
+00000440: 6a00 6401 8301 0c00 7318 7c00 6a00 6402  j.d.....s.|.j.d.
+00000450: 8301 0c00 721c 6400 5300 7401 7c00 6a00  ....r.d.S.t.|.j.
+00000460: 6401 8301 8301 6403 6702 7d02 7c00 6a00  d.....d.g.}.|.j.
+00000470: 6401 8301 6404 6b02 7286 7c02 6a02 6405  d...d.k.r.|.j.d.
+00000480: 8301 0100 7c02 6a02 7401 7c00 6a00 6402  ....|.j.t.|.j.d.
+00000490: 8301 8301 8301 0100 7c00 6a00 6406 8301  ........|.j.d...
+000004a0: 7282 7c02 6a02 6407 8301 0100 7c02 6a02  r.|.j.d.....|.j.
+000004b0: 7401 7c00 6a00 6406 8301 8301 8301 0100  t.|.j.d.........
+000004c0: 9002 6ec2 7c00 6a00 6401 8301 6408 6b02  ..n.|.j.d...d.k.
+000004d0: 9001 720e 7c02 6a02 7401 7c00 6a00 6402  ..r.|.j.t.|.j.d.
+000004e0: 8301 8301 8301 0100 7952 7403 6a04 7c00  ........yRt.j.|.
+000004f0: 6a00 6409 8301 8301 0100 7c02 6a02 640a  j.d.......|.j.d.
+00000500: 6a05 7c00 6a00 6409 8301 8301 8301 0100  j.|.j.d.........
+00000510: 7c00 6a00 6406 8301 72fa 7c02 6a02 640b  |.j.d...r.|.j.d.
+00000520: 8301 0100 7c02 6a02 7401 7c00 6a00 6406  ....|.j.t.|.j.d.
+00000530: 8301 8301 8301 0100 5700 6e0c 0100 0100  ........W.n.....
+00000540: 0100 5900 6e02 5800 9002 6e3a 7c00 6a00  ..Y.n.X...n:|.j.
+00000550: 6401 8301 640c 6b02 9001 72ce 7c02 6a02  d...d.k...r.|.j.
+00000560: 7406 7401 7c00 6a00 640d 8301 8301 8301  t.t.|.j.d.......
+00000570: 8301 0100 7c00 6a00 6409 8301 9001 7264  ....|.j.d.....rd
+00000580: 7c02 6a02 640e 8301 0100 7c02 6a02 7406  |.j.d.....|.j.t.
+00000590: 7401 7c00 6a00 6409 8301 8301 8301 8301  t.|.j.d.........
+000005a0: 0100 7c02 6a02 640f 8301 0100 7c02 6a02  ..|.j.d.....|.j.
+000005b0: 7401 7c00 6a00 6410 8301 8301 8301 0100  t.|.j.d.........
+000005c0: 7c02 6a02 6405 8301 0100 7c02 6a02 7401  |.j.d.....|.j.t.
+000005d0: 7c00 6a00 6402 8301 8301 8301 0100 7c00  |.j.d.........|.
+000005e0: 6a00 6406 8301 9003 7248 7c02 6a02 6407  j.d.....rH|.j.d.
+000005f0: 8301 0100 7c02 6a02 7401 7c00 6a00 6406  ....|.j.t.|.j.d.
+00000600: 8301 8301 8301 0100 9001 6e7a 7c01 9001  ..........nz|...
+00000610: 72d8 6411 6e08 7c00 6a00 6410 8301 7d03  r.d.n.|.j.d...}.
+00000620: 7c01 9001 72ee 7c01 6a07 6e08 7c00 6a00  |...r.|.j.n.|.j.
+00000630: 6412 8301 7d04 7c00 6a00 640d 8301 9002  d...}.|.j.d.....
+00000640: 725a 7c02 6a02 7406 7401 7c00 6a00 640d  rZ|.j.t.t.|.j.d.
+00000650: 8301 8301 8301 8301 0100 7c00 6a00 6409  ..........|.j.d.
+00000660: 8301 9002 724a 7c02 6a02 640e 8301 0100  ....rJ|.j.d.....
+00000670: 7c02 6a02 7406 7401 7c00 6a00 6409 8301  |.j.t.t.|.j.d...
+00000680: 8301 8301 8301 0100 7c03 9002 725a 7c02  ........|...rZ|.
+00000690: 6a02 640f 8301 0100 7c03 9002 7296 7c02  j.d.....|...r.|.
+000006a0: 6a02 7401 7c03 8301 8301 0100 7c04 9002  j.t.|.......|...
+000006b0: 728c 7c02 6a02 640e 8301 0100 7c02 6a02  r.|.j.d.....|.j.
+000006c0: 7401 7c04 8301 8301 0100 7c02 6a02 6405  t.|.......|.j.d.
+000006d0: 8301 0100 7c00 6a00 6401 8301 6413 6b03  ....|.j.d...d.k.
+000006e0: 9002 72ba 7c02 6a02 7401 7c00 6a00 6402  ..r.|.j.t.|.j.d.
+000006f0: 8301 8301 8301 0100 7c00 6a00 6406 8301  ........|.j.d...
+00000700: 9002 72e6 7c02 6a02 6407 8301 0100 7c02  ..r.|.j.d.....|.
+00000710: 6a02 7401 7c00 6a00 6406 8301 8301 8301  j.t.|.j.d.......
+00000720: 0100 6e62 7c00 6a00 6401 8301 6414 6b02  ..nb|.j.d...d.k.
+00000730: 9003 7202 7c02 6a02 6415 8301 0100 6e46  ..r.|.j.d.....nF
+00000740: 7c00 6a00 6401 8301 6416 6b02 9003 721e  |.j.d...d.k...r.
+00000750: 7c02 6a02 6417 8301 0100 6e2a 7c00 6a00  |.j.d.....n*|.j.
+00000760: 6401 8301 6413 6b02 9003 7248 7c02 6a02  d...d.k...rH|.j.
+00000770: 6418 6a05 7406 7c00 6a00 6402 8301 8301  d.j.t.|.j.d.....
+00000780: 8301 8301 0100 6419 6a08 7c02 8301 5300  ......d.j.|...S.
+00000790: 291a 4eda 0665 6e67 696e 65da 046e 616d  ).N..engine..nam
+000007a0: 657a 033a 2f2f da06 7371 6c69 7465 fa01  ez.://..sqlite..
+000007b0: 2fda 0565 7874 7261 fa01 3fda 0862 6967  /..extra..?..big
+000007c0: 7175 6572 79da 0870 6173 7377 6f72 647a  query..passwordz
+000007d0: 163f 6372 6564 656e 7469 616c 735f 6261  .?credentials_ba
+000007e0: 7365 3634 3d7b 7dfa 0126 da09 736e 6f77  se64={}..&..snow
+000007f0: 666c 616b 65da 0475 7365 72fa 013a fa01  flake..user..:..
+00000800: 40da 0468 6f73 747a 0931 3237 2e30 2e30  @..hostz.127.0.0
+00000810: 2e31 da04 706f 7274 da06 6f72 6163 6c65  .1..port..oracle
+00000820: da05 6d79 7371 6c7a 0d3f 6368 6172 7365  ..mysqlz.?charse
+00000830: 743d 7574 6638 7a0c 6d73 7371 6c2b 7079  t=utf8z.mssql+py
+00000840: 6f64 6263 7a0f 3f64 7269 7665 723d 4672  odbcz.?driver=Fr
+00000850: 6565 5444 537a 103f 7365 7276 6963 655f  eeTDSz.?service_
+00000860: 6e61 6d65 3d7b 7dda 0029 09da 0367 6574  name={}..)...get
+00000870: da03 7374 72da 0661 7070 656e 64da 0662  ..str..append..b
+00000880: 6173 6536 34da 0962 3634 6465 636f 6465  ase64..b64decode
+00000890: da06 666f 726d 6174 7218 0000 00da 0f6c  ..formatr......l
+000008a0: 6f63 616c 5f62 696e 645f 706f 7274 da04  ocal_bind_port..
+000008b0: 6a6f 696e 2905 da04 636f 6e66 da06 7475  join)...conf..tu
+000008c0: 6e6e 656c da03 7572 6c72 2600 0000 7227  nnel..urlr&...r'
+000008d0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000008e0: 0000 da10 6275 696c 645f 656e 6769 6e65  ....build_engine
+000008f0: 5f75 726c 2600 0000 7376 0000 0000 0118  _url&...sv......
+00000900: 0104 030c 0106 030e 010a 0114 020a 010a  ................
+00000910: 0118 0110 0114 0202 0110 0116 020a 010a  ................
+00000920: 0118 0106 010a 0110 0118 020c 010a 0118  ................
+00000930: 020a 0214 010a 0214 020c 010a 0118 0214  ................
+00000940: 0116 020c 0118 020c 010a 0118 0206 010a  ................
+00000950: 0206 010e 0206 010a 010e 020a 0210 0114  ................
+00000960: 020c 010a 0116 0110 010c 0110 010c 0110  ................
+00000970: 011a 0272 3600 0000 6301 0000 0000 0000  ...r6...c.......
+00000980: 0001 0000 0013 0000 0043 0000 0073 8e00  .........C...s..
+00000990: 0000 7400 7401 6a02 7c00 6a03 6401 8301  ..t.t.j.|.j.d...
+000009a0: 7c00 6a03 6402 8301 7c00 6a03 6403 8301  |.j.d...|.j.d...
+000009b0: 7c00 6a03 6404 8301 7c00 6a03 6405 8301  |.j.d...|.j.d...
+000009c0: 7c00 6a03 6406 8301 7c00 6a03 6407 8301  |.j.d...|.j.d...
+000009d0: 7c00 6a03 6408 8301 7c00 6a03 6409 8301  |.j.d...|.j.d...
+000009e0: 7c00 6a03 640a 8301 7c00 6a03 640b 8301  |.j.d...|.j.d...
+000009f0: 7c00 6a03 640c 8301 7c00 6a03 640d 8301  |.j.d...|.j.d...
+00000a00: 7c00 6a03 640e 8301 7c00 6a03 640f 8301  |.j.d...|.j.d...
+00000a10: 7c00 6a03 6410 8301 6710 8301 8301 5300  |.j.d...g.....S.
+00000a20: 2911 4e72 1900 0000 7226 0000 0072 2700  ).Nr....r&...r'.
+00000a30: 0000 721a 0000 0072 2300 0000 7220 0000  ..r....r#...r ..
+00000a40: 00da 046f 6e6c 79da 0665 7863 6570 74da  ...only..except.
+00000a50: 0673 6368 656d 61da 0673 736c 5f63 61da  .schema..ssl_ca.
+00000a60: 0873 736c 5f63 6572 74da 0773 736c 5f6b  .ssl_cert..ssl_k
+00000a70: 6579 da08 7373 685f 686f 7374 da08 7373  ey..ssh_host..ss
+00000a80: 685f 706f 7274 da08 7373 685f 7573 6572  h_port..ssh_user
+00000a90: da0f 7373 685f 7072 6976 6174 655f 6b65  ..ssh_private_ke
+00000aa0: 7929 0472 0700 0000 da04 6a73 6f6e da05  y).r......json..
+00000ab0: 6475 6d70 7372 2b00 0000 2901 7233 0000  dumpsr+...).r3..
+00000ac0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000ad0: da11 6765 745f 636f 6e6e 6563 7469 6f6e  ..get_connection
+00000ae0: 5f69 647a 0000 0073 2200 0000 0001 0601  _idz...s".......
+00000af0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00000b00: 0801 0801 0801 0801 0801 0801 0801 7243  ..............rC
+00000b10: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
+00000b20: 0400 0000 4300 0000 731a 0000 0074 006a  ....C...s....t.j
+00000b30: 017c 006a 0264 0183 017c 006a 0264 0283  .|.j.d...|.j.d..
+00000b40: 0167 0283 0153 0029 034e 721d 0000 00da  .g...S.).Nr.....
+00000b50: 0b63 6f6e 6e65 6374 696f 6e73 2903 7241  .connections).rA
+00000b60: 0000 0072 4200 0000 722b 0000 0029 0172  ...rB...r+...).r
+00000b70: 3300 0000 7216 0000 0072 1600 0000 7217  3...r....r....r.
+00000b80: 0000 00da 1867 6574 5f63 6f6e 6e65 6374  .....get_connect
+00000b90: 696f 6e5f 7061 7261 6d73 5f69 648f 0000  ion_params_id...
+00000ba0: 0073 0600 0000 0001 0401 0801 7245 0000  .s..........rE..
+00000bb0: 0063 0100 0000 0000 0000 0100 0000 0700  .c..............
+00000bc0: 0000 0300 0000 731e 0000 0074 0074 0187  ......s....t.t..
+00000bd0: 0066 0164 0164 0284 0864 0364 0464 0564  .f.d.d...d.d.d.d
+00000be0: 0667 0483 0283 0153 0029 074e 6301 0000  .g.....S.).Nc...
+00000bf0: 0000 0000 0001 0000 0002 0000 0013 0000  ................
+00000c00: 0073 0a00 0000 8800 6a00 7c00 8301 5300  .s......j.|...S.
+00000c10: 2901 4e29 0172 2b00 0000 2901 da01 7829  ).N).r+...)...x)
+00000c20: 0172 3300 0000 7216 0000 0072 1700 0000  .r3...r....r....
+00000c30: da08 3c6c 616d 6264 613e 9700 0000 7300  ..<lambda>....s.
+00000c40: 0000 007a 2669 735f 7475 6e6e 656c 5f63  ...z&is_tunnel_c
+00000c50: 6f6e 6e65 6374 696f 6e2e 3c6c 6f63 616c  onnection.<local
+00000c60: 733e 2e3c 6c61 6d62 6461 3e72 3d00 0000  s>.<lambda>r=...
+00000c70: 723e 0000 0072 3f00 0000 7240 0000 0029  r>...r?...r@...)
+00000c80: 02da 0361 6c6c da03 6d61 7029 0172 3300  ...all..map).r3.
+00000c90: 0000 7216 0000 0029 0172 3300 0000 7217  ..r....).r3...r.
+00000ca0: 0000 00da 1469 735f 7475 6e6e 656c 5f63  .....is_tunnel_c
+00000cb0: 6f6e 6e65 6374 696f 6e96 0000 0073 0200  onnection....s..
+00000cc0: 0000 0001 724a 0000 0063 0100 0000 0000  ....rJ...c......
+00000cd0: 0000 0400 0000 0a00 0000 0300 0000 73a0  ..............s.
+00000ce0: 0000 0074 0088 0083 0173 0c64 0053 0074  ...t.....s.d.S.t
+00000cf0: 0188 0083 017d 0174 0288 007c 0183 0289  .....}.t...|....
+00000d00: 0174 036a 0464 016a 0588 0183 0183 0101  .t.j.d.j........
+00000d10: 0087 0087 0166 0264 0264 0384 087d 0274  .....f.d.d...}.t
+00000d20: 0688 0188 006a 0764 0483 0188 006a 0764  .....j.d.....j.d
+00000d30: 0583 0188 006a 0764 0683 0188 006a 0764  .....j.d.....j.d
+00000d40: 0783 016a 0864 0864 0983 0288 006a 0764  ...j.d.d.....j.d
+00000d50: 0a83 0188 006a 0764 0b83 017c 0264 0c8d  .....j.d...|.d..
+00000d60: 087d 037c 036a 0983 0001 0074 036a 0464  .}.|.j.....t.j.d
+00000d70: 0d6a 057c 036a 0a88 0183 0283 0101 007c  .j.|.j.........|
+00000d80: 0353 0029 0e4e 7a2a 5374 6172 7469 6e67  .S.).Nz*Starting
+00000d90: 2053 5348 2074 756e 6e65 6c20 666f 7220   SSH tunnel for 
+00000da0: 636f 6e6e 6563 7469 6f6e 2022 7b7d 222e  connection "{}".
+00000db0: 2e2e 6300 0000 0000 0000 0002 0000 0003  ..c.............
+00000dc0: 0000 0013 0000 0073 4400 0000 7400 8800  .......sD...t...
+00000dd0: 8301 7d00 7401 6a02 7c00 8301 7d01 7c01  ..}.t.j.|...}.|.
+00000de0: 7230 7403 6a04 6401 6a05 8801 8301 8301  r0t.j.d.j.......
+00000df0: 0100 7406 8800 8301 0100 6e10 7403 6a04  ..t.......n.t.j.
+00000e00: 6402 6a05 8801 8301 8301 0100 6400 5300  d.j.........d.S.
+00000e10: 2903 4e7a 2f53 5348 2074 756e 6e65 6c20  ).Nz/SSH tunnel 
+00000e20: 6973 2063 6c6f 7365 642c 2064 6973 706f  is closed, dispo
+00000e30: 7369 6e67 2063 6f6e 6e65 6374 696f 6e20  sing connection 
+00000e40: 227b 7d22 7a28 5353 4820 7475 6e6e 656c  "{}"z(SSH tunnel
+00000e50: 2069 7320 636c 6f73 6564 2066 6f72 2063   is closed for c
+00000e60: 6f6e 6e65 6374 696f 6e20 227b 7d22 2907  onnection "{}").
+00000e70: 7243 0000 0072 4400 0000 722b 0000 0072  rC...rD...r+...r
+00000e80: 1400 0000 da04 696e 666f 7230 0000 00da  ......infor0....
+00000e90: 1264 6973 706f 7365 5f63 6f6e 6e65 6374  .dispose_connect
+00000ea0: 696f 6e29 02da 0d63 6f6e 6e65 6374 696f  ion)...connectio
+00000eb0: 6e5f 6964 da0a 636f 6e6e 6563 7469 6f6e  n_id..connection
+00000ec0: 2902 7233 0000 00da 0f63 6f6e 6e65 6374  ).r3.....connect
+00000ed0: 696f 6e5f 6e61 6d65 7216 0000 0072 1700  ion_namer....r..
+00000ee0: 0000 da08 6f6e 5f63 6c6f 7365 cc00 0000  ....on_close....
+00000ef0: 730c 0000 0000 0108 010a 0204 0110 010a  s...............
+00000f00: 027a 2767 6574 5f63 6f6e 6e65 6374 696f  .z'get_connectio
+00000f10: 6e5f 7475 6e6e 656c 2e3c 6c6f 6361 6c73  n_tunnel.<locals
+00000f20: 3e2e 6f6e 5f63 6c6f 7365 723d 0000 0072  >.on_closer=...r
+00000f30: 3e00 0000 723f 0000 0072 4000 0000 7a02  >...r?...r@...z.
+00000f40: 5c6e da01 0a72 2600 0000 7227 0000 0029  \n...r&...r'...)
+00000f50: 0872 1a00 0000 723d 0000 0072 3e00 0000  .r....r=...r>...
+00000f60: 723f 0000 0072 4000 0000 5a0b 7265 6d6f  r?...r@...Z.remo
+00000f70: 7465 5f68 6f73 745a 0b72 656d 6f74 655f  te_hostZ.remote_
+00000f80: 706f 7274 7250 0000 007a 3153 5348 2074  portrP...z1SSH t
+00000f90: 756e 6e65 6c20 7374 6172 7465 6420 6f6e  unnel started on
+00000fa0: 2070 6f72 7420 7b7d 2066 6f72 2063 6f6e   port {} for con
+00000fb0: 6e65 6374 696f 6e20 227b 7d22 290b 724a  nection "{}").rJ
+00000fc0: 0000 00da 1567 6574 5f63 6f6e 6e65 6374  .....get_connect
+00000fd0: 696f 6e5f 7363 6865 6d61 da13 6765 745f  ion_schema..get_
+00000fe0: 636f 6e6e 6563 7469 6f6e 5f6e 616d 6572  connection_namer
+00000ff0: 1400 0000 724b 0000 0072 3000 0000 7206  ....rK...r0...r.
+00001000: 0000 0072 2b00 0000 da07 7265 706c 6163  ...r+.....replac
+00001010: 65da 0573 7461 7274 7231 0000 0029 0472  e..startr1...).r
+00001020: 3300 0000 7239 0000 0072 5000 0000 7234  3...r9...rP...r4
+00001030: 0000 0072 1600 0000 2902 7233 0000 0072  ...r....).r3...r
+00001040: 4f00 0000 7217 0000 00da 1567 6574 5f63  O...r......get_c
+00001050: 6f6e 6e65 6374 696f 6e5f 7475 6e6e 656c  onnection_tunnel
+00001060: 9a00 0000 7324 0000 0000 0108 0104 0208  ....s$..........
+00001070: 010a 2b10 020e 0a02 0102 0108 0108 0108  ..+.............
+00001080: 0110 0108 0108 0108 0208 0214 0272 5600  .............rV.
+00001090: 0000 6301 0000 0000 0000 0002 0000 0003  ..c.............
+000010a0: 0000 0043 0000 0073 4600 0000 7c00 6a00  ...C...sF...|.j.
+000010b0: 6401 8301 7222 7c00 6a00 6401 8301 6402  d...r"|.j.d...d.
+000010c0: 6b03 7222 7c00 6a00 6401 8301 6e02 6400  k.r"|.j.d...n.d.
+000010d0: 7d01 7c01 0c00 7242 7c00 6a00 6403 6402  }.|...rB|.j.d.d.
+000010e0: 8302 6a01 6404 8301 7242 6405 7d01 7c01  ..j.d...rBd.}.|.
+000010f0: 5300 2906 4e72 3900 0000 722a 0000 0072  S.).Nr9...r*...r
+00001100: 1900 0000 5a05 6d73 7371 6c5a 0364 626f  ....Z.mssqlZ.dbo
+00001110: 2902 722b 0000 00da 0a73 7461 7274 7377  ).r+.....startsw
+00001120: 6974 6829 0272 3300 0000 7239 0000 0072  ith).r3...r9...r
+00001130: 1600 0000 7216 0000 0072 1700 0000 7252  ....r....r....rR
+00001140: 0000 00e7 0000 0073 0800 0000 0001 2602  .......s......&.
+00001150: 1801 0402 7252 0000 0063 0200 0000 0000  ....rR...c......
+00001160: 0000 0500 0000 0600 0000 4300 0000 7372  ..........C...sr
+00001170: 0000 0064 017d 0274 0074 0069 007c 0083  ...d.}.t.t.i.|..
+00001180: 0264 027c 0269 0183 027d 0374 017c 0383  .d.|.i...}.t.|..
+00001190: 017d 047c 0472 307c 046a 027c 0264 0383  .}.|.r0|.j.|.d..
+000011a0: 027d 047c 0172 427c 0464 046a 037c 0183  .}.|.rB|.d.j.|..
+000011b0: 0137 007d 0474 047c 0083 0172 6e7c 0464  .7.}.t.|...rn|.d
+000011c0: 056a 037c 006a 0564 0683 017c 006a 0564  .j.|.j.d...|.j.d
+000011d0: 0783 017c 006a 0564 0883 0183 0337 007d  ...|.j.d.....7.}
+000011e0: 047c 0453 0029 094e 5a0f 5f5f 4a45 545f  .|.S.).NZ.__JET_
+000011f0: 4442 5f50 4153 535f 5f72 2000 0000 7a08  DB_PASS__r ...z.
+00001200: 2a2a 2a2a 2a2a 2a2a 7a03 3a7b 7d7a 0f20  ********z.:{}z. 
+00001210: 2876 6961 207b 7d40 7b7d 3a7b 7d29 723f  (via {}@{}:{})r?
+00001220: 0000 0072 3d00 0000 723e 0000 0029 0672  ...r=...r>...).r
+00001230: 1100 0000 7236 0000 0072 5400 0000 7230  ....r6...rT...r0
+00001240: 0000 0072 4a00 0000 722b 0000 0029 0572  ...rJ...r+...).r
+00001250: 3300 0000 7239 0000 005a 0e70 6173 7377  3...r9...Z.passw
+00001260: 6f72 645f 746f 6b65 6e5a 086c 6f67 5f63  ord_tokenZ.log_c
+00001270: 6f6e 6672 4f00 0000 7216 0000 0072 1600  onfrO...r....r..
+00001280: 0000 7217 0000 0072 5300 0000 f000 0000  ..r....rS.......
+00001290: 7314 0000 0000 0104 0114 0208 0104 010c  s...............
+000012a0: 0104 010e 0108 0124 0272 5300 0000 6302  .......$.rS...c.
+000012b0: 0000 0000 0000 0005 0000 000a 0000 0043  ...............C
+000012c0: 0000 0073 8a00 0000 7c00 7400 6b07 720c  ...s....|.t.k.r.
+000012d0: 6400 5300 7400 7c00 1900 7d02 7401 6a02  d.S.t.|...}.t.j.
+000012e0: 6401 6a03 7c01 8301 8301 0100 7c02 6402  d.j.|.......|.d.
+000012f0: 1900 7d03 7c03 8f20 0100 7404 6403 6404  ..}.|.. ..t.d.d.
+00001300: 8d01 6a05 8300 7d04 7c03 6a06 7c04 6405  ..j...}.|.j.|.d.
+00001310: 8d01 0100 5700 6400 5100 5200 5800 7c00  ....W.d.Q.R.X.|.
+00001320: 7407 6b06 7276 7401 6a02 6406 6a03 7c01  t.k.rvt.j.d.j.|.
+00001330: 8301 8301 0100 7407 7c00 1900 5300 7401  ......t.|...S.t.
+00001340: 6a02 6407 6a03 7c01 8301 8301 0100 6400  j.d.j.|.......d.
+00001350: 5300 2908 4e7a 2357 6169 7469 6e67 2064  S.).Nz#Waiting d
+00001360: 6174 6162 6173 6520 636f 6e6e 6563 7469  atabase connecti
+00001370: 6f6e 2022 7b7d 222e 2e2e da09 636f 6e6e  on "{}".....conn
+00001380: 6563 7465 64e9 0a00 0000 2901 da07 6d69  ected.....)...mi
+00001390: 6e75 7465 7329 01da 0774 696d 656f 7574  nutes)...timeout
+000013a0: 7a1e 466f 756e 6420 6461 7461 6261 7365  z.Found database
+000013b0: 2063 6f6e 6e65 6374 696f 6e20 227b 7d22   connection "{}"
+000013c0: 7a22 4e6f 7420 666f 756e 6420 6461 7461  z"Not found data
+000013d0: 6261 7365 2063 6f6e 6e65 6374 696f 6e20  base connection 
+000013e0: 227b 7d22 2908 da13 7065 6e64 696e 675f  "{}")...pending_
+000013f0: 636f 6e6e 6563 7469 6f6e 7372 1400 0000  connectionsr....
+00001400: 724b 0000 0072 3000 0000 7202 0000 00da  rK...r0...r.....
+00001410: 0d74 6f74 616c 5f73 6563 6f6e 6473 da04  .total_seconds..
+00001420: 7761 6974 7244 0000 0029 0572 4d00 0000  waitrD...).rM...
+00001430: 724f 0000 00da 1270 656e 6469 6e67 5f63  rO.....pending_c
+00001440: 6f6e 6e65 6374 696f 6eda 1363 6f6e 6e65  onnection..conne
+00001450: 6374 6564 5f63 6f6e 6469 7469 6f6e 725b  cted_conditionr[
+00001460: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00001470: 0000 da17 7761 6974 5f70 656e 6469 6e67  ....wait_pending
+00001480: 5f63 6f6e 6e65 6374 696f 6eff 0000 0073  _connection....s
+00001490: 1800 0000 0001 0801 0402 0802 1002 0801  ................
+000014a0: 0601 0e01 1602 0801 1001 0802 7261 0000  ............ra..
+000014b0: 0063 0200 0000 0000 0000 0600 0000 0800  .c..............
+000014c0: 0000 4300 0000 7316 0100 0074 007c 007c  ..C...s....t.|.|
+000014d0: 0183 027d 027c 0273 1674 0164 0183 0182  ...}.|.s.t.d....
+000014e0: 017c 006a 0264 0283 0164 036b 0272 2c74  .|.j.d...d.k.r,t
+000014f0: 037c 0283 0153 007c 006a 0264 0283 0164  .|...S.|.j.d...d
+00001500: 046b 0272 a869 007d 037c 006a 0264 0583  .k.r.i.}.|.j.d..
+00001510: 017c 006a 0264 0683 017c 006a 0264 0783  .|.j.d...|.j.d..
+00001520: 0164 089c 037d 0474 0474 0574 0664 0964  .d...}.t.t.t.d.d
+00001530: 0a84 007c 046a 0783 0083 0283 0183 017d  ...|.j.........}
+00001540: 0574 087c 0583 0172 867c 057c 0364 0b3c  .t.|...r.|.|.d.<
+00001550: 0074 037c 027c 006a 0264 0c83 0164 0d64  .t.|.|.j.d...d.d
+00001560: 0e64 0f64 1064 1169 017c 0396 0264 128d  .d.d.d.i.|...d..
+00001570: 0653 007c 006a 0264 0283 0164 136b 0272  .S.|.j.d...d.k.r
+00001580: ce74 037c 027c 006a 0264 0c83 0164 0d64  .t.|.|.j.d...d.d
+00001590: 0e64 0f64 148d 0553 007c 006a 0264 0283  .d.d...S.|.j.d..
+000015a0: 0164 156b 0272 f474 037c 027c 006a 0264  .d.k.r.t.|.|.j.d
+000015b0: 0c83 0164 0d64 0e64 0f64 148d 0553 0074  ...d.d.d.d...S.t
+000015c0: 037c 027c 006a 0264 0c83 0164 0d64 0e64  .|.|.j.d...d.d.d
+000015d0: 0f64 1064 1169 0164 128d 0653 0064 0053  .d.d.i.d...S.d.S
+000015e0: 0029 164e 7a21 4461 7461 6261 7365 2063  .).Nz!Database c
+000015f0: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
+00001600: 6e6f 7420 7365 7472 1900 0000 721b 0000  not setr....r...
+00001610: 0072 2900 0000 723a 0000 0072 3b00 0000  .r)...r:...r;...
+00001620: 723c 0000 0029 03da 0263 61da 0463 6572  r<...)...ca..cer
+00001630: 74da 036b 6579 6301 0000 0000 0000 0001  t..keyc.........
+00001640: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
+00001650: 7c00 6401 1900 5300 2902 4ee9 0100 0000  |.d...S.).N.....
+00001660: 7216 0000 0029 0172 4600 0000 7216 0000  r....).rF...r...
+00001670: 0072 1600 0000 7217 0000 0072 4700 0000  .r....r....rG...
+00001680: 2201 0000 7300 0000 007a 2a63 7265 6174  "...s....z*creat
+00001690: 655f 636f 6e6e 6563 7469 6f6e 5f65 6e67  e_connection_eng
+000016a0: 696e 652e 3c6c 6f63 616c 733e 2e3c 6c61  ine.<locals>.<la
+000016b0: 6d62 6461 3eda 0373 736c 7244 0000 0054  mbda>..sslrD...T
+000016c0: 7265 0000 0069 2c01 0000 da0f 636f 6e6e  re...i,.....conn
+000016d0: 6563 745f 7469 6d65 6f75 74e9 0500 0000  ect_timeout.....
+000016e0: 2905 da09 706f 6f6c 5f73 697a 65da 0d70  )...pool_size..p
+000016f0: 6f6f 6c5f 7072 655f 7069 6e67 da0c 6d61  ool_pre_ping..ma
+00001700: 785f 6f76 6572 666c 6f77 da0c 706f 6f6c  x_overflow..pool
+00001710: 5f72 6563 7963 6c65 da0c 636f 6e6e 6563  _recycle..connec
+00001720: 745f 6172 6773 721f 0000 0029 0472 6900  t_argsr....).ri.
+00001730: 0000 726a 0000 0072 6b00 0000 726c 0000  ..rj...rk...rl..
+00001740: 0072 2800 0000 2909 7236 0000 00da 0945  .r(...).r6.....E
+00001750: 7863 6570 7469 6f6e 722b 0000 0072 0c00  xceptionr+...r..
+00001760: 0000 da04 6469 6374 da04 6c69 7374 da06  ....dict..list..
+00001770: 6669 6c74 6572 da05 6974 656d 73da 036c  filter..items..l
+00001780: 656e 2906 7233 0000 0072 3400 0000 5a0a  en).r3...r4...Z.
+00001790: 656e 6769 6e65 5f75 726c 726d 0000 0072  engine_urlrm...r
+000017a0: 6600 0000 5a07 7373 6c5f 7365 7472 1600  f...Z.ssl_setr..
+000017b0: 0000 7216 0000 0072 1700 0000 da18 6372  ..r....r......cr
+000017c0: 6561 7465 5f63 6f6e 6e65 6374 696f 6e5f  eate_connection_
+000017d0: 656e 6769 6e65 1301 0000 7354 0000 0000  engine....sT....
+000017e0: 010a 0204 0108 020e 0108 010e 0104 0208  ................
+000017f0: 0108 010e 021a 0208 0108 0202 0102 0108  ................
+00001800: 0102 0102 0102 0206 010a 030e 0102 0102  ................
+00001810: 0108 0102 0102 0108 020e 0102 0102 0108  ................
+00001820: 0102 0102 0108 0302 0102 0108 0102 0102  ................
+00001830: 0102 0172 7400 0000 6301 0000 0000 0000  ...rt...c.......
+00001840: 0002 0000 0003 0000 0003 0000 0073 1000  .............s..
+00001850: 0000 8700 6601 6401 6402 8408 7d01 7c01  ....f.d.d...}.|.
+00001860: 5300 2903 4e63 0200 0000 0000 0000 0200  S.).Nc..........
+00001870: 0000 0300 0000 1300 0000 7344 0000 0088  ..........sD....
+00001880: 006a 0064 0183 0164 006b 0972 207c 0088  .j.d...d.k.r |..
+00001890: 006a 0064 0183 016b 0772 2064 0253 0088  .j.d...k.r d.S..
+000018a0: 006a 0064 0383 0164 006b 0972 407c 0088  .j.d...d.k.r@|..
+000018b0: 006a 0064 0383 016b 0672 4064 0253 0064  .j.d...k.r@d.S.d
+000018c0: 0453 0029 054e 7237 0000 0046 7238 0000  .S.).Nr7...Fr8..
+000018d0: 0054 2901 722b 0000 0029 02da 0574 6162  .T).r+...)...tab
+000018e0: 6c65 da04 6d65 7461 2901 7233 0000 0072  le..meta).r3...r
+000018f0: 1600 0000 7217 0000 0072 3700 0000 4e01  ....r....r7...N.
+00001900: 0000 730a 0000 0000 011c 0104 011c 0104  ..s.............
+00001910: 017a 2b67 6574 5f63 6f6e 6e65 6374 696f  .z+get_connectio
+00001920: 6e5f 6f6e 6c79 5f70 7265 6469 6361 7465  n_only_predicate
+00001930: 2e3c 6c6f 6361 6c73 3e2e 6f6e 6c79 7216  .<locals>.onlyr.
+00001940: 0000 0029 0272 3300 0000 7237 0000 0072  ...).r3...r7...r
+00001950: 1600 0000 2901 7233 0000 0072 1700 0000  ....).r3...r....
+00001960: da1d 6765 745f 636f 6e6e 6563 7469 6f6e  ..get_connection
+00001970: 5f6f 6e6c 795f 7072 6564 6963 6174 654d  _only_predicateM
+00001980: 0100 0073 0400 0000 0001 0c06 7277 0000  ...s........rw..
+00001990: 0063 0100 0000 0000 0000 1d00 0000 2300  .c............#.
+000019a0: 0000 4300 0000 73e0 0200 0074 007c 0083  ..C...s....t.|..
+000019b0: 017d 0174 017c 0083 017d 027c 0174 026b  .}.t.|...}.|.t.k
+000019c0: 0672 3874 027c 0119 0064 0119 007c 026b  .r8t.|...d...|.k
+000019d0: 0272 3074 027c 0119 0053 0074 037c 0083  .r0t.|...S.t.|..
+000019e0: 0101 0074 047c 0083 017d 0374 057c 007c  ...t.|...}.t.|.|
+000019f0: 0383 027d 0474 067c 017c 0483 027d 057c  ...}.t.|.|...}.|
+00001a00: 0572 5c7c 0553 0074 076a 0883 007d 067c  .r\|.S.t.j...}.|
+00001a10: 0164 0064 0285 0219 007d 0774 096a 0a83  .d.d.....}.t.j..
+00001a20: 007d 0874 0b64 0383 017d 097c 097c 047c  .}.t.d...}.|.|.|
+00001a30: 006a 0c64 0483 017c 006a 0c64 0583 017c  .j.d...|.j.d...|
+00001a40: 066a 0d83 007c 0864 069c 067d 0a7c 0a74  .j...|.d...}.|.t
+00001a50: 0e7c 013c 0064 007d 0b90 017a ec90 0179  .|.<.d.}...z...y
+00001a60: ae74 0f7c 0083 017d 0b7c 0b7c 0a64 073c  .t.|...}.|.|.d.<
+00001a70: 0074 107c 007c 0b83 027d 0c7c 0c7c 0a64  .t.|.|...}.|.|.d
+00001a80: 083c 0074 1174 127c 0c64 098d 0183 017d  .<.t.t.|.d.....}
+00001a90: 0d7c 0d83 007d 0e74 136a 1464 0a6a 157c  .|...}.t.j.d.j.|
+00001aa0: 077c 0483 0283 0101 0074 166a 1683 007d  .|.......t.j...}
+00001ab0: 0f7c 0e6a 1783 0090 018f 3e7d 1074 166a  .|.j......>}.t.j
+00001ac0: 1683 007d 1174 187c 117c 0f18 0064 0b83  ...}.t.|.|...d..
+00001ad0: 027d 1274 136a 1464 0c6a 157c 077c 0483  .}.t.j.d.j.|.|..
+00001ae0: 0283 0101 0074 197c 0e83 017d 1374 136a  .....t.|...}.t.j
+00001af0: 1464 0d6a 157c 077c 0483 0283 0101 0074  .d.j.|.|.......t
+00001b00: 166a 1683 007d 1474 1a7c 037c 1064 0e8d  .j...}.t.|.|.d..
+00001b10: 027d 1574 1b7c 0083 017d 1674 1c7c 077c  .}.t.|...}.t.|.|
+00001b20: 157c 0c7c 167c 0a64 0f64 108d 0601 0074  .|.|.|.d.d.....t
+00001b30: 166a 1683 007d 1774 187c 177c 1418 0064  .j...}.t.|.|...d
+00001b40: 0b83 027d 1874 136a 1464 116a 157c 077c  ...}.t.j.d.j.|.|
+00001b50: 0474 1d83 0083 0383 0101 0074 1e7c 1564  .t.........t.|.d
+00001b60: 128d 017d 1974 1f7c 1983 0101 0078 4a7c  ...}.t.|.....xJ|
+00001b70: 196a 206a 216a 2283 0044 005d 3a5c 027d  .j j!j"..D.]:\.}
+00001b80: 1a7d 1b74 237c 1b6a 246a 2583 0164 136b  .}.t#|.j$j%..d.k
+00001b90: 0290 0172 d07c 1a7c 196a 266b 0790 0172  ...r.|.|.j&k...r
+00001ba0: d074 136a 2764 146a 157c 077c 1a83 0283  .t.j'd.j.|.|....
+00001bb0: 0101 0090 0171 d057 007c 017c 047c 0c7c  .....q.W.|.|.|.|
+00001bc0: 0d7c 197c 027c 137c 0b69 0074 096a 2883  .|.|.|.|.i.t.j(.
+00001bd0: 007c 006a 0c64 0483 017c 006a 0c64 0583  .|.j.d...|.j.d..
+00001be0: 017c 066a 0d83 007c 127c 1864 159c 0f74  .|.j...|.|.d...t
+00001bf0: 027c 013c 0057 0064 0051 0052 0058 007c  .|.<.W.d.Q.R.X.|
+00001c00: 0e6a 2983 0001 0074 027c 0119 0053 0004  .j)....t.|...S..
+00001c10: 0074 2a6b 0a90 0272 9801 007d 1c01 007a  .t*k...r...}...z
+00001c20: 187c 0b90 0272 847c 0b6a 2983 0001 007c  .|...r.|.j)....|
+00001c30: 1c82 0157 0059 0064 0064 007d 1c7e 1c58  ...W.Y.d.d.}.~.X
+00001c40: 006e 0258 0057 0064 007c 0174 0e6b 0690  .n.X.W.d.|.t.k..
+00001c50: 0272 c274 0e7c 0119 006a 0c64 1683 017c  .r.t.|...j.d...|
+00001c60: 096b 0290 0272 c274 0e7c 013d 007c 088f  .k...r.t.|.=.|..
+00001c70: 0e01 007c 086a 2b83 0001 0057 0064 0051  ...|.j+....W.d.Q
+00001c80: 0052 0058 0058 0064 0053 0029 174e da09  .R.X.X.d.S.).N..
+00001c90: 7061 7261 6d73 5f69 64e9 0400 0000 e920  params_id...... 
+00001ca0: 0000 00da 0770 726f 6a65 6374 da05 746f  .....project..to
+00001cb0: 6b65 6e29 06da 0269 6472 1a00 0000 727b  ken)...idr....r{
+00001cc0: 0000 0072 7c00 0000 da0a 696e 6974 5f73  ...r|.....init_s
+00001cd0: 7461 7274 7258 0000 0072 3400 0000 7219  tartrX...r4...r.
+00001ce0: 0000 0029 01da 0462 696e 647a 235b 7b7d  ...)...bindz#[{}
+00001cf0: 5d20 436f 6e6e 6563 7469 6e67 2074 6f20  ] Connecting to 
+00001d00: 6461 7461 6261 7365 2022 7b7d 222e 2e2e  database "{}"...
+00001d10: e903 0000 007a 215b 7b7d 5d20 4765 7474  .....z![{}] Gett
+00001d20: 696e 6720 6462 2074 7970 6573 2066 6f72  ing db types for
+00001d30: 2022 7b7d 222e 2e2e 7a1f 5b7b 7d5d 2047   "{}"...z.[{}] G
+00001d40: 6574 7469 6e67 2073 6368 656d 6120 666f  etting schema fo
+00001d50: 7220 227b 7d22 2e2e 2e29 0272 3900 0000  r "{}"...).r9...
+00001d60: 727f 0000 0054 2903 7237 0000 0072 5f00  r....T).r7...r_.
+00001d70: 0000 5a05 7669 6577 737a 1f5b 7b7d 5d20  ..Z.viewsz.[{}] 
+00001d80: 436f 6e6e 6563 7465 6420 746f 2022 7b7d  Connected to "{}
+00001d90: 2220 284d 656d 3a7b 7d29 2901 da08 6d65  " (Mem:{}))...me
+00001da0: 7461 6461 7461 7201 0000 007a 3d5b 7b7d  tadatar....z=[{}
+00001db0: 5d20 5461 626c 6520 227b 7d22 2064 6f65  ] Table "{}" doe
+00001dc0: 7320 6e6f 7420 6861 7665 2070 7269 6d61  s not have prima
+00001dd0: 7279 206b 6579 2061 6e64 2077 696c 6c20  ry key and will 
+00001de0: 6265 2069 676e 6f72 6564 290f 727d 0000  be ignored).r}..
+00001df0: 0072 1a00 0000 7219 0000 00da 0753 6573  .r....r......Ses
+00001e00: 7369 6f6e da0a 4d61 7070 6564 4261 7365  sion..MappedBase
+00001e10: 7278 0000 00da 1574 7970 655f 636f 6465  rx.....type_code
+00001e20: 5f74 6f5f 7371 6c5f 7479 7065 7234 0000  _to_sql_typer4..
+00001e30: 00da 0563 6163 6865 da04 6c6f 636b 727b  ...cache..lockr{
+00001e40: 0000 0072 7c00 0000 727e 0000 00da 0c63  ...r|...r~.....c
+00001e50: 6f6e 6e65 6374 5f74 696d 65da 0c72 6566  onnect_time..ref
+00001e60: 6c65 6374 5f74 696d 6572 7d00 0000 292c  lect_timer}...),
+00001e70: 7243 0000 0072 4500 0000 7244 0000 0072  rC...rE...rD...r
+00001e80: 4c00 0000 7252 0000 0072 5300 0000 7261  L...rR...rS...ra
+00001e90: 0000 0072 0300 0000 da03 6e6f 77da 0974  ...r......now..t
+00001ea0: 6872 6561 6469 6e67 da09 436f 6e64 6974  hreading..Condit
+00001eb0: 696f 6e72 1000 0000 722b 0000 00da 0969  ionr....r+.....i
+00001ec0: 736f 666f 726d 6174 725c 0000 0072 5600  soformatr\...rV.
+00001ed0: 0000 7274 0000 0072 0f00 0000 720e 0000  ..rt...r....r...
+00001ee0: 0072 1400 0000 724b 0000 0072 3000 0000  .r....rK...r0...
+00001ef0: da04 7469 6d65 724e 0000 00da 0572 6f75  ..timerN.....rou
+00001f00: 6e64 7209 0000 0072 0d00 0000 7277 0000  ndr....r....rw..
+00001f10: 0072 0500 0000 7208 0000 0072 0400 0000  .r....r....r....
+00001f20: da10 6c6f 6164 5f6d 6170 7065 645f 6261  ..load_mapped_ba
+00001f30: 7365 7281 0000 005a 0674 6162 6c65 7372  ser....Z.tablesr
+00001f40: 7200 0000 7273 0000 005a 0b70 7269 6d61  r...rs...Z.prima
+00001f50: 7279 5f6b 6579 da07 636f 6c75 6d6e 73da  ry_key..columns.
+00001f60: 0763 6c61 7373 6573 da07 7761 726e 696e  .classes..warnin
+00001f70: 67da 044c 6f63 6bda 0563 6c6f 7365 726e  g..Lock..closern
+00001f80: 0000 00da 0a6e 6f74 6966 795f 616c 6c29  .....notify_all)
+00001f90: 1d72 3300 0000 724d 0000 005a 1463 6f6e  .r3...rM...Z.con
+00001fa0: 6e65 6374 696f 6e5f 7061 7261 6d73 5f69  nection_params_i
+00001fb0: 6472 3900 0000 724f 0000 005a 1365 7869  dr9...rO...Z.exi
+00001fc0: 7374 696e 675f 636f 6e6e 6563 7469 6f6e  sting_connection
+00001fd0: 727e 0000 005a 0869 645f 7368 6f72 7472  r~...Z.id_shortr
+00001fe0: 6000 0000 5a15 7065 6e64 696e 675f 636f  `...Z.pending_co
+00001ff0: 6e6e 6563 7469 6f6e 5f69 6472 5f00 0000  nnection_idr_...
+00002000: 7234 0000 0072 1900 0000 7282 0000 00da  r4...r....r.....
+00002010: 0773 6573 7369 6f6e 5a0d 636f 6e6e 6563  .sessionZ.connec
+00002020: 745f 7374 6172 7472 4e00 0000 5a0b 636f  t_startrN...Z.co
+00002030: 6e6e 6563 745f 656e 6472 8700 0000 7284  nnect_endr....r.
+00002040: 0000 005a 0d72 6566 6c65 6374 5f73 7461  ...Z.reflect_sta
+00002050: 7274 7281 0000 0072 3700 0000 5a0b 7265  rtr....r7...Z.re
+00002060: 666c 6563 745f 656e 6472 8800 0000 7283  flect_endr....r.
+00002070: 0000 005a 0a74 6162 6c65 5f6e 616d 6572  ...Z.table_namer
+00002080: 7500 0000 da01 6572 1600 0000 7216 0000  u.....er....r...
+00002090: 0072 1700 0000 da10 636f 6e6e 6563 745f  .r......connect_
+000020a0: 6461 7461 6261 7365 5701 0000 7396 0000  databaseW...s...
+000020b0: 0000 0308 0108 0208 0110 0108 0208 0208  ................
+000020c0: 010a 020a 0104 0104 0208 020c 0108 0108  ................
+000020d0: 0202 0102 0108 0108 0106 0108 0308 0104  ................
+000020e0: 0208 0108 0108 020a 0108 020e 0106 0212  ................
+000020f0: 0208 010c 0108 010e 0212 0108 0212 0208  ................
+00002100: 020c 0108 0114 0208 010e 0216 020a 0108  ................
+00002110: 0216 011e 0118 0302 0102 0102 0102 0102  ................
+00002120: 0102 0102 0102 0102 0106 0108 0108 0106  ................
+00002130: 0102 0116 0308 0208 0112 0106 0108 021a  ................
+00002140: 021e 0106 0206 0172 9800 0000 6301 0000  .......r....c...
+00002150: 0000 0000 0001 0000 000b 0000 0043 0000  .............C..
+00002160: 0073 4000 0000 7926 7c00 6401 1900 6a00  .s@...y&|.d...j.
+00002170: 8300 0100 7c00 6a01 6402 8301 7224 7c00  ....|.j.d...r$|.
+00002180: 6402 1900 6a02 8300 0100 6403 5300 0400  d...j.....d.S...
+00002190: 7403 6b0a 723a 0100 0100 0100 6404 5300  t.k.r:......d.S.
+000021a0: 5800 6400 5300 2905 4e72 1900 0000 7234  X.d.S.).Nr....r4
+000021b0: 0000 0054 4629 04da 0764 6973 706f 7365  ...TF)...dispose
+000021c0: 722b 0000 0072 9400 0000 726e 0000 0029  r+...r....rn...)
+000021d0: 0172 4e00 0000 7216 0000 0072 1600 0000  .rN...r....r....
+000021e0: 7217 0000 00da 1964 6973 706f 7365 5f63  r......dispose_c
+000021f0: 6f6e 6e65 6374 696f 6e5f 6f62 6a65 6374  onnection_object
+00002200: c501 0000 730e 0000 0000 0102 010c 020a  ....s...........
+00002210: 010c 0204 010e 0172 9a00 0000 6301 0000  .......r....c...
+00002220: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+00002230: 0073 2c00 0000 7400 7c00 8301 7d01 7401  .s,...t.|...}.t.
+00002240: 6a02 7c01 8301 7d02 7c02 7228 7403 7c02  j.|...}.|.r(t.|.
+00002250: 8301 7228 7401 7c01 3d00 6401 5300 6402  ..r(t.|.=.d.S.d.
+00002260: 5300 2903 4e54 4629 0472 4300 0000 7244  S.).NTF).rC...rD
+00002270: 0000 0072 2b00 0000 729a 0000 0029 0372  ...r+...r....).r
+00002280: 3300 0000 724d 0000 0072 4e00 0000 7216  3...rM...rN...r.
+00002290: 0000 0072 1600 0000 7217 0000 0072 4c00  ...r....r....rL.
+000022a0: 0000 d101 0000 730c 0000 0000 0308 010a  ......s.........
+000022b0: 020c 0106 0104 0272 4c00 0000 6301 0000  .......rL...c...
+000022c0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000022d0: 0073 0c00 0000 7400 7401 7c00 8301 8301  .s....t.t.|.....
+000022e0: 5300 2901 4e29 0272 4c00 0000 da08 6765  S.).N).rL.....ge
+000022f0: 745f 636f 6e66 2901 da07 7265 7175 6573  t_conf)...reques
+00002300: 7472 1600 0000 7216 0000 0072 1700 0000  tr....r....r....
+00002310: da1a 6469 7370 6f73 655f 7265 7175 6573  ..dispose_reques
+00002320: 745f 636f 6e6e 6563 7469 6f6e de01 0000  t_connection....
+00002330: 7302 0000 0000 0172 9d00 0000 6300 0000  s......r....c...
+00002340: 0000 0000 0000 0000 0015 0000 0043 0000  .............C..
+00002350: 0073 5600 0000 7400 6a01 7400 6a02 7400  .sV...t.j.t.j.t.
+00002360: 6a03 7400 6a04 7400 6a05 7400 6a06 7400  j.t.j.t.j.t.j.t.
+00002370: 6a07 7400 6a08 7400 6a09 7400 6a0a 7400  j.t.j.t.j.t.j.t.
+00002380: 6a0b 7400 6a0c 7400 6a0d 7400 6a0e 7400  j.t.j.t.j.t.j.t.
+00002390: 6a0f 7400 6a10 7400 6a11 7400 6a12 7400  j.t.j.t.j.t.j.t.
+000023a0: 6a13 7400 6a14 6401 9c14 5300 2902 4e29  j.t.j.d...S.).N)
+000023b0: 1472 1900 0000 7226 0000 0072 2700 0000  .r....r&...r'...
+000023c0: 721a 0000 0072 2300 0000 7220 0000 0072  r....r#...r ...r
+000023d0: 1d00 0000 7244 0000 0072 3700 0000 7238  ....rD...r7...r8
+000023e0: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
+000023f0: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+00002400: 0072 3f00 0000 7240 0000 0072 7b00 0000  .r?...r@...r{...
+00002410: 727c 0000 0029 1572 1300 0000 da0f 4441  r|...).r......DA
+00002420: 5441 4241 5345 5f45 4e47 494e 45da 0d44  TABASE_ENGINE..D
+00002430: 4154 4142 4153 455f 484f 5354 da0d 4441  ATABASE_HOST..DA
+00002440: 5441 4241 5345 5f50 4f52 54da 0d44 4154  TABASE_PORT..DAT
+00002450: 4142 4153 455f 4e41 4d45 da0d 4441 5441  ABASE_NAME..DATA
+00002460: 4241 5345 5f55 5345 52da 1144 4154 4142  BASE_USER..DATAB
+00002470: 4153 455f 5041 5353 574f 5244 da0e 4441  ASE_PASSWORD..DA
+00002480: 5441 4241 5345 5f45 5854 5241 da14 4441  TABASE_EXTRA..DA
+00002490: 5441 4241 5345 5f43 4f4e 4e45 4354 494f  TABASE_CONNECTIO
+000024a0: 4e53 da0d 4441 5441 4241 5345 5f4f 4e4c  NS..DATABASE_ONL
+000024b0: 59da 0f44 4154 4142 4153 455f 4558 4345  Y..DATABASE_EXCE
+000024c0: 5054 da0f 4441 5441 4241 5345 5f53 4348  PT..DATABASE_SCH
+000024d0: 454d 41da 0f44 4154 4142 4153 455f 5353  EMA..DATABASE_SS
+000024e0: 4c5f 4341 da11 4441 5441 4241 5345 5f53  L_CA..DATABASE_S
+000024f0: 534c 5f43 4552 54da 1044 4154 4142 4153  SL_CERT..DATABAS
+00002500: 455f 5353 4c5f 4b45 59da 1144 4154 4142  E_SSL_KEY..DATAB
+00002510: 4153 455f 5353 485f 484f 5354 da11 4441  ASE_SSH_HOST..DA
+00002520: 5441 4241 5345 5f53 5348 5f50 4f52 54da  TABASE_SSH_PORT.
+00002530: 1144 4154 4142 4153 455f 5353 485f 5553  .DATABASE_SSH_US
+00002540: 4552 da18 4441 5441 4241 5345 5f53 5348  ER..DATABASE_SSH
+00002550: 5f50 5249 5641 5445 5f4b 4559 da07 5052  _PRIVATE_KEY..PR
+00002560: 4f4a 4543 54da 0554 4f4b 454e 7216 0000  OJECT..TOKENr...
+00002570: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00002580: da11 6765 745f 7365 7474 696e 6773 5f63  ..get_settings_c
+00002590: 6f6e 66e2 0100 0073 2800 0000 0002 0401  onf....s(.......
+000025a0: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+000025b0: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+000025c0: 0401 0401 72b2 0000 0063 0100 0000 0000  ....r....c......
+000025d0: 0000 0200 0000 1500 0000 4300 0000 73ba  ..........C...s.
+000025e0: 0000 007c 006a 0083 007d 017c 0173 1064  ...|.j...}.|.s.d
+000025f0: 0053 007c 016a 0164 0183 017c 016a 0164  .S.|.j.d...|.j.d
+00002600: 0283 017c 016a 0164 0383 017c 016a 0164  ...|.j.d...|.j.d
+00002610: 0483 017c 016a 0164 0583 017c 016a 0164  ...|.j.d...|.j.d
+00002620: 0683 017c 016a 0164 0783 017c 016a 0164  ...|.j.d...|.j.d
+00002630: 0874 026a 0383 027c 016a 0164 0983 017c  .t.j...|.j.d...|
+00002640: 016a 0164 0a83 017c 016a 0164 0b83 017c  .j.d...|.j.d...|
+00002650: 016a 0164 0c83 017c 016a 0164 0d83 017c  .j.d...|.j.d...|
+00002660: 016a 0164 0e83 017c 016a 0164 0f83 017c  .j.d...|.j.d...|
+00002670: 016a 0164 1083 017c 016a 0164 1183 017c  .j.d...|.j.d...|
+00002680: 016a 0164 1283 017c 016a 0164 1383 017c  .j.d...|.j.d...|
+00002690: 016a 0164 1483 0164 159c 1453 0029 164e  .j.d...d...S.).N
+000026a0: da0f 6461 7461 6261 7365 5f65 6e67 696e  ..database_engin
+000026b0: 65da 0d64 6174 6162 6173 655f 686f 7374  e..database_host
+000026c0: da0d 6461 7461 6261 7365 5f70 6f72 74da  ..database_port.
+000026d0: 0d64 6174 6162 6173 655f 6e61 6d65 da0d  .database_name..
+000026e0: 6461 7461 6261 7365 5f75 7365 72da 1164  database_user..d
+000026f0: 6174 6162 6173 655f 7061 7373 776f 7264  atabase_password
+00002700: da0e 6461 7461 6261 7365 5f65 7874 7261  ..database_extra
+00002710: 5a14 6461 7461 6261 7365 5f63 6f6e 6e65  Z.database_conne
+00002720: 6374 696f 6e73 da0d 6461 7461 6261 7365  ctions..database
+00002730: 5f6f 6e6c 79da 0f64 6174 6162 6173 655f  _only..database_
+00002740: 6578 6365 7074 da0f 6461 7461 6261 7365  except..database
+00002750: 5f73 6368 656d 61da 0f64 6174 6162 6173  _schema..databas
+00002760: 655f 7373 6c5f 6361 da11 6461 7461 6261  e_ssl_ca..databa
+00002770: 7365 5f73 736c 5f63 6572 74da 1064 6174  se_ssl_cert..dat
+00002780: 6162 6173 655f 7373 6c5f 6b65 79da 1164  abase_ssl_key..d
+00002790: 6174 6162 6173 655f 7373 685f 686f 7374  atabase_ssh_host
+000027a0: da11 6461 7461 6261 7365 5f73 7368 5f70  ..database_ssh_p
+000027b0: 6f72 74da 1164 6174 6162 6173 655f 7373  ort..database_ss
+000027c0: 685f 7573 6572 da18 6461 7461 6261 7365  h_user..database
+000027d0: 5f73 7368 5f70 7269 7661 7465 5f6b 6579  _ssh_private_key
+000027e0: 727b 0000 0072 7c00 0000 2914 7219 0000  r{...r|...).r...
+000027f0: 0072 2600 0000 7227 0000 0072 1a00 0000  .r&...r'...r....
+00002800: 7223 0000 0072 2000 0000 721d 0000 0072  r#...r ...r....r
+00002810: 4400 0000 7237 0000 0072 3800 0000 7239  D...r7...r8...r9
+00002820: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
+00002830: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
+00002840: 0072 4000 0000 727b 0000 0072 7c00 0000  .r@...r{...r|...
+00002850: 2904 5a13 6765 745f 6272 6964 6765 5f73  ).Z.get_bridge_s
+00002860: 6574 7469 6e67 7372 2b00 0000 7213 0000  ettingsr+...r...
+00002870: 0072 a500 0000 2902 729c 0000 005a 0f62  .r....).r....Z.b
+00002880: 7269 6467 655f 7365 7474 696e 6773 7216  ridge_settingsr.
+00002890: 0000 0072 1600 0000 7217 0000 00da 1067  ...r....r......g
+000028a0: 6574 5f72 6571 7565 7374 5f63 6f6e 66fb  et_request_conf.
+000028b0: 0100 0073 2e00 0000 0001 0802 0401 0403  ...s............
+000028c0: 0801 0801 0801 0801 0801 0801 0801 0c01  ................
+000028d0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+000028e0: 0801 0801 0801 72c4 0000 0063 0100 0000  ......r....c....
+000028f0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00002900: 731a 0000 0074 007c 0083 017d 017c 0172  s....t.|...}.|.r
+00002910: 107c 0153 0074 0183 0053 0064 0053 0029  .|.S.t...S.d.S.)
+00002920: 014e 2902 72c4 0000 0072 b200 0000 2902  .N).r....r....).
+00002930: 729c 0000 005a 0c72 6571 7565 7374 5f63  r....Z.request_c
+00002940: 6f6e 6672 1600 0000 7216 0000 0072 1700  onfr....r....r..
+00002950: 0000 729b 0000 0019 0200 0073 0800 0000  ..r........s....
+00002960: 0001 0802 0401 0402 729b 0000 0063 0100  ........r....c..
+00002970: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
+00002980: 0000 731a 0000 0074 007c 0083 017d 0174  ..s....t.|...}.t
+00002990: 017c 0183 017d 0274 026a 037c 0283 0153  .|...}.t.j.|...S
+000029a0: 0029 014e 2904 729b 0000 0072 4300 0000  .).N).r....rC...
+000029b0: 7244 0000 0072 2b00 0000 2903 729c 0000  rD...r+...).r...
+000029c0: 0072 3300 0000 724d 0000 0072 1600 0000  .r3...rM...r....
+000029d0: 7216 0000 0072 1700 0000 da0e 6765 745f  r....r......get_
+000029e0: 636f 6e6e 6563 7469 6f6e 2202 0000 7306  connection"...s.
+000029f0: 0000 0000 0108 0108 0172 c500 0000 6300  .........r....c.
+00002a00: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+00002a10: 0000 0073 1800 0000 7400 6a01 6401 6b02  ...s....t.j.d.k.
+00002a20: 720e 6400 5300 7402 7403 8300 8301 5300  r.d.S.t.t.....S.
+00002a30: 2902 4eda 046e 6f6e 6529 0472 1300 0000  ).N..none).r....
+00002a40: 729e 0000 0072 9800 0000 72b2 0000 0072  r....r....r....r
+00002a50: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00002a60: 0000 00da 1e63 6f6e 6e65 6374 5f64 6174  .....connect_dat
+00002a70: 6162 6173 655f 6672 6f6d 5f73 6574 7469  abase_from_setti
+00002a80: 6e67 7328 0200 0073 0600 0000 0001 0a01  ngs(...s........
+00002a90: 0401 72c7 0000 0063 0100 0000 0000 0000  ..r....c........
+00002aa0: 0100 0000 0300 0000 4300 0000 730c 0000  ........C...s...
+00002ab0: 0074 0074 017c 0083 0183 0153 0029 014e  .t.t.|.....S.).N
+00002ac0: 2902 7298 0000 0072 9b00 0000 2901 729c  ).r....r....).r.
+00002ad0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00002ae0: 0000 da16 6765 745f 7265 7175 6573 745f  ....get_request_
+00002af0: 636f 6e6e 6563 7469 6f6e 2e02 0000 7302  connection....s.
+00002b00: 0000 0000 0172 c800 0000 6301 0000 0000  .....r....c.....
+00002b10: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00002b20: 1a00 0000 7400 7c00 8301 7d01 7c01 7310  ....t.|...}.|.s.
+00002b30: 6400 5300 7c01 6401 1900 8300 5300 2902  d.S.|.d.....S.).
+00002b40: 4e72 8200 0000 2901 72c8 0000 0029 0272  Nr....).r....).r
+00002b50: 9c00 0000 724e 0000 0072 1600 0000 7216  ....rN...r....r.
+00002b60: 0000 0072 1700 0000 da0e 6372 6561 7465  ...r......create
+00002b70: 5f73 6573 7369 6f6e 3202 0000 7308 0000  _session2...s...
+00002b80: 0000 0108 0104 0104 0172 c900 0000 6301  .........r....c.
+00002b90: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00002ba0: 0000 0073 2a00 0000 7400 7c00 8301 7d01  ...s*...t.|...}.
+00002bb0: 7c01 0c00 7316 6401 7c01 6b07 721a 6400  |...s.d.|.k.r.d.
+00002bc0: 5300 7c01 6401 1900 6400 6402 8502 1900  S.|.d...d.d.....
+00002bd0: 5300 2903 4e72 7d00 0000 7279 0000 0029  S.).Nr}...ry...)
+00002be0: 0172 c800 0000 2902 729c 0000 0072 4e00  .r....).r....rN.
+00002bf0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00002c00: 00da 1767 6574 5f63 6f6e 6e65 6374 696f  ...get_connectio
+00002c10: 6e5f 6964 5f73 686f 7274 3902 0000 7308  n_id_short9...s.
+00002c20: 0000 0000 0108 010e 0104 0172 ca00 0000  ...........r....
+00002c30: 6301 0000 0000 0000 0002 0000 0002 0000  c...............
+00002c40: 0043 0000 0073 1800 0000 7400 7c00 8301  .C...s....t.|...
+00002c50: 7d01 7c01 7310 6400 5300 7c01 6401 1900  }.|.s.d.S.|.d...
+00002c60: 5300 2902 4e72 8300 0000 2901 72c8 0000  S.).Nr....).r...
+00002c70: 0029 0272 9c00 0000 724e 0000 0072 1600  .).r....rN...r..
+00002c80: 0000 7216 0000 0072 1700 0000 da0f 6765  ..r....r......ge
+00002c90: 745f 6d61 7070 6564 5f62 6173 6540 0200  t_mapped_base@..
+00002ca0: 0073 0800 0000 0001 0801 0401 0401 72cb  .s............r.
+00002cb0: 0000 0063 0100 0000 0000 0000 0200 0000  ...c............
+00002cc0: 0200 0000 4300 0000 7318 0000 0074 007c  ....C...s....t.|
+00002cd0: 0083 017d 017c 0173 1064 0053 007c 0164  ...}.|.s.d.S.|.d
+00002ce0: 0119 0053 0029 024e 7219 0000 0029 0172  ...S.).Nr....).r
+00002cf0: c800 0000 2902 729c 0000 0072 4e00 0000  ....).r....rN...
+00002d00: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00002d10: 0a67 6574 5f65 6e67 696e 6547 0200 0073  .get_engineG...s
+00002d20: 0800 0000 0001 0801 0401 0401 72cc 0000  ............r...
+00002d30: 0063 0100 0000 0000 0000 0200 0000 0200  .c..............
+00002d40: 0000 4300 0000 7318 0000 0074 007c 0083  ..C...s....t.|..
+00002d50: 017d 017c 0173 1064 0053 007c 0164 0119  .}.|.s.d.S.|.d..
+00002d60: 0053 0029 024e 7284 0000 0029 0172 c800  .S.).Nr....).r..
+00002d70: 0000 2902 729c 0000 0072 4e00 0000 7216  ..).r....rN...r.
+00002d80: 0000 0072 1600 0000 7217 0000 00da 1967  ...r....r......g
+00002d90: 6574 5f74 7970 655f 636f 6465 5f74 6f5f  et_type_code_to_
+00002da0: 7371 6c5f 7479 7065 4e02 0000 7308 0000  sql_typeN...s...
+00002db0: 0000 0108 0104 0104 0172 cd00 0000 6301  .........r....c.
+00002dc0: 0000 0000 0000 0002 0000 0009 0000 0063  ...............c
+00002dd0: 0000 0073 3400 0000 7400 7c00 8301 7d01  ...s4...t.|...}.
+00002de0: 7c01 7312 6900 5600 0100 7c01 6401 1900  |.s.i.V...|.d...
+00002df0: 8f10 0100 7c01 6402 1900 5600 0100 5700  ....|.d...V...W.
+00002e00: 6400 5100 5200 5800 6400 5300 2903 4e72  d.Q.R.X.d.S.).Nr
+00002e10: 8600 0000 7285 0000 0029 0172 c800 0000  ....r....).r....
+00002e20: 2902 729c 0000 0072 4e00 0000 7216 0000  ).r....rN...r...
+00002e30: 0072 1600 0000 7217 0000 00da 1063 6f6e  .r....r......con
+00002e40: 6e65 6374 696f 6e5f 6361 6368 6555 0200  nection_cacheU..
+00002e50: 0073 0a00 0000 0002 0801 0401 0601 0a01  .s..............
+00002e60: 72ce 0000 0063 0300 0000 0000 0000 0400  r....c..........
+00002e70: 0000 0a00 0000 4300 0000 7334 0000 0074  ......C...s4...t
+00002e80: 007c 0083 017d 037c 0373 1064 0053 007c  .|...}.|.s.d.S.|
+00002e90: 0364 0119 008f 1201 007c 0364 0219 006a  .d.......|.d...j
+00002ea0: 017c 017c 0283 0253 0051 0052 0058 0064  .|.|...S.Q.R.X.d
+00002eb0: 0053 0029 034e 7286 0000 0072 8500 0000  .S.).Nr....r....
+00002ec0: 2902 72c8 0000 0072 2b00 0000 2904 729c  ).r....r+...).r.
+00002ed0: 0000 0072 1a00 0000 da07 6465 6661 756c  ...r......defaul
+00002ee0: 7472 4e00 0000 7216 0000 0072 1600 0000  trN...r....r....
+00002ef0: 7217 0000 00da 1463 6f6e 6e65 6374 696f  r......connectio
+00002f00: 6e5f 6361 6368 655f 6765 745e 0200 0073  n_cache_get^...s
+00002f10: 0a00 0000 0001 0801 0401 0401 0a01 72d0  ..............r.
+00002f20: 0000 0063 0300 0000 0000 0000 0400 0000  ...c............
+00002f30: 0a00 0000 4300 0000 7334 0000 0074 007c  ....C...s4...t.|
+00002f40: 0083 017d 037c 0373 1064 0053 007c 0364  ...}.|.s.d.S.|.d
+00002f50: 0119 008f 1201 007c 027c 0364 0219 007c  .......|.|.d...|
+00002f60: 013c 0057 0064 0051 0052 0058 0064 0053  .<.W.d.Q.R.X.d.S
+00002f70: 0029 034e 7286 0000 0072 8500 0000 2901  .).Nr....r....).
+00002f80: 72c8 0000 0029 0472 9c00 0000 721a 0000  r....).r....r...
+00002f90: 0072 1500 0000 724e 0000 0072 1600 0000  .r....rN...r....
+00002fa0: 7216 0000 0072 1700 0000 da14 636f 6e6e  r....r......conn
+00002fb0: 6563 7469 6f6e 5f63 6163 6865 5f73 6574  ection_cache_set
+00002fc0: 6602 0000 730a 0000 0000 0108 0104 0104  f...s...........
+00002fd0: 010a 0172 d100 0000 6301 0000 0000 0000  ...r....c.......
+00002fe0: 0002 0000 0003 0000 0043 0000 0073 1e00  .........C...s..
+00002ff0: 0000 7400 7c00 8301 7d01 7401 7c01 6401  ..t.|...}.t.|.d.
+00003000: 8302 0100 7402 7c00 8301 0100 6400 5300  ....t.|.....d.S.
+00003010: 2902 4e54 2903 72cb 0000 0072 8f00 0000  ).NT).r....r....
+00003020: da1d 7265 6c6f 6164 5f72 6571 7565 7374  ..reload_request
+00003030: 5f67 7261 7068 716c 5f73 6368 656d 6129  _graphql_schema)
+00003040: 0272 9c00 0000 7283 0000 0072 1600 0000  .r....r....r....
+00003050: 7216 0000 0072 1700 0000 da1a 7265 6c6f  r....r......relo
+00003060: 6164 5f72 6571 7565 7374 5f6d 6170 7065  ad_request_mappe
+00003070: 645f 6261 7365 6e02 0000 7306 0000 0000  d_basen...s.....
+00003080: 0108 010a 0172 d300 0000 6302 0000 0000  .....r....c.....
+00003090: 0000 0004 0000 000a 0000 0043 0000 0073  ...........C...s
+000030a0: 4600 0000 7400 7c00 8301 8f34 7d02 7c01  F...t.|....4}.|.
+000030b0: 6400 6b08 7224 6400 7c02 6401 3c00 6400  d.k.r$d.|.d.<.d.
+000030c0: 7c02 6402 3c00 6e14 7c01 722c 6402 6e02  |.d.<.n.|.r,d.n.
+000030d0: 6401 7d03 6400 7c02 7c03 3c00 5700 6400  d.}.d.|.|.<.W.d.
+000030e0: 5100 5200 5800 6400 5300 2903 4e5a 0e67  Q.R.X.d.S.).NZ.g
+000030f0: 7261 7068 716c 5f73 6368 656d 615a 1467  raphql_schemaZ.g
+00003100: 7261 7068 716c 5f73 6368 656d 615f 6472  raphql_schema_dr
+00003110: 6166 7429 0172 ce00 0000 2904 729c 0000  aft).r....).r...
+00003120: 00da 0564 7261 6674 7285 0000 005a 0a73  ...draftr....Z.s
+00003130: 6368 656d 615f 6b65 7972 1600 0000 7216  chema_keyr....r.
+00003140: 0000 0072 1700 0000 72d2 0000 0074 0200  ...r....r....t..
+00003150: 0073 0c00 0000 0001 0a01 0801 0801 0a02  .s..............
+00003160: 0c01 72d2 0000 0063 0200 0000 0000 0000  ..r....c........
+00003170: 0200 0000 0300 0000 4300 0000 7330 0000  ........C...s0..
+00003180: 007c 016a 0072 227c 016a 007c 006a 006b  .|.j.r"|.j.|.j.k
+00003190: 0372 2264 016a 017c 016a 007c 016a 0283  .r"d.j.|.j.|.j..
+000031a0: 0253 0074 037c 016a 0283 0153 0064 0053  .S.t.|.j...S.d.S
+000031b0: 0029 024e 7a05 7b7d 2e7b 7d29 0472 3900  .).Nz.{}.{}).r9.
+000031c0: 0000 7230 0000 0072 1a00 0000 722c 0000  ..r0...r....r,..
+000031d0: 0029 0272 8100 0000 7275 0000 0072 1600  .).r....ru...r..
+000031e0: 0000 7216 0000 0072 1700 0000 da0e 6765  ..r....r......ge
+000031f0: 745f 7461 626c 655f 6e61 6d65 7e02 0000  t_table_name~...
+00003200: 7306 0000 0000 0112 0110 0272 d500 0000  s..........r....
+00003210: 4663 0200 0000 0000 0000 0500 0000 0500  Fc..............
+00003220: 0000 0300 0000 7348 0000 0087 0066 0164  ......sH.....f.d
+00003230: 0164 0284 087d 0264 0364 0484 007d 0364  .d...}.d.d...}.d
+00003240: 0564 0684 007d 047c 0172 3488 006a 006a  .d...}.|.r4..j.j
+00003250: 0183 0001 0088 006a 026a 0383 0001 0088  .......j.j......
+00003260: 006a 047c 027c 037c 0464 078d 0301 0064  .j.|.|.|.d.....d
+00003270: 0053 0029 084e 6303 0000 0000 0000 0003  .S.).Nc.........
+00003280: 0000 0003 0000 0013 0000 0073 0c00 0000  ...........s....
+00003290: 7400 8800 6a01 7c02 8302 5300 2901 4e29  t...j.|...S.).N)
+000032a0: 0272 d500 0000 7281 0000 0029 03da 0462  .r....r....)...b
+000032b0: 6173 655a 0974 6162 6c65 6e61 6d65 7275  aseZ.tablenameru
+000032c0: 0000 0029 0172 8300 0000 7216 0000 0072  ...).r....r....r
+000032d0: 1700 0000 da13 636c 6173 736e 616d 655f  ......classname_
+000032e0: 666f 725f 7461 626c 6586 0200 0073 0200  for_table....s..
+000032f0: 0000 0001 7a2d 6c6f 6164 5f6d 6170 7065  ....z-load_mappe
+00003300: 645f 6261 7365 2e3c 6c6f 6361 6c73 3e2e  d_base.<locals>.
+00003310: 636c 6173 736e 616d 655f 666f 725f 7461  classname_for_ta
+00003320: 626c 6563 0400 0000 0000 0000 0600 0000  blec............
+00003330: 0500 0000 5300 0000 7370 0000 0074 007c  ....S...sp...t.|
+00003340: 036a 0183 0172 147c 036a 0164 0119 006e  .j...r.|.j.d...n
+00003350: 0264 007d 047c 0472 3e64 026a 027c 046a  .d.}.|.r>d.j.|.j
+00003360: 036a 0464 037c 046a 056a 066a 047c 046a  .j.d.|.j.j.j.|.j
+00003370: 056a 0467 0483 017d 056e 0a7c 026a 076a  .j.g...}.n.|.j.j
+00003380: 0883 007d 057c 057c 036a 036a 096b 0672  ...}.|.|.j.j.k.r
+00003390: 6c7c 0564 0417 007d 0574 0a6a 0b64 056a  l|.d...}.t.j.d.j
+000033a0: 0c7c 0583 0183 0101 007c 0553 0029 064e  .|.......|.S.).N
+000033b0: 7201 0000 00da 025f 5fda 0274 6fda 095f  r......__..to.._
+000033c0: 7265 6c61 7469 6f6e 7a26 416c 7265 6164  relationz&Alread
+000033d0: 7920 6465 7465 6374 6564 2063 6f6c 756d  y detected colum
+000033e0: 6e20 6e61 6d65 2c20 7573 696e 6720 7b7d  n name, using {}
+000033f0: 290d 7273 0000 00da 0865 6c65 6d65 6e74  ).rs.....element
+00003400: 7372 3200 0000 da06 7061 7265 6e74 721a  sr2.....parentr.
+00003410: 0000 00da 0663 6f6c 756d 6e72 7500 0000  .....columnru...
+00003420: da08 5f5f 6e61 6d65 5f5f da05 6c6f 7765  ..__name__..lowe
+00003430: 7272 9000 0000 7214 0000 0072 9200 0000  rr....r....r....
+00003440: 7230 0000 0029 0672 d600 0000 da09 6c6f  r0...).r......lo
+00003450: 6361 6c5f 636c 73da 0c72 6566 6572 7265  cal_cls..referre
+00003460: 645f 636c 73da 0a63 6f6e 7374 7261 696e  d_cls..constrain
+00003470: 74da 0b66 6f72 6569 676e 5f6b 6579 721a  t..foreign_keyr.
+00003480: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00003490: 0000 da1c 6e61 6d65 5f66 6f72 5f73 6361  ....name_for_sca
+000034a0: 6c61 725f 7265 6c61 7469 6f6e 7368 6970  lar_relationship
+000034b0: 8902 0000 7310 0000 0000 0118 0104 0122  ....s.........."
+000034c0: 020a 020c 0108 0110 027a 366c 6f61 645f  .........z6load_
+000034d0: 6d61 7070 6564 5f62 6173 652e 3c6c 6f63  mapped_base.<loc
+000034e0: 616c 733e 2e6e 616d 655f 666f 725f 7363  als>.name_for_sc
+000034f0: 616c 6172 5f72 656c 6174 696f 6e73 6869  alar_relationshi
+00003500: 7063 0400 0000 0000 0000 0600 0000 0500  pc..............
+00003510: 0000 5300 0000 7370 0000 0074 007c 036a  ..S...sp...t.|.j
+00003520: 0183 0172 147c 036a 0164 0119 006e 0264  ...r.|.j.d...n.d
+00003530: 007d 047c 0472 3e64 026a 027c 046a 036a  .}.|.r>d.j.|.j.j
+00003540: 046a 057c 046a 036a 0564 037c 046a 066a  .j.|.j.j.d.|.j.j
+00003550: 0567 0483 017d 056e 0a7c 026a 076a 0883  .g...}.n.|.j.j..
+00003560: 007d 057c 057c 036a 036a 096b 0672 6c7c  .}.|.|.j.j.k.rl|
+00003570: 0564 0417 007d 0574 0a6a 0b64 056a 0c7c  .d...}.t.j.d.j.|
+00003580: 0583 0183 0101 007c 0553 0029 064e 7201  .......|.S.).Nr.
+00003590: 0000 0072 d800 0000 72d9 0000 0072 da00  ...r....r....r..
+000035a0: 0000 7a26 416c 7265 6164 7920 6465 7465  ..z&Already dete
+000035b0: 6374 6564 2063 6f6c 756d 6e20 6e61 6d65  cted column name
+000035c0: 2c20 7573 696e 6720 7b7d 290d 7273 0000  , using {}).rs..
+000035d0: 0072 db00 0000 7232 0000 0072 dc00 0000  .r....r2...r....
+000035e0: 7275 0000 0072 1a00 0000 72dd 0000 0072  ru...r....r....r
+000035f0: de00 0000 72df 0000 0072 9000 0000 7214  ....r....r....r.
+00003600: 0000 0072 9200 0000 7230 0000 0029 0672  ...r....r0...).r
+00003610: d600 0000 72e0 0000 0072 e100 0000 72e2  ....r....r....r.
+00003620: 0000 0072 e300 0000 721a 0000 0072 1600  ...r....r....r..
+00003630: 0000 7216 0000 0072 1700 0000 da20 6e61  ..r....r..... na
+00003640: 6d65 5f66 6f72 5f63 6f6c 6c65 6374 696f  me_for_collectio
+00003650: 6e5f 7265 6c61 7469 6f6e 7368 6970 9602  n_relationship..
+00003660: 0000 7310 0000 0000 0118 0104 0122 020a  ..s.........."..
+00003670: 020c 0108 0110 027a 3a6c 6f61 645f 6d61  .......z:load_ma
+00003680: 7070 6564 5f62 6173 652e 3c6c 6f63 616c  pped_base.<local
+00003690: 733e 2e6e 616d 655f 666f 725f 636f 6c6c  s>.name_for_coll
+000036a0: 6563 7469 6f6e 5f72 656c 6174 696f 6e73  ection_relations
+000036b0: 6869 7029 0372 d700 0000 72e4 0000 0072  hip).r....r....r
+000036c0: e500 0000 2905 da08 7265 6769 7374 7279  ....)...registry
+000036d0: 7299 0000 0072 9100 0000 da05 636c 6561  r....r......clea
+000036e0: 72da 0770 7265 7061 7265 2905 7283 0000  r..prepare).r...
+000036f0: 0072 e700 0000 72d7 0000 0072 e400 0000  .r....r....r....
+00003700: 72e5 0000 0072 1600 0000 2901 7283 0000  r....r....).r...
+00003710: 0072 1700 0000 728f 0000 0085 0200 0073  .r....r........s
+00003720: 1400 0000 0001 0c03 080d 080d 0401 0a01  ................
+00003730: 0a02 0401 0201 0201 728f 0000 0029 014e  ........r....).N
+00003740: 2901 4e29 014e 2901 4629 4b72 2e00 0000  ).N).N).F)Kr....
+00003750: da0a 636f 6e74 6578 746c 6962 7241 0000  ..contextlibrA..
+00003760: 0072 8a00 0000 728d 0000 0072 0300 0000  .r....r....r....
+00003770: 7202 0000 005a 176a 6574 5f62 7269 6467  r....Z.jet_bridg
+00003780: 655f 6261 7365 2e61 7574 6f6d 6170 7204  e_base.automapr.
+00003790: 0000 005a 176a 6574 5f62 7269 6467 655f  ...Z.jet_bridge_
+000037a0: 6261 7365 2e72 6566 6c65 6374 7205 0000  base.reflectr...
+000037b0: 005a 1a6a 6574 5f62 7269 6467 655f 6261  .Z.jet_bridge_ba
+000037c0: 7365 2e73 7368 5f74 756e 6e65 6c72 0600  se.ssh_tunnelr..
+000037d0: 0000 5a1b 6a65 745f 6272 6964 6765 5f62  ..Z.jet_bridge_b
+000037e0: 6173 652e 7574 696c 732e 6372 7970 7472  ase.utils.cryptr
+000037f0: 0700 0000 5a1d 6a65 745f 6272 6964 6765  ....Z.jet_bridge
+00003800: 5f62 6173 652e 7574 696c 732e 7072 6f63  _base.utils.proc
+00003810: 6573 7372 0800 0000 5a20 6a65 745f 6272  essr....Z jet_br
+00003820: 6964 6765 5f62 6173 652e 7574 696c 732e  idge_base.utils.
+00003830: 7479 7065 5f63 6f64 6573 7209 0000 00da  type_codesr.....
+00003840: 0373 6978 720a 0000 005a 1673 6978 2e6d  .sixr....Z.six.m
+00003850: 6f76 6573 2e75 726c 6c69 625f 7061 7273  oves.urllib_pars
+00003860: 6572 0b00 0000 5a0a 7371 6c61 6c63 6865  er....Z.sqlalche
+00003870: 6d79 720c 0000 0072 0d00 0000 5a0e 7371  myr....r....Z.sq
+00003880: 6c61 6c63 6865 6d79 2e6f 726d 720e 0000  lalchemy.ormr...
+00003890: 0072 0f00 0000 da1c 6a65 745f 6272 6964  .r......jet_brid
+000038a0: 6765 5f62 6173 652e 7574 696c 732e 636f  ge_base.utils.co
+000038b0: 6d6d 6f6e 7210 0000 0072 1100 0000 5a0b  mmonr....r....Z.
+000038c0: 6765 6f61 6c63 6865 6d79 3272 1200 0000  geoalchemy2r....
+000038d0: da0b 496d 706f 7274 4572 726f 72da 0f6a  ..ImportError..j
+000038e0: 6574 5f62 7269 6467 655f 6261 7365 7213  et_bridge_baser.
+000038f0: 0000 00da 166a 6574 5f62 7269 6467 655f  .....jet_bridge_
+00003900: 6261 7365 2e6c 6f67 6765 7272 1400 0000  base.loggerr....
+00003910: 7244 0000 0072 5c00 0000 7218 0000 0072  rD...r\...r....r
+00003920: 3600 0000 7243 0000 0072 4500 0000 724a  6...rC...rE...rJ
+00003930: 0000 0072 5600 0000 7252 0000 0072 5300  ...rV...rR...rS.
+00003940: 0000 7261 0000 0072 7400 0000 7277 0000  ..ra...rt...rw..
+00003950: 0072 9800 0000 729a 0000 0072 4c00 0000  .r....r....rL...
+00003960: 729d 0000 0072 b200 0000 72c4 0000 0072  r....r....r....r
+00003970: 9b00 0000 72c5 0000 0072 c700 0000 72c8  ....r....r....r.
+00003980: 0000 0072 c900 0000 72ca 0000 0072 cb00  ...r....r....r..
+00003990: 0000 72cc 0000 0072 cd00 0000 da0e 636f  ..r....r......co
+000039a0: 6e74 6578 746d 616e 6167 6572 72ce 0000  ntextmanagerr...
+000039b0: 0072 d000 0000 72d1 0000 0072 d300 0000  .r....r....r....
+000039c0: 72d2 0000 0072 d500 0000 728f 0000 0072  r....r....r....r
+000039d0: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+000039e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000039f0: 0073 7200 0000 0801 0801 0801 0801 0801  .sr.............
+00003a00: 1002 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00003a10: 0c02 1001 1002 1002 0201 1001 0e01 0602  ................
+00003a20: 0c01 0c02 0401 0403 0804 0a54 0815 0807  ...........T....
+00003a30: 0804 084d 0809 080f 0814 083a 080a 086e  ...M.......:...n
+00003a40: 080c 080d 0804 0819 081e 0809 0806 0806  ................
+00003a50: 0804 0807 0807 0807 0807 0807 0e09 0a08  ................
+00003a60: 0808 0806 0a0a 0807                      ........
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/db.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/db.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/encoders.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/encoders.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/sentry.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/sentry.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/configuration.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/configuration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/router.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/router.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/status.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/settings.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/settings.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,147 +1,151 @@
-00000000: 330d 0d0a 76b0 eb63 5008 0000 e300 0000  3...v..cP.......
-00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000020: 0073 ee00 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c03 6d04 5a04 0100 6500 6a05 6a06  d.l.m.Z...e.j.j.
-00000050: 6500 6a05 6a07 6508 8301 8301 5a09 6501  e.j.j.e.....Z.e.
-00000060: 6a0a 650b 1900 5a0c 6403 5a0d 6403 5a0e  j.e...Z.d.Z.d.Z.
-00000070: 6404 5a0f 6401 5a10 6401 5a11 6401 5a12  d.Z.d.Z.d.Z.d.Z.
-00000080: 6404 5a13 6401 5a14 6405 5a15 6401 5a16  d.Z.d.Z.d.Z.d.Z.
-00000090: 6401 5a17 6401 5a18 6401 5a19 6401 5a1a  d.Z.d.Z.d.Z.d.Z.
-000000a0: 6401 5a1b 6401 5a1c 6401 5a1d 6401 5a1e  d.Z.d.Z.d.Z.d.Z.
-000000b0: 6401 5a1f 6401 5a20 6401 5a21 6401 5a22  d.Z.d.Z d.Z!d.Z"
-000000c0: 6401 5a23 6401 5a24 6401 5a25 6401 5a26  d.Z#d.Z$d.Z%d.Z&
-000000d0: 6401 5a27 6401 5a28 6401 5a29 6401 5a2a  d.Z'd.Z(d.Z)d.Z*
-000000e0: 6401 5a2b 6401 5a2c 6401 5a2d 6900 5a2e  d.Z+d.Z,d.Z-i.Z.
-000000f0: 6406 5a2f 6407 5a30 6407 5a31 6407 5a32  d.Z/d.Z0d.Z1d.Z2
-00000100: 6407 5a33 6407 5a34 6408 6409 8400 5a35  d.Z3d.Z4d.d...Z5
-00000110: 6401 5300 290a e900 0000 004e 2901 da10  d.S.)......N)...
-00000120: 7365 745f 6c6f 6767 6572 5f6c 6576 656c  set_logger_level
-00000130: 4654 6120 0300 002d 2d2d 2d2d 4245 4749  FTa ...-----BEGI
-00000140: 4e20 5055 424c 4943 204b 4559 2d2d 2d2d  N PUBLIC KEY----
-00000150: 2d0a 4d49 4943 496a 414e 4267 6b71 686b  -.MIICIjANBgkqhk
-00000160: 6947 3977 3042 4151 4546 4141 4f43 4167  iG9w0BAQEFAAOCAg
-00000170: 3841 4d49 4943 4367 4b43 4167 4541 7966  8AMIICCgKCAgEAyf
-00000180: 4a61 626c 7363 5a6d 7368 3765 4869 7357  JablscZmsh7eHisW
-00000190: 4869 0a2f 7832 674a 556a 6339 6a75 4c34  Hi./x2gJUjc9juL4
-000001a0: 564c 6b45 7070 3650 4839 4168 2b77 4274  VLkEpp6PH9Ah+wBt
-000001b0: 476d 5046 396e 666f 566c 5173 6748 3968  GmPF9nfoVlQsgH9h
-000001c0: 7261 3633 504f 6961 4c55 7a49 7757 2f65  ra63POiaLUzIwW/e
-000001d0: 774f 6c0a 6a79 5046 3046 4a6e 6773 7872  wOl.jyPF0FJngsxr
-000001e0: 6543 784e 7338 6c6d 642f 574e 5872 636e  eCxNs8lmd/WNXrcn
-000001f0: 617a 6b6e 4649 746b 4646 6558 4a75 4d54  azknFItkFFeXJuMT
-00000200: 666f 4250 5147 695a 4f6d 5659 6231 346a  foBPQGiZOmVYb14j
-00000210: 6d76 6b63 0a39 764d 6d65 5859 6a72 6254  mvkc.9vMmeXYjrbT
-00000220: 2b39 3553 5661 794e 3345 3644 7a4c 6f48  +95SVayN3E6DzLoH
-00000230: 4468 6e79 344d 6b61 314f 7378 7649 5035  Dhny4Mka1OsxvIP5
-00000240: 7337 3773 3064 4f6f 3638 547a 6f45 6642  s77s0dOo68TzoEfB
-00000250: 5665 7574 6f0a 492f 646f 7047 3836 4456  Veuto.I/dopG86DV
-00000260: 7534 7759 5674 5950 4954 7a4a 347a 3437  u4wYVtYPITzJ4z47
-00000270: 4f46 5650 4b43 7959 5679 7935 6152 332b  OFVPKCyYVyy5aR3+
-00000280: 4455 6e6d 644b 3778 5452 5672 2b69 576d  DUnmdK7xTRVr+iWm
-00000290: 4870 6372 3765 0a68 6f65 5663 4c34 4371  Hpcr7e.hoeVcL4Cq
-000002a0: 4149 4c5a 3067 6435 346b 516d 6e48 6267  AILZ0gd54kQmnHbg
-000002b0: 3742 7536 7838 4a74 516b 694c 5535 5451  7Bu6x8JtQkiLU5TQ
-000002c0: 7657 7a6a 694e 3030 696f 3465 7964 7649  vWzjiN00io4eydvI
-000002d0: 416b 5154 4161 520a 6d64 6433 324f 3176  AkQTAaR.mdd32O1v
-000002e0: 4a62 5348 6d4c 7943 5232 7445 572f 7556  JbSHmLyCR2tEW/uV
-000002f0: 3750 3235 6e61 5055 6c6b 4170 7875 4c7a  7P25naPUlkApxuLz
-00000300: 6835 4332 3153 3058 4a78 4e4a 2f50 3037  h5C21S0XJxNJ/P07
-00000310: 4b53 4d79 6d74 3555 0a31 6c57 7174 3443  KSMymt5U.1lWqt4C
-00000320: 496e 706a 4177 4d49 3871 7339 4d6b 4577  InpjAwMI8qs9MkEw
-00000330: 4a65 7635 2b79 756d 7871 4972 444b 6351  Jev5+yumxqIrDKcQ
-00000340: 4c4d 5233 5442 4c4a 5a49 622b 724c 3174  LMR3TBLJZIb+rL1t
-00000350: 6543 4c4f 5732 3871 420a 4c36 5653 4b68  eCLOW28qB.L6VSKh
-00000360: 664b 5249 6158 5564 4c70 5277 4163 5375  fKRIaXUdLpRwAcSu
-00000370: 5872 6154 7a77 6139 6f43 435a 6131 3974  XraTzwa9oCCZa19t
-00000380: 7733 7569 7a4d 654d 4672 4372 7634 3359  w3uizMeMFrCrv43Y
-00000390: 6279 4f73 5339 6837 4a51 0a38 6978 6a2f  byOsS9h7JQ.8ixj/
-000003a0: 6131 522f 7564 3066 4372 6858 5755 6c37  a1R/ud0fCrhXWUl7
-000003b0: 6e4b 6c7a 3062 3135 6b6f 494c 4c47 3154  nKlz0b15koILLG1T
-000003c0: 732b 4d55 546d 4961 456e 4854 5645 5937  s+MUTmIaEnHTVEY7
-000003d0: 3443 664a 5671 3777 6177 390a 7832 6b79  4CfJVq7waw9.x2ky
-000003e0: 7a53 7a62 736d 4d58 7646 6b72 567a 546d  zSzbsmMXvFkrVzTm
-000003f0: 7949 6d54 4e36 3331 2b67 6174 552b 6e70  yImTN631+gatU+np
-00000400: 4a33 7674 6344 3953 6f6f 455a 4c4f 434c  J3vtcD9SooEZLOCL
-00000410: 6134 7062 2b44 4973 7639 5031 0a45 6549  a4pb+DIsv9P1.EeI
-00000420: 4541 6831 565a 4337 7332 7173 515a 7369  EAh1VZC7s2qsQZsi
-00000430: 5954 4730 4341 7745 4141 513d 3d0a 2d2d  YTG0CAwEAAQ==.--
-00000440: 2d2d 2d45 4e44 2050 5542 4c49 4320 4b45  ---END PUBLIC KE
-00000450: 592d 2d2d 2d2d 0ada 012a da00 6301 0000  Y-----...*..c...
-00000460: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-00000470: 0073 4800 0000 782a 7c00 6a00 8300 4400  .sH...x*|.j...D.
-00000480: 5d1e 5c02 7d01 7d02 7c02 6400 6b08 721c  ].\.}.}.|.d.k.r.
-00000490: 710a 7401 7402 7c01 7c02 8303 0100 710a  q.t.t.|.|.....q.
-000004a0: 5700 7403 7236 7404 6a03 6e04 7404 6a05  W.t.r6t.j.n.t.j.
-000004b0: 7d03 7406 7c03 8301 0100 6400 5300 2901  }.t.|.....d.S.).
-000004c0: 4e29 07da 0569 7465 6d73 da07 7365 7461  N)...items..seta
-000004d0: 7474 72da 0e43 5552 5245 4e54 5f4d 4f44  ttr..CURRENT_MOD
-000004e0: 554c 45da 0544 4542 5547 da07 6c6f 6767  ULE..DEBUG..logg
-000004f0: 696e 67da 0449 4e46 4f72 0200 0000 2904  ing..INFOr....).
-00000500: da08 7365 7474 696e 6773 da03 6b65 79da  ..settings..key.
-00000510: 0576 616c 7565 da05 6c65 7665 6ca9 0072  .value..level..r
-00000520: 0f00 0000 fa5f 2f55 7365 7273 2f66 316e  ....._/Users/f1n
-00000530: 616c 2f44 726f 7062 6f78 2f70 7974 686f  al/Dropbox/pytho
-00000540: 6e2f 6a65 742d 6272 6964 6765 2f73 7263  n/jet-bridge/src
-00000550: 2f70 6163 6b61 6765 732f 6a65 745f 6272  /packages/jet_br
-00000560: 6964 6765 5f62 6173 652f 6a65 745f 6272  idge_base/jet_br
-00000570: 6964 6765 5f62 6173 652f 7365 7474 696e  idge_base/settin
-00000580: 6773 2e70 79da 0c73 6574 5f73 6574 7469  gs.py..set_setti
-00000590: 6e67 733d 0000 0073 0c00 0000 0001 1201  ngs=...s........
-000005a0: 0801 0201 1002 1001 7211 0000 0029 36da  ........r....)6.
-000005b0: 026f 73da 0373 7973 7209 0000 00da 166a  .os..sysr......j
-000005c0: 6574 5f62 7269 6467 655f 6261 7365 2e6c  et_bridge_base.l
-000005d0: 6f67 6765 7272 0200 0000 da04 7061 7468  oggerr......path
-000005e0: da07 6469 726e 616d 65da 0761 6273 7061  ..dirname..abspa
-000005f0: 7468 da08 5f5f 6669 6c65 5f5f 5a08 4241  th..__file__Z.BA
-00000600: 5345 5f44 4952 da07 6d6f 6475 6c65 73da  SE_DIR..modules.
-00000610: 085f 5f6e 616d 655f 5f72 0700 0000 7208  .__name__r....r.
-00000620: 0000 005a 0952 4541 445f 4f4e 4c59 5a12  ...Z.READ_ONLYZ.
-00000630: 4155 544f 5f4f 5045 4e5f 5245 4749 5354  AUTO_OPEN_REGIST
-00000640: 4552 5a07 5052 4f4a 4543 545a 0554 4f4b  ERZ.PROJECTZ.TOK
-00000650: 454e 5a0b 454e 5649 524f 4e4d 454e 545a  ENZ.ENVIRONMENTZ
-00000660: 0c43 4f52 535f 4845 4144 4552 535a 0842  .CORS_HEADERSZ.B
-00000670: 4153 455f 5552 4c5a 0e4a 5754 5f56 4552  ASE_URLZ.JWT_VER
-00000680: 4946 595f 4b45 595a 0f42 4541 5245 525f  IFY_KEYZ.BEARER_
-00000690: 4155 5448 5f4b 4559 5a10 454e 5649 524f  AUTH_KEYZ.ENVIRO
-000006a0: 4e4d 454e 545f 5459 5045 5a0c 5745 425f  NMENT_TYPEZ.WEB_
-000006b0: 4241 5345 5f55 524c 5a0c 4150 495f 4241  BASE_URLZ.API_BA
-000006c0: 5345 5f55 524c 5a0f 4441 5441 4241 5345  SE_URLZ.DATABASE
-000006d0: 5f45 4e47 494e 455a 0d44 4154 4142 4153  _ENGINEZ.DATABAS
-000006e0: 455f 484f 5354 5a0d 4441 5441 4241 5345  E_HOSTZ.DATABASE
-000006f0: 5f50 4f52 545a 0d44 4154 4142 4153 455f  _PORTZ.DATABASE_
-00000700: 5553 4552 5a11 4441 5441 4241 5345 5f50  USERZ.DATABASE_P
-00000710: 4153 5357 4f52 445a 0d44 4154 4142 4153  ASSWORDZ.DATABAS
-00000720: 455f 4e41 4d45 5a0e 4441 5441 4241 5345  E_NAMEZ.DATABASE
-00000730: 5f45 5854 5241 5a14 4441 5441 4241 5345  _EXTRAZ.DATABASE
-00000740: 5f43 4f4e 4e45 4354 494f 4e53 5a0d 4441  _CONNECTIONSZ.DA
-00000750: 5441 4241 5345 5f4f 4e4c 595a 0f44 4154  TABASE_ONLYZ.DAT
-00000760: 4142 4153 455f 4558 4345 5054 5a0f 4441  ABASE_EXCEPTZ.DA
-00000770: 5441 4241 5345 5f53 4348 454d 415a 1144  TABASE_SCHEMAZ.D
-00000780: 4154 4142 4153 455f 5353 485f 484f 5354  ATABASE_SSH_HOST
-00000790: 5a11 4441 5441 4241 5345 5f53 5348 5f50  Z.DATABASE_SSH_P
-000007a0: 4f52 545a 1144 4154 4142 4153 455f 5353  ORTZ.DATABASE_SS
-000007b0: 485f 5553 4552 5a18 4441 5441 4241 5345  H_USERZ.DATABASE
-000007c0: 5f53 5348 5f50 5249 5641 5445 5f4b 4559  _SSH_PRIVATE_KEY
-000007d0: 5a0f 434f 4f4b 4945 5f53 414d 4553 4954  Z.COOKIE_SAMESIT
-000007e0: 455a 0d43 4f4f 4b49 455f 5345 4355 5245  EZ.COOKIE_SECURE
-000007f0: 5a0d 434f 4f4b 4945 5f44 4f4d 4149 4e5a  Z.COOKIE_DOMAINZ
-00000800: 0f43 4f4f 4b49 455f 434f 4d50 5245 5353  .COOKIE_COMPRESS
-00000810: 5a0a 5354 4f52 455f 5041 5448 5a10 5353  Z.STORE_PATHZ.SS
-00000820: 4f5f 4150 504c 4943 4154 494f 4e53 5a0c  O_APPLICATIONSZ.
-00000830: 414c 4c4f 575f 4f52 4947 494e 5a0f 5452  ALLOW_ORIGINZ.TR
-00000840: 4143 4b5f 4441 5441 4241 5345 535a 1854  ACK_DATABASESZ.T
-00000850: 5241 434b 5f44 4154 4142 4153 4553 5f45  RACK_DATABASES_E
-00000860: 4e44 504f 494e 545a 1454 5241 434b 5f44  NDPOINTZ.TRACK_D
-00000870: 4154 4142 4153 4553 5f41 5554 485a 1554  ATABASES_AUTHZ.T
-00000880: 5241 434b 5f4d 4f44 454c 535f 454e 4450  RACK_MODELS_ENDP
-00000890: 4f49 4e54 5a11 5452 4143 4b5f 4d4f 4445  OINTZ.TRACK_MODE
-000008a0: 4c53 5f41 5554 4872 1100 0000 720f 0000  LS_AUTHr....r...
-000008b0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000008c0: da08 3c6d 6f64 756c 653e 0100 0000 735c  ..<module>....s\
-000008d0: 0000 0008 0108 0108 020c 0214 010a 0204  ................
-000008e0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-000008f0: 0104 0104 0204 0104 0204 0104 0104 0104  ................
-00000900: 0104 0104 0104 0104 0104 0104 0104 0204  ................
-00000910: 0104 0104 0104 0204 0104 0104 0104 0204  ................
-00000920: 0204 0204 0204 0104 0104 0204 0104 03    ...............
+00000000: 420d 0d0a 0000 0000 9e18 3964 8008 0000  B.........9d....
+00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
+00000020: 0040 0000 0073 f600 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 5a00 6400 6401 6c01 5a01 6400 6401 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 6400 6402 6c03 6d04 5a04 0100 6500  Z.d.d.l.m.Z...e.
+00000050: 6a05 a006 6500 6a05 a007 6508 a101 a101  j...e.j...e.....
+00000060: 5a09 6501 6a0a 650b 1900 5a0c 6403 5a0d  Z.e.j.e...Z.d.Z.
+00000070: 6403 5a0e 6404 5a0f 6401 5a10 6401 5a11  d.Z.d.Z.d.Z.d.Z.
+00000080: 6401 5a12 6404 5a13 6401 5a14 6405 5a15  d.Z.d.Z.d.Z.d.Z.
+00000090: 6401 5a16 6401 5a17 6401 5a18 6401 5a19  d.Z.d.Z.d.Z.d.Z.
+000000a0: 6401 5a1a 6401 5a1b 6401 5a1c 6401 5a1d  d.Z.d.Z.d.Z.d.Z.
+000000b0: 6401 5a1e 6401 5a1f 6401 5a20 6401 5a21  d.Z.d.Z.d.Z d.Z!
+000000c0: 6401 5a22 6401 5a23 6401 5a24 6401 5a25  d.Z"d.Z#d.Z$d.Z%
+000000d0: 6401 5a26 6401 5a27 6401 5a28 6401 5a29  d.Z&d.Z'd.Z(d.Z)
+000000e0: 6401 5a2a 6401 5a2b 6401 5a2c 6401 5a2d  d.Z*d.Z+d.Z,d.Z-
+000000f0: 6401 5a2e 6900 5a2f 6406 5a30 6407 5a31  d.Z.i.Z/d.Z0d.Z1
+00000100: 6407 5a32 6407 5a33 6407 5a34 6407 5a35  d.Z2d.Z3d.Z4d.Z5
+00000110: 6401 5a36 6408 6409 8400 5a37 6401 5300  d.Z6d.d...Z7d.S.
+00000120: 290a e900 0000 004e 2901 da10 7365 745f  )......N)...set_
+00000130: 6c6f 6767 6572 5f6c 6576 656c 4654 6120  logger_levelFTa 
+00000140: 0300 002d 2d2d 2d2d 4245 4749 4e20 5055  ...-----BEGIN PU
+00000150: 424c 4943 204b 4559 2d2d 2d2d 2d0a 4d49  BLIC KEY-----.MI
+00000160: 4943 496a 414e 4267 6b71 686b 6947 3977  ICIjANBgkqhkiG9w
+00000170: 3042 4151 4546 4141 4f43 4167 3841 4d49  0BAQEFAAOCAg8AMI
+00000180: 4943 4367 4b43 4167 4541 7966 4a61 626c  ICCgKCAgEAyfJabl
+00000190: 7363 5a6d 7368 3765 4869 7357 4869 0a2f  scZmsh7eHisWHi./
+000001a0: 7832 674a 556a 6339 6a75 4c34 564c 6b45  x2gJUjc9juL4VLkE
+000001b0: 7070 3650 4839 4168 2b77 4274 476d 5046  pp6PH9Ah+wBtGmPF
+000001c0: 396e 666f 566c 5173 6748 3968 7261 3633  9nfoVlQsgH9hra63
+000001d0: 504f 6961 4c55 7a49 7757 2f65 774f 6c0a  POiaLUzIwW/ewOl.
+000001e0: 6a79 5046 3046 4a6e 6773 7872 6543 784e  jyPF0FJngsxreCxN
+000001f0: 7338 6c6d 642f 574e 5872 636e 617a 6b6e  s8lmd/WNXrcnazkn
+00000200: 4649 746b 4646 6558 4a75 4d54 666f 4250  FItkFFeXJuMTfoBP
+00000210: 5147 695a 4f6d 5659 6231 346a 6d76 6b63  QGiZOmVYb14jmvkc
+00000220: 0a39 764d 6d65 5859 6a72 6254 2b39 3553  .9vMmeXYjrbT+95S
+00000230: 5661 794e 3345 3644 7a4c 6f48 4468 6e79  VayN3E6DzLoHDhny
+00000240: 344d 6b61 314f 7378 7649 5035 7337 3773  4Mka1OsxvIP5s77s
+00000250: 3064 4f6f 3638 547a 6f45 6642 5665 7574  0dOo68TzoEfBVeut
+00000260: 6f0a 492f 646f 7047 3836 4456 7534 7759  o.I/dopG86DVu4wY
+00000270: 5674 5950 4954 7a4a 347a 3437 4f46 5650  VtYPITzJ4z47OFVP
+00000280: 4b43 7959 5679 7935 6152 332b 4455 6e6d  KCyYVyy5aR3+DUnm
+00000290: 644b 3778 5452 5672 2b69 576d 4870 6372  dK7xTRVr+iWmHpcr
+000002a0: 3765 0a68 6f65 5663 4c34 4371 4149 4c5a  7e.hoeVcL4CqAILZ
+000002b0: 3067 6435 346b 516d 6e48 6267 3742 7536  0gd54kQmnHbg7Bu6
+000002c0: 7838 4a74 516b 694c 5535 5451 7657 7a6a  x8JtQkiLU5TQvWzj
+000002d0: 694e 3030 696f 3465 7964 7649 416b 5154  iN00io4eydvIAkQT
+000002e0: 4161 520a 6d64 6433 324f 3176 4a62 5348  AaR.mdd32O1vJbSH
+000002f0: 6d4c 7943 5232 7445 572f 7556 3750 3235  mLyCR2tEW/uV7P25
+00000300: 6e61 5055 6c6b 4170 7875 4c7a 6835 4332  naPUlkApxuLzh5C2
+00000310: 3153 3058 4a78 4e4a 2f50 3037 4b53 4d79  1S0XJxNJ/P07KSMy
+00000320: 6d74 3555 0a31 6c57 7174 3443 496e 706a  mt5U.1lWqt4CInpj
+00000330: 4177 4d49 3871 7339 4d6b 4577 4a65 7635  AwMI8qs9MkEwJev5
+00000340: 2b79 756d 7871 4972 444b 6351 4c4d 5233  +yumxqIrDKcQLMR3
+00000350: 5442 4c4a 5a49 622b 724c 3174 6543 4c4f  TBLJZIb+rL1teCLO
+00000360: 5732 3871 420a 4c36 5653 4b68 664b 5249  W28qB.L6VSKhfKRI
+00000370: 6158 5564 4c70 5277 4163 5375 5872 6154  aXUdLpRwAcSuXraT
+00000380: 7a77 6139 6f43 435a 6131 3974 7733 7569  zwa9oCCZa19tw3ui
+00000390: 7a4d 654d 4672 4372 7634 3359 6279 4f73  zMeMFrCrv43YbyOs
+000003a0: 5339 6837 4a51 0a38 6978 6a2f 6131 522f  S9h7JQ.8ixj/a1R/
+000003b0: 7564 3066 4372 6858 5755 6c37 6e4b 6c7a  ud0fCrhXWUl7nKlz
+000003c0: 3062 3135 6b6f 494c 4c47 3154 732b 4d55  0b15koILLG1Ts+MU
+000003d0: 546d 4961 456e 4854 5645 5937 3443 664a  TmIaEnHTVEY74CfJ
+000003e0: 5671 3777 6177 390a 7832 6b79 7a53 7a62  Vq7waw9.x2kyzSzb
+000003f0: 736d 4d58 7646 6b72 567a 546d 7949 6d54  smMXvFkrVzTmyImT
+00000400: 4e36 3331 2b67 6174 552b 6e70 4a33 7674  N631+gatU+npJ3vt
+00000410: 6344 3953 6f6f 455a 4c4f 434c 6134 7062  cD9SooEZLOCLa4pb
+00000420: 2b44 4973 7639 5031 0a45 6549 4541 6831  +DIsv9P1.EeIEAh1
+00000430: 565a 4337 7332 7173 515a 7369 5954 4730  VZC7s2qsQZsiYTG0
+00000440: 4341 7745 4141 513d 3d0a 2d2d 2d2d 2d45  CAwEAAQ==.-----E
+00000450: 4e44 2050 5542 4c49 4320 4b45 592d 2d2d  ND PUBLIC KEY---
+00000460: 2d2d 0ada 012a da00 6301 0000 0000 0000  --...*..c.......
+00000470: 0004 0000 0005 0000 0043 0000 0073 4800  .........C...sH.
+00000480: 0000 782a 7c00 a000 a100 4400 5d1e 5c02  ..x*|.....D.].\.
+00000490: 7d01 7d02 7c02 6400 6b08 721c 710a 7401  }.}.|.d.k.r.q.t.
+000004a0: 7402 7c01 7c02 8303 0100 710a 5700 7403  t.|.|.....q.W.t.
+000004b0: 7236 7404 6a03 6e04 7404 6a05 7d03 7406  r6t.j.n.t.j.}.t.
+000004c0: 7c03 8301 0100 6400 5300 2901 4e29 07da  |.....d.S.).N)..
+000004d0: 0569 7465 6d73 da07 7365 7461 7474 72da  .items..setattr.
+000004e0: 0e43 5552 5245 4e54 5f4d 4f44 554c 45da  .CURRENT_MODULE.
+000004f0: 0544 4542 5547 da07 6c6f 6767 696e 67da  .DEBUG..logging.
+00000500: 0449 4e46 4f72 0200 0000 2904 da08 7365  .INFOr....)...se
+00000510: 7474 696e 6773 da03 6b65 79da 0576 616c  ttings..key..val
+00000520: 7565 da05 6c65 7665 6ca9 0072 0f00 0000  ue..level..r....
+00000530: fa5f 2f55 7365 7273 2f66 316e 616c 2f44  ._/Users/f1nal/D
+00000540: 726f 7062 6f78 2f70 7974 686f 6e2f 6a65  ropbox/python/je
+00000550: 742d 6272 6964 6765 2f73 7263 2f70 6163  t-bridge/src/pac
+00000560: 6b61 6765 732f 6a65 745f 6272 6964 6765  kages/jet_bridge
+00000570: 5f62 6173 652f 6a65 745f 6272 6964 6765  _base/jet_bridge
+00000580: 5f62 6173 652f 7365 7474 696e 6773 2e70  _base/settings.p
+00000590: 79da 0c73 6574 5f73 6574 7469 6e67 7340  y..set_settings@
+000005a0: 0000 0073 0c00 0000 0001 1201 0801 0201  ...s............
+000005b0: 1002 1001 7211 0000 0029 38da 026f 73da  ....r....)8..os.
+000005c0: 0373 7973 7209 0000 005a 166a 6574 5f62  .sysr....Z.jet_b
+000005d0: 7269 6467 655f 6261 7365 2e6c 6f67 6765  ridge_base.logge
+000005e0: 7272 0200 0000 da04 7061 7468 da07 6469  rr......path..di
+000005f0: 726e 616d 65da 0761 6273 7061 7468 da08  rname..abspath..
+00000600: 5f5f 6669 6c65 5f5f 5a08 4241 5345 5f44  __file__Z.BASE_D
+00000610: 4952 da07 6d6f 6475 6c65 73da 085f 5f6e  IR..modules..__n
+00000620: 616d 655f 5f72 0700 0000 7208 0000 005a  ame__r....r....Z
+00000630: 0952 4541 445f 4f4e 4c59 5a12 4155 544f  .READ_ONLYZ.AUTO
+00000640: 5f4f 5045 4e5f 5245 4749 5354 4552 5a07  _OPEN_REGISTERZ.
+00000650: 5052 4f4a 4543 545a 0554 4f4b 454e 5a0b  PROJECTZ.TOKENZ.
+00000660: 454e 5649 524f 4e4d 454e 545a 0c43 4f52  ENVIRONMENTZ.COR
+00000670: 535f 4845 4144 4552 535a 0842 4153 455f  S_HEADERSZ.BASE_
+00000680: 5552 4c5a 0e4a 5754 5f56 4552 4946 595f  URLZ.JWT_VERIFY_
+00000690: 4b45 595a 0f42 4541 5245 525f 4155 5448  KEYZ.BEARER_AUTH
+000006a0: 5f4b 4559 5a10 454e 5649 524f 4e4d 454e  _KEYZ.ENVIRONMEN
+000006b0: 545f 5459 5045 5a0c 5745 425f 4241 5345  T_TYPEZ.WEB_BASE
+000006c0: 5f55 524c 5a0c 4150 495f 4241 5345 5f55  _URLZ.API_BASE_U
+000006d0: 524c 5a0f 4441 5441 4241 5345 5f45 4e47  RLZ.DATABASE_ENG
+000006e0: 494e 455a 0d44 4154 4142 4153 455f 484f  INEZ.DATABASE_HO
+000006f0: 5354 5a0d 4441 5441 4241 5345 5f50 4f52  STZ.DATABASE_POR
+00000700: 545a 0d44 4154 4142 4153 455f 5553 4552  TZ.DATABASE_USER
+00000710: 5a11 4441 5441 4241 5345 5f50 4153 5357  Z.DATABASE_PASSW
+00000720: 4f52 445a 0d44 4154 4142 4153 455f 4e41  ORDZ.DATABASE_NA
+00000730: 4d45 5a0e 4441 5441 4241 5345 5f45 5854  MEZ.DATABASE_EXT
+00000740: 5241 5a14 4441 5441 4241 5345 5f43 4f4e  RAZ.DATABASE_CON
+00000750: 4e45 4354 494f 4e53 5a0d 4441 5441 4241  NECTIONSZ.DATABA
+00000760: 5345 5f4f 4e4c 595a 0f44 4154 4142 4153  SE_ONLYZ.DATABAS
+00000770: 455f 4558 4345 5054 5a13 4441 5441 4241  E_EXCEPTZ.DATABA
+00000780: 5345 5f4d 4158 5f54 4142 4c45 535a 0f44  SE_MAX_TABLESZ.D
+00000790: 4154 4142 4153 455f 5343 4845 4d41 5a11  ATABASE_SCHEMAZ.
+000007a0: 4441 5441 4241 5345 5f53 5348 5f48 4f53  DATABASE_SSH_HOS
+000007b0: 545a 1144 4154 4142 4153 455f 5353 485f  TZ.DATABASE_SSH_
+000007c0: 504f 5254 5a11 4441 5441 4241 5345 5f53  PORTZ.DATABASE_S
+000007d0: 5348 5f55 5345 525a 1844 4154 4142 4153  SH_USERZ.DATABAS
+000007e0: 455f 5353 485f 5052 4956 4154 455f 4b45  E_SSH_PRIVATE_KE
+000007f0: 595a 0f43 4f4f 4b49 455f 5341 4d45 5349  YZ.COOKIE_SAMESI
+00000800: 5445 5a0d 434f 4f4b 4945 5f53 4543 5552  TEZ.COOKIE_SECUR
+00000810: 455a 0d43 4f4f 4b49 455f 444f 4d41 494e  EZ.COOKIE_DOMAIN
+00000820: 5a0f 434f 4f4b 4945 5f43 4f4d 5052 4553  Z.COOKIE_COMPRES
+00000830: 535a 0a53 544f 5245 5f50 4154 485a 1053  SZ.STORE_PATHZ.S
+00000840: 534f 5f41 5050 4c49 4341 5449 4f4e 535a  SO_APPLICATIONSZ
+00000850: 0c41 4c4c 4f57 5f4f 5249 4749 4e5a 0f54  .ALLOW_ORIGINZ.T
+00000860: 5241 434b 5f44 4154 4142 4153 4553 5a18  RACK_DATABASESZ.
+00000870: 5452 4143 4b5f 4441 5441 4241 5345 535f  TRACK_DATABASES_
+00000880: 454e 4450 4f49 4e54 5a14 5452 4143 4b5f  ENDPOINTZ.TRACK_
+00000890: 4441 5441 4241 5345 535f 4155 5448 5a15  DATABASES_AUTHZ.
+000008a0: 5452 4143 4b5f 4d4f 4445 4c53 5f45 4e44  TRACK_MODELS_END
+000008b0: 504f 494e 545a 1154 5241 434b 5f4d 4f44  POINTZ.TRACK_MOD
+000008c0: 454c 535f 4155 5448 5a0c 4449 5341 424c  ELS_AUTHZ.DISABL
+000008d0: 455f 4155 5448 7211 0000 0072 0f00 0000  E_AUTHr....r....
+000008e0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+000008f0: 083c 6d6f 6475 6c65 3e01 0000 0073 6000  .<module>....s`.
+00000900: 0000 0801 0801 0802 0c02 1401 0a02 0401  ................
+00000910: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00000920: 0401 0402 0401 0402 0401 0401 0401 0401  ................
+00000930: 0401 0401 0401 0401 0401 0401 0401 0402  ................
+00000940: 0401 0401 0401 0402 0401 0401 0401 0402  ................
+00000950: 0402 0402 0402 0401 0401 0402 0401 0402  ................
+00000960: 0403                                     ..
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/configuration.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/configuration.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/reflect.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/reflect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/media_cache.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/media_cache.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/permissions.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/permissions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/ssh_tunnel.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/ssh_tunnel.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/router.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/router.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/logger.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/logger.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/request.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/request.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/permissions.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/permissions.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 4784 1064 8b1c 0000 e300 0000  3...G..d........
+00000000: 330d 0d0a eb10 c264 751c 0000 e300 0000  3......du.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 b000 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -242,15 +242,15 @@
 00000f10: 6e46 723a 0000 0072 4600 0000 722f 0000  nFr:...rF...r/..
 00000f20: 00da 010a 6301 0000 0000 0000 0002 0000  ....c...........
 00000f30: 0003 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
 00000f40: 7c00 5d0c 7d01 7c01 6a00 8300 9102 7104  |.].}.|.j.....q.
 00000f50: 5300 7211 0000 0029 01da 066c 7374 7269  S.r....)...lstri
 00000f60: 7029 02da 022e 30da 046c 696e 6572 1100  p)....0..liner..
 00000f70: 0000 7211 0000 0072 1200 0000 fa0a 3c6c  ..r....r......<l
-00000f80: 6973 7463 6f6d 703e 9100 0000 7302 0000  istcomp>....s...
+00000f80: 6973 7463 6f6d 703e 9000 0000 7302 0000  istcomp>....s...
 00000f90: 0006 007a 3848 6173 5072 6f6a 6563 7450  ...z8HasProjectP
 00000fa0: 6572 6d69 7373 696f 6e73 2e68 6173 5f70  ermissions.has_p
 00000fb0: 6572 6d69 7373 696f 6e2e 3c6c 6f63 616c  ermission.<local
 00000fc0: 733e 2e3c 6c69 7374 636f 6d70 3e7a 025c  s>.<listcomp>z.\
 00000fd0: 6e72 0e00 0000 da05 5253 3235 3629 02da  nr......RS256)..
 00000fe0: 036b 6579 da0a 616c 676f 7269 7468 6d73  .key..algorithms
 00000ff0: 5a08 7072 6f6a 6563 7473 da0b 656e 7669  Z.projects..envi
@@ -271,18 +271,18 @@
 000010e0: 726f 6a65 6374 5f74 6f6b 656e 5f70 7265  roject_token_pre
 000010f0: 6669 78da 1362 6561 7265 725f 746f 6b65  fix..bearer_toke
 00001100: 6e5f 7072 6566 6978 da0f 4245 4152 4552  n_prefix..BEARER
 00001110: 5f41 5554 485f 4b45 5929 0c72 1b00 0000  _AUTH_KEY).r....
 00001120: 721c 0000 0072 1d00 0000 723a 0000 0072  r....r....r:...r
 00001130: 5200 0000 da0f 6272 6964 6765 5f73 6574  R.....bridge_set
 00001140: 7469 6e67 7372 5400 0000 7246 0000 0072  tingsrT...rF...r
-00001150: 6b00 0000 7239 0000 0072 5300 0000 da07  k...r9...rS.....
+00001150: 6b00 0000 7239 0000 0072 5300 0000 5a07  k...r9...rS...Z.
 00001160: 7573 6572 5f69 6472 1100 0000 7211 0000  user_idr....r...
 00001170: 0072 1200 0000 721e 0000 007f 0000 0073  .r....r........s
-00001180: 4800 0000 0002 1201 1802 0401 0402 0802  H...............
+00001180: 4800 0000 0001 1201 1802 0401 0402 0802  H...............
 00001190: 0401 0a01 0c02 0601 0602 1001 1c02 0201  ................
 000011a0: 1a01 0e01 0602 1202 0801 0402 0c01 0c01  ................
 000011b0: 0602 0a01 0a01 1002 0a02 0e01 1001 1605  ................
 000011c0: 0801 1001 1605 0801 1001 1602 7a24 4861  ............z$Ha
 000011d0: 7350 726f 6a65 6374 5065 726d 6973 7369  sProjectPermissi
 000011e0: 6f6e 732e 6861 735f 7065 726d 6973 7369  ons.has_permissi
 000011f0: 6f6e 4e29 0a72 2100 0000 7222 0000 0072  onN).r!...r"...r
@@ -297,27 +297,27 @@
 00001280: 6402 8400 5a03 6403 5300 2904 da08 5265  d...Z.d.S.)...Re
 00001290: 6164 4f6e 6c79 6303 0000 0000 0000 0003  adOnlyc.........
 000012a0: 0000 0005 0000 0043 0000 0073 1c00 0000  .......C...s....
 000012b0: 7400 6a01 730a 6401 5300 7c02 6a02 6407  t.j.s.d.S.|.j.d.
 000012c0: 6b06 7218 6406 5300 6401 5300 2908 4e54  k.r.d.S.d.S.).NT
 000012d0: da06 6372 6561 7465 da06 7570 6461 7465  ..create..update
 000012e0: da0e 7061 7274 6961 6c5f 7570 6461 7465  ..partial_update
-000012f0: da07 6465 7374 726f 7946 2904 7276 0000  ..destroyF).rv..
-00001300: 0072 7700 0000 7278 0000 0072 7900 0000  .rw...rx...ry...
+000012f0: da07 6465 7374 726f 7946 2904 7275 0000  ..destroyF).ru..
+00001300: 0072 7600 0000 7277 0000 0072 7800 0000  .rv...rw...rx...
 00001310: 2903 7203 0000 00da 0952 4541 445f 4f4e  ).r......READ_ON
 00001320: 4c59 da06 6163 7469 6f6e 2903 721b 0000  LY..action).r...
 00001330: 0072 1c00 0000 721d 0000 0072 1100 0000  .r....r....r....
-00001340: 7211 0000 0072 1200 0000 721e 0000 00be  r....r....r.....
+00001340: 7211 0000 0072 1200 0000 721e 0000 00bd  r....r....r.....
 00001350: 0000 0073 0a00 0000 0001 0601 0401 0a01  ...s............
 00001360: 0401 7a17 5265 6164 4f6e 6c79 2e68 6173  ..z.ReadOnly.has
 00001370: 5f70 6572 6d69 7373 696f 6e4e 2904 7221  _permissionN).r!
 00001380: 0000 0072 2200 0000 7223 0000 0072 1e00  ...r"...r#...r..
 00001390: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
-000013a0: 0072 1200 0000 7275 0000 00bc 0000 0073  .r....ru.......s
-000013b0: 0200 0000 0802 7275 0000 0063 0000 0000  ......ru...c....
+000013a0: 0072 1200 0000 7274 0000 00bb 0000 0073  .r....rt.......s
+000013b0: 0200 0000 0802 7274 0000 0063 0000 0000  ......rt...c....
 000013c0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
 000013d0: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
 000013e0: 0284 005a 0364 0353 0029 04da 1841 646d  ...Z.d.S.)...Adm
 000013f0: 696e 6973 7472 6174 6f72 5065 726d 6973  inistratorPermis
 00001400: 7369 6f6e 7363 0300 0000 0000 0000 0700  sionsc..........
 00001410: 0000 0b00 0000 4300 0000 738c 0000 007c  ......C...s....|
 00001420: 026a 0064 0164 0083 027d 037c 0373 1464  .j.d.d...}.|.s.d
@@ -331,46 +331,46 @@
 000014a0: 0253 0064 0353 0064 0053 0029 0b4e 7260  .S.d.S.d.S.).Nr`
 000014b0: 0000 0046 5472 5a00 0000 6301 0000 0000  ...FTrZ...c.....
 000014c0: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
 000014d0: 1400 0000 6700 7c00 5d0c 7d01 7c01 6a00  ....g.|.].}.|.j.
 000014e0: 8300 9102 7104 5300 7211 0000 0029 0172  ....q.S.r....).r
 000014f0: 5b00 0000 2902 725c 0000 0072 5d00 0000  [...).r\...r]...
 00001500: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00001510: 5e00 0000 d000 0000 7302 0000 0006 007a  ^.......s......z
+00001510: 5e00 0000 cf00 0000 7302 0000 0006 007a  ^.......s......z
 00001520: 3b41 646d 696e 6973 7472 6174 6f72 5065  ;AdministratorPe
 00001530: 726d 6973 7369 6f6e 732e 6861 735f 7065  rmissions.has_pe
 00001540: 726d 6973 7369 6f6e 2e3c 6c6f 6361 6c73  rmission.<locals
 00001550: 3e2e 3c6c 6973 7463 6f6d 703e 7a02 5c6e  >.<listcomp>z.\n
 00001560: 725f 0000 0029 0272 6000 0000 7261 0000  r_...).r`...ra..
 00001570: 00da 0561 646d 696e 290a da0c 6765 745f  ...admin)...get_
 00001580: 6172 6775 6d65 6e74 7203 0000 0072 7200  argumentr....rr.
 00001590: 0000 726a 0000 0072 6b00 0000 722b 0000  ..rj...rk...r+..
 000015a0: 0072 6c00 0000 720c 0000 0072 0200 0000  .rl...r....r....
 000015b0: 724c 0000 0029 0772 1b00 0000 721c 0000  rL...).r....r...
 000015c0: 0072 1d00 0000 7260 0000 0072 6b00 0000  .r....r`...rk...
-000015d0: 7239 0000 0072 7d00 0000 7211 0000 0072  r9...r}...r....r
-000015e0: 1100 0000 7212 0000 0072 1e00 0000 c700  ....r....r......
+000015d0: 7239 0000 0072 7c00 0000 7211 0000 0072  r9...r|...r....r
+000015e0: 1100 0000 7212 0000 0072 1e00 0000 c600  ....r....r......
 000015f0: 0000 731c 0000 0000 010c 0204 0104 0210  ..s.............
 00001600: 0104 021c 0202 0116 010e 0106 020c 0204  ................
 00001610: 0104 027a 2741 646d 696e 6973 7472 6174  ...z'Administrat
 00001620: 6f72 5065 726d 6973 7369 6f6e 732e 6861  orPermissions.ha
 00001630: 735f 7065 726d 6973 7369 6f6e 4e29 0472  s_permissionN).r
 00001640: 2100 0000 7222 0000 0072 2300 0000 721e  !...r"...r#...r.
 00001650: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-00001660: 0000 7212 0000 0072 7c00 0000 c600 0000  ..r....r|.......
-00001670: 7302 0000 0008 0172 7c00 0000 2914 7208  s......r|...).r.
+00001660: 0000 7212 0000 0072 7b00 0000 c500 0000  ..r....r{.......
+00001670: 7302 0000 0008 0172 7b00 0000 2914 7208  s......r{...).r.
 00001680: 0000 0072 0a00 0000 724d 0000 0072 6c00  ...r....rM...rl.
 00001690: 0000 7202 0000 00da 0f6a 6574 5f62 7269  ..r......jet_bri
 000016a0: 6467 655f 6261 7365 7203 0000 00da 166a  dge_baser......j
 000016b0: 6574 5f62 7269 6467 655f 6261 7365 2e73  et_bridge_base.s
 000016c0: 656e 7472 7972 0400 0000 da1d 6a65 745f  entryr......jet_
 000016d0: 6272 6964 6765 5f62 6173 652e 7574 696c  bridge_base.util
 000016e0: 732e 6261 636b 656e 6472 0500 0000 da1b  s.backendr......
 000016f0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
 00001700: 7574 696c 732e 6372 7970 7472 0600 0000  utils.cryptr....
 00001710: 7213 0000 0072 1900 0000 da06 6f62 6a65  r....r......obje
-00001720: 6374 721a 0000 0072 2400 0000 7275 0000  ctr....r$...ru..
-00001730: 0072 7c00 0000 7211 0000 0072 1100 0000  .r|...r....r....
+00001720: 6374 721a 0000 0072 2400 0000 7274 0000  ctr....r$...rt..
+00001730: 0072 7b00 0000 7211 0000 0072 1100 0000  .r{...r....r....
 00001740: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
 00001750: 756c 653e 0100 0000 731e 0000 0008 0108  ule>....s.......
 00001760: 0108 0208 010c 020c 010c 010c 010c 0308  ................
-00001770: 0908 0910 0910 7f00 1410 0a              ...........
+00001770: 0908 0910 0910 7f00 1310 0a              ...........
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/__pycache__/reflect.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/__pycache__/reflect.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,216 @@
-00000000: 330d 0d0a 76b0 eb63 110f 0000 e300 0000  3...v..c........
+00000000: 330d 0d0a ce22 c264 1b12 0000 e300 0000  3....".d........
 00000010: 0000 0000 0000 0000 0008 0000 0040 0000  .............@..
-00000020: 0073 5600 0000 6400 6401 6c00 6d01 5a01  .sV...d.d.l.m.Z.
+00000020: 0073 7800 0000 6400 6401 6c00 6d01 5a01  .sx...d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c02 6d04 5a04 0100 6400 6404 6c02  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6405 6c02 6d06 5a06  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6406 6c07 6d08 5a08 0100 640c  ..d.d.l.m.Z...d.
-00000070: 640a 640b 8401 5a09 6407 5300 290d e900  d.d...Z.d.S.)...
-00000080: 0000 0029 01da 0e5f 6269 6e64 5f6f 725f  ...)..._bind_or_
-00000090: 6572 726f 7229 01da 0554 6162 6c65 2901  error)...Table).
-000000a0: da03 6578 6329 01da 0a69 6e73 7065 6374  ..exc)...inspect
-000000b0: 696f 6e29 01da 0475 7469 6c29 01da 066c  ion)...util)...l
-000000c0: 6f67 6765 724e 4654 6309 0000 0000 0000  oggerNFTc.......
-000000d0: 0018 0000 0019 0000 000b 0000 0073 aa02  .............s..
-000000e0: 0000 7c01 6400 6b08 7210 7400 8803 8301  ..|.d.k.r.t.....
-000000f0: 7d01 7401 6a02 7c01 8301 6a03 8300 9002  }.t.j.|...j.....
-00000100: 8f80 7d0a 7c0a 8802 7c06 7c07 7404 8300  ..}.|...|.|.t...
-00000110: 6401 9c05 7d0b 7c0b 6a05 7c09 8301 0100  d...}.|.j.|.....
-00000120: 8805 6400 6b08 724c 8803 6a06 8905 8805  ..d.k.rL..j.....
-00000130: 6400 6b09 725c 8805 7c0b 6402 3c00 7407  d.k.r\..|.d.<.t.
-00000140: 6a08 7c0a 6a09 8805 8301 8301 8900 7c03  j.|.j.........|.
-00000150: 7280 8800 6a05 7c0a 6a0a 8805 8301 8301  r...j.|.j.......
-00000160: 0100 8805 6400 6b09 72a2 7407 6a08 8705  ....d.k.r.t.j...
-00000170: 6601 6403 6404 8408 8800 4400 8301 8301  f.d.d.....D.....
-00000180: 7d0c 6e04 8800 7d0c 7404 8803 6a0b 8301  }.n...}.t...j...
-00000190: 8901 8804 6400 6b08 72d4 8701 8702 6602  ....d.k.r.....f.
-000001a0: 6405 6404 8408 740c 8800 7c0c 8302 4400  d.d...t...|...D.
-000001b0: 8301 7d0d 6e84 740d 8804 8301 72fc 8701  ..}.n.t.....r...
-000001c0: 8702 8703 8704 6604 6406 6404 8408 740c  ......f.d.d...t.
-000001d0: 8800 7c0c 8302 4400 8301 7d0d 6e5c 8700  ..|...D...}.n\..
-000001e0: 6601 6407 6404 8408 8804 4400 8301 7d0e  f.d.d.....D...}.
-000001f0: 7c0e 9001 7244 8805 9001 7224 6408 8805  |...rD....r$d...
-00000200: 1600 9001 7026 6409 7d0f 740e 6a0f 640a  ....p&d.}.t.j.d.
-00000210: 7c01 6a10 7c0f 640b 6a11 7c0e 8301 6603  |.j.|.d.j.|...f.
-00000220: 1600 8301 8201 8701 8702 6602 640c 6404  ..........f.d.d.
-00000230: 8408 8804 4400 8301 7d0d 7c08 9001 726a  ....D...}.|...rj
-00000240: 7412 7c0d 8301 7c08 640d 3c00 640e 7d10  t.|...|.d.<.d.}.
-00000250: 9001 782a 7c0d 4400 9001 5d20 7d11 79ca  ..x*|.D...] }.y.
-00000260: 7413 6a14 640f 6a15 7c11 7c10 6410 1700  t.j.d.j.|.|.d...
-00000270: 7412 7c0d 8301 8303 8301 0100 7416 7c11  t.|.........t.|.
-00000280: 8803 6602 7c0b 8e01 7d12 6700 7d13 6411  ..f.|...}.g.}.d.
-00000290: 7d14 6400 7d15 7832 7c12 6a17 4400 5d28  }.d.}.x2|.j.D.](
-000002a0: 7d16 7c14 0c00 9001 72d4 7c16 6a18 9001  }.|.....r.|.j...
-000002b0: 72d4 6412 7d14 7c15 6400 6b08 9001 72bc  r.d.}.|.d.k...r.
-000002c0: 7c16 7d15 9001 71bc 5700 7c14 0c00 9002  |.}...q.W.|.....
-000002d0: 7244 7c15 6400 6b09 9002 7244 7413 6a19  rD|.d.k...rDt.j.
-000002e0: 6413 6a15 7c11 7c15 6a1a 8302 8301 0100  d.j.|.|.j.......
-000002f0: 6412 7c15 5f18 7c13 6a1b 7c15 8301 0100  d.|._.|.j.|.....
-00000300: 6412 7c0b 6414 3c00 7416 7c11 8803 6602  d.|.d.<.t.|...f.
-00000310: 7c13 9e02 7c0b 8e01 7d12 741c 7c12 6415  |...|...}.t.|.d.
-00000320: 6412 8303 0100 5700 6e38 0400 740e 6a1d  d.....W.n8..t.j.
-00000330: 6b0a 9002 727e 0100 7d17 0100 7a18 7407  k...r~..}...z.t.
-00000340: 6a1e 6416 7c11 7c17 6602 1600 8301 0100  j.d.|.|.f.......
-00000350: 5700 5900 6400 6400 7d17 7e17 5800 6e02  W.Y.d.d.}.~.X.n.
-00000360: 5800 7c10 6410 3700 7d10 7c08 9001 7276  X.|.d.7.}.|...rv
-00000370: 7c10 7c08 6417 3c00 9001 7176 5700 5700  |.|.d.<...qvW.W.
-00000380: 6400 5100 5200 5800 6400 5300 2918 4e29  d.Q.R.X.d.S.).N)
-00000390: 055a 0d61 7574 6f6c 6f61 645f 7769 7468  .Z.autoload_with
-000003a0: da0f 6578 7465 6e64 5f65 7869 7374 696e  ..extend_existin
-000003b0: 67da 1061 7574 6f6c 6f61 645f 7265 706c  g..autoload_repl
-000003c0: 6163 65da 0b72 6573 6f6c 7665 5f66 6b73  ace..resolve_fks
-000003d0: 5a0a 5f65 7874 656e 645f 6f6e da06 7363  Z._extend_on..sc
-000003e0: 6865 6d61 6301 0000 0000 0000 0002 0000  hemac...........
-000003f0: 0005 0000 0013 0000 0073 1800 0000 6700  .........s....g.
-00000400: 7c00 5d10 7d01 6400 8800 7c01 6602 1600  |.].}.d...|.f...
-00000410: 9102 7104 5300 2901 7a05 2573 2e25 73a9  ..q.S.).z.%s.%s.
-00000420: 0029 02da 022e 30da 046e 616d 6529 0172  .)....0..name).r
-00000430: 0b00 0000 720c 0000 00fa 5e2f 5573 6572  ....r.....^/User
-00000440: 732f 6631 6e61 6c2f 4472 6f70 626f 782f  s/f1nal/Dropbox/
-00000450: 7079 7468 6f6e 2f6a 6574 2d62 7269 6467  python/jet-bridg
-00000460: 652f 7372 632f 7061 636b 6167 6573 2f6a  e/src/packages/j
-00000470: 6574 5f62 7269 6467 655f 6261 7365 2f6a  et_bridge_base/j
-00000480: 6574 5f62 7269 6467 655f 6261 7365 2f72  et_bridge_base/r
-00000490: 6566 6c65 6374 2e70 79fa 0a3c 6c69 7374  eflect.py..<list
-000004a0: 636f 6d70 3e30 0000 0073 0200 0000 0600  comp>0...s......
-000004b0: 7a1b 7265 666c 6563 742e 3c6c 6f63 616c  z.reflect.<local
-000004c0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-000004d0: 0000 0000 0000 0300 0000 0400 0000 1300  ................
-000004e0: 0000 7320 0000 0067 007c 005d 185c 027d  ..s ...g.|.].\.}
-000004f0: 017d 0288 0173 187c 0288 006b 0772 047c  .}...s.|...k.r.|
-00000500: 0191 0271 0453 0072 0c00 0000 720c 0000  ...q.S.r....r...
-00000510: 0029 0372 0d00 0000 720e 0000 00da 0773  .).r....r......s
-00000520: 6368 6e61 6d65 2902 da07 6375 7272 656e  chname)...curren
-00000530: 7472 0800 0000 720c 0000 0072 0f00 0000  tr....r....r....
-00000540: 7210 0000 0039 0000 0073 0400 0000 0601  r....9...s......
-00000550: 0601 6301 0000 0000 0000 0003 0000 0005  ..c.............
-00000560: 0000 0013 0000 0073 2a00 0000 6700 7c00  .......s*...g.|.
-00000570: 5d22 5c02 7d01 7d02 8801 7318 7c02 8800  ]"\.}.}...s.|...
-00000580: 6b07 7204 8803 7c01 8802 8302 7204 7c01  k.r...|.....r.|.
-00000590: 9102 7104 5300 720c 0000 0072 0c00 0000  ..q.S.r....r....
-000005a0: 2903 720d 0000 0072 0e00 0000 7211 0000  ).r....r....r...
-000005b0: 0029 0472 1200 0000 7208 0000 00da 086d  .).r....r......m
-000005c0: 6574 6164 6174 61da 046f 6e6c 7972 0c00  etadata..onlyr..
-000005d0: 0000 720f 0000 0072 1000 0000 3f00 0000  ..r....r....?...
-000005e0: 7306 0000 0006 0106 010c 0163 0100 0000  s..........c....
-000005f0: 0000 0000 0200 0000 0400 0000 1300 0000  ................
-00000600: 7318 0000 0067 007c 005d 107d 017c 0188  s....g.|.].}.|..
-00000610: 006b 0772 047c 0191 0271 0453 0072 0c00  .k.r.|...q.S.r..
-00000620: 0000 720c 0000 0029 0272 0d00 0000 720e  ..r....).r....r.
-00000630: 0000 0029 01da 0961 7661 696c 6162 6c65  ...)...available
-00000640: 720c 0000 0072 0f00 0000 7210 0000 0045  r....r....r....E
-00000650: 0000 0073 0200 0000 0600 7a0c 2073 6368  ...s......z. sch
-00000660: 656d 6120 2725 7327 da00 7a41 436f 756c  ema '%s'..zACoul
-00000670: 6420 6e6f 7420 7265 666c 6563 743a 2072  d not reflect: r
-00000680: 6571 7565 7374 6564 2074 6162 6c65 2873  equested table(s
-00000690: 2920 6e6f 7420 6176 6169 6c61 626c 6520  ) not available 
-000006a0: 696e 2025 7225 733a 2028 2573 297a 022c  in %r%s: (%s)z.,
-000006b0: 2063 0100 0000 0000 0000 0200 0000 0400   c..............
-000006c0: 0000 1300 0000 731c 0000 0067 007c 005d  ......s....g.|.]
-000006d0: 147d 0188 0173 147c 0188 006b 0772 047c  .}...s.|...k.r.|
-000006e0: 0191 0271 0453 0072 0c00 0000 720c 0000  ...q.S.r....r...
-000006f0: 0029 0272 0d00 0000 720e 0000 0029 0272  .).r....r....).r
-00000700: 1200 0000 7208 0000 0072 0c00 0000 720f  ....r....r....r.
-00000710: 0000 0072 1000 0000 4d00 0000 7304 0000  ...r....M...s...
-00000720: 0006 0102 015a 0c74 6162 6c65 735f 746f  .....Z.tables_to
-00000730: 7461 6c72 0100 0000 7a22 416e 616c 797a  talr....z"Analyz
-00000740: 696e 6720 7461 626c 6520 227b 7d22 2028  ing table "{}" (
-00000750: 7b7d 202f 207b 7d29 222e 2e2e e901 0000  {} / {})".......
-00000760: 0046 547a 3354 6162 6c65 2022 7b7d 2220  .FTz3Table "{}" 
-00000770: 6973 206d 6973 7369 6e67 2050 4b3a 2022  is missing PK: "
-00000780: 7b7d 2220 636f 6c75 6d6e 2077 6173 2073  {}" column was s
-00000790: 6574 2061 7320 504b 7208 0000 005a 0f5f  et as PKr....Z._
-000007a0: 5f6a 6574 5f61 7574 6f5f 706b 5f5f 7a15  _jet_auto_pk__z.
-000007b0: 536b 6970 7069 6e67 2074 6162 6c65 2025  Skipping table %
-000007c0: 733a 2025 735a 1074 6162 6c65 735f 7072  s: %sZ.tables_pr
-000007d0: 6f63 6573 7365 6429 1f72 0200 0000 7205  ocessed).r....r.
-000007e0: 0000 00da 0769 6e73 7065 6374 5a13 5f69  .....inspectZ._i
-000007f0: 6e73 7065 6374 696f 6e5f 636f 6e74 6578  nspection_contex
-00000800: 74da 0373 6574 da06 7570 6461 7465 720b  t..set..updater.
-00000810: 0000 0072 0600 0000 5a0a 4f72 6465 7265  ...r....Z.Ordere
-00000820: 6453 6574 5a0f 6765 745f 7461 626c 655f  dSetZ.get_table_
-00000830: 6e61 6d65 735a 0e67 6574 5f76 6965 775f  namesZ.get_view_
-00000840: 6e61 6d65 73da 0674 6162 6c65 73da 037a  names..tables..z
-00000850: 6970 da08 6361 6c6c 6162 6c65 7204 0000  ip..callabler...
-00000860: 005a 1349 6e76 616c 6964 5265 7175 6573  .Z.InvalidReques
-00000870: 7445 7272 6f72 da06 656e 6769 6e65 da04  tError..engine..
-00000880: 6a6f 696e da03 6c65 6e72 0700 0000 da04  join..lenr......
-00000890: 696e 666f da06 666f 726d 6174 7203 0000  info..formatr...
-000008a0: 00da 0763 6f6c 756d 6e73 da0b 7072 696d  ...columns..prim
-000008b0: 6172 795f 6b65 79da 0777 6172 6e69 6e67  ary_key..warning
-000008c0: 720e 0000 00da 0661 7070 656e 64da 0773  r......append..s
-000008d0: 6574 6174 7472 5a17 556e 7265 666c 6563  etattrZ.Unreflec
-000008e0: 7461 626c 6554 6162 6c65 4572 726f 72da  tableTableError.
-000008f0: 0477 6172 6e29 1872 1300 0000 da04 6269  .warn).r......bi
-00000900: 6e64 720b 0000 005a 0576 6965 7773 7214  ndr....Z.viewsr.
-00000910: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00000920: 0000 da12 7065 6e64 696e 675f 636f 6e6e  ....pending_conn
-00000930: 6563 7469 6f6e 5a0e 6469 616c 6563 745f  ectionZ.dialect_
-00000940: 6b77 6172 6773 5a04 696e 7370 5a0c 7265  kwargsZ.inspZ.re
-00000950: 666c 6563 745f 6f70 7473 5a12 6176 6169  flect_optsZ.avai
-00000960: 6c61 626c 655f 775f 7363 6865 6d61 da04  lable_w_schema..
-00000970: 6c6f 6164 da07 6d69 7373 696e 67da 0173  load..missing..s
-00000980: da01 6972 0e00 0000 da05 7461 626c 65da  ..ir......table.
-00000990: 0461 7267 735a 0668 6173 5f70 6b5a 0c66  .argsZ.has_pkZ.f
-000009a0: 6972 7374 5f63 6f6c 756d 6eda 0469 7465  irst_column..ite
-000009b0: 6d5a 0475 6572 7272 0c00 0000 2906 7215  mZ.uerrr....).r.
-000009c0: 0000 0072 1200 0000 7208 0000 0072 1300  ...r....r....r..
-000009d0: 0000 7214 0000 0072 0b00 0000 720f 0000  ..r....r....r...
-000009e0: 00da 0772 6566 6c65 6374 0a00 0000 737e  ...reflect....s~
-000009f0: 0000 0000 0c08 0108 0212 0202 0102 0102  ................
-00000a00: 0102 010a 030a 0208 0106 0208 0108 0210  ................
-00000a10: 0104 0110 0208 0104 0116 0304 020a 0208  ................
-00000a20: 020c 0110 0308 0210 0110 0512 0106 0114  ................
-00000a30: 0104 0102 0116 030c 0108 0806 010c 0204  ................
-00000a40: 010e 0102 011c 010e 0204 0104 0104 020c  ................
-00000a50: 0110 0104 010a 010a 0212 0114 0206 010a  ................
-00000a60: 0108 0112 0110 0314 0124 0208 0206 0118  .........$......
-00000a70: 0472 3200 0000 2908 4e4e 464e 4654 544e  .r2...).NNFNFTTN
-00000a80: 290a 5a13 7371 6c61 6c63 6865 6d79 2e73  ).Z.sqlalchemy.s
-00000a90: 716c 2e62 6173 6572 0200 0000 da0a 7371  ql.baser......sq
-00000aa0: 6c61 6c63 6865 6d79 7203 0000 0072 0400  lalchemyr....r..
-00000ab0: 0000 7205 0000 0072 0600 0000 da16 6a65  ..r....r......je
-00000ac0: 745f 6272 6964 6765 5f62 6173 652e 6c6f  t_bridge_base.lo
-00000ad0: 6767 6572 7207 0000 0072 3200 0000 720c  ggerr....r2...r.
-00000ae0: 0000 0072 0c00 0000 720c 0000 0072 0f00  ...r....r....r..
-00000af0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000b00: 731a 0000 000c 010c 010c 010c 010c 020c  s...............
-00000b10: 0500 0100 0100 0100 0100 0100 0100 01    ...............
+00000060: 0100 6400 6406 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6407 6c09 6d0a 5a0a 0100 6400 6408 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0c 5a0c 0100 6410 640b 640c 8401 5a0d  m.Z...d.d.d...Z.
+00000090: 6411 640e 640f 8401 5a0e 6409 5300 2912  d.d.d...Z.d.S.).
+000000a0: e900 0000 0029 01da 0e5f 6269 6e64 5f6f  .....)..._bind_o
+000000b0: 725f 6572 726f 7229 01da 0554 6162 6c65  r_error)...Table
+000000c0: 2901 da03 6578 6329 01da 0a69 6e73 7065  )...exc)...inspe
+000000d0: 6374 696f 6e29 01da 0475 7469 6c29 01da  ction)...util)..
+000000e0: 0873 6574 7469 6e67 7329 01da 066c 6f67  .settings)...log
+000000f0: 6765 7229 01da 1667 6574 5f6d 656d 6f72  ger)...get_memor
+00000100: 795f 7573 6167 655f 6875 6d61 6e4e 4663  y_usage_humanNFc
+00000110: 0700 0000 0000 0000 0c00 0000 0600 0000  ................
+00000120: 0300 0000 7306 0100 0067 007d 0774 006a  ....s....g.}.t.j
+00000130: 017c 006a 0288 0583 0183 0189 007c 0472  .|.j.........|.r
+00000140: 2c7c 006a 0388 0583 017d 0788 006a 047c  ,|.j.....}...j.|
+00000150: 0783 0101 0088 0564 006b 0972 4e74 006a  .......d.k.rNt.j
+00000160: 0187 0566 0164 0164 0284 0888 0044 0083  ...f.d.d.....D..
+00000170: 0183 017d 086e 0488 007d 0874 0588 036a  ...}.n...}.t...j
+00000180: 0683 0189 0188 0464 006b 0872 8087 0187  .......d.k.r....
+00000190: 0266 0264 0364 0284 0874 0788 007c 0883  .f.d.d...t...|..
+000001a0: 0244 0083 017d 096e 7e74 0888 0483 0172  .D...}.n~t.....r
+000001b0: a887 0187 0287 0387 0466 0464 0464 0284  .........f.d.d..
+000001c0: 0874 0788 007c 0883 0244 0083 017d 096e  .t...|...D...}.n
+000001d0: 5687 0066 0164 0564 0284 0888 0444 0083  V..f.d.d.....D..
+000001e0: 017d 0a7c 0a72 ea88 0572 ca64 0688 0516  .}.|.r...r.d....
+000001f0: 0070 cc64 077d 0b74 096a 0a64 087c 026a  .p.d.}.t.j.d.|.j
+00000200: 0b7c 0b64 096a 0c7c 0a83 0166 0316 0083  .|.d.j.|...f....
+00000210: 0182 0187 0187 0266 0264 0a64 0284 0888  .......f.d.d....
+00000220: 0444 0083 017d 097c 097c 0766 0253 0029  .D...}.|.|.f.S.)
+00000230: 0b4e 6301 0000 0000 0000 0002 0000 0005  .Nc.............
+00000240: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
+00000250: 5d10 7d01 6400 8800 7c01 6602 1600 9102  ].}.d...|.f.....
+00000260: 7104 5300 2901 7a05 2573 2e25 73a9 0029  q.S.).z.%s.%s..)
+00000270: 02da 022e 30da 046e 616d 6529 01da 0673  ....0..name)...s
+00000280: 6368 656d 6172 0a00 0000 fa5e 2f55 7365  chemar.....^/Use
+00000290: 7273 2f66 316e 616c 2f44 726f 7062 6f78  rs/f1nal/Dropbox
+000002a0: 2f70 7974 686f 6e2f 6a65 742d 6272 6964  /python/jet-brid
+000002b0: 6765 2f73 7263 2f70 6163 6b61 6765 732f  ge/src/packages/
+000002c0: 6a65 745f 6272 6964 6765 5f62 6173 652f  jet_bridge_base/
+000002d0: 6a65 745f 6272 6964 6765 5f62 6173 652f  jet_bridge_base/
+000002e0: 7265 666c 6563 742e 7079 fa0a 3c6c 6973  reflect.py..<lis
+000002f0: 7463 6f6d 703e 1e00 0000 7302 0000 0006  tcomp>....s.....
+00000300: 007a 1e67 6574 5f74 6162 6c65 732e 3c6c  .z.get_tables.<l
+00000310: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000320: 3e63 0100 0000 0000 0000 0300 0000 0400  >c..............
+00000330: 0000 1300 0000 7320 0000 0067 007c 005d  ......s ...g.|.]
+00000340: 185c 027d 017d 0288 0173 187c 0288 006b  .\.}.}...s.|...k
+00000350: 0772 047c 0191 0271 0453 0072 0a00 0000  .r.|...q.S.r....
+00000360: 720a 0000 0029 0372 0b00 0000 720c 0000  r....).r....r...
+00000370: 00da 0773 6368 6e61 6d65 2902 da07 6375  ...schname)...cu
+00000380: 7272 656e 74da 0f65 7874 656e 645f 6578  rrent..extend_ex
+00000390: 6973 7469 6e67 720a 0000 0072 0e00 0000  istingr....r....
+000003a0: 720f 0000 0027 0000 0073 0400 0000 0601  r....'...s......
+000003b0: 0601 6301 0000 0000 0000 0003 0000 0005  ..c.............
+000003c0: 0000 0013 0000 0073 2a00 0000 6700 7c00  .......s*...g.|.
+000003d0: 5d22 5c02 7d01 7d02 8801 7318 7c02 8800  ]"\.}.}...s.|...
+000003e0: 6b07 7204 8803 7c01 8802 8302 7204 7c01  k.r...|.....r.|.
+000003f0: 9102 7104 5300 720a 0000 0072 0a00 0000  ..q.S.r....r....
+00000400: 2903 720b 0000 0072 0c00 0000 7210 0000  ).r....r....r...
+00000410: 0029 0472 1100 0000 7212 0000 00da 086d  .).r....r......m
+00000420: 6574 6164 6174 61da 046f 6e6c 7972 0a00  etadata..onlyr..
+00000430: 0000 720e 0000 0072 0f00 0000 2d00 0000  ..r....r....-...
+00000440: 7306 0000 0006 0106 010c 0163 0100 0000  s..........c....
+00000450: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00000460: 7318 0000 0067 007c 005d 107d 017c 0188  s....g.|.].}.|..
+00000470: 006b 0772 047c 0191 0271 0453 0072 0a00  .k.r.|...q.S.r..
+00000480: 0000 720a 0000 0029 0272 0b00 0000 720c  ..r....).r....r.
+00000490: 0000 0029 01da 0961 7661 696c 6162 6c65  ...)...available
+000004a0: 720a 0000 0072 0e00 0000 720f 0000 0033  r....r....r....3
+000004b0: 0000 0073 0200 0000 0600 7a0c 2073 6368  ...s......z. sch
+000004c0: 656d 6120 2725 7327 da00 7a41 436f 756c  ema '%s'..zACoul
+000004d0: 6420 6e6f 7420 7265 666c 6563 743a 2072  d not reflect: r
+000004e0: 6571 7565 7374 6564 2074 6162 6c65 2873  equested table(s
+000004f0: 2920 6e6f 7420 6176 6169 6c61 626c 6520  ) not available 
+00000500: 696e 2025 7225 733a 2028 2573 297a 022c  in %r%s: (%s)z.,
+00000510: 2063 0100 0000 0000 0000 0200 0000 0400   c..............
+00000520: 0000 1300 0000 731c 0000 0067 007c 005d  ......s....g.|.]
+00000530: 147d 0188 0173 147c 0188 006b 0772 047c  .}...s.|...k.r.|
+00000540: 0191 0271 0453 0072 0a00 0000 720a 0000  ...q.S.r....r...
+00000550: 0029 0272 0b00 0000 720c 0000 0029 0272  .).r....r....).r
+00000560: 1100 0000 7212 0000 0072 0a00 0000 720e  ....r....r....r.
+00000570: 0000 0072 0f00 0000 3b00 0000 7304 0000  ...r....;...s...
+00000580: 0006 0102 0129 0d72 0600 0000 da0a 4f72  .....).r......Or
+00000590: 6465 7265 6453 6574 da0f 6765 745f 7461  deredSet..get_ta
+000005a0: 626c 655f 6e61 6d65 73da 0e67 6574 5f76  ble_names..get_v
+000005b0: 6965 775f 6e61 6d65 73da 0675 7064 6174  iew_names..updat
+000005c0: 65da 0373 6574 da06 7461 626c 6573 da03  e..set..tables..
+000005d0: 7a69 70da 0863 616c 6c61 626c 6572 0400  zip..callabler..
+000005e0: 0000 da13 496e 7661 6c69 6452 6571 7565  ....InvalidReque
+000005f0: 7374 4572 726f 72da 0665 6e67 696e 65da  stError..engine.
+00000600: 046a 6f69 6e29 0cda 0469 6e73 7072 1300  .join)...inspr..
+00000610: 0000 da04 6269 6e64 720d 0000 00da 0576  ....bindr......v
+00000620: 6965 7773 7214 0000 0072 1200 0000 da0a  iewsr....r......
+00000630: 7669 6577 5f6e 616d 6573 da12 6176 6169  view_names..avai
+00000640: 6c61 626c 655f 775f 7363 6865 6d61 da04  lable_w_schema..
+00000650: 6c6f 6164 da07 6d69 7373 696e 67da 0173  load..missing..s
+00000660: 720a 0000 0029 0672 1500 0000 7211 0000  r....).r....r...
+00000670: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000680: 720d 0000 0072 0e00 0000 da0a 6765 745f  r....r......get_
+00000690: 7461 626c 6573 0c00 0000 7332 0000 0000  tables....s2....
+000006a0: 0904 0210 0104 010a 010a 0208 0104 0116  ................
+000006b0: 0304 020a 0208 020c 0110 0308 0210 0110  ................
+000006c0: 0512 0104 0110 0104 0102 0116 030c 0108  ................
+000006d0: 0472 2a00 0000 5463 0a00 0000 0000 0000  .r*...Tc........
+000006e0: 1700 0000 1a00 0000 4b00 0000 7318 0200  ........K...s...
+000006f0: 007c 0264 006b 0872 1074 007c 0183 017d  .|.d.k.r.t.|...}
+00000700: 0274 016a 027c 0283 016a 0383 0090 018f  .t.j.|...j......
+00000710: ee7d 0b7c 0b7c 067c 077c 0874 0483 0064  .}.|.|.|.|.t...d
+00000720: 019c 057d 0c7c 0c6a 057c 0a83 0101 007c  ...}.|.j.|.....|
+00000730: 0364 006b 0872 4c7c 016a 067d 037c 0364  .d.k.rL|.j.}.|.d
+00000740: 006b 0972 5c7c 037c 0c64 023c 0074 077c  .k.r\|.|.d.<.t.|
+00000750: 0b7c 017c 027c 037c 047c 057c 0683 075c  .|.|.|.|.|.|...\
+00000760: 027d 0d7d 0e7c 0972 8474 087c 0d83 017c  .}.}.|.r.t.|...|
+00000770: 0964 033c 0064 047d 0f90 0178 7e7c 0d44  .d.<.d.}...x~|.D
+00000780: 0090 015d 747d 107c 1064 116b 0672 a071  ...]t}.|.d.k.r.q
+00000790: 9079 ea74 096a 0a64 066a 0b7c 007c 107c  .y.t.j.d.j.|.|.|
+000007a0: 0f64 0717 0074 087c 0d83 0174 0c83 0083  .d...t.|...t....
+000007b0: 0583 0101 0074 0d7c 107c 0166 027c 0c8e  .....t.|.|.f.|..
+000007c0: 017d 117c 0e72 ea7c 107c 0e6b 0672 ea74  .}.|.r.|.|.k.r.t
+000007d0: 0e7c 1164 0864 0983 0301 0067 007d 1264  .|.d.d.....g.}.d
+000007e0: 0a7d 1364 007d 1478 327c 116a 0f44 005d  .}.d.}.x2|.j.D.]
+000007f0: 287d 157c 130c 0090 0172 167c 156a 1090  (}.|.....r.|.j..
+00000800: 0172 1664 097d 137c 1464 006b 0890 0072  .r.d.}.|.d.k...r
+00000810: fe7c 157d 1490 0071 fe57 007c 130c 0090  .|.}...q.W.|....
+00000820: 0172 887c 1464 006b 0990 0172 8874 096a  .r.|.d.k...r.t.j
+00000830: 1164 0b6a 0b7c 007c 107c 146a 1283 0383  .d.j.|.|.|.j....
+00000840: 0101 0064 097c 145f 107c 126a 137c 1483  ...d.|._.|.j.|..
+00000850: 0101 0064 097c 0c64 0c3c 0074 0d7c 107c  ...d.|.d.<.t.|.|
+00000860: 0166 027c 129e 027c 0c8e 017d 1174 0e7c  .f.|...|...}.t.|
+00000870: 1164 0d64 0983 0301 0057 006e 3804 0074  .d.d.....W.n8..t
+00000880: 146a 156b 0a90 0172 c201 007d 1601 007a  .j.k...r...}...z
+00000890: 1874 166a 1764 0e7c 107c 1666 0216 0083  .t.j.d.|.|.f....
+000008a0: 0101 0057 0059 0064 0064 007d 167e 1658  ...W.Y.d.d.}.~.X
+000008b0: 006e 0258 007c 0f64 0737 007d 0f74 186a  .n.X.|.d.7.}.t.j
+000008c0: 1964 006b 0990 0172 fa7c 0f74 186a 196b  .d.k...r.|.t.j.k
+000008d0: 0590 0172 fa74 096a 1164 0f6a 0b7c 0074  ...r.t.j.d.j.|.t
+000008e0: 186a 1983 0283 0101 0050 007c 0972 907c  .j.......P.|.r.|
+000008f0: 0f7c 0964 103c 0071 9057 0057 0064 0051  .|.d.<.q.W.W.d.Q
+00000900: 0052 0058 0064 0053 0029 124e 2905 da0d  .R.X.d.S.).N)...
+00000910: 6175 746f 6c6f 6164 5f77 6974 6872 1200  autoload_withr..
+00000920: 0000 da10 6175 746f 6c6f 6164 5f72 6570  ....autoload_rep
+00000930: 6c61 6365 da0b 7265 736f 6c76 655f 666b  lace..resolve_fk
+00000940: 73da 0a5f 6578 7465 6e64 5f6f 6e72 0d00  s.._extend_onr..
+00000950: 0000 5a0c 7461 626c 6573 5f74 6f74 616c  ..Z.tables_total
+00000960: 7201 0000 00da 1270 675f 7374 6174 5f73  r......pg_stat_s
+00000970: 7461 7465 6d65 6e74 737a 305b 7b7d 5d20  tatementsz0[{}] 
+00000980: 416e 616c 797a 696e 6720 7461 626c 6520  Analyzing table 
+00000990: 227b 7d22 2028 7b7d 202f 207b 7d29 2220  "{}" ({} / {})" 
+000009a0: 284d 656d 3a7b 7d29 2e2e 2ee9 0100 0000  (Mem:{})........
+000009b0: 5a0f 5f5f 6a65 745f 6973 5f76 6965 775f  Z.__jet_is_view_
+000009c0: 5f54 467a 385b 7b7d 5d20 5461 626c 6520  _TFz8[{}] Table 
+000009d0: 227b 7d22 2069 7320 6d69 7373 696e 6720  "{}" is missing 
+000009e0: 504b 3a20 227b 7d22 2063 6f6c 756d 6e20  PK: "{}" column 
+000009f0: 7761 7320 7365 7420 6173 2050 4b72 1200  was set as PKr..
+00000a00: 0000 5a0f 5f5f 6a65 745f 6175 746f 5f70  ..Z.__jet_auto_p
+00000a10: 6b5f 5f7a 1553 6b69 7070 696e 6720 7461  k__z.Skipping ta
+00000a20: 626c 6520 2573 3a20 2573 7a22 5b7b 7d5d  ble %s: %sz"[{}]
+00000a30: 204d 6178 2074 6162 6c65 7320 6c69 6d69   Max tables limi
+00000a40: 7420 287b 7d29 2072 6561 6368 6564 5a10  t ({}) reachedZ.
+00000a50: 7461 626c 6573 5f70 726f 6365 7373 6564  tables_processed
+00000a60: 2901 722f 0000 0029 1a72 0200 0000 7205  ).r/...).r....r.
+00000a70: 0000 00da 0769 6e73 7065 6374 da13 5f69  .....inspect.._i
+00000a80: 6e73 7065 6374 696f 6e5f 636f 6e74 6578  nspection_contex
+00000a90: 7472 1b00 0000 721a 0000 0072 0d00 0000  tr....r....r....
+00000aa0: 722a 0000 00da 036c 656e 7208 0000 00da  r*.....lenr.....
+00000ab0: 0469 6e66 6fda 0666 6f72 6d61 7472 0900  .info..formatr..
+00000ac0: 0000 7203 0000 00da 0773 6574 6174 7472  ..r......setattr
+00000ad0: da07 636f 6c75 6d6e 73da 0b70 7269 6d61  ..columns..prima
+00000ae0: 7279 5f6b 6579 da07 7761 726e 696e 6772  ry_key..warningr
+00000af0: 0c00 0000 da06 6170 7065 6e64 7204 0000  ......appendr...
+00000b00: 00da 1755 6e72 6566 6c65 6374 6162 6c65  ...Unreflectable
+00000b10: 5461 626c 6545 7272 6f72 7206 0000 00da  TableErrorr.....
+00000b20: 0477 6172 6e72 0700 0000 da13 4441 5441  .warnr......DATA
+00000b30: 4241 5345 5f4d 4158 5f54 4142 4c45 5329  BASE_MAX_TABLES)
+00000b40: 175a 0963 6964 5f73 686f 7274 7213 0000  .Z.cid_shortr...
+00000b50: 0072 2300 0000 720d 0000 0072 2400 0000  .r#...r....r$...
+00000b60: 7214 0000 0072 1200 0000 722c 0000 0072  r....r....r,...r
+00000b70: 2d00 0000 da12 7065 6e64 696e 675f 636f  -.....pending_co
+00000b80: 6e6e 6563 7469 6f6e da0e 6469 616c 6563  nnection..dialec
+00000b90: 745f 6b77 6172 6773 7222 0000 00da 0c72  t_kwargsr".....r
+00000ba0: 6566 6c65 6374 5f6f 7074 7372 2700 0000  eflect_optsr'...
+00000bb0: 7225 0000 00da 0169 720c 0000 00da 0574  r%.....ir......t
+00000bc0: 6162 6c65 da04 6172 6773 da06 6861 735f  able..args..has_
+00000bd0: 706b 5a0c 6669 7273 745f 636f 6c75 6d6e  pkZ.first_column
+00000be0: da04 6974 656d da04 7565 7272 720a 0000  ..item..uerrr...
+00000bf0: 0072 0a00 0000 720e 0000 00da 0772 6566  .r....r......ref
+00000c00: 6c65 6374 4300 0000 7362 0000 0000 0d08  lectC...sb......
+00000c10: 0108 0212 0202 0102 0102 0102 010a 030a  ................
+00000c20: 0208 0106 0208 0108 0218 0604 010c 0204  ................
+00000c30: 010e 0108 0102 0202 0122 010e 020c 010c  ........."......
+00000c40: 0204 0104 0104 020c 0110 0104 010a 010a  ................
+00000c50: 0212 0116 0206 010a 0108 0112 0110 0314  ................
+00000c60: 0124 0208 0218 0114 0102 0204 0116 0472  .$.............r
+00000c70: 4700 0000 2905 4e4e 464e 4629 084e 4e46  G...).NNFNF).NNF
+00000c80: 4e46 5454 4e29 0f5a 1373 716c 616c 6368  NFTTN).Z.sqlalch
+00000c90: 656d 792e 7371 6c2e 6261 7365 7202 0000  emy.sql.baser...
+00000ca0: 00da 0a73 716c 616c 6368 656d 7972 0300  ...sqlalchemyr..
+00000cb0: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
+00000cc0: 00da 0f6a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
+00000cd0: 7365 7207 0000 00da 166a 6574 5f62 7269  ser......jet_bri
+00000ce0: 6467 655f 6261 7365 2e6c 6f67 6765 7272  dge_base.loggerr
+00000cf0: 0800 0000 da1d 6a65 745f 6272 6964 6765  ......jet_bridge
+00000d00: 5f62 6173 652e 7574 696c 732e 7072 6f63  _base.utils.proc
+00000d10: 6573 7372 0900 0000 722a 0000 0072 4700  essr....r*...rG.
+00000d20: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00000d30: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000d40: 0100 0000 7328 0000 000c 010c 010c 010c  ....s(..........
+00000d50: 010c 020c 010c 010c 0600 0100 0100 0100  ................
+00000d60: 010a 3300 0100 0100 0100 0100 0100 0100  ..3.............
+00000d70: 01                                       .
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/logger.py` & `jet-bridge-base-1.8.2/jet_bridge_base/logger.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/api.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/request_error.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/request_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/not_found.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/not_found.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/sql.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/sql.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/sql.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/sql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/missing_argument_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/not_found.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/not_found.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/request_error.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/request_error.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/permission_denied.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/validation_error.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-00000000: 330d 0d0a 5c73 7063 fa00 0000 e300 0000  3...\spc........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2c00 0000 6400 6401 6c00 6d01 5a01  .s,...d.d.l.m.Z.
-00000030: 0100 6400 6402 6c02 6d03 5a03 0100 4700  ..d.d.l.m.Z...G.
-00000040: 6403 6404 8400 6404 6503 8303 5a04 6405  d.d...d.e...Z.d.
-00000050: 5300 2906 e900 0000 0029 01da 0673 7461  S.)......)...sta
-00000060: 7475 7329 01da 0c41 5049 4578 6365 7074  tus)...APIExcept
-00000070: 696f 6e63 0000 0000 0000 0000 0000 0000  ionc............
-00000080: 0100 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
-00000090: 0164 005a 0264 015a 0364 025a 0465 056a  .d.Z.d.Z.d.Z.e.j
-000000a0: 065a 0764 0353 0029 04da 0f56 616c 6964  .Z.d.S.)...Valid
-000000b0: 6174 696f 6e45 7272 6f72 7a0d 696e 7661  ationErrorz.inva
-000000c0: 6c69 6420 696e 7075 74da 0769 6e76 616c  lid input..inval
-000000d0: 6964 4e29 08da 085f 5f6e 616d 655f 5fda  idN)...__name__.
-000000e0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000000f0: 7561 6c6e 616d 655f 5fda 0e64 6566 6175  ualname__..defau
-00000100: 6c74 5f64 6574 6169 6cda 0c64 6566 6175  lt_detail..defau
-00000110: 6c74 5f63 6f64 6572 0200 0000 da14 4854  lt_coder......HT
-00000120: 5450 5f34 3030 5f42 4144 5f52 4551 5545  TP_400_BAD_REQUE
-00000130: 5354 da13 6465 6661 756c 745f 7374 6174  ST..default_stat
-00000140: 7573 5f63 6f64 65a9 0072 0d00 0000 720d  us_code..r....r.
-00000150: 0000 00fa 722f 5573 6572 732f 6631 6e61  ....r/Users/f1na
-00000160: 6c2f 4472 6f70 626f 782f 7079 7468 6f6e  l/Dropbox/python
-00000170: 2f6a 6574 2d62 7269 6467 652f 7372 632f  /jet-bridge/src/
-00000180: 7061 636b 6167 6573 2f6a 6574 5f62 7269  packages/jet_bri
-00000190: 6467 655f 6261 7365 2f6a 6574 5f62 7269  dge_base/jet_bri
-000001a0: 6467 655f 6261 7365 2f65 7863 6570 7469  dge_base/excepti
-000001b0: 6f6e 732f 7661 6c69 6461 7469 6f6e 5f65  ons/validation_e
-000001c0: 7272 6f72 2e70 7972 0400 0000 0500 0000  rror.pyr........
-000001d0: 7306 0000 0008 0104 0104 0172 0400 0000  s..........r....
-000001e0: 4e29 05da 0f6a 6574 5f62 7269 6467 655f  N)...jet_bridge_
-000001f0: 6261 7365 7202 0000 00da 1e6a 6574 5f62  baser......jet_b
-00000200: 7269 6467 655f 6261 7365 2e65 7863 6570  ridge_base.excep
-00000210: 7469 6f6e 732e 6170 6972 0300 0000 7204  tions.apir....r.
-00000220: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000230: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000240: 3e01 0000 0073 0400 0000 0c01 0c03       >....s........
+00000000: 420d 0d0a 0000 0000 5c73 7063 fa00 0000  B.......\spc....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 2c00 0000 6400 6401 6c00  .@...s,...d.d.l.
+00000030: 6d01 5a01 0100 6400 6402 6c02 6d03 5a03  m.Z...d.d.l.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 8303  ..G.d.d...d.e...
+00000050: 5a04 6405 5300 2906 e900 0000 0029 01da  Z.d.S.)......)..
+00000060: 0673 7461 7475 7329 01da 0c41 5049 4578  .status)...APIEx
+00000070: 6365 7074 696f 6e63 0000 0000 0000 0000  ceptionc........
+00000080: 0000 0000 0100 0000 4000 0000 731a 0000  ........@...s...
+00000090: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+000000a0: 0465 056a 065a 0764 0353 0029 04da 0f56  .e.j.Z.d.S.)...V
+000000b0: 616c 6964 6174 696f 6e45 7272 6f72 7a0d  alidationErrorz.
+000000c0: 696e 7661 6c69 6420 696e 7075 74da 0769  invalid input..i
+000000d0: 6e76 616c 6964 4e29 08da 085f 5f6e 616d  nvalidN)...__nam
+000000e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000000f0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0e64  .__qualname__..d
+00000100: 6566 6175 6c74 5f64 6574 6169 6cda 0c64  efault_detail..d
+00000110: 6566 6175 6c74 5f63 6f64 6572 0200 0000  efault_coder....
+00000120: da14 4854 5450 5f34 3030 5f42 4144 5f52  ..HTTP_400_BAD_R
+00000130: 4551 5545 5354 da13 6465 6661 756c 745f  EQUEST..default_
+00000140: 7374 6174 7573 5f63 6f64 65a9 0072 0d00  status_code..r..
+00000150: 0000 720d 0000 00fa 722f 5573 6572 732f  ..r.....r/Users/
+00000160: 6631 6e61 6c2f 4472 6f70 626f 782f 7079  f1nal/Dropbox/py
+00000170: 7468 6f6e 2f6a 6574 2d62 7269 6467 652f  thon/jet-bridge/
+00000180: 7372 632f 7061 636b 6167 6573 2f6a 6574  src/packages/jet
+00000190: 5f62 7269 6467 655f 6261 7365 2f6a 6574  _bridge_base/jet
+000001a0: 5f62 7269 6467 655f 6261 7365 2f65 7863  _bridge_base/exc
+000001b0: 6570 7469 6f6e 732f 7661 6c69 6461 7469  eptions/validati
+000001c0: 6f6e 5f65 7272 6f72 2e70 7972 0400 0000  on_error.pyr....
+000001d0: 0500 0000 7306 0000 0008 0104 0104 0172  ....s..........r
+000001e0: 0400 0000 4e29 05da 0f6a 6574 5f62 7269  ....N)...jet_bri
+000001f0: 6467 655f 6261 7365 7202 0000 00da 1e6a  dge_baser......j
+00000200: 6574 5f62 7269 6467 655f 6261 7365 2e65  et_bridge_base.e
+00000210: 7863 6570 7469 6f6e 732e 6170 6972 0300  xceptions.apir..
+00000220: 0000 7204 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000230: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
+00000240: 6475 6c65 3e01 0000 0073 0400 0000 0c01  dule>....s......
+00000250: 0c03                                     ..
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/__pycache__/api.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/__pycache__/api.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/exceptions/api.py` & `jet-bridge-base-1.8.2/jet_bridge_base/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/model_group.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/model_group.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/relationship_override.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/relationship_override.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/reset_order.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/reset_order.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_group.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_group.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/serializer.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/serializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/serializer.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/serializer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/sql.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/sql.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 06b2 0a64 1335 0000 e300 0000  3......d.5......
+00000000: 330d 0d0a 308e c364 8f36 0000 e300 0000  3...0..d.6......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6c01 0000 6400 6401 6c00 6d01 5a01  .sl...d.d.l.m.Z.
 00000030: 6d02 5a02 0100 6400 6402 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000040: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d09 5a09 6d0a 5a0a 0100 6400 6403 6c03  m.Z.m.Z...d.d.l.
 00000060: 6d0b 5a0b 0100 6400 6404 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0e 6d0f 5a0f 0100 6400  ..d.d.l.m.Z...d.
@@ -471,297 +471,307 @@
 00001d60: 0000 0072 0800 0000 2904 724c 0000 0072  ...r....).rL...r
 00001d70: 2100 0000 da0a 6465 7363 656e 6469 6e67  !.....descending
 00001d80: 7286 0000 0072 2300 0000 7223 0000 0072  r....r#...r#...r
 00001d90: 2400 0000 da0f 6d61 705f 6f72 6465 725f  $.....map_order_
 00001da0: 6669 656c 64e1 0000 0073 1000 0000 0001  field....s......
 00001db0: 0401 0a01 0c01 0401 0801 0401 0801 7a1d  ..............z.
 00001dc0: 5371 6c53 6572 6961 6c69 7a65 722e 6d61  SqlSerializer.ma
-00001dd0: 705f 6f72 6465 725f 6669 656c 6463 0300  p_order_fieldc..
-00001de0: 0000 0000 0000 0400 0000 0500 0000 0300  ................
-00001df0: 0000 7330 0000 0064 017c 026b 0672 2c74  ..s0...d.|.k.r,t
+00001dd0: 705f 6f72 6465 725f 6669 656c 6463 0400  p_order_fieldc..
+00001de0: 0000 0000 0000 0700 0000 0500 0000 0300  ................
+00001df0: 0000 7384 0000 0064 017c 026b 0672 2e74  ..s....d.|.k.r.t
 00001e00: 0074 0187 0066 0164 0264 0384 087c 0264  .t...f.d.d...|.d
-00001e10: 0119 0083 0283 017d 037c 016a 027c 038e  .......}.|.j.|..
-00001e20: 007d 017c 0153 0029 044e 726a 0000 0063  .}.|.S.).Nrj...c
-00001e30: 0100 0000 0000 0000 0100 0000 0200 0000  ................
-00001e40: 1300 0000 730a 0000 0088 006a 007c 0083  ....s......j.|..
-00001e50: 0153 0029 014e 2901 7298 0000 0029 0172  .S.).N).r....).r
-00001e60: 4100 0000 2901 724c 0000 0072 2300 0000  A...).rL...r#...
-00001e70: 7224 0000 0072 4300 0000 ed00 0000 7300  r$...rC.......s.
-00001e80: 0000 007a 2d53 716c 5365 7269 616c 697a  ...z-SqlSerializ
-00001e90: 6572 2e73 6f72 745f 7175 6572 7973 6574  er.sort_queryset
-00001ea0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00001eb0: 613e 2903 7267 0000 0072 4a00 0000 726a  a>).rg...rJ...rj
-00001ec0: 0000 0029 0472 4c00 0000 726d 0000 0072  ...).rL...rm...r
-00001ed0: 5600 0000 726a 0000 0072 2300 0000 2901  V...rj...r#...).
-00001ee0: 724c 0000 0072 2400 0000 da0d 736f 7274  rL...r$.....sort
-00001ef0: 5f71 7565 7279 7365 74eb 0000 0073 0800  _queryset....s..
-00001f00: 0000 0001 0801 1a01 0a02 7a1b 5371 6c53  ..........z.SqlS
-00001f10: 6572 6961 6c69 7a65 722e 736f 7274 5f71  erializer.sort_q
-00001f20: 7565 7279 7365 7463 0200 0000 0000 0000  uerysetc........
-00001f30: 1300 0000 2e00 0000 0300 0000 7352 0300  ............sR..
-00001f40: 007c 006a 006a 0164 0183 017d 027c 026a  .|.j.j.d...}.|.j
-00001f50: 027d 037c 0164 0219 007d 047c 0164 0319  .}.|.d...}.|.d..
-00001f60: 0064 046b 0572 347c 016a 0164 0569 0083  .d.k.r4|.j.d.i..
-00001f70: 027d 056e 0c7c 016a 0164 0667 0083 027d  .}.n.|.j.d.g...}
-00001f80: 057c 016a 0164 0783 0164 006b 0972 7e79  .|.j.d...d.k.r~y
-00001f90: 1274 037c 037c 0164 0719 0083 0201 0057  .t.|.|.d.......W
-00001fa0: 006e 1c04 0074 046b 0a72 7c01 0001 0001  .n...t.k.r|.....
-00001fb0: 007c 036a 0583 0001 0059 006e 0258 0064  .|.j.....Y.n.X.d
-00001fc0: 087c 016b 0672 bc79 187c 036a 0664 0964  .|.k.r.y.|.j.d.d
-00001fd0: 087c 0164 0819 0069 0183 0201 0057 006e  .|.d...i.....W.n
-00001fe0: 1c04 0074 046b 0a72 ba01 0001 0001 007c  ...t.k.r.......|
-00001ff0: 036a 0583 0001 0059 006e 0258 0074 077c  .j.....Y.n.X.t.|
-00002000: 0483 016a 0883 006a 0964 0a83 017d 0664  ...j...j.d...}.d
-00002010: 007d 077c 0164 0b19 0090 0172 5079 4074  .}.|.d.....rPy@t
-00002020: 0a74 0b6a 0c83 0067 0183 016a 0d7c 0683  .t.j...g...j.|..
-00002030: 017d 087c 006a 0e7c 087c 0183 027d 087c  .}.|.j.|.|...}.|
-00002040: 036a 067c 087c 0583 027d 097c 096a 0f83  .j.|.|...}.|.j..
-00002050: 0064 0c19 0064 0c19 007d 0757 006e 3204  .d...d...}.W.n2.
-00002060: 0074 046b 0a90 0172 3a01 0001 0001 007c  .t.k...r:......|
-00002070: 036a 0583 0001 0059 006e 1604 0074 106b  .j.....Y.n...t.k
-00002080: 0a90 0172 4e01 0001 0001 0059 006e 0258  ...rN......Y.n.X
-00002090: 0090 017a f090 0179 6064 0d7c 016b 0690  ...z...y`d.|.k..
-000020a0: 0172 707c 006a 117c 067c 0183 027d 0a6e  .rp|.j.|.|...}.n
-000020b0: 3464 0e7c 016b 0690 0173 8464 0f7c 016b  4d.|.k...s.d.|.k
-000020c0: 0690 0172 947c 006a 127c 067c 017c 0383  ...r.|.j.|.|.|..
-000020d0: 037d 0a6e 1074 0a64 1067 0183 016a 0d7c  .}.n.t.d.g...j.|
-000020e0: 0683 017d 0a7c 006a 0e7c 0a7c 0183 027d  ...}.|.j.|.|...}
-000020f0: 0a64 0d7c 016b 0790 0172 da64 0f7c 016b  .d.|.k...r.d.|.k
-00002100: 0790 0172 da64 0e7c 016b 0790 0172 da7c  ...r.d.|.k...r.|
-00002110: 006a 137c 0a7c 0183 027d 0a64 0f7c 016b  .j.|.|...}.d.|.k
-00002120: 0790 0172 fa64 0e7c 016b 0790 0172 fa7c  ...r.d.|.k...r.|
-00002130: 006a 147c 0a7c 0183 027d 0a7c 036a 067c  .j.|.|...}.|.j.|
-00002140: 0a7c 0583 027d 0b64 1164 1284 007d 0c64  .|...}.d.d...}.d
-00002150: 1364 1484 0089 0087 0066 0164 1564 1684  .d.......f.d.d..
-00002160: 087d 0d7c 0b6a 1583 007d 0e64 0e7c 016b  .}.|.j...}.d.|.k
-00002170: 0690 0273 3e64 0f7c 016b 0690 0272 5074  ...s>d.|.k...rPt
-00002180: 1674 1764 1764 1884 007c 0e83 0283 017d  .t.d.d...|.....}
-00002190: 0e7c 0b6a 186a 197d 0f74 1674 177c 0d7c  .|.j.j.}.t.t.|.|
-000021a0: 0b83 0283 0174 1674 177c 0c7c 0e83 0283  .....t.t.|.|....
-000021b0: 0164 199c 027d 1074 1a7c 0283 0189 0188  .d...}.t.|......
-000021c0: 0190 0272 a287 0166 0164 1a64 1b84 087d  ...r...f.d.d...}
-000021d0: 1174 1b74 177c 117c 0f83 0283 017c 1064  .t.t.|.|.....|.d
-000021e0: 1c3c 007c 0764 006b 0990 0272 b47c 077c  .<.|.d.k...r.|.|
-000021f0: 1064 0b3c 007c 1053 0004 0074 046b 0a90  .d.<.|.S...t.k..
-00002200: 0272 ea01 007d 1201 007a 167c 036a 0583  .r...}...z.|.j..
-00002210: 0001 0074 1c7c 1283 0182 0157 0059 0064  ...t.|.....W.Y.d
-00002220: 0064 007d 127e 1258 006e 5604 0074 1d6b  .d.}.~.X.nV..t.k
-00002230: 0a90 0372 1401 007d 1201 007a 0e74 1c7c  ...r...}...z.t.|
-00002240: 1283 0182 0157 0059 0064 0064 007d 127e  .....W.Y.d.d.}.~
-00002250: 1258 006e 2c04 0074 106b 0a90 0372 3e01  .X.n,..t.k...r>.
-00002260: 007d 1201 007a 0e74 1c7c 1283 0182 0157  .}...z.t.|.....W
-00002270: 0059 0064 0064 007d 127e 1258 006e 0258  .Y.d.d.}.~.X.n.X
-00002280: 0057 0064 007c 036a 1e83 0001 0058 0064  .W.d.|.j.....X.d
-00002290: 0053 0029 1d4e 726f 0000 0072 3c00 0000  .S.).Nro...r<...
-000022a0: 7244 0000 0072 4500 0000 da0a 7061 7261  rD...rE.....para
-000022b0: 6d73 5f6f 626a da06 7061 7261 6d73 da08  ms_obj..params..
-000022c0: 7469 6d65 7a6f 6e65 da06 7363 6865 6d61  timezone..schema
-000022d0: 7a1a 5345 5420 7365 6172 6368 5f70 6174  z.SET search_pat
-000022e0: 6820 544f 203a 7363 6865 6d61 5a08 5f5f  h TO :schemaZ.__
-000022f0: 6a65 745f 7132 da05 636f 756e 7472 0100  jet_q2..countr..
-00002300: 0000 7250 0000 0072 5c00 0000 725a 0000  ..rP...r\...rZ..
-00002310: 00da 012a 6301 0000 0000 0000 0001 0000  ...*c...........
-00002320: 0002 0000 0053 0000 0073 1000 0000 7c00  .....S...s....|.
-00002330: 6401 6b02 720c 6400 5300 7c00 5300 2902  d.k.r.d.S.|.S.).
-00002340: 4e7a 083f 636f 6c75 6d6e 3f72 2300 0000  Nz.?column?r#...
-00002350: 2901 7241 0000 0072 2300 0000 7223 0000  ).rA...r#...r#..
-00002360: 0072 2400 0000 7289 0000 002c 0100 0073  .r$...r....,...s
-00002370: 0600 0000 0001 0801 0401 7a29 5371 6c53  ..........z)SqlS
-00002380: 6572 6961 6c69 7a65 722e 6578 6563 7574  erializer.execut
-00002390: 652e 3c6c 6f63 616c 733e 2e6d 6170 5f63  e.<locals>.map_c
-000023a0: 6f6c 756d 6e63 0100 0000 0000 0000 0100  olumnc..........
-000023b0: 0000 0b00 0000 5300 0000 7338 0000 0074  ......S...s8...t
-000023c0: 007c 0074 0183 0272 3079 0a7c 006a 0264  .|.t...r0y.|.j.d
-000023d0: 0183 0153 0004 0074 036b 0a72 2c01 0001  ...S...t.k.r,...
-000023e0: 0001 007c 006a 0483 0053 0058 006e 047c  ...|.j...S.X.n.|
-000023f0: 0053 0064 0053 0029 024e 7a05 7574 662d  .S.d.S.).Nz.utf-
-00002400: 3829 0572 7c00 0000 da05 6279 7465 73da  8).r|.....bytes.
-00002410: 0664 6563 6f64 65da 1255 6e69 636f 6465  .decode..Unicode
-00002420: 4465 636f 6465 4572 726f 72da 0368 6578  DecodeError..hex
-00002430: 2901 7241 0000 0072 2300 0000 7223 0000  ).rA...r#...r#..
-00002440: 0072 2400 0000 da0e 6d61 705f 726f 775f  .r$.....map_row_
-00002450: 636f 6c75 6d6e 3101 0000 730c 0000 0000  column1...s.....
-00002460: 010a 0102 010a 010e 010c 027a 2d53 716c  ...........z-Sql
-00002470: 5365 7269 616c 697a 6572 2e65 7865 6375  Serializer.execu
-00002480: 7465 2e3c 6c6f 6361 6c73 3e2e 6d61 705f  te.<locals>.map_
-00002490: 726f 775f 636f 6c75 6d6e 6301 0000 0000  row_columnc.....
-000024a0: 0000 0001 0000 0005 0000 0013 0000 0073  ...............s
-000024b0: 1c00 0000 7400 7401 8701 8700 6602 6401  ....t.t.....f.d.
-000024c0: 6402 8408 8800 6a02 8300 8302 8301 5300  d.....j.......S.
-000024d0: 2903 4e63 0100 0000 0000 0000 0100 0000  ).Nc............
-000024e0: 0300 0000 1300 0000 730c 0000 0088 0088  ........s.......
-000024f0: 017c 0019 0083 0153 0029 014e 7223 0000  .|.....S.).Nr#..
-00002500: 0029 0172 4100 0000 2902 72a4 0000 00da  .).rA...).r.....
-00002510: 0372 6f77 7223 0000 0072 2400 0000 7243  .rowr#...r$...rC
-00002520: 0000 003b 0100 0073 0000 0000 7a38 5371  ...;...s....z8Sq
-00002530: 6c53 6572 6961 6c69 7a65 722e 6578 6563  lSerializer.exec
-00002540: 7574 652e 3c6c 6f63 616c 733e 2e6d 6170  ute.<locals>.map
-00002550: 5f72 6f77 2e3c 6c6f 6361 6c73 3e2e 3c6c  _row.<locals>.<l
-00002560: 616d 6264 613e 2903 7267 0000 0072 4a00  ambda>).rg...rJ.
-00002570: 0000 da04 6b65 7973 2901 72a5 0000 0029  ....keys).r....)
-00002580: 0172 a400 0000 2901 72a5 0000 0072 2400  .r....).r....r$.
-00002590: 0000 da07 6d61 705f 726f 773a 0100 0073  ....map_row:...s
-000025a0: 0200 0000 0001 7a26 5371 6c53 6572 6961  ......z&SqlSeria
-000025b0: 6c69 7a65 722e 6578 6563 7574 652e 3c6c  lizer.execute.<l
-000025c0: 6f63 616c 733e 2e6d 6170 5f72 6f77 6301  ocals>.map_rowc.
-000025d0: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
-000025e0: 0000 0073 1000 0000 7c00 6401 6b02 720c  ...s....|.d.k.r.
-000025f0: 6402 5300 7c00 5300 2903 4eda 0767 726f  d.S.|.S.).N..gro
-00002600: 7570 5f31 725a 0000 0072 2300 0000 2901  up_1rZ...r#...).
-00002610: 7241 0000 0072 2300 0000 7223 0000 0072  rA...r#...r#...r
-00002620: 2400 0000 7243 0000 0040 0100 0073 0000  $...rC...@...s..
-00002630: 0000 7a27 5371 6c53 6572 6961 6c69 7a65  ..z'SqlSerialize
-00002640: 722e 6578 6563 7574 652e 3c6c 6f63 616c  r.execute.<local
-00002650: 733e 2e3c 6c61 6d62 6461 3e29 0272 5600  s>.<lambda>).rV.
-00002660: 0000 7270 0000 0063 0100 0000 0000 0000  ..rp...c........
-00002670: 0300 0000 0400 0000 1300 0000 7346 0000  ............sF..
-00002680: 0074 007c 0064 0183 0272 107c 006a 016e  .t.|.d...r.|.j.n
-00002690: 0264 027d 0174 007c 0064 0383 0272 2a88  .d.}.t.|.d...r*.
-000026a0: 006a 027c 006a 0383 016e 0264 007d 027c  .j.|.j...n.d.}.|
-000026b0: 0164 047c 0272 3e74 047c 0283 016e 0264  .d.|.r>t.|...n.d
-000026c0: 0069 0166 0253 0029 054e 7221 0000 00da  .i.f.S.).Nr!....
-000026d0: 00da 0974 7970 655f 636f 6465 7286 0000  ...type_coder...
-000026e0: 0029 05da 0768 6173 6174 7472 7221 0000  .)...hasattrr!..
-000026f0: 0072 5100 0000 72aa 0000 0072 1b00 0000  .rQ...r....r....
-00002700: 2903 7206 0000 0072 2100 0000 da08 7371  ).r....r!.....sq
-00002710: 6c5f 7479 7065 2901 da15 7479 7065 5f63  l_type)...type_c
-00002720: 6f64 655f 746f 5f73 716c 5f74 7970 6572  ode_to_sql_typer
-00002730: 2300 0000 7224 0000 00da 166d 6170 5f63  #...r$.....map_c
-00002740: 6f6c 756d 6e5f 6465 7363 7269 7074 696f  olumn_descriptio
-00002750: 6e4a 0100 0073 0800 0000 0001 1401 1a01  nJ...s..........
-00002760: 0201 7a35 5371 6c53 6572 6961 6c69 7a65  ..z5SqlSerialize
-00002770: 722e 6578 6563 7574 652e 3c6c 6f63 616c  r.execute.<local
-00002780: 733e 2e6d 6170 5f63 6f6c 756d 6e5f 6465  s>.map_column_de
-00002790: 7363 7269 7074 696f 6eda 1363 6f6c 756d  scription..colum
-000027a0: 6e5f 6465 7363 7269 7074 696f 6e73 291f  n_descriptions).
-000027b0: 728a 0000 0072 5100 0000 725e 0000 0072  r....rQ...r^...r
-000027c0: 0300 0000 720d 0000 00da 0872 6f6c 6c62  ....r......rollb
-000027d0: 6163 6bda 0765 7865 6375 7465 7204 0000  ack..executer...
-000027e0: 0072 7000 0000 7255 0000 0072 0500 0000  .rp...rU...r....
-000027f0: 7207 0000 0072 9e00 0000 7254 0000 0072  r....r....rT...r
-00002800: 9000 0000 da03 616c 6cda 0945 7863 6570  ......all..Excep
-00002810: 7469 6f6e 7259 0000 0072 6e00 0000 7294  tionrY...rn...r.
-00002820: 0000 0072 9900 0000 72a6 0000 0072 6700  ...r....r....rg.
-00002830: 0000 724a 0000 00da 0663 7572 736f 72da  ..rJ.....cursor.
-00002840: 0b64 6573 6372 6970 7469 6f6e 7210 0000  .descriptionr...
-00002850: 00da 0464 6963 7472 1100 0000 da09 5479  ...dictr......Ty
-00002860: 7065 4572 726f 72da 0563 6c6f 7365 2913  peError..close).
-00002870: 724c 0000 0072 5600 0000 726f 0000 0072  rL...rV...ro...r
-00002880: 5e00 0000 723c 0000 0072 9b00 0000 7255  ^...r<...r....rU
-00002890: 0000 005a 0a63 6f75 6e74 5f72 6f77 735a  ...Z.count_rowsZ
-000028a0: 0e63 6f75 6e74 5f71 7565 7279 7365 745a  .count_querysetZ
-000028b0: 0c63 6f75 6e74 5f72 6573 756c 7472 6d00  .count_resultrm.
-000028c0: 0000 da06 7265 7375 6c74 7289 0000 0072  ....resultr....r
-000028d0: a700 0000 da0c 636f 6c75 6d6e 5f6e 616d  ......column_nam
-000028e0: 6573 da12 6375 7273 6f72 5f64 6573 6372  es..cursor_descr
-000028f0: 6970 7469 6f6e da08 7265 7370 6f6e 7365  iption..response
-00002900: 72ae 0000 00da 0165 7223 0000 0029 0272  r......er#...).r
-00002910: a400 0000 72ad 0000 0072 2400 0000 72b1  ....r....r$...r.
-00002920: 0000 00f2 0000 0073 8400 0000 0001 0c01  .......s........
-00002930: 0602 0802 0c01 0e02 0c02 0e01 0201 1201  ................
-00002940: 0e01 0801 0602 0801 0201 1801 0e01 0801  ................
-00002950: 0602 1201 0402 0a01 0201 1401 0c02 0c01  ................
-00002960: 1401 1001 0c01 1001 0602 0801 0a01 0e01  ................
-00002970: 1401 1002 1002 0c02 1e01 0c02 1401 0c02  ................
-00002980: 0c02 0805 0809 0c03 0802 1401 1202 0802  ................
-00002990: 0c01 1203 0801 0601 0c07 1202 0a01 0802  ................
-000029a0: 0401 1201 0801 1801 1201 1801 1201 1e02  ................
-000029b0: 7a15 5371 6c53 6572 6961 6c69 7a65 722e  z.SqlSerializer.
-000029c0: 6578 6563 7574 654e 2925 721d 0000 0072  executeN)%r....r
-000029d0: 1e00 0000 721f 0000 0072 0e00 0000 7220  ....r....r....r 
-000029e0: 0000 0072 3c00 0000 da0c 496e 7465 6765  ...r<.....Intege
-000029f0: 7246 6965 6c64 7291 0000 0072 9200 0000  rFieldr....r....
-00002a00: 726a 0000 00da 0c42 6f6f 6c65 616e 4669  rj.....BooleanFi
-00002a10: 656c 6472 9e00 0000 721c 0000 0072 7000  eldr....r....rp.
-00002a20: 0000 7225 0000 0072 7500 0000 722a 0000  ..r%...ru...r*..
-00002a30: 0072 5000 0000 722b 0000 0072 5a00 0000  .rP...r+...rZ...
-00002a40: 7231 0000 0072 5c00 0000 729c 0000 0072  r1...r\...r....r
-00002a50: 9d00 0000 7213 0000 0072 9b00 0000 da09  ....r....r......
-00002a60: 4a53 4f4e 4669 656c 6472 9a00 0000 7244  JSONFieldr....rD
-00002a70: 0000 0072 4f00 0000 7259 0000 0072 6e00  ...rO...rY...rn.
-00002a80: 0000 7290 0000 0072 9400 0000 7298 0000  ..r....r....r...
-00002a90: 0072 9900 0000 72b1 0000 0072 2300 0000  .r....r....r#...
-00002aa0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-00002ab0: 3400 0000 3500 0000 732e 0000 0008 0108  4...5...s.......
-00002ac0: 010c 010c 010e 010c 010c 010c 010a 010a  ................
-00002ad0: 010a 010c 010c 010a 010c 010c 0208 0f08  ................
-00002ae0: 0c08 3008 4408 0c08 0a08 0772 3400 0000  ..0.D......r4...
-00002af0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-00002b00: 0040 0000 0073 1e00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00002b10: 5a02 6503 6401 6402 8d01 5a04 6403 6404  Z.e.d.d...Z.d.d.
-00002b20: 8400 5a05 6405 5300 2906 da0e 5371 6c73  ..Z.d.S.)...Sqls
-00002b30: 5365 7269 616c 697a 6572 5429 0172 3200  SerializerT).r2.
-00002b40: 0000 6302 0000 0000 0000 0003 0000 0005  ..c.............
-00002b50: 0000 0003 0000 0073 2a00 0000 7400 7c00  .......s*...t.|.
-00002b60: 6a01 6401 8d01 8900 8700 6601 6402 6403  j.d.......f.d.d.
-00002b70: 8408 7d02 7402 7403 7c02 7c01 6404 1900  ..}.t.t.|.|.d...
-00002b80: 8302 8301 5300 2905 4e29 0172 8a00 0000  ....S.).N).r....
-00002b90: 6301 0000 0000 0000 0002 0000 0010 0000  c...............
-00002ba0: 0013 0000 0073 3a00 0000 790a 8800 6a00  .....s:...y...j.
-00002bb0: 7c00 8301 5300 0400 7401 6b0a 7234 0100  |...S...t.k.r4..
-00002bc0: 7d01 0100 7a0e 6401 7402 7c01 6a03 8301  }...z.d.t.|.j...
-00002bd0: 6901 5300 6400 7d01 7e01 5800 6e02 5800  i.S.d.}.~.X.n.X.
-00002be0: 6400 5300 2902 4eda 0565 7272 6f72 2904  d.S.).N..error).
-00002bf0: 72b1 0000 0072 1100 0000 da03 7374 72da  r....r......str.
-00002c00: 0664 6574 6169 6c29 0272 3c00 0000 72bd  .detail).r<...r.
-00002c10: 0000 0029 01da 0a73 6572 6961 6c69 7a65  ...)...serialize
-00002c20: 7272 2300 0000 7224 0000 00da 096d 6170  rr#...r$.....map
-00002c30: 5f71 7565 7279 6801 0000 7308 0000 0000  _queryh...s.....
-00002c40: 0102 010a 0110 017a 2953 716c 7353 6572  .......z)SqlsSer
-00002c50: 6961 6c69 7a65 722e 6578 6563 7574 652e  ializer.execute.
-00002c60: 3c6c 6f63 616c 733e 2e6d 6170 5f71 7565  <locals>.map_que
-00002c70: 7279 da07 7175 6572 6965 7329 0472 3400  ry..queries).r4.
-00002c80: 0000 728a 0000 0072 6700 0000 724a 0000  ..r....rg...rJ..
-00002c90: 0029 0372 4c00 0000 7256 0000 0072 c600  .).rL...rV...r..
-00002ca0: 0000 7223 0000 0029 0172 c500 0000 7224  ..r#...).r....r$
-00002cb0: 0000 0072 b100 0000 6501 0000 7306 0000  ...r....e...s...
-00002cc0: 0000 010c 020c 067a 1653 716c 7353 6572  .......z.SqlsSer
-00002cd0: 6961 6c69 7a65 722e 6578 6563 7574 654e  ializer.executeN
-00002ce0: 2906 721d 0000 0072 1e00 0000 721f 0000  ).r....r....r...
-00002cf0: 0072 3400 0000 72c7 0000 0072 b100 0000  .r4...r....r....
-00002d00: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
-00002d10: 2400 0000 72c1 0000 0062 0100 0073 0400  $...r....b...s..
-00002d20: 0000 0801 0a02 72c1 0000 004e 2931 da1e  ......r....N)1..
-00002d30: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00002d40: 7574 696c 732e 7175 6572 7973 6574 7202  utils.querysetr.
-00002d50: 0000 0072 0300 0000 da0a 7371 6c61 6c63  ...r......sqlalc
-00002d60: 6865 6d79 7204 0000 0072 0500 0000 7206  hemyr....r....r.
-00002d70: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00002d80: 0000 720a 0000 0072 0b00 0000 5a0e 7371  ..r....r....Z.sq
-00002d90: 6c61 6c63 6865 6d79 2e73 716c 720c 0000  lalchemy.sqlr...
-00002da0: 00da 0e73 716c 616c 6368 656d 792e 6578  ...sqlalchemy.ex
-00002db0: 6372 0d00 0000 da0f 6a65 745f 6272 6964  cr......jet_brid
-00002dc0: 6765 5f62 6173 6572 0e00 0000 da12 6a65  ge_baser......je
-00002dd0: 745f 6272 6964 6765 5f62 6173 652e 6462  t_bridge_base.db
-00002de0: 720f 0000 0072 1000 0000 5a1e 6a65 745f  r....r....Z.jet_
-00002df0: 6272 6964 6765 5f62 6173 652e 6578 6365  bridge_base.exce
-00002e00: 7074 696f 6e73 2e73 716c 7211 0000 00da  ptions.sqlr.....
-00002e10: 2b6a 6574 5f62 7269 6467 655f 6261 7365  +jet_bridge_base
-00002e20: 2e65 7863 6570 7469 6f6e 732e 7661 6c69  .exceptions.vali
-00002e30: 6461 7469 6f6e 5f65 7272 6f72 7212 0000  dation_errorr...
-00002e40: 005a 216a 6574 5f62 7269 6467 655f 6261  .Z!jet_bridge_ba
-00002e50: 7365 2e66 6965 6c64 732e 7371 6c5f 7061  se.fields.sql_pa
-00002e60: 7261 6d73 7213 0000 00da 176a 6574 5f62  ramsr......jet_b
-00002e70: 7269 6467 655f 6261 7365 2e66 696c 7465  ridge_base.filte
-00002e80: 7273 7214 0000 00da 1e6a 6574 5f62 7269  rsr......jet_bri
-00002e90: 6467 655f 6261 7365 2e66 696c 7465 7273  dge_base.filters
-00002ea0: 2e66 696c 7465 7272 1500 0000 da23 6a65  .filterr.....#je
-00002eb0: 745f 6272 6964 6765 5f62 6173 652e 6669  t_bridge_base.fi
-00002ec0: 6c74 6572 732e 6d6f 6465 6c5f 6772 6f75  lters.model_grou
-00002ed0: 7072 1600 0000 7217 0000 00da 2a6a 6574  pr....r.....*jet
-00002ee0: 5f62 7269 6467 655f 6261 7365 2e66 696c  _bridge_base.fil
-00002ef0: 7465 7273 2e66 696c 7465 725f 666f 725f  ters.filter_for_
-00002f00: 6462 6669 656c 6472 1800 0000 da26 6a65  dbfieldr.....&je
-00002f10: 745f 6272 6964 6765 5f62 6173 652e 7365  t_bridge_base.se
-00002f20: 7269 616c 697a 6572 732e 7365 7269 616c  rializers.serial
-00002f30: 697a 6572 7219 0000 005a 1e6a 6574 5f62  izerr....Z.jet_b
-00002f40: 7269 6467 655f 6261 7365 2e75 7469 6c73  ridge_base.utils
-00002f50: 2e64 625f 7479 7065 7372 1a00 0000 721b  .db_typesr....r.
-00002f60: 0000 0072 1c00 0000 7225 0000 0072 2a00  ...r....r%...r*.
-00002f70: 0000 722b 0000 0072 3000 0000 7231 0000  ..r+...r0...r1..
-00002f80: 0072 3400 0000 72c1 0000 0072 2300 0000  .r4...r....r#...
-00002f90: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00002fa0: 083c 6d6f 6475 6c65 3e01 0000 0073 3200  .<module>....s2.
-00002fb0: 0000 1001 2401 0c01 0c01 0c02 0c01 1001  ....$...........
-00002fc0: 0c01 0c01 0c01 0c01 0c01 1001 0c01 0c01  ................
-00002fd0: 1003 1005 1005 1005 1007 1005 1006 107f  ................
-00002fe0: 007f 002f                                .../
+00001e10: 0119 0083 0283 017d 047c 016a 027c 048e  .......}.|.j.|..
+00001e20: 007d 016e 5264 047c 026b 0772 8064 057c  .}.nRd.|.k.r.d.|
+00001e30: 026b 0772 8064 067c 026b 0772 8074 037c  .k.r.d.|.k.r.t.|
+00001e40: 0383 0164 076b 0272 8078 2c7c 026a 0464  ...d.k.r.x,|.j.d
+00001e50: 0867 0083 0244 005d 1c7d 0574 057c 0564  .g...D.].}.t.|.d
+00001e60: 0919 0083 017d 067c 016a 027c 0683 017d  .....}.|.j.|...}
+00001e70: 0150 0071 6057 007c 0153 0029 0a4e 726a  .P.q`W.|.S.).Nrj
+00001e80: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
+00001e90: 0200 0000 1300 0000 730a 0000 0088 006a  ........s......j
+00001ea0: 007c 0083 0153 0029 014e 2901 7298 0000  .|...S.).N).r...
+00001eb0: 0029 0172 4100 0000 2901 724c 0000 0072  .).rA...).rL...r
+00001ec0: 2300 0000 7224 0000 0072 4300 0000 ed00  #...r$...rC.....
+00001ed0: 0000 7300 0000 007a 2d53 716c 5365 7269  ..s....z-SqlSeri
+00001ee0: 616c 697a 6572 2e73 6f72 745f 7175 6572  alizer.sort_quer
+00001ef0: 7973 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c  yset.<locals>.<l
+00001f00: 616d 6264 613e 7250 0000 0072 5a00 0000  ambda>rP...rZ...
+00001f10: 725c 0000 0072 5d00 0000 7270 0000 0072  r\...r]...rp...r
+00001f20: 2100 0000 2906 7267 0000 0072 4a00 0000  !...).rg...rJ...
+00001f30: 726a 0000 0072 0200 0000 7251 0000 0072  rj...r....rQ...r
+00001f40: 0600 0000 2907 724c 0000 0072 6d00 0000  ....).rL...rm...
+00001f50: 7256 0000 0072 5e00 0000 726a 0000 0072  rV...r^...rj...r
+00001f60: 8500 0000 7286 0000 0072 2300 0000 2901  ....r....r#...).
+00001f70: 724c 0000 0072 2400 0000 da0d 736f 7274  rL...r$.....sort
+00001f80: 5f71 7565 7279 7365 74eb 0000 0073 1400  _queryset....s..
+00001f90: 0000 0001 0801 1a01 0c02 1801 0c01 1201  ................
+00001fa0: 0c01 0a01 0602 7a1b 5371 6c53 6572 6961  ......z.SqlSeria
+00001fb0: 6c69 7a65 722e 736f 7274 5f71 7565 7279  lizer.sort_query
+00001fc0: 7365 7463 0200 0000 0000 0000 1300 0000  setc............
+00001fd0: 2e00 0000 0300 0000 7354 0300 007c 006a  ........sT...|.j
+00001fe0: 006a 0164 0183 017d 027c 026a 027d 037c  .j.d...}.|.j.}.|
+00001ff0: 0164 0219 007d 047c 0164 0319 0064 046b  .d...}.|.d...d.k
+00002000: 0572 347c 016a 0164 0569 0083 027d 056e  .r4|.j.d.i...}.n
+00002010: 0c7c 016a 0164 0667 0083 027d 057c 016a  .|.j.d.g...}.|.j
+00002020: 0164 0783 0164 006b 0972 7e79 1274 037c  .d...d.k.r~y.t.|
+00002030: 037c 0164 0719 0083 0201 0057 006e 1c04  .|.d.......W.n..
+00002040: 0074 046b 0a72 7c01 0001 0001 007c 036a  .t.k.r|......|.j
+00002050: 0583 0001 0059 006e 0258 0064 087c 016b  .....Y.n.X.d.|.k
+00002060: 0672 bc79 187c 036a 0664 0964 087c 0164  .r.y.|.j.d.d.|.d
+00002070: 0819 0069 0183 0201 0057 006e 1c04 0074  ...i.....W.n...t
+00002080: 046b 0a72 ba01 0001 0001 007c 036a 0583  .k.r.......|.j..
+00002090: 0001 0059 006e 0258 0074 077c 0483 016a  ...Y.n.X.t.|...j
+000020a0: 0883 006a 0964 0a83 017d 0664 007d 077c  ...j.d...}.d.}.|
+000020b0: 0164 0b19 0090 0172 5079 4074 0a74 0b6a  .d.....rPy@t.t.j
+000020c0: 0c83 0067 0183 016a 0d7c 0683 017d 087c  ...g...j.|...}.|
+000020d0: 006a 0e7c 087c 0183 027d 087c 036a 067c  .j.|.|...}.|.j.|
+000020e0: 087c 0583 027d 097c 096a 0f83 0064 0c19  .|...}.|.j...d..
+000020f0: 0064 0c19 007d 0757 006e 3204 0074 046b  .d...}.W.n2..t.k
+00002100: 0a90 0172 3a01 0001 0001 007c 036a 0583  ...r:......|.j..
+00002110: 0001 0059 006e 1604 0074 106b 0a90 0172  ...Y.n...t.k...r
+00002120: 4e01 0001 0001 0059 006e 0258 0090 017a  N......Y.n.X...z
+00002130: f290 0179 6264 0d7c 016b 0690 0172 707c  ...ybd.|.k...rp|
+00002140: 006a 117c 067c 0183 027d 0a6e 3464 0e7c  .j.|.|...}.n4d.|
+00002150: 016b 0690 0173 8464 0f7c 016b 0690 0172  .k...s.d.|.k...r
+00002160: 947c 006a 127c 067c 017c 0383 037d 0a6e  .|.j.|.|.|...}.n
+00002170: 1074 0a64 1067 0183 016a 0d7c 0683 017d  .t.d.g...j.|...}
+00002180: 0a7c 006a 0e7c 0a7c 0183 027d 0a64 0d7c  .|.j.|.|...}.d.|
+00002190: 016b 0790 0172 da64 0f7c 016b 0790 0172  .k...r.d.|.k...r
+000021a0: da64 0e7c 016b 0790 0172 da7c 006a 137c  .d.|.k...r.|.j.|
+000021b0: 0a7c 0183 027d 0a64 0f7c 016b 0790 0172  .|...}.d.|.k...r
+000021c0: fc64 0e7c 016b 0790 0172 fc7c 006a 147c  .d.|.k...r.|.j.|
+000021d0: 0a7c 017c 0383 037d 0a7c 036a 067c 0a7c  .|.|...}.|.j.|.|
+000021e0: 0583 027d 0b64 1164 1284 007d 0c64 1364  ...}.d.d...}.d.d
+000021f0: 1484 0089 0087 0066 0164 1564 1684 087d  .......f.d.d...}
+00002200: 0d7c 0b6a 1583 007d 0e64 0e7c 016b 0690  .|.j...}.d.|.k..
+00002210: 0273 4064 0f7c 016b 0690 0272 5274 1674  .s@d.|.k...rRt.t
+00002220: 1764 1764 1884 007c 0e83 0283 017d 0e7c  .d.d...|.....}.|
+00002230: 0b6a 186a 197d 0f74 1674 177c 0d7c 0b83  .j.j.}.t.t.|.|..
+00002240: 0283 0174 1674 177c 0c7c 0e83 0283 0164  ...t.t.|.|.....d
+00002250: 199c 027d 1074 1a7c 0283 0189 0188 0190  ...}.t.|........
+00002260: 0272 a487 0166 0164 1a64 1b84 087d 1174  .r...f.d.d...}.t
+00002270: 1b74 177c 117c 0f83 0283 017c 1064 1c3c  .t.|.|.....|.d.<
+00002280: 007c 0764 006b 0990 0272 b67c 077c 1064  .|.d.k...r.|.|.d
+00002290: 0b3c 007c 1053 0004 0074 046b 0a90 0272  .<.|.S...t.k...r
+000022a0: ec01 007d 1201 007a 167c 036a 0583 0001  ...}...z.|.j....
+000022b0: 0074 1c7c 1283 0182 0157 0059 0064 0064  .t.|.....W.Y.d.d
+000022c0: 007d 127e 1258 006e 5604 0074 1d6b 0a90  .}.~.X.nV..t.k..
+000022d0: 0372 1601 007d 1201 007a 0e74 1c7c 1283  .r...}...z.t.|..
+000022e0: 0182 0157 0059 0064 0064 007d 127e 1258  ...W.Y.d.d.}.~.X
+000022f0: 006e 2c04 0074 106b 0a90 0372 4001 007d  .n,..t.k...r@..}
+00002300: 1201 007a 0e74 1c7c 1283 0182 0157 0059  ...z.t.|.....W.Y
+00002310: 0064 0064 007d 127e 1258 006e 0258 0057  .d.d.}.~.X.n.X.W
+00002320: 0064 007c 036a 1e83 0001 0058 0064 0053  .d.|.j.....X.d.S
+00002330: 0029 1d4e 726f 0000 0072 3c00 0000 7244  .).Nro...r<...rD
+00002340: 0000 0072 4500 0000 da0a 7061 7261 6d73  ...rE.....params
+00002350: 5f6f 626a da06 7061 7261 6d73 da08 7469  _obj..params..ti
+00002360: 6d65 7a6f 6e65 da06 7363 6865 6d61 7a1a  mezone..schemaz.
+00002370: 5345 5420 7365 6172 6368 5f70 6174 6820  SET search_path 
+00002380: 544f 203a 7363 6865 6d61 5a08 5f5f 6a65  TO :schemaZ.__je
+00002390: 745f 7132 da05 636f 756e 7472 0100 0000  t_q2..countr....
+000023a0: 7250 0000 0072 5c00 0000 725a 0000 00da  rP...r\...rZ....
+000023b0: 012a 6301 0000 0000 0000 0001 0000 0002  .*c.............
+000023c0: 0000 0053 0000 0073 1000 0000 7c00 6401  ...S...s....|.d.
+000023d0: 6b02 720c 6400 5300 7c00 5300 2902 4e7a  k.r.d.S.|.S.).Nz
+000023e0: 083f 636f 6c75 6d6e 3f72 2300 0000 2901  .?column?r#...).
+000023f0: 7241 0000 0072 2300 0000 7223 0000 0072  rA...r#...r#...r
+00002400: 2400 0000 7289 0000 0033 0100 0073 0600  $...r....3...s..
+00002410: 0000 0001 0801 0401 7a29 5371 6c53 6572  ........z)SqlSer
+00002420: 6961 6c69 7a65 722e 6578 6563 7574 652e  ializer.execute.
+00002430: 3c6c 6f63 616c 733e 2e6d 6170 5f63 6f6c  <locals>.map_col
+00002440: 756d 6e63 0100 0000 0000 0000 0100 0000  umnc............
+00002450: 0b00 0000 5300 0000 7338 0000 0074 007c  ....S...s8...t.|
+00002460: 0074 0183 0272 3079 0a7c 006a 0264 0183  .t...r0y.|.j.d..
+00002470: 0153 0004 0074 036b 0a72 2c01 0001 0001  .S...t.k.r,.....
+00002480: 007c 006a 0483 0053 0058 006e 047c 0053  .|.j...S.X.n.|.S
+00002490: 0064 0053 0029 024e 7a05 7574 662d 3829  .d.S.).Nz.utf-8)
+000024a0: 0572 7c00 0000 da05 6279 7465 73da 0664  .r|.....bytes..d
+000024b0: 6563 6f64 65da 1255 6e69 636f 6465 4465  ecode..UnicodeDe
+000024c0: 636f 6465 4572 726f 72da 0368 6578 2901  codeError..hex).
+000024d0: 7241 0000 0072 2300 0000 7223 0000 0072  rA...r#...r#...r
+000024e0: 2400 0000 da0e 6d61 705f 726f 775f 636f  $.....map_row_co
+000024f0: 6c75 6d6e 3801 0000 730c 0000 0000 010a  lumn8...s.......
+00002500: 0102 010a 010e 010c 027a 2d53 716c 5365  .........z-SqlSe
+00002510: 7269 616c 697a 6572 2e65 7865 6375 7465  rializer.execute
+00002520: 2e3c 6c6f 6361 6c73 3e2e 6d61 705f 726f  .<locals>.map_ro
+00002530: 775f 636f 6c75 6d6e 6301 0000 0000 0000  w_columnc.......
+00002540: 0001 0000 0005 0000 0013 0000 0073 1c00  .............s..
+00002550: 0000 7400 7401 8701 8700 6602 6401 6402  ..t.t.....f.d.d.
+00002560: 8408 8800 6a02 8300 8302 8301 5300 2903  ....j.......S.).
+00002570: 4e63 0100 0000 0000 0000 0100 0000 0300  Nc..............
+00002580: 0000 1300 0000 730c 0000 0088 0088 017c  ......s........|
+00002590: 0019 0083 0153 0029 014e 7223 0000 0029  .....S.).Nr#...)
+000025a0: 0172 4100 0000 2902 72a4 0000 00da 0372  .rA...).r......r
+000025b0: 6f77 7223 0000 0072 2400 0000 7243 0000  owr#...r$...rC..
+000025c0: 0042 0100 0073 0000 0000 7a38 5371 6c53  .B...s....z8SqlS
+000025d0: 6572 6961 6c69 7a65 722e 6578 6563 7574  erializer.execut
+000025e0: 652e 3c6c 6f63 616c 733e 2e6d 6170 5f72  e.<locals>.map_r
+000025f0: 6f77 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ow.<locals>.<lam
+00002600: 6264 613e 2903 7267 0000 0072 4a00 0000  bda>).rg...rJ...
+00002610: da04 6b65 7973 2901 72a5 0000 0029 0172  ..keys).r....).r
+00002620: a400 0000 2901 72a5 0000 0072 2400 0000  ....).r....r$...
+00002630: da07 6d61 705f 726f 7741 0100 0073 0200  ..map_rowA...s..
+00002640: 0000 0001 7a26 5371 6c53 6572 6961 6c69  ....z&SqlSeriali
+00002650: 7a65 722e 6578 6563 7574 652e 3c6c 6f63  zer.execute.<loc
+00002660: 616c 733e 2e6d 6170 5f72 6f77 6301 0000  als>.map_rowc...
+00002670: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00002680: 0073 1000 0000 7c00 6401 6b02 720c 6402  .s....|.d.k.r.d.
+00002690: 5300 7c00 5300 2903 4eda 0767 726f 7570  S.|.S.).N..group
+000026a0: 5f31 725a 0000 0072 2300 0000 2901 7241  _1rZ...r#...).rA
+000026b0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+000026c0: 0000 7243 0000 0047 0100 0073 0000 0000  ..rC...G...s....
+000026d0: 7a27 5371 6c53 6572 6961 6c69 7a65 722e  z'SqlSerializer.
+000026e0: 6578 6563 7574 652e 3c6c 6f63 616c 733e  execute.<locals>
+000026f0: 2e3c 6c61 6d62 6461 3e29 0272 5600 0000  .<lambda>).rV...
+00002700: 7270 0000 0063 0100 0000 0000 0000 0300  rp...c..........
+00002710: 0000 0400 0000 1300 0000 7346 0000 0074  ..........sF...t
+00002720: 007c 0064 0183 0272 107c 006a 016e 0264  .|.d...r.|.j.n.d
+00002730: 027d 0174 007c 0064 0383 0272 2a88 006a  .}.t.|.d...r*..j
+00002740: 027c 006a 0383 016e 0264 007d 027c 0164  .|.j...n.d.}.|.d
+00002750: 047c 0272 3e74 047c 0283 016e 0264 0069  .|.r>t.|...n.d.i
+00002760: 0166 0253 0029 054e 7221 0000 00da 00da  .f.S.).Nr!......
+00002770: 0974 7970 655f 636f 6465 7286 0000 0029  .type_coder....)
+00002780: 05da 0768 6173 6174 7472 7221 0000 0072  ...hasattrr!...r
+00002790: 5100 0000 72aa 0000 0072 1b00 0000 2903  Q...r....r....).
+000027a0: 7206 0000 0072 2100 0000 da08 7371 6c5f  r....r!.....sql_
+000027b0: 7479 7065 2901 da15 7479 7065 5f63 6f64  type)...type_cod
+000027c0: 655f 746f 5f73 716c 5f74 7970 6572 2300  e_to_sql_typer#.
+000027d0: 0000 7224 0000 00da 166d 6170 5f63 6f6c  ..r$.....map_col
+000027e0: 756d 6e5f 6465 7363 7269 7074 696f 6e51  umn_descriptionQ
+000027f0: 0100 0073 0800 0000 0001 1401 1a01 0201  ...s............
+00002800: 7a35 5371 6c53 6572 6961 6c69 7a65 722e  z5SqlSerializer.
+00002810: 6578 6563 7574 652e 3c6c 6f63 616c 733e  execute.<locals>
+00002820: 2e6d 6170 5f63 6f6c 756d 6e5f 6465 7363  .map_column_desc
+00002830: 7269 7074 696f 6eda 1363 6f6c 756d 6e5f  ription..column_
+00002840: 6465 7363 7269 7074 696f 6e73 291f 728a  descriptions).r.
+00002850: 0000 0072 5100 0000 725e 0000 0072 0300  ...rQ...r^...r..
+00002860: 0000 720d 0000 00da 0872 6f6c 6c62 6163  ..r......rollbac
+00002870: 6bda 0765 7865 6375 7465 7204 0000 0072  k..executer....r
+00002880: 7000 0000 7255 0000 0072 0500 0000 7207  p...rU...r....r.
+00002890: 0000 0072 9e00 0000 7254 0000 0072 9000  ...r....rT...r..
+000028a0: 0000 da03 616c 6cda 0945 7863 6570 7469  ....all..Excepti
+000028b0: 6f6e 7259 0000 0072 6e00 0000 7294 0000  onrY...rn...r...
+000028c0: 0072 9900 0000 72a6 0000 0072 6700 0000  .r....r....rg...
+000028d0: 724a 0000 00da 0663 7572 736f 72da 0b64  rJ.....cursor..d
+000028e0: 6573 6372 6970 7469 6f6e 7210 0000 00da  escriptionr.....
+000028f0: 0464 6963 7472 1100 0000 da09 5479 7065  .dictr......Type
+00002900: 4572 726f 72da 0563 6c6f 7365 2913 724c  Error..close).rL
+00002910: 0000 0072 5600 0000 726f 0000 0072 5e00  ...rV...ro...r^.
+00002920: 0000 723c 0000 0072 9b00 0000 7255 0000  ..r<...r....rU..
+00002930: 005a 0a63 6f75 6e74 5f72 6f77 735a 0e63  .Z.count_rowsZ.c
+00002940: 6f75 6e74 5f71 7565 7279 7365 745a 0c63  ount_querysetZ.c
+00002950: 6f75 6e74 5f72 6573 756c 7472 6d00 0000  ount_resultrm...
+00002960: da06 7265 7375 6c74 7289 0000 0072 a700  ..resultr....r..
+00002970: 0000 da0c 636f 6c75 6d6e 5f6e 616d 6573  ....column_names
+00002980: da12 6375 7273 6f72 5f64 6573 6372 6970  ..cursor_descrip
+00002990: 7469 6f6e da08 7265 7370 6f6e 7365 72ae  tion..responser.
+000029a0: 0000 00da 0165 7223 0000 0029 0272 a400  .....er#...).r..
+000029b0: 0000 72ad 0000 0072 2400 0000 72b1 0000  ..r....r$...r...
+000029c0: 00f9 0000 0073 8400 0000 0001 0c01 0602  .....s..........
+000029d0: 0802 0c01 0e02 0c02 0e01 0201 1201 0e01  ................
+000029e0: 0801 0602 0801 0201 1801 0e01 0801 0602  ................
+000029f0: 1201 0402 0a01 0201 1401 0c02 0c01 1401  ................
+00002a00: 1001 0c01 1001 0602 0801 0a01 0e01 1401  ................
+00002a10: 1002 1002 0c02 1e01 0c02 1401 0e02 0c02  ................
+00002a20: 0805 0809 0c03 0802 1401 1202 0802 0c01  ................
+00002a30: 1203 0801 0601 0c07 1202 0a01 0802 0401  ................
+00002a40: 1201 0801 1801 1201 1801 1201 1e02 7a15  ..............z.
+00002a50: 5371 6c53 6572 6961 6c69 7a65 722e 6578  SqlSerializer.ex
+00002a60: 6563 7574 654e 2925 721d 0000 0072 1e00  ecuteN)%r....r..
+00002a70: 0000 721f 0000 0072 0e00 0000 7220 0000  ..r....r....r ..
+00002a80: 0072 3c00 0000 da0c 496e 7465 6765 7246  .r<.....IntegerF
+00002a90: 6965 6c64 7291 0000 0072 9200 0000 726a  ieldr....r....rj
+00002aa0: 0000 00da 0c42 6f6f 6c65 616e 4669 656c  .....BooleanFiel
+00002ab0: 6472 9e00 0000 721c 0000 0072 7000 0000  dr....r....rp...
+00002ac0: 7225 0000 0072 7500 0000 722a 0000 0072  r%...ru...r*...r
+00002ad0: 5000 0000 722b 0000 0072 5a00 0000 7231  P...r+...rZ...r1
+00002ae0: 0000 0072 5c00 0000 729c 0000 0072 9d00  ...r\...r....r..
+00002af0: 0000 7213 0000 0072 9b00 0000 da09 4a53  ..r....r......JS
+00002b00: 4f4e 4669 656c 6472 9a00 0000 7244 0000  ONFieldr....rD..
+00002b10: 0072 4f00 0000 7259 0000 0072 6e00 0000  .rO...rY...rn...
+00002b20: 7290 0000 0072 9400 0000 7298 0000 0072  r....r....r....r
+00002b30: 9900 0000 72b1 0000 0072 2300 0000 7223  ....r....r#...r#
+00002b40: 0000 0072 2300 0000 7224 0000 0072 3400  ...r#...r$...r4.
+00002b50: 0000 3500 0000 732e 0000 0008 0108 010c  ..5...s.........
+00002b60: 010c 010e 010c 010c 010c 010a 010a 010a  ................
+00002b70: 010c 010c 010a 010c 010c 0208 0f08 0c08  ................
+00002b80: 3008 4408 0c08 0a08 0e72 3400 0000 6300  0.D......r4...c.
+00002b90: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00002ba0: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00002bb0: 6503 6401 6402 8d01 5a04 6403 6404 8400  e.d.d...Z.d.d...
+00002bc0: 5a05 6405 5300 2906 da0e 5371 6c73 5365  Z.d.S.)...SqlsSe
+00002bd0: 7269 616c 697a 6572 5429 0172 3200 0000  rializerT).r2...
+00002be0: 6302 0000 0000 0000 0003 0000 0005 0000  c...............
+00002bf0: 0003 0000 0073 2a00 0000 7400 7c00 6a01  .....s*...t.|.j.
+00002c00: 6401 8d01 8900 8700 6601 6402 6403 8408  d.......f.d.d...
+00002c10: 7d02 7402 7403 7c02 7c01 6404 1900 8302  }.t.t.|.|.d.....
+00002c20: 8301 5300 2905 4e29 0172 8a00 0000 6301  ..S.).N).r....c.
+00002c30: 0000 0000 0000 0002 0000 0010 0000 0013  ................
+00002c40: 0000 0073 3a00 0000 790a 8800 6a00 7c00  ...s:...y...j.|.
+00002c50: 8301 5300 0400 7401 6b0a 7234 0100 7d01  ..S...t.k.r4..}.
+00002c60: 0100 7a0e 6401 7402 7c01 6a03 8301 6901  ..z.d.t.|.j...i.
+00002c70: 5300 6400 7d01 7e01 5800 6e02 5800 6400  S.d.}.~.X.n.X.d.
+00002c80: 5300 2902 4eda 0565 7272 6f72 2904 72b1  S.).N..error).r.
+00002c90: 0000 0072 1100 0000 da03 7374 72da 0664  ...r......str..d
+00002ca0: 6574 6169 6c29 0272 3c00 0000 72bd 0000  etail).r<...r...
+00002cb0: 0029 01da 0a73 6572 6961 6c69 7a65 7272  .)...serializerr
+00002cc0: 2300 0000 7224 0000 00da 096d 6170 5f71  #...r$.....map_q
+00002cd0: 7565 7279 6f01 0000 7308 0000 0000 0102  ueryo...s.......
+00002ce0: 010a 0110 017a 2953 716c 7353 6572 6961  .....z)SqlsSeria
+00002cf0: 6c69 7a65 722e 6578 6563 7574 652e 3c6c  lizer.execute.<l
+00002d00: 6f63 616c 733e 2e6d 6170 5f71 7565 7279  ocals>.map_query
+00002d10: da07 7175 6572 6965 7329 0472 3400 0000  ..queries).r4...
+00002d20: 728a 0000 0072 6700 0000 724a 0000 0029  r....rg...rJ...)
+00002d30: 0372 4c00 0000 7256 0000 0072 c600 0000  .rL...rV...r....
+00002d40: 7223 0000 0029 0172 c500 0000 7224 0000  r#...).r....r$..
+00002d50: 0072 b100 0000 6c01 0000 7306 0000 0000  .r....l...s.....
+00002d60: 010c 020c 067a 1653 716c 7353 6572 6961  .....z.SqlsSeria
+00002d70: 6c69 7a65 722e 6578 6563 7574 654e 2906  lizer.executeN).
+00002d80: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00002d90: 3400 0000 72c7 0000 0072 b100 0000 7223  4...r....r....r#
+00002da0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00002db0: 0000 72c1 0000 0069 0100 0073 0400 0000  ..r....i...s....
+00002dc0: 0801 0a02 72c1 0000 004e 2931 da1e 6a65  ....r....N)1..je
+00002dd0: 745f 6272 6964 6765 5f62 6173 652e 7574  t_bridge_base.ut
+00002de0: 696c 732e 7175 6572 7973 6574 7202 0000  ils.querysetr...
+00002df0: 0072 0300 0000 da0a 7371 6c61 6c63 6865  .r......sqlalche
+00002e00: 6d79 7204 0000 0072 0500 0000 7206 0000  myr....r....r...
+00002e10: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+00002e20: 720a 0000 0072 0b00 0000 5a0e 7371 6c61  r....r....Z.sqla
+00002e30: 6c63 6865 6d79 2e73 716c 720c 0000 00da  lchemy.sqlr.....
+00002e40: 0e73 716c 616c 6368 656d 792e 6578 6372  .sqlalchemy.excr
+00002e50: 0d00 0000 da0f 6a65 745f 6272 6964 6765  ......jet_bridge
+00002e60: 5f62 6173 6572 0e00 0000 da12 6a65 745f  _baser......jet_
+00002e70: 6272 6964 6765 5f62 6173 652e 6462 720f  bridge_base.dbr.
+00002e80: 0000 0072 1000 0000 5a1e 6a65 745f 6272  ...r....Z.jet_br
+00002e90: 6964 6765 5f62 6173 652e 6578 6365 7074  idge_base.except
+00002ea0: 696f 6e73 2e73 716c 7211 0000 00da 2b6a  ions.sqlr.....+j
+00002eb0: 6574 5f62 7269 6467 655f 6261 7365 2e65  et_bridge_base.e
+00002ec0: 7863 6570 7469 6f6e 732e 7661 6c69 6461  xceptions.valida
+00002ed0: 7469 6f6e 5f65 7272 6f72 7212 0000 005a  tion_errorr....Z
+00002ee0: 216a 6574 5f62 7269 6467 655f 6261 7365  !jet_bridge_base
+00002ef0: 2e66 6965 6c64 732e 7371 6c5f 7061 7261  .fields.sql_para
+00002f00: 6d73 7213 0000 00da 176a 6574 5f62 7269  msr......jet_bri
+00002f10: 6467 655f 6261 7365 2e66 696c 7465 7273  dge_base.filters
+00002f20: 7214 0000 00da 1e6a 6574 5f62 7269 6467  r......jet_bridg
+00002f30: 655f 6261 7365 2e66 696c 7465 7273 2e66  e_base.filters.f
+00002f40: 696c 7465 7272 1500 0000 da23 6a65 745f  ilterr.....#jet_
+00002f50: 6272 6964 6765 5f62 6173 652e 6669 6c74  bridge_base.filt
+00002f60: 6572 732e 6d6f 6465 6c5f 6772 6f75 7072  ers.model_groupr
+00002f70: 1600 0000 7217 0000 00da 2a6a 6574 5f62  ....r.....*jet_b
+00002f80: 7269 6467 655f 6261 7365 2e66 696c 7465  ridge_base.filte
+00002f90: 7273 2e66 696c 7465 725f 666f 725f 6462  rs.filter_for_db
+00002fa0: 6669 656c 6472 1800 0000 da26 6a65 745f  fieldr.....&jet_
+00002fb0: 6272 6964 6765 5f62 6173 652e 7365 7269  bridge_base.seri
+00002fc0: 616c 697a 6572 732e 7365 7269 616c 697a  alizers.serializ
+00002fd0: 6572 7219 0000 005a 1e6a 6574 5f62 7269  err....Z.jet_bri
+00002fe0: 6467 655f 6261 7365 2e75 7469 6c73 2e64  dge_base.utils.d
+00002ff0: 625f 7479 7065 7372 1a00 0000 721b 0000  b_typesr....r...
+00003000: 0072 1c00 0000 7225 0000 0072 2a00 0000  .r....r%...r*...
+00003010: 722b 0000 0072 3000 0000 7231 0000 0072  r+...r0...r1...r
+00003020: 3400 0000 72c1 0000 0072 2300 0000 7223  4...r....r#...r#
+00003030: 0000 0072 2300 0000 7224 0000 00da 083c  ...r#...r$.....<
+00003040: 6d6f 6475 6c65 3e01 0000 0073 3200 0000  module>....s2...
+00003050: 1001 2401 0c01 0c01 0c02 0c01 1001 0c01  ..$.............
+00003060: 0c01 0c01 0c01 0c01 1001 0c01 0c01 1003  ................
+00003070: 1005 1005 1005 1007 1005 1006 107f 007f  ................
+00003080: 0036                                     .6
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/sql.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/sql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_group.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_group.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/message.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/message.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/message.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reorder.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reorder.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reset_order.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reset_order.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/table.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/table.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_serializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reset_order.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reset_order.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_description.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_description.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-00000000: 330d 0d0a 76b0 eb63 e008 0000 e300 0000  3...v..c........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4c00 0000 6400 6401 6c00 6d01 5a02  .sL...d.d.l.m.Z.
-00000030: 0100 6400 6402 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
-00000040: 6403 6404 8400 6404 6504 8303 5a05 4700  d.d...d.e...Z.G.
-00000050: 6405 6406 8400 6406 6504 8303 5a06 4700  d.d...d.e...Z.G.
-00000060: 6407 6408 8400 6408 6504 8303 5a07 6409  d.d...d.e...Z.d.
-00000070: 5300 290a e900 0000 0029 01da 0666 6965  S.)......)...fie
-00000080: 6c64 7329 01da 0a53 6572 6961 6c69 7a65  lds)...Serialize
-00000090: 7263 0000 0000 0000 0000 0000 0000 0300  rc..............
-000000a0: 0000 4000 0000 73dc 0000 0065 005a 0164  ..@...s....e.Z.d
-000000b0: 005a 0265 036a 0483 005a 0565 036a 0483  .Z.e.j...Z.e.j..
-000000c0: 005a 0665 036a 0483 005a 0765 036a 0483  .Z.e.j...Z.e.j..
-000000d0: 005a 0865 036a 0983 005a 0a65 036a 0983  .Z.e.j...Z.e.j..
-000000e0: 005a 0b65 036a 0983 005a 0c65 036a 0d83  .Z.e.j...Z.e.j..
-000000f0: 005a 0e65 036a 0464 0164 028d 015a 0f65  .Z.e.j.d.d...Z.e
-00000100: 036a 0464 0164 028d 015a 1065 036a 0d64  .j.d.d...Z.e.j.d
-00000110: 0164 028d 015a 1165 036a 0464 0164 028d  .d...Z.e.j.d.d..
-00000120: 015a 1265 036a 0964 0164 028d 015a 1365  .Z.e.j.d.d...Z.e
-00000130: 036a 0464 0164 028d 015a 1465 036a 0964  .j.d.d...Z.e.j.d
-00000140: 0164 028d 015a 1565 036a 0464 0164 028d  .d...Z.e.j.d.d..
-00000150: 015a 1665 036a 1764 0164 028d 015a 1865  .Z.e.j.d.d...Z.e
-00000160: 036a 1964 0164 028d 015a 1a65 036a 0d64  .j.d.d...Z.e.j.d
-00000170: 0164 028d 015a 1b65 036a 0464 0164 028d  .d...Z.e.j.d.d..
-00000180: 015a 1c64 0353 0029 04da 1f4d 6f64 656c  .Z.d.S.)...Model
-00000190: 4465 7363 7269 7074 696f 6e46 6965 6c64  DescriptionField
-000001a0: 5365 7269 616c 697a 6572 4629 01da 0872  SerializerF)...r
-000001b0: 6571 7569 7265 644e 291d da08 5f5f 6e61  equiredN)...__na
-000001c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000001d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-000001e0: 6669 656c 6473 5fda 0943 6861 7246 6965  fields_..CharFie
-000001f0: 6c64 da04 6e61 6d65 da09 6462 5f63 6f6c  ld..name..db_col
-00000200: 756d 6eda 0566 6965 6c64 da08 6462 5f66  umn..field..db_f
-00000210: 6965 6c64 da0c 426f 6f6c 6561 6e46 6965  ield..BooleanFie
-00000220: 6c64 da0a 6669 6c74 6572 6162 6c65 da04  ld..filterable..
-00000230: 6e75 6c6c da08 6564 6974 6162 6c65 da09  null..editable..
-00000240: 4a53 4f4e 4669 656c 64da 0670 6172 616d  JSONField..param
-00000250: 73da 1164 6174 615f 736f 7572 6365 5f66  s..data_source_f
-00000260: 6965 6c64 da10 6461 7461 5f73 6f75 7263  ield..data_sourc
-00000270: 655f 6e61 6d65 da12 6461 7461 5f73 6f75  e_name..data_sou
-00000280: 7263 655f 7061 7261 6d73 da17 6461 7461  rce_params..data
-00000290: 5f73 6f75 7263 655f 6f72 6465 725f 6166  _source_order_af
-000002a0: 7465 72da 1264 6174 615f 736f 7572 6365  ter..data_source
-000002b0: 5f68 6964 6465 6eda 0c76 6572 626f 7365  _hidden..verbose
-000002c0: 5f6e 616d 6572 0500 0000 da0c 6465 6661  _namer......defa
-000002d0: 756c 745f 7479 7065 da08 5261 7746 6965  ult_type..RawFie
-000002e0: 6c64 da0d 6465 6661 756c 745f 7661 6c75  ld..default_valu
-000002f0: 65da 0c49 6e74 6567 6572 4669 656c 64da  e..IntegerField.
-00000300: 066c 656e 6774 68da 0d72 656c 6174 6564  .length..related
-00000310: 5f6d 6f64 656c da12 6375 7374 6f6d 5f70  _model..custom_p
-00000320: 7269 6d61 7279 5f6b 6579 a900 7222 0000  rimary_key..r"..
-00000330: 0072 2200 0000 fa74 2f55 7365 7273 2f66  .r"....t/Users/f
-00000340: 316e 616c 2f44 726f 7062 6f78 2f70 7974  1nal/Dropbox/pyt
-00000350: 686f 6e2f 6a65 742d 6272 6964 6765 2f73  hon/jet-bridge/s
-00000360: 7263 2f70 6163 6b61 6765 732f 6a65 745f  rc/packages/jet_
-00000370: 6272 6964 6765 5f62 6173 652f 6a65 745f  bridge_base/jet_
-00000380: 6272 6964 6765 5f62 6173 652f 7365 7269  bridge_base/seri
-00000390: 616c 697a 6572 732f 6d6f 6465 6c5f 6465  alizers/model_de
-000003a0: 7363 7269 7074 696f 6e2e 7079 7204 0000  scription.pyr...
-000003b0: 0005 0000 0073 2800 0000 0801 0801 0801  .....s(.........
-000003c0: 0801 0801 0801 0801 0801 0801 0c01 0c01  ................
+00000000: 420d 0d0a 0000 0000 76b0 eb63 e008 0000  B.......v..c....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 4c00 0000 6400 6401 6c00  .@...sL...d.d.l.
+00000030: 6d01 5a02 0100 6400 6402 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6504 8303  ..G.d.d...d.e...
+00000050: 5a05 4700 6405 6406 8400 6406 6504 8303  Z.G.d.d...d.e...
+00000060: 5a06 4700 6407 6408 8400 6408 6504 8303  Z.G.d.d...d.e...
+00000070: 5a07 6409 5300 290a e900 0000 0029 01da  Z.d.S.)......)..
+00000080: 0666 6965 6c64 7329 01da 0a53 6572 6961  .fields)...Seria
+00000090: 6c69 7a65 7263 0000 0000 0000 0000 0000  lizerc..........
+000000a0: 0000 0300 0000 4000 0000 73dc 0000 0065  ......@...s....e
+000000b0: 005a 0164 005a 0265 03a0 04a1 005a 0565  .Z.d.Z.e.....Z.e
+000000c0: 03a0 04a1 005a 0665 03a0 04a1 005a 0765  .....Z.e.....Z.e
+000000d0: 03a0 04a1 005a 0865 03a0 09a1 005a 0a65  .....Z.e.....Z.e
+000000e0: 03a0 09a1 005a 0b65 03a0 09a1 005a 0c65  .....Z.e.....Z.e
+000000f0: 03a0 0da1 005a 0e65 036a 0464 0164 028d  .....Z.e.j.d.d..
+00000100: 015a 0f65 036a 0464 0164 028d 015a 1065  .Z.e.j.d.d...Z.e
+00000110: 036a 0d64 0164 028d 015a 1165 036a 0464  .j.d.d...Z.e.j.d
+00000120: 0164 028d 015a 1265 036a 0964 0164 028d  .d...Z.e.j.d.d..
+00000130: 015a 1365 036a 0464 0164 028d 015a 1465  .Z.e.j.d.d...Z.e
+00000140: 036a 0964 0164 028d 015a 1565 036a 0464  .j.d.d...Z.e.j.d
+00000150: 0164 028d 015a 1665 036a 1764 0164 028d  .d...Z.e.j.d.d..
+00000160: 015a 1865 036a 1964 0164 028d 015a 1a65  .Z.e.j.d.d...Z.e
+00000170: 036a 0d64 0164 028d 015a 1b65 036a 0464  .j.d.d...Z.e.j.d
+00000180: 0164 028d 015a 1c64 0353 0029 04da 1f4d  .d...Z.d.S.)...M
+00000190: 6f64 656c 4465 7363 7269 7074 696f 6e46  odelDescriptionF
+000001a0: 6965 6c64 5365 7269 616c 697a 6572 4629  ieldSerializerF)
+000001b0: 01da 0872 6571 7569 7265 644e 291d da08  ...requiredN)...
+000001c0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000001d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000001e0: 5f5f da07 6669 656c 6473 5fda 0943 6861  __..fields_..Cha
+000001f0: 7246 6965 6c64 da04 6e61 6d65 da09 6462  rField..name..db
+00000200: 5f63 6f6c 756d 6eda 0566 6965 6c64 da08  _column..field..
+00000210: 6462 5f66 6965 6c64 da0c 426f 6f6c 6561  db_field..Boolea
+00000220: 6e46 6965 6c64 da0a 6669 6c74 6572 6162  nField..filterab
+00000230: 6c65 da04 6e75 6c6c da08 6564 6974 6162  le..null..editab
+00000240: 6c65 da09 4a53 4f4e 4669 656c 64da 0670  le..JSONField..p
+00000250: 6172 616d 73da 1164 6174 615f 736f 7572  arams..data_sour
+00000260: 6365 5f66 6965 6c64 da10 6461 7461 5f73  ce_field..data_s
+00000270: 6f75 7263 655f 6e61 6d65 da12 6461 7461  ource_name..data
+00000280: 5f73 6f75 7263 655f 7061 7261 6d73 da17  _source_params..
+00000290: 6461 7461 5f73 6f75 7263 655f 6f72 6465  data_source_orde
+000002a0: 725f 6166 7465 72da 1264 6174 615f 736f  r_after..data_so
+000002b0: 7572 6365 5f68 6964 6465 6eda 0c76 6572  urce_hidden..ver
+000002c0: 626f 7365 5f6e 616d 6572 0500 0000 da0c  bose_namer......
+000002d0: 6465 6661 756c 745f 7479 7065 da08 5261  default_type..Ra
+000002e0: 7746 6965 6c64 da0d 6465 6661 756c 745f  wField..default_
+000002f0: 7661 6c75 65da 0c49 6e74 6567 6572 4669  value..IntegerFi
+00000300: 656c 64da 066c 656e 6774 68da 0d72 656c  eld..length..rel
+00000310: 6174 6564 5f6d 6f64 656c da12 6375 7374  ated_model..cust
+00000320: 6f6d 5f70 7269 6d61 7279 5f6b 6579 a900  om_primary_key..
+00000330: 7222 0000 0072 2200 0000 fa74 2f55 7365  r"...r"....t/Use
+00000340: 7273 2f66 316e 616c 2f44 726f 7062 6f78  rs/f1nal/Dropbox
+00000350: 2f70 7974 686f 6e2f 6a65 742d 6272 6964  /python/jet-brid
+00000360: 6765 2f73 7263 2f70 6163 6b61 6765 732f  ge/src/packages/
+00000370: 6a65 745f 6272 6964 6765 5f62 6173 652f  jet_bridge_base/
+00000380: 6a65 745f 6272 6964 6765 5f62 6173 652f  jet_bridge_base/
+00000390: 7365 7269 616c 697a 6572 732f 6d6f 6465  serializers/mode
+000003a0: 6c5f 6465 7363 7269 7074 696f 6e2e 7079  l_description.py
+000003b0: 7204 0000 0005 0000 0073 2800 0000 0801  r........s(.....
+000003c0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
 000003d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000003e0: 0c01 7204 0000 0063 0000 0000 0000 0000  ..r....c........
-000003f0: 0000 0000 0100 0000 4000 0000 7334 0000  ........@...s4..
-00000400: 0065 005a 0164 005a 0265 036a 0483 005a  .e.Z.d.Z.e.j...Z
-00000410: 0565 036a 0483 005a 0665 036a 0483 005a  .e.j...Z.e.j...Z
-00000420: 0765 036a 0483 005a 0865 036a 0483 005a  .e.j...Z.e.j...Z
-00000430: 0964 0153 0029 02da 224d 6f64 656c 4465  .d.S.).."ModelDe
-00000440: 7363 7269 7074 696f 6e52 656c 6174 696f  scriptionRelatio
-00000450: 6e53 6572 6961 6c69 7a65 724e 290a 7206  nSerializerN).r.
-00000460: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00000470: 0000 720a 0000 0072 0b00 0000 da09 6469  ..r....r......di
-00000480: 7265 6374 696f 6eda 0b6c 6f63 616c 5f66  rection..local_f
-00000490: 6965 6c64 7220 0000 00da 0d72 656c 6174  ieldr .....relat
-000004a0: 6564 5f66 6965 6c64 7222 0000 0072 2200  ed_fieldr"...r".
-000004b0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-000004c0: 001c 0000 0073 0a00 0000 0801 0801 0801  .....s..........
-000004d0: 0801 0801 7224 0000 0063 0000 0000 0000  ....r$...c......
-000004e0: 0000 0000 0000 0400 0000 4000 0000 73b4  ..........@...s.
-000004f0: 0000 0065 005a 0164 005a 0265 036a 0483  ...e.Z.d.Z.e.j..
-00000500: 005a 0565 036a 0483 005a 0665 036a 0783  .Z.e.j...Z.e.j..
-00000510: 005a 0865 036a 0483 005a 0965 036a 0783  .Z.e.j...Z.e.j..
-00000520: 005a 0a65 0b64 0164 028d 015a 0c65 0d64  .Z.e.d.d...Z.e.d
-00000530: 0164 028d 015a 0e65 0d64 0164 0364 048d  .d...Z.e.d.d.d..
-00000540: 025a 0f65 036a 0464 0364 058d 015a 1065  .Z.e.j.d.d...Z.e
-00000550: 036a 0464 0364 058d 015a 1165 036a 0464  .j.d.d...Z.e.j.d
-00000560: 0364 058d 015a 1265 036a 0464 0364 058d  .d...Z.e.j.d.d..
-00000570: 015a 1365 036a 0464 0364 058d 015a 1465  .Z.e.j.d.d...Z.e
-00000580: 036a 0464 0364 058d 015a 1565 036a 0464  .j.d.d...Z.e.j.d
-00000590: 0364 058d 015a 1665 036a 0764 0364 058d  .d...Z.e.j.d.d..
-000005a0: 015a 1764 0653 0029 07da 1a4d 6f64 656c  .Z.d.S.)...Model
-000005b0: 4465 7363 7269 7074 696f 6e53 6572 6961  DescriptionSeria
-000005c0: 6c69 7a65 7254 2901 da04 6d61 6e79 4629  lizerT)...manyF)
-000005d0: 0272 2900 0000 7205 0000 0029 0172 0500  .r)...r....).r..
-000005e0: 0000 4e29 1872 0600 0000 7207 0000 0072  ..N).r....r....r
-000005f0: 0800 0000 7209 0000 0072 0a00 0000 da05  ....r....r......
-00000600: 6d6f 6465 6cda 0864 625f 7461 626c 6572  model..db_tabler
-00000610: 0f00 0000 da06 6869 6464 656e da11 7072  ......hidden..pr
-00000620: 696d 6172 795f 6b65 795f 6669 656c 64da  imary_key_field.
-00000630: 1070 7269 6d61 7279 5f6b 6579 5f61 7574  .primary_key_aut
-00000640: 6f72 0400 0000 7202 0000 0072 2400 0000  or....r....r$...
-00000650: da09 7265 6c61 7469 6f6e 73da 1272 656c  ..relations..rel
-00000660: 6174 696f 6e5f 6f76 6572 7269 6465 7372  ation_overridesr
-00000670: 1a00 0000 5a13 7665 7262 6f73 655f 6e61  ....Z.verbose_na
-00000680: 6d65 5f70 6c75 7261 6c5a 0d64 6973 706c  me_pluralZ.displ
-00000690: 6179 5f66 6965 6c64 5a10 6465 6661 756c  ay_fieldZ.defaul
-000006a0: 745f 6f72 6465 725f 6279 7216 0000 00da  t_order_byr.....
-000006b0: 1764 6174 615f 736f 7572 6365 5f6e 616d  .data_source_nam
-000006c0: 655f 706c 7572 616c 7218 0000 0072 1900  e_pluralr....r..
-000006d0: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
-000006e0: 0072 2300 0000 7228 0000 0024 0000 0073  .r#...r(...$...s
-000006f0: 2000 0000 0801 0801 0801 0801 0801 0801   ...............
-00000700: 0a01 0a01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000710: 0c01 0c01 7228 0000 004e 2908 da0f 6a65  ....r(...N)...je
-00000720: 745f 6272 6964 6765 5f62 6173 6572 0200  t_bridge_baser..
-00000730: 0000 7209 0000 00da 266a 6574 5f62 7269  ..r.....&jet_bri
-00000740: 6467 655f 6261 7365 2e73 6572 6961 6c69  dge_base.seriali
-00000750: 7a65 7273 2e73 6572 6961 6c69 7a65 7272  zers.serializerr
-00000760: 0300 0000 7204 0000 0072 2400 0000 7228  ....r....r$...r(
-00000770: 0000 0072 2200 0000 7222 0000 0072 2200  ...r"...r"...r".
-00000780: 0000 7223 0000 00da 083c 6d6f 6475 6c65  ..r#.....<module
-00000790: 3e01 0000 0073 0800 0000 0c01 0c03 1017  >....s..........
-000007a0: 1008                                     ..
+000003e0: 0c01 0c01 0c01 7204 0000 0063 0000 0000  ......r....c....
+000003f0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+00000400: 7334 0000 0065 005a 0164 005a 0265 03a0  s4...e.Z.d.Z.e..
+00000410: 04a1 005a 0565 03a0 04a1 005a 0665 03a0  ...Z.e.....Z.e..
+00000420: 04a1 005a 0765 03a0 04a1 005a 0865 03a0  ...Z.e.....Z.e..
+00000430: 04a1 005a 0964 0153 0029 02da 224d 6f64  ...Z.d.S.).."Mod
+00000440: 656c 4465 7363 7269 7074 696f 6e52 656c  elDescriptionRel
+00000450: 6174 696f 6e53 6572 6961 6c69 7a65 724e  ationSerializerN
+00000460: 290a 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
+00000470: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000480: da09 6469 7265 6374 696f 6eda 0b6c 6f63  ..direction..loc
+00000490: 616c 5f66 6965 6c64 7220 0000 00da 0d72  al_fieldr .....r
+000004a0: 656c 6174 6564 5f66 6965 6c64 7222 0000  elated_fieldr"..
+000004b0: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+000004c0: 7224 0000 001c 0000 0073 0a00 0000 0801  r$.......s......
+000004d0: 0801 0801 0801 0801 7224 0000 0063 0000  ........r$...c..
+000004e0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+000004f0: 0000 73b4 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
+00000500: 03a0 04a1 005a 0565 03a0 04a1 005a 0665  .....Z.e.....Z.e
+00000510: 03a0 07a1 005a 0865 03a0 04a1 005a 0965  .....Z.e.....Z.e
+00000520: 03a0 07a1 005a 0a65 0b64 0164 028d 015a  .....Z.e.d.d...Z
+00000530: 0c65 0d64 0164 028d 015a 0e65 0d64 0164  .e.d.d...Z.e.d.d
+00000540: 0364 048d 025a 0f65 036a 0464 0364 058d  .d...Z.e.j.d.d..
+00000550: 015a 1065 036a 0464 0364 058d 015a 1165  .Z.e.j.d.d...Z.e
+00000560: 036a 0464 0364 058d 015a 1265 036a 0464  .j.d.d...Z.e.j.d
+00000570: 0364 058d 015a 1365 036a 0464 0364 058d  .d...Z.e.j.d.d..
+00000580: 015a 1465 036a 0464 0364 058d 015a 1565  .Z.e.j.d.d...Z.e
+00000590: 036a 0464 0364 058d 015a 1665 036a 0764  .j.d.d...Z.e.j.d
+000005a0: 0364 058d 015a 1764 0653 0029 07da 1a4d  .d...Z.d.S.)...M
+000005b0: 6f64 656c 4465 7363 7269 7074 696f 6e53  odelDescriptionS
+000005c0: 6572 6961 6c69 7a65 7254 2901 da04 6d61  erializerT)...ma
+000005d0: 6e79 4629 0272 2900 0000 7205 0000 0029  nyF).r)...r....)
+000005e0: 0172 0500 0000 4e29 1872 0600 0000 7207  .r....N).r....r.
+000005f0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000600: 0000 da05 6d6f 6465 6cda 0864 625f 7461  ....model..db_ta
+00000610: 626c 6572 0f00 0000 da06 6869 6464 656e  bler......hidden
+00000620: da11 7072 696d 6172 795f 6b65 795f 6669  ..primary_key_fi
+00000630: 656c 64da 1070 7269 6d61 7279 5f6b 6579  eld..primary_key
+00000640: 5f61 7574 6f72 0400 0000 7202 0000 0072  _autor....r....r
+00000650: 2400 0000 da09 7265 6c61 7469 6f6e 73da  $.....relations.
+00000660: 1272 656c 6174 696f 6e5f 6f76 6572 7269  .relation_overri
+00000670: 6465 7372 1a00 0000 5a13 7665 7262 6f73  desr....Z.verbos
+00000680: 655f 6e61 6d65 5f70 6c75 7261 6c5a 0d64  e_name_pluralZ.d
+00000690: 6973 706c 6179 5f66 6965 6c64 5a10 6465  isplay_fieldZ.de
+000006a0: 6661 756c 745f 6f72 6465 725f 6279 7216  fault_order_byr.
+000006b0: 0000 00da 1764 6174 615f 736f 7572 6365  .....data_source
+000006c0: 5f6e 616d 655f 706c 7572 616c 7218 0000  _name_pluralr...
+000006d0: 0072 1900 0000 7222 0000 0072 2200 0000  .r....r"...r"...
+000006e0: 7222 0000 0072 2300 0000 7228 0000 0024  r"...r#...r(...$
+000006f0: 0000 0073 2000 0000 0801 0801 0801 0801  ...s ...........
+00000700: 0801 0801 0a01 0a01 0c01 0c01 0c01 0c01  ................
+00000710: 0c01 0c01 0c01 0c01 7228 0000 004e 2908  ........r(...N).
+00000720: da0f 6a65 745f 6272 6964 6765 5f62 6173  ..jet_bridge_bas
+00000730: 6572 0200 0000 7209 0000 00da 266a 6574  er....r.....&jet
+00000740: 5f62 7269 6467 655f 6261 7365 2e73 6572  _bridge_base.ser
+00000750: 6961 6c69 7a65 7273 2e73 6572 6961 6c69  ializers.seriali
+00000760: 7a65 7272 0300 0000 7204 0000 0072 2400  zerr....r....r$.
+00000770: 0000 7228 0000 0072 2200 0000 7222 0000  ..r(...r"...r"..
+00000780: 0072 2200 0000 7223 0000 00da 083c 6d6f  .r"...r#.....<mo
+00000790: 6475 6c65 3e01 0000 0073 0800 0000 0c01  dule>....s......
+000007a0: 0c03 1017 1008                           ......
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/table.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/relationship_override.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/relationship_override.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/proxy_request.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/model_description.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/model_description.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/__pycache__/reorder.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/__pycache__/reorder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/model_description.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/model_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 class ModelDescriptionSerializer(Serializer):
     model = fields_.CharField()
     db_table = fields_.CharField()
     hidden = fields_.BooleanField()
     primary_key_field = fields_.CharField()
     primary_key_auto = fields_.BooleanField()
+    is_view = fields_.BooleanField()
     fields = ModelDescriptionFieldSerializer(many=True)
     relations = ModelDescriptionRelationSerializer(many=True)
     relation_overrides = ModelDescriptionRelationSerializer(many=True, required=False)
     verbose_name = fields_.CharField(required=False)
     verbose_name_plural = fields_.CharField(required=False)
     display_field = fields_.CharField(required=False)
     default_order_by = fields_.CharField(required=False)
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/reorder.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/reorder.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/serializer.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/table.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/table.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/sql.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,18 +228,25 @@
             name = name[1:]
             descending = True
         field = column(name)
         if descending:
             field = desc(field)
         return field
 
-    def sort_queryset(self, queryset, data):
+    def sort_queryset(self, queryset, data, session):
         if 'order_by' in data:
             order_by = list(map(lambda x: self.map_order_field(x), data['order_by']))
             queryset = queryset.order_by(*order_by)
+        else:
+            if 'aggregate' not in data and 'group' not in data and 'groups' not in data:
+                if get_session_engine(session) == 'mssql':
+                    for item in data.get('columns', []):
+                        field = column(item['name'])
+                        queryset = queryset.order_by(field)
+                        break
 
         return queryset
 
     def execute(self, data):
         request = self.context.get('request')
         session = request.session
 
@@ -289,15 +296,15 @@
 
             queryset = self.filter_queryset(queryset, data)
 
             if 'aggregate' not in data and 'group' not in data and 'groups' not in data:
                 queryset = self.paginate_queryset(queryset, data)
 
             if 'group' not in data and 'groups' not in data:
-                queryset = self.sort_queryset(queryset, data)
+                queryset = self.sort_queryset(queryset, data, session)
 
             result = session.execute(queryset, params)
 
             def map_column(x):
                 if x == '?column?':
                     return
                 return x
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/proxy_request.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/proxy_request.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/serializers/model_serializer.py` & `jet-bridge-base-1.8.2/jet_bridge_base/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/media_cache.py` & `jet-bridge-base-1.8.2/jet_bridge_base/media_cache.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/settings.py` & `jet-bridge-base-1.8.2/jet_bridge_base/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,16 +28,21 @@
 DATABASE_USER = None
 DATABASE_PASSWORD = None
 DATABASE_NAME = None
 DATABASE_EXTRA = None
 DATABASE_CONNECTIONS = None
 DATABASE_ONLY = None
 DATABASE_EXCEPT = None
+DATABASE_MAX_TABLES = None
 DATABASE_SCHEMA = None
 
+DATABASE_SSL_CA = None
+DATABASE_SSL_CERT = None
+DATABASE_SSL_KEY = None
+
 DATABASE_SSH_HOST = None
 DATABASE_SSH_PORT = None
 DATABASE_SSH_USER = None
 DATABASE_SSH_PRIVATE_KEY = None
 
 COOKIE_SAMESITE = None
 COOKIE_SECURE = None
@@ -53,14 +58,16 @@
 TRACK_DATABASES = ''
 TRACK_DATABASES_ENDPOINT = ''
 TRACK_DATABASES_AUTH = ''
 
 TRACK_MODELS_ENDPOINT = ''
 TRACK_MODELS_AUTH = ''
 
+DISABLE_AUTH = None
+
 
 def set_settings(settings):
     for key, value in settings.items():
         if value is None:
             continue
         setattr(CURRENT_MODULE, key, value)
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/permissions.py` & `jet-bridge-base-1.8.2/jet_bridge_base/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
                     continue
 
             return view_permission_actions in item_actions
 
         return False
 
     def has_permission(self, view, request):
-        # return True
         token = self.parse_token(request.headers.get('AUTHORIZATION'))
         view_permissions = view.required_project_permission(request) if hasattr(view, 'required_project_permission') else None
 
         if not token:
             return False
 
         bridge_settings = request.get_bridge_settings()
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/templates/500.debug.html` & `jet-bridge-base-1.8.2/jet_bridge_base/templates/500.debug.html`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/templates/external_auth_complete.html` & `jet-bridge-base-1.8.2/jet_bridge_base/templates/external_auth_complete.html`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/field.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/field.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/float.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/float.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/char.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/char.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/float.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/float.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/raw.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/raw.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/raw.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/raw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/datetime.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/datetime.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/sql_params.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/sql_params.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/field.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/field.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/char.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/char.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/array.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/boolean.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/boolean.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/array.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/array.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/boolean.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/boolean.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/datetime.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/datetime.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/char.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/char.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/integer.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/integer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/json.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/json.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/wkt.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/wkt.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/wkt.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/wkt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/integer.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/integer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/field.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/field.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/__init__.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/json.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/json.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/sql_params.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/sql_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/__pycache__/__init__.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/boolean.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/integer.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/integer.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/wkt.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/wkt.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,13 @@
         except ArgumentError as e:
             self.error('invalid', error=six.text_type(e))
 
     def to_representation_item(self, value):
         if value is None:
             return
         from geoalchemy2.shape import to_shape
-        return to_shape(value).to_wkt()
+        shape = to_shape(value)
+        if hasattr(shape, 'wkt'):
+            return shape.wkt
+        else:
+            # Backward compatibility Shapely <1.8.0
+            return shape.to_wkt()
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/array.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/array.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/datetime.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/datetime.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/fields/json.py` & `jet-bridge-base-1.8.2/jet_bridge_base/fields/json.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/commands/check_token.py` & `jet-bridge-base-1.8.2/jet_bridge_base/commands/check_token.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/check_token.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/check_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/commands/__pycache__/check_token.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/commands/__pycache__/check_token.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/ssh_tunnel.py` & `jet-bridge-base-1.8.2/jet_bridge_base/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/sentry.py` & `jet-bridge-base-1.8.2/jet_bridge_base/sentry.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/graphql.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/graphql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import threading
 import time
 from datetime import timedelta
 
 from graphql import GraphQLError
 
-from jet_bridge_base.db import connection_cache
+from jet_bridge_base.db import connection_cache, get_table_name, get_mapped_base, get_connection_id_short
 from jet_bridge_base.exceptions.permission_denied import PermissionDenied
 from jet_bridge_base.logger import logger
 from jet_bridge_base.permissions import HasProjectPermissions
 from jet_bridge_base.responses.json import JSONResponse
 from jet_bridge_base.utils.common import get_random_string
 from jet_bridge_base.utils.graphql import GraphQLSchemaGenerator
+from jet_bridge_base.utils.process import get_memory_usage_human
+from jet_bridge_base.utils.track_database import track_database_async
 from jet_bridge_base.views.base.api import APIView
 
 
 class GraphQLView(APIView):
     permission_classes = (HasProjectPermissions,)
 
     def before_dispatch_permissions_check(self, request):
@@ -33,57 +35,89 @@
         else:
             return str(error)
 
     def wait_schema(self, request, schema_key, wait_schema):
         if not wait_schema:
             return
 
-        logger.info('Waiting GraphQL schema "{}"...'.format(wait_schema['id']))
+        id_short = get_connection_id_short(request)
+
+        logger.info('[{}] Waiting GraphQL schema "{}"...'.format(id_short, wait_schema['id']))
 
         generated_condition = wait_schema['generated']
         with generated_condition:
             timeout = timedelta(minutes=10).total_seconds()
             generated_condition.wait(timeout=timeout)
 
         with connection_cache(request) as cache:
             cached_schema = cache.get(schema_key)
             if cached_schema and cached_schema['instance']:
-                logger.info('Found GraphQL schema "{}"'.format(wait_schema['id']))
+                logger.info('[{}] Found GraphQL schema "{}"'.format(id_short, wait_schema['id']))
                 return cached_schema['instance']
             else:
-                logger.info('Not found GraphQL schema "{}"'.format(wait_schema['id']))
+                logger.info('[{}] Not found GraphQL schema "{}"'.format(id_short, wait_schema['id']))
 
     def create_schema_object(self):
         new_schema_id = get_random_string(32)
         new_schema_generated = threading.Condition()
         return {'id': new_schema_id, 'instance': None, 'get_schema_time': None, 'generated': new_schema_generated}
 
     def create_schema(self, request, schema_key, new_schema, draft):
+        id_short = get_connection_id_short(request)
+
         try:
-            logger.info('Generating GraphQL schema "{}"...'.format(new_schema['id']))
+            logger.info('[{}] Generating GraphQL schema "{}"...'.format(id_short, new_schema['id']))
 
             def before_resolve(request, mapper, *args, **kwargs):
-                request.context['model'] = mapper.selectable.name
+                MappedBase = get_mapped_base(request)
+                request.context['model'] = get_table_name(MappedBase.metadata, mapper.selectable)
                 self.check_permissions(request)
 
+            def on_progress_updated(request, new_schema, current_name, i, total):
+                if current_name is not None:
+                    logger.info('[{}] Generating GraphQL schema "{}" ({} / {}) (Mem:{})...'.format(
+                        id_short,
+                        current_name,
+                        i + 1,
+                        total,
+                        get_memory_usage_human()
+                    ))
+
+                with connection_cache(request) as cache:
+                    cached_schema = cache.get(schema_key)
+
+                    if cached_schema and cached_schema['id'] == new_schema['id']:
+                        new_schema = {**cached_schema, 'tables_processed': i, 'tables_total': total}
+                        cache[schema_key] = new_schema
+
             get_schema_start = time.time()
-            schema = GraphQLSchemaGenerator().get_schema(request, draft, before_resolve=before_resolve)
+            schema = GraphQLSchemaGenerator().get_schema(
+                request,
+                draft,
+                before_resolve=before_resolve,
+                on_progress_updated=lambda name, i, total: on_progress_updated(request, new_schema, name, i, total)
+            )
             get_schema_end = time.time()
             get_schema_time = round(get_schema_end - get_schema_start, 3)
 
             with connection_cache(request) as cache:
                 cached_schema = cache.get(schema_key)
 
                 if cached_schema and cached_schema['id'] == new_schema['id']:
-                    new_schema = {**new_schema, 'instance': schema, 'get_schema_time': get_schema_time}
+                    new_schema = {**cached_schema, 'instance': schema, 'get_schema_time': get_schema_time}
                     cache[schema_key] = new_schema
 
-                    logger.info('Saved GraphQL schema "{}"'.format(new_schema['id']))
+                    logger.info('[{}] Saved GraphQL schema "{}" (Mem:{})'.format(
+                        id_short,
+                        new_schema['id'],
+                        get_memory_usage_human())
+                    )
                 else:
-                    logger.info('Ignoring GraphQL schema result "{}", existing: "{}"'.format(
+                    logger.info('[{}] Ignoring GraphQL schema result "{}", existing: "{}"'.format(
+                        id_short,
                         new_schema['id'],
                         cached_schema.get('id') if cached_schema else None
                     ))
 
             return schema
         except Exception as e:
             with connection_cache(request) as cache:
@@ -124,14 +158,16 @@
 
         return self.create_schema(request, schema_key, new_schema, draft)
 
     def get(self, request, *args, **kwargs):
         return self.post(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
+        track_database_async(request)
+
         draft = bool(request.get_argument('draft', False))
         validate = bool(request.data.get('validate', True))
 
         if 'query' not in request.data:
             return JSONResponse({})
 
         try:
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/register.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/register.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/reload.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/reload.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/update.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/update.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/list.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/list.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/create.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/create.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/destroy.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/destroy.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/update.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/update.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/create.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/model.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/update.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/list.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/list.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/model.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/list.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/list.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 76b0 eb63 6c05 0000 e300 0000  3...v..cl.......
+00000000: 330d 0d0a ec82 9964 6c05 0000 e300 0000  3......dl.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 4400 0000 6400 6401 6c00 6d01 5a01  .sD...d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6508 8303 5a09 6407 5300 2908 e900 0000  e...Z.d.S.).....
 00000070: 0029 01da 1474 7261 636b 5f64 6174 6162  .)...track_datab
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/retrieve.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/create.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/create.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/__pycache__/destroy.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/mixins/model.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/mixins/model.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/login.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/login.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/login.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/login.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/__pycache__/complete.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/complete.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/complete.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/external_auth/login.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/external_auth/login.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/message.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/message.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/register.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/register.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/image_resize.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/image_resize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/file_upload.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/file_upload.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/reload.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/reload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/api.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/proxy_request.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/proxy_request.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/register.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/register.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/status.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/status.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-00000000: 330d 0d0a 16c1 f563 4815 0000 e300 0000  3......cH.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 a000 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
-00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
-00000040: 6d04 5a04 6d05 5a05 0100 6400 6404 6c06  m.Z.m.Z...d.d.l.
-00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6406 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6407 6c0c 6d0d 5a0d 0100 6400 6408 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
-00000090: 6d13 5a13 6d14 5a14 0100 6400 6409 6c15  m.Z.m.Z...d.d.l.
-000000a0: 6d16 5a16 0100 6400 640a 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
-000000b0: 0100 4700 640b 640c 8400 640c 6516 8303  ..G.d.d...d.e...
-000000c0: 5a19 6401 5300 290d e900 0000 004e 2901  Z.d.S.)......N).
-000000d0: da0d 636f 6e66 6967 7572 6174 696f 6e29  ..configuration)
-000000e0: 02da 0b63 6f6e 6e65 6374 696f 6e73 da13  ...connections..
-000000f0: 7065 6e64 696e 675f 636f 6e6e 6563 7469  pending_connecti
-00000100: 6f6e 7329 01da 1841 646d 696e 6973 7472  ons)...Administr
-00000110: 6174 6f72 5065 726d 6973 7369 6f6e 7329  atorPermissions)
-00000120: 01da 0c4a 534f 4e52 6573 706f 6e73 6529  ...JSONResponse)
-00000130: 01da 1173 656e 7472 795f 636f 6e74 726f  ...sentry_contro
-00000140: 6c6c 6572 2901 da0f 6973 7375 6263 6c61  ller)...issubcla
-00000150: 7373 5f73 6166 6529 06da 104d 6f64 656c  ss_safe)...Model
-00000160: 4669 6c74 6572 7354 7970 65da 154d 6f64  FiltersType..Mod
-00000170: 656c 4669 6c74 6572 7346 6965 6c64 5479  elFiltersFieldTy
-00000180: 7065 da1c 4d6f 6465 6c46 696c 7465 7273  pe..ModelFilters
-00000190: 5265 6c61 7469 6f6e 7368 6970 5479 7065  RelationshipType
-000001a0: da10 4d6f 6465 6c4c 6f6f 6b75 7073 5479  ..ModelLookupsTy
-000001b0: 7065 da15 4d6f 6465 6c4c 6f6f 6b75 7073  pe..ModelLookups
-000001c0: 4669 656c 6454 7970 65da 1c4d 6f64 656c  FieldType..Model
-000001d0: 4c6f 6f6b 7570 7352 656c 6174 696f 6e73  LookupsRelations
-000001e0: 6869 7054 7970 6529 01da 0b42 6173 6541  hipType)...BaseA
-000001f0: 5049 5669 6577 2901 da07 696e 7370 6563  PIView)...inspec
-00000200: 7463 0000 0000 0000 0000 0000 0000 0200  tc..............
-00000210: 0000 4000 0000 733a 0000 0065 005a 0164  ..@...s:...e.Z.d
-00000220: 005a 0265 0366 015a 0464 0164 0284 005a  .Z.e.f.Z.d.d...Z
-00000230: 0564 0364 0484 005a 0664 0564 0684 005a  .d.d...Z.d.d...Z
-00000240: 0764 0764 0884 005a 0864 0964 0a84 005a  .d.d...Z.d.d...Z
-00000250: 0964 0b53 0029 0cda 0a53 7461 7475 7356  .d.S.)...StatusV
-00000260: 6965 7763 0200 0000 0000 0000 0c00 0000  iewc............
-00000270: 0a00 0000 4300 0000 7312 0100 007c 0173  ....C...s....|.s
-00000280: 0c64 0164 0269 0153 007c 016a 0064 0383  .d.d.i.S.|.j.d..
-00000290: 017d 027c 0290 0172 0674 017c 026a 026a  .}.|...r.t.|.j.j
-000002a0: 0383 0083 017d 0364 047d 0464 047d 0564  .....}.d.}.d.}.d
-000002b0: 047d 0664 047d 0764 047d 0864 047d 097c  .}.d.}.d.}.d.}.|
-000002c0: 016a 0064 0583 017d 0a78 a07c 026a 026a  .j.d...}.x.|.j.j
-000002d0: 0383 0044 005d 927d 0b74 047c 0b64 0683  ...D.].}.t.|.d..
-000002e0: 0273 6871 5874 057c 0b6a 0674 0783 0272  .shqXt.|.j.t...r
-000002f0: 7e7c 0464 0737 007d 0471 5874 057c 0b6a  ~|.d.7.}.qXt.|.j
-00000300: 0674 0883 0272 947c 0564 0737 007d 0571  .t...r.|.d.7.}.q
-00000310: 5874 057c 0b6a 0674 0983 0272 aa7c 0664  Xt.|.j.t...r.|.d
-00000320: 0737 007d 0671 5874 057c 0b6a 0674 0a83  .7.}.qXt.|.j.t..
-00000330: 0272 c07c 0764 0737 007d 0771 5874 057c  .r.|.d.7.}.qXt.|
-00000340: 0b6a 0674 0b83 0272 d67c 0864 0737 007d  .j.t...r.|.d.7.}
-00000350: 0871 5874 057c 0b6a 0674 0c83 0272 587c  .qXt.|.j.t...rX|
-00000360: 0964 0737 007d 0971 5857 0064 087c 037c  .d.7.}.qXW.d.|.|
-00000370: 047c 057c 067c 077c 087c 097c 0a64 099c  .|.|.|.|.|.|.d..
-00000380: 0953 0064 0164 0a69 0153 0064 0053 0029  .S.d.d.i.S.d.S.)
-00000390: 0b4e da06 7374 6174 7573 5a09 6e6f 5f73  .N..statusZ.no_s
-000003a0: 6368 656d 61da 0869 6e73 7461 6e63 6572  chema..instancer
-000003b0: 0100 0000 da0f 6765 745f 7363 6865 6d61  ......get_schema
-000003c0: 5f74 696d 65da 0d67 7261 7068 656e 655f  _time..graphene_
-000003d0: 7479 7065 e901 0000 00da 026f 6b29 0972  type.......ok).r
-000003e0: 1200 0000 da05 7479 7065 73da 0766 696c  ......types..fil
-000003f0: 7465 7273 5a0e 6669 6c74 6572 735f 6669  tersZ.filters_fi
-00000400: 656c 6473 5a15 6669 6c74 6572 735f 7265  eldsZ.filters_re
-00000410: 6c61 7469 6f6e 7368 6970 73da 076c 6f6f  lationships..loo
-00000420: 6b75 7073 5a0e 6c6f 6f6b 7570 735f 6669  kupsZ.lookups_fi
-00000430: 656c 6473 5a15 6c6f 6f6b 7570 735f 7265  eldsZ.lookups_re
-00000440: 6c61 7469 6f6e 7368 6970 7372 1400 0000  lationshipsr....
-00000450: da07 7065 6e64 696e 6729 0dda 0367 6574  ..pending)...get
-00000460: da03 6c65 6eda 095f 7479 7065 5f6d 6170  ..len.._type_map
-00000470: da06 7661 6c75 6573 da07 6861 7361 7474  ..values..hasatt
-00000480: 7272 0800 0000 7215 0000 0072 0900 0000  rr....r....r....
-00000490: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-000004a0: 0d00 0000 720e 0000 0029 0cda 0473 656c  ....r....)...sel
-000004b0: 66da 0673 6368 656d 6172 1300 0000 5a0b  f..schemar....Z.
-000004c0: 7479 7065 735f 636f 756e 745a 0d66 696c  types_countZ.fil
-000004d0: 7465 7273 5f63 6f75 6e74 5a14 6669 6c74  ters_countZ.filt
-000004e0: 6572 735f 6669 656c 6473 5f63 6f75 6e74  ers_fields_count
-000004f0: 5a1b 6669 6c74 6572 735f 7265 6c61 7469  Z.filters_relati
-00000500: 6f6e 7368 6970 735f 636f 756e 745a 0d6c  onships_countZ.l
-00000510: 6f6f 6b75 7073 5f63 6f75 6e74 5a14 6c6f  ookups_countZ.lo
-00000520: 6f6b 7570 735f 6669 656c 6473 5f63 6f75  okups_fields_cou
-00000530: 6e74 5a1b 6c6f 6f6b 7570 735f 7265 6c61  ntZ.lookups_rela
-00000540: 7469 6f6e 7368 6970 735f 636f 756e 7472  tionships_countr
-00000550: 1400 0000 da04 6974 656d a900 7224 0000  ......item..r$..
-00000560: 00fa 632f 5573 6572 732f 6631 6e61 6c2f  ..c/Users/f1nal/
-00000570: 4472 6f70 626f 782f 7079 7468 6f6e 2f6a  Dropbox/python/j
-00000580: 6574 2d62 7269 6467 652f 7372 632f 7061  et-bridge/src/pa
-00000590: 636b 6167 6573 2f6a 6574 5f62 7269 6467  ckages/jet_bridg
-000005a0: 655f 6261 7365 2f6a 6574 5f62 7269 6467  e_base/jet_bridg
-000005b0: 655f 6261 7365 2f76 6965 7773 2f73 7461  e_base/views/sta
-000005c0: 7475 732e 7079 da1d 6d61 705f 636f 6e6e  tus.py..map_conn
-000005d0: 6563 7469 6f6e 5f67 7261 7068 716c 5f73  ection_graphql_s
-000005e0: 6368 656d 6112 0000 0073 4a00 0000 0001  chema....sJ.....
-000005f0: 0401 0802 0a02 0601 0e01 0401 0401 0401  ................
-00000600: 0401 0401 0401 0a02 1001 0a01 0202 0c01  ................
-00000610: 0a01 0c01 0a01 0c01 0a01 0c01 0a01 0c01  ................
-00000620: 0a01 0c01 0c03 0201 0201 0201 0201 0201  ................
-00000630: 0201 0201 0201 0803 7a28 5374 6174 7573  ........z(Status
-00000640: 5669 6577 2e6d 6170 5f63 6f6e 6e65 6374  View.map_connect
-00000650: 696f 6e5f 6772 6170 6871 6c5f 7363 6865  ion_graphql_sche
-00000660: 6d61 6302 0000 0000 0000 0002 0000 0005  mac.............
-00000670: 0000 0043 0000 0073 2e00 0000 7c01 7308  ...C...s....|.s.
-00000680: 6400 5300 7c01 6a00 6401 6a01 7c01 6a02  d.S.|.j.d.j.|.j.
-00000690: 7c01 6a03 8302 6401 6a01 7c01 6a04 7c01  |.j...d.j.|.j.|.
-000006a0: 6a05 8302 6402 9c03 5300 2903 4e7a 057b  j...d...S.).Nz.{
-000006b0: 7d3a 7b7d 2903 da09 6973 5f61 6374 6976  }:{})...is_activ
-000006c0: 65da 0d6c 6f63 616c 5f61 6464 7265 7373  e..local_address
-000006d0: da0e 7265 6d6f 7465 5f61 6464 7265 7373  ..remote_address
-000006e0: 2906 7227 0000 00da 0666 6f72 6d61 74da  ).r'.....format.
-000006f0: 0f6c 6f63 616c 5f62 696e 645f 686f 7374  .local_bind_host
-00000700: da0f 6c6f 6361 6c5f 6269 6e64 5f70 6f72  ..local_bind_por
-00000710: 74da 0873 7368 5f68 6f73 74da 0873 7368  t..ssh_host..ssh
-00000720: 5f70 6f72 7429 0272 2100 0000 da06 7475  _port).r!.....tu
-00000730: 6e6e 656c 7224 0000 0072 2400 0000 7225  nnelr$...r$...r%
-00000740: 0000 00da 0a6d 6170 5f74 756e 6e65 6c41  .....map_tunnelA
-00000750: 0000 0073 0a00 0000 0001 0401 0403 0401  ...s............
-00000760: 0e01 7a15 5374 6174 7573 5669 6577 2e6d  ..z.StatusView.m
-00000770: 6170 5f74 756e 6e65 6c63 0200 0000 0000  ap_tunnelc......
-00000780: 0000 0c00 0000 1100 0000 4300 0000 73f4  ..........C...s.
-00000790: 0000 007c 0164 0119 007d 027c 0164 0219  ...|.d...}.|.d..
-000007a0: 007d 0364 037d 0464 037d 0578 647c 036a  .}.d.}.d.}.xd|.j
-000007b0: 0044 005d 5a7d 0679 2874 017c 0683 017d  .D.]Z}.y(t.|...}
-000007c0: 077c 0474 027c 076a 0383 0137 007d 047c  .|.t.|.j...7.}.|
-000007d0: 0574 027c 076a 0483 0137 007d 0557 0071  .t.|.j...7.}.W.q
-000007e0: 2004 0074 056b 0a72 7801 007d 0801 007a   ..t.k.rx..}...z
-000007f0: 1074 066a 077c 0883 0101 0057 0059 0064  .t.j.|.....W.Y.d
-00000800: 0064 007d 087e 0858 0071 2058 0071 2057  .d.}.~.X.q X.q W
-00000810: 007c 006a 087c 026a 0964 0483 0183 017d  .|.j.|.j.d.....}
-00000820: 097c 006a 087c 026a 0964 0583 0183 017d  .|.j.|.j.d.....}
-00000830: 0a7c 006a 0a7c 016a 0964 0683 0183 017d  .|.j.|.j.d.....}
-00000840: 0b7c 0164 0719 007c 016a 0964 0883 017c  .|.d...|.j.d...|
-00000850: 016a 0964 0983 0174 027c 036a 0083 017c  .j.d...t.|.j...|
-00000860: 047c 057c 097c 0a7c 016a 0964 0a83 017c  .|.|.|.|.j.d...|
-00000870: 016a 0964 0b83 017c 016a 0964 0c83 017c  .j.d...|.j.d...|
-00000880: 0b64 0d9c 0c53 0029 0e4e da05 6361 6368  .d...S.).N..cach
-00000890: 65da 0a4d 6170 7065 6442 6173 6572 0100  e..MappedBaser..
-000008a0: 0000 da0e 6772 6170 6871 6c5f 7363 6865  ....graphql_sche
-000008b0: 6d61 da14 6772 6170 6871 6c5f 7363 6865  ma..graphql_sche
-000008c0: 6d61 5f64 7261 6674 722f 0000 00da 046e  ma_draftr/.....n
-000008d0: 616d 65da 0770 726f 6a65 6374 da05 746f  ame..project..to
-000008e0: 6b65 6eda 0a69 6e69 745f 7374 6172 74da  ken..init_start.
-000008f0: 0c63 6f6e 6e65 6374 5f74 696d 65da 0c72  .connect_time..r
-00000900: 6566 6c65 6374 5f74 696d 6529 0c72 3500  eflect_time).r5.
-00000910: 0000 7236 0000 0072 3700 0000 da06 7461  ..r6...r7.....ta
-00000920: 626c 6573 da07 636f 6c75 6d6e 73da 0d72  bles..columns..r
-00000930: 656c 6174 696f 6e73 6869 7073 7233 0000  elationshipsr3..
-00000940: 0072 3400 0000 7238 0000 0072 3900 0000  .r4...r8...r9...
-00000950: 723a 0000 0072 2f00 0000 290b da07 636c  r:...r/...)...cl
-00000960: 6173 7365 7372 1000 0000 721d 0000 0072  assesr....r....r
-00000970: 3c00 0000 723d 0000 00da 0945 7863 6570  <...r=.....Excep
-00000980: 7469 6f6e 7207 0000 00da 1163 6170 7475  tionr......captu
-00000990: 7265 5f65 7863 6570 7469 6f6e 7226 0000  re_exceptionr&..
-000009a0: 0072 1c00 0000 7230 0000 0029 0c72 2100  .r....r0...).r!.
-000009b0: 0000 da0a 636f 6e6e 6563 7469 6f6e 7231  ....connectionr1
-000009c0: 0000 0072 3200 0000 5a0c 636f 6c75 6d6e  ...r2...Z.column
-000009d0: 5f63 6f75 6e74 5a13 7265 6c61 7469 6f6e  _countZ.relation
-000009e0: 7368 6970 735f 636f 756e 74da 054d 6f64  ships_count..Mod
-000009f0: 656c da06 6d61 7070 6572 da01 6572 3300  el..mapper..er3.
-00000a00: 0000 7234 0000 0072 2f00 0000 7224 0000  ..r4...r/...r$..
-00000a10: 0072 2400 0000 7225 0000 00da 0e6d 6170  .r$...r%.....map
-00000a20: 5f63 6f6e 6e65 6374 696f 6e4b 0000 0073  _connectionK...s
-00000a30: 3400 0000 0001 0801 0801 0401 0402 0c01  4...............
-00000a40: 0201 0801 0e01 1201 1001 2002 1001 1001  .......... .....
-00000a50: 1003 0601 0801 0801 0801 0201 0201 0201  ................
-00000a60: 0201 0801 0801 0801 7a19 5374 6174 7573  ........z.Status
-00000a70: 5669 6577 2e6d 6170 5f63 6f6e 6e65 6374  View.map_connect
-00000a80: 696f 6e63 0200 0000 0000 0000 0300 0000  ionc............
-00000a90: 0800 0000 4300 0000 7346 0000 007c 006a  ....C...sF...|.j
-00000aa0: 007c 016a 0164 0183 0183 017d 027c 0164  .|.j.d.....}.|.d
-00000ab0: 0219 007c 016a 0164 0383 017c 016a 0164  ...|.j.d...|.j.d
-00000ac0: 0483 017c 016a 0164 0583 017c 016a 0164  ...|.j.d...|.j.d
-00000ad0: 0683 017c 016a 0164 0783 017c 0264 089c  ...|.j.d...|.d..
-00000ae0: 0753 0029 094e 722f 0000 0072 3500 0000  .S.).Nr/...r5...
-00000af0: 7236 0000 0072 3700 0000 7238 0000 00da  r6...r7...r8....
-00000b00: 1074 6162 6c65 735f 7072 6f63 6573 7365  .tables_processe
-00000b10: 64da 0c74 6162 6c65 735f 746f 7461 6c29  d..tables_total)
-00000b20: 0772 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
-00000b30: 7238 0000 0072 4600 0000 7247 0000 0072  r8...rF...rG...r
-00000b40: 2f00 0000 2902 7230 0000 0072 1c00 0000  /...).r0...r....
-00000b50: 2903 7221 0000 00da 1270 656e 6469 6e67  ).r!.....pending
-00000b60: 5f63 6f6e 6e65 6374 696f 6e72 2f00 0000  _connectionr/...
-00000b70: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-00000b80: 166d 6170 5f70 656e 6469 6e67 5f63 6f6e  .map_pending_con
-00000b90: 6e65 6374 696f 6e6c 0000 0073 1000 0000  nectionl...s....
-00000ba0: 0001 1003 0601 0801 0801 0801 0801 0801  ................
-00000bb0: 7a21 5374 6174 7573 5669 6577 2e6d 6170  z!StatusView.map
-00000bc0: 5f70 656e 6469 6e67 5f63 6f6e 6e65 6374  _pending_connect
-00000bd0: 696f 6e63 0200 0000 0000 0000 0600 0000  ionc............
-00000be0: 0800 0000 0f00 0000 735e 0000 0074 006a  ........s^...t.j
-00000bf0: 0083 007d 0474 017c 0474 026a 0318 0083  ...}.t.|.t.j....
-00000c00: 017d 0574 0474 0574 066a 0783 0083 0174  .}.t.t.t.j.....t
-00000c10: 0574 086a 0783 0083 0174 0987 0066 0164  .t.j.....t...f.d
-00000c20: 0164 0284 0874 066a 0a83 0083 0274 0987  .d...t.j.....t..
-00000c30: 0066 0164 0364 0284 0874 086a 0a83 0083  .f.d.d...t.j....
-00000c40: 027c 0564 049c 0583 0153 0029 054e 6301  .|.d.....S.).Nc.
-00000c50: 0000 0000 0000 0001 0000 0002 0000 0013  ................
-00000c60: 0000 0073 0a00 0000 8800 6a00 7c00 8301  ...s......j.|...
-00000c70: 5300 2901 4e29 0172 4900 0000 2901 da01  S.).N).rI...)...
-00000c80: 7829 0172 2100 0000 7224 0000 0072 2500  x).r!...r$...r%.
-00000c90: 0000 da08 3c6c 616d 6264 613e 8000 0000  ....<lambda>....
-00000ca0: 7300 0000 007a 2053 7461 7475 7356 6965  s....z StatusVie
-00000cb0: 772e 6765 742e 3c6c 6f63 616c 733e 2e3c  w.get.<locals>.<
-00000cc0: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
-00000cd0: 0100 0000 0200 0000 1300 0000 730a 0000  ............s...
-00000ce0: 0088 006a 007c 0083 0153 0029 014e 2901  ...j.|...S.).N).
-00000cf0: 7245 0000 0029 0172 4a00 0000 2901 7221  rE...).rJ...).r!
-00000d00: 0000 0072 2400 0000 7225 0000 0072 4b00  ...r$...r%...rK.
-00000d10: 0000 8100 0000 7300 0000 0029 055a 1974  ......s....).Z.t
-00000d20: 6f74 616c 5f70 656e 6469 6e67 5f63 6f6e  otal_pending_con
-00000d30: 6e65 6374 696f 6e73 5a11 746f 7461 6c5f  nectionsZ.total_
-00000d40: 636f 6e6e 6563 7469 6f6e 7372 0400 0000  connectionsr....
-00000d50: 7203 0000 00da 0675 7074 696d 6529 0bda  r......uptime)..
-00000d60: 0474 696d 65da 0572 6f75 6e64 7202 0000  .time..roundr...
-00000d70: 00da 0969 6e69 745f 7469 6d65 7206 0000  ...init_timer...
-00000d80: 0072 1d00 0000 7204 0000 00da 046b 6579  .r....r......key
-00000d90: 7372 0300 0000 da03 6d61 7072 1f00 0000  sr......mapr....
-00000da0: 2906 7221 0000 00da 0772 6571 7565 7374  ).r!.....request
-00000db0: da04 6172 6773 da06 6b77 6172 6773 da03  ..args..kwargs..
-00000dc0: 6e6f 7772 4c00 0000 7224 0000 0029 0172  nowrL...r$...).r
-00000dd0: 2100 0000 7225 0000 0072 1c00 0000 7900  !...r%...r....y.
-00000de0: 0000 7310 0000 0000 0108 010e 0202 010a  ..s.............
-00000df0: 010a 0114 0114 017a 0e53 7461 7475 7356  .......z.StatusV
-00000e00: 6965 772e 6765 744e 290a da08 5f5f 6e61  iew.getN)...__na
-00000e10: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000e20: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7205  ..__qualname__r.
-00000e30: 0000 00da 1270 6572 6d69 7373 696f 6e5f  .....permission_
-00000e40: 636c 6173 7365 7372 2600 0000 7230 0000  classesr&...r0..
-00000e50: 0072 4500 0000 7249 0000 0072 1c00 0000  .rE...rI...r....
-00000e60: 7224 0000 0072 2400 0000 7224 0000 0072  r$...r$...r$...r
-00000e70: 2500 0000 7211 0000 000f 0000 0073 0c00  %...r........s..
-00000e80: 0000 0801 0602 082f 080a 0821 080d 7211  ......./...!..r.
-00000e90: 0000 0029 1a72 4d00 0000 da1d 6a65 745f  ...).rM.....jet_
-00000ea0: 6272 6964 6765 5f62 6173 652e 636f 6e66  bridge_base.conf
-00000eb0: 6967 7572 6174 696f 6e72 0200 0000 da12  igurationr......
-00000ec0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00000ed0: 6462 7203 0000 0072 0400 0000 da1b 6a65  dbr....r......je
-00000ee0: 745f 6272 6964 6765 5f62 6173 652e 7065  t_bridge_base.pe
-00000ef0: 726d 6973 7369 6f6e 7372 0500 0000 da1e  rmissionsr......
-00000f00: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-00000f10: 7265 7370 6f6e 7365 732e 6a73 6f6e 7206  responses.jsonr.
-00000f20: 0000 00da 166a 6574 5f62 7269 6467 655f  .....jet_bridge_
-00000f30: 6261 7365 2e73 656e 7472 7972 0700 0000  base.sentryr....
-00000f40: da1d 6a65 745f 6272 6964 6765 5f62 6173  ..jet_bridge_bas
-00000f50: 652e 7574 696c 732e 636c 6173 7365 7372  e.utils.classesr
-00000f60: 0800 0000 da1d 6a65 745f 6272 6964 6765  ......jet_bridge
-00000f70: 5f62 6173 652e 7574 696c 732e 6772 6170  _base.utils.grap
-00000f80: 6871 6c72 0900 0000 720a 0000 0072 0b00  hqlr....r....r..
-00000f90: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000fa0: 00da 1e6a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
-00000fb0: 7365 2e76 6965 7773 2e62 6173 652e 6170  se.views.base.ap
-00000fc0: 6972 0f00 0000 da0a 7371 6c61 6c63 6865  ir......sqlalche
-00000fd0: 6d79 7210 0000 0072 1100 0000 7224 0000  myr....r....r$..
-00000fe0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00000ff0: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
-00001000: 0000 0008 020c 0110 010c 010c 010c 010c  ................
-00001010: 0120 020c 010c 03                        . .....
+00000000: 420d 0d0a 0000 0000 16c1 f563 4815 0000  B..........cH...
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 a000 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 5a00 6400 6402 6c01 6d02 5a02 0100 6400  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6408 6c0e 6d0f 5a0f 6d10 5a10 6d11 5a11  d.l.m.Z.m.Z.m.Z.
+00000090: 6d12 5a12 6d13 5a13 6d14 5a14 0100 6400  m.Z.m.Z.m.Z...d.
+000000a0: 6409 6c15 6d16 5a16 0100 6400 640a 6c17  d.l.m.Z...d.d.l.
+000000b0: 6d18 5a18 0100 4700 640b 640c 8400 640c  m.Z...G.d.d...d.
+000000c0: 6516 8303 5a19 6401 5300 290d e900 0000  e...Z.d.S.).....
+000000d0: 004e 2901 da0d 636f 6e66 6967 7572 6174  .N)...configurat
+000000e0: 696f 6e29 02da 0b63 6f6e 6e65 6374 696f  ion)...connectio
+000000f0: 6e73 da13 7065 6e64 696e 675f 636f 6e6e  ns..pending_conn
+00000100: 6563 7469 6f6e 7329 01da 1841 646d 696e  ections)...Admin
+00000110: 6973 7472 6174 6f72 5065 726d 6973 7369  istratorPermissi
+00000120: 6f6e 7329 01da 0c4a 534f 4e52 6573 706f  ons)...JSONRespo
+00000130: 6e73 6529 01da 1173 656e 7472 795f 636f  nse)...sentry_co
+00000140: 6e74 726f 6c6c 6572 2901 da0f 6973 7375  ntroller)...issu
+00000150: 6263 6c61 7373 5f73 6166 6529 06da 104d  bclass_safe)...M
+00000160: 6f64 656c 4669 6c74 6572 7354 7970 65da  odelFiltersType.
+00000170: 154d 6f64 656c 4669 6c74 6572 7346 6965  .ModelFiltersFie
+00000180: 6c64 5479 7065 da1c 4d6f 6465 6c46 696c  ldType..ModelFil
+00000190: 7465 7273 5265 6c61 7469 6f6e 7368 6970  tersRelationship
+000001a0: 5479 7065 da10 4d6f 6465 6c4c 6f6f 6b75  Type..ModelLooku
+000001b0: 7073 5479 7065 da15 4d6f 6465 6c4c 6f6f  psType..ModelLoo
+000001c0: 6b75 7073 4669 656c 6454 7970 65da 1c4d  kupsFieldType..M
+000001d0: 6f64 656c 4c6f 6f6b 7570 7352 656c 6174  odelLookupsRelat
+000001e0: 696f 6e73 6869 7054 7970 6529 01da 0b42  ionshipType)...B
+000001f0: 6173 6541 5049 5669 6577 2901 da07 696e  aseAPIView)...in
+00000200: 7370 6563 7463 0000 0000 0000 0000 0000  spectc..........
+00000210: 0000 0200 0000 4000 0000 733a 0000 0065  ......@...s:...e
+00000220: 005a 0164 005a 0265 0366 015a 0464 0164  .Z.d.Z.e.f.Z.d.d
+00000230: 0284 005a 0564 0364 0484 005a 0664 0564  ...Z.d.d...Z.d.d
+00000240: 0684 005a 0764 0764 0884 005a 0864 0964  ...Z.d.d...Z.d.d
+00000250: 0a84 005a 0964 0b53 0029 0cda 0a53 7461  ...Z.d.S.)...Sta
+00000260: 7475 7356 6965 7763 0200 0000 0000 0000  tusViewc........
+00000270: 0c00 0000 0a00 0000 4300 0000 7312 0100  ........C...s...
+00000280: 007c 0173 0c64 0164 0269 0153 007c 01a0  .|.s.d.d.i.S.|..
+00000290: 0064 03a1 017d 027c 0290 0172 0674 017c  .d...}.|...r.t.|
+000002a0: 026a 02a0 03a1 0083 017d 0364 047d 0464  .j.......}.d.}.d
+000002b0: 047d 0564 047d 0664 047d 0764 047d 0864  .}.d.}.d.}.d.}.d
+000002c0: 047d 097c 01a0 0064 05a1 017d 0a78 a07c  .}.|...d...}.x.|
+000002d0: 026a 02a0 03a1 0044 005d 927d 0b74 047c  .j.....D.].}.t.|
+000002e0: 0b64 0683 0273 6871 5874 057c 0b6a 0674  .d...shqXt.|.j.t
+000002f0: 0783 0272 7e7c 0464 0737 007d 0471 5874  ...r~|.d.7.}.qXt
+00000300: 057c 0b6a 0674 0883 0272 947c 0564 0737  .|.j.t...r.|.d.7
+00000310: 007d 0571 5874 057c 0b6a 0674 0983 0272  .}.qXt.|.j.t...r
+00000320: aa7c 0664 0737 007d 0671 5874 057c 0b6a  .|.d.7.}.qXt.|.j
+00000330: 0674 0a83 0272 c07c 0764 0737 007d 0771  .t...r.|.d.7.}.q
+00000340: 5874 057c 0b6a 0674 0b83 0272 d67c 0864  Xt.|.j.t...r.|.d
+00000350: 0737 007d 0871 5874 057c 0b6a 0674 0c83  .7.}.qXt.|.j.t..
+00000360: 0272 587c 0964 0737 007d 0971 5857 0064  .rX|.d.7.}.qXW.d
+00000370: 087c 037c 047c 057c 067c 077c 087c 097c  .|.|.|.|.|.|.|.|
+00000380: 0a64 099c 0953 0064 0164 0a69 0153 0064  .d...S.d.d.i.S.d
+00000390: 0053 0029 0b4e da06 7374 6174 7573 5a09  .S.).N..statusZ.
+000003a0: 6e6f 5f73 6368 656d 61da 0869 6e73 7461  no_schema..insta
+000003b0: 6e63 6572 0100 0000 da0f 6765 745f 7363  ncer......get_sc
+000003c0: 6865 6d61 5f74 696d 65da 0d67 7261 7068  hema_time..graph
+000003d0: 656e 655f 7479 7065 e901 0000 00da 026f  ene_type.......o
+000003e0: 6b29 0972 1200 0000 da05 7479 7065 73da  k).r......types.
+000003f0: 0766 696c 7465 7273 5a0e 6669 6c74 6572  .filtersZ.filter
+00000400: 735f 6669 656c 6473 5a15 6669 6c74 6572  s_fieldsZ.filter
+00000410: 735f 7265 6c61 7469 6f6e 7368 6970 73da  s_relationships.
+00000420: 076c 6f6f 6b75 7073 5a0e 6c6f 6f6b 7570  .lookupsZ.lookup
+00000430: 735f 6669 656c 6473 5a15 6c6f 6f6b 7570  s_fieldsZ.lookup
+00000440: 735f 7265 6c61 7469 6f6e 7368 6970 7372  s_relationshipsr
+00000450: 1400 0000 da07 7065 6e64 696e 6729 0dda  ......pending)..
+00000460: 0367 6574 da03 6c65 6eda 095f 7479 7065  .get..len.._type
+00000470: 5f6d 6170 da06 7661 6c75 6573 da07 6861  _map..values..ha
+00000480: 7361 7474 7272 0800 0000 7215 0000 0072  sattrr....r....r
+00000490: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
+000004a0: 0000 0072 0d00 0000 720e 0000 0029 0cda  ...r....r....)..
+000004b0: 0473 656c 66da 0673 6368 656d 6172 1300  .self..schemar..
+000004c0: 0000 5a0b 7479 7065 735f 636f 756e 745a  ..Z.types_countZ
+000004d0: 0d66 696c 7465 7273 5f63 6f75 6e74 5a14  .filters_countZ.
+000004e0: 6669 6c74 6572 735f 6669 656c 6473 5f63  filters_fields_c
+000004f0: 6f75 6e74 5a1b 6669 6c74 6572 735f 7265  ountZ.filters_re
+00000500: 6c61 7469 6f6e 7368 6970 735f 636f 756e  lationships_coun
+00000510: 745a 0d6c 6f6f 6b75 7073 5f63 6f75 6e74  tZ.lookups_count
+00000520: 5a14 6c6f 6f6b 7570 735f 6669 656c 6473  Z.lookups_fields
+00000530: 5f63 6f75 6e74 5a1b 6c6f 6f6b 7570 735f  _countZ.lookups_
+00000540: 7265 6c61 7469 6f6e 7368 6970 735f 636f  relationships_co
+00000550: 756e 7472 1400 0000 da04 6974 656d a900  untr......item..
+00000560: 7224 0000 00fa 632f 5573 6572 732f 6631  r$....c/Users/f1
+00000570: 6e61 6c2f 4472 6f70 626f 782f 7079 7468  nal/Dropbox/pyth
+00000580: 6f6e 2f6a 6574 2d62 7269 6467 652f 7372  on/jet-bridge/sr
+00000590: 632f 7061 636b 6167 6573 2f6a 6574 5f62  c/packages/jet_b
+000005a0: 7269 6467 655f 6261 7365 2f6a 6574 5f62  ridge_base/jet_b
+000005b0: 7269 6467 655f 6261 7365 2f76 6965 7773  ridge_base/views
+000005c0: 2f73 7461 7475 732e 7079 da1d 6d61 705f  /status.py..map_
+000005d0: 636f 6e6e 6563 7469 6f6e 5f67 7261 7068  connection_graph
+000005e0: 716c 5f73 6368 656d 6112 0000 0073 4a00  ql_schema....sJ.
+000005f0: 0000 0001 0401 0802 0a02 0601 0e01 0401  ................
+00000600: 0401 0401 0401 0401 0401 0a02 1001 0a01  ................
+00000610: 0202 0c01 0a01 0c01 0a01 0c01 0a01 0c01  ................
+00000620: 0a01 0c01 0a01 0c01 0c03 0201 0201 0201  ................
+00000630: 0201 0201 0201 0201 0201 0803 7a28 5374  ............z(St
+00000640: 6174 7573 5669 6577 2e6d 6170 5f63 6f6e  atusView.map_con
+00000650: 6e65 6374 696f 6e5f 6772 6170 6871 6c5f  nection_graphql_
+00000660: 7363 6865 6d61 6302 0000 0000 0000 0002  schemac.........
+00000670: 0000 0006 0000 0043 0000 0073 2e00 0000  .......C...s....
+00000680: 7c01 7308 6400 5300 7c01 6a00 6401 a001  |.s.d.S.|.j.d...
+00000690: 7c01 6a02 7c01 6a03 a102 6401 a001 7c01  |.j.|.j...d...|.
+000006a0: 6a04 7c01 6a05 a102 6402 9c03 5300 2903  j.|.j...d...S.).
+000006b0: 4e7a 057b 7d3a 7b7d 2903 da09 6973 5f61  Nz.{}:{})...is_a
+000006c0: 6374 6976 65da 0d6c 6f63 616c 5f61 6464  ctive..local_add
+000006d0: 7265 7373 da0e 7265 6d6f 7465 5f61 6464  ress..remote_add
+000006e0: 7265 7373 2906 7227 0000 00da 0666 6f72  ress).r'.....for
+000006f0: 6d61 74da 0f6c 6f63 616c 5f62 696e 645f  mat..local_bind_
+00000700: 686f 7374 da0f 6c6f 6361 6c5f 6269 6e64  host..local_bind
+00000710: 5f70 6f72 74da 0873 7368 5f68 6f73 74da  _port..ssh_host.
+00000720: 0873 7368 5f70 6f72 7429 0272 2100 0000  .ssh_port).r!...
+00000730: da06 7475 6e6e 656c 7224 0000 0072 2400  ..tunnelr$...r$.
+00000740: 0000 7225 0000 00da 0a6d 6170 5f74 756e  ..r%.....map_tun
+00000750: 6e65 6c41 0000 0073 0a00 0000 0001 0401  nelA...s........
+00000760: 0403 0401 0e01 7a15 5374 6174 7573 5669  ......z.StatusVi
+00000770: 6577 2e6d 6170 5f74 756e 6e65 6c63 0200  ew.map_tunnelc..
+00000780: 0000 0000 0000 0c00 0000 0d00 0000 4300  ..............C.
+00000790: 0000 73f4 0000 007c 0164 0119 007d 027c  ..s....|.d...}.|
+000007a0: 0164 0219 007d 0364 037d 0464 037d 0578  .d...}.d.}.d.}.x
+000007b0: 647c 036a 0044 005d 5a7d 0679 2874 017c  d|.j.D.]Z}.y(t.|
+000007c0: 0683 017d 077c 0474 027c 076a 0383 0137  ...}.|.t.|.j...7
+000007d0: 007d 047c 0574 027c 076a 0483 0137 007d  .}.|.t.|.j...7.}
+000007e0: 0557 0071 2004 0074 056b 0a72 7801 007d  .W.q ..t.k.rx..}
+000007f0: 0801 007a 0e74 06a0 077c 08a1 0101 0057  ...z.t...|.....W
+00000800: 0064 0064 007d 087e 0858 0059 0071 2058  .d.d.}.~.X.Y.q X
+00000810: 0071 2057 007c 00a0 087c 02a0 0964 04a1  .q W.|...|...d..
+00000820: 01a1 017d 097c 00a0 087c 02a0 0964 05a1  ...}.|...|...d..
+00000830: 01a1 017d 0a7c 00a0 0a7c 01a0 0964 06a1  ...}.|...|...d..
+00000840: 01a1 017d 0b7c 0164 0719 007c 01a0 0964  ...}.|.d...|...d
+00000850: 08a1 017c 01a0 0964 09a1 0174 027c 036a  ...|...d...t.|.j
+00000860: 0083 017c 047c 057c 097c 0a7c 01a0 0964  ...|.|.|.|.|...d
+00000870: 0aa1 017c 01a0 0964 0ba1 017c 01a0 0964  ...|...d...|...d
+00000880: 0ca1 017c 0b64 0d9c 0c53 0029 0e4e da05  ...|.d...S.).N..
+00000890: 6361 6368 65da 0a4d 6170 7065 6442 6173  cache..MappedBas
+000008a0: 6572 0100 0000 da0e 6772 6170 6871 6c5f  er......graphql_
+000008b0: 7363 6865 6d61 da14 6772 6170 6871 6c5f  schema..graphql_
+000008c0: 7363 6865 6d61 5f64 7261 6674 722f 0000  schema_draftr/..
+000008d0: 00da 046e 616d 65da 0770 726f 6a65 6374  ...name..project
+000008e0: da05 746f 6b65 6eda 0a69 6e69 745f 7374  ..token..init_st
+000008f0: 6172 74da 0c63 6f6e 6e65 6374 5f74 696d  art..connect_tim
+00000900: 65da 0c72 6566 6c65 6374 5f74 696d 6529  e..reflect_time)
+00000910: 0c72 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
+00000920: da06 7461 626c 6573 da07 636f 6c75 6d6e  ..tables..column
+00000930: 73da 0d72 656c 6174 696f 6e73 6869 7073  s..relationships
+00000940: 7233 0000 0072 3400 0000 7238 0000 0072  r3...r4...r8...r
+00000950: 3900 0000 723a 0000 0072 2f00 0000 290b  9...r:...r/...).
+00000960: da07 636c 6173 7365 7372 1000 0000 721d  ..classesr....r.
+00000970: 0000 0072 3c00 0000 723d 0000 00da 0945  ...r<...r=.....E
+00000980: 7863 6570 7469 6f6e 7207 0000 00da 1163  xceptionr......c
+00000990: 6170 7475 7265 5f65 7863 6570 7469 6f6e  apture_exception
+000009a0: 7226 0000 0072 1c00 0000 7230 0000 0029  r&...r....r0...)
+000009b0: 0c72 2100 0000 da0a 636f 6e6e 6563 7469  .r!.....connecti
+000009c0: 6f6e 7231 0000 0072 3200 0000 5a0c 636f  onr1...r2...Z.co
+000009d0: 6c75 6d6e 5f63 6f75 6e74 5a13 7265 6c61  lumn_countZ.rela
+000009e0: 7469 6f6e 7368 6970 735f 636f 756e 74da  tionships_count.
+000009f0: 054d 6f64 656c da06 6d61 7070 6572 da01  .Model..mapper..
+00000a00: 6572 3300 0000 7234 0000 0072 2f00 0000  er3...r4...r/...
+00000a10: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00000a20: 0e6d 6170 5f63 6f6e 6e65 6374 696f 6e4b  .map_connectionK
+00000a30: 0000 0073 3400 0000 0001 0801 0801 0401  ...s4...........
+00000a40: 0402 0c01 0201 0801 0e01 1201 1001 2002  .............. .
+00000a50: 1001 1001 1003 0601 0801 0801 0801 0201  ................
+00000a60: 0201 0201 0201 0801 0801 0801 7a19 5374  ............z.St
+00000a70: 6174 7573 5669 6577 2e6d 6170 5f63 6f6e  atusView.map_con
+00000a80: 6e65 6374 696f 6e63 0200 0000 0000 0000  nectionc........
+00000a90: 0300 0000 0800 0000 4300 0000 7346 0000  ........C...sF..
+00000aa0: 007c 00a0 007c 01a0 0164 01a1 01a1 017d  .|...|...d.....}
+00000ab0: 027c 0164 0219 007c 01a0 0164 03a1 017c  .|.d...|...d...|
+00000ac0: 01a0 0164 04a1 017c 01a0 0164 05a1 017c  ...d...|...d...|
+00000ad0: 01a0 0164 06a1 017c 01a0 0164 07a1 017c  ...d...|...d...|
+00000ae0: 0264 089c 0753 0029 094e 722f 0000 0072  .d...S.).Nr/...r
+00000af0: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
+00000b00: 0000 00da 1074 6162 6c65 735f 7072 6f63  .....tables_proc
+00000b10: 6573 7365 64da 0c74 6162 6c65 735f 746f  essed..tables_to
+00000b20: 7461 6c29 0772 3500 0000 7236 0000 0072  tal).r5...r6...r
+00000b30: 3700 0000 7238 0000 0072 4600 0000 7247  7...r8...rF...rG
+00000b40: 0000 0072 2f00 0000 2902 7230 0000 0072  ...r/...).r0...r
+00000b50: 1c00 0000 2903 7221 0000 00da 1270 656e  ....).r!.....pen
+00000b60: 6469 6e67 5f63 6f6e 6e65 6374 696f 6e72  ding_connectionr
+00000b70: 2f00 0000 7224 0000 0072 2400 0000 7225  /...r$...r$...r%
+00000b80: 0000 00da 166d 6170 5f70 656e 6469 6e67  .....map_pending
+00000b90: 5f63 6f6e 6e65 6374 696f 6e6c 0000 0073  _connectionl...s
+00000ba0: 1000 0000 0001 1003 0601 0801 0801 0801  ................
+00000bb0: 0801 0801 7a21 5374 6174 7573 5669 6577  ....z!StatusView
+00000bc0: 2e6d 6170 5f70 656e 6469 6e67 5f63 6f6e  .map_pending_con
+00000bd0: 6e65 6374 696f 6e63 0200 0000 0000 0000  nectionc........
+00000be0: 0600 0000 0800 0000 0f00 0000 735e 0000  ............s^..
+00000bf0: 0074 00a0 00a1 007d 0474 017c 0474 026a  .t.....}.t.|.t.j
+00000c00: 0318 0083 017d 0574 0474 0574 06a0 07a1  .....}.t.t.t....
+00000c10: 0083 0174 0574 08a0 07a1 0083 0174 0987  ...t.t.......t..
+00000c20: 0066 0164 0164 0284 0874 06a0 0aa1 0083  .f.d.d...t......
+00000c30: 0274 0987 0066 0164 0364 0284 0874 08a0  .t...f.d.d...t..
+00000c40: 0aa1 0083 027c 0564 049c 0583 0153 0029  .....|.d.....S.)
+00000c50: 054e 6301 0000 0000 0000 0001 0000 0003  .Nc.............
+00000c60: 0000 0013 0000 0073 0a00 0000 8800 a000  .......s........
+00000c70: 7c00 a101 5300 2901 4e29 0172 4900 0000  |...S.).N).rI...
+00000c80: 2901 da01 7829 0172 2100 0000 7224 0000  )...x).r!...r$..
+00000c90: 0072 2500 0000 da08 3c6c 616d 6264 613e  .r%.....<lambda>
+00000ca0: 8000 0000 f300 0000 007a 2053 7461 7475  .........z Statu
+00000cb0: 7356 6965 772e 6765 742e 3c6c 6f63 616c  sView.get.<local
+00000cc0: 733e 2e3c 6c61 6d62 6461 3e63 0100 0000  s>.<lambda>c....
+00000cd0: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00000ce0: 730a 0000 0088 00a0 007c 00a1 0153 0029  s........|...S.)
+00000cf0: 014e 2901 7245 0000 0029 0172 4a00 0000  .N).rE...).rJ...
+00000d00: 2901 7221 0000 0072 2400 0000 7225 0000  ).r!...r$...r%..
+00000d10: 0072 4b00 0000 8100 0000 724c 0000 0029  .rK.......rL...)
+00000d20: 055a 1974 6f74 616c 5f70 656e 6469 6e67  .Z.total_pending
+00000d30: 5f63 6f6e 6e65 6374 696f 6e73 5a11 746f  _connectionsZ.to
+00000d40: 7461 6c5f 636f 6e6e 6563 7469 6f6e 7372  tal_connectionsr
+00000d50: 0400 0000 7203 0000 00da 0675 7074 696d  ....r......uptim
+00000d60: 6529 0bda 0474 696d 65da 0572 6f75 6e64  e)...time..round
+00000d70: 7202 0000 00da 0969 6e69 745f 7469 6d65  r......init_time
+00000d80: 7206 0000 0072 1d00 0000 7204 0000 00da  r....r....r.....
+00000d90: 046b 6579 7372 0300 0000 da03 6d61 7072  .keysr......mapr
+00000da0: 1f00 0000 2906 7221 0000 00da 0772 6571  ....).r!.....req
+00000db0: 7565 7374 da04 6172 6773 da06 6b77 6172  uest..args..kwar
+00000dc0: 6773 da03 6e6f 7772 4d00 0000 7224 0000  gs..nowrM...r$..
+00000dd0: 0029 0172 2100 0000 7225 0000 0072 1c00  .).r!...r%...r..
+00000de0: 0000 7900 0000 7310 0000 0000 0108 010e  ..y...s.........
+00000df0: 0202 010a 010a 0114 0114 017a 0e53 7461  ...........z.Sta
+00000e00: 7475 7356 6965 772e 6765 744e 290a da08  tusView.getN)...
+00000e10: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000e20: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000e30: 5f5f 7205 0000 00da 1270 6572 6d69 7373  __r......permiss
+00000e40: 696f 6e5f 636c 6173 7365 7372 2600 0000  ion_classesr&...
+00000e50: 7230 0000 0072 4500 0000 7249 0000 0072  r0...rE...rI...r
+00000e60: 1c00 0000 7224 0000 0072 2400 0000 7224  ....r$...r$...r$
+00000e70: 0000 0072 2500 0000 7211 0000 000f 0000  ...r%...r.......
+00000e80: 0073 0c00 0000 0801 0602 082f 080a 0821  .s........./...!
+00000e90: 080d 7211 0000 0029 1a72 4e00 0000 da1d  ..r....).rN.....
+00000ea0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+00000eb0: 636f 6e66 6967 7572 6174 696f 6e72 0200  configurationr..
+00000ec0: 0000 da12 6a65 745f 6272 6964 6765 5f62  ....jet_bridge_b
+00000ed0: 6173 652e 6462 7203 0000 0072 0400 0000  ase.dbr....r....
+00000ee0: da1b 6a65 745f 6272 6964 6765 5f62 6173  ..jet_bridge_bas
+00000ef0: 652e 7065 726d 6973 7369 6f6e 7372 0500  e.permissionsr..
+00000f00: 0000 da1e 6a65 745f 6272 6964 6765 5f62  ....jet_bridge_b
+00000f10: 6173 652e 7265 7370 6f6e 7365 732e 6a73  ase.responses.js
+00000f20: 6f6e 7206 0000 00da 166a 6574 5f62 7269  onr......jet_bri
+00000f30: 6467 655f 6261 7365 2e73 656e 7472 7972  dge_base.sentryr
+00000f40: 0700 0000 da1d 6a65 745f 6272 6964 6765  ......jet_bridge
+00000f50: 5f62 6173 652e 7574 696c 732e 636c 6173  _base.utils.clas
+00000f60: 7365 7372 0800 0000 da1d 6a65 745f 6272  sesr......jet_br
+00000f70: 6964 6765 5f62 6173 652e 7574 696c 732e  idge_base.utils.
+00000f80: 6772 6170 6871 6c72 0900 0000 720a 0000  graphqlr....r...
+00000f90: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000fa0: 720e 0000 00da 1e6a 6574 5f62 7269 6467  r......jet_bridg
+00000fb0: 655f 6261 7365 2e76 6965 7773 2e62 6173  e_base.views.bas
+00000fc0: 652e 6170 6972 0f00 0000 da0a 7371 6c61  e.apir......sqla
+00000fd0: 6c63 6865 6d79 7210 0000 0072 1100 0000  lchemyr....r....
+00000fe0: 7224 0000 0072 2400 0000 7224 0000 0072  r$...r$...r$...r
+00000ff0: 2500 0000 da08 3c6d 6f64 756c 653e 0100  %.....<module>..
+00001000: 0000 7314 0000 0008 020c 0110 010c 010c  ..s.............
+00001010: 010c 010c 0120 020c 010c 03              ..... .....
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a aeae 0a64 d223 0000 e300 0000  3......d.#......
+00000000: 330d 0d0a ab6f c364 d223 0000 e300 0000  3....o.d.#......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 1401 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6406 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 0100 6400 6408 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/graphql.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/graphql.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,315 +1,321 @@
-00000000: 330d 0d0a 41b1 0164 3718 0000 e300 0000  3...A..d7.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 9c00 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6408 6c0e 6d0f 5a0f 0100 6400 6409 6c10  d.l.m.Z...d.d.l.
-00000090: 6d11 5a11 0100 6400 640a 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 640b 6c14 6d15 5a15 0100 4700  ..d.d.l.m.Z...G.
-000000b0: 640c 640d 8400 640d 6515 8303 5a16 6401  d.d...d.e...Z.d.
-000000c0: 5300 290e e900 0000 004e 2901 da09 7469  S.)......N)...ti
-000000d0: 6d65 6465 6c74 6129 01da 0c47 7261 7068  medelta)...Graph
-000000e0: 514c 4572 726f 7229 01da 1063 6f6e 6e65  QLError)...conne
-000000f0: 6374 696f 6e5f 6361 6368 6529 01da 1050  ction_cache)...P
-00000100: 6572 6d69 7373 696f 6e44 656e 6965 6429  ermissionDenied)
-00000110: 01da 066c 6f67 6765 7229 01da 1548 6173  ...logger)...Has
-00000120: 5072 6f6a 6563 7450 6572 6d69 7373 696f  ProjectPermissio
-00000130: 6e73 2901 da0c 4a53 4f4e 5265 7370 6f6e  ns)...JSONRespon
-00000140: 7365 2901 da11 6765 745f 7261 6e64 6f6d  se)...get_random
-00000150: 5f73 7472 696e 6729 01da 1647 7261 7068  _string)...Graph
-00000160: 514c 5363 6865 6d61 4765 6e65 7261 746f  QLSchemaGenerato
-00000170: 7229 01da 0741 5049 5669 6577 6300 0000  r)...APIViewc...
-00000180: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00000190: 0073 5a00 0000 6500 5a01 6400 5a02 6503  .sZ...e.Z.d.Z.e.
-000001a0: 6601 5a04 6401 6402 8400 5a05 6403 6404  f.Z.d.d...Z.d.d.
-000001b0: 8400 5a06 6405 6406 8400 5a07 6407 6408  ..Z.d.d...Z.d.d.
-000001c0: 8400 5a08 6409 640a 8400 5a09 640b 640c  ..Z.d.d...Z.d.d.
-000001d0: 8400 5a0a 640d 640e 8400 5a0b 640f 6410  ..Z.d.d...Z.d.d.
-000001e0: 8400 5a0c 6411 6412 8400 5a0d 6413 5300  ..Z.d.d...Z.d.S.
-000001f0: 2914 da0b 4772 6170 6851 4c56 6965 7763  )...GraphQLViewc
-00000200: 0200 0000 0000 0000 0200 0000 0100 0000  ................
-00000210: 4300 0000 7304 0000 0064 0053 0029 014e  C...s....d.S.).N
-00000220: a900 2902 da04 7365 6c66 da07 7265 7175  ..)...self..requ
-00000230: 6573 7472 0d00 0000 720d 0000 00fa 642f  estr....r.....d/
-00000240: 5573 6572 732f 6631 6e61 6c2f 4472 6f70  Users/f1nal/Drop
-00000250: 626f 782f 7079 7468 6f6e 2f6a 6574 2d62  box/python/jet-b
-00000260: 7269 6467 652f 7372 632f 7061 636b 6167  ridge/src/packag
-00000270: 6573 2f6a 6574 5f62 7269 6467 655f 6261  es/jet_bridge_ba
-00000280: 7365 2f6a 6574 5f62 7269 6467 655f 6261  se/jet_bridge_ba
-00000290: 7365 2f76 6965 7773 2f67 7261 7068 716c  se/views/graphql
-000002a0: 2e70 79da 2162 6566 6f72 655f 6469 7370  .py.!before_disp
-000002b0: 6174 6368 5f70 6572 6d69 7373 696f 6e73  atch_permissions
-000002c0: 5f63 6865 636b 1400 0000 7302 0000 0000  _check....s.....
-000002d0: 017a 2d47 7261 7068 514c 5669 6577 2e62  .z-GraphQLView.b
-000002e0: 6566 6f72 655f 6469 7370 6174 6368 5f70  efore_dispatch_p
-000002f0: 6572 6d69 7373 696f 6e73 5f63 6865 636b  ermissions_check
-00000300: 6302 0000 0000 0000 0002 0000 0004 0000  c...............
-00000310: 0043 0000 0073 1400 0000 6401 7c01 6a00  .C...s....d.|.j.
-00000320: 6a01 6401 8301 6402 6403 9c03 5300 2904  j.d...d.d...S.).
-00000330: 4eda 056d 6f64 656c da01 7229 03da 0f70  N..model..r)...p
-00000340: 6572 6d69 7373 696f 6e5f 7479 7065 da11  ermission_type..
-00000350: 7065 726d 6973 7369 6f6e 5f6f 626a 6563  permission_objec
-00000360: 74da 1270 6572 6d69 7373 696f 6e5f 6163  t..permission_ac
-00000370: 7469 6f6e 7329 02da 0763 6f6e 7465 7874  tions)...context
-00000380: da03 6765 7429 0272 0e00 0000 720f 0000  ..get).r....r...
-00000390: 0072 0d00 0000 720d 0000 0072 1000 0000  .r....r....r....
-000003a0: da1b 7265 7175 6972 6564 5f70 726f 6a65  ..required_proje
-000003b0: 6374 5f70 6572 6d69 7373 696f 6e17 0000  ct_permission...
-000003c0: 0073 0600 0000 0002 0201 0a01 7a27 4772  .s..........z'Gr
-000003d0: 6170 6851 4c56 6965 772e 7265 7175 6972  aphQLView.requir
-000003e0: 6564 5f70 726f 6a65 6374 5f70 6572 6d69  ed_project_permi
-000003f0: 7373 696f 6e63 0200 0000 0000 0000 0200  ssionc..........
-00000400: 0000 0300 0000 4300 0000 731c 0000 0074  ......C...s....t
-00000410: 007c 0174 0183 0272 107c 016a 0253 0074  .|.t...r.|.j.S.t
-00000420: 037c 0183 0153 0064 0053 0029 014e 2904  .|...S.d.S.).N).
-00000430: da0a 6973 696e 7374 616e 6365 7203 0000  ..isinstancer...
-00000440: 00da 076d 6573 7361 6765 da03 7374 7229  ...message..str)
-00000450: 0272 0e00 0000 da05 6572 726f 7272 0d00  .r......errorr..
-00000460: 0000 720d 0000 0072 1000 0000 da0d 6d61  ..r....r......ma
-00000470: 705f 6771 6c5f 6572 726f 721e 0000 0073  p_gql_error....s
-00000480: 0600 0000 0001 0a01 0602 7a19 4772 6170  ..........z.Grap
-00000490: 6851 4c56 6965 772e 6d61 705f 6771 6c5f  hQLView.map_gql_
-000004a0: 6572 726f 7263 0400 0000 0000 0000 0800  errorc..........
-000004b0: 0000 1200 0000 4300 0000 73ac 0000 007c  ......C...s....|
-000004c0: 0373 0864 0053 0074 006a 0164 016a 027c  .s.d.S.t.j.d.j.|
-000004d0: 0364 0219 0083 0183 0101 007c 0364 0319  .d.........|.d..
-000004e0: 007d 047c 048f 2001 0074 0364 0464 058d  .}.|.. ..t.d.d..
-000004f0: 016a 0483 007d 057c 046a 057c 0564 068d  .j...}.|.j.|.d..
-00000500: 0101 0057 0064 0051 0052 0058 0074 067c  ...W.d.Q.R.X.t.|
-00000510: 0183 018f 4c7d 067c 066a 077c 0283 017d  ....L}.|.j.|...}
-00000520: 077c 0772 8a7c 0764 0719 0072 8a74 006a  .|.r.|.d...r.t.j
-00000530: 0164 086a 027c 0364 0219 0083 0183 0101  .d.j.|.d........
-00000540: 007c 0764 0719 0053 0074 006a 0164 096a  .|.d...S.t.j.d.j
-00000550: 027c 0364 0219 0083 0183 0101 0057 0064  .|.d.........W.d
-00000560: 0051 0052 0058 0064 0053 0029 0a4e 7a1e  .Q.R.X.d.S.).Nz.
-00000570: 5761 6974 696e 6720 4772 6170 6851 4c20  Waiting GraphQL 
-00000580: 7363 6865 6d61 2022 7b7d 222e 2e2e da02  schema "{}".....
-00000590: 6964 da09 6765 6e65 7261 7465 64e9 0a00  id..generated...
-000005a0: 0000 2901 da07 6d69 6e75 7465 7329 01da  ..)...minutes)..
-000005b0: 0774 696d 656f 7574 da08 696e 7374 616e  .timeout..instan
-000005c0: 6365 7a19 466f 756e 6420 4772 6170 6851  cez.Found GraphQ
-000005d0: 4c20 7363 6865 6d61 2022 7b7d 227a 1d4e  L schema "{}"z.N
-000005e0: 6f74 2066 6f75 6e64 2047 7261 7068 514c  ot found GraphQL
-000005f0: 2073 6368 656d 6120 227b 7d22 2908 7206   schema "{}").r.
-00000600: 0000 00da 0469 6e66 6fda 0666 6f72 6d61  .....info..forma
-00000610: 7472 0200 0000 da0d 746f 7461 6c5f 7365  tr......total_se
-00000620: 636f 6e64 73da 0477 6169 7472 0400 0000  conds..waitr....
-00000630: 7218 0000 0029 0872 0e00 0000 720f 0000  r....).r....r...
-00000640: 00da 0a73 6368 656d 615f 6b65 79da 0b77  ...schema_key..w
-00000650: 6169 745f 7363 6865 6d61 da13 6765 6e65  ait_schema..gene
-00000660: 7261 7465 645f 636f 6e64 6974 696f 6e72  rated_conditionr
-00000670: 2300 0000 da05 6361 6368 65da 0d63 6163  #.....cache..cac
-00000680: 6865 645f 7363 6865 6d61 720d 0000 0072  hed_schemar....r
-00000690: 0d00 0000 7210 0000 0072 2a00 0000 2400  ....r....r*...$.
-000006a0: 0000 731a 0000 0000 0104 0104 0214 0208  ..s.............
-000006b0: 0106 010e 0116 020a 010a 010c 0114 0108  ................
-000006c0: 027a 1747 7261 7068 514c 5669 6577 2e77  .z.GraphQLView.w
-000006d0: 6169 745f 7363 6865 6d61 6301 0000 0000  ait_schemac.....
-000006e0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000006f0: 1e00 0000 7400 6401 8301 7d01 7401 6a02  ....t.d...}.t.j.
-00000700: 8300 7d02 7c01 6400 6400 7c02 6402 9c04  ..}.|.d.d.|.d...
-00000710: 5300 2903 4ee9 2000 0000 2904 721f 0000  S.).N. ...).r...
-00000720: 0072 2400 0000 da0f 6765 745f 7363 6865  .r$.....get_sche
-00000730: 6d61 5f74 696d 6572 2000 0000 2903 7209  ma_timer ...).r.
-00000740: 0000 00da 0974 6872 6561 6469 6e67 da09  .....threading..
-00000750: 436f 6e64 6974 696f 6e29 0372 0e00 0000  Condition).r....
-00000760: 5a0d 6e65 775f 7363 6865 6d61 5f69 645a  Z.new_schema_idZ
-00000770: 146e 6577 5f73 6368 656d 615f 6765 6e65  .new_schema_gene
-00000780: 7261 7465 6472 0d00 0000 720d 0000 0072  ratedr....r....r
-00000790: 1000 0000 da14 6372 6561 7465 5f73 6368  ......create_sch
-000007a0: 656d 615f 6f62 6a65 6374 3700 0000 7306  ema_object7...s.
-000007b0: 0000 0000 0108 0108 017a 2047 7261 7068  .........z Graph
-000007c0: 514c 5669 6577 2e63 7265 6174 655f 7363  QLView.create_sc
-000007d0: 6865 6d61 5f6f 626a 6563 7463 0500 0000  hema_objectc....
-000007e0: 0000 0000 0e00 0000 2300 0000 0300 0000  ........#.......
-000007f0: 736a 0100 0090 017a 4079 d674 006a 0164  sj.....z@y.t.j.d
-00000800: 016a 027c 0364 0219 0083 0183 0101 0087  .j.|.d..........
-00000810: 0066 0164 0364 0484 087d 0574 036a 0383  .f.d.d...}.t.j..
-00000820: 007d 0674 0483 006a 057c 017c 047c 0564  .}.t...j.|.|.|.d
-00000830: 058d 037d 0774 036a 0383 007d 0874 067c  ...}.t.j...}.t.|
-00000840: 087c 0618 0064 0683 027d 0974 077c 0183  .|...d...}.t.|..
-00000850: 018f 747d 0a7c 0a6a 087c 0283 017d 0b7c  ..t}.|.j.|...}.|
-00000860: 0b72 aa7c 0b64 0219 007c 0364 0219 006b  .r.|.d...|.d...k
-00000870: 0272 aa7c 037c 077c 0964 079c 0296 027d  .r.|.|.|.d.....}
-00000880: 037c 037c 0a7c 023c 0074 006a 0164 086a  .|.|.|.<.t.j.d.j
-00000890: 027c 0364 0219 0083 0183 0101 006e 2474  .|.d.........n$t
-000008a0: 006a 0164 096a 027c 0364 0219 007c 0b72  .j.d.j.|.d...|.r
-000008b0: c67c 0b6a 0864 0283 016e 0264 0083 0283  .|.j.d...n.d....
-000008c0: 0101 0057 0064 0051 0052 0058 007c 0753  ...W.d.Q.R.X.|.S
-000008d0: 0004 0074 096b 0a90 0172 3e01 007d 0c01  ...t.k...r>..}..
-000008e0: 007a 4674 077c 0183 018f 2e7d 0a7c 0a6a  .zFt.|.....}.|.j
-000008f0: 087c 0283 017d 0b7c 0b90 0172 207c 0b64  .|...}.|...r |.d
-00000900: 0219 007c 0364 0219 006b 0290 0172 207c  ...|.d...k...r |
-00000910: 0a7c 023d 0057 0064 0051 0052 0058 007c  .|.=.W.d.Q.R.X.|
-00000920: 0c82 0157 0059 0064 0064 007d 0c7e 0c58  ...W.Y.d.d.}.~.X
-00000930: 006e 0258 0057 0064 007c 0364 0a19 007d  .n.X.W.d.|.d...}
-00000940: 0d7c 0d8f 0e01 007c 0d6a 0a83 0001 0057  .|.....|.j.....W
-00000950: 0064 0051 0052 0058 0058 0064 0053 0029  .d.Q.R.X.X.d.S.)
-00000960: 0b4e 7a21 4765 6e65 7261 7469 6e67 2047  .Nz!Generating G
-00000970: 7261 7068 514c 2073 6368 656d 6120 227b  raphQL schema "{
-00000980: 7d22 2e2e 2e72 1f00 0000 6302 0000 0000  }"...r....c.....
-00000990: 0000 0004 0000 0003 0000 001f 0000 0073  ...............s
-000009a0: 1c00 0000 7c01 6a00 6a01 7c00 6a02 6401  ....|.j.j.|.j.d.
-000009b0: 3c00 8800 6a03 7c00 8301 0100 6400 5300  <...j.|.....d.S.
-000009c0: 2902 4e72 1200 0000 2904 da0a 7365 6c65  ).Nr....)...sele
-000009d0: 6374 6162 6c65 da04 6e61 6d65 7217 0000  ctable..namer...
-000009e0: 00da 1163 6865 636b 5f70 6572 6d69 7373  ...check_permiss
-000009f0: 696f 6e73 2904 720f 0000 00da 066d 6170  ions).r......map
-00000a00: 7065 72da 0461 7267 73da 066b 7761 7267  per..args..kwarg
-00000a10: 7329 0172 0e00 0000 720d 0000 0072 1000  s).r....r....r..
-00000a20: 0000 da0e 6265 666f 7265 5f72 6573 6f6c  ....before_resol
-00000a30: 7665 4000 0000 7304 0000 0000 010e 017a  ve@...s........z
-00000a40: 3147 7261 7068 514c 5669 6577 2e63 7265  1GraphQLView.cre
-00000a50: 6174 655f 7363 6865 6d61 2e3c 6c6f 6361  ate_schema.<loca
-00000a60: 6c73 3e2e 6265 666f 7265 5f72 6573 6f6c  ls>.before_resol
-00000a70: 7665 2901 7239 0000 00e9 0300 0000 2902  ve).r9........).
-00000a80: 7224 0000 0072 2f00 0000 7a19 5361 7665  r$...r/...z.Save
-00000a90: 6420 4772 6170 6851 4c20 7363 6865 6d61  d GraphQL schema
-00000aa0: 2022 7b7d 227a 3349 676e 6f72 696e 6720   "{}"z3Ignoring 
-00000ab0: 4772 6170 6851 4c20 7363 6865 6d61 2072  GraphQL schema r
-00000ac0: 6573 756c 7420 227b 7d22 2c20 6578 6973  esult "{}", exis
-00000ad0: 7469 6e67 3a20 227b 7d22 7220 0000 0029  ting: "{}"r ...)
-00000ae0: 0b72 0600 0000 7225 0000 0072 2600 0000  .r....r%...r&...
-00000af0: da04 7469 6d65 720a 0000 00da 0a67 6574  ..timer......get
-00000b00: 5f73 6368 656d 61da 0572 6f75 6e64 7204  _schema..roundr.
-00000b10: 0000 0072 1800 0000 da09 4578 6365 7074  ...r......Except
-00000b20: 696f 6eda 0a6e 6f74 6966 795f 616c 6c29  ion..notify_all)
-00000b30: 0e72 0e00 0000 720f 0000 0072 2900 0000  .r....r....r)...
-00000b40: da0a 6e65 775f 7363 6865 6d61 da05 6472  ..new_schema..dr
-00000b50: 6166 7472 3900 0000 5a10 6765 745f 7363  aftr9...Z.get_sc
-00000b60: 6865 6d61 5f73 7461 7274 da06 7363 6865  hema_start..sche
-00000b70: 6d61 5a0e 6765 745f 7363 6865 6d61 5f65  maZ.get_schema_e
-00000b80: 6e64 722f 0000 0072 2c00 0000 722d 0000  ndr/...r,...r-..
-00000b90: 00da 0165 722b 0000 0072 0d00 0000 2901  ...er+...r....).
-00000ba0: 720e 0000 0072 1000 0000 da0d 6372 6561  r....r......crea
-00000bb0: 7465 5f73 6368 656d 613c 0000 0073 3400  te_schema<...s4.
-00000bc0: 0000 0001 0601 1402 0c04 0801 1201 0801  ................
-00000bd0: 0e02 0a01 0a02 1401 0e01 0802 1602 0801  ................
-00000be0: 0601 2003 0401 1201 0a01 0a02 1801 1002  .. .............
-00000bf0: 1a02 0801 0601 7a19 4772 6170 6851 4c56  ......z.GraphQLV
-00000c00: 6965 772e 6372 6561 7465 5f73 6368 656d  iew.create_schem
-00000c10: 6163 0300 0000 0000 0000 0900 0000 1300  ac..............
-00000c20: 0000 4300 0000 73b4 0000 007c 0272 0864  ..C...s....|.r.d
-00000c30: 016e 0264 027d 0364 007d 0474 007c 0183  .n.d.}.d.}.t.|..
-00000c40: 018f 487d 057c 056a 017c 0383 017d 067c  ..H}.|.j.|...}.|
-00000c50: 0672 387c 0664 0319 0072 387c 0664 0319  .r8|.d...r8|.d..
-00000c60: 0053 007c 0672 4c7c 0664 0319 000c 0072  .S.|.rL|.d.....r
-00000c70: 4c7c 067d 046e 107c 006a 0283 007d 077c  L|.}.n.|.j...}.|
-00000c80: 077c 057c 033c 0057 0064 0051 0052 0058  .|.|.<.W.d.Q.R.X
-00000c90: 007c 0472 a47c 006a 037c 017c 037c 0483  .|.r.|.j.|.|.|..
-00000ca0: 037d 087c 0872 807c 0853 0074 007c 0183  .}.|.r.|.S.t.|..
-00000cb0: 018f 167d 057c 006a 0283 007d 077c 077c  ...}.|.j...}.|.|
-00000cc0: 057c 033c 0057 0064 0051 0052 0058 007c  .|.<.W.d.Q.R.X.|
-00000cd0: 006a 047c 017c 037c 077c 0283 0453 0029  .j.|.|.|.|...S.)
-00000ce0: 044e da14 6772 6170 6871 6c5f 7363 6865  .N..graphql_sche
-00000cf0: 6d61 5f64 7261 6674 da0e 6772 6170 6871  ma_draft..graphq
-00000d00: 6c5f 7363 6865 6d61 7224 0000 0029 0572  l_schemar$...).r
-00000d10: 0400 0000 7218 0000 0072 3200 0000 722a  ....r....r2...r*
-00000d20: 0000 0072 4400 0000 2909 720e 0000 0072  ...rD...).r....r
-00000d30: 0f00 0000 7241 0000 0072 2900 0000 722a  ....rA...r)...r*
-00000d40: 0000 0072 2c00 0000 722d 0000 0072 4000  ...r,...r-...r@.
-00000d50: 0000 5a0f 6578 6973 7469 6e67 5f73 6368  ..Z.existing_sch
-00000d60: 656d 6172 0d00 0000 720d 0000 0072 1000  emar....r....r..
-00000d70: 0000 723c 0000 0065 0000 0073 2400 0000  ..r<...e...s$...
-00000d80: 0001 0c01 0402 0a01 0a02 0c01 0801 0e01  ................
-00000d90: 0602 0801 1202 0401 0e01 0401 0402 0a01  ................
-00000da0: 0801 1202 7a16 4772 6170 6851 4c56 6965  ....z.GraphQLVie
-00000db0: 772e 6765 745f 7363 6865 6d61 6302 0000  w.get_schemac...
-00000dc0: 0000 0000 0004 0000 0003 0000 004f 0000  .............O..
-00000dd0: 0073 1200 0000 7c00 6a00 7c01 6601 7c02  .s....|.j.|.f.|.
-00000de0: 9e02 7c03 8e01 5300 2901 4e29 01da 0470  ..|...S.).N)...p
-00000df0: 6f73 7429 0472 0e00 0000 720f 0000 0072  ost).r....r....r
-00000e00: 3700 0000 7238 0000 0072 0d00 0000 720d  7...r8...r....r.
-00000e10: 0000 0072 1000 0000 7218 0000 007f 0000  ...r....r.......
-00000e20: 0073 0200 0000 0001 7a0f 4772 6170 6851  .s......z.GraphQ
-00000e30: 4c56 6965 772e 6765 7463 0200 0000 0000  LView.getc......
-00000e40: 0000 0c00 0000 1400 0000 0f00 0000 7306  ..............s.
-00000e50: 0100 0074 007c 016a 0164 0164 0283 0283  ...t.|.j.d.d....
-00000e60: 017d 0474 007c 016a 026a 0364 0364 0483  .}.t.|.j.j.d.d..
-00000e70: 0283 017d 0564 057c 016a 026b 0772 3474  ...}.d.|.j.k.r4t
-00000e80: 0469 0083 0153 0079 1088 006a 057c 017c  .i...S.y...j.|.|
-00000e90: 0483 027d 0657 006e 3004 0074 066b 0a72  ...}.W.n0..t.k.r
-00000ea0: 7401 007d 0701 007a 1474 0464 0664 076a  t..}...z.t.d.d.j
-00000eb0: 077c 0783 0167 0169 0183 0153 0064 007d  .|...g.i...S.d.}
-00000ec0: 077e 0758 006e 0258 007c 016a 026a 0364  .~.X.n.X.|.j.j.d
-00000ed0: 0583 017d 087c 017c 016a 0864 089c 027d  ...}.|.|.j.d...}
-00000ee0: 097c 066a 097c 0869 007c 097c 0564 098d  .|.j.|.i.|.|.d..
-00000ef0: 047d 0a7c 0a6a 0a64 006b 0972 f874 0b7c  .}.|.j.d.k.r.t.|
-00000f00: 0a6a 0a83 0172 f87c 0a6a 0a64 0a19 007d  .j...r.|.j.d...}
-00000f10: 0b74 0c7c 0b64 0b83 0272 ce7c 0b6a 0d7d  .t.|.d...r.|.j.}
-00000f20: 0b74 0e7c 0b74 0f83 0272 dc7c 0b82 0174  .t.|.t...r.|...t
-00000f30: 0464 0674 1087 0066 0164 0c64 0d84 087c  .d.t...f.d.d...|
-00000f40: 0a6a 0a83 0269 0183 0153 0074 0464 0e7c  .j...i...S.t.d.|
-00000f50: 0a6a 0269 0183 0153 0029 0f4e 7241 0000  .j.i...S.).NrA..
-00000f60: 0046 da08 7661 6c69 6461 7465 54da 0571  .F..validateT..q
-00000f70: 7565 7279 da06 6572 726f 7273 7a1e 4661  uery..errorsz.Fa
-00000f80: 696c 6564 2074 6f20 6765 7420 7461 626c  iled to get tabl
-00000f90: 6520 7363 6865 6d61 3a20 7b7d 2902 720f  e schema: {}).r.
-00000fa0: 0000 00da 0773 6573 7369 6f6e 2903 da09  .....session)...
-00000fb0: 7661 7269 6162 6c65 73da 0d63 6f6e 7465  variables..conte
-00000fc0: 7874 5f76 616c 7565 7248 0000 0072 0100  xt_valuerH...r..
-00000fd0: 0000 da0e 6f72 6967 696e 616c 5f65 7272  ....original_err
-00000fe0: 6f72 6301 0000 0000 0000 0001 0000 0002  orc.............
-00000ff0: 0000 0013 0000 0073 0a00 0000 8800 6a00  .......s......j.
-00001000: 7c00 8301 5300 2901 4e29 0172 1e00 0000  |...S.).N).r....
-00001010: 2901 da01 7829 0172 0e00 0000 720d 0000  )...x).r....r...
-00001020: 0072 1000 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
-00001030: a000 0000 7300 0000 007a 2247 7261 7068  ....s....z"Graph
-00001040: 514c 5669 6577 2e70 6f73 742e 3c6c 6f63  QLView.post.<loc
-00001050: 616c 733e 2e3c 6c61 6d62 6461 3eda 0464  als>.<lambda>..d
-00001060: 6174 6129 11da 0462 6f6f 6cda 0c67 6574  ata)...bool..get
-00001070: 5f61 7267 756d 656e 7472 5100 0000 7218  _argumentrQ...r.
-00001080: 0000 0072 0800 0000 723c 0000 0072 3e00  ...r....r<...r>.
-00001090: 0000 7226 0000 0072 4b00 0000 da07 6578  ..r&...rK.....ex
-000010a0: 6563 7574 6572 4a00 0000 da03 6c65 6eda  ecuterJ.....len.
-000010b0: 0768 6173 6174 7472 724e 0000 0072 1a00  .hasattrrN...r..
-000010c0: 0000 7205 0000 00da 036d 6170 290c 720e  ..r......map).r.
-000010d0: 0000 0072 0f00 0000 7237 0000 0072 3800  ...r....r7...r8.
-000010e0: 0000 7241 0000 0072 4800 0000 7242 0000  ..rA...rH...rB..
-000010f0: 0072 4300 0000 7249 0000 0072 4d00 0000  .rC...rI...rM...
-00001100: da06 7265 7375 6c74 721d 0000 0072 0d00  ..resultr....r..
-00001110: 0000 2901 720e 0000 0072 1000 0000 7247  ..).r....r....rG
-00001120: 0000 0082 0000 0073 3200 0000 0001 1001  .......s2.......
-00001130: 1202 0a01 0802 0201 1001 1001 2002 0c02  ............ ...
-00001140: 0201 0a02 0401 0201 0201 0201 0803 1401  ................
-00001150: 0a01 0a01 0601 0a01 0401 1c02 0201 7a10  ..............z.
-00001160: 4772 6170 6851 4c56 6965 772e 706f 7374  GraphQLView.post
-00001170: 4e29 0eda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00001180: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001190: 6c6e 616d 655f 5f72 0700 0000 da12 7065  lname__r......pe
-000011a0: 726d 6973 7369 6f6e 5f63 6c61 7373 6573  rmission_classes
-000011b0: 7211 0000 0072 1900 0000 721e 0000 0072  r....r....r....r
-000011c0: 2a00 0000 7232 0000 0072 4400 0000 723c  *...r2...rD...r<
-000011d0: 0000 0072 1800 0000 7247 0000 0072 0d00  ...r....rG...r..
-000011e0: 0000 720d 0000 0072 0d00 0000 7210 0000  ..r....r....r...
-000011f0: 0072 0c00 0000 1100 0000 7314 0000 0008  .r........s.....
-00001200: 0106 0208 0308 0708 0608 1308 0508 2908  ..............).
-00001210: 1a08 0372 0c00 0000 2917 7230 0000 0072  ...r....).r0...r
-00001220: 3b00 0000 da08 6461 7465 7469 6d65 7202  ;.....datetimer.
-00001230: 0000 005a 0767 7261 7068 716c 7203 0000  ...Z.graphqlr...
-00001240: 00da 126a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
-00001250: 7365 2e64 6272 0400 0000 da2c 6a65 745f  se.dbr.....,jet_
-00001260: 6272 6964 6765 5f62 6173 652e 6578 6365  bridge_base.exce
-00001270: 7074 696f 6e73 2e70 6572 6d69 7373 696f  ptions.permissio
-00001280: 6e5f 6465 6e69 6564 7205 0000 00da 166a  n_deniedr......j
-00001290: 6574 5f62 7269 6467 655f 6261 7365 2e6c  et_bridge_base.l
-000012a0: 6f67 6765 7272 0600 0000 5a1b 6a65 745f  oggerr....Z.jet_
-000012b0: 6272 6964 6765 5f62 6173 652e 7065 726d  bridge_base.perm
-000012c0: 6973 7369 6f6e 7372 0700 0000 da1e 6a65  issionsr......je
-000012d0: 745f 6272 6964 6765 5f62 6173 652e 7265  t_bridge_base.re
-000012e0: 7370 6f6e 7365 732e 6a73 6f6e 7208 0000  sponses.jsonr...
-000012f0: 00da 1c6a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
-00001300: 7365 2e75 7469 6c73 2e63 6f6d 6d6f 6e72  se.utils.commonr
-00001310: 0900 0000 5a1d 6a65 745f 6272 6964 6765  ....Z.jet_bridge
-00001320: 5f62 6173 652e 7574 696c 732e 6772 6170  _base.utils.grap
-00001330: 6871 6c72 0a00 0000 da1e 6a65 745f 6272  hqlr......jet_br
-00001340: 6964 6765 5f62 6173 652e 7669 6577 732e  idge_base.views.
-00001350: 6261 7365 2e61 7069 720b 0000 0072 0c00  base.apir....r..
-00001360: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00001370: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001380: 0100 0000 7318 0000 0008 0108 010c 020c  ....s...........
-00001390: 020c 010c 010c 010c 010c 010c 010c 010c  ................
-000013a0: 03                                       .
+00000000: 420d 0d0a 0000 0000 4d5d 2d64 a418 0000  B.......M]-d....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 a800 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 5a00 6400 6401 6c01 5a01 6400 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
+00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6408 6c0e 6d0f 5a0f 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6409 6c10 6d11 5a11 0100 6400 640a 6c12  d.l.m.Z...d.d.l.
+000000a0: 6d13 5a13 0100 6400 640b 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 640c 6c16 6d17 5a17 0100 4700  ..d.d.l.m.Z...G.
+000000c0: 640d 640e 8400 640e 6517 8303 5a18 6401  d.d...d.e...Z.d.
+000000d0: 5300 290f e900 0000 004e 2901 da09 7469  S.)......N)...ti
+000000e0: 6d65 6465 6c74 6129 01da 0c47 7261 7068  medelta)...Graph
+000000f0: 514c 4572 726f 7229 01da 1063 6f6e 6e65  QLError)...conne
+00000100: 6374 696f 6e5f 6361 6368 6529 01da 1050  ction_cache)...P
+00000110: 6572 6d69 7373 696f 6e44 656e 6965 6429  ermissionDenied)
+00000120: 01da 066c 6f67 6765 7229 01da 1548 6173  ...logger)...Has
+00000130: 5072 6f6a 6563 7450 6572 6d69 7373 696f  ProjectPermissio
+00000140: 6e73 2901 da0c 4a53 4f4e 5265 7370 6f6e  ns)...JSONRespon
+00000150: 7365 2901 da11 6765 745f 7261 6e64 6f6d  se)...get_random
+00000160: 5f73 7472 696e 6729 01da 1647 7261 7068  _string)...Graph
+00000170: 514c 5363 6865 6d61 4765 6e65 7261 746f  QLSchemaGenerato
+00000180: 7229 01da 1474 7261 636b 5f64 6174 6162  r)...track_datab
+00000190: 6173 655f 6173 796e 6329 01da 0741 5049  ase_async)...API
+000001a0: 5669 6577 6300 0000 0000 0000 0000 0000  Viewc...........
+000001b0: 0002 0000 0040 0000 0073 5a00 0000 6500  .....@...sZ...e.
+000001c0: 5a01 6400 5a02 6503 6601 5a04 6401 6402  Z.d.Z.e.f.Z.d.d.
+000001d0: 8400 5a05 6403 6404 8400 5a06 6405 6406  ..Z.d.d...Z.d.d.
+000001e0: 8400 5a07 6407 6408 8400 5a08 6409 640a  ..Z.d.d...Z.d.d.
+000001f0: 8400 5a09 640b 640c 8400 5a0a 640d 640e  ..Z.d.d...Z.d.d.
+00000200: 8400 5a0b 640f 6410 8400 5a0c 6411 6412  ..Z.d.d...Z.d.d.
+00000210: 8400 5a0d 6413 5300 2914 da0b 4772 6170  ..Z.d.S.)...Grap
+00000220: 6851 4c56 6965 7763 0200 0000 0000 0000  hQLViewc........
+00000230: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+00000240: 0064 0053 0029 014e a900 2902 da04 7365  .d.S.).N..)...se
+00000250: 6c66 da07 7265 7175 6573 7472 0e00 0000  lf..requestr....
+00000260: 720e 0000 00fa 642f 5573 6572 732f 6631  r.....d/Users/f1
+00000270: 6e61 6c2f 4472 6f70 626f 782f 7079 7468  nal/Dropbox/pyth
+00000280: 6f6e 2f6a 6574 2d62 7269 6467 652f 7372  on/jet-bridge/sr
+00000290: 632f 7061 636b 6167 6573 2f6a 6574 5f62  c/packages/jet_b
+000002a0: 7269 6467 655f 6261 7365 2f6a 6574 5f62  ridge_base/jet_b
+000002b0: 7269 6467 655f 6261 7365 2f76 6965 7773  ridge_base/views
+000002c0: 2f67 7261 7068 716c 2e70 79da 2162 6566  /graphql.py.!bef
+000002d0: 6f72 655f 6469 7370 6174 6368 5f70 6572  ore_dispatch_per
+000002e0: 6d69 7373 696f 6e73 5f63 6865 636b 1500  missions_check..
+000002f0: 0000 7302 0000 0000 017a 2d47 7261 7068  ..s......z-Graph
+00000300: 514c 5669 6577 2e62 6566 6f72 655f 6469  QLView.before_di
+00000310: 7370 6174 6368 5f70 6572 6d69 7373 696f  spatch_permissio
+00000320: 6e73 5f63 6865 636b 6302 0000 0000 0000  ns_checkc.......
+00000330: 0002 0000 0004 0000 0043 0000 0073 1400  .........C...s..
+00000340: 0000 6401 7c01 6a00 a001 6401 a101 6402  ..d.|.j...d...d.
+00000350: 6403 9c03 5300 2904 4eda 056d 6f64 656c  d...S.).N..model
+00000360: da01 7229 03da 0f70 6572 6d69 7373 696f  ..r)...permissio
+00000370: 6e5f 7479 7065 da11 7065 726d 6973 7369  n_type..permissi
+00000380: 6f6e 5f6f 626a 6563 74da 1270 6572 6d69  on_object..permi
+00000390: 7373 696f 6e5f 6163 7469 6f6e 7329 02da  ssion_actions)..
+000003a0: 0763 6f6e 7465 7874 da03 6765 7429 0272  .context..get).r
+000003b0: 0f00 0000 7210 0000 0072 0e00 0000 720e  ....r....r....r.
+000003c0: 0000 0072 1100 0000 da1b 7265 7175 6972  ...r......requir
+000003d0: 6564 5f70 726f 6a65 6374 5f70 6572 6d69  ed_project_permi
+000003e0: 7373 696f 6e18 0000 0073 0600 0000 0002  ssion....s......
+000003f0: 0201 0a01 7a27 4772 6170 6851 4c56 6965  ....z'GraphQLVie
+00000400: 772e 7265 7175 6972 6564 5f70 726f 6a65  w.required_proje
+00000410: 6374 5f70 6572 6d69 7373 696f 6e63 0200  ct_permissionc..
+00000420: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000430: 0000 731c 0000 0074 007c 0174 0183 0272  ..s....t.|.t...r
+00000440: 107c 016a 0253 0074 037c 0183 0153 0064  .|.j.S.t.|...S.d
+00000450: 0053 0029 014e 2904 da0a 6973 696e 7374  .S.).N)...isinst
+00000460: 616e 6365 7203 0000 00da 076d 6573 7361  ancer......messa
+00000470: 6765 da03 7374 7229 0272 0f00 0000 da05  ge..str).r......
+00000480: 6572 726f 7272 0e00 0000 720e 0000 0072  errorr....r....r
+00000490: 1100 0000 da0d 6d61 705f 6771 6c5f 6572  ......map_gql_er
+000004a0: 726f 721f 0000 0073 0600 0000 0001 0a01  ror....s........
+000004b0: 0602 7a19 4772 6170 6851 4c56 6965 772e  ..z.GraphQLView.
+000004c0: 6d61 705f 6771 6c5f 6572 726f 7263 0400  map_gql_errorc..
+000004d0: 0000 0000 0000 0800 0000 0900 0000 4300  ..............C.
+000004e0: 0000 73ac 0000 007c 0373 0864 0053 0074  ..s....|.s.d.S.t
+000004f0: 00a0 0164 01a0 027c 0364 0219 00a1 01a1  ...d...|.d......
+00000500: 0101 007c 0364 0319 007d 047c 048f 2001  ...|.d...}.|.. .
+00000510: 0074 0364 0464 058d 01a0 04a1 007d 057c  .t.d.d.......}.|
+00000520: 046a 057c 0564 068d 0101 0057 0064 0051  .j.|.d.....W.d.Q
+00000530: 0052 0058 0074 067c 0183 018f 4c7d 067c  .R.X.t.|....L}.|
+00000540: 06a0 077c 02a1 017d 077c 0772 8a7c 0764  ...|...}.|.r.|.d
+00000550: 0719 0072 8a74 00a0 0164 08a0 027c 0364  ...r.t...d...|.d
+00000560: 0219 00a1 01a1 0101 007c 0764 0719 0053  .........|.d...S
+00000570: 0074 00a0 0164 09a0 027c 0364 0219 00a1  .t...d...|.d....
+00000580: 01a1 0101 0057 0064 0051 0052 0058 0064  .....W.d.Q.R.X.d
+00000590: 0053 0029 0a4e 7a1e 5761 6974 696e 6720  .S.).Nz.Waiting 
+000005a0: 4772 6170 6851 4c20 7363 6865 6d61 2022  GraphQL schema "
+000005b0: 7b7d 222e 2e2e da02 6964 da09 6765 6e65  {}".....id..gene
+000005c0: 7261 7465 64e9 0a00 0000 2901 da07 6d69  rated.....)...mi
+000005d0: 6e75 7465 7329 01da 0774 696d 656f 7574  nutes)...timeout
+000005e0: da08 696e 7374 616e 6365 7a19 466f 756e  ..instancez.Foun
+000005f0: 6420 4772 6170 6851 4c20 7363 6865 6d61  d GraphQL schema
+00000600: 2022 7b7d 227a 1d4e 6f74 2066 6f75 6e64   "{}"z.Not found
+00000610: 2047 7261 7068 514c 2073 6368 656d 6120   GraphQL schema 
+00000620: 227b 7d22 2908 7206 0000 00da 0469 6e66  "{}").r......inf
+00000630: 6fda 0666 6f72 6d61 7472 0200 0000 da0d  o..formatr......
+00000640: 746f 7461 6c5f 7365 636f 6e64 73da 0477  total_seconds..w
+00000650: 6169 7472 0400 0000 7219 0000 0029 0872  aitr....r....).r
+00000660: 0f00 0000 7210 0000 00da 0a73 6368 656d  ....r......schem
+00000670: 615f 6b65 79da 0b77 6169 745f 7363 6865  a_key..wait_sche
+00000680: 6d61 da13 6765 6e65 7261 7465 645f 636f  ma..generated_co
+00000690: 6e64 6974 696f 6e72 2400 0000 da05 6361  nditionr$.....ca
+000006a0: 6368 65da 0d63 6163 6865 645f 7363 6865  che..cached_sche
+000006b0: 6d61 720e 0000 0072 0e00 0000 7211 0000  mar....r....r...
+000006c0: 0072 2b00 0000 2500 0000 731a 0000 0000  .r+...%...s.....
+000006d0: 0104 0104 0214 0208 0106 010e 0116 020a  ................
+000006e0: 010a 010c 0114 0108 027a 1747 7261 7068  .........z.Graph
+000006f0: 514c 5669 6577 2e77 6169 745f 7363 6865  QLView.wait_sche
+00000700: 6d61 6301 0000 0000 0000 0003 0000 0005  mac.............
+00000710: 0000 0043 0000 0073 1e00 0000 7400 6401  ...C...s....t.d.
+00000720: 8301 7d01 7401 a002 a100 7d02 7c01 6400  ..}.t.....}.|.d.
+00000730: 6400 7c02 6402 9c04 5300 2903 4ee9 2000  d.|.d...S.).N. .
+00000740: 0000 2904 7220 0000 0072 2500 0000 da0f  ..).r ...r%.....
+00000750: 6765 745f 7363 6865 6d61 5f74 696d 6572  get_schema_timer
+00000760: 2100 0000 2903 7209 0000 00da 0974 6872  !...).r......thr
+00000770: 6561 6469 6e67 da09 436f 6e64 6974 696f  eading..Conditio
+00000780: 6e29 0372 0f00 0000 5a0d 6e65 775f 7363  n).r....Z.new_sc
+00000790: 6865 6d61 5f69 645a 146e 6577 5f73 6368  hema_idZ.new_sch
+000007a0: 656d 615f 6765 6e65 7261 7465 6472 0e00  ema_generatedr..
+000007b0: 0000 720e 0000 0072 1100 0000 da14 6372  ..r....r......cr
+000007c0: 6561 7465 5f73 6368 656d 615f 6f62 6a65  eate_schema_obje
+000007d0: 6374 3800 0000 7306 0000 0000 0108 0108  ct8...s.........
+000007e0: 017a 2047 7261 7068 514c 5669 6577 2e63  .z GraphQLView.c
+000007f0: 7265 6174 655f 7363 6865 6d61 5f6f 626a  reate_schema_obj
+00000800: 6563 7463 0500 0000 0000 0000 0e00 0000  ectc............
+00000810: 0f00 0000 0300 0000 736a 0100 0090 017a  ........sj.....z
+00000820: 4079 d674 00a0 0164 01a0 027c 0364 0219  @y.t...d...|.d..
+00000830: 00a1 01a1 0101 0087 0066 0164 0364 0484  .........f.d.d..
+00000840: 087d 0574 03a0 03a1 007d 0674 0483 006a  .}.t.....}.t...j
+00000850: 057c 017c 047c 0564 058d 037d 0774 03a0  .|.|.|.d...}.t..
+00000860: 03a1 007d 0874 067c 087c 0618 0064 0683  ...}.t.|.|...d..
+00000870: 027d 0974 077c 0183 018f 747d 0a7c 0aa0  .}.t.|....t}.|..
+00000880: 087c 02a1 017d 0b7c 0b72 aa7c 0b64 0219  .|...}.|.r.|.d..
+00000890: 007c 0364 0219 006b 0272 aa7c 037c 077c  .|.d...k.r.|.|.|
+000008a0: 0964 079c 0296 027d 037c 037c 0a7c 023c  .d.....}.|.|.|.<
+000008b0: 0074 00a0 0164 08a0 027c 0364 0219 00a1  .t...d...|.d....
+000008c0: 01a1 0101 006e 2474 00a0 0164 09a0 027c  .....n$t...d...|
+000008d0: 0364 0219 007c 0b72 c67c 0ba0 0864 02a1  .d...|.r.|...d..
+000008e0: 016e 0264 00a1 02a1 0101 0057 0064 0051  .n.d.......W.d.Q
+000008f0: 0052 0058 007c 0753 0004 0074 096b 0a90  .R.X.|.S...t.k..
+00000900: 0172 3e01 007d 0c01 007a 4474 077c 0183  .r>..}...zDt.|..
+00000910: 018f 2e7d 0a7c 0aa0 087c 02a1 017d 0b7c  ...}.|...|...}.|
+00000920: 0b90 0172 207c 0b64 0219 007c 0364 0219  ...r |.d...|.d..
+00000930: 006b 0290 0172 207c 0a7c 023d 0057 0064  .k...r |.|.=.W.d
+00000940: 0051 0052 0058 007c 0c82 0157 0064 0064  .Q.R.X.|...W.d.d
+00000950: 007d 0c7e 0c58 0059 006e 0258 0057 0064  .}.~.X.Y.n.X.W.d
+00000960: 007c 0364 0a19 007d 0d7c 0d8f 0e01 007c  .|.d...}.|.....|
+00000970: 0da0 0aa1 0001 0057 0064 0051 0052 0058  .......W.d.Q.R.X
+00000980: 0058 0064 0053 0029 0b4e 7a21 4765 6e65  .X.d.S.).Nz!Gene
+00000990: 7261 7469 6e67 2047 7261 7068 514c 2073  rating GraphQL s
+000009a0: 6368 656d 6120 227b 7d22 2e2e 2e72 2000  chema "{}"...r .
+000009b0: 0000 6302 0000 0000 0000 0004 0000 0003  ..c.............
+000009c0: 0000 001f 0000 0073 1c00 0000 7c01 6a00  .......s....|.j.
+000009d0: 6a01 7c00 6a02 6401 3c00 8800 a003 7c00  j.|.j.d.<.....|.
+000009e0: a101 0100 6400 5300 2902 4e72 1300 0000  ....d.S.).Nr....
+000009f0: 2904 da0a 7365 6c65 6374 6162 6c65 da04  )...selectable..
+00000a00: 6e61 6d65 7218 0000 00da 1163 6865 636b  namer......check
+00000a10: 5f70 6572 6d69 7373 696f 6e73 2904 7210  _permissions).r.
+00000a20: 0000 00da 066d 6170 7065 72da 0461 7267  .....mapper..arg
+00000a30: 73da 066b 7761 7267 7329 0172 0f00 0000  s..kwargs).r....
+00000a40: 720e 0000 0072 1100 0000 da0e 6265 666f  r....r......befo
+00000a50: 7265 5f72 6573 6f6c 7665 4100 0000 7304  re_resolveA...s.
+00000a60: 0000 0000 010e 017a 3147 7261 7068 514c  .......z1GraphQL
+00000a70: 5669 6577 2e63 7265 6174 655f 7363 6865  View.create_sche
+00000a80: 6d61 2e3c 6c6f 6361 6c73 3e2e 6265 666f  ma.<locals>.befo
+00000a90: 7265 5f72 6573 6f6c 7665 2901 723a 0000  re_resolve).r:..
+00000aa0: 00e9 0300 0000 2902 7225 0000 0072 3000  ......).r%...r0.
+00000ab0: 0000 7a19 5361 7665 6420 4772 6170 6851  ..z.Saved GraphQ
+00000ac0: 4c20 7363 6865 6d61 2022 7b7d 227a 3349  L schema "{}"z3I
+00000ad0: 676e 6f72 696e 6720 4772 6170 6851 4c20  gnoring GraphQL 
+00000ae0: 7363 6865 6d61 2072 6573 756c 7420 227b  schema result "{
+00000af0: 7d22 2c20 6578 6973 7469 6e67 3a20 227b  }", existing: "{
+00000b00: 7d22 7221 0000 0029 0b72 0600 0000 7226  }"r!...).r....r&
+00000b10: 0000 0072 2700 0000 da04 7469 6d65 720a  ...r'.....timer.
+00000b20: 0000 00da 0a67 6574 5f73 6368 656d 61da  .....get_schema.
+00000b30: 0572 6f75 6e64 7204 0000 0072 1900 0000  .roundr....r....
+00000b40: da09 4578 6365 7074 696f 6eda 0a6e 6f74  ..Exception..not
+00000b50: 6966 795f 616c 6c29 0e72 0f00 0000 7210  ify_all).r....r.
+00000b60: 0000 0072 2a00 0000 da0a 6e65 775f 7363  ...r*.....new_sc
+00000b70: 6865 6d61 da05 6472 6166 7472 3a00 0000  hema..draftr:...
+00000b80: 5a10 6765 745f 7363 6865 6d61 5f73 7461  Z.get_schema_sta
+00000b90: 7274 da06 7363 6865 6d61 5a0e 6765 745f  rt..schemaZ.get_
+00000ba0: 7363 6865 6d61 5f65 6e64 7230 0000 0072  schema_endr0...r
+00000bb0: 2d00 0000 722e 0000 00da 0165 722c 0000  -...r......er,..
+00000bc0: 0072 0e00 0000 2901 720f 0000 0072 1100  .r....).r....r..
+00000bd0: 0000 da0d 6372 6561 7465 5f73 6368 656d  ....create_schem
+00000be0: 613d 0000 0073 3400 0000 0001 0601 1402  a=...s4.........
+00000bf0: 0c04 0801 1201 0801 0e02 0a01 0a02 1401  ................
+00000c00: 0e01 0802 1602 0801 0601 2003 0401 1201  .......... .....
+00000c10: 0a01 0a02 1801 1002 1a02 0801 0601 7a19  ..............z.
+00000c20: 4772 6170 6851 4c56 6965 772e 6372 6561  GraphQLView.crea
+00000c30: 7465 5f73 6368 656d 6163 0300 0000 0000  te_schemac......
+00000c40: 0000 0900 0000 0900 0000 4300 0000 73b2  ..........C...s.
+00000c50: 0000 007c 0272 0864 016e 0264 027d 0364  ...|.r.d.n.d.}.d
+00000c60: 007d 0474 007c 0183 018f 467d 057c 05a0  .}.t.|....F}.|..
+00000c70: 017c 03a1 017d 067c 0672 387c 0664 0319  .|...}.|.r8|.d..
+00000c80: 0072 387c 0664 0319 0053 007c 0672 4a7c  .r8|.d...S.|.rJ|
+00000c90: 0664 0319 0073 4a7c 067d 046e 107c 00a0  .d...sJ|.}.n.|..
+00000ca0: 02a1 007d 077c 077c 057c 033c 0057 0064  ...}.|.|.|.<.W.d
+00000cb0: 0051 0052 0058 007c 0472 a27c 00a0 037c  .Q.R.X.|.r.|...|
+00000cc0: 017c 037c 04a1 037d 087c 0872 7e7c 0853  .|.|...}.|.r~|.S
+00000cd0: 0074 007c 0183 018f 167d 057c 00a0 02a1  .t.|.....}.|....
+00000ce0: 007d 077c 077c 057c 033c 0057 0064 0051  .}.|.|.|.<.W.d.Q
+00000cf0: 0052 0058 007c 00a0 047c 017c 037c 077c  .R.X.|...|.|.|.|
+00000d00: 02a1 0453 0029 044e da14 6772 6170 6871  ...S.).N..graphq
+00000d10: 6c5f 7363 6865 6d61 5f64 7261 6674 da0e  l_schema_draft..
+00000d20: 6772 6170 6871 6c5f 7363 6865 6d61 7225  graphql_schemar%
+00000d30: 0000 0029 0572 0400 0000 7219 0000 0072  ...).r....r....r
+00000d40: 3300 0000 722b 0000 0072 4500 0000 2909  3...r+...rE...).
+00000d50: 720f 0000 0072 1000 0000 7242 0000 0072  r....r....rB...r
+00000d60: 2a00 0000 722b 0000 0072 2d00 0000 722e  *...r+...r-...r.
+00000d70: 0000 0072 4100 0000 5a0f 6578 6973 7469  ...rA...Z.existi
+00000d80: 6e67 5f73 6368 656d 6172 0e00 0000 720e  ng_schemar....r.
+00000d90: 0000 0072 1100 0000 723d 0000 0066 0000  ...r....r=...f..
+00000da0: 0073 2400 0000 0001 0c01 0402 0a01 0a02  .s$.............
+00000db0: 0c01 0801 0c01 0602 0801 1202 0401 0e01  ................
+00000dc0: 0401 0402 0a01 0801 1202 7a16 4772 6170  ..........z.Grap
+00000dd0: 6851 4c56 6965 772e 6765 745f 7363 6865  hQLView.get_sche
+00000de0: 6d61 6302 0000 0000 0000 0004 0000 0003  mac.............
+00000df0: 0000 004f 0000 0073 1200 0000 7c00 6a00  ...O...s....|.j.
+00000e00: 7c01 6601 7c02 9e02 7c03 8e01 5300 2901  |.f.|...|...S.).
+00000e10: 4e29 01da 0470 6f73 7429 0472 0f00 0000  N)...post).r....
+00000e20: 7210 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
+00000e30: 0e00 0000 720e 0000 0072 1100 0000 7219  ....r....r....r.
+00000e40: 0000 0080 0000 0073 0200 0000 0001 7a0f  .......s......z.
+00000e50: 4772 6170 6851 4c56 6965 772e 6765 7463  GraphQLView.getc
+00000e60: 0200 0000 0000 0000 0c00 0000 0a00 0000  ................
+00000e70: 0f00 0000 7314 0100 0074 007c 0183 0101  ....s....t.|....
+00000e80: 0074 017c 01a0 0264 0164 02a1 0283 017d  .t.|...d.d.....}
+00000e90: 0474 017c 016a 03a0 0464 0364 04a1 0283  .t.|.j...d.d....
+00000ea0: 017d 0564 057c 016a 036b 0772 3c74 0569  .}.d.|.j.k.r<t.i
+00000eb0: 0083 0153 0079 1088 00a0 067c 017c 04a1  ...S.y.....|.|..
+00000ec0: 027d 0657 006e 3204 0074 076b 0a72 7e01  .}.W.n2..t.k.r~.
+00000ed0: 007d 0701 007a 1474 0564 0664 07a0 087c  .}...z.t.d.d...|
+00000ee0: 07a1 0167 0169 0183 0153 0064 007d 077e  ...g.i...S.d.}.~
+00000ef0: 0758 0059 006e 0258 007c 016a 03a0 0464  .X.Y.n.X.|.j...d
+00000f00: 05a1 017d 087c 017c 016a 0964 089c 027d  ...}.|.|.j.d...}
+00000f10: 097c 066a 0a7c 0869 007c 097c 0564 098d  .|.j.|.i.|.|.d..
+00000f20: 047d 0a7c 0a6a 0b64 006b 0990 0172 0674  .}.|.j.d.k...r.t
+00000f30: 0c7c 0a6a 0b83 0190 0172 067c 0a6a 0b64  .|.j.....r.|.j.d
+00000f40: 0a19 007d 0b74 0d7c 0b64 0b83 0272 dc7c  ...}.t.|.d...r.|
+00000f50: 0b6a 0e7d 0b74 0f7c 0b74 1083 0272 ea7c  .j.}.t.|.t...r.|
+00000f60: 0b82 0174 0564 0674 1187 0066 0164 0c64  ...t.d.t...f.d.d
+00000f70: 0d84 087c 0a6a 0b83 0269 0183 0153 0074  ...|.j...i...S.t
+00000f80: 0564 0e7c 0a6a 0369 0183 0153 0029 0f4e  .d.|.j.i...S.).N
+00000f90: 7242 0000 0046 da08 7661 6c69 6461 7465  rB...F..validate
+00000fa0: 54da 0571 7565 7279 da06 6572 726f 7273  T..query..errors
+00000fb0: 7a1e 4661 696c 6564 2074 6f20 6765 7420  z.Failed to get 
+00000fc0: 7461 626c 6520 7363 6865 6d61 3a20 7b7d  table schema: {}
+00000fd0: 2902 7210 0000 00da 0773 6573 7369 6f6e  ).r......session
+00000fe0: 2903 5a09 7661 7269 6162 6c65 73da 0d63  ).Z.variables..c
+00000ff0: 6f6e 7465 7874 5f76 616c 7565 7249 0000  ontext_valuerI..
+00001000: 0072 0100 0000 da0e 6f72 6967 696e 616c  .r......original
+00001010: 5f65 7272 6f72 6301 0000 0000 0000 0001  _errorc.........
+00001020: 0000 0003 0000 0013 0000 0073 0a00 0000  ...........s....
+00001030: 8800 a000 7c00 a101 5300 2901 4e29 0172  ....|...S.).N).r
+00001040: 1f00 0000 2901 da01 7829 0172 0f00 0000  ....)...x).r....
+00001050: 720e 0000 0072 1100 0000 da08 3c6c 616d  r....r......<lam
+00001060: 6264 613e a300 0000 f300 0000 007a 2247  bda>.........z"G
+00001070: 7261 7068 514c 5669 6577 2e70 6f73 742e  raphQLView.post.
+00001080: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00001090: 3eda 0464 6174 6129 1272 0b00 0000 da04  >..data).r......
+000010a0: 626f 6f6c da0c 6765 745f 6172 6775 6d65  bool..get_argume
+000010b0: 6e74 7252 0000 0072 1900 0000 7208 0000  ntrR...r....r...
+000010c0: 0072 3d00 0000 723f 0000 0072 2700 0000  .r=...r?...r'...
+000010d0: 724c 0000 00da 0765 7865 6375 7465 724b  rL.....executerK
+000010e0: 0000 00da 036c 656e da07 6861 7361 7474  .....len..hasatt
+000010f0: 7272 4e00 0000 721b 0000 0072 0500 0000  rrN...r....r....
+00001100: da03 6d61 7029 0c72 0f00 0000 7210 0000  ..map).r....r...
+00001110: 0072 3800 0000 7239 0000 0072 4200 0000  .r8...r9...rB...
+00001120: 7249 0000 0072 4300 0000 7244 0000 0072  rI...rC...rD...r
+00001130: 4a00 0000 724d 0000 00da 0672 6573 756c  J...rM.....resul
+00001140: 7472 1e00 0000 720e 0000 0029 0172 0f00  tr....r....).r..
+00001150: 0000 7211 0000 0072 4800 0000 8300 0000  ..r....rH.......
+00001160: 7334 0000 0000 0108 0210 0112 020a 0108  s4..............
+00001170: 0202 0110 0110 0122 020c 0202 010a 0204  ......."........
+00001180: 0102 0102 0102 0108 0318 010a 010a 0106  ................
+00001190: 010a 0104 011c 0202 017a 1047 7261 7068  .........z.Graph
+000011a0: 514c 5669 6577 2e70 6f73 744e 290e da08  QLView.postN)...
+000011b0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000011c0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000011d0: 5f5f 7207 0000 00da 1270 6572 6d69 7373  __r......permiss
+000011e0: 696f 6e5f 636c 6173 7365 7372 1200 0000  ion_classesr....
+000011f0: 721a 0000 0072 1f00 0000 722b 0000 0072  r....r....r+...r
+00001200: 3300 0000 7245 0000 0072 3d00 0000 7219  3...rE...r=...r.
+00001210: 0000 0072 4800 0000 720e 0000 0072 0e00  ...rH...r....r..
+00001220: 0000 720e 0000 0072 1100 0000 720d 0000  ..r....r....r...
+00001230: 0012 0000 0073 1400 0000 0801 0602 0803  .....s..........
+00001240: 0807 0806 0813 0805 0829 081a 0803 720d  .........)....r.
+00001250: 0000 0029 1972 3100 0000 723c 0000 00da  ...).r1...r<....
+00001260: 0864 6174 6574 696d 6572 0200 0000 5a07  .datetimer....Z.
+00001270: 6772 6170 6871 6c72 0300 0000 da12 6a65  graphqlr......je
+00001280: 745f 6272 6964 6765 5f62 6173 652e 6462  t_bridge_base.db
+00001290: 7204 0000 00da 2c6a 6574 5f62 7269 6467  r.....,jet_bridg
+000012a0: 655f 6261 7365 2e65 7863 6570 7469 6f6e  e_base.exception
+000012b0: 732e 7065 726d 6973 7369 6f6e 5f64 656e  s.permission_den
+000012c0: 6965 6472 0500 0000 da16 6a65 745f 6272  iedr......jet_br
+000012d0: 6964 6765 5f62 6173 652e 6c6f 6767 6572  idge_base.logger
+000012e0: 7206 0000 00da 1b6a 6574 5f62 7269 6467  r......jet_bridg
+000012f0: 655f 6261 7365 2e70 6572 6d69 7373 696f  e_base.permissio
+00001300: 6e73 7207 0000 00da 1e6a 6574 5f62 7269  nsr......jet_bri
+00001310: 6467 655f 6261 7365 2e72 6573 706f 6e73  dge_base.respons
+00001320: 6573 2e6a 736f 6e72 0800 0000 da1c 6a65  es.jsonr......je
+00001330: 745f 6272 6964 6765 5f62 6173 652e 7574  t_bridge_base.ut
+00001340: 696c 732e 636f 6d6d 6f6e 7209 0000 005a  ils.commonr....Z
+00001350: 1d6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
+00001360: 2e75 7469 6c73 2e67 7261 7068 716c 720a  .utils.graphqlr.
+00001370: 0000 005a 246a 6574 5f62 7269 6467 655f  ...Z$jet_bridge_
+00001380: 6261 7365 2e75 7469 6c73 2e74 7261 636b  base.utils.track
+00001390: 5f64 6174 6162 6173 6572 0b00 0000 da1e  _databaser......
+000013a0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+000013b0: 7669 6577 732e 6261 7365 2e61 7069 720c  views.base.apir.
+000013c0: 0000 0072 0d00 0000 720e 0000 0072 0e00  ...r....r....r..
+000013d0: 0000 720e 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+000013e0: 6f64 756c 653e 0100 0000 731a 0000 0008  odule>....s.....
+000013f0: 0108 010c 020c 020c 010c 010c 010c 010c  ................
+00001400: 010c 010c 010c 010c 03                   .........
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/sql.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/sql.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/sql.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/sql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/message.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/message.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/message.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table_column.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table_column.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/file_upload.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/file_upload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/reload.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/reload.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model_description.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 5673 f763 012f 0000 e300 0000  3...Vs.c./......
+00000000: 330d 0d0a 1b53 b564 902f 0000 e300 0000  3....S.d./......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 1c01 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6406 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
@@ -232,220 +232,224 @@
 00000e70: 0000 7265 0000 0072 6600 0000 7233 0000  ..re...rf...r3..
 00000e80: 0072 6700 0000 2902 da08 6f76 6572 7269  .rg...)...overri
 00000e90: 6465 7263 0000 0072 1d00 0000 721d 0000  derc...r....r...
 00000ea0: 0072 1e00 0000 da19 6d61 705f 7265 6c61  .r......map_rela
 00000eb0: 7469 6f6e 7368 6970 5f6f 7665 7272 6964  tionship_overrid
 00000ec0: 65b0 0000 0073 0c00 0000 0002 0401 0401  e....s..........
 00000ed0: 0401 0401 0a03 726f 0000 0063 0400 0000  ......ro...c....
-00000ee0: 0000 0000 1600 0000 1500 0000 0300 0000  ................
-00000ef0: 73aa 0100 0074 007c 0183 017d 047c 046a  s....t.|...}.|.j
+00000ee0: 0000 0000 1700 0000 1600 0000 0300 0000  ................
+00000ef0: 73c6 0100 0074 007c 0183 017d 047c 046a  s....t.|...}.|.j
 00000f00: 0164 0119 007d 0574 0288 006a 037c 0583  .d...}.t...j.|..
 00000f10: 027d 067c 046a 0464 0119 007d 077c 0564  .}.|.j.d...}.|.d
 00000f20: 006b 0972 3c74 057c 0564 0264 0383 036e  .k.r<t.|.d.d...n
-00000f30: 0264 007d 0867 0089 017c 026a 067c 0683  .d.}.g...|.j.|..
-00000f40: 017d 0964 0164 046c 076d 087d 0a01 007c  .}.d.d.l.m.}...|
-00000f50: 0a6a 097c 0683 017d 0b64 007d 0c64 007d  .j.|...}.d.}.d.}
-00000f60: 0d64 007d 0e64 007d 0f7c 056a 0a90 0172  .d.}.d.}.|.j...r
-00000f70: 0a79 7674 0b6a 0c7c 056a 0a83 017d 1074  .yvt.j.|.j...}.t
-00000f80: 0d7c 1074 0e83 0273 9874 0f82 017c 106a  .|.t...s.t...|.j
-00000f90: 0664 0583 017d 117c 106a 0664 0683 017d  .d...}.|.j.d...}
-00000fa0: 127c 106a 0664 0783 017d 137c 106a 0664  .|.j.d...}.|.j.d
-00000fb0: 0883 017d 147c 1164 006b 0972 cc7c 117d  ...}.|.d.k.r.|.}
-00000fc0: 0c7c 1264 006b 0972 d87c 127d 0d7c 1364  .|.d.k.r.|.}.|.d
-00000fd0: 006b 0972 e47c 137d 0e7c 1464 006b 0972  .k.r.|.}.|.d.k.r
-00000fe0: f07c 147d 0f57 006e 1604 0074 0f6b 0a90  .|.}.W.n...t.k..
-00000ff0: 0172 0801 0001 0001 0059 006e 0258 007c  .r.......Y.n.X.|
-00001000: 067c 0674 1074 1187 0087 0166 0264 0964  .|.t.t.....f.d.d
-00001010: 0a84 087c 046a 1283 0283 0174 1074 1187  ...|.j.....t.t..
-00001020: 0066 0164 0b64 0a84 0874 1364 0c64 0a84  .f.d.d...t.d.d..
-00001030: 007c 046a 1483 0283 0283 017c 0990 0172  .|.j.......|...r
-00001040: 5e74 1074 1164 0d64 0a84 007c 0983 0283  ^t.t.d.d...|....
-00001050: 016e 0264 007c 067c 036b 0690 0170 747c  .n.d.|.|.k...pt|
-00001060: 067c 0a6a 1583 006b 067c 0764 006b 0990  .|.j...k.|.d.k..
-00001070: 0172 847c 076a 166e 0264 007c 087c 0c7c  .r.|.j.n.d.|.|.|
-00001080: 0d7c 0e7c 0f64 0e9c 0c7d 157c 0b90 0172  .|.|.d...}.|...r
-00001090: a674 177c 157c 0b83 027d 157c 1553 0029  .t.|.|...}.|.S.)
-000010a0: 0f4e 7201 0000 00da 0f5f 5f6a 6574 5f61  .Nr......__jet_a
-000010b0: 7574 6f5f 706b 5f5f 4629 01da 0d63 6f6e  uto_pk__F)...con
-000010c0: 6669 6775 7261 7469 6f6e 7236 0000 005a  figurationr6...Z
-000010d0: 0b6e 616d 655f 706c 7572 616c 723d 0000  .name_pluralr=..
-000010e0: 0072 3e00 0000 6301 0000 0000 0000 0001  .r>...c.........
-000010f0: 0000 0005 0000 0013 0000 0073 1400 0000  ...........s....
-00001100: 7400 8800 6a01 7c00 7c00 6a02 8801 6b07  t...j.|.|.j...k.
-00001110: 8303 5300 2901 4e29 0372 6400 0000 725a  ..S.).N).rd...rZ
-00001120: 0000 0072 3600 0000 2901 7237 0000 0029  ...r6...).r7...)
-00001130: 02da 0a4d 6170 7065 6442 6173 65da 0c6e  ...MappedBase..n
-00001140: 6f6e 5f65 6469 7461 626c 6572 1d00 0000  on_editabler....
-00001150: 721e 0000 0072 3800 0000 1b01 0000 7300  r....r8.......s.
-00001160: 0000 007a 1b6d 6170 5f74 6162 6c65 2e3c  ...z.map_table.<
-00001170: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00001180: 6301 0000 0000 0000 0001 0000 0003 0000  c...............
-00001190: 0013 0000 0073 0c00 0000 7400 8800 6a01  .....s....t...j.
-000011a0: 7c00 8302 5300 2901 4e29 0272 6d00 0000  |...S.).N).rm...
-000011b0: 725a 0000 0029 0172 3700 0000 2901 7272  rZ...).r7...).rr
-000011c0: 0000 0072 1d00 0000 721e 0000 0072 3800  ...r....r....r8.
-000011d0: 0000 1c01 0000 7300 0000 0063 0100 0000  ......s....c....
-000011e0: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
-000011f0: 730e 0000 007c 006a 0074 0174 0267 026b  s....|.j.t.t.g.k
-00001200: 0653 0029 014e 2903 7265 0000 0072 0900  .S.).N).re...r..
-00001210: 0000 720a 0000 0029 0172 3700 0000 721d  ..r....).r7...r.
-00001220: 0000 0072 1d00 0000 721e 0000 0072 3800  ...r....r....r8.
-00001230: 0000 1c01 0000 7300 0000 0063 0100 0000  ......s....c....
-00001240: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
-00001250: 7308 0000 0074 007c 0083 0153 0029 014e  s....t.|...S.).N
-00001260: 2901 726f 0000 0029 0172 3700 0000 721d  ).ro...).r7...r.
-00001270: 0000 0072 1d00 0000 721e 0000 0072 3800  ...r....r....r8.
-00001280: 0000 1d01 0000 7300 0000 0029 0c72 3200  ......s....).r2.
-00001290: 0000 da08 6462 5f74 6162 6c65 da06 6669  ....db_table..fi
-000012a0: 656c 6473 da09 7265 6c61 7469 6f6e 735a  elds..relationsZ
-000012b0: 1272 656c 6174 696f 6e5f 6f76 6572 7269  .relation_overri
-000012c0: 6465 7372 3e00 0000 da11 7072 696d 6172  desr>.....primar
-000012d0: 795f 6b65 795f 6669 656c 64da 1070 7269  y_key_field..pri
-000012e0: 6d61 7279 5f6b 6579 5f61 7574 6f72 4400  mary_key_autorD.
-000012f0: 0000 da17 6461 7461 5f73 6f75 7263 655f  ....data_source_
-00001300: 6e61 6d65 5f70 6c75 7261 6c72 4600 0000  name_pluralrF...
-00001310: 7247 0000 0029 1872 0500 0000 da06 7461  rG...).r......ta
-00001320: 626c 6573 720e 0000 0072 5a00 0000 724e  blesr....rZ...rN
-00001330: 0000 00da 0767 6574 6174 7472 7259 0000  .....getattrrY..
-00001340: 005a 1d6a 6574 5f62 7269 6467 655f 6261  .Z.jet_bridge_ba
-00001350: 7365 2e63 6f6e 6669 6775 7261 7469 6f6e  se.configuration
-00001360: 7271 0000 00da 1567 6574 5f6d 6f64 656c  rq.....get_model
-00001370: 5f64 6573 6372 6970 7469 6f6e 7254 0000  _descriptionrT..
-00001380: 0072 5500 0000 7256 0000 0072 2900 0000  .rU...rV...r)...
-00001390: 7257 0000 0072 5800 0000 da04 6c69 7374  rW...rX.....list
-000013a0: 7252 0000 0072 4f00 0000 da06 6669 6c74  rR...rO.....filt
-000013b0: 6572 da0d 7265 6c61 7469 6f6e 7368 6970  er..relationship
-000013c0: 73da 1c67 6574 5f68 6964 6465 6e5f 6d6f  s..get_hidden_mo
-000013d0: 6465 6c5f 6465 7363 7269 7074 696f 6e72  del_descriptionr
-000013e0: 3600 0000 7213 0000 0029 1672 7200 0000  6...r....).rr...
-000013f0: da03 636c 73da 1772 656c 6174 696f 6e73  ..cls..relations
-00001400: 6869 7073 5f6f 7665 7272 6964 6573 723e  hips_overridesr>
-00001410: 0000 00da 066d 6170 7065 7272 4d00 0000  .....mapperrM...
-00001420: 7236 0000 0072 4e00 0000 7278 0000 00da  r6...rN...rx....
-00001430: 1d6d 6f64 656c 5f72 656c 6174 696f 6e73  .model_relations
-00001440: 6869 7073 5f6f 7665 7272 6964 6573 7271  hips_overridesrq
-00001450: 0000 00da 0a61 6464 6974 696f 6e61 6c72  .....additionalr
-00001460: 4400 0000 7279 0000 0072 4600 0000 7247  D...ry...rF...rG
-00001470: 0000 0072 5f00 0000 7260 0000 005a 106d  ...r_...r`...Z.m
-00001480: 6574 615f 6e61 6d65 5f70 6c75 7261 6c72  eta_name_pluralr
-00001490: 6100 0000 7262 0000 0072 6300 0000 721d  a...rb...rc...r.
-000014a0: 0000 0029 0272 7200 0000 7273 0000 0072  ...).rr...rs...r
-000014b0: 1e00 0000 da09 6d61 705f 7461 626c 65f0  ......map_table.
-000014c0: 0000 0073 5e00 0000 0001 0801 0a01 0c01  ...s^...........
-000014d0: 0a01 1801 0401 0a02 0c01 0a02 0401 0401  ................
-000014e0: 0401 0402 0801 0201 0c02 0a01 0402 0a01  ................
-000014f0: 0a01 0a01 0a02 0801 0401 0801 0401 0801  ................
-00001500: 0401 0801 0801 1001 0603 0201 0201 1801  ................
-00001510: 2001 1a01 1402 1201 0201 0201 0201 0201   ...............
-00001520: 0803 0601 0a02 7286 0000 0063 0000 0000  ......r....c....
-00001530: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00001540: 7326 0000 0065 005a 0164 005a 0265 035a  s&...e.Z.d.Z.e.Z
-00001550: 0465 0566 015a 0664 0164 0284 005a 0764  .e.f.Z.d.d...Z.d
-00001560: 0364 0484 005a 0864 0553 0029 06da 144d  .d...Z.d.S.)...M
-00001570: 6f64 656c 4465 7363 7269 7074 696f 6e56  odelDescriptionV
-00001580: 6965 7763 0200 0000 0000 0000 0700 0000  iewc............
-00001590: 0c00 0000 0300 0000 73b8 0000 0064 0167  ........s....d.g
-000015a0: 0189 0174 007c 0183 0189 0069 0089 0274  ...t.|.....i...t
-000015b0: 017c 016a 0264 0264 0383 0283 017d 0274  .|.j.d.d.....}.t
-000015c0: 036a 0483 0072 9c74 057c 0183 017d 0374  .j...r.t.|...}.t
-000015d0: 036a 0683 008f 5c7d 047c 046a 0774 0883  .j....\}.|.j.t..
-000015e0: 016a 0974 086a 0a7c 0364 0419 006b 027c  .j.t.j.|.d...k.|
-000015f0: 027c 026b 0283 026a 0b83 007d 0578 307c  .|.k...j...}.x0|
-00001600: 0544 005d 287d 067c 066a 0c88 026b 0772  .D.](}.|.j...k.r
-00001610: 7e67 0088 027c 066a 0c3c 0088 027c 066a  ~g...|.j.<...|.j
-00001620: 0c19 006a 0d7c 0683 0101 0071 6657 0057  ...j.|.....qfW.W
-00001630: 0064 0051 0052 0058 0074 0e74 0f87 0087  .d.Q.R.X.t.t....
-00001640: 0187 0266 0364 0564 0684 0888 006a 1083  ...f.d.d.....j..
-00001650: 0283 0153 0029 074e 5a0c 5f5f 6a65 745f  ...S.).NZ.__jet_
-00001660: 5f74 6f6b 656e da05 6472 6166 7446 da02  _token..draftF..
-00001670: 6964 6301 0000 0000 0000 0001 0000 0005  idc.............
-00001680: 0000 0013 0000 0073 0e00 0000 7400 8800  .......s....t...
-00001690: 7c00 8802 8801 8304 5300 2901 4e29 0172  |.......S.).N).r
-000016a0: 8600 0000 2901 7237 0000 0029 0372 7200  ....).r7...).rr.
-000016b0: 0000 723e 0000 0072 8200 0000 721d 0000  ..r>...r....r...
-000016c0: 0072 1e00 0000 7238 0000 0046 0100 0073  .r....r8...F...s
-000016d0: 0000 0000 7a33 4d6f 6465 6c44 6573 6372  ....z3ModelDescr
-000016e0: 6970 7469 6f6e 5669 6577 2e67 6574 5f71  iptionView.get_q
-000016f0: 7565 7279 7365 742e 3c6c 6f63 616c 733e  ueryset.<locals>
-00001700: 2e3c 6c61 6d62 6461 3e29 1172 0c00 0000  .<lambda>).r....
-00001710: da04 626f 6f6c da0c 6765 745f 6172 6775  ..bool..get_argu
-00001720: 6d65 6e74 7203 0000 00da 0569 735f 6f6b  mentr......is_ok
-00001730: 720d 0000 00da 0773 6573 7369 6f6e da05  r......session..
-00001740: 7175 6572 7972 0200 0000 727e 0000 00da  queryr....r~....
-00001750: 0d63 6f6e 6e65 6374 696f 6e5f 6964 da03  .connection_id..
-00001760: 616c 6c72 3200 0000 da06 6170 7065 6e64  allr2.....append
-00001770: 727d 0000 0072 5200 0000 da07 636c 6173  r}...rR.....clas
-00001780: 7365 7329 07da 0473 656c 66da 0772 6571  ses)...self..req
-00001790: 7565 7374 7288 0000 00da 0a63 6f6e 6e65  uestr......conne
-000017a0: 6374 696f 6e72 8d00 0000 da09 6f76 6572  ctionr......over
-000017b0: 7269 6465 7372 6e00 0000 721d 0000 0029  ridesrn...r....)
-000017c0: 0372 7200 0000 723e 0000 0072 8200 0000  .rr...r>...r....
-000017d0: 721e 0000 00da 0c67 6574 5f71 7565 7279  r......get_query
-000017e0: 7365 7432 0100 0073 1e00 0000 0001 0601  set2...s........
-000017f0: 0801 0401 1002 0801 0802 0a01 0a01 0c01  ................
-00001800: 0e03 0a01 0a01 0a01 1e02 7a21 4d6f 6465  ..........z!Mode
-00001810: 6c44 6573 6372 6970 7469 6f6e 5669 6577  lDescriptionView
-00001820: 2e67 6574 5f71 7565 7279 7365 7463 0200  .get_querysetc..
-00001830: 0000 0000 0000 0600 0000 0400 0000 4f00  ..............O.
-00001840: 0000 7322 0000 007c 006a 007c 0183 017d  ..s"...|.j.|...}
-00001850: 047c 006a 017c 0464 0164 028d 027d 0574  .|.j.|.d.d...}.t
-00001860: 027c 056a 0383 0153 0029 034e 5429 02da  .|.j...S.).NT)..
-00001870: 0869 6e73 7461 6e63 65da 046d 616e 7929  .instance..many)
-00001880: 0472 9700 0000 da10 7365 7269 616c 697a  .r......serializ
-00001890: 6572 5f63 6c61 7373 7211 0000 00da 1372  er_classr......r
-000018a0: 6570 7265 7365 6e74 6174 696f 6e5f 6461  epresentation_da
-000018b0: 7461 2906 7293 0000 0072 9400 0000 da04  ta).r....r......
-000018c0: 6172 6773 da06 6b77 6172 6773 da08 7175  args..kwargs..qu
-000018d0: 6572 7973 6574 da0a 7365 7269 616c 697a  eryset..serializ
-000018e0: 6572 721d 0000 0072 1d00 0000 721e 0000  err....r....r...
-000018f0: 0072 5900 0000 4801 0000 7306 0000 0000  .rY...H...s.....
-00001900: 010a 010e 017a 184d 6f64 656c 4465 7363  .....z.ModelDesc
-00001910: 7269 7074 696f 6e56 6965 772e 6765 744e  riptionView.getN
-00001920: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00001930: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00001940: 6e61 6d65 5f5f 7212 0000 0072 9a00 0000  name__r....r....
-00001950: 7210 0000 00da 1270 6572 6d69 7373 696f  r......permissio
-00001960: 6e5f 636c 6173 7365 7372 9700 0000 7259  n_classesr....rY
-00001970: 0000 0072 1d00 0000 721d 0000 0072 1d00  ...r....r....r..
-00001980: 0000 721e 0000 0072 8700 0000 2e01 0000  ..r....r........
-00001990: 7308 0000 0008 0104 0106 0208 1672 8700  s............r..
-000019a0: 0000 292d 7255 0000 0072 2c00 0000 5a2e  ..)-rU...r,...Z.
-000019b0: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
-000019c0: 6d6f 6465 6c73 2e6d 6f64 656c 5f72 656c  models.model_rel
-000019d0: 6174 696f 6e5f 6f76 6572 7269 6465 7202  ation_overrider.
-000019e0: 0000 00da 156a 6574 5f62 7269 6467 655f  .....jet_bridge_
-000019f0: 6261 7365 2e73 746f 7265 7203 0000 00da  base.storer.....
-00001a00: 1f6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00001a10: 2e75 7469 6c73 2e72 656c 6174 696f 6e73  .utils.relations
-00001a20: 7204 0000 00da 0a73 716c 616c 6368 656d  r......sqlalchem
-00001a30: 7972 0500 0000 7206 0000 0072 0700 0000  yr....r....r....
-00001a40: 7208 0000 00da 0e73 716c 616c 6368 656d  r......sqlalchem
-00001a50: 792e 6f72 6d72 0900 0000 720a 0000 005a  y.ormr....r....Z
-00001a60: 1773 716c 616c 6368 656d 792e 7371 6c2e  .sqlalchemy.sql.
-00001a70: 656c 656d 656e 7473 720b 0000 00da 126a  elementsr......j
-00001a80: 6574 5f62 7269 6467 655f 6261 7365 2e64  et_bridge_base.d
-00001a90: 6272 0c00 0000 720d 0000 0072 0e00 0000  br....r....r....
-00001aa0: da16 6a65 745f 6272 6964 6765 5f62 6173  ..jet_bridge_bas
-00001ab0: 652e 6d6f 6465 6c73 720f 0000 00da 1b6a  e.modelsr......j
-00001ac0: 6574 5f62 7269 6467 655f 6261 7365 2e70  et_bridge_base.p
-00001ad0: 6572 6d69 7373 696f 6e73 7210 0000 00da  ermissionsr.....
-00001ae0: 1e6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00001af0: 2e72 6573 706f 6e73 6573 2e6a 736f 6e72  .responses.jsonr
-00001b00: 1100 0000 5a2d 6a65 745f 6272 6964 6765  ....Z-jet_bridge
-00001b10: 5f62 6173 652e 7365 7269 616c 697a 6572  _base.serializer
-00001b20: 732e 6d6f 6465 6c5f 6465 7363 7269 7074  s.model_descript
-00001b30: 696f 6e72 1200 0000 da1c 6a65 745f 6272  ionr......jet_br
-00001b40: 6964 6765 5f62 6173 652e 7574 696c 732e  idge_base.utils.
-00001b50: 636f 6d6d 6f6e 7213 0000 0072 1400 0000  commonr....r....
-00001b60: da1e 6a65 745f 6272 6964 6765 5f62 6173  ..jet_bridge_bas
-00001b70: 652e 7574 696c 732e 6462 5f74 7970 6573  e.utils.db_types
-00001b80: 7215 0000 0072 1600 0000 da1e 6a65 745f  r....r......jet_
-00001b90: 6272 6964 6765 5f62 6173 652e 7669 6577  bridge_base.view
-00001ba0: 732e 6261 7365 2e61 7069 7217 0000 0072  s.base.apir....r
-00001bb0: 1f00 0000 7230 0000 0072 6400 0000 726d  ....r0...rd...rm
-00001bc0: 0000 0072 6f00 0000 7286 0000 0072 8700  ...ro...r....r..
-00001bd0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00001be0: 0072 1e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001bf0: 0100 0000 732c 0000 0008 0108 020c 010c  ....s,..........
-00001c00: 010c 0118 0110 010c 0214 010c 010c 010c  ................
-00001c10: 010c 0110 0110 010c 0308 0408 2808 5f08  ............(._.
-00001c20: 1008 4008 3e                             ..@.>
+00000f30: 0264 007d 087c 0564 006b 0972 5474 057c  .d.}.|.d.k.rTt.|
+00000f40: 0564 0464 0383 036e 0264 037d 0967 0089  .d.d...n.d.}.g..
+00000f50: 017c 026a 067c 0683 017d 0a64 0164 056c  .|.j.|...}.d.d.l
+00000f60: 076d 087d 0b01 007c 0b6a 097c 0683 017d  .m.}...|.j.|...}
+00000f70: 0c64 007d 0d64 007d 0e64 007d 0f64 007d  .d.}.d.}.d.}.d.}
+00000f80: 107c 056a 0a90 0172 2479 7874 0b6a 0c7c  .|.j...r$yxt.j.|
+00000f90: 056a 0a83 017d 1174 0d7c 1174 0e83 0273  .j...}.t.|.t...s
+00000fa0: b074 0f82 017c 116a 0664 0683 017d 127c  .t...|.j.d...}.|
+00000fb0: 116a 0664 0783 017d 137c 116a 0664 0883  .j.d...}.|.j.d..
+00000fc0: 017d 147c 116a 0664 0983 017d 157c 1264  .}.|.j.d...}.|.d
+00000fd0: 006b 0972 e47c 127d 0d7c 1364 006b 0972  .k.r.|.}.|.d.k.r
+00000fe0: f07c 137d 0e7c 1464 006b 0972 fc7c 147d  .|.}.|.d.k.r.|.}
+00000ff0: 0f7c 1564 006b 0990 0172 0a7c 157d 1057  .|.d.k...r.|.}.W
+00001000: 006e 1604 0074 0f6b 0a90 0172 2201 0001  .n...t.k...r"...
+00001010: 0001 0059 006e 0258 007c 067c 0674 1074  ...Y.n.X.|.|.t.t
+00001020: 1187 0087 0166 0264 0a64 0b84 087c 046a  .....f.d.d...|.j
+00001030: 1283 0283 0174 1074 1187 0066 0164 0c64  .....t.t...f.d.d
+00001040: 0b84 0874 1364 0d64 0b84 007c 046a 1483  ...t.d.d...|.j..
+00001050: 0283 0283 017c 0a90 0172 7874 1074 1164  .....|...rxt.t.d
+00001060: 0e64 0b84 007c 0a83 0283 016e 0264 007c  .d...|.....n.d.|
+00001070: 067c 036b 0690 0170 8e7c 067c 0b6a 1583  .|.k...p.|.|.j..
+00001080: 006b 067c 0764 006b 0990 0172 9e7c 076a  .k.|.d.k...r.|.j
+00001090: 166e 0264 007c 087c 097c 0d7c 0e7c 0f7c  .n.d.|.|.|.|.|.|
+000010a0: 1064 0f9c 0d7d 167c 0c90 0172 c274 177c  .d...}.|...r.t.|
+000010b0: 167c 0c83 027d 167c 1653 0029 104e 7201  .|...}.|.S.).Nr.
+000010c0: 0000 00da 0f5f 5f6a 6574 5f61 7574 6f5f  .....__jet_auto_
+000010d0: 706b 5f5f 46da 0f5f 5f6a 6574 5f69 735f  pk__F..__jet_is_
+000010e0: 7669 6577 5f5f 2901 da0d 636f 6e66 6967  view__)...config
+000010f0: 7572 6174 696f 6e72 3600 0000 5a0b 6e61  urationr6...Z.na
+00001100: 6d65 5f70 6c75 7261 6c72 3d00 0000 723e  me_pluralr=...r>
+00001110: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
+00001120: 0500 0000 1300 0000 7314 0000 0074 0088  ........s....t..
+00001130: 006a 017c 007c 006a 0288 016b 0783 0353  .j.|.|.j...k...S
+00001140: 0029 014e 2903 7264 0000 0072 5a00 0000  .).N).rd...rZ...
+00001150: 7236 0000 0029 0172 3700 0000 2902 da0a  r6...).r7...)...
+00001160: 4d61 7070 6564 4261 7365 da0c 6e6f 6e5f  MappedBase..non_
+00001170: 6564 6974 6162 6c65 721d 0000 0072 1e00  editabler....r..
+00001180: 0000 7238 0000 001c 0100 0073 0000 0000  ..r8.......s....
+00001190: 7a1b 6d61 705f 7461 626c 652e 3c6c 6f63  z.map_table.<loc
+000011a0: 616c 733e 2e3c 6c61 6d62 6461 3e63 0100  als>.<lambda>c..
+000011b0: 0000 0000 0000 0100 0000 0300 0000 1300  ................
+000011c0: 0000 730c 0000 0074 0088 006a 017c 0083  ..s....t...j.|..
+000011d0: 0253 0029 014e 2902 726d 0000 0072 5a00  .S.).N).rm...rZ.
+000011e0: 0000 2901 7237 0000 0029 0172 7300 0000  ..).r7...).rs...
+000011f0: 721d 0000 0072 1e00 0000 7238 0000 001d  r....r....r8....
+00001200: 0100 0073 0000 0000 6301 0000 0000 0000  ...s....c.......
+00001210: 0001 0000 0003 0000 0053 0000 0073 0e00  .........S...s..
+00001220: 0000 7c00 6a00 7401 7402 6702 6b06 5300  ..|.j.t.t.g.k.S.
+00001230: 2901 4e29 0372 6500 0000 7209 0000 0072  ).N).re...r....r
+00001240: 0a00 0000 2901 7237 0000 0072 1d00 0000  ....).r7...r....
+00001250: 721d 0000 0072 1e00 0000 7238 0000 001d  r....r....r8....
+00001260: 0100 0073 0000 0000 6301 0000 0000 0000  ...s....c.......
+00001270: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
+00001280: 0000 7400 7c00 8301 5300 2901 4e29 0172  ..t.|...S.).N).r
+00001290: 6f00 0000 2901 7237 0000 0072 1d00 0000  o...).r7...r....
+000012a0: 721d 0000 0072 1e00 0000 7238 0000 001e  r....r....r8....
+000012b0: 0100 0073 0000 0000 290d 7232 0000 00da  ...s....).r2....
+000012c0: 0864 625f 7461 626c 65da 0666 6965 6c64  .db_table..field
+000012d0: 73da 0972 656c 6174 696f 6e73 5a12 7265  s..relationsZ.re
+000012e0: 6c61 7469 6f6e 5f6f 7665 7272 6964 6573  lation_overrides
+000012f0: 723e 0000 00da 1170 7269 6d61 7279 5f6b  r>.....primary_k
+00001300: 6579 5f66 6965 6c64 da10 7072 696d 6172  ey_field..primar
+00001310: 795f 6b65 795f 6175 746f da07 6973 5f76  y_key_auto..is_v
+00001320: 6965 7772 4400 0000 da17 6461 7461 5f73  iewrD.....data_s
+00001330: 6f75 7263 655f 6e61 6d65 5f70 6c75 7261  ource_name_plura
+00001340: 6c72 4600 0000 7247 0000 0029 1872 0500  lrF...rG...).r..
+00001350: 0000 da06 7461 626c 6573 720e 0000 0072  ....tablesr....r
+00001360: 5a00 0000 724e 0000 00da 0767 6574 6174  Z...rN.....getat
+00001370: 7472 7259 0000 005a 1d6a 6574 5f62 7269  trrY...Z.jet_bri
+00001380: 6467 655f 6261 7365 2e63 6f6e 6669 6775  dge_base.configu
+00001390: 7261 7469 6f6e 7272 0000 00da 1567 6574  rationrr.....get
+000013a0: 5f6d 6f64 656c 5f64 6573 6372 6970 7469  _model_descripti
+000013b0: 6f6e 7254 0000 0072 5500 0000 7256 0000  onrT...rU...rV..
+000013c0: 0072 2900 0000 7257 0000 0072 5800 0000  .r)...rW...rX...
+000013d0: da04 6c69 7374 7252 0000 0072 4f00 0000  ..listrR...rO...
+000013e0: da06 6669 6c74 6572 da0d 7265 6c61 7469  ..filter..relati
+000013f0: 6f6e 7368 6970 73da 1c67 6574 5f68 6964  onships..get_hid
+00001400: 6465 6e5f 6d6f 6465 6c5f 6465 7363 7269  den_model_descri
+00001410: 7074 696f 6e72 3600 0000 7213 0000 0029  ptionr6...r....)
+00001420: 1772 7300 0000 da03 636c 73da 1772 656c  .rs.....cls..rel
+00001430: 6174 696f 6e73 6869 7073 5f6f 7665 7272  ationships_overr
+00001440: 6964 6573 723e 0000 00da 066d 6170 7065  idesr>.....mappe
+00001450: 7272 4d00 0000 7236 0000 0072 4e00 0000  rrM...r6...rN...
+00001460: 7279 0000 0072 7a00 0000 da1d 6d6f 6465  ry...rz.....mode
+00001470: 6c5f 7265 6c61 7469 6f6e 7368 6970 735f  l_relationships_
+00001480: 6f76 6572 7269 6465 7372 7200 0000 da0a  overridesrr.....
+00001490: 6164 6469 7469 6f6e 616c 7244 0000 0072  additionalrD...r
+000014a0: 7b00 0000 7246 0000 0072 4700 0000 725f  {...rF...rG...r_
+000014b0: 0000 0072 6000 0000 5a10 6d65 7461 5f6e  ...r`...Z.meta_n
+000014c0: 616d 655f 706c 7572 616c 7261 0000 0072  ame_pluralra...r
+000014d0: 6200 0000 7263 0000 0072 1d00 0000 2902  b...rc...r....).
+000014e0: 7273 0000 0072 7400 0000 721e 0000 00da  rs...rt...r.....
+000014f0: 096d 6170 5f74 6162 6c65 f000 0000 7362  .map_table....sb
+00001500: 0000 0000 0108 010a 010c 010a 0118 0118  ................
+00001510: 0104 010a 020c 010a 0204 0104 0104 0104  ................
+00001520: 0208 0102 010c 020a 0104 020a 010a 010a  ................
+00001530: 010a 0208 0104 0108 0104 0108 0104 010a  ................
+00001540: 0108 0110 0106 0302 0102 0118 0120 011a  ............. ..
+00001550: 0114 0212 0102 0102 0102 0102 0102 0108  ................
+00001560: 0306 010a 0272 8800 0000 6300 0000 0000  .....r....c.....
+00001570: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00001580: 2600 0000 6500 5a01 6400 5a02 6503 5a04  &...e.Z.d.Z.e.Z.
+00001590: 6505 6601 5a06 6401 6402 8400 5a07 6403  e.f.Z.d.d...Z.d.
+000015a0: 6404 8400 5a08 6405 5300 2906 da14 4d6f  d...Z.d.S.)...Mo
+000015b0: 6465 6c44 6573 6372 6970 7469 6f6e 5669  delDescriptionVi
+000015c0: 6577 6302 0000 0000 0000 0007 0000 000c  ewc.............
+000015d0: 0000 0003 0000 0073 b800 0000 6401 6701  .......s....d.g.
+000015e0: 8901 7400 7c01 8301 8900 6900 8902 7401  ..t.|.....i...t.
+000015f0: 7c01 6a02 6402 6403 8302 8301 7d02 7403  |.j.d.d.....}.t.
+00001600: 6a04 8300 729c 7405 7c01 8301 7d03 7403  j...r.t.|...}.t.
+00001610: 6a06 8300 8f5c 7d04 7c04 6a07 7408 8301  j....\}.|.j.t...
+00001620: 6a09 7408 6a0a 7c03 6404 1900 6b02 7c02  j.t.j.|.d...k.|.
+00001630: 7c02 6b02 8302 6a0b 8300 7d05 7830 7c05  |.k...j...}.x0|.
+00001640: 4400 5d28 7d06 7c06 6a0c 8802 6b07 727e  D.](}.|.j...k.r~
+00001650: 6700 8802 7c06 6a0c 3c00 8802 7c06 6a0c  g...|.j.<...|.j.
+00001660: 1900 6a0d 7c06 8301 0100 7166 5700 5700  ..j.|.....qfW.W.
+00001670: 6400 5100 5200 5800 740e 740f 8700 8701  d.Q.R.X.t.t.....
+00001680: 8702 6603 6405 6406 8408 8800 6a10 8302  ..f.d.d.....j...
+00001690: 8301 5300 2907 4e5a 0c5f 5f6a 6574 5f5f  ..S.).NZ.__jet__
+000016a0: 746f 6b65 6eda 0564 7261 6674 46da 0269  token..draftF..i
+000016b0: 6463 0100 0000 0000 0000 0100 0000 0500  dc..............
+000016c0: 0000 1300 0000 730e 0000 0074 0088 007c  ......s....t...|
+000016d0: 0088 0288 0183 0453 0029 014e 2901 7288  .......S.).N).r.
+000016e0: 0000 0029 0172 3700 0000 2903 7273 0000  ...).r7...).rs..
+000016f0: 0072 3e00 0000 7284 0000 0072 1d00 0000  .r>...r....r....
+00001700: 721e 0000 0072 3800 0000 4801 0000 7300  r....r8...H...s.
+00001710: 0000 007a 334d 6f64 656c 4465 7363 7269  ...z3ModelDescri
+00001720: 7074 696f 6e56 6965 772e 6765 745f 7175  ptionView.get_qu
+00001730: 6572 7973 6574 2e3c 6c6f 6361 6c73 3e2e  eryset.<locals>.
+00001740: 3c6c 616d 6264 613e 2911 720c 0000 00da  <lambda>).r.....
+00001750: 0462 6f6f 6cda 0c67 6574 5f61 7267 756d  .bool..get_argum
+00001760: 656e 7472 0300 0000 da05 6973 5f6f 6b72  entr......is_okr
+00001770: 0d00 0000 da07 7365 7373 696f 6eda 0571  ......session..q
+00001780: 7565 7279 7202 0000 0072 8000 0000 da0d  ueryr....r......
+00001790: 636f 6e6e 6563 7469 6f6e 5f69 64da 0361  connection_id..a
+000017a0: 6c6c 7232 0000 00da 0661 7070 656e 6472  llr2.....appendr
+000017b0: 7f00 0000 7252 0000 00da 0763 6c61 7373  ....rR.....class
+000017c0: 6573 2907 da04 7365 6c66 da07 7265 7175  es)...self..requ
+000017d0: 6573 7472 8a00 0000 da0a 636f 6e6e 6563  estr......connec
+000017e0: 7469 6f6e 728f 0000 00da 096f 7665 7272  tionr......overr
+000017f0: 6964 6573 726e 0000 0072 1d00 0000 2903  idesrn...r....).
+00001800: 7273 0000 0072 3e00 0000 7284 0000 0072  rs...r>...r....r
+00001810: 1e00 0000 da0c 6765 745f 7175 6572 7973  ......get_querys
+00001820: 6574 3401 0000 731e 0000 0000 0106 0108  et4...s.........
+00001830: 0104 0110 0208 0108 020a 010a 010c 010e  ................
+00001840: 030a 010a 010a 011e 027a 214d 6f64 656c  .........z!Model
+00001850: 4465 7363 7269 7074 696f 6e56 6965 772e  DescriptionView.
+00001860: 6765 745f 7175 6572 7973 6574 6302 0000  get_querysetc...
+00001870: 0000 0000 0006 0000 0004 0000 004f 0000  .............O..
+00001880: 0073 2200 0000 7c00 6a00 7c01 8301 7d04  .s"...|.j.|...}.
+00001890: 7c00 6a01 7c04 6401 6402 8d02 7d05 7402  |.j.|.d.d...}.t.
+000018a0: 7c05 6a03 8301 5300 2903 4e54 2902 da08  |.j...S.).NT)...
+000018b0: 696e 7374 616e 6365 da04 6d61 6e79 2904  instance..many).
+000018c0: 7299 0000 00da 1073 6572 6961 6c69 7a65  r......serialize
+000018d0: 725f 636c 6173 7372 1100 0000 da13 7265  r_classr......re
+000018e0: 7072 6573 656e 7461 7469 6f6e 5f64 6174  presentation_dat
+000018f0: 6129 0672 9500 0000 7296 0000 00da 0461  a).r....r......a
+00001900: 7267 73da 066b 7761 7267 73da 0871 7565  rgs..kwargs..que
+00001910: 7279 7365 74da 0a73 6572 6961 6c69 7a65  ryset..serialize
+00001920: 7272 1d00 0000 721d 0000 0072 1e00 0000  rr....r....r....
+00001930: 7259 0000 004a 0100 0073 0600 0000 0001  rY...J...s......
+00001940: 0a01 0e01 7a18 4d6f 6465 6c44 6573 6372  ....z.ModelDescr
+00001950: 6970 7469 6f6e 5669 6577 2e67 6574 4e29  iptionView.getN)
+00001960: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00001970: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001980: 616d 655f 5f72 1200 0000 729c 0000 0072  ame__r....r....r
+00001990: 1000 0000 da12 7065 726d 6973 7369 6f6e  ......permission
+000019a0: 5f63 6c61 7373 6573 7299 0000 0072 5900  _classesr....rY.
+000019b0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
+000019c0: 0072 1e00 0000 7289 0000 0030 0100 0073  .r....r....0...s
+000019d0: 0800 0000 0801 0401 0602 0816 7289 0000  ............r...
+000019e0: 0029 2d72 5500 0000 722c 0000 005a 2e6a  .)-rU...r,...Z.j
+000019f0: 6574 5f62 7269 6467 655f 6261 7365 2e6d  et_bridge_base.m
+00001a00: 6f64 656c 732e 6d6f 6465 6c5f 7265 6c61  odels.model_rela
+00001a10: 7469 6f6e 5f6f 7665 7272 6964 6572 0200  tion_overrider..
+00001a20: 0000 da15 6a65 745f 6272 6964 6765 5f62  ....jet_bridge_b
+00001a30: 6173 652e 7374 6f72 6572 0300 0000 da1f  ase.storer......
+00001a40: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+00001a50: 7574 696c 732e 7265 6c61 7469 6f6e 7372  utils.relationsr
+00001a60: 0400 0000 da0a 7371 6c61 6c63 6865 6d79  ......sqlalchemy
+00001a70: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00001a80: 0800 0000 da0e 7371 6c61 6c63 6865 6d79  ......sqlalchemy
+00001a90: 2e6f 726d 7209 0000 0072 0a00 0000 5a17  .ormr....r....Z.
+00001aa0: 7371 6c61 6c63 6865 6d79 2e73 716c 2e65  sqlalchemy.sql.e
+00001ab0: 6c65 6d65 6e74 7372 0b00 0000 da12 6a65  lementsr......je
+00001ac0: 745f 6272 6964 6765 5f62 6173 652e 6462  t_bridge_base.db
+00001ad0: 720c 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00001ae0: 166a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
+00001af0: 2e6d 6f64 656c 7372 0f00 0000 da1b 6a65  .modelsr......je
+00001b00: 745f 6272 6964 6765 5f62 6173 652e 7065  t_bridge_base.pe
+00001b10: 726d 6973 7369 6f6e 7372 1000 0000 da1e  rmissionsr......
+00001b20: 6a65 745f 6272 6964 6765 5f62 6173 652e  jet_bridge_base.
+00001b30: 7265 7370 6f6e 7365 732e 6a73 6f6e 7211  responses.jsonr.
+00001b40: 0000 005a 2d6a 6574 5f62 7269 6467 655f  ...Z-jet_bridge_
+00001b50: 6261 7365 2e73 6572 6961 6c69 7a65 7273  base.serializers
+00001b60: 2e6d 6f64 656c 5f64 6573 6372 6970 7469  .model_descripti
+00001b70: 6f6e 7212 0000 00da 1c6a 6574 5f62 7269  onr......jet_bri
+00001b80: 6467 655f 6261 7365 2e75 7469 6c73 2e63  dge_base.utils.c
+00001b90: 6f6d 6d6f 6e72 1300 0000 7214 0000 00da  ommonr....r.....
+00001ba0: 1e6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
+00001bb0: 2e75 7469 6c73 2e64 625f 7479 7065 7372  .utils.db_typesr
+00001bc0: 1500 0000 7216 0000 00da 1e6a 6574 5f62  ....r......jet_b
+00001bd0: 7269 6467 655f 6261 7365 2e76 6965 7773  ridge_base.views
+00001be0: 2e62 6173 652e 6170 6972 1700 0000 721f  .base.apir....r.
+00001bf0: 0000 0072 3000 0000 7264 0000 0072 6d00  ...r0...rd...rm.
+00001c00: 0000 726f 0000 0072 8800 0000 7289 0000  ..ro...r....r...
+00001c10: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+00001c20: 721e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001c30: 0000 0073 2c00 0000 0801 0802 0c01 0c01  ...s,...........
+00001c40: 0c01 1801 1001 0c02 1401 0c01 0c01 0c01  ................
+00001c50: 0c01 1001 1001 0c03 0804 0828 085f 0810  ...........(._..
+00001c60: 0840 0840                                .@.@
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/image_resize.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/image_resize.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/trigger_exception.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/trigger_exception.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table_column.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table_column.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/graphql.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/graphql.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/table.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/api.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/api.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 76b0 eb63 1d02 0000 e300 0000  3...v..c........
+00000000: 330d 0d0a a56f c364 1d02 0000 e300 0000  3....o.d........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 4400 0000 6400 6401 6c00 6d01 5a01  .sD...d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6507 8303 5a08 6407 5300 2908 e900 0000  e...Z.d.S.).....
 00000070: 0029 01da 0d63 6f6e 6669 6775 7261 7469  .)...configurati
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/proxy_request.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/proxy_request.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model_description.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/__pycache__/model_description_relationship_override.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/model.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/model.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/api.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/api.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/table_column.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/table_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 
 def map_dto_column(table_name, column, metadata):
     args = []
     column_kwargs = {}
     autoincrement = False
     server_default = None
-    column_type = db_to_sql_type(column['db_field']) if 'db_field' in column else map_to_sql_type(column['field'])
+    db_type = column.get('db_field')
+    map_type = column.get('field')
+    column_type = db_to_sql_type(db_type) if db_type else map_to_sql_type(map_type)
 
     if column.get('primary_key', False):
         autoincrement = True
 
     if 'default_type' in column:
         if column['default_type'] == 'value':
             server_default = column['default_value']
@@ -43,14 +45,21 @@
             autoincrement = True
 
     params = column.get('params')
     if params:
         if 'length' in params:
             column_kwargs['length'] = params['length']
 
+    try:
+        from geoalchemy2 import types
+        if column_type is types.Geography:
+            column_kwargs['geometry_type'] = 'POINT'
+    except ImportError:
+        pass
+
     if callable(column_type):
         try:
             column_type = column_type(**column_kwargs)
         except TypeError:
             pass
 
     if params:
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/image_resize.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/image_resize.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/model_description.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/model_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,21 @@
 
     if isinstance(column.type, Enum):
         params['options'] = map(lambda x: {'name': x, 'value': x}, column.type.enums)
 
     if isinstance(column.type, String):
         params['length'] = column.type.length
 
+    try:
+        from geoalchemy2 import types
+        if isinstance(column.type, types.Geography):
+            params['output_format'] = 'postgresql'
+    except ImportError:
+        pass
+
     optional = is_column_optional(column)
 
     if column.comment:
         try:
             data_source_meta = json.loads(column.comment)
 
             if not isinstance(data_source_meta, dict):
@@ -202,51 +209,52 @@
 #     }
 #
 # def table_relations(mapper):
 #     return list(map(map_relation, filter(lambda x: x.direction == ONETOMANY and hasattr(x, 'table'), mapper.relationships)))
 #
 # def table_m2m_relations(mapper):
 #     result = []
-#     name = mapper.selectable.name
+#     name = mapper.selectable.fullname
 #
 #     for relation in mapper.relationships:
 #         if relation.direction != ONETOMANY or not hasattr(relation, 'table'):
 #             continue
 #
 #         m2m_relationships = relation.mapper.relationships.values()
 #
 #         if len(m2m_relationships) != 2:
 #             continue
 #
 #         if len(relation.table.columns) > 5:
 #             continue
 #
-#         self_relationship = m2m_relationships[1] if m2m_relationships[1].table.name == name else \
+#         self_relationship = m2m_relationships[1] if m2m_relationships[1].table.fullname == name else \
 #         m2m_relationships[0]
 #         other_relationship = m2m_relationships[0] if self_relationship == m2m_relationships[1] else \
 #         m2m_relationships[1]
 #
 #         result.append({
-#             'name': 'M2M {} {}'.format(self_relationship.table.name, other_relationship.table.name),
+#             'name': 'M2M {} {}'.format(self_relationship.table.fullname, other_relationship.table.fullname),
 #             'related_model': {
-#                 'model': other_relationship.table.name
+#                 'model': other_relationship.table.fullname
 #             },
 #             'field': 'ManyToManyField',
-#             'related_model_field': self_relationship.table.name,
-#             'through': {'model': relation.table.name}
+#             'related_model_field': self_relationship.table.fullname,
+#             'through': {'model': relation.table.fullname}
 #         })
 #
 #     return result
 
 def map_table(MappedBase, cls, relationships_overrides, hidden):
     mapper = inspect(cls)
     table = mapper.tables[0]
     name = get_table_name(MappedBase.metadata, table)
     primary_key = mapper.primary_key[0]
     primary_key_auto = getattr(table, '__jet_auto_pk__', False) if table is not None else None
+    is_view = getattr(table, '__jet_is_view__', False) if table is not None else False
     non_editable = []
     model_relationships_overrides = relationships_overrides.get(name)
 
     from jet_bridge_base.configuration import configuration
     additional = configuration.get_model_description(name)
 
     data_source_name = None
@@ -283,14 +291,15 @@
         'fields': list(map(lambda x: map_column(MappedBase.metadata, x, x.name not in non_editable), mapper.columns)),
         'relations': list(map(lambda x: map_relationship(MappedBase.metadata, x), filter(lambda x: x.direction in [MANYTOONE, ONETOMANY], mapper.relationships))),
         'relation_overrides': list(map(lambda x: map_relationship_override(x), model_relationships_overrides)) if model_relationships_overrides else None,
         'hidden': name in hidden or name in configuration.get_hidden_model_description(),
         # 'relations': table_relations(mapper) + table_m2m_relations(mapper),
         'primary_key_field': primary_key.name if primary_key is not None else None,
         'primary_key_auto': primary_key_auto,
+        'is_view': is_view,
         'data_source_name': data_source_name,
         'data_source_name_plural': data_source_name_plural,
         'data_source_order_after': data_source_order_after,
         'data_source_hidden': data_source_hidden
     }
 
     if additional:
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/table.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/table.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/sql.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/sql.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/proxy_request.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/proxy_request.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/model_description_relationship_override.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/model_description_relationship_override.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/generic_api.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/generic_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/api.cpython-310.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/generic_api.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/generic_api.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/base/__pycache__/api.cpython-36.pyc` & `jet-bridge-base-1.8.2/jet_bridge_base/views/base/__pycache__/api.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 76b0 eb63 5618 0000 e300 0000  3...v..cV.......
+00000000: 330d 0d0a 356e c364 e918 0000 e300 0000  3...5n.d........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 cc00 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
 00000030: 6402 6c01 6d01 5a01 0100 6400 6401 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6401 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
@@ -135,252 +135,257 @@
 00000860: 01da 1270 6572 6d69 7373 696f 6e5f 636c  ...permission_cl
 00000870: 6173 7365 7329 0172 1e00 0000 7214 0000  asses).r....r...
 00000880: 0072 1400 0000 7215 0000 00da 0f67 6574  .r....r......get
 00000890: 5f70 6572 6d69 7373 696f 6e73 3100 0000  _permissions1...
 000008a0: 7302 0000 0000 017a 1b42 6173 6541 5049  s......z.BaseAPI
 000008b0: 5669 6577 2e67 6574 5f70 6572 6d69 7373  View.get_permiss
 000008c0: 696f 6e73 6302 0000 0000 0000 0003 0000  ionsc...........
-000008d0: 0006 0000 0043 0000 0073 3200 0000 782c  .....C...s2...x,
-000008e0: 7c00 6a00 8300 4400 5d20 7d02 7c02 6a01  |.j...D.] }.|.j.
-000008f0: 7c00 7c01 8302 730a 7402 7403 7c02 6401  |.|...s.t.t.|.d.
-00000900: 6402 8303 8301 8201 710a 5700 6400 5300  d.......q.W.d.S.
-00000910: 2903 4eda 076d 6573 7361 6765 da09 666f  ).N..message..fo
-00000920: 7262 6964 6465 6e29 0472 2e00 0000 5a0e  rbidden).r....Z.
-00000930: 6861 735f 7065 726d 6973 7369 6f6e 7208  has_permissionr.
-00000940: 0000 00da 0767 6574 6174 7472 2903 721e  .....getattr).r.
-00000950: 0000 0072 1f00 0000 722b 0000 0072 1400  ...r....r+...r..
-00000960: 0000 7214 0000 0072 1500 0000 7227 0000  ..r....r....r'..
-00000970: 0034 0000 0073 0600 0000 0001 0e01 0c01  .4...s..........
-00000980: 7a1d 4261 7365 4150 4956 6965 772e 6368  z.BaseAPIView.ch
-00000990: 6563 6b5f 7065 726d 6973 7369 6f6e 7363  eck_permissionsc
-000009a0: 0300 0000 0000 0000 0400 0000 0600 0000  ................
-000009b0: 4300 0000 7334 0000 0078 2e7c 006a 0083  C...s4...x.|.j..
-000009c0: 0044 005d 227d 037c 036a 017c 007c 017c  .D.]"}.|.j.|.|.|
-000009d0: 0283 0373 0a74 0274 037c 0364 0164 0283  ...s.t.t.|.d.d..
-000009e0: 0383 0182 0171 0a57 0064 0053 0029 034e  .....q.W.d.S.).N
-000009f0: 722f 0000 0072 3000 0000 2904 722e 0000  r/...r0...).r...
-00000a00: 005a 1568 6173 5f6f 626a 6563 745f 7065  .Z.has_object_pe
-00000a10: 726d 6973 7369 6f6e 7208 0000 0072 3100  rmissionr....r1.
-00000a20: 0000 2904 721e 0000 0072 1f00 0000 da03  ..).r....r......
-00000a30: 6f62 6a72 2b00 0000 7214 0000 0072 1400  objr+...r....r..
-00000a40: 0000 7215 0000 00da 1863 6865 636b 5f6f  ..r......check_o
-00000a50: 626a 6563 745f 7065 726d 6973 7369 6f6e  bject_permission
-00000a60: 7339 0000 0073 0600 0000 0001 0e01 0e01  s9...s..........
-00000a70: 7a24 4261 7365 4150 4956 6965 772e 6368  z$BaseAPIView.ch
+000008d0: 0006 0000 0043 0000 0073 3c00 0000 7400  .....C...s<...t.
+000008e0: 6a01 720a 6400 5300 782c 7c00 6a02 8300  j.r.d.S.x,|.j...
+000008f0: 4400 5d20 7d02 7c02 6a03 7c00 7c01 8302  D.] }.|.j.|.|...
+00000900: 7314 7404 7405 7c02 6401 6402 8303 8301  s.t.t.|.d.d.....
+00000910: 8201 7114 5700 6400 5300 2903 4eda 076d  ..q.W.d.S.).N..m
+00000920: 6573 7361 6765 da09 666f 7262 6964 6465  essage..forbidde
+00000930: 6e29 0672 0300 0000 da0c 4449 5341 424c  n).r......DISABL
+00000940: 455f 4155 5448 722e 0000 005a 0e68 6173  E_AUTHr....Z.has
+00000950: 5f70 6572 6d69 7373 696f 6e72 0800 0000  _permissionr....
+00000960: da07 6765 7461 7474 7229 0372 1e00 0000  ..getattr).r....
+00000970: 721f 0000 0072 2b00 0000 7214 0000 0072  r....r+...r....r
+00000980: 1400 0000 7215 0000 0072 2700 0000 3400  ....r....r'...4.
+00000990: 0000 730a 0000 0000 0106 0104 020e 010c  ..s.............
+000009a0: 017a 1d42 6173 6541 5049 5669 6577 2e63  .z.BaseAPIView.c
+000009b0: 6865 636b 5f70 6572 6d69 7373 696f 6e73  heck_permissions
+000009c0: 6303 0000 0000 0000 0004 0000 0006 0000  c...............
+000009d0: 0043 0000 0073 3e00 0000 7400 6a01 720a  .C...s>...t.j.r.
+000009e0: 6400 5300 782e 7c00 6a02 8300 4400 5d22  d.S.x.|.j...D.]"
+000009f0: 7d03 7c03 6a03 7c00 7c01 7c02 8303 7314  }.|.j.|.|.|...s.
+00000a00: 7404 7405 7c03 6401 6402 8303 8301 8201  t.t.|.d.d.......
+00000a10: 7114 5700 6400 5300 2903 4e72 2f00 0000  q.W.d.S.).Nr/...
+00000a20: 7230 0000 0029 0672 0300 0000 7231 0000  r0...).r....r1..
+00000a30: 0072 2e00 0000 5a15 6861 735f 6f62 6a65  .r....Z.has_obje
+00000a40: 6374 5f70 6572 6d69 7373 696f 6e72 0800  ct_permissionr..
+00000a50: 0000 7232 0000 0029 0472 1e00 0000 721f  ..r2...).r....r.
+00000a60: 0000 00da 036f 626a 722b 0000 0072 1400  .....objr+...r..
+00000a70: 0000 7214 0000 0072 1500 0000 da18 6368  ..r....r......ch
 00000a80: 6563 6b5f 6f62 6a65 6374 5f70 6572 6d69  eck_object_permi
-00000a90: 7373 696f 6e73 6301 0000 0000 0000 0002  ssionsc.........
-00000aa0: 0000 0003 0000 0043 0000 0073 3800 0000  .......C...s8...
-00000ab0: 6900 7d01 7400 6a01 7234 7400 6a02 7c01  i.}.t.j.r4t.j.|.
-00000ac0: 6401 3c00 6402 7c01 6403 3c00 6404 7c01  d.<.d.|.d.<.d.|.
-00000ad0: 6405 3c00 6406 7c01 6407 3c00 6408 7c01  d.<.d.|.d.<.d.|.
-00000ae0: 6409 3c00 7c01 5300 290a 4e7a 1b41 6363  d.<.|.S.).Nz.Acc
-00000af0: 6573 732d 436f 6e74 726f 6c2d 416c 6c6f  ess-Control-Allo
-00000b00: 772d 4f72 6967 696e 7a26 4745 542c 2050  w-Originz&GET, P
-00000b10: 4f53 542c 2050 5554 2c20 5041 5443 482c  OST, PUT, PATCH,
-00000b20: 2044 454c 4554 452c 204f 5054 494f 4e53   DELETE, OPTIONS
-00000b30: 7a1c 4163 6365 7373 2d43 6f6e 7472 6f6c  z.Access-Control
-00000b40: 2d41 6c6c 6f77 2d4d 6574 686f 6473 7aaf  -Allow-Methodsz.
-00000b50: 4175 7468 6f72 697a 6174 696f 6e2c 444e  Authorization,DN
-00000b60: 542c 5573 6572 2d41 6765 6e74 2c58 2d52  T,User-Agent,X-R
-00000b70: 6571 7565 7374 6564 2d57 6974 682c 4966  equested-With,If
-00000b80: 2d4d 6f64 6966 6965 642d 5369 6e63 652c  -Modified-Since,
-00000b90: 4361 6368 652d 436f 6e74 726f 6c2c 436f  Cache-Control,Co
-00000ba0: 6e74 656e 742d 5479 7065 2c52 616e 6765  ntent-Type,Range
-00000bb0: 2c58 2d41 7070 6c69 6361 7469 6f6e 2d57  ,X-Application-W
-00000bc0: 6172 6e69 6e67 2c58 2d48 5454 502d 4d65  arning,X-HTTP-Me
-00000bd0: 7468 6f64 2d4f 7665 7272 6964 652c 582d  thod-Override,X-
-00000be0: 4272 6964 6765 2d53 6574 7469 6e67 732c  Bridge-Settings,
-00000bf0: 582d 5374 6963 6b2d 5365 7373 696f 6e7a  X-Stick-Sessionz
-00000c00: 1c41 6363 6573 732d 436f 6e74 726f 6c2d  .Access-Control-
-00000c10: 416c 6c6f 772d 4865 6164 6572 737a 5343  Allow-HeaderszSC
-00000c20: 6f6e 7465 6e74 2d4c 656e 6774 682c 436f  ontent-Length,Co
-00000c30: 6e74 656e 742d 5261 6e67 652c 436f 6e74  ntent-Range,Cont
-00000c40: 656e 742d 4469 7370 6f73 6974 696f 6e2c  ent-Disposition,
-00000c50: 436f 6e74 656e 742d 5479 7065 2c58 2d41  Content-Type,X-A
-00000c60: 7070 6c69 6361 7469 6f6e 2d57 6172 6e69  pplication-Warni
-00000c70: 6e67 7a1d 4163 6365 7373 2d43 6f6e 7472  ngz.Access-Contr
-00000c80: 6f6c 2d45 7870 6f73 652d 4865 6164 6572  ol-Expose-Header
-00000c90: 73da 0474 7275 657a 2041 6363 6573 732d  s..truez Access-
-00000ca0: 436f 6e74 726f 6c2d 416c 6c6f 772d 4372  Control-Allow-Cr
-00000cb0: 6564 656e 7469 616c 7329 0372 0300 0000  edentials).r....
-00000cc0: da0c 434f 5253 5f48 4541 4445 5253 da0c  ..CORS_HEADERS..
-00000cd0: 414c 4c4f 575f 4f52 4947 494e 2902 721e  ALLOW_ORIGIN).r.
-00000ce0: 0000 0072 2200 0000 7214 0000 0072 1400  ...r"...r....r..
-00000cf0: 0000 7215 0000 00da 0f64 6566 6175 6c74  ..r......default
-00000d00: 5f68 6561 6465 7273 3e00 0000 7310 0000  _headers>...s...
-00000d10: 0000 0104 0206 010a 0108 0108 0108 0108  ................
-00000d20: 027a 1b42 6173 6541 5049 5669 6577 2e64  .z.BaseAPIView.d
-00000d30: 6566 6175 6c74 5f68 6561 6465 7273 6305  efault_headersc.
-00000d40: 0000 0000 0000 000c 0000 000a 0000 0043  ...............C
-00000d50: 0000 0073 7a01 0000 7400 7c03 7401 8302  ...sz...t.|.t...
-00000d60: 721e 7402 6401 6402 6403 7c01 6a03 6901  r.t.d.d.d.|.j.i.
-00000d70: 6404 8d03 5300 7400 7c03 7404 8302 723c  d...S.t.|.t...r<
-00000d80: 7402 6405 6406 6403 7c01 6a03 6901 6404  t.d.d.d.|.j.i.d.
-00000d90: 8d03 5300 7400 7c03 7405 8302 725c 7406  ..S.t.|.t...r\t.
-00000da0: 7c03 8301 7d05 7407 7c05 7c03 6a08 6407  |...}.t.|.|.j.d.
-00000db0: 8d02 5300 7400 7c03 7409 8302 727e 7407  ..S.t.|.t...r~t.
-00000dc0: 7c03 6a0a 7c03 6a0b 6408 9c02 7c03 6a08  |.j.|.j.d...|.j.
-00000dd0: 6407 8d02 5300 740c 6a0d 9001 726a 7c01  d...S.t.j...rj|.
-00000de0: 7290 7c01 6a03 6e02 6400 7c01 72ac 7c01  r.|.j.n.d.|.r.|.
-00000df0: 6a0e 6409 1700 7c01 6a0f 1700 7c01 6a03  j.d...|.j...|.j.
-00000e00: 1700 6e02 6400 7c01 72b8 7c01 6a10 6e02  ..n.d.|.r.|.j.n.
-00000e10: 6400 7411 6a12 8300 7411 6a13 8300 7414  d.t.j...t.j...t.
-00000e20: 6a15 8300 6a16 640a 8301 7417 6a18 8300  j...j.d...t.j...
-00000e30: 7419 6a1a 7419 6a03 640b 9c09 7d06 7c03  t.j.t.j.d...}.|.
-00000e40: 9001 7204 7c06 6a1b 7c02 6a1c 741d 6a1e  ..r.|.j.|.j.t.j.
-00000e50: 7c03 8301 640c 9c02 8301 0100 7c04 9001  |...d.......|...
-00000e60: 7252 7c04 7d07 7814 7c07 6a1f 9001 7222  rR|.}.x.|.j...r"
-00000e70: 7c07 6a1f 7d07 9001 7110 5700 7c07 6a20  |.j.}...q.W.|.j 
-00000e80: 7d08 7c08 6a21 6a22 7d09 7c08 6a21 6a23  }.|.j!j"}.|.j!j#
-00000e90: 7d0a 7c08 6a24 7d0b 7c06 6a1b 7c0b 7c09  }.|.j$}.|.j.|.|.
-00000ea0: 7c0a 640d 9c03 8301 0100 7425 6a26 7c03  |.d.......t%j&|.
-00000eb0: 8301 0100 7402 640e 640f 7c06 6404 8d03  ....t.d.d.|.d...
-00000ec0: 5300 7402 6410 640f 6407 8d02 5300 6400  S.t.d.d.d...S.d.
-00000ed0: 5300 2911 4e7a 0834 3033 2e68 746d 6c69  S.).Nz.403.htmli
-00000ee0: 9301 0000 da04 7061 7468 2902 da06 7374  ......path)...st
-00000ef0: 6174 7573 da04 6461 7461 7a08 3430 342e  atus..dataz.404.
-00000f00: 6874 6d6c 6994 0100 0029 0172 3900 0000  htmli....).r9...
-00000f10: 2902 da05 6572 726f 725a 0a65 7272 6f72  )...errorZ.error
-00000f20: 5f63 6f64 657a 033a 2f2f 7a02 2563 2909  _codez.://z.%c).
-00000f30: 7238 0000 00da 0966 756c 6c5f 7061 7468  r8.....full_path
-00000f40: 721c 0000 00da 0474 7970 65da 0776 6572  r......type..ver
-00000f50: 7369 6f6e 5a10 6375 7272 656e 745f 6461  sionZ.current_da
-00000f60: 7465 7469 6d65 da0e 7079 7468 6f6e 5f76  tetime..python_v
-00000f70: 6572 7369 6f6e 5a11 7079 7468 6f6e 5f65  ersionZ.python_e
-00000f80: 7865 6375 7461 626c 655a 0b70 7974 686f  xecutableZ.pytho
-00000f90: 6e5f 7061 7468 2902 da0e 6578 6365 7074  n_path)...except
-00000fa0: 696f 6e5f 7479 7065 5a0f 6578 6365 7074  ion_typeZ.except
-00000fb0: 696f 6e5f 7661 6c75 6529 035a 1d65 7863  ion_value).Z.exc
-00000fc0: 6570 7469 6f6e 5f6c 6173 745f 7472 6163  eption_last_trac
-00000fd0: 6562 6163 6b5f 6c69 6e65 5a1d 6578 6365  eback_lineZ.exce
-00000fe0: 7074 696f 6e5f 6c61 7374 5f74 7261 6365  ption_last_trace
-00000ff0: 6261 636b 5f66 756e 635a 1d65 7863 6570  back_funcZ.excep
-00001000: 7469 6f6e 5f6c 6173 745f 7472 6163 6562  tion_last_traceb
-00001010: 6163 6b5f 6669 6c65 7a0e 3530 302e 6465  ack_filez.500.de
-00001020: 6275 672e 6874 6d6c 69f4 0100 007a 0835  bug.htmli....z.5
-00001030: 3030 2e68 746d 6c29 27da 0a69 7369 6e73  00.html)'..isins
-00001040: 7461 6e63 6572 0800 0000 720b 0000 0072  tancer....r....r
-00001050: 3800 0000 7207 0000 0072 0900 0000 720d  8...r....r....r.
-00001060: 0000 0072 0a00 0000 da0b 7374 6174 7573  ...r......status
-00001070: 5f63 6f64 6572 0600 0000 da06 6465 7461  _coder......deta
-00001080: 696c da04 636f 6465 7203 0000 00da 0544  il..coder......D
-00001090: 4542 5547 da08 7072 6f74 6f63 6f6c da04  EBUG..protocol..
-000010a0: 686f 7374 721c 0000 0072 0400 0000 da08  hostr....r......
-000010b0: 6765 745f 7479 7065 da0b 6765 745f 7665  get_type..get_ve
-000010c0: 7273 696f 6e72 0200 0000 da03 6e6f 77da  rsionr......now.
-000010d0: 0873 7472 6674 696d 65da 0870 6c61 7466  .strftime..platf
-000010e0: 6f72 6d72 3f00 0000 da03 7379 73da 0a65  ormr?.....sys..e
-000010f0: 7865 6375 7461 626c 65da 0675 7064 6174  xecutable..updat
-00001100: 65da 085f 5f6e 616d 655f 5fda 0373 6978  e..__name__..six
-00001110: da09 7465 7874 5f74 7970 65da 0774 625f  ..text_type..tb_
-00001120: 6e65 7874 da08 7462 5f66 7261 6d65 da06  next..tb_frame..
-00001130: 665f 636f 6465 da07 636f 5f6e 616d 65da  f_code..co_name.
-00001140: 0b63 6f5f 6669 6c65 6e61 6d65 da08 665f  .co_filename..f_
-00001150: 6c69 6e65 6e6f 720c 0000 00da 0965 7863  linenor......exc
-00001160: 6570 7469 6f6e 290c 721e 0000 0072 1f00  eption).r....r..
-00001170: 0000 da08 6578 635f 7479 7065 da03 6578  ....exc_type..ex
-00001180: 63da 0974 7261 6365 6261 636b da08 7265  c..traceback..re
-00001190: 7370 6f6e 7365 da03 6374 78da 0e6c 6173  sponse..ctx..las
-000011a0: 745f 7472 6163 6562 6163 6bda 0566 7261  t_traceback..fra
-000011b0: 6d65 da09 6675 6e63 5f6e 616d 65da 0966  me..func_name..f
-000011c0: 696c 655f 6e61 6d65 da0b 6c69 6e65 5f6e  ile_name..line_n
-000011d0: 756d 6265 7272 1400 0000 7214 0000 0072  umberr....r....r
-000011e0: 1500 0000 da0e 6572 726f 725f 7265 7370  ......error_resp
-000011f0: 6f6e 7365 4a00 0000 7356 0000 0000 010a  onseJ...sV......
-00001200: 0106 010e 020a 0106 010e 020a 0108 010e  ................
-00001210: 010a 0102 0104 0108 010a 0208 020c 011c  ................
-00001220: 010c 0106 0106 010c 0106 0104 010a 0306  ................
-00001230: 0104 0104 0110 0306 0104 020a 010c 0206  ................
-00001240: 0108 0108 0106 0204 0102 0102 010a 030a  ................
-00001250: 020e 027a 1a42 6173 6541 5049 5669 6577  ...z.BaseAPIView
-00001260: 2e65 7272 6f72 5f72 6573 706f 6e73 6563  .error_responsec
-00001270: 0300 0000 0000 0000 0500 0000 0300 0000  ................
-00001280: 4f00 0000 7326 0000 0074 007c 007c 0183  O...s&...t.|.|..
-00001290: 0273 1074 0183 0082 0174 027c 007c 0183  .s.t.....t.|.|..
-000012a0: 027c 0266 017c 039e 027c 048e 0153 0029  .|.f.|...|...S.)
-000012b0: 014e 2903 da07 6861 7361 7474 7272 0700  .N)...hasattrr..
-000012c0: 0000 7231 0000 0029 0572 1e00 0000 da06  ..r1...).r......
-000012d0: 6163 7469 6f6e 721f 0000 00da 0461 7267  actionr......arg
-000012e0: 73da 066b 7761 7267 7372 1400 0000 7214  s..kwargsr....r.
-000012f0: 0000 0072 1500 0000 da08 6469 7370 6174  ...r......dispat
-00001300: 6368 8600 0000 7306 0000 0000 010a 0106  ch....s.........
-00001310: 017a 1442 6173 6541 5049 5669 6577 2e64  .z.BaseAPIView.d
-00001320: 6973 7061 7463 684e 290f 7250 0000 00da  ispatchN).rP....
-00001330: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00001340: 7561 6c6e 616d 655f 5f72 2d00 0000 7221  ualname__r-...r!
-00001350: 0000 0072 2500 0000 7224 0000 0072 2800  ...r%...r$...r(.
-00001360: 0000 7229 0000 0072 2e00 0000 7227 0000  ..r)...r....r'..
-00001370: 0072 3300 0000 7237 0000 0072 6400 0000  .r3...r7...rd...
-00001380: 7269 0000 0072 1400 0000 7214 0000 0072  ri...r....r....r
-00001390: 1400 0000 7215 0000 0072 0e00 0000 1400  ....r....r......
-000013a0: 0000 7318 0000 0008 0304 0208 0508 0908  ..s.............
-000013b0: 0408 0308 0308 0308 0508 0508 0c08 3c72  ..............<r
-000013c0: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000013d0: 0003 0000 0000 0000 0073 2800 0000 6500  .........s(...e.
-000013e0: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
-000013f0: 5a03 8700 6601 6403 6404 8408 5a04 8700  Z...f.d.d...Z...
-00001400: 0400 5a05 5300 2905 da07 4150 4956 6965  ..Z.S.)...APIVie
-00001410: 7763 0200 0000 0000 0000 0300 0000 1000  wc..............
-00001420: 0000 0300 0000 7352 0000 0074 0074 017c  ......sR...t.t.|
-00001430: 0083 026a 027c 0183 0101 0079 0e74 037c  ...j.|.....y.t.|
-00001440: 0183 017c 015f 0457 006e 2e04 0074 056b  ...|._.W.n...t.k
-00001450: 0a72 4c01 007d 0201 007a 1274 0674 077c  .rL..}...z.t.t.|
-00001460: 0283 0183 0182 0157 0059 0064 0064 007d  .......W.Y.d.d.}
-00001470: 027e 0258 006e 0258 0064 0053 0029 014e  .~.X.n.X.d.S.).N
-00001480: 2908 da05 7375 7065 7272 6c00 0000 7225  )...superrl...r%
-00001490: 0000 0072 0500 0000 da07 7365 7373 696f  ...r......sessio
-000014a0: 6eda 0945 7863 6570 7469 6f6e 7209 0000  n..Exceptionr...
-000014b0: 00da 0373 7472 2903 721e 0000 0072 1f00  ...str).r....r..
-000014c0: 0000 da01 6529 01da 095f 5f63 6c61 7373  ....e)...__class
-000014d0: 5f5f 7214 0000 0072 1500 0000 7225 0000  __r....r....r%..
-000014e0: 0091 0000 0073 0a00 0000 0001 1002 0201  .....s..........
-000014f0: 0e01 1001 7a17 4150 4956 6965 772e 6265  ....z.APIView.be
-00001500: 666f 7265 5f64 6973 7061 7463 6863 0200  fore_dispatchc..
-00001510: 0000 0000 0000 0200 0000 0300 0000 0300  ................
-00001520: 0000 732a 0000 0074 0074 017c 0083 026a  ..s*...t.t.|...j
-00001530: 027c 0183 0101 007c 016a 0372 267c 016a  .|.....|.j.r&|.j
-00001540: 036a 0483 0001 0064 007c 015f 0364 0053  .j.....d.|._.d.S
-00001550: 0029 014e 2905 726d 0000 0072 6c00 0000  .).N).rm...rl...
-00001560: 7228 0000 0072 6e00 0000 da05 636c 6f73  r(...rn.....clos
-00001570: 6529 0272 1e00 0000 721f 0000 0029 0172  e).r....r....).r
-00001580: 7200 0000 7214 0000 0072 1500 0000 7228  r...r....r....r(
-00001590: 0000 0099 0000 0073 0800 0000 0001 1002  .......s........
-000015a0: 0601 0a01 7a16 4150 4956 6965 772e 6166  ....z.APIView.af
-000015b0: 7465 725f 6469 7370 6174 6368 2906 7250  ter_dispatch).rP
-000015c0: 0000 0072 6a00 0000 726b 0000 0072 2500  ...rj...rk...r%.
-000015d0: 0000 7228 0000 00da 0d5f 5f63 6c61 7373  ..r(.....__class
-000015e0: 6365 6c6c 5f5f 7214 0000 0072 1400 0000  cell__r....r....
-000015f0: 2901 7272 0000 0072 1500 0000 726c 0000  ).rr...r....rl..
-00001600: 008f 0000 0073 0400 0000 0802 0c08 726c  .....s........rl
-00001610: 0000 0029 1d72 4c00 0000 7202 0000 0072  ...).rL...r....r
-00001620: 4d00 0000 7251 0000 00da 0f6a 6574 5f62  M...rQ.....jet_b
-00001630: 7269 6467 655f 6261 7365 7203 0000 00da  ridge_baser.....
-00001640: 1d6a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00001650: 2e63 6f6e 6669 6775 7261 7469 6f6e 7204  .configurationr.
-00001660: 0000 00da 126a 6574 5f62 7269 6467 655f  .....jet_bridge_
-00001670: 6261 7365 2e64 6272 0500 0000 da1e 6a65  base.dbr......je
-00001680: 745f 6272 6964 6765 5f62 6173 652e 6578  t_bridge_base.ex
-00001690: 6365 7074 696f 6e73 2e61 7069 7206 0000  ceptions.apir...
-000016a0: 005a 246a 6574 5f62 7269 6467 655f 6261  .Z$jet_bridge_ba
-000016b0: 7365 2e65 7863 6570 7469 6f6e 732e 6e6f  se.exceptions.no
-000016c0: 745f 666f 756e 6472 0700 0000 5a2c 6a65  t_foundr....Z,je
-000016d0: 745f 6272 6964 6765 5f62 6173 652e 6578  t_bridge_base.ex
-000016e0: 6365 7074 696f 6e73 2e70 6572 6d69 7373  ceptions.permiss
-000016f0: 696f 6e5f 6465 6e69 6564 7208 0000 005a  ion_deniedr....Z
-00001700: 2b6a 6574 5f62 7269 6467 655f 6261 7365  +jet_bridge_base
-00001710: 2e65 7863 6570 7469 6f6e 732e 7661 6c69  .exceptions.vali
-00001720: 6461 7469 6f6e 5f65 7272 6f72 7209 0000  dation_errorr...
-00001730: 00da 1e6a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
-00001740: 7365 2e72 6573 706f 6e73 6573 2e6a 736f  se.responses.jso
-00001750: 6e72 0a00 0000 5a22 6a65 745f 6272 6964  nr....Z"jet_brid
-00001760: 6765 5f62 6173 652e 7265 7370 6f6e 7365  ge_base.response
-00001770: 732e 7465 6d70 6c61 7465 720b 0000 00da  s.templater.....
-00001780: 166a 6574 5f62 7269 6467 655f 6261 7365  .jet_bridge_base
-00001790: 2e6c 6f67 6765 7272 0c00 0000 5a20 6a65  .loggerr....Z je
-000017a0: 745f 6272 6964 6765 5f62 6173 652e 7574  t_bridge_base.ut
-000017b0: 696c 732e 6578 6365 7074 696f 6e73 720d  ils.exceptionsr.
-000017c0: 0000 00da 066f 626a 6563 7472 0e00 0000  .....objectr....
-000017d0: 726c 0000 0072 1400 0000 7214 0000 0072  rl...r....r....r
-000017e0: 1400 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
-000017f0: 6c65 3e01 0000 0073 2000 0000 0801 0c01  le>....s .......
-00001800: 0802 0802 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001810: 0c01 0c01 0c01 0c01 0c03 107b            ...........{
+00000a90: 7373 696f 6e73 3c00 0000 730a 0000 0000  ssions<...s.....
+00000aa0: 0106 0104 020e 010e 017a 2442 6173 6541  .........z$BaseA
+00000ab0: 5049 5669 6577 2e63 6865 636b 5f6f 626a  PIView.check_obj
+00000ac0: 6563 745f 7065 726d 6973 7369 6f6e 7363  ect_permissionsc
+00000ad0: 0100 0000 0000 0000 0200 0000 0300 0000  ................
+00000ae0: 4300 0000 7338 0000 0069 007d 0174 006a  C...s8...i.}.t.j
+00000af0: 0172 3474 006a 027c 0164 013c 0064 027c  .r4t.j.|.d.<.d.|
+00000b00: 0164 033c 0064 047c 0164 053c 0064 067c  .d.<.d.|.d.<.d.|
+00000b10: 0164 073c 0064 087c 0164 093c 007c 0153  .d.<.d.|.d.<.|.S
+00000b20: 0029 0a4e 7a1b 4163 6365 7373 2d43 6f6e  .).Nz.Access-Con
+00000b30: 7472 6f6c 2d41 6c6c 6f77 2d4f 7269 6769  trol-Allow-Origi
+00000b40: 6e7a 2647 4554 2c20 504f 5354 2c20 5055  nz&GET, POST, PU
+00000b50: 542c 2050 4154 4348 2c20 4445 4c45 5445  T, PATCH, DELETE
+00000b60: 2c20 4f50 5449 4f4e 537a 1c41 6363 6573  , OPTIONSz.Acces
+00000b70: 732d 436f 6e74 726f 6c2d 416c 6c6f 772d  s-Control-Allow-
+00000b80: 4d65 7468 6f64 737a af41 7574 686f 7269  Methodsz.Authori
+00000b90: 7a61 7469 6f6e 2c44 4e54 2c55 7365 722d  zation,DNT,User-
+00000ba0: 4167 656e 742c 582d 5265 7175 6573 7465  Agent,X-Requeste
+00000bb0: 642d 5769 7468 2c49 662d 4d6f 6469 6669  d-With,If-Modifi
+00000bc0: 6564 2d53 696e 6365 2c43 6163 6865 2d43  ed-Since,Cache-C
+00000bd0: 6f6e 7472 6f6c 2c43 6f6e 7465 6e74 2d54  ontrol,Content-T
+00000be0: 7970 652c 5261 6e67 652c 582d 4170 706c  ype,Range,X-Appl
+00000bf0: 6963 6174 696f 6e2d 5761 726e 696e 672c  ication-Warning,
+00000c00: 582d 4854 5450 2d4d 6574 686f 642d 4f76  X-HTTP-Method-Ov
+00000c10: 6572 7269 6465 2c58 2d42 7269 6467 652d  erride,X-Bridge-
+00000c20: 5365 7474 696e 6773 2c58 2d53 7469 636b  Settings,X-Stick
+00000c30: 2d53 6573 7369 6f6e 7a1c 4163 6365 7373  -Sessionz.Access
+00000c40: 2d43 6f6e 7472 6f6c 2d41 6c6c 6f77 2d48  -Control-Allow-H
+00000c50: 6561 6465 7273 7a53 436f 6e74 656e 742d  eaderszSContent-
+00000c60: 4c65 6e67 7468 2c43 6f6e 7465 6e74 2d52  Length,Content-R
+00000c70: 616e 6765 2c43 6f6e 7465 6e74 2d44 6973  ange,Content-Dis
+00000c80: 706f 7369 7469 6f6e 2c43 6f6e 7465 6e74  position,Content
+00000c90: 2d54 7970 652c 582d 4170 706c 6963 6174  -Type,X-Applicat
+00000ca0: 696f 6e2d 5761 726e 696e 677a 1d41 6363  ion-Warningz.Acc
+00000cb0: 6573 732d 436f 6e74 726f 6c2d 4578 706f  ess-Control-Expo
+00000cc0: 7365 2d48 6561 6465 7273 da04 7472 7565  se-Headers..true
+00000cd0: 7a20 4163 6365 7373 2d43 6f6e 7472 6f6c  z Access-Control
+00000ce0: 2d41 6c6c 6f77 2d43 7265 6465 6e74 6961  -Allow-Credentia
+00000cf0: 6c73 2903 7203 0000 00da 0c43 4f52 535f  ls).r......CORS_
+00000d00: 4845 4144 4552 53da 0c41 4c4c 4f57 5f4f  HEADERS..ALLOW_O
+00000d10: 5249 4749 4e29 0272 1e00 0000 7222 0000  RIGIN).r....r"..
+00000d20: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000d30: da0f 6465 6661 756c 745f 6865 6164 6572  ..default_header
+00000d40: 7344 0000 0073 1000 0000 0001 0402 0601  sD...s..........
+00000d50: 0a01 0801 0801 0801 0802 7a1b 4261 7365  ..........z.Base
+00000d60: 4150 4956 6965 772e 6465 6661 756c 745f  APIView.default_
+00000d70: 6865 6164 6572 7363 0500 0000 0000 0000  headersc........
+00000d80: 0c00 0000 0a00 0000 4300 0000 7384 0100  ........C...s...
+00000d90: 0074 007c 0374 0183 0272 1e74 0264 0164  .t.|.t...r.t.d.d
+00000da0: 0264 037c 016a 0369 0164 048d 0353 0074  .d.|.j.i.d...S.t
+00000db0: 007c 0374 0483 0272 3c74 0264 0564 0664  .|.t...r<t.d.d.d
+00000dc0: 037c 016a 0369 0164 048d 0353 0074 007c  .|.j.i.d...S.t.|
+00000dd0: 0374 0583 0272 5c74 067c 0383 017d 0574  .t...r\t.|...}.t
+00000de0: 077c 057c 036a 0864 078d 0253 0074 007c  .|.|.j.d...S.t.|
+00000df0: 0374 0983 0272 7e74 077c 036a 0a7c 036a  .t...r~t.|.j.|.j
+00000e00: 0b64 089c 027c 036a 0864 078d 0253 0074  .d...|.j.d...S.t
+00000e10: 0c6a 0d90 0172 6a7c 0172 907c 016a 036e  .j...rj|.r.|.j.n
+00000e20: 0264 007c 0172 ac7c 016a 0e64 0917 007c  .d.|.r.|.j.d...|
+00000e30: 016a 0f17 007c 016a 0317 006e 0264 007c  .j...|.j...n.d.|
+00000e40: 0172 b87c 016a 106e 0264 0074 116a 1283  .r.|.j.n.d.t.j..
+00000e50: 0074 116a 1383 0074 146a 1583 006a 1664  .t.j...t.j...j.d
+00000e60: 0a83 0174 176a 1883 0074 196a 1a74 196a  ...t.j...t.j.t.j
+00000e70: 0364 0b9c 097d 067c 0390 0172 047c 066a  .d...}.|...r.|.j
+00000e80: 1b7c 026a 1c74 1d6a 1e7c 0383 0164 0c9c  .|.j.t.j.|...d..
+00000e90: 0283 0101 007c 0490 0172 527c 047d 0778  .....|...rR|.}.x
+00000ea0: 147c 076a 1f90 0172 227c 076a 1f7d 0790  .|.j...r"|.j.}..
+00000eb0: 0171 1057 007c 076a 207d 087c 086a 216a  .q.W.|.j }.|.j!j
+00000ec0: 227d 097c 086a 216a 237d 0a7c 086a 247d  "}.|.j!j#}.|.j$}
+00000ed0: 0b7c 066a 1b7c 0b7c 097c 0a64 0d9c 0383  .|.j.|.|.|.d....
+00000ee0: 0101 0074 256a 267c 0383 0101 0074 0264  ...t%j&|.....t.d
+00000ef0: 0e64 0f7c 0664 048d 0353 0074 256a 267c  .d.|.d...S.t%j&|
+00000f00: 0383 0101 0074 0264 1064 0f64 078d 0253  .....t.d.d.d...S
+00000f10: 0064 0053 0029 114e 7a08 3430 332e 6874  .d.S.).Nz.403.ht
+00000f20: 6d6c 6993 0100 00da 0470 6174 6829 02da  mli......path)..
+00000f30: 0673 7461 7475 73da 0464 6174 617a 0834  .status..dataz.4
+00000f40: 3034 2e68 746d 6c69 9401 0000 2901 723a  04.htmli....).r:
+00000f50: 0000 0029 02da 0565 7272 6f72 5a0a 6572  ...)...errorZ.er
+00000f60: 726f 725f 636f 6465 7a03 3a2f 2f7a 0225  ror_codez.://z.%
+00000f70: 6329 0972 3900 0000 da09 6675 6c6c 5f70  c).r9.....full_p
+00000f80: 6174 6872 1c00 0000 da04 7479 7065 da07  athr......type..
+00000f90: 7665 7273 696f 6e5a 1063 7572 7265 6e74  versionZ.current
+00000fa0: 5f64 6174 6574 696d 65da 0e70 7974 686f  _datetime..pytho
+00000fb0: 6e5f 7665 7273 696f 6e5a 1170 7974 686f  n_versionZ.pytho
+00000fc0: 6e5f 6578 6563 7574 6162 6c65 5a0b 7079  n_executableZ.py
+00000fd0: 7468 6f6e 5f70 6174 6829 02da 0e65 7863  thon_path)...exc
+00000fe0: 6570 7469 6f6e 5f74 7970 655a 0f65 7863  eption_typeZ.exc
+00000ff0: 6570 7469 6f6e 5f76 616c 7565 2903 5a1d  eption_value).Z.
+00001000: 6578 6365 7074 696f 6e5f 6c61 7374 5f74  exception_last_t
+00001010: 7261 6365 6261 636b 5f6c 696e 655a 1d65  raceback_lineZ.e
+00001020: 7863 6570 7469 6f6e 5f6c 6173 745f 7472  xception_last_tr
+00001030: 6163 6562 6163 6b5f 6675 6e63 5a1d 6578  aceback_funcZ.ex
+00001040: 6365 7074 696f 6e5f 6c61 7374 5f74 7261  ception_last_tra
+00001050: 6365 6261 636b 5f66 696c 657a 0e35 3030  ceback_filez.500
+00001060: 2e64 6562 7567 2e68 746d 6c69 f401 0000  .debug.htmli....
+00001070: 7a08 3530 302e 6874 6d6c 2927 da0a 6973  z.500.html)'..is
+00001080: 696e 7374 616e 6365 7208 0000 0072 0b00  instancer....r..
+00001090: 0000 7239 0000 0072 0700 0000 7209 0000  ..r9...r....r...
+000010a0: 0072 0d00 0000 720a 0000 00da 0b73 7461  .r....r......sta
+000010b0: 7475 735f 636f 6465 7206 0000 00da 0664  tus_coder......d
+000010c0: 6574 6169 6cda 0463 6f64 6572 0300 0000  etail..coder....
+000010d0: da05 4445 4255 47da 0870 726f 746f 636f  ..DEBUG..protoco
+000010e0: 6cda 0468 6f73 7472 1c00 0000 7204 0000  l..hostr....r...
+000010f0: 00da 0867 6574 5f74 7970 65da 0b67 6574  ...get_type..get
+00001100: 5f76 6572 7369 6f6e 7202 0000 00da 036e  _versionr......n
+00001110: 6f77 da08 7374 7266 7469 6d65 da08 706c  ow..strftime..pl
+00001120: 6174 666f 726d 7240 0000 00da 0373 7973  atformr@.....sys
+00001130: da0a 6578 6563 7574 6162 6c65 da06 7570  ..executable..up
+00001140: 6461 7465 da08 5f5f 6e61 6d65 5f5f da03  date..__name__..
+00001150: 7369 78da 0974 6578 745f 7479 7065 da07  six..text_type..
+00001160: 7462 5f6e 6578 74da 0874 625f 6672 616d  tb_next..tb_fram
+00001170: 65da 0666 5f63 6f64 65da 0763 6f5f 6e61  e..f_code..co_na
+00001180: 6d65 da0b 636f 5f66 696c 656e 616d 65da  me..co_filename.
+00001190: 0866 5f6c 696e 656e 6f72 0c00 0000 da09  .f_linenor......
+000011a0: 6578 6365 7074 696f 6e29 0c72 1e00 0000  exception).r....
+000011b0: 721f 0000 00da 0865 7863 5f74 7970 65da  r......exc_type.
+000011c0: 0365 7863 da09 7472 6163 6562 6163 6bda  .exc..traceback.
+000011d0: 0872 6573 706f 6e73 65da 0363 7478 da0e  .response..ctx..
+000011e0: 6c61 7374 5f74 7261 6365 6261 636b da05  last_traceback..
+000011f0: 6672 616d 65da 0966 756e 635f 6e61 6d65  frame..func_name
+00001200: da09 6669 6c65 5f6e 616d 65da 0b6c 696e  ..file_name..lin
+00001210: 655f 6e75 6d62 6572 7214 0000 0072 1400  e_numberr....r..
+00001220: 0000 7215 0000 00da 0e65 7272 6f72 5f72  ..r......error_r
+00001230: 6573 706f 6e73 6550 0000 0073 5800 0000  esponseP...sX...
+00001240: 0001 0a01 0601 0e02 0a01 0601 0e02 0a01  ................
+00001250: 0801 0e01 0a01 0201 0401 0801 0a02 0802  ................
+00001260: 0c01 1c01 0c01 0601 0601 0c01 0601 0401  ................
+00001270: 0a03 0601 0401 0401 1003 0601 0402 0a01  ................
+00001280: 0c02 0601 0801 0801 0602 0401 0201 0201  ................
+00001290: 0a03 0a02 0e02 0a02 7a1a 4261 7365 4150  ........z.BaseAP
+000012a0: 4956 6965 772e 6572 726f 725f 7265 7370  IView.error_resp
+000012b0: 6f6e 7365 6303 0000 0000 0000 0005 0000  onsec...........
+000012c0: 0003 0000 004f 0000 0073 2600 0000 7400  .....O...s&...t.
+000012d0: 7c00 7c01 8302 7310 7401 8300 8201 7402  |.|...s.t.....t.
+000012e0: 7c00 7c01 8302 7c02 6601 7c03 9e02 7c04  |.|...|.f.|...|.
+000012f0: 8e01 5300 2901 4e29 03da 0768 6173 6174  ..S.).N)...hasat
+00001300: 7472 7207 0000 0072 3200 0000 2905 721e  trr....r2...).r.
+00001310: 0000 00da 0661 6374 696f 6e72 1f00 0000  .....actionr....
+00001320: da04 6172 6773 da06 6b77 6172 6773 7214  ..args..kwargsr.
+00001330: 0000 0072 1400 0000 7215 0000 00da 0864  ...r....r......d
+00001340: 6973 7061 7463 688e 0000 0073 0600 0000  ispatch....s....
+00001350: 0001 0a01 0601 7a14 4261 7365 4150 4956  ......z.BaseAPIV
+00001360: 6965 772e 6469 7370 6174 6368 4e29 0f72  iew.dispatchN).r
+00001370: 5100 0000 da0a 5f5f 6d6f 6475 6c65 5f5f  Q.....__module__
+00001380: da0c 5f5f 7175 616c 6e61 6d65 5f5f 722d  ..__qualname__r-
+00001390: 0000 0072 2100 0000 7225 0000 0072 2400  ...r!...r%...r$.
+000013a0: 0000 7228 0000 0072 2900 0000 722e 0000  ..r(...r)...r...
+000013b0: 0072 2700 0000 7234 0000 0072 3800 0000  .r'...r4...r8...
+000013c0: 7265 0000 0072 6a00 0000 7214 0000 0072  re...rj...r....r
+000013d0: 1400 0000 7214 0000 0072 1500 0000 720e  ....r....r....r.
+000013e0: 0000 0014 0000 0073 1800 0000 0803 0402  .......s........
+000013f0: 0805 0809 0804 0803 0803 0803 0808 0808  ................
+00001400: 080c 083e 720e 0000 0063 0000 0000 0000  ...>r....c......
+00001410: 0000 0000 0000 0300 0000 0000 0000 7328  ..............s(
+00001420: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00001430: 0164 0284 085a 0387 0066 0164 0364 0484  .d...Z...f.d.d..
+00001440: 085a 0487 0004 005a 0553 0029 05da 0741  .Z.....Z.S.)...A
+00001450: 5049 5669 6577 6302 0000 0000 0000 0003  PIViewc.........
+00001460: 0000 0010 0000 0003 0000 0073 5200 0000  ...........sR...
+00001470: 7400 7401 7c00 8302 6a02 7c01 8301 0100  t.t.|...j.|.....
+00001480: 790e 7403 7c01 8301 7c01 5f04 5700 6e2e  y.t.|...|._.W.n.
+00001490: 0400 7405 6b0a 724c 0100 7d02 0100 7a12  ..t.k.rL..}...z.
+000014a0: 7406 7407 7c02 8301 8301 8201 5700 5900  t.t.|.......W.Y.
+000014b0: 6400 6400 7d02 7e02 5800 6e02 5800 6400  d.d.}.~.X.n.X.d.
+000014c0: 5300 2901 4e29 08da 0573 7570 6572 726d  S.).N)...superrm
+000014d0: 0000 0072 2500 0000 7205 0000 00da 0773  ...r%...r......s
+000014e0: 6573 7369 6f6e da09 4578 6365 7074 696f  ession..Exceptio
+000014f0: 6e72 0900 0000 da03 7374 7229 0372 1e00  nr......str).r..
+00001500: 0000 721f 0000 00da 0165 2901 da09 5f5f  ..r......e)...__
+00001510: 636c 6173 735f 5f72 1400 0000 7215 0000  class__r....r...
+00001520: 0072 2500 0000 9900 0000 730a 0000 0000  .r%.......s.....
+00001530: 0110 0202 010e 0110 017a 1741 5049 5669  .........z.APIVi
+00001540: 6577 2e62 6566 6f72 655f 6469 7370 6174  ew.before_dispat
+00001550: 6368 6302 0000 0000 0000 0002 0000 0003  chc.............
+00001560: 0000 0003 0000 0073 2a00 0000 7400 7401  .......s*...t.t.
+00001570: 7c00 8302 6a02 7c01 8301 0100 7c01 6a03  |...j.|.....|.j.
+00001580: 7226 7c01 6a03 6a04 8300 0100 6400 7c01  r&|.j.j.....d.|.
+00001590: 5f03 6400 5300 2901 4e29 0572 6e00 0000  _.d.S.).N).rn...
+000015a0: 726d 0000 0072 2800 0000 726f 0000 00da  rm...r(...ro....
+000015b0: 0563 6c6f 7365 2902 721e 0000 0072 1f00  .close).r....r..
+000015c0: 0000 2901 7273 0000 0072 1400 0000 7215  ..).rs...r....r.
+000015d0: 0000 0072 2800 0000 a100 0000 7308 0000  ...r(.......s...
+000015e0: 0000 0110 0206 010a 017a 1641 5049 5669  .........z.APIVi
+000015f0: 6577 2e61 6674 6572 5f64 6973 7061 7463  ew.after_dispatc
+00001600: 6829 0672 5100 0000 726b 0000 0072 6c00  h).rQ...rk...rl.
+00001610: 0000 7225 0000 0072 2800 0000 da0d 5f5f  ..r%...r(.....__
+00001620: 636c 6173 7363 656c 6c5f 5f72 1400 0000  classcell__r....
+00001630: 7214 0000 0029 0172 7300 0000 7215 0000  r....).rs...r...
+00001640: 0072 6d00 0000 9700 0000 7304 0000 0008  .rm.......s.....
+00001650: 020c 0872 6d00 0000 291d 724d 0000 0072  ...rm...).rM...r
+00001660: 0200 0000 724e 0000 0072 5200 0000 da0f  ....rN...rR.....
+00001670: 6a65 745f 6272 6964 6765 5f62 6173 6572  jet_bridge_baser
+00001680: 0300 0000 da1d 6a65 745f 6272 6964 6765  ......jet_bridge
+00001690: 5f62 6173 652e 636f 6e66 6967 7572 6174  _base.configurat
+000016a0: 696f 6e72 0400 0000 da12 6a65 745f 6272  ionr......jet_br
+000016b0: 6964 6765 5f62 6173 652e 6462 7205 0000  idge_base.dbr...
+000016c0: 00da 1e6a 6574 5f62 7269 6467 655f 6261  ...jet_bridge_ba
+000016d0: 7365 2e65 7863 6570 7469 6f6e 732e 6170  se.exceptions.ap
+000016e0: 6972 0600 0000 5a24 6a65 745f 6272 6964  ir....Z$jet_brid
+000016f0: 6765 5f62 6173 652e 6578 6365 7074 696f  ge_base.exceptio
+00001700: 6e73 2e6e 6f74 5f66 6f75 6e64 7207 0000  ns.not_foundr...
+00001710: 005a 2c6a 6574 5f62 7269 6467 655f 6261  .Z,jet_bridge_ba
+00001720: 7365 2e65 7863 6570 7469 6f6e 732e 7065  se.exceptions.pe
+00001730: 726d 6973 7369 6f6e 5f64 656e 6965 6472  rmission_deniedr
+00001740: 0800 0000 5a2b 6a65 745f 6272 6964 6765  ....Z+jet_bridge
+00001750: 5f62 6173 652e 6578 6365 7074 696f 6e73  _base.exceptions
+00001760: 2e76 616c 6964 6174 696f 6e5f 6572 726f  .validation_erro
+00001770: 7272 0900 0000 da1e 6a65 745f 6272 6964  rr......jet_brid
+00001780: 6765 5f62 6173 652e 7265 7370 6f6e 7365  ge_base.response
+00001790: 732e 6a73 6f6e 720a 0000 005a 226a 6574  s.jsonr....Z"jet
+000017a0: 5f62 7269 6467 655f 6261 7365 2e72 6573  _bridge_base.res
+000017b0: 706f 6e73 6573 2e74 656d 706c 6174 6572  ponses.templater
+000017c0: 0b00 0000 da16 6a65 745f 6272 6964 6765  ......jet_bridge
+000017d0: 5f62 6173 652e 6c6f 6767 6572 720c 0000  _base.loggerr...
+000017e0: 005a 206a 6574 5f62 7269 6467 655f 6261  .Z jet_bridge_ba
+000017f0: 7365 2e75 7469 6c73 2e65 7863 6570 7469  se.utils.excepti
+00001800: 6f6e 7372 0d00 0000 da06 6f62 6a65 6374  onsr......object
+00001810: 720e 0000 0072 6d00 0000 7214 0000 0072  r....rm...r....r
+00001820: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+00001830: 3c6d 6f64 756c 653e 0100 0000 7322 0000  <module>....s"..
+00001840: 0008 010c 0108 0208 020c 010c 010c 010c  ................
+00001850: 010c 010c 010c 010c 010c 010c 010c 0310  ................
+00001860: 7f00 04                                  ...
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/base/api.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/base/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,25 @@
     def on_finish(self):
         pass
 
     def get_permissions(self):
         return [permission() for permission in self.permission_classes]
 
     def check_permissions(self, request):
+        if settings.DISABLE_AUTH:
+            return
+
         for permission in self.get_permissions():
             if not permission.has_permission(self, request):
                 raise PermissionDenied(getattr(permission, 'message', 'forbidden'))
 
     def check_object_permissions(self, request, obj):
+        if settings.DISABLE_AUTH:
+            return
+
         for permission in self.get_permissions():
             if not permission.has_object_permission(self, request, obj):
                 raise PermissionDenied(getattr(permission, 'message', 'forbidden'))
 
     def default_headers(self):
         headers = {}
 
@@ -125,14 +131,16 @@
                         'exception_last_traceback_file': file_name,
                     })
 
                 logger.exception(exc)
 
                 return TemplateResponse('500.debug.html', status=500, data=ctx)
             else:
+                logger.exception(exc)
+
                 return TemplateResponse('500.html', status=500)
 
     def dispatch(self, action, request, *args, **kwargs):
         if not hasattr(self, action):
             raise NotFound()
         return getattr(self, action)(request, *args, **kwargs)
```

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/base/generic_api.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/base/generic_api.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/views/file_upload.py` & `jet-bridge-base-1.8.2/jet_bridge_base/views/file_upload.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-base-1.7.9/jet_bridge_base/status.py` & `jet-bridge-base-1.8.2/jet_bridge_base/status.py`

 * *Files identical despite different names*

