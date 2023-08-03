# Comparing `tmp/tap-pendo-1.0.0.tar.gz` & `tmp/tap-pendo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-pendo-1.0.0.tar", last modified: Thu Jul 27 15:08:44 2023, max compression
+gzip compressed data, was "tap-pendo-1.0.1.tar", last modified: Thu Aug  3 11:19:59 2023, max compression
```

## Comparing `tap-pendo-1.0.0.tar` & `tap-pendo-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16198 2023-07-27 14:41:26.000000 tap-pendo-1.0.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      916 2023-07-27 15:05:22.000000 tap-pendo-1.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.422115 tap-pendo-1.0.0/tap_pendo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6721 2023-07-27 08:24:30.000000 tap-pendo-1.0.0/tap_pendo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5091 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/tap_pendo/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      838 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/feature_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/features.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-07-27 14:41:26.000000 tap-pendo-1.0.0/tap_pendo/schemas/guide_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6000 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/guides.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/metadata_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/metadata_visitors.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2023-07-27 08:18:39.000000 tap-pendo-1.0.0/tap_pendo/schemas/page_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/pages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/poll_events.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/tap_pendo/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/shared/metadata.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/track_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2383 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/track_types.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1262 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/visitor_history.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/visitors.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    59547 2023-07-27 14:41:26.000000 tap-pendo-1.0.0/tap_pendo/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4201 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.422115 tap-pendo-1.0.0/tap_pendo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 11:19:59.583463 tap-pendo-1.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      314 2023-08-03 11:19:59.583463 tap-pendo-1.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16198 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-08-03 11:19:59.583463 tap-pendo-1.0.1/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      916 2023-08-03 10:59:18.000000 tap-pendo-1.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 11:19:59.571463 tap-pendo-1.0.1/tap_pendo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6721 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5091 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 11:19:59.583463 tap-pendo-1.0.1/tap_pendo/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      838 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/feature_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/schemas/features.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/schemas/guide_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6000 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/schemas/guides.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/metadata_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/metadata_visitors.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/page_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/schemas/pages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/schemas/poll_events.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 11:19:59.583463 tap-pendo-1.0.1/tap_pendo/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/shared/metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/track_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2383 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/schemas/track_types.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1262 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/visitor_history.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/schemas/visitors.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    59571 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4201 2023-08-02 10:09:44.000000 tap-pendo-1.0.1/tap_pendo/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-03-27 13:02:34.000000 tap-pendo-1.0.1/tap_pendo/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 11:19:59.575463 tap-pendo-1.0.1/tap_pendo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      314 2023-08-03 11:19:59.000000 tap-pendo-1.0.1/tap_pendo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-08-03 11:19:59.000000 tap-pendo-1.0.1/tap_pendo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-03 11:19:59.000000 tap-pendo-1.0.1/tap_pendo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-08-03 11:19:59.000000 tap-pendo-1.0.1/tap_pendo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-08-03 11:19:59.000000 tap-pendo-1.0.1/tap_pendo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-08-03 11:19:59.000000 tap-pendo-1.0.1/tap_pendo.egg-info/top_level.txt
```

### Comparing `tap-pendo-1.0.0/LICENSE` & `tap-pendo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/README.md` & `tap-pendo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/setup.py` & `tap-pendo-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-pendo",
-    version="1.0.0",
+    version="1.0.1",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="https://github.com/singer-io/tap-pendo",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_pendo"],
     install_requires=[
         'singer-python==5.13.0',
```

### Comparing `tap-pendo-1.0.0/tap_pendo/__init__.py` & `tap-pendo-1.0.1/tap_pendo/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/discover.py` & `tap-pendo-1.0.1/tap_pendo/discover.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/accounts.json` & `tap-pendo-1.0.1/tap_pendo/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/events.json` & `tap-pendo-1.0.1/tap_pendo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/feature_events.json` & `tap-pendo-1.0.1/tap_pendo/schemas/feature_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/features.json` & `tap-pendo-1.0.1/tap_pendo/schemas/features.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/guide_events.json` & `tap-pendo-1.0.1/tap_pendo/schemas/guide_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/guides.json` & `tap-pendo-1.0.1/tap_pendo/schemas/guides.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/metadata_accounts.json` & `tap-pendo-1.0.1/tap_pendo/schemas/metadata_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/metadata_visitors.json` & `tap-pendo-1.0.1/tap_pendo/schemas/metadata_visitors.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/page_events.json` & `tap-pendo-1.0.1/tap_pendo/schemas/page_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/pages.json` & `tap-pendo-1.0.1/tap_pendo/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/poll_events.json` & `tap-pendo-1.0.1/tap_pendo/schemas/poll_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/shared/metadata.json` & `tap-pendo-1.0.1/tap_pendo/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/track_events.json` & `tap-pendo-1.0.1/tap_pendo/schemas/track_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/track_types.json` & `tap-pendo-1.0.1/tap_pendo/schemas/track_types.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/visitor_history.json` & `tap-pendo-1.0.1/tap_pendo/schemas/visitor_history.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/schemas/visitors.json` & `tap-pendo-1.0.1/tap_pendo/schemas/visitors.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/streams.py` & `tap-pendo-1.0.1/tap_pendo/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,15 +587,15 @@
                     last_processed.append(last)
 
         # This is a corner cases where all records in the set have same timestamp
         # This can occur if record limit is set very smaller compared to the max record limit
         # In this case we will try to set record limit to max limit to make it harder to run into this issue
         # But still can't completely dismiss the minor possibility of this issue occurring
         if len(records) == 0 or not last_processed:
-            self.record_limit = API_RECORD_LIMIT
+            self.record_limit = max(self.record_limit, API_RECORD_LIMIT)
 
         return records, last_processed
 
     def get_first_parameter_value(self, body):
         return body['request']['pipeline'][0]['source']['timeSeries'].get('first', 0)
 
     def set_time_series_first(self, body, records, first=None):
```

### Comparing `tap-pendo-1.0.0/tap_pendo/sync.py` & `tap-pendo-1.0.1/tap_pendo/sync.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo/utils.py` & `tap-pendo-1.0.1/tap_pendo/utils.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-1.0.0/tap_pendo.egg-info/SOURCES.txt` & `tap-pendo-1.0.1/tap_pendo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

