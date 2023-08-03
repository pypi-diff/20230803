# Comparing `tmp/tidy_tweet-1.0.0a5.tar.gz` & `tmp/tidy_tweet-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0a5.tar", last modified: Tue Aug  1 07:12:34 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0a6.tar", last modified: Thu Aug  3 04:10:27 2023, max compression
```

## Comparing `tidy_tweet-1.0.0a5.tar` & `tidy_tweet-1.0.0a6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.277779 tidy_tweet-1.0.0a5/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17895 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 07:12:34.000000 tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:12:34.281779 tidy_tweet-1.0.0a5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 07:12:13.000000 tidy_tweet-1.0.0a5/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.321129 tidy_tweet-1.0.0a6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 04:10:27.329129 tidy_tweet-1.0.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 04:10:27.329129 tidy_tweet-1.0.0a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.321129 tidy_tweet-1.0.0a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 04:10:27.000000 tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:10:27.325129 tidy_tweet-1.0.0a6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 04:10:04.000000 tidy_tweet-1.0.0a6/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0a5/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0a6/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/.github/workflows/tests.yml` & `tidy_tweet-1.0.0a6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/LICENSE` & `tidy_tweet-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/PKG-INFO` & `tidy_tweet-1.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a5/README.md` & `tidy_tweet-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/contributing.md` & `tidy_tweet-1.0.0a6/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/docs/data_model.drawio` & `tidy_tweet-1.0.0a6/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/docs/data_model.svg` & `tidy_tweet-1.0.0a6/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/docs/schema.md` & `tidy_tweet-1.0.0a6/docs/schema.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/generate_schema_diagram.py` & `tidy_tweet-1.0.0a6/generate_schema_diagram.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/setup.cfg` & `tidy_tweet-1.0.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0a6/src/tidy_tweet/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0a6/src/tidy_tweet/database.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0a6/src/tidy_tweet/processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from logging import getLogger
 from tidy_tweet.utilities import add_mappings
 
 logger = getLogger(__name__)
 
 
 def _load_page_object(
-    file_name: str, page_json: Mapping, connection: sqlite3.Connection
+    file_name: str, page_num: int, page_json: Mapping, connection: sqlite3.Connection
 ):
     """
     Takes a page of twarc Twitter API results and loads it into the database.
 
     If using this function to parse Twitter data from an object direct from Twarc
     without saving the JSON Twarc output, we recommend you save the raw data Twarc json
     output by some other means.
@@ -29,17 +29,19 @@
     # Metadata
     logger.debug("Processing metadata section of page")
     twitter_metadata = page_json.get("meta", {})
     twarc_metadata = page_json.get("__twarc", {})
     # Write this first so we can get the page id
     db.execute(
         mapping.sql_by_table["results_page"]["insert"],
-        mapping.map_page_metadata(file_name, twitter_metadata, twarc_metadata),
+        mapping.map_page_metadata(
+            file_name, page_num, twitter_metadata, twarc_metadata
+        ),
     )
-    page_info = (file_name, db.lastrowid)
+    page_info = (file_name, page_num)
 
     # Includes
     logger.debug("Processing includes section of page")
     if "media" in page_json["includes"]:
         add_mappings(mappings, mapping.map_media(page_json["includes"]["media"]))
 
     for user in page_json["includes"].get("users", []):
@@ -98,15 +100,15 @@
 
         page_num = 0
         for page in json_fh:
             page_num = page_num + 1
             logger.info(f"Processing page {page_num} of {filename}")
             page_json = json.loads(page)
             try:
-                _load_page_object(str(filename), page_json, connection)
+                _load_page_object(str(filename), page_num, page_json, connection)
             except Exception as e:
                 raise PageParsingError(filename, page_num) from e
 
         logger.info(f"All {page_num} pages of {filename} processed")
     return page_num
```

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0a6/src/tidy_tweet/tweet_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,36 +315,36 @@
     protected text,
     description text,
     location text,
     pinned_tweet_id text,
     verified integer, -- boolean
     url text,
     username text,
-    page_id integer references results_page (id),
+    source_page integer references results_page (page),
     source_file text references results_page (file_name),
-    primary key (id, page_id)
+    primary key (id, source_file, source_page)
 )
     """,
     "insert": """
 insert or ignore into user_by_page (
     id, username, name, url,
     profile_image_url, description,
     created_at,
     protected, verified,
     location,
     pinned_tweet_id,
-    page_id, source_file
+    source_page, source_file
 ) values (
     :id, :username, :name, :url,
     :profile_image_url, :description,
     :created_at,
     :protected, :verified,
     :location,
     :pinned_tweet_id,
-    :page_id, :source_file
+    :page_num, :source_file
 )
     """,
 }
 sql_views[
     "user"
 ] = """
 create view user as
@@ -353,34 +353,36 @@
     profile_image_url, description,
     created_at,
     protected, verified,
     location,
     pinned_tweet_id,
     max(retrieved_at) as retrieved_at
 from user_by_page
-left join results_page on user_by_page.page_id = results_page.id
+left join results_page on
+    user_by_page.source_page = results_page.page
+    and user_by_page.source_file = results_page.file_name
 group by user_by_page.id
 """
 
 
-def map_user(user_json, source_file, page_id) -> Dict[str, List[Dict]]:
+def map_user(user_json, source_file, page_num) -> Dict[str, List[Dict]]:
     user_map = {
         "id": user_json["id"],
         "username": user_json["username"],
         "name": user_json["name"],
         "url": user_json["url"],
         "profile_image_url": user_json["profile_image_url"],
         "description": user_json.get("description", None),
         "created_at": user_json["created_at"],
         "protected": user_json["protected"],
         "verified": user_json["verified"],
         "location": user_json.get("location", None),
         "pinned_tweet_id": user_json.get("pinned_tweet_id", None),
         "source_file": source_file,
-        "page_id": page_id,
+        "page_num": page_num,
     }
 
     mappings = {"user_by_page": [user_map]}
 
     # Entities
     if "entities" in user_json:
         for field, entities in user_json["entities"].items():
@@ -396,15 +398,15 @@
 # - entities
 # - context_annotations
 
 sql_by_table["tweet_by_page"] = {
     "create": """
 create table tweet_by_page (
     id text,
-    page_id integer references results_page (id),
+    source_page integer references results_page (page),
     reply_settings text,
     conversation_id text,
     created_at text,
     retweeted_tweet_id text references tweet (id),
     quoted_tweet_id text references tweet (id),
     replied_to_tweet_id text references tweet (id),
     in_reply_to_user_id text references user (id),
@@ -415,42 +417,42 @@
     possibly_sensitive integer, -- boolean
     like_count integer,
     quote_count integer,
     reply_count integer,
     retweet_count integer,
     source_file text references results_page (file_name),
     directly_collected integer, -- boolean
-    primary key (id, page_id)
+    primary key (id, source_file, source_page)
 )
     """,
     "insert": """
 insert or ignore into tweet_by_page (
     id, author_id,
     text, lang, source,
     possibly_sensitive, reply_settings,
     created_at,
     conversation_id,
     retweeted_tweet_id,
     quoted_tweet_id,
     replied_to_tweet_id,
     in_reply_to_user_id,
     like_count, quote_count, reply_count, retweet_count,
-    directly_collected, source_file, page_id
+    directly_collected, source_file, source_page
 ) values (
     :id, :author_id,
     :text, :lang, :source,
     :possibly_sensitive, :reply_settings,
     :created_at,
     :conversation_id,
     :retweeted_tweet_id,
     :quoted_tweet_id,
     :replied_to_tweet_id,
     :in_reply_to_user_id,
     :like_count, :quote_count, :reply_count, :retweet_count,
-    :directly_collected, :source_file, :page_id
+    :directly_collected, :source_file, :source_page
 )
     """,
 }
 sql_views[
     "tweet"
 ] = """
 create view tweet as
@@ -463,21 +465,23 @@
     retweeted_tweet_id,
     quoted_tweet_id,
     replied_to_tweet_id,
     in_reply_to_user_id,
     like_count, quote_count, reply_count, retweet_count,
     max(retrieved_at) as retrieved_at
 from tweet_by_page
-left join results_page on tweet_by_page.page_id = results_page.id
+left join results_page on
+    tweet_by_page.source_page = results_page.page
+    and tweet_by_page.source_file = results_page.file_name
 group by tweet_by_page.id
 """
 
 
 def map_tweet(
-    tweet_json, directly_collected: bool, source_file: str, page_id
+    tweet_json, directly_collected: bool, source_file: str, page_num
 ) -> Dict[str, List[Dict]]:
     tweet_map = {
         "id": tweet_json["id"],
         "author_id": tweet_json["author_id"],
         "text": tweet_json["text"],
         "lang": tweet_json["lang"],
         "source": tweet_json.get("source", None),
@@ -488,15 +492,15 @@
         "in_reply_to_user_id": None,
         "like_count": tweet_json["public_metrics"]["like_count"],
         "quote_count": tweet_json["public_metrics"]["quote_count"],
         "reply_count": tweet_json["public_metrics"]["reply_count"],
         "retweet_count": tweet_json["public_metrics"]["retweet_count"],
         "directly_collected": directly_collected,
         "source_file": source_file,
-        "page_id": page_id,
+        "source_page": page_num,
     }
 
     if "in_reply_to_user_id" in tweet_json:
         tweet_map["in_reply_to_user_id"] = tweet_json["in_reply_to_user_id"]
 
     # A tweet can have no more than one referenced tweet per type, but may have
     # multiple references of different types.
@@ -530,36 +534,37 @@
 
 
 # --- Metadata ---
 # --- Results files
 sql_by_table["results_page"] = {
     "create": """
 create table results_page (
-    id integer primary key,
+    page integer,  -- page number within the file
     file_name text,
     oldest_id text,  -- oldest tweet id in page
     newest_id text,  -- newest tweet id in page
     result_count integer,  -- count given in API response
     inserted_at text default current_timestamp,
     twarc_version text,
     tidy_tweet_version text,
     retrieved_at text, -- time response from twitter was recorded
     request_url text,
-    additional_metadata text -- extra metadata from twarc and twitter
+    additional_metadata text, -- extra metadata from twarc and twitter
+    primary key (file_name, page)
 )
     """,
     "insert": """
 insert into results_page (
-    file_name,
+    page, file_name,
     oldest_id, newest_id, result_count,
     retrieved_at, request_url,
     twarc_version, tidy_tweet_version,
     additional_metadata
 ) values (
-    :file_name,
+    :page, :file_name,
     :oldest_id, :newest_id, :result_count,
     :retrieved_at, :request_url,
     :twarc_version, :tidy_tweet_version,
     :additional_metadata
 )
     """,
 }
@@ -579,17 +584,17 @@
     max(retrieved_at) as retrieved_at_max -- latest retrieval time for pages in file
 from results_page
 group by file_name
 """
 
 
 def map_page_metadata(
-    filename: str, page_metadata_json: Dict, twarc_metadata_json: Dict
+    filename: str, page_num: int, page_metadata_json: Dict, twarc_metadata_json: Dict
 ) -> Dict:
-    metadata = {"file_name": filename}
+    metadata = {"file_name": filename, "page": page_num}
 
     # Tidy tweet metadata
     metadata["tidy_tweet_version"] = version
 
     # Twitter result page metadata
     key_columns = ["oldest_id", "newest_id", "result_count"]
     for key in key_columns:
```

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0a6/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a5/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0a6/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0a6/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/tests/test_cli.py` & `tidy_tweet-1.0.0a6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a5/tests/test_overall.py` & `tidy_tweet-1.0.0a6/tests/test_overall.py`

 * *Files identical despite different names*

