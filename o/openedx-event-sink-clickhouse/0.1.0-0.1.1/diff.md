# Comparing `tmp/openedx_event_sink_clickhouse-0.1.0.tar.gz` & `tmp/openedx_event_sink_clickhouse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx_event_sink_clickhouse-0.1.0.tar", last modified: Thu May 11 20:34:07 2023, max compression
+gzip compressed data, was "openedx_event_sink_clickhouse-0.1.1.tar", last modified: Thu Aug  3 16:08:05 2023, max compression
```

## Comparing `openedx_event_sink_clickhouse-0.1.0.tar` & `openedx_event_sink_clickhouse-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9638 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.852161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.852161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6928 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/management/commands/dump_courses_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/sinks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (122)    18100 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/sinks/course_published.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.852161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/templates/event_sink_clickhouse/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/templates/event_sink_clickhouse/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9638 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-11 20:34:07.000000 openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 20:34:07.856161 openedx_event_sink_clickhouse-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     7920 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/tests/test_course_published.py
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/tests/test_django_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-11 20:34:03.000000 openedx_event_sink_clickhouse-0.1.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.386287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.386287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.386287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/management/commands/dump_courses_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/sinks/course_published.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.386287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/templates/event_sink_clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/templates/event_sink_clickhouse/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 16:08:05.000000 openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5383 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:08:05.390287 openedx_event_sink_clickhouse-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/tests/test_course_published.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/tests/test_django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 16:07:59.000000 openedx_event_sink_clickhouse-0.1.1/tests/test_models.py
```

### Comparing `openedx_event_sink_clickhouse-0.1.0/CHANGELOG.rst` & `openedx_event_sink_clickhouse-0.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/LICENSE.txt` & `openedx_event_sink_clickhouse-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/PKG-INFO` & `openedx_event_sink_clickhouse-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx_event_sink_clickhouse
-Version: 0.1.0
+Version: 0.1.1
 Summary: A sink for Open edX events to send them to ClickHouse
 Home-page: https://github.com/openedx/openedx_event_sink_clickhouse
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -228,15 +228,15 @@
 file in this repo.
 
 .. _Backstage: https://open-edx-backstage.herokuapp.com/catalog/default/component/openedx-event-sink-clickhouse
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-event-sink-clickhouse.svg
     :target: https://pypi.python.org/pypi/openedx-event-sink-clickhouse/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-event-sink-clickhouse/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-event-sink-clickhouse/actions
```

### Comparing `openedx_event_sink_clickhouse-0.1.0/README.rst` & `openedx_event_sink_clickhouse-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 file in this repo.
 
 .. _Backstage: https://open-edx-backstage.herokuapp.com/catalog/default/component/openedx-event-sink-clickhouse
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-event-sink-clickhouse.svg
     :target: https://pypi.python.org/pypi/openedx-event-sink-clickhouse/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-event-sink-clickhouse/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-event-sink-clickhouse/actions
```

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/apps.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/apps.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/management/commands/dump_courses_to_clickhouse.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/management/commands/dump_courses_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/settings/common.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/settings/common.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/signals.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/signals.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/sinks/base_sink.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/sinks/course_published.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/sinks/course_published.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         output = io.StringIO()
         writer = csv.writer(output, quoting=csv.QUOTE_NONNUMERIC)
         writer.writerow(serialized_overview.values())
 
         request = requests.Request(
             'POST',
             self.ch_url,
-            data=output.getvalue(),
+            data=output.getvalue().encode("utf-8"),
             params=params,
             auth=self.ch_auth
         )
 
         self._send_clickhouse_request(request, expected_insert_rows=1)
 
     def _send_xblocks(self, serialized_xblocks):
@@ -266,15 +266,15 @@
 
         for node in serialized_xblocks:
             writer.writerow(node.values())
 
         request = requests.Request(
             'POST',
             self.ch_url,
-            data=output.getvalue(),
+            data=output.getvalue().encode("utf-8"),
             params=params,
             auth=self.ch_auth
         )
 
         self._send_clickhouse_request(request, expected_insert_rows=len(serialized_xblocks))
 
     def _send_relationships(self, relationships):
```

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/tasks.py` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/tasks.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/event_sink_clickhouse/templates/event_sink_clickhouse/base.html` & `openedx_event_sink_clickhouse-0.1.1/event_sink_clickhouse/templates/event_sink_clickhouse/base.html`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/PKG-INFO` & `openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-event-sink-clickhouse
-Version: 0.1.0
+Version: 0.1.1
 Summary: A sink for Open edX events to send them to ClickHouse
 Home-page: https://github.com/openedx/openedx_event_sink_clickhouse
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -228,15 +228,15 @@
 file in this repo.
 
 .. _Backstage: https://open-edx-backstage.herokuapp.com/catalog/default/component/openedx-event-sink-clickhouse
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-event-sink-clickhouse.svg
     :target: https://pypi.python.org/pypi/openedx-event-sink-clickhouse/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-event-sink-clickhouse/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-event-sink-clickhouse/actions
```

### Comparing `openedx_event_sink_clickhouse-0.1.0/openedx_event_sink_clickhouse.egg-info/SOURCES.txt` & `openedx_event_sink_clickhouse-0.1.1/openedx_event_sink_clickhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/requirements/constraints.txt` & `openedx_event_sink_clickhouse-0.1.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/setup.py` & `openedx_event_sink_clickhouse-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/tests/test_course_published.py` & `openedx_event_sink_clickhouse-0.1.1/tests/test_course_published.py`

 * *Files identical despite different names*

### Comparing `openedx_event_sink_clickhouse-0.1.0/tests/test_django_settings.py` & `openedx_event_sink_clickhouse-0.1.1/tests/test_django_settings.py`

 * *Files identical despite different names*

