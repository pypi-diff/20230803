# Comparing `tmp/mozilla_nimbus_schemas-2023.7.1.tar.gz` & `tmp/mozilla_nimbus_schemas-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_nimbus_schemas-2023.7.1.tar", max compression
+gzip compressed data, was "mozilla_nimbus_schemas-2023.8.1.tar", max compression
```

## Comparing `mozilla_nimbus_schemas-2023.7.1.tar` & `mozilla_nimbus_schemas-2023.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    16725 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/LICENSE
--rw-r--r--   0        0        0      839 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/README.md
--rw-r--r--   0        0        0        0 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/__init__.py
--rw-r--r--   0        0        0      824 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/__init__.py
--rw-r--r--   0        0        0      624 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/analysis_errors.py
--rw-r--r--   0        0        0     1591 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/metadata.py
--rw-r--r--   0        0        0     1264 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/population_sizing.py
--rw-r--r--   0        0        0      753 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/statistics.py
--rw-r--r--   0        0        0     4646 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py
--rw-r--r--   0        0        0     2266 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py
--rw-r--r--   0        0        0     3947 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_population_sizing.py
--rw-r--r--   0        0        0     2521 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py
--rw-r--r--   0        0        0     1043 2023-07-25 12:47:08.313301 mozilla_nimbus_schemas-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.7.1/setup.py
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/LICENSE
+-rw-r--r--   0        0        0      839 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/__init__.py
+-rw-r--r--   0        0        0      824 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/__init__.py
+-rw-r--r--   0        0        0      624 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/analysis_errors.py
+-rw-r--r--   0        0        0     1560 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/metadata.py
+-rw-r--r--   0        0        0     1239 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/population_sizing.py
+-rw-r--r--   0        0        0      753 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/statistics.py
+-rw-r--r--   0        0        0     4646 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py
+-rw-r--r--   0        0        0     2266 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py
+-rw-r--r--   0        0        0     3843 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_population_sizing.py
+-rw-r--r--   0        0        0     2521 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py
+-rw-r--r--   0        0        0     1043 2023-08-03 15:29:19.159890 mozilla_nimbus_schemas-2023.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.8.1/setup.py
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.8.1/PKG-INFO
```

### Comparing `mozilla_nimbus_schemas-2023.7.1/LICENSE` & `mozilla_nimbus_schemas-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/README.md` & `mozilla_nimbus_schemas-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/__init__.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/analysis_errors.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/analysis_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/metadata.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pydantic import BaseModel, HttpUrl, validator
 
 from mozilla_nimbus_schemas.jetstream.statistics import SCHEMA_VERSION, AnalysisBasis
 
 
 def nonstrict_json_loads(*args, **kwargs):
-    kwargs.update({"strict": False})
+    kwargs["strict"] = False
     return json.loads(*args, **kwargs)
 
 
 class Metric(BaseModel):
     analysis_bases: list[AnalysisBasis]
     bigger_is_better: bool
     description: Optional[str] = None
@@ -46,14 +46,12 @@
     external_config: Optional[ExternalConfig] = None
     metrics: dict[str, Metric]
     outcomes: dict[str, Outcome] = {}
     schema_version: int = SCHEMA_VERSION
 
     @validator("analysis_start_time", pre=True)
     def treat_empty_str_as_none(cls, v):
-        if v == "":
-            return None
-        return v
+        return None if v == "" else v
 
     class Config:
         # override json_loads because `description` field in Metric may contain \n
         json_loads = nonstrict_json_loads
```

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/population_sizing.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/population_sizing.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 class SizingRecipe(BaseModel):
     app_id: str
     channel: SizingReleaseChannel
     locale: str
     country: str
     new_or_existing: SizingUserType
-    minimum_version: str
 
 
 class SizingTarget(BaseModel):
     target_recipe: SizingRecipe
     sample_sizes: dict[str, SizingDetails]
```

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/jetstream/statistics.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/jetstream/statistics.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_population_sizing.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_population_sizing.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 
 
 class TestPopulationSizing(TestCase):
     def test_parse_population_sizing(self):
         """Test against known good data."""
         sizing_test_data = """
         {
-            "firefox_desktop:release:['EN-US']:US:108": {
+            "firefox_desktop:release:['EN-US']:US": {
                 "new": {
                     "target_recipe": {
                         "app_id": "firefox_desktop",
                         "channel": "release",
                         "locale": "('EN-US')",
                         "country": "US",
-                        "new_or_existing": "new",
-                        "minimum_version": "108"
+                        "new_or_existing": "new"
                     },
                     "sample_sizes": {
                         "Power0.8EffectSize0.05": {
                             "metrics": {
                                 "active_hours": {
                                     "number_of_clients_targeted": 35,
                                     "sample_size_per_branch": 3.0,
@@ -51,16 +50,15 @@
                 },
                 "existing": {
                     "target_recipe": {
                         "app_id": "firefox_desktop",
                         "channel": "release",
                         "locale": "('EN-US')",
                         "country": "US",
-                        "new_or_existing": "existing",
-                        "minimum_version": "108"
+                        "new_or_existing": "existing"
                     },
                     "sample_sizes": {
                         "Power0.8EffectSize0.05": {
                             "metrics": {
                                 "active_hours": {
                                     "number_of_clients_targeted": 10000,
                                     "sample_size_per_branch": 100000.0,
```

### Comparing `mozilla_nimbus_schemas-2023.7.1/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py` & `mozilla_nimbus_schemas-2023.8.1/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.7.1/pyproject.toml` & `mozilla_nimbus_schemas-2023.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mozilla-nimbus-schemas"
-version = "2023.7.1"
+version = "2023.8.1"
 description = "Schemas used by Mozilla Nimbus and related projects."
 authors = ["mikewilli"]
 license = "MPL 2.0"
 readme = "README.md"
 packages = [{include = "mozilla_nimbus_schemas"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mozilla_nimbus_schemas-2023.7.1/setup.py` & `mozilla_nimbus_schemas-2023.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'mozilla-nimbus-schemas',
-    'version': '2023.7.1',
+    'version': '2023.8.1',
     'description': 'Schemas used by Mozilla Nimbus and related projects.',
     'long_description': '# Nimbus Schemas\n\nThis directory contains a published package of schemas used by different parts of the Mozilla Nimbus experimentation ecosystem.\n\n## Versioning\n`mozilla-nimbus-schemas` uses a date-based versioning scheme. The format is `yyyy.m.#`, where `m` is the non-zero-padded month, and `#` is an incrementing number starting from 1 for each month. For example, the second release in June of 2023 would have a version of `2023.6.2`.\n\n## Installation/Usage\n### Prerequisites\n- python ^3.10\n- poetry ^1.2.2\n\nFrom project root (i.e., parent to this directory)\n- Install: `make schemas_install`\n- Run linting and tests: `make schemas_check`\n- Code formatting: `make schemas_code_format`\n\n## Schemas\n### Jetstream\n\nContains schemas describing analysis results, metadata, and errors from [Jetstream](https://github.com/mozilla/jetstream).\n',
     'author': 'mikewilli',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mozilla_nimbus_schemas-2023.7.1/PKG-INFO` & `mozilla_nimbus_schemas-2023.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-nimbus-schemas
-Version: 2023.7.1
+Version: 2023.8.1
 Summary: Schemas used by Mozilla Nimbus and related projects.
 License: MPL 2.0
 Author: mikewilli
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

