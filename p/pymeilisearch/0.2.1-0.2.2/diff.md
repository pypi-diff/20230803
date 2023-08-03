# Comparing `tmp/pymeilisearch-0.2.1.tar.gz` & `tmp/pymeilisearch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeilisearch-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pymeilisearch-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pymeilisearch-0.2.1.tar` & `pymeilisearch-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1089 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/LICENSE
--rw-r--r--   0        0        0     4870 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/README.rst
--rw-r--r--   0        0        0     2114 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      317 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/__init__.py
--rw-r--r--   0        0        0      167 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/__main__.py
--rw-r--r--   0        0        0     4082 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/all_doc_indexer.py
--rw-r--r--   0        0        0     3781 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/cli.py
--rw-r--r--   0        0        0     3195 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/client.py
--rw-r--r--   0        0        0     5209 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/create_indexes.py
--rw-r--r--   0        0        0     5353 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/get_pages.py
--rw-r--r--   0        0        0     6890 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/scrapper.py
--rw-r--r--   0        0        0     3761 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/server.py
--rw-r--r--   0        0        0     3853 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/__init__.py
--rw-r--r--   0        0        0      412 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/default.json
--rw-r--r--   0        0        0      597 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/sphinx_pydata.json
--rw-r--r--   0        0        0     1349 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/utils.py
--rw-r--r--   0        0        0     3665 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/utils.py
--rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 pymeilisearch-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4870 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/README.rst
+-rw-r--r--   0        0        0     2114 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/__init__.py
+-rw-r--r--   0        0        0      167 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/__main__.py
+-rw-r--r--   0        0        0     4082 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/all_doc_indexer.py
+-rw-r--r--   0        0        0     3781 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/cli.py
+-rw-r--r--   0        0        0     3195 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/client.py
+-rw-r--r--   0        0        0     5209 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/create_indexes.py
+-rw-r--r--   0        0        0     5353 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/get_pages.py
+-rw-r--r--   0        0        0     6858 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/scrapper.py
+-rw-r--r--   0        0        0     3761 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/server.py
+-rw-r--r--   0        0        0     3853 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/__init__.py
+-rw-r--r--   0        0        0      412 2023-08-03 13:30:44.075391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/default.json
+-rw-r--r--   0        0        0      644 2023-08-03 13:30:44.079391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/sphinx_pydata.json
+-rw-r--r--   0        0        0     1349 2023-08-03 13:30:44.079391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/utils.py
+-rw-r--r--   0        0        0     3665 2023-08-03 13:30:44.079391 pymeilisearch-0.2.2/src/ansys/tools/meilisearch/utils.py
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 pymeilisearch-0.2.2/PKG-INFO
```

### Comparing `pymeilisearch-0.2.1/LICENSE` & `pymeilisearch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/README.rst` & `pymeilisearch-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/pyproject.toml` & `pymeilisearch-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pymeilisearch"
-version = "0.2.1"
+version = "0.2.2"
 description = " A Python library for effortless indexing and searching of documentation using MeiliSearch."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/all_doc_indexer.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/all_doc_indexer.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/cli.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/cli.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/client.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/client.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/create_indexes.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/create_indexes.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/get_pages.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/get_pages.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/scrapper.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/scrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         str
             Name of the temporary configuration file that was created.
         """
         temp_config_file = get_temp_file_name(".json")
         render_template(
             template, url, temp_config_file, index_uid=index_uid, stop_urls_default=stop_urls
         )
-        print(temp_config_file)
         return temp_config_file
 
     def _scrape_url_command(self, temp_config_file):
         """
         Scrape the URL for a web page.
 
         Parameters
```

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/server.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/server.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/__init__.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/sphinx_pydata.json` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/sphinx_pydata.json`

 * *Files 17% similar despite different names*

```diff
@@ -13,9 +13,9 @@
         "lvl3": ".bd-content h3",
         "lvl4": ".bd-content h4",
         "lvl5": ".bd-content h5",
         "lvl6": ".bd-content h6",
         "text": ".bd-content p, .bd-content li, .bd-content td"
     },
     "strip_chars": " .,;:#",
-    "min_indexed_level": 2
+    "selectors_exclude": [".bd-sidebar-primary", ".bd-sidebar-secondary"]
   }
```

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/utils.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/templates/utils.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/utils.py` & `pymeilisearch-0.2.2/src/ansys/tools/meilisearch/utils.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.1/PKG-INFO` & `pymeilisearch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeilisearch
-Version: 0.2.1
+Version: 0.2.2
 Summary:  A Python library for effortless indexing and searching of documentation using MeiliSearch.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys Core Team <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

