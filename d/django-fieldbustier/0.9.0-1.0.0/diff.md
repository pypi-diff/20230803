# Comparing `tmp/django-fieldbustier-0.9.0.tar.gz` & `tmp/django-fieldbustier-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-fieldbustier-0.9.0.tar", last modified: Mon Aug 15 14:39:01 2022, max compression
+gzip compressed data, was "dist/django-fieldbustier-1.0.0.tar", last modified: Thu Aug  3 14:57:53 2023, max compression
```

## Comparing `django-fieldbustier-0.9.0.tar` & `django-fieldbustier-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jmad      (1000) jmad      (1000)        0 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     1063 2019-01-28 00:12:14.000000 django-fieldbustier-0.9.0/LICENSE
--rw-r--r--   0 jmad      (1000) jmad      (1000)       70 2019-02-08 21:54:18.000000 django-fieldbustier-0.9.0/MANIFEST.in
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     5807 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/PKG-INFO
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     4112 2022-08-15 14:24:09.000000 django-fieldbustier-0.9.0/README.md
-drwxrwxr-x   0 jmad      (1000) jmad      (1000)        0 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/django_fieldbustier/
--rw-rw-r--   0 jmad      (1000) jmad      (1000)       67 2019-02-17 22:29:08.000000 django-fieldbustier-0.9.0/django_fieldbustier/__init__.py
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     3711 2022-08-15 14:23:59.000000 django-fieldbustier-0.9.0/django_fieldbustier/apps.py
--rw-rw-r--   0 jmad      (1000) jmad      (1000)      630 2022-08-15 14:05:30.000000 django-fieldbustier-0.9.0/django_fieldbustier/fieldbustier_config.py
--rw-rw-r--   0 jmad      (1000) jmad      (1000)       17 2019-02-17 22:29:08.000000 django-fieldbustier-0.9.0/django_fieldbustier/urls.py
--rw-rw-r--   0 jmad      (1000) jmad      (1000)       22 2022-08-15 14:23:59.000000 django-fieldbustier-0.9.0/django_fieldbustier/version.py
-drwxrwxr-x   0 jmad      (1000) jmad      (1000)        0 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/django_fieldbustier.egg-info/
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     5807 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/django_fieldbustier.egg-info/PKG-INFO
--rw-rw-r--   0 jmad      (1000) jmad      (1000)      455 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/django_fieldbustier.egg-info/SOURCES.txt
--rw-rw-r--   0 jmad      (1000) jmad      (1000)        1 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/django_fieldbustier.egg-info/dependency_links.txt
--rw-rw-r--   0 jmad      (1000) jmad      (1000)        1 2019-02-08 21:49:25.000000 django-fieldbustier-0.9.0/django_fieldbustier.egg-info/not-zip-safe
--rw-rw-r--   0 jmad      (1000) jmad      (1000)       20 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/django_fieldbustier.egg-info/top_level.txt
--rw-rw-r--   0 jmad      (1000) jmad      (1000)       28 2022-08-15 14:23:59.000000 django-fieldbustier-0.9.0/requirements_lints.txt
--rw-r--r--   0 jmad      (1000) jmad      (1000)      406 2022-08-15 14:39:01.000000 django-fieldbustier-0.9.0/setup.cfg
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     1237 2020-02-10 16:46:24.000000 django-fieldbustier-0.9.0/setup.py
--rw-rw-r--   0 jmad      (1000) jmad      (1000)     1748 2022-08-15 14:23:59.000000 django-fieldbustier-0.9.0/tox.ini
+drwxrwxr-x   0 jmad      (1000) jmad      (1000)        0 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/
+drwxrwxr-x   0 jmad      (1000) jmad      (1000)        0 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/django_fieldbustier/
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)       67 2019-02-17 22:29:08.000000 django-fieldbustier-1.0.0/django_fieldbustier/__init__.py
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)      630 2022-08-15 14:05:30.000000 django-fieldbustier-1.0.0/django_fieldbustier/fieldbustier_config.py
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)       22 2023-08-03 14:57:09.000000 django-fieldbustier-1.0.0/django_fieldbustier/version.py
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     3801 2023-06-06 22:16:31.000000 django-fieldbustier-1.0.0/django_fieldbustier/apps.py
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)       17 2019-02-17 22:29:08.000000 django-fieldbustier-1.0.0/django_fieldbustier/urls.py
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)       28 2022-08-15 14:23:59.000000 django-fieldbustier-1.0.0/requirements_lints.txt
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     1523 2023-06-06 22:16:31.000000 django-fieldbustier-1.0.0/tox.ini
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     1063 2019-01-28 00:12:14.000000 django-fieldbustier-1.0.0/LICENSE
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     5807 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/PKG-INFO
+-rw-r--r--   0 jmad      (1000) jmad      (1000)      406 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/setup.cfg
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     4112 2022-08-15 14:24:09.000000 django-fieldbustier-1.0.0/README.md
+drwxrwxr-x   0 jmad      (1000) jmad      (1000)        0 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/django_fieldbustier.egg-info/
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)        1 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/django_fieldbustier.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)      455 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/django_fieldbustier.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     5807 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/django_fieldbustier.egg-info/PKG-INFO
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)        1 2019-02-08 21:49:25.000000 django-fieldbustier-1.0.0/django_fieldbustier.egg-info/not-zip-safe
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)       20 2023-08-03 14:57:53.000000 django-fieldbustier-1.0.0/django_fieldbustier.egg-info/top_level.txt
+-rw-rw-r--   0 jmad      (1000) jmad      (1000)     1237 2020-02-10 16:46:24.000000 django-fieldbustier-1.0.0/setup.py
+-rw-r--r--   0 jmad      (1000) jmad      (1000)       70 2019-02-08 21:54:18.000000 django-fieldbustier-1.0.0/MANIFEST.in
```

### Comparing `django-fieldbustier-0.9.0/LICENSE` & `django-fieldbustier-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fieldbustier-0.9.0/PKG-INFO` & `django-fieldbustier-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fieldbustier
-Version: 0.9.0
+Version: 1.0.0
 Summary: A package that allows modifying a model of any django app from the outside, without modifying the code of the app itself.
 Home-page: https://github.com/mrjmad/django-fieldbustier
 Author: MrJmad
 Author-email: j-mad@j-mad.com
 License: MIT License
 Description: ![gitHub Actions Status](https://github.com/mrjmad/django-fieldbustier/actions/workflows/actions.yml/badge.svg)
         # django-fieldbustier
```

### Comparing `django-fieldbustier-0.9.0/README.md` & `django-fieldbustier-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-fieldbustier-0.9.0/django_fieldbustier/apps.py` & `django-fieldbustier-1.0.0/django_fieldbustier/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from collections import defaultdict
 from importlib import import_module
 from sys import argv
 
 from django.apps import AppConfig
 from django.apps import apps
 from django.conf import settings
-from django.utils.translation import ugettext_lazy as _
+
+
+try:
+    from django.utils.translation import ugettext_lazy as _
+except ImportError:
+    from django.utils.translation import gettext_lazy as _
 
 
 def import_object(path_to_object):
     path_module, object_name = path_to_object.rsplit(".", 1)
 
     imported_module = import_module(path_module)
     return getattr(imported_module, object_name)
```

### Comparing `django-fieldbustier-0.9.0/django_fieldbustier/fieldbustier_config.py` & `django-fieldbustier-1.0.0/django_fieldbustier/fieldbustier_config.py`

 * *Files identical despite different names*

### Comparing `django-fieldbustier-0.9.0/django_fieldbustier.egg-info/PKG-INFO` & `django-fieldbustier-1.0.0/django_fieldbustier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fieldbustier
-Version: 0.9.0
+Version: 1.0.0
 Summary: A package that allows modifying a model of any django app from the outside, without modifying the code of the app itself.
 Home-page: https://github.com/mrjmad/django-fieldbustier
 Author: MrJmad
 Author-email: j-mad@j-mad.com
 License: MIT License
 Description: ![gitHub Actions Status](https://github.com/mrjmad/django-fieldbustier/actions/workflows/actions.yml/badge.svg)
         # django-fieldbustier
```

### Comparing `django-fieldbustier-0.9.0/setup.py` & `django-fieldbustier-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-fieldbustier-0.9.0/tox.ini` & `django-fieldbustier-1.0.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = django111,lints
+envlist = django111,lints,django22,django32,django42
 
 [testenv]
 usedevelop = True
 setenv =
     PYTHONPATH = {toxinidir}
 deps =
     flake8
@@ -16,45 +16,38 @@
 deps =
     django>=1.11,<1.11.99
     {[testenv]deps}
 commands = 
     python demo_tests/manage.py test demo_app --noinput
     python demo_tests/manage.py test fieldbustier_tests --settings=demo_tests.settings_with_fieldbustier --noinput
 
-[testenv:django20]
+[testenv:django22]
 deps =
-    django>=2.0,<2.0.99
+    django>=2.2,<2.2.99
     {[testenv]deps}
 commands =
     python demo_tests/manage.py test demo_app --noinput
     python demo_tests/manage.py test fieldbustier_tests --settings=demo_tests.settings_with_fieldbustier --noinput
 
-[testenv:django21]
+[testenv:django32]
 deps =
-    django>=2.1,<2.1.99
+    django>=3.2,<3.2.99
     {[testenv]deps}
 commands =
     python demo_tests/manage.py test demo_app --noinput
     python demo_tests/manage.py test fieldbustier_tests --settings=demo_tests.settings_with_fieldbustier --noinput
 
-[testenv:django22]
+[testenv:django42]
 deps =
-    django>=2.2,<2.2.99
+    django>=4.2,<4.2.99
     {[testenv]deps}
 commands =
     python demo_tests/manage.py test demo_app --noinput
     python demo_tests/manage.py test fieldbustier_tests --settings=demo_tests.settings_with_fieldbustier --noinput
 
-[testenv:django32]
-deps =
-    django>=3.2,<3.2.99
-    {[testenv]deps}
-commands =
-    python demo_tests/manage.py test demo_app --noinput
-    python demo_tests/manage.py test fieldbustier_tests --settings=demo_tests.settings_with_fieldbustier --noinput
 
 [testenv:lints]
 deps =
     {[testenv]deps}
 commands =
     black --check -l120 django_fieldbustier
     black --check -l120 demo_tests
```

