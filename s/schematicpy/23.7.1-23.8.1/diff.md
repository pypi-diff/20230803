# Comparing `tmp/schematicpy-23.7.1.tar.gz` & `tmp/schematicpy-23.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-23.7.1.tar", max compression
+gzip compressed data, was "schematicpy-23.8.1.tar", max compression
```

## Comparing `schematicpy-23.7.1.tar` & `schematicpy-23.8.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1073 2023-07-27 16:28:02.621153 schematicpy-23.7.1/LICENSE
--rw-r--r--   0        0        0    17198 2023-07-27 16:28:02.621153 schematicpy-23.7.1/README.md
--rw-r--r--   0        0        0     3356 2023-07-27 16:28:37.349772 schematicpy-23.7.1/pyproject.toml
--rw-r--r--   0        0        0     1424 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/__init__.py
--rw-r--r--   0        0        0     1421 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/__main__.py
--rw-r--r--   0        0        0        0 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/configuration/__init__.py
--rw-r--r--   0        0        0     6996 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/configuration/configuration.py
--rw-r--r--   0        0        0     5034 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/configuration/dataclasses.py
--rw-r--r--   0        0        0      663 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2023-07-27 16:28:02.625153 schematicpy-23.7.1/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     3193 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/exceptions.py
--rw-r--r--   0        0        0    10581 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/help.py
--rw-r--r--   0        0        0     3415 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/loader.py
--rw-r--r--   0        0        0       59 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/manifest/__init__.py
--rw-r--r--   0        0        0     9339 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/manifest/commands.py
--rw-r--r--   0        0        0    77864 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/manifest/generator.py
--rw-r--r--   0        0        0    22894 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/__init__.py
--rw-r--r--   0        0        0     6616 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/commands.py
--rw-r--r--   0        0        0    16680 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/metadata.py
--rw-r--r--   0        0        0    44816 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    11604 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      166 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     2470 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/commands.py
--rw-r--r--   0        0        0     4291 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/curie.py
--rw-r--r--   0        0        0    34388 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/df_parser.py
--rw-r--r--   0        0        0    46753 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/explorer.py
--rw-r--r--   0        0        0    29741 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/generator.py
--rw-r--r--   0        0        0     7070 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/validator.py
--rw-r--r--   0        0        0       96 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/store/base.py
--rw-r--r--   0        0        0   110877 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/store/synapse.py
--rw-r--r--   0        0        0        0 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/__init__.py
--rw-r--r--   0        0        0     2524 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     2785 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0     8182 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/df_utils.py
--rw-r--r--   0        0        0     6806 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/general.py
--rw-r--r--   0        0        0     7338 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1140 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/io_utils.py
--rw-r--r--   0        0        0     9804 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0     9565 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     2621 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      236 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0      119 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/version.py
--rw-r--r--   0        0        0      135 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/__init__.py
--rw-r--r--   0        0        0    10207 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     3548 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/commands.py
--rw-r--r--   0        0        0    37113 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    19629 1970-01-01 00:00:00.000000 schematicpy-23.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-03 21:25:22.531747 schematicpy-23.8.1/LICENSE
+-rw-r--r--   0        0        0    17125 2023-08-03 21:25:22.531747 schematicpy-23.8.1/README.md
+-rw-r--r--   0        0        0     3422 2023-08-03 21:26:06.967971 schematicpy-23.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/__init__.py
+-rw-r--r--   0        0        0     1421 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/configuration/__init__.py
+-rw-r--r--   0        0        0     6996 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/configuration/configuration.py
+-rw-r--r--   0        0        0     5034 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/configuration/dataclasses.py
+-rw-r--r--   0        0        0      663 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2023-08-03 21:25:22.535748 schematicpy-23.8.1/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3193 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/exceptions.py
+-rw-r--r--   0        0        0    10581 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/help.py
+-rw-r--r--   0        0        0     3415 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/loader.py
+-rw-r--r--   0        0        0       59 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0     9339 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    77864 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    22894 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/models/__init__.py
+-rw-r--r--   0        0        0     6616 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/models/commands.py
+-rw-r--r--   0        0        0    16680 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/models/metadata.py
+-rw-r--r--   0        0        0    44816 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    11604 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      166 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     2470 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     4291 2023-08-03 21:25:22.543748 schematicpy-23.8.1/schematic/schemas/curie.py
+-rw-r--r--   0        0        0    34388 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/schemas/df_parser.py
+-rw-r--r--   0        0        0    46753 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/schemas/explorer.py
+-rw-r--r--   0        0        0    29741 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/schemas/generator.py
+-rw-r--r--   0        0        0     7070 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/schemas/validator.py
+-rw-r--r--   0        0        0       96 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/store/base.py
+-rw-r--r--   0        0        0   110765 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/store/synapse.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     2524 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     2785 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0     8182 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0     8686 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/general.py
+-rw-r--r--   0        0        0     7338 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1140 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0     9804 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0     9565 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     2621 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      236 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/version.py
+-rw-r--r--   0        0        0      135 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    10207 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     3548 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    37113 2023-08-03 21:25:22.547748 schematicpy-23.8.1/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    19556 1970-01-01 00:00:00.000000 schematicpy-23.8.1/PKG-INFO
```

### Comparing `schematicpy-23.7.1/LICENSE` & `schematicpy-23.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/README.md` & `schematicpy-23.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ```
 This command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)
 
 5. Fill in credential files: 
 *Note*: If you won't interact with Synapse, please ignore this section.
 
 There are two main configuration files that need to be edited:
-[config.yml](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml)
+config.yml
 and [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)
 
 <strong>Configure .synapseConfig File</strong>
 
 Download a copy of the ``.synapseConfig`` file, open the file in the
 editor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section
```

### Comparing `schematicpy-23.7.1/pyproject.toml` & `schematicpy-23.8.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v23.7.1"
+version = "v23.8.1"
 description = "Package for biomedical data model and metadata ingress management"
 authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
@@ -70,15 +70,15 @@
 pylint = "^2.16.1"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose"
 testpaths = [ "tests",]
 filterwarnings = [ "ignore::DeprecationWarning",]
-markers = [ "google_credentials_needed: marks tests requiring Google credentials (skipped on GitHub CI) ", "schematic_api: marks tests covering API functionality (skipped on regular GitHub CI test suite)\n    ", "rule_combos: marks tests covering combinations of rules that aren't always necessary and can add significantly to CI runtime (skipped on GitHub CI unless prompted to run in commit message)\n    ", "table_operations: marks tests covering table operations that pass locally but fail on CI due to interactions with Synapse (skipped on GitHub CI)\n    ", "rule_benchmark: marks tests covering validation rule benchmarking\n    ",]
+markers = [ "google_credentials_needed: marks tests requiring Google credentials (skipped on GitHub CI) ", "not_windows: tests that don't work on on windows machine\n    ", "schematic_api: marks tests covering API functionality (skipped on regular GitHub CI test suite)\n    ", "rule_combos: marks tests covering combinations of rules that aren't always necessary and can add significantly to CI runtime (skipped on GitHub CI unless prompted to run in commit message)\n    ", "table_operations: marks tests covering table operations that pass locally but fail on CI due to interactions with Synapse (skipped on GitHub CI)\n    ", "rule_benchmark: marks tests covering validation rule benchmarking\n    ",]
 
 [tool.poetry.dependencies.connexion]
 extras = [ "swagger-ui",]
 version = "^2.8.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 markers = "python_version < \"3.9\""
```

### Comparing `schematicpy-23.7.1/schematic/__init__.py` & `schematicpy-23.8.1/schematic/__init__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/__main__.py` & `schematicpy-23.8.1/schematic/__main__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/configuration/configuration.py` & `schematicpy-23.8.1/schematic/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/configuration/dataclasses.py` & `schematicpy-23.8.1/schematic/configuration/dataclasses.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/etc/README.md` & `schematicpy-23.8.1/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-23.8.1/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-23.8.1/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-23.8.1/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-23.8.1/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-23.8.1/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/exceptions.py` & `schematicpy-23.8.1/schematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/help.py` & `schematicpy-23.8.1/schematic/help.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/loader.py` & `schematicpy-23.8.1/schematic/loader.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/manifest/commands.py` & `schematicpy-23.8.1/schematic/manifest/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/manifest/generator.py` & `schematicpy-23.8.1/schematic/manifest/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1596,15 +1596,15 @@
         # Make sure want Ids are placed at end of manifest, in given order.
         for id_name in ['Uuid', 'Id', 'entityId']:
             if id_name in end_columns:
                 end_columns.remove(id_name)
                 end_columns.append(id_name)
         
         # Add entity_id to the end columns if it should be there but isn't
-        if 'entityId' in (current_schema_headers or existing_manfiest_headers) and 'entityId' not in end_columns:
+        if 'entityId' in (current_schema_headers or existing_manifest_headers) and 'entityId' not in end_columns:
             end_columns.append('entityId')
         return end_columns
 
     def _update_dataframe_with_existing_df(self, empty_manifest_url: str, existing_df: pd.DataFrame) -> pd.DataFrame:
         """
         Handle scenario when existing manifest does not match new manifest template due to changes in the data model:
             the sheet column header reflect the latest schema the existing manifest column-set may be outdated
@@ -1617,15 +1617,15 @@
         Returns:
             updated_df (Pd.DataFrame): existing_df with new_columns added.
             out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
         """
 
         # Get headers for the current schema and existing manifest df.
         current_schema_headers = list(self.get_dataframe_by_url(manifest_url=empty_manifest_url).columns)
-        existing_manfiest_headers = list(existing_df.columns)
+        existing_manifest_headers = list(existing_df.columns)
 
         # Find columns that exist in the current schema, but are not in the manifest being downloaded.
         new_columns = self._get_missing_columns(current_schema_headers, existing_manifest_headers)
 
         # Find columns that exist in the manifest being downloaded, but not in the current schema.
         out_of_schema_columns = self._get_missing_columns(existing_manifest_headers, current_schema_headers)
```

### Comparing `schematicpy-23.7.1/schematic/models/GE_Helpers.py` & `schematicpy-23.8.1/schematic/models/GE_Helpers.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/models/commands.py` & `schematicpy-23.8.1/schematic/models/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/models/metadata.py` & `schematicpy-23.8.1/schematic/models/metadata.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/models/validate_attribute.py` & `schematicpy-23.8.1/schematic/models/validate_attribute.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/models/validate_manifest.py` & `schematicpy-23.8.1/schematic/models/validate_manifest.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/schemas/commands.py` & `schematicpy-23.8.1/schematic/schemas/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/schemas/curie.py` & `schematicpy-23.8.1/schematic/schemas/curie.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/schemas/df_parser.py` & `schematicpy-23.8.1/schematic/schemas/df_parser.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/schemas/explorer.py` & `schematicpy-23.8.1/schematic/schemas/explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/schemas/generator.py` & `schematicpy-23.8.1/schematic/schemas/generator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/schemas/validator.py` & `schematicpy-23.8.1/schematic/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/store/synapse.py` & `schematicpy-23.8.1/schematic/store/synapse.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import uuid  # used to generate unique names for entities
 import json
 import atexit
 import logging
 import secrets
 from dataclasses import dataclass
-import tempfile
+import shutil
 
 # allows specifying explicit variable types
 from typing import Dict, List, Tuple, Sequence, Union
 from collections import OrderedDict
 from tenacity import retry, stop_after_attempt, wait_chain, wait_fixed, retry_if_exception_type
 
 import numpy as np
@@ -39,25 +39,25 @@
 from synapseutils.copy_functions import changeFileMetaData
 
 import uuid
 
 from schematic_db.rdb.synapse_database import SynapseDatabase
 
 
-from schematic.utils.df_utils import update_df, load_df, col_in_dataframe, populate_df_col_with_another_col
+from schematic.utils.df_utils import update_df, load_df, col_in_dataframe
 from schematic.utils.validate_utils import comma_separated_list_regex, rule_in_rule_list
-from schematic.utils.general import entity_type_mapping, get_dir_size, convert_size, convert_gb_to_bytes, create_temp_folder
+from schematic.utils.general import entity_type_mapping, get_dir_size, convert_gb_to_bytes, create_temp_folder, check_synapse_cache_size, clear_synapse_cache
 from schematic.schemas.explorer import SchemaExplorer
 from schematic.schemas.generator import SchemaGenerator
 from schematic.store.base import BaseStorage
 from schematic.exceptions import MissingConfigValueError, AccessCredentialsError
 
 from schematic.configuration.configuration import CONFIG
 
-from schematic.utils.general import profile
+from schematic.utils.general import profile, calculate_datetime
 
 logger = logging.getLogger("Synapse storage")
 
 @dataclass
 class ManifestDownload(object):
     """
     syn: an object of type synapseclient.
@@ -71,20 +71,24 @@
         try downloading a manifest to local cache or a given folder
         manifest
         Return:
             manifest_data: A Synapse file entity of the downloaded manifest
         """
         if "SECRETS_MANAGER_SECRETS" in os.environ:
             temporary_manifest_storage = "/var/tmp/temp_manifest_download"
+            # clear out all the existing manifests
+            if os.path.exists(temporary_manifest_storage):
+                shutil.rmtree(temporary_manifest_storage)
+            # create a new directory to store manifest
             if not os.path.exists(temporary_manifest_storage):
-                os.mkdir("/var/tmp/temp_manifest_download")
+                os.mkdir(temporary_manifest_storage)
+            # create temporary folders for storing manifests
             download_location = create_temp_folder(temporary_manifest_storage)
         else:
             download_location=CONFIG.manifest_folder
-
         manifest_data = self.syn.get(
                 self.manifest_id,
                 downloadLocation=download_location,
                 ifcollision="overwrite.local",
             )
         return manifest_data
 
@@ -173,49 +177,42 @@
             KeyError: when the 'storage' config object is missing values for essential keys.
             AttributeError: when the 'storageFileview' attribute (of class SynapseStorage) does not have a value associated with it.
             synapseclient.core.exceptions.SynapseHTTPError: check if the current user has permission to access the Synapse entity.
             ValueError: when Admin fileview cannot be found (describe further).
         Typical usage example:
             syn_store = SynapseStorage()
         """
-
+        # TODO: turn root_synapse_cache to a parameter in init
         self.syn = self.login(token, access_token)
         self.project_scope = project_scope
         self.storageFileview = CONFIG.synapse_master_fileview_id
         self.manifest = CONFIG.synapse_manifest_basename
+        self.root_synapse_cache = "/root/.synapseCache"
         self._query_fileview()
 
-    def _purge_synapse_cache(self, root_dir: str = "/var/www/.synapseCache/", maximum_storage_allowed_cache_gb=7):
+    def _purge_synapse_cache(self, maximum_storage_allowed_cache_gb=1):
         """
-        Purge synapse cache if it exceeds 7GB
+        Purge synapse cache if it exceeds a certain size. Default to 1GB. 
         Args:
-            root_dir: directory of the .synapseCache function
-            maximum_storage_allowed_cache_gb: the maximum storage allowed before purging cache. Default is 7 GB. 
-
-        Returns: 
-            if size of cache reaches a certain threshold (default is 7GB), return the number of files that get deleted
-            otherwise, return the total remaining space (assuming total ephemeral storage is 20GB on AWS )
+            maximum_storage_allowed_cache_gb: the maximum storage allowed before purging cache. Default is 1 GB. 
         """
         # try clearing the cache
         # scan a directory and check size of files
-        cache = self.syn.cache
-        if os.path.exists(root_dir):
+        if os.path.exists(self.root_synapse_cache):
             maximum_storage_allowed_cache_bytes = convert_gb_to_bytes(maximum_storage_allowed_cache_gb)
-            total_ephemeral_storag_gb = 20
-            total_ephemeral_storage_bytes = convert_gb_to_bytes(total_ephemeral_storag_gb)
-            nbytes = get_dir_size(root_dir)
-            # if 7 GB has already been taken, purge cache before 15 min
-            if nbytes >= maximum_storage_allowed_cache_bytes:
-                minutes_earlier = datetime.strftime(datetime.utcnow()- timedelta(minutes = 15), '%s')
-                num_of_deleted_files = cache.purge(before_date = int(minutes_earlier))
-                logger.info(f'{num_of_deleted_files} number of files have been deleted from {root_dir}')
+            nbytes = get_dir_size(self.root_synapse_cache)
+            dir_size_bytes = check_synapse_cache_size(directory=self.root_synapse_cache)
+            # if 1 GB has already been taken, purge cache before 15 min
+            if dir_size_bytes >= maximum_storage_allowed_cache_bytes:
+                num_of_deleted_files = clear_synapse_cache(self.syn.cache, minutes=15)
+                logger.info(f'{num_of_deleted_files}  files have been deleted from {self.root_synapse_cache}')
             else:
-                remaining_space = total_ephemeral_storage_bytes - nbytes
-                converted_space = convert_size(remaining_space)
-                logger.info(f'Estimated {remaining_space} bytes (which is approximately {converted_space}) remained in ephemeral storage after calculating size of .synapseCache excluding OS')
+                # on AWS, OS takes around 14-17% of our ephemeral storage (20GiB)
+                # instead of guessing how much space that we left, print out .synapseCache here
+                logger.info(f'the total size of .synapseCache is: {nbytes} bytes')
 
     def _query_fileview(self):
         self._purge_synapse_cache()
         try:
             self.storageFileview = CONFIG.synapse_master_fileview_id
             self.manifest = CONFIG.synapse_manifest_basename
             if self.project_scope:
```

### Comparing `schematicpy-23.7.1/schematic/utils/cli_utils.py` & `schematicpy-23.8.1/schematic/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/curie_utils.py` & `schematicpy-23.8.1/schematic/utils/curie_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/df_utils.py` & `schematicpy-23.8.1/schematic/utils/df_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/google_api_utils.py` & `schematicpy-23.8.1/schematic/utils/google_api_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/io_utils.py` & `schematicpy-23.8.1/schematic/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/schema_utils.py` & `schematicpy-23.8.1/schematic/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/validate_rules_utils.py` & `schematicpy-23.8.1/schematic/utils/validate_rules_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/utils/validate_utils.py` & `schematicpy-23.8.1/schematic/utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/visualization/attributes_explorer.py` & `schematicpy-23.8.1/schematic/visualization/attributes_explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/visualization/commands.py` & `schematicpy-23.8.1/schematic/visualization/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/schematic/visualization/tangled_tree.py` & `schematicpy-23.8.1/schematic/visualization/tangled_tree.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.7.1/PKG-INFO` & `schematicpy-23.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schematicpy
-Version: 23.7.1
+Version: 23.8.1
 Summary: Package for biomedical data model and metadata ingress management
 Home-page: https://github.com/Sage-Bionetworks/schematic
 Keywords: schema,metadata,validation,data model,linked data
 Author: Milen Nikolov
 Author-email: milen.nikolov@sagebase.org
 Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -126,15 +126,15 @@
 ```
 This command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)
 
 5. Fill in credential files: 
 *Note*: If you won't interact with Synapse, please ignore this section.
 
 There are two main configuration files that need to be edited:
-[config.yml](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml)
+config.yml
 and [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)
 
 <strong>Configure .synapseConfig File</strong>
 
 Download a copy of the ``.synapseConfig`` file, open the file in the
 editor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section
```

