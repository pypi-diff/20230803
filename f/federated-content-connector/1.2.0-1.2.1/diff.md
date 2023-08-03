# Comparing `tmp/federated-content-connector-1.2.0.tar.gz` & `tmp/federated-content-connector-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-1.2.0.tar", last modified: Tue Jul 18 13:07:34 2023, max compression
+gzip compressed data, was "federated-content-connector-1.2.1.tar", last modified: Thu Aug  3 06:54:55 2023, max compression
```

## Comparing `federated-content-connector-1.2.0.tar` & `federated-content-connector-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10362 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/course_metadata_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/commands/import_course_runs_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.173981 federated-content-connector-1.2.0/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.456503 federated-content-connector-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-08-03 06:54:55.456503 federated-content-connector-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10362 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/management/commands/import_course_runs_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/management/commands/refresh_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/migrations/0002_coursedetailsimportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.448503 federated-content-connector-1.2.1/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-03 06:54:55.000000 federated-content-connector-1.2.1/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.452503 federated-content-connector-1.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-08-03 06:54:55.456503 federated-content-connector-1.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:54:55.456503 federated-content-connector-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-08-03 06:54:48.000000 federated-content-connector-1.2.1/tests/test_signals.py
```

### Comparing `federated-content-connector-1.2.0/CHANGELOG.rst` & `federated-content-connector-1.2.1/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.2.1 – 2023-08-03
+------------------
+* feat: hook for modify course enrollment data
+
 1.2.0 – 2023-07-18
 ------------------
 * Refactor `import_course_runs_metadata` command to import all courseruns
 
 1.1.0 – 2023-06-21
 ------------------
 * Management command to refresh CourseDetails data
```

### Comparing `federated-content-connector-1.2.0/LICENSE.txt` & `federated-content-connector-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/PKG-INFO` & `federated-content-connector-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.2.0
+Version: 1.2.1
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.2.1 – 2023-08-03
+------------------
+* feat: hook for modify course enrollment data
+
 1.2.0 – 2023-07-18
 ------------------
 * Refactor `import_course_runs_metadata` command to import all courseruns
 
 1.1.0 – 2023-06-21
 ------------------
 * Management command to refresh CourseDetails data
```

### Comparing `federated-content-connector-1.2.0/README.rst` & `federated-content-connector-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/apps.py` & `federated-content-connector-1.2.1/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/course_metadata_importer.py` & `federated-content-connector-1.2.1/federated_content_connector/course_metadata_importer.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.2.1/federated_content_connector/filters/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Open edx Filters Pipeline for the federated content connector."""
 from django.conf import settings
+from django.utils import timezone
 from openedx.core.djangoapps.catalog.utils import get_course_data
 from openedx_filters import PipelineStep
 
 from federated_content_connector.constants import EXEC_ED_COURSE_TYPE, EXEC_ED_LANDING_PAGE, PRODUCT_SOURCE_2U
+from federated_content_connector.models import CourseDetails
 
 
 class CreateCustomUrlForCourseStep(PipelineStep):
     """
     Step that modifies the url for the course home page.
 
     Example usage:
@@ -34,7 +36,43 @@
             course_type = course_data.get('course_type')
             product_source = course_data.get('product_source')
             product_source_slug = product_source['slug'] if isinstance(product_source, dict) else product_source
             if course_type == EXEC_ED_COURSE_TYPE and product_source_slug == PRODUCT_SOURCE_2U:
                 course_home_url = getattr(settings, 'EXEC_ED_LANDING_PAGE', EXEC_ED_LANDING_PAGE)
 
         return {'course_key': course_key, 'course_home_url': course_home_url}
+
+
+class CreateApiRenderEnrollmentStep(PipelineStep):
+    """
+    Step that modifies the enrollment data for the course.
+
+    Example usage:
+
+    Add the following configurations to your configuration file:
+
+        "OPEN_EDX_FILTERS_CONFIG": {
+            "org.openedx.learning.home.enrollment.api.rendered.v1": {
+                "fail_silently": False,
+                "pipeline": [
+                    "federated_content_connector.filters.pipeline.CreateApiRenderEnrollmentStep"
+                ]
+            }
+        }
+    """
+
+    def run_filter(self, course_key, serialized_enrollment):  # pylint: disable=arguments-differ
+        """
+        Pipeline step that modifies the enrollment data for the course.
+        """
+        try:
+            course_details = CourseDetails.objects.get(id=course_key)
+            course_type = course_details.course_type
+            product_source = course_details.product_source
+            start_date = course_details.start_date
+            if product_source == PRODUCT_SOURCE_2U and course_type == EXEC_ED_COURSE_TYPE:
+                if start_date and start_date <= timezone.now():
+                    serialized_enrollment['hasStarted'] = True
+        except CourseDetails.DoesNotExist:
+            pass
+
+        return {'course_key': course_key, 'serialized_enrollment': serialized_enrollment}
```

### Comparing `federated-content-connector-1.2.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py` & `federated-content-connector-1.2.1/federated_content_connector/management/commands/refresh_course_runs_metadata.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/migrations/0001_initial.py` & `federated-content-connector-1.2.1/federated_content_connector/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py` & `federated-content-connector-1.2.1/federated_content_connector/migrations/0002_coursedetailsimportstatus.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/models.py` & `federated-content-connector-1.2.1/federated_content_connector/models.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/signals.py` & `federated-content-connector-1.2.1/federated_content_connector/signals.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/tasks.py` & `federated-content-connector-1.2.1/federated_content_connector/tasks.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.2.1/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.2.1/federated_content_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.2.0
+Version: 1.2.1
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.2.1 – 2023-08-03
+------------------
+* feat: hook for modify course enrollment data
+
 1.2.0 – 2023-07-18
 ------------------
 * Refactor `import_course_runs_metadata` command to import all courseruns
 
 1.1.0 – 2023-06-21
 ------------------
 * Management command to refresh CourseDetails data
```

### Comparing `federated-content-connector-1.2.0/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.2.1/federated_content_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/requirements/constraints.txt` & `federated-content-connector-1.2.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/setup.py` & `federated-content-connector-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.2.0/tests/test_signals.py` & `federated-content-connector-1.2.1/tests/test_signals.py`

 * *Files identical despite different names*

