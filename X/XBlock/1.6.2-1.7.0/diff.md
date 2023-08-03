# Comparing `tmp/XBlock-1.6.2.tar.gz` & `tmp/XBlock-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XBlock-1.6.2.tar", last modified: Fri Jan 27 19:25:39 2023, max compression
+gzip compressed data, was "XBlock-1.7.0.tar", last modified: Thu Aug  3 13:56:29 2023, max compression
```

## Comparing `XBlock-1.6.2.tar` & `XBlock-1.7.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.066269 XBlock-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-01-27 19:25:36.000000 XBlock-1.6.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-01-27 19:25:36.000000 XBlock-1.6.2/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-01-27 19:25:36.000000 XBlock-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-01-27 19:25:36.000000 XBlock-1.6.2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-01-27 19:25:39.066269 XBlock-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5602 2023-01-27 19:25:36.000000 XBlock-1.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.062270 XBlock-1.6.2/XBlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-01-27 19:25:38.000000 XBlock-1.6.2/XBlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-01-27 19:25:39.000000 XBlock-1.6.2/XBlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-27 19:25:38.000000 XBlock-1.6.2/XBlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-01-27 19:25:38.000000 XBlock-1.6.2/XBlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-27 19:25:38.000000 XBlock-1.6.2/XBlock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-01-27 19:25:39.070270 XBlock-1.6.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1807 2023-01-27 19:25:36.000000 XBlock-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.062270 XBlock-1.6.2/xblock/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/completable.py
--rw-r--r--   0 runner    (1001) docker     (122)    11650 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.066269 XBlock-1.6.2/xblock/django/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/django/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4374 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/field_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    39066 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/fragment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/internal.py
--rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     6676 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.066269 XBlock-1.6.2/xblock/reference/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/reference/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/reference/user_service.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/run_script.py
--rw-r--r--   0 runner    (1001) docker     (122)    49193 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/scorable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.066269 XBlock-1.6.2/xblock/test/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.066269 XBlock-1.6.2/xblock/test/django/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/django/test_field_translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/django/test_request.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.062270 XBlock-1.6.2/xblock/test/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.062270 XBlock-1.6.2/xblock/test/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 19:25:39.066269 XBlock-1.6.2/xblock/test/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     7432 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_asides.py
--rw-r--r--   0 runner    (1001) docker     (122)     5560 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_completable.py
--rw-r--r--   0 runner    (1001) docker     (122)    40042 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_field_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31443 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)    18963 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2534 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_json_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)    18738 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    17659 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)    27326 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)     2350 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_scorable.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_user_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     4439 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/test/toy_runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3364 2023-01-27 19:25:36.000000 XBlock-1.6.2/xblock/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.465762 XBlock-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-08-03 13:56:25.000000 XBlock-1.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-03 13:56:25.000000 XBlock-1.7.0/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-08-03 13:56:25.000000 XBlock-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-08-03 13:56:25.000000 XBlock-1.7.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-08-03 13:56:29.465762 XBlock-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-08-03 13:56:25.000000 XBlock-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.461762 XBlock-1.7.0/XBlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-08-03 13:56:29.000000 XBlock-1.7.0/XBlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-08-03 13:56:29.000000 XBlock-1.7.0/XBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 13:56:29.000000 XBlock-1.7.0/XBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-08-03 13:56:29.000000 XBlock-1.7.0/XBlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-03 13:56:29.000000 XBlock-1.7.0/XBlock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-08-03 13:56:29.465762 XBlock-1.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1807 2023-08-03 13:56:25.000000 XBlock-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.461762 XBlock-1.7.0/xblock/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/completable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11650 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.461762 XBlock-1.7.0/xblock/django/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/django/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4374 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/field_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39066 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/internal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6676 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.461762 XBlock-1.7.0/xblock/reference/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/reference/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/reference/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/run_script.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49193 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/scorable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.465762 XBlock-1.7.0/xblock/test/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.465762 XBlock-1.7.0/xblock/test/django/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/django/test_field_translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/django/test_request.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.457762 XBlock-1.7.0/xblock/test/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.457762 XBlock-1.7.0/xblock/test/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:56:29.465762 XBlock-1.7.0/xblock/test/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7432 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_asides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5560 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_completable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40042 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_field_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31443 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18963 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2534 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_json_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18738 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17659 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27326 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2350 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_scorable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_user_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4439 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/test/toy_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3364 2023-08-03 13:56:25.000000 XBlock-1.7.0/xblock/validation.py
```

### Comparing `XBlock-1.6.2/AUTHORS` & `XBlock-1.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/LICENSE.TXT` & `XBlock-1.7.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/NOTICE.txt` & `XBlock-1.7.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/PKG-INFO` & `XBlock-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBlock
-Version: 1.6.2
+Version: 1.7.0
 Summary: XBlock Core Library
 Home-page: https://github.com/openedx/XBlock
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `XBlock-1.6.2/XBlock.egg-info/PKG-INFO` & `XBlock-1.7.0/XBlock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBlock
-Version: 1.6.2
+Version: 1.7.0
 Summary: XBlock Core Library
 Home-page: https://github.com/openedx/XBlock
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `XBlock-1.6.2/XBlock.egg-info/SOURCES.txt` & `XBlock-1.7.0/XBlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/setup.py` & `XBlock-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/__init__.py` & `XBlock-1.7.0/xblock/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         super().__init__(*args, **kwargs)
 
 
 # For backwards compatibility, provide the XBlockMixin in xblock.fields
 # without causing a circular import
 xblock.fields.XBlockMixin = XBlockMixin
 
-__version__ = '1.6.2'
+__version__ = '1.7.0'
```

### Comparing `XBlock-1.6.2/xblock/completable.py` & `XBlock-1.7.0/xblock/completable.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/core.py` & `XBlock-1.7.0/xblock/core.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/django/request.py` & `XBlock-1.7.0/xblock/django/request.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/exceptions.py` & `XBlock-1.7.0/xblock/exceptions.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/field_data.py` & `XBlock-1.7.0/xblock/field_data.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/fields.py` & `XBlock-1.7.0/xblock/fields.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/fragment.py` & `XBlock-1.7.0/xblock/fragment.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/internal.py` & `XBlock-1.7.0/xblock/internal.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/mixins.py` & `XBlock-1.7.0/xblock/mixins.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/plugin.py` & `XBlock-1.7.0/xblock/plugin.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/reference/plugins.py` & `XBlock-1.7.0/xblock/reference/plugins.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/reference/user_service.py` & `XBlock-1.7.0/xblock/reference/user_service.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/runtime.py` & `XBlock-1.7.0/xblock/runtime.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/scorable.py` & `XBlock-1.7.0/xblock/scorable.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/django/test_field_translation.py` & `XBlock-1.7.0/xblock/test/django/test_field_translation.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/django/test_request.py` & `XBlock-1.7.0/xblock/test/django/test_request.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/locale/de/LC_MESSAGES/django.po` & `XBlock-1.7.0/xblock/test/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/settings.py` & `XBlock-1.7.0/xblock/test/settings.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_asides.py` & `XBlock-1.7.0/xblock/test/test_asides.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_completable.py` & `XBlock-1.7.0/xblock/test/test_completable.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_core.py` & `XBlock-1.7.0/xblock/test/test_core.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_field_data.py` & `XBlock-1.7.0/xblock/test/test_field_data.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_fields.py` & `XBlock-1.7.0/xblock/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_fields_api.py` & `XBlock-1.7.0/xblock/test/test_fields_api.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_fragment.py` & `XBlock-1.7.0/xblock/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_internal.py` & `XBlock-1.7.0/xblock/test/test_internal.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_json_conversion.py` & `XBlock-1.7.0/xblock/test/test_json_conversion.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_mixins.py` & `XBlock-1.7.0/xblock/test/test_mixins.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_parsing.py` & `XBlock-1.7.0/xblock/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_plugin.py` & `XBlock-1.7.0/xblock/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_runtime.py` & `XBlock-1.7.0/xblock/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_scorable.py` & `XBlock-1.7.0/xblock/test/test_scorable.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_test_tools.py` & `XBlock-1.7.0/xblock/test/test_test_tools.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_user_service.py` & `XBlock-1.7.0/xblock/test/test_user_service.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/test_validation.py` & `XBlock-1.7.0/xblock/test/test_validation.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/tools.py` & `XBlock-1.7.0/xblock/test/tools.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/test/toy_runtime.py` & `XBlock-1.7.0/xblock/test/toy_runtime.py`

 * *Files identical despite different names*

### Comparing `XBlock-1.6.2/xblock/validation.py` & `XBlock-1.7.0/xblock/validation.py`

 * *Files identical despite different names*

