# Comparing `tmp/dbt_metricflow-0.0.5.tar.gz` & `tmp/dbt_metricflow-0.1.0rc1.tar.gz`

## Comparing `dbt_metricflow-0.0.5.tar` & `dbt_metricflow-0.1.0rc1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.5/.gitignore
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.5/LICENSE
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.5/README.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 dbt_metricflow-0.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 dbt_metricflow-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 dbt_metricflow-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 dbt_metricflow-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 dbt_metricflow-0.1.0rc1/PKG-INFO
```

### Comparing `dbt_metricflow-0.0.5/.gitignore` & `dbt_metricflow-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.5/LICENSE` & `dbt_metricflow-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.5/README.md` & `dbt_metricflow-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.5/pyproject.toml` & `dbt_metricflow-0.1.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling~=1.14.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbt-metricflow"
-version = "0.0.5"
+version = "0.1.0.rc1"
 description = "Execute commands against the MetricFlow semantic layer with dbt."
 readme = "README.md"
 requires-python = ">=3.8,<3.12"
 license = "BUSL-1.1"
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
 ]
@@ -21,26 +21,35 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "dbt-core~=1.6.0rc2",
-  "metricflow==0.200.0.dev15"
+  "metricflow==0.200.0.rc1"
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/dbt-labs/metricflow/tree/main/dbt-metricflow"
 
 [project.optional-dependencies]
+bigquery = [
+  "dbt-bigquery~=1.6.0"
+]
+databricks = [
+  "dbt-databricks~=1.6.0"
+]
 postgres = [
-  "dbt-postgres>=1.6.0b6"
+  "dbt-postgres~=1.6.0"
+]
+redshift = [
+  "dbt-redshift~=1.6.0"
 ]
 snowflake = [
-  "dbt-snowflake>=1.6.0b3"
+  "dbt-snowflake~=1.6.0"
 ]
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
   "/.changes",
   ".changie.yaml",
```

### Comparing `dbt_metricflow-0.0.5/PKG-INFO` & `dbt_metricflow-0.1.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-metricflow
-Version: 0.0.5
+Version: 0.1.0rc1
 Summary: Execute commands against the MetricFlow semantic layer with dbt.
 Project-URL: Source Code, https://github.com/dbt-labs/metricflow/tree/main/dbt-metricflow
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: BUSL-1.1
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -12,19 +12,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.12,>=3.8
 Requires-Dist: dbt-core~=1.6.0rc2
-Requires-Dist: metricflow==0.200.0.dev15
+Requires-Dist: metricflow==0.200.0.rc1
+Provides-Extra: bigquery
+Requires-Dist: dbt-bigquery~=1.6.0; extra == 'bigquery'
+Provides-Extra: databricks
+Requires-Dist: dbt-databricks~=1.6.0; extra == 'databricks'
 Provides-Extra: postgres
-Requires-Dist: dbt-postgres>=1.6.0b6; extra == 'postgres'
+Requires-Dist: dbt-postgres~=1.6.0; extra == 'postgres'
+Provides-Extra: redshift
+Requires-Dist: dbt-redshift~=1.6.0; extra == 'redshift'
 Provides-Extra: snowflake
-Requires-Dist: dbt-snowflake>=1.6.0b3; extra == 'snowflake'
+Requires-Dist: dbt-snowflake~=1.6.0; extra == 'snowflake'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a target="_blank" href="https://twitter.com/dbt_labs">
     <img src="https://img.shields.io/twitter/follow/dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat">
   </a>
     <a target="_blank" href="https://www.getdbt.com/community/">
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-Metadata-Version: 2.1 Name: dbt-metricflow Version: 0.0.5 Summary: Execute
+Metadata-Version: 2.1 Name: dbt-metricflow Version: 0.1.0rc1 Summary: Execute
 commands against the MetricFlow semantic layer with dbt. Project-URL: Source
 Code, https://github.com/dbt-labs/metricflow/tree/main/dbt-metricflow Author-
 email: dbt Labs
 dbtlabs.com> License-Expression: BUSL-1.1 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: <3.12,>=3.8
-Requires-Dist: dbt-core~=1.6.0rc2 Requires-Dist: metricflow==0.200.0.dev15
-Provides-Extra: postgres Requires-Dist: dbt-postgres>=1.6.0b6; extra ==
-'postgres' Provides-Extra: snowflake Requires-Dist: dbt-snowflake>=1.6.0b3;
-extra == 'snowflake' Description-Content-Type: text/markdown
+Requires-Dist: dbt-core~=1.6.0rc2 Requires-Dist: metricflow==0.200.0.rc1
+Provides-Extra: bigquery Requires-Dist: dbt-bigquery~=1.6.0; extra ==
+'bigquery' Provides-Extra: databricks Requires-Dist: dbt-databricks~=1.6.0;
+extra == 'databricks' Provides-Extra: postgres Requires-Dist: dbt-
+postgres~=1.6.0; extra == 'postgres' Provides-Extra: redshift Requires-Dist:
+dbt-redshift~=1.6.0; extra == 'redshift' Provides-Extra: snowflake Requires-
+Dist: dbt-snowflake~=1.6.0; extra == 'snowflake' Description-Content-Type:
+text/markdown
                     [https://img.shields.io/twitter/follow/
  dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat] [https://
     img.shields.io/badge/Slack-join-163B36] [https://img.shields.io/badge/
                         code%20style-black-000000.svg]
 # Welcome to dbt-metricflow This repo encapsulates the dbt-core, MetricFlow,
 and supported dbt-adapters packages. This package will manage the versioning
 between these packages such that they are compatible with each other. ## Repo
```

