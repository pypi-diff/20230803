# Comparing `tmp/osm_easy_api-1.1.0.tar.gz` & `tmp/osm_easy_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-1.1.0.tar", last modified: Fri Jul 28 18:12:54 2023, max compression
+gzip compressed data, was "osm_easy_api-1.1.1.tar", last modified: Thu Aug  3 11:36:09 2023, max compression
```

## Comparing `osm_easy_api-1.1.0.tar` & `osm_easy_api-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.039069 osm_easy_api-1.1.0/
--rw-rw-rw-   0        0        0     3874 2023-07-28 18:02:48.000000 osm_easy_api-1.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0    45559 2023-07-28 18:12:54.040069 osm_easy_api-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4947 2023-07-24 09:37:44.000000 osm_easy_api-1.1.0/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2023-07-28 18:12:54.064991 osm_easy_api-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.906185 osm_easy_api-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.936883 osm_easy_api-1.1.0/src/osm_easy_api/
--rw-rw-rw-   0        0        0      107 2023-07-28 18:03:22.000000 osm_easy_api-1.1.0/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.984165 osm_easy_api-1.1.0/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     4368 2023-07-28 17:51:03.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.000993 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    14856 2023-07-28 17:56:51.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    11507 2023-07-24 09:44:18.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.024094 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.030530 osm_easy_api-1.1.0/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.1.0/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.1.0/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.037071 osm_easy_api-1.1.0/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.975348 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    45559 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.505921 osm_easy_api-1.1.1/
+-rw-rw-rw-   0        0        0     4084 2023-08-03 11:34:19.000000 osm_easy_api-1.1.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0    45769 2023-08-03 11:36:09.506919 osm_easy_api-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2023-07-24 09:37:44.000000 osm_easy_api-1.1.1/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-08-03 11:36:09.515426 osm_easy_api-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.436298 osm_easy_api-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.448828 osm_easy_api-1.1.1/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      107 2023-08-03 11:31:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.476600 osm_easy_api-1.1.1/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3033 2023-08-03 11:30:52.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-07-28 17:51:03.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.486372 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    14856 2023-07-28 17:56:51.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    11508 2023-08-03 11:32:24.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.498397 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.1.1/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.501396 osm_easy_api-1.1.1/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.1.1/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.1.1/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.504913 osm_easy_api-1.1.1/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.1.1/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:36:09.471583 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    45769 2023-08-03 11:36:09.000000 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-08-03 11:36:09.000000 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:36:09.000000 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-08-03 11:36:09.000000 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 11:36:09.000000 osm_easy_api-1.1.1/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-1.1.0/CHANGELOG.md` & `osm_easy_api-1.1.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.1]
+### Fixed
+- Corrected character when adding parameters in endpoint `api.notes.get_bbox()` (from `?` to `&`).
+- Fixed the `limit` parameter restrictions in `api.notes.get_bbox()` documentation.
+
 ## [1.1.0]
 ### Added
 - `limit` parameter for `api.changeset.get_query()` endpoint.
 
 ### Fixed
 - Corrected character when adding parameters in endpoint `api.changeset.get_query()` (from `;` to `&`).
```

### Comparing `osm_easy_api-1.1.0/LICENSE.md` & `osm_easy_api-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/PKG-INFO` & `osm_easy_api-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -171,14 +171,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.1]
+### Fixed
+- Corrected character when adding parameters in endpoint `api.notes.get_bbox()` (from `?` to `&`).
+- Fixed the `limit` parameter restrictions in `api.notes.get_bbox()` documentation.
+
 ## [1.1.0]
 ### Added
 - `limit` parameter for `api.changeset.get_query()` endpoint.
 
 ### Fixed
 - Corrected character when adding parameters in endpoint `api.changeset.get_query()` (from `;` to `&`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm_easy_api Version: 1.1.0 Summary: Python package
+Metadata-Version: 2.1 Name: osm_easy_api Version: 1.1.1 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -65,16 +65,19 @@
 d.get(generator=False) deleted_nodes = osmChange.get(Node, Action.DELETE) for
 node in deleted_nodes: print(node.id) ``` but it can consume large amounts of
 ram and use of this method is not recommended for large diff's. # Tests You
 will need to install `test-requirements.txt`. You can use tox. To run tests
 manually use `python -m unittest discover`. # Changelog All notable changes to
 this project will be documented in this file. The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.1.0] ###
-Added - `limit` parameter for `api.changeset.get_query()` endpoint. ### Fixed -
+[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.1.1] ###
+Fixed - Corrected character when adding parameters in endpoint
+`api.notes.get_bbox()` (from `?` to `&`). - Fixed the `limit` parameter
+restrictions in `api.notes.get_bbox()` documentation. ## [1.1.0] ### Added -
+`limit` parameter for `api.changeset.get_query()` endpoint. ### Fixed -
 Corrected character when adding parameters in endpoint `api.changeset.get_query
 ()` (from `;` to `&`). ## [1.0.2] ### Fixed - Auth problems in API when using
 characters unsupported by latin-1 codec. ## [1.0.1] ### Fixed -
 `api.notes.create()` created only anonymous notes. ## [1.0.0] ### Added -
 `to_xml()` method in `OsmChange`. - `upload()` method in `changeset` `endpoint`
 has new optional arguments. - Test for `to_xml()` method in `OsmChange`. - `#
 pragma: no cover` for unexpected api errors (Those that are not in the
```

### Comparing `osm_easy_api-1.1.0/README.md` & `osm_easy_api-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/setup.cfg` & `osm_easy_api-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/_URLs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,14 @@
             "get_query": six_url + "/users?users=",
             "get_current": six_url + "/user/details",
             "preferences": six_url + "/user/preferences"
         }
 
         self.note: Dict[str, str] = {
             "get": six_url + "/notes/{id}",
-            "get_bbox": six_url + "/notes?bbox={left},{bottom},{right},{top}?limit={limit}?closed={closed_days}",
+            "get_bbox": six_url + "/notes?bbox={left},{bottom},{right},{top}&limit={limit}&closed={closed_days}",
             "create": six_url + "/notes?lat={latitude}&lon={longitude}&text={text}",
             "comment": six_url + "/notes/{id}/comment?text={text}",
             "close": six_url + "/notes/{id}/close",
             "reopen": six_url + "/notes/{id}/reopen",
             "search": six_url + "/notes/search?q={text}&limit={limit}&closed={closed}"
         }
```

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/api.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/elements.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         """Get notes in bbox.
 
         Args:
             left (str): Left bbox
             bottom (str): Bottom bbox
             right (str): Right bbox
             top (str): Top bbox
-            limit (int, optional): Max number of notes (1 < limit < 1000). Defaults to 100.
+            limit (int, optional): Max number of notes (1 < limit < 10000). Defaults to 100.
             closed_days (int, optional): Number of days a note needs to be closed to no longer be returned (0 - only open, -1 - all). Defaults to 7.
 
         Raises:
             ValueError: Any of args limit is exceeded.
 
         Returns:
             list[Note]: List of notes.
```

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-1.1.1/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/OsmChange.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/OsmChange.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/note.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/note.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/relation.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/relation.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/user.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/way.py` & `osm_easy_api-1.1.1/src/osm_easy_api/data_classes/way.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/diff/diff.py` & `osm_easy_api-1.1.1/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-1.1.1/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-1.1.1/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-easy-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -171,14 +171,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.1]
+### Fixed
+- Corrected character when adding parameters in endpoint `api.notes.get_bbox()` (from `?` to `&`).
+- Fixed the `limit` parameter restrictions in `api.notes.get_bbox()` documentation.
+
 ## [1.1.0]
 ### Added
 - `limit` parameter for `api.changeset.get_query()` endpoint.
 
 ### Fixed
 - Corrected character when adding parameters in endpoint `api.changeset.get_query()` (from `;` to `&`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-easy-api Version: 1.1.0 Summary: Python package
+Metadata-Version: 2.1 Name: osm-easy-api Version: 1.1.1 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -65,16 +65,19 @@
 d.get(generator=False) deleted_nodes = osmChange.get(Node, Action.DELETE) for
 node in deleted_nodes: print(node.id) ``` but it can consume large amounts of
 ram and use of this method is not recommended for large diff's. # Tests You
 will need to install `test-requirements.txt`. You can use tox. To run tests
 manually use `python -m unittest discover`. # Changelog All notable changes to
 this project will be documented in this file. The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.1.0] ###
-Added - `limit` parameter for `api.changeset.get_query()` endpoint. ### Fixed -
+[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.1.1] ###
+Fixed - Corrected character when adding parameters in endpoint
+`api.notes.get_bbox()` (from `?` to `&`). - Fixed the `limit` parameter
+restrictions in `api.notes.get_bbox()` documentation. ## [1.1.0] ### Added -
+`limit` parameter for `api.changeset.get_query()` endpoint. ### Fixed -
 Corrected character when adding parameters in endpoint `api.changeset.get_query
 ()` (from `;` to `&`). ## [1.0.2] ### Fixed - Auth problems in API when using
 characters unsupported by latin-1 codec. ## [1.0.1] ### Fixed -
 `api.notes.create()` created only anonymous notes. ## [1.0.0] ### Added -
 `to_xml()` method in `OsmChange`. - `upload()` method in `changeset` `endpoint`
 has new optional arguments. - Test for `to_xml()` method in `OsmChange`. - `#
 pragma: no cover` for unexpected api errors (Those that are not in the
```

### Comparing `osm_easy_api-1.1.0/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-1.1.1/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

