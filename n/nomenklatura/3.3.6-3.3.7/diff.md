# Comparing `tmp/nomenklatura-3.3.6.tar.gz` & `tmp/nomenklatura-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.6.tar", last modified: Thu Jul 27 15:01:54 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.7.tar", last modified: Thu Aug  3 07:53:47 2023, max compression
```

## Comparing `nomenklatura-3.3.6.tar` & `nomenklatura-3.3.7.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:00:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.389739 nomenklatura-3.3.7/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:52:45.000000 nomenklatura-3.3.7/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/setup.py
```

### Comparing `nomenklatura-3.3.6/LICENSE` & `nomenklatura-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/PKG-INFO` & `nomenklatura-3.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.6
+Version: 3.3.7
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.3.6/README.md` & `nomenklatura-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/cache.py` & `nomenklatura-3.3.7/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/cli.py` & `nomenklatura-3.3.7/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.7/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.7/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.7/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.7/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.7/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.7/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.7/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/dataset/util.py` & `nomenklatura-3.3.7/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/db.py` & `nomenklatura-3.3.7/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.7/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.7/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/common.py` & `nomenklatura-3.3.7/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.7/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.7/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.7/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/entity.py` & `nomenklatura-3.3.7/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/index/entry.py` & `nomenklatura-3.3.7/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/index/index.py` & `nomenklatura-3.3.7/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.7/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/judgement.py` & `nomenklatura-3.3.7/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.7/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.7/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.7/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.7/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/types.py` & `nomenklatura-3.3.7/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/util.py` & `nomenklatura-3.3.7/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.7/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.7/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.7/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.7/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.7/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.7/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.7/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.7/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.7/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.7/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.7/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.7/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/publish/dates.py` & `nomenklatura-3.3.7/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/publish/edges.py` & `nomenklatura-3.3.7/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/publish/names.py` & `nomenklatura-3.3.7/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.7/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.7/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.7/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/senzing.py` & `nomenklatura-3.3.7/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/statement/__init__.py` & `nomenklatura-3.3.7/nomenklatura/statement/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/statement/db.py` & `nomenklatura-3.3.7/nomenklatura/statement/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.7/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/statement/statement.py` & `nomenklatura-3.3.7/nomenklatura/statement/statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,14 +189,18 @@
         )
 
     @classmethod
     def from_row(cls: Type[S], data: Dict[str, str]) -> S:
         typed_data = cast(StatementDict, data)
         typed_data["target"] = text_bool(data.get("target"))
         typed_data["external"] = text_bool(data.get("external"))
+        if data.get("lang") == "":
+            typed_data["lang"] = None
+        if data.get("original_value") == "":
+            typed_data["original_value"] = None
         return cls.from_dict(typed_data)
 
     @classmethod
     def from_db_row(cls: Type[S], row: Row) -> S:
         return cls(
             id=row.id,
             canonical_id=row.canonical_id,
```

### Comparing `nomenklatura-3.3.6/nomenklatura/store/__init__.py` & `nomenklatura-3.3.7/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/store/base.py` & `nomenklatura-3.3.7/nomenklatura/store/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
     def pop(self, entity_id: str) -> List[Statement]:
         raise NotImplementedError()
 
     def flush(self) -> None:
         pass
 
+    def close(self) -> None:
+        self.store.close()
+
     def __enter__(self) -> "Writer[DS, CE]":
         return self
 
     def __exit__(
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
```

### Comparing `nomenklatura-3.3.6/nomenklatura/store/level.py` & `nomenklatura-3.3.7/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/store/memory.py` & `nomenklatura-3.3.7/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/store/util.py` & `nomenklatura-3.3.7/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/stream.py` & `nomenklatura-3.3.7/nomenklatura/stream.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/tui/app.py` & `nomenklatura-3.3.7/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.7/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/tui/util.py` & `nomenklatura-3.3.7/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/util.py` & `nomenklatura-3.3.7/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura/xref.py` & `nomenklatura-3.3.7/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.7/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.6
+Version: 3.3.7
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.3.6/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.7/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.6/setup.py` & `nomenklatura-3.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.6",
+    version="3.3.7",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

