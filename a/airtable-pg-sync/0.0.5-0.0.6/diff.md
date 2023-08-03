# Comparing `tmp/airtable_pg_sync-0.0.5.tar.gz` & `tmp/airtable_pg_sync-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_pg_sync-0.0.5.tar", last modified: Wed Aug  2 17:36:15 2023, max compression
+gzip compressed data, was "airtable_pg_sync-0.0.6.tar", last modified: Wed Aug  2 18:13:43 2023, max compression
```

## Comparing `airtable_pg_sync-0.0.5.tar` & `airtable_pg_sync-0.0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.660860 airtable_pg_sync-0.0.5/
--rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.5/LICENSE
--rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.5/MANIFEST.in
--rw-r--r--   0 benurwin   (501) staff       (20)     5647 2023-08-02 17:36:15.660713 airtable_pg_sync-0.0.5/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     3962 2023-08-01 09:33:58.000000 airtable_pg_sync-0.0.5/README.md
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.655371 airtable_pg_sync-0.0.5/airtable_pg_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2770 2023-08-01 01:27:51.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/cli.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.656739 airtable_pg_sync-0.0.5/airtable_pg_sync/core/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4322 2023-08-01 00:08:07.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/change_handler.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.657561 airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4159 2023-08-01 00:08:58.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/airtable.py
--rw-r--r--   0 benurwin   (501) staff       (20)     8578 2023-08-01 00:08:40.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/postgres.py
--rw-r--r--   0 benurwin   (501) staff       (20)     7169 2023-08-01 00:09:07.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/response_parser.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1661 2023-08-01 00:06:21.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/env.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.658712 airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      708 2023-08-01 00:06:57.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/bridges.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1858 2023-08-01 00:09:12.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/changes.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/concepts.py
--rw-r--r--   0 benurwin   (501) staff       (20)      822 2023-07-30 17:51:12.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/env_types.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.659988 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      502 2023-08-01 00:07:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/initial_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     3515 2023-08-01 00:10:06.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/row_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2325 2023-08-01 00:07:51.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/schema_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2620 2023-08-01 00:09:47.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/table_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1031 2023-08-01 00:10:16.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/view_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/logging.conf
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.660402 airtable_pg_sync-0.0.5/airtable_pg_sync/perpetual_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/perpetual_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1139 2023-08-01 00:10:35.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1849 2023-08-02 17:32:42.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/perpetual_sync/webhook_listener.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1296 2023-08-01 00:05:42.000000 airtable_pg_sync-0.0.5/airtable_pg_sync/sync.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 17:36:15.656260 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/
--rw-r--r--   0 benurwin   (501) staff       (20)     5647 2023-08-02 17:36:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-02 17:36:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/SOURCES.txt
--rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-02 17:36:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/dependency_links.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-02 17:36:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/entry_points.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-02 17:36:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/requires.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-02 17:36:15.000000 airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/top_level.txt
--rw-r--r--   0 benurwin   (501) staff       (20)      859 2023-08-02 17:32:49.000000 airtable_pg_sync-0.0.5/pyproject.toml
--rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-02 17:36:15.660898 airtable_pg_sync-0.0.5/setup.cfg
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.736741 airtable_pg_sync-0.0.6/
+-rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.6/LICENSE
+-rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.6/MANIFEST.in
+-rw-r--r--   0 benurwin   (501) staff       (20)     5647 2023-08-02 18:13:43.736602 airtable_pg_sync-0.0.6/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     3962 2023-08-01 09:33:58.000000 airtable_pg_sync-0.0.6/README.md
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.731375 airtable_pg_sync-0.0.6/airtable_pg_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2770 2023-08-01 01:27:51.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/cli.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.732655 airtable_pg_sync-0.0.6/airtable_pg_sync/core/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4322 2023-08-01 00:08:07.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/change_handler.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.733524 airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4159 2023-08-01 00:08:58.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/airtable.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     8578 2023-08-01 00:08:40.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/postgres.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     7169 2023-08-01 00:09:07.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/response_parser.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1661 2023-08-01 00:06:21.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/env.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.734541 airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      708 2023-08-01 00:06:57.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/bridges.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1858 2023-08-01 00:09:12.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/changes.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/concepts.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      822 2023-07-30 17:51:12.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/env_types.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.735783 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      502 2023-08-01 00:07:15.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/initial_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     3515 2023-08-01 00:10:06.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/row_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2325 2023-08-01 00:07:51.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/schema_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2620 2023-08-01 00:09:47.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/table_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1031 2023-08-01 00:10:16.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/view_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/logging.conf
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.736298 airtable_pg_sync-0.0.6/airtable_pg_sync/perpetual_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/perpetual_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1139 2023-08-01 00:10:35.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2062 2023-08-02 18:13:27.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/perpetual_sync/webhook_listener.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1296 2023-08-01 00:05:42.000000 airtable_pg_sync-0.0.6/airtable_pg_sync/sync.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-02 18:13:43.732176 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/
+-rw-r--r--   0 benurwin   (501) staff       (20)     5647 2023-08-02 18:13:43.000000 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-02 18:13:43.000000 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-02 18:13:43.000000 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-02 18:13:43.000000 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/entry_points.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-02 18:13:43.000000 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/requires.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-02 18:13:43.000000 airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/top_level.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)      859 2023-08-02 18:13:38.000000 airtable_pg_sync-0.0.6/pyproject.toml
+-rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-02 18:13:43.736782 airtable_pg_sync-0.0.6/setup.cfg
```

### Comparing `airtable_pg_sync-0.0.5/LICENSE` & `airtable_pg_sync-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/PKG-INFO` & `airtable_pg_sync-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtable_pg_sync
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sync an Airtable base to a Postgres schema in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `airtable_pg_sync-0.0.5/README.md` & `airtable_pg_sync-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/cli.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/cli.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/change_handler.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/change_handler.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/airtable.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/airtable.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/postgres.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/postgres.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/clients/response_parser.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/clients/response_parser.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/env.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/env.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/bridges.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/bridges.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/changes.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/changes.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/concepts.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/concepts.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/core/types/env_types.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/core/types/env_types.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/row_syncer.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/row_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/schema_syncer.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/schema_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/table_syncer.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/table_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/initial_sync/view_syncer.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/initial_sync/view_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/perpetual_sync/perpetual_syncer.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/perpetual_sync/perpetual_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/perpetual_sync/webhook_listener.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/perpetual_sync/webhook_listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     async def handle_event(self, request):
         self.logger.info('Received webhook event - adding to queue')
         res = json.loads(await request.text())
         self.queue.add(res['webhook']['id'])
 
         return web.Response(text="Nice Webhook")
 
+    async def health_check(self, request):
+        return web.Response(text="I'm alive!")
+
     def create_webhook(self):
         self.logger.info('Creating webhook')
         airtable.Client().setup_webhook()
 
     def start(self):
         self.logger.info('Starting webhook listener')
         # TODO: Remove this before publishing and provide a way to set up / tear down webhooks
@@ -42,15 +45,20 @@
 
         # TODO: Provide a way to pass in webhooks too and handle error when too many have been created
 
         try:
             self.create_webhook()
 
             app = web.Application()
-            app.add_routes([web.post('/', self.handle_event)])
+            app.add_routes(
+                [
+                    web.post('/', self.handle_event),
+                    web.get('/', self.health_check)
+                 ]
+            )
             runner = web.AppRunner(app)
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
             loop.run_until_complete(runner.setup())
             site = web.TCPSite(runner, '0.0.0.0', env.LISTENER_INFO.port)
             loop.run_until_complete(site.start())
             loop.run_forever()
```

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync/sync.py` & `airtable_pg_sync-0.0.6/airtable_pg_sync/sync.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/PKG-INFO` & `airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtable-pg-sync
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sync an Airtable base to a Postgres schema in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `airtable_pg_sync-0.0.5/airtable_pg_sync.egg-info/SOURCES.txt` & `airtable_pg_sync-0.0.6/airtable_pg_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.5/pyproject.toml` & `airtable_pg_sync-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtable_pg_sync"
-version = "0.0.5"
+version = "0.0.6"
 description = "Sync an Airtable base to a Postgres schema in real time"
 readme = "README.md"
 authors = [{ name = "Benjamin Urwin", email = "benurwin@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

