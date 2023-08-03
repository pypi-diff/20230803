# Comparing `tmp/django-glue-0.4.2.tar.gz` & `tmp/django-glue-0.4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.4.2.tar", last modified: Wed Aug  2 16:09:27 2023, max compression
+gzip compressed data, was "django-glue-0.4.2.1.tar", last modified: Thu Aug  3 16:58:27 2023, max compression
```

## Comparing `django-glue-0.4.2.tar` & `django-glue-0.4.2.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-02 16:09:15.000000 django-glue-0.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-02 16:09:15.000000 django-glue-0.4.2/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 16:09:15.000000 django-glue-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 16:09:15.000000 django-glue-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 16:09:27.310497 django-glue-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-02 16:09:15.000000 django-glue-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.302497 django-glue-0.4.2/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.302497 django-glue-0.4.2/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.302497 django-glue-0.4.2/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 16:09:15.000000 django-glue-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 16:09:27.314497 django-glue-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 16:09:15.000000 django-glue-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.952915 django-glue-0.4.2.1/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.948915 django-glue-0.4.2.1/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.948915 django-glue-0.4.2.1/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.948915 django-glue-0.4.2.1/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.952915 django-glue-0.4.2.1/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/wsgi.py
```

### Comparing `django-glue-0.4.2/CHANGELOG.md` & `django-glue-0.4.2.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog for Django Glue
 
+## 0.4.2.1
+
+### Changes
+- Model default values now work with glue.
+
 ## 0.4.2
 
 ### Changes
 - Context data to construct model object fields in js
 - Session data updated inside of keep live ajax
 - Cleaning js functions (more needed)
```

### Comparing `django-glue-0.4.2/LICENSE.md` & `django-glue-0.4.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/PKG-INFO` & `django-glue-0.4.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.2
+Version: 0.4.2.1
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.2/README.md` & `django-glue-0.4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/context_processors.py` & `django-glue-0.4.2.1/django_glue/context_processors.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django_glue.conf import settings
 from django_glue import __version__
 from django_glue.sessions import GlueSession
 
 
 def glue(request):
-    print(json.dumps(GlueSession(request).session))
     return {
         'DJANGO_GLUE_VERSION': __version__,
         settings.DJANGO_GLUE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_SESSION_NAME, {}).get('context'),
         settings.DJANGO_GLUE_KEEP_LIVE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_KEEP_LIVE_SESSION_NAME, {}),
         'DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS': settings.DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_SECONDS * 1000,
         'GLUE_SESSION_DATA': json.dumps(GlueSession(request).session),
     }
```

### Comparing `django-glue-0.4.2/django_glue/data_classes.py` & `django-glue-0.4.2.1/django_glue/data_classes.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/enums.py` & `django-glue-0.4.2.1/django_glue/enums.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/glue.py` & `django-glue-0.4.2.1/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/handlers.py` & `django-glue-0.4.2.1/django_glue/handlers.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/middleware.py` & `django-glue-0.4.2.1/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/responses.py` & `django-glue-0.4.2.1/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/services/model_objects.py` & `django-glue-0.4.2.1/django_glue/services/model_objects.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/services/query_sets.py` & `django-glue-0.4.2.1/django_glue/services/query_sets.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/services/services.py` & `django-glue-0.4.2.1/django_glue/services/services.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/services/templates.py` & `django-glue-0.4.2.1/django_glue/services/templates.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/sessions.py` & `django-glue-0.4.2.1/django_glue/sessions.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_ajax.js` & `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_model_object.js` & `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,14 @@
 class GlueModelObject {
     constructor(unique_name) {
         this.glue_unique_name = unique_name
 
         for (let key in window.glue_session_data['context'][unique_name].fields) {
-            this[key] = null
+            this[key] = window.glue_session_data['context'][unique_name].fields[key].value
+            console.log(key, this[key])
         }
 
         window.glue_keep_live.add_unique_name(unique_name)
     }
 
     async create() {
         return await glue_ajax_request(
```

### Comparing `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_query_set.js` & `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 class GlueQuerySet {
     constructor(unique_name) {
         this.glue_unique_name = unique_name
 
         for (let key in window.glue_session_data['context'][unique_name].fields) {
-            this[key] = null
+            this[key] = window.glue_session_data['context'][unique_name].fields[key].value
         }
 
         window.glue_keep_live.add_unique_name(unique_name)
     }
 
     async all() {
         let model_object_list = []
```

### Comparing `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_template.js` & `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_view.js` & `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/templates/django_glue/django_glue.html` & `django-glue-0.4.2.1/django_glue/templates/django_glue/django_glue.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 {% load static %}
 
 {% load django_glue %}
 
 {% csrf_token %}
 
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_keep_live.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
+
 <script type="application/javascript">
     const DJANGO_DEBUG = {% if debug %}true{% else %}false{% endif %}
     const DJANGO_GLUE_AJAX_URL = '{% url 'django_glue:django_glue_data_handler' %}'
     const DJANGO_GLUE_KEEP_LIVE_URL = '{% url 'django_glue:django_glue_keep_live_handler' %}'
 
     window.glue_keep_live = new GlueKeepLive()
     window.glue_session_data = {{ GLUE_SESSION_DATA|safe }}
 
-
+    setInterval(() => {
+        window.glue_keep_live.update(DJANGO_GLUE_KEEP_LIVE_URL)
+    }, 2000)
 
 </script>
 
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_csrf.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_ajax.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_event.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_response.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
```

### Comparing `django-glue-0.4.2/django_glue/templatetags/django_glue.py` & `django-glue-0.4.2.1/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/utils.py` & `django-glue-0.4.2.1/django_glue/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue/views.py` & `django-glue-0.4.2.1/django_glue/views.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/django_glue.egg-info/PKG-INFO` & `django-glue-0.4.2.1/django_glue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.2
+Version: 0.4.2.1
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.2/django_glue.egg-info/SOURCES.txt` & `django-glue-0.4.2.1/django_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/setup.py` & `django-glue-0.4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/tests/manage.py` & `django-glue-0.4.2.1/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/tests/migrations/0001_initial.py` & `django-glue-0.4.2.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/tests/models.py` & `django-glue-0.4.2.1/tests/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from django.db import models
-from django.utils.timezone import now
+from django.utils.timezone import now, localdate
 
 from django_glue.data_classes import GlueJsonResponseData
 
 
 class TestModel(models.Model):
     first_name = models.CharField(max_length=32)
     last_name = models.CharField(max_length=32)
     description = models.TextField()
     favorite_number = models.IntegerField()
     anniversary_datetime = models.DateTimeField(default=now)
-    birth_date = models.DateField(default=now)
+    birth_date = models.DateField(default=localdate)
     weight_lbs = models.DecimalField(max_digits=7, decimal_places=3)
 
     def __str__(self):
         return f'{self.first_name} {self.last_name}'
 
     def is_lighter_than(self, check_weight: float) -> bool:
         if self.weight_lbs < check_weight:
```

### Comparing `django-glue-0.4.2/tests/settings.py` & `django-glue-0.4.2.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/tests/urls.py` & `django-glue-0.4.2.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/tests/utils.py` & `django-glue-0.4.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2/tests/views.py` & `django-glue-0.4.2.1/tests/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class QuerySetView(TemplateView):
     template_name = 'page/query_set_page.html'
 
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
-        add_glue(self.request, 'test_query_1', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'delete', exclude=('birth_date', 'anniversary_datetime'), methods=['is_lighter_than', 'get_full_name'])
+        add_glue(self.request, 'test_query_1', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'delete', exclude=('anniversary_datetime', 'birth_date'), methods=['is_lighter_than', 'get_full_name'])
         add_glue(self.request, 'test_query_2', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'add', exclude=('birth_date', 'anniversary_datetime'))
         add_glue(self.request, 'test_query_3', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'change', exclude=('birth_date', 'anniversary_datetime'))
 
         context_data['model_object_id'] = TestModel.objects.filter(id__gte=1).filter(id__lte=10000).first().id
         return context_data
```

