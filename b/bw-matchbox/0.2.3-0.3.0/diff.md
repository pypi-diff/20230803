# Comparing `tmp/bw_matchbox-0.2.3.tar.gz` & `tmp/bw_matchbox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.2.3.tar", last modified: Wed Aug  2 20:58:42 2023, max compression
+gzip compressed data, was "bw_matchbox-0.3.0.tar", last modified: Wed Aug  2 21:10:16 2023, max compression
```

## Comparing `bw_matchbox-0.2.3.tar` & `bw_matchbox-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,74 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.413441 bw_matchbox-0.2.3/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.2.3/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      216 2023-08-01 11:41:22.000000 bw_matchbox-0.2.3/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 20:58:42.413569 bw_matchbox-0.2.3/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.396561 bw_matchbox-0.2.3/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-02 20:57:58.000000 bw_matchbox-0.2.3/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.394621 bw_matchbox-0.2.3/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.399222 bw_matchbox-0.2.3/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2144 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     5022 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     3320 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.399584 bw_matchbox-0.2.3/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.400144 bw_matchbox-0.2.3/bw_matchbox/assets/js/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4283 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/js/CommonHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.406078 bw_matchbox-0.2.3/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4144 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/file.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2341 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     4135 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.406568 bw_matchbox-0.2.3/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.409586 bw_matchbox-0.2.3/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.2.3/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    20517 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.412288 bw_matchbox-0.2.3/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     3080 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.410283 bw_matchbox-0.2.3/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.2.3/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.2.3/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1881 2023-08-02 20:58:42.414655 bw_matchbox-0.2.3/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.457498 bw_matchbox-0.3.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.3.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.3.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 21:10:16.457621 bw_matchbox-0.3.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.438184 bw_matchbox-0.3.0/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-02 21:10:10.000000 bw_matchbox-0.3.0/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.435615 bw_matchbox-0.3.0/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.440408 bw_matchbox-0.3.0/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2144 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5022 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3320 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.440580 bw_matchbox-0.3.0/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.441127 bw_matchbox-0.3.0/bw_matchbox/assets/js/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4283 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/CommonHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.443479 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    18042 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      946 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    10108 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.444803 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2764 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      269 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      651 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3867 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3968 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      755 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3918 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1982 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3143 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.448195 bw_matchbox-0.3.0/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4144 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/file.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2341 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4135 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.448639 bw_matchbox-0.3.0/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.451048 bw_matchbox-0.3.0/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.3.0/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20517 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.455962 bw_matchbox-0.3.0/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4480 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.453494 bw_matchbox-0.3.0/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.3.0/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.3.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1935 2023-08-02 21:10:16.458064 bw_matchbox-0.3.0/setup.cfg
```

### Comparing `bw_matchbox-0.2.3/LICENSE` & `bw_matchbox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/PKG-INFO` & `bw_matchbox-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.2.3
+Version: 0.3.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.2.3/README.md` & `bw_matchbox-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.3.0/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.3.0/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/js/CommonHelpers.js` & `bw_matchbox-0.3.0/bw_matchbox/assets/js/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/file.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/file.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.3.0/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.3.0/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/data/dare.json` & `bw_matchbox-0.3.0/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/utils.py` & `bw_matchbox-0.3.0/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox/webapp.py` & `bw_matchbox-0.3.0/bw_matchbox/webapp.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.3.0/bw_matchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.2.3
+Version: 0.3.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.2.3/docs/conf.py` & `bw_matchbox-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.3/setup.cfg` & `bw_matchbox-0.3.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 where = .
 exclude = 
 	tests
 
 [options.package_data]
 bw_matchbox = 
 	assets/js/*.js
+	assets/js/ProcessesList/*.js
+	assets/js/Compare/*.js
 	assets/images/*.ico
 	assets/templates/*.html
 	assets/css/*.css
 	data/*.json
 	VERSION
 
 [options.extras_require]
```

