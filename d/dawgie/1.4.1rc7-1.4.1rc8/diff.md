# Comparing `tmp/dawgie-1.4.1rc7.tar.gz` & `tmp/dawgie-1.4.1rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.1rc7.tar", last modified: Wed Aug  2 23:45:26 2023, max compression
+gzip compressed data, was "dawgie-1.4.1rc8.tar", last modified: Thu Aug  3 01:01:14 2023, max compression
```

## Comparing `dawgie-1.4.1rc7.tar` & `dawgie-1.4.1rc8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/dawgie.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-08-02 23:14:25.000000 dawgie-1.4.1rc7/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-08-03 01:01:14.858321 dawgie-1.4.1rc8/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-08-03 01:01:14.858321 dawgie-1.4.1rc8/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-08-03 01:01:14.854321 dawgie-1.4.1rc8/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-08-03 01:01:14.000000 dawgie-1.4.1rc8/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-08-03 01:01:14.858321 dawgie-1.4.1rc8/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-08-03 00:41:50.000000 dawgie-1.4.1rc8/setup.py
```

### Comparing `dawgie-1.4.1rc7/LICENSE` & `dawgie-1.4.1rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc7/PKG-INFO` & `dawgie-1.4.1rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc7
+Version: 1.4.1rc8
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dawgie-1.4.1rc7/README.md` & `dawgie-1.4.1rc8/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc7/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.1rc8/dawgie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc7
+Version: 1.4.1rc8
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dawgie-1.4.1rc7/dawgie.egg-info/SOURCES.txt` & `dawgie-1.4.1rc8/dawgie.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,116 @@
 LICENSE
 README.md
 setup.py
 ../LICENSE.txt
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/context.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/security.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/util.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/lockview.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/post.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/test.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/testdata.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/shelve/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/shelve/comms.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/shelve/enums.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/shelve/model.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/shelve/state.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/shelve/util.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/dbsinfo.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/extract.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/inter.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/list.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/post2shelve.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/purge.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/sandbox.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/util.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/tools/worm.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/util/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/db/util/aspect.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/de/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/de/html.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/__main__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/app.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/requirements.txt
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/submit.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/svrender.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/images/loading.gif
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/javascripts/algorithms_table.js
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/javascripts/application.js
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/javascripts/db.js
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/javascripts/schedule.js
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/javascripts/tasks_table.js
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/javascripts/welcome.js
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/about/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/algorithms/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/command/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/database/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/database/primary_table/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/database/targets/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/database/tasks/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/database/versions/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/exoplanet_systems/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/logs/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/pipelines/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/schedule/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/search/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/pages/tasks/index.html
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/fe/stylesheets/application.css
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/__main__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/dag.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/farm.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/jobinfo.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/message.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/promotion.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/resources.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/scan.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/schedule.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/snapshot.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/state.dot
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/state.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/util.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/version.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/logger/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/logger/fe.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/worker/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/worker/__main__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/worker/aws.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/pl/worker/cluster.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/__init__.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/compliant.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/dag.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/detach.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/logfile.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/resources.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/submit.py
-/tmp/tmp.m8WFuGRiT9/Python/dawgie/tools/trace.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/context.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/security.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/util.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/lockview.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/post.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/test.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/testdata.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/shelve/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/shelve/comms.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/shelve/enums.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/shelve/model.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/shelve/state.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/shelve/util.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/dbsinfo.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/extract.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/inter.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/list.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/post2shelve.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/purge.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/sandbox.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/util.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/tools/worm.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/util/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/db/util/aspect.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/de/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/de/html.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/__main__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/app.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/requirements.txt
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/submit.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/svrender.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/images/loading.gif
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/javascripts/algorithms_table.js
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/javascripts/application.js
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/javascripts/db.js
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/javascripts/schedule.js
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/javascripts/tasks_table.js
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/javascripts/welcome.js
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/about/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/algorithms/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/command/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/database/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/database/primary_table/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/database/targets/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/database/tasks/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/database/versions/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/exoplanet_systems/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/logs/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/pipelines/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/schedule/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/search/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/pages/tasks/index.html
+/tmp/tmp.L4cUi8X24G/Python/dawgie/fe/stylesheets/application.css
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/__main__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/dag.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/farm.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/jobinfo.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/message.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/promotion.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/resources.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/scan.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/schedule.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/snapshot.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/state.dot
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/state.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/util.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/version.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/logger/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/logger/fe.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/worker/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/worker/__main__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/worker/aws.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/pl/worker/cluster.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/__init__.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/compliant.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/dag.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/detach.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/logfile.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/resources.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/submit.py
+/tmp/tmp.L4cUi8X24G/Python/dawgie/tools/trace.py
 dawgie.egg-info/PKG-INFO
 dawgie.egg-info/SOURCES.txt
 dawgie.egg-info/dependency_links.txt
 dawgie.egg-info/requires.txt
 dawgie.egg-info/top_level.txt
```

### Comparing `dawgie-1.4.1rc7/setup.py` & `dawgie-1.4.1rc8/setup.py`

 * *Files identical despite different names*

