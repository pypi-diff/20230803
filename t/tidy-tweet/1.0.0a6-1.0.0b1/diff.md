# Comparing `tmp/tidy_tweet-1.0.0a6.tar.gz` & `tmp/tidy_tweet-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0a6.tar", last modified: Thu Aug  3 04:10:27 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0b1.tar", last modified: Thu Aug  3 05:19:06 2023, max compression
```

## Comparing `tidy_tweet-1.0.0a6.tar` & `tidy_tweet-1.0.0b1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.321129 tidy_tweet-1.0.0a6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 04:10:27.329129 tidy_tweet-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 04:10:27.329129 tidy_tweet-1.0.0a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.321129 tidy_tweet-1.0.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.405187 tidy_tweet-1.0.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.409187 tidy_tweet-1.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.409187 tidy_tweet-1.0.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.405187 tidy_tweet-1.0.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.409187 tidy_tweet-1.0.0b1/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0a6/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0b1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/.github/workflows/tests.yml` & `tidy_tweet-1.0.0b1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/LICENSE` & `tidy_tweet-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/PKG-INFO` & `tidy_tweet-1.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 1.0.0a6
+Version: 1.0.0b1
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a6/README.md` & `tidy_tweet-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/contributing.md` & `tidy_tweet-1.0.0b1/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/docs/data_model.drawio` & `tidy_tweet-1.0.0b1/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/docs/data_model.svg` & `tidy_tweet-1.0.0b1/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/docs/schema.md` & `tidy_tweet-1.0.0b1/docs/schema.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/generate_schema_diagram.py` & `tidy_tweet-1.0.0b1/generate_schema_diagram.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/setup.cfg` & `tidy_tweet-1.0.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0b1/src/tidy_tweet/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,23 @@
 
 logger = getLogger(__name__)
 
 
 @click.command()
 @click.argument("database", type=click.Path(path_type=Path), required=True)
 @click.argument("json_files", type=click.Path(exists=True), nargs=-1)
-def tidy_twarc_jsons(database: Path, json_files: Collection[Union[str, PathLike]]):
+@click.option(
+    "--strict/--no_strict",
+    default=True,
+    help="Should the SQLite tables be created in strict mode (defaults to yes)? "
+    "Irrelevant if adding files to an existing database.",
+)
+def tidy_twarc_jsons(
+    database: Path, json_files: Collection[Union[str, PathLike]], strict
+):
     """
     Tidies Twitter json collected with Twarc into relational tables.
 
     Can take one or more JSON_FILES (produced by Twarc) as input, tidies the
     tweet data within those files, and stores the date in DATABASE.
 
     DATABASE is the filename for the tidy data database (should end in .db), for
@@ -51,15 +59,15 @@
         except Exception as e:
             raise e
 
         click.echo("Using existing tidy tweet database: " + str(database))
     else:
         # If database doesn't exist, initialise it
         click.echo("Creating new tidy tweet database: " + str(database))
-        db.initialise_sqlite(database)
+        db.initialise_sqlite(database, strict_mode=strict)
 
     # Load files into database
     num_files = len(json_files)
     n = 0
     total_pages = 0
     for file in json_files:
         n = n + 1  # Count files for user messaging only
```

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0b1/src/tidy_tweet/database.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0b1/src/tidy_tweet/processing.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0b1/src/tidy_tweet/tweet_mapping.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0b1/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 1.0.0a6
+Version: 1.0.0b1
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0b1/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/tests/test_cli.py` & `tidy_tweet-1.0.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a6/tests/test_overall.py` & `tidy_tweet-1.0.0b1/tests/test_overall.py`

 * *Files identical despite different names*

