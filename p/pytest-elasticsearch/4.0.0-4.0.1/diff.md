# Comparing `tmp/pytest-elasticsearch-4.0.0.tar.gz` & `tmp/pytest-elasticsearch-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-elasticsearch-4.0.0.tar", last modified: Fri Jul 28 19:11:33 2023, max compression
+gzip compressed data, was "pytest-elasticsearch-4.0.1.tar", last modified: Thu Aug  3 12:59:09 2023, max compression
```

## Comparing `pytest-elasticsearch-4.0.0.tar` & `pytest-elasticsearch-4.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/pytest_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:59:09.027833 pytest-elasticsearch-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-08-03 12:59:09.027833 pytest-elasticsearch-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:59:09.023833 pytest-elasticsearch-4.0.1/pytest_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:57.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:59:09.023833 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-08-03 12:59:09.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-03 12:59:09.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:59:09.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 12:59:09.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 12:59:09.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 12:59:09.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:59:08.000000 pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:59:09.027833 pytest-elasticsearch-4.0.1/setup.cfg
```

### Comparing `pytest-elasticsearch-4.0.0/CHANGES.rst` & `pytest-elasticsearch-4.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+4.0.1 (2023-08-03)
+==================
+
+Bugfixes
+--------
+
+- Fixed compatibility with elasticsearch client 7.x (`#512 <https://github.com/ClearcodeHQ/pytest-elasticsearch/issues/512>`__)
+
+
 4.0.0 (2023-07-28)
 ==================
 
 Breaking changes
 ----------------
 
 - Drop support for elastisearch older than 7 (`#384 <https://github.com/ClearcodeHQ/pytest-elasticsearch/issues/384>`__)
```

### Comparing `pytest-elasticsearch-4.0.0/CONTRIBUTING.rst` & `pytest-elasticsearch-4.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/COPYING` & `pytest-elasticsearch-4.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/COPYING.lesser` & `pytest-elasticsearch-4.0.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/PKG-INFO` & `pytest-elasticsearch-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytest-elasticsearch
-Version: 4.0.0
+Version: 4.0.1
 Summary: Elasticsearch fixtures and fixture factories for Pytest.
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-elasticsearch
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-elasticsearch/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-elasticsearch/blob/v4.0.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-elasticsearch/blob/v4.0.1/CHANGES.rst
 Keywords: tests,pytest,fixture,elasticsearch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-elasticsearch-4.0.0/README.rst` & `pytest-elasticsearch-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/pyproject.toml` & `pytest-elasticsearch-4.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-elasticsearch"
-version = "4.0.0"
+version = "4.0.1"
 description = "Elasticsearch fixtures and fixture factories for Pytest."
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "elasticsearch"]
 license = {file = "LICENSE"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -26,22 +26,22 @@
     "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
 ]
 dependencies = [
     "pytest >= 6.2",
     "port-for >= 0.7.1",
     "mirakuru",
-    "elasticsearch",
+    "elasticsearch >= 7",
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-elasticsearch"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-elasticsearch/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-elasticsearch/blob/v4.0.0/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-elasticsearch/blob/v4.0.1/CHANGES.rst"
 
 [project.entry-points."pytest11"]
 pytest_elasticsearch = "pytest_elasticsearch.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -102,15 +102,15 @@
 
 [[tool.towncrier.type]]
 directory = "misc"
 name = "Miscellaneus"
 showcontent = false
 
 [tool.tbump.version]
-current = "4.0.0"
+current = "4.0.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch/__init__.py` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-elasticsearch.  If not, see <http://www.gnu.org/licenses/>.
 """Main packge for pytest-elasticsearch."""
-__version__ = "4.0.0"
+__version__ = "4.0.1"
```

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch/config.py` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch/executor.py` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch/executor.py`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch/factories.py` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """Fixture factories."""
 import shutil
 from pathlib import Path
 from typing import Callable, Iterator, Optional
 
 import pytest
 from elasticsearch import Elasticsearch
+from elasticsearch import __version__ as elastic_version
 from mirakuru import ProcessExitedWithError
 from port_for import get_port
 from port_for.api import PortType
 from pytest import FixtureRequest, TempPathFactory
 
 from pytest_elasticsearch.config import get_config
 from pytest_elasticsearch.executor import ElasticSearchExecutor, NoopElasticsearch
@@ -97,15 +98,14 @@
             logs_path,
             work_path,
             elasticsearch_cluster_name,
             elasticsearch_network_publish_host,
             elasticsearch_index_store_type,
             timeout=60,
         )
-        print(elasticsearch_executor.command)
 
         elasticsearch_executor.start()
         yield elasticsearch_executor
         try:
             elasticsearch_executor.stop()
         except ProcessExitedWithError:
             pass
@@ -157,14 +157,15 @@
         if not process.running():
             process.start()
         client = Elasticsearch(
             hosts=[{"host": process.host, "port": process.port, "scheme": "http"}],
             request_timeout=30,
             verify_certs=False,
         )
-        client.options(ignore_status=400)
+        if elastic_version >= (8, 0, 0):
+            client.options(ignore_status=400)
 
         yield client
         for index in client.indices.get_alias():
             client.indices.delete(index=index)
 
     return elasticsearch_fixture
```

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch/plugin.py` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/PKG-INFO` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytest-elasticsearch
-Version: 4.0.0
+Version: 4.0.1
 Summary: Elasticsearch fixtures and fixture factories for Pytest.
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-elasticsearch
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-elasticsearch/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-elasticsearch/blob/v4.0.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-elasticsearch/blob/v4.0.1/CHANGES.rst
 Keywords: tests,pytest,fixture,elasticsearch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/SOURCES.txt` & `pytest-elasticsearch-4.0.1/pytest_elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

