# Comparing `tmp/bento_lib-7.2.0.tar.gz` & `tmp/bento_lib-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-7.2.0.tar", last modified: Wed Jul 26 19:51:22 2023, max compression
+gzip compressed data, was "bento_lib-7.2.1.tar", last modified: Thu Aug  3 17:06:03 2023, max compression
```

## Comparing `bento_lib-7.2.0.tar` & `bento_lib-7.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-26 19:51:11.000000 bento_lib-7.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 19:51:11.000000 bento_lib-7.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-26 19:51:22.226414 bento_lib-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-26 19:51:11.000000 bento_lib-7.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.222414 bento_lib-7.2.0/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.222414 bento_lib-7.2.0/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.222414 bento_lib-7.2.0/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:51:22.226414 bento_lib-7.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-26 19:51:11.000000 bento_lib-7.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-03 17:05:53.000000 bento_lib-7.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 17:05:53.000000 bento_lib-7.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-03 17:06:03.356580 bento_lib-7.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-03 17:05:53.000000 bento_lib-7.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.352580 bento_lib-7.2.1/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.352580 bento_lib-7.2.1/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.356580 bento_lib-7.2.1/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-03 17:05:53.000000 bento_lib-7.2.1/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:06:03.352580 bento_lib-7.2.1/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-03 17:06:03.000000 bento_lib-7.2.1/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-03 17:06:03.000000 bento_lib-7.2.1/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:06:03.000000 bento_lib-7.2.1/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 17:06:03.000000 bento_lib-7.2.1/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 17:06:03.000000 bento_lib-7.2.1/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:06:03.356580 bento_lib-7.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-03 17:05:53.000000 bento_lib-7.2.1/setup.py
```

### Comparing `bento_lib-7.2.0/LICENSE` & `bento_lib-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/PKG-INFO` & `bento_lib-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 7.2.0
+Version: 7.2.1
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.2.0/README.md` & `bento_lib-7.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/auth/middleware/base.py` & `bento_lib-7.2.1/bento_lib/auth/middleware/base.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/auth/middleware/django.py` & `bento_lib-7.2.1/bento_lib/auth/middleware/django.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/auth/middleware/fastapi.py` & `bento_lib-7.2.1/bento_lib/auth/middleware/fastapi.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/auth/middleware/flask.py` & `bento_lib-7.2.1/bento_lib/auth/middleware/flask.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/drs/utils.py` & `bento_lib-7.2.1/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/events/_event_bus.py` & `bento_lib-7.2.1/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/events/notifications.py` & `bento_lib-7.2.1/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/events/types.py` & `bento_lib-7.2.1/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/responses/errors.py` & `bento_lib-7.2.1/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.2.1/bento_lib/responses/fastapi_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/responses/flask_errors.py` & `bento_lib-7.2.1/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.2.1/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.2.1/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.2.1/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/search/data_structure.py` & `bento_lib-7.2.1/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/search/operations.py` & `bento_lib-7.2.1/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/search/postgres.py` & `bento_lib-7.2.1/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/search/queries.py` & `bento_lib-7.2.1/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/types.py` & `bento_lib-7.2.1/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib/workflows.py` & `bento_lib-7.2.1/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.2.1/bento_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 7.2.0
+Version: 7.2.1
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.2.0/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.2.1/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-7.2.0/setup.py` & `bento_lib-7.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "redis>=4.5.4,<5.0",
         "requests>=2.28.1,<3",
         "Werkzeug>=2.2.3,<3",
     ],
     extras_require={
         "flask": ["Flask>=2.2.5,<3"],
         "django": ["Django>=4.2.1,<5", "djangorestframework>=3.14.0,<3.15"],
-        "fastapi": ["fastapi>=0.95.2,<0.98"],
+        "fastapi": ["fastapi>=0.95.2,<0.101"],
     },
 
     author=config["package"]["authors"],
     author_email=config["package"]["author_emails"],
 
     description="A set of common utilities and helpers for Bento platform services.",
     long_description=long_description,
```

