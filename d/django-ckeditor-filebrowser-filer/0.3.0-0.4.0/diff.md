# Comparing `tmp/django-ckeditor-filebrowser-filer-0.3.0.tar.gz` & `tmp/django-ckeditor-filebrowser-filer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-ckeditor-filebrowser-filer-0.3.0.tar", last modified: Fri Mar 22 23:50:23 2019, max compression
+gzip compressed data, was "django-ckeditor-filebrowser-filer-0.4.0.tar", last modified: Thu Aug  3 10:53:56 2023, max compression
```

## Comparing `django-ckeditor-filebrowser-filer-0.3.0.tar` & `django-ckeditor-filebrowser-filer-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/admin/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/admin/img/
--rw-rw-r--   0 yakky     (1000)     1004     1200 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/admin/img/icon_deletelink.gif
--rw-rw-r--   0 yakky     (1000)     1004     1118 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/admin/img/icon_searchbox.png
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/dialogs/
--rwxrwxr-x   0 yakky     (1000)     1004    11870 2018-03-29 19:38:57.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/icons/
--rw-rw-r--   0 yakky     (1000)     1004     3573 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/
--rw-rw-r--   0 yakky     (1000)     1004      601 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/en.js
--rw-rw-r--   0 yakky     (1000)     1004      678 2017-03-14 07:34:09.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/fr.js
--rw-rw-r--   0 yakky     (1000)     1004      524 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/it.js
--rw-rw-r--   0 yakky     (1000)     1004      906 2018-03-29 19:38:54.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/ru.js
--rwxrwxr-x   0 yakky     (1000)     1004     3081 2018-03-29 19:38:54.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/plugin.js
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/dialogs/
--rwxrwxr-x   0 yakky     (1000)     1004    11870 2018-03-29 19:38:57.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/icons/
--rw-rw-r--   0 yakky     (1000)     1004     3573 2015-09-05 15:03:00.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/
--rw-rw-r--   0 yakky     (1000)     1004      601 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/en.js
--rw-rw-r--   0 yakky     (1000)     1004      678 2017-03-14 07:34:09.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/fr.js
--rw-rw-r--   0 yakky     (1000)     1004      524 2016-10-08 20:27:52.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/it.js
--rw-rw-r--   0 yakky     (1000)     1004      906 2018-03-29 19:38:54.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/ru.js
--rwxrwxr-x   0 yakky     (1000)     1004     3081 2018-03-29 19:38:54.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/plugin.js
--rw-rw-r--   0 yakky     (1000)     1004       46 2019-03-22 23:50:19.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/__init__.py
--rw-rw-r--   0 yakky     (1000)     1004       23 2015-08-23 10:36:42.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/models.py
--rw-rw-r--   0 yakky     (1000)     1004     1031 2017-01-01 21:50:06.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/urls.py
--rw-rw-r--   0 yakky     (1000)     1004     4444 2019-03-22 23:47:55.000000 django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/views.py
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/
--rw-rw-r--   0 yakky     (1000)     1004     7196 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/PKG-INFO
--rw-rw-r--   0 yakky     (1000)     1004     2009 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/SOURCES.txt
--rw-rw-r--   0 yakky     (1000)     1004        1 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/dependency_links.txt
--rw-rw-r--   0 yakky     (1000)     1004        1 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/not-zip-safe
--rw-rw-r--   0 yakky     (1000)     1004       18 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/requires.txt
--rw-rw-r--   0 yakky     (1000)     1004       27 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/top_level.txt
--rw-rw-r--   0 yakky     (1000)     1004      275 2018-03-29 19:39:45.000000 django-ckeditor-filebrowser-filer-0.3.0/AUTHORS.rst
--rw-rw-r--   0 yakky     (1000)     1004     3443 2015-08-23 10:36:42.000000 django-ckeditor-filebrowser-filer-0.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 yakky     (1000)     1004      955 2019-03-22 23:49:53.000000 django-ckeditor-filebrowser-filer-0.3.0/HISTORY.rst
--rw-rw-r--   0 yakky     (1000)     1004     1496 2015-08-23 10:36:42.000000 django-ckeditor-filebrowser-filer-0.3.0/LICENSE
--rw-rw-r--   0 yakky     (1000)     1004      193 2015-08-23 10:36:42.000000 django-ckeditor-filebrowser-filer-0.3.0/MANIFEST.in
--rw-rw-r--   0 yakky     (1000)     1004     3895 2019-03-22 23:49:53.000000 django-ckeditor-filebrowser-filer-0.3.0/README.rst
--rw-rw-r--   0 yakky     (1000)     1004      125 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/setup.cfg
--rwxrwxr-x   0 yakky     (1000)     1004     1860 2019-03-22 23:49:53.000000 django-ckeditor-filebrowser-filer-0.3.0/setup.py
--rw-rw-r--   0 yakky     (1000)     1004     7196 2019-03-22 23:50:23.000000 django-ckeditor-filebrowser-filer-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.578996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/admin/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/admin/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/admin/img/icon_searchbox.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.578996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.582996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:53:56.586996 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-08-03 10:53:56.000000 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-03 10:53:56.000000 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:53:56.000000 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:53:40.000000 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 10:53:56.000000 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 10:53:56.000000 django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-03 10:53:56.590996 django-ckeditor-filebrowser-filer-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:53:09.000000 django-ckeditor-filebrowser-filer-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/admin/img/icon_deletelink.gif` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/admin/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/admin/img/icon_searchbox.png` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/admin/img/icon_searchbox.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/en.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/fr.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/it.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/ru.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/plugin.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/ckeditor/ckeditor/plugins/filerimage/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/dialogs/filerImageDialog.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/icons/filerimage.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/en.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/fr.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/it.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/ru.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/plugin.js` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/static/djangocms_text_ckeditor/ckeditor/plugins/filerimage/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/ckeditor_filebrowser_filer/views.py` & `django-ckeditor-filebrowser-filer-0.4.0/ckeditor_filebrowser_filer/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,59 @@
-# -*- coding: utf-8 -*-
 import json
-from distutils.version import LooseVersion
 
-from django import http
+from django import http, urls
 from django.conf import settings
-from django import urls
 from django.http import HttpResponseRedirect
-
-from filer.models import File
+from filer.models import File, ThumbnailOption
 from filer.server.views import server
 
-try:
-    from filer.models import ThumbnailOption
-except ImportError:
-    from cmsplugin_filer_image.models import ThumbnailOption
-
 
 def filer_version(request):
-    import filer
-    filer_legacy = LooseVersion(filer.__version__) < LooseVersion('1.1')
-    filer_11 = not filer_legacy and LooseVersion(filer.__version__) < LooseVersion('1.2')
-    filer_12 = LooseVersion(filer.__version__) >= LooseVersion('1.2')
-    if filer_11:
-        version = '1.1'
-    elif filer_12:
-        version = '1.2'
-    else:
-        version = '1.0'
+    version = "1.2"
     return http.HttpResponse(version)
 
 
 def get_setting(request, setting):
-    setting = 'CKEDITOR_FILEBROWSER_{}'.format(setting).upper()
+    setting = "CKEDITOR_FILEBROWSER_{}".format(setting).upper()
     try:
         return http.HttpResponse(int(getattr(settings, setting, False)))
     except ValueError:
         return http.HttpResponse(getattr(settings, setting, False))
 
 
 def url_reverse(request):
     """
     Reverse the requested URL (passed via GET / POST as `url_name` parameter)
 
     :param request: Request object
     :return: The reversed path
     """
-    if request.method in ('GET', 'POST'): 
-        data = getattr(request, request.method) 
-        url_name = data.get('url_name') 
-        try: 
-            path = urls.reverse(url_name, args=data.getlist('args')) 
+    if request.method in ("GET", "POST"):
+        data = getattr(request, request.method)
+        url_name = data.get("url_name")
+        try:
+            path = urls.reverse(url_name, args=data.getlist("args"))
             (view_func, args, kwargs) = urls.resolve(path)
-            return http.HttpResponse(path, content_type='text/plain')
-        except urls.NoReverseMatch: 
-            return http.HttpResponse('Error', content_type='text/plain')
-    return http.HttpResponseNotAllowed(('GET', 'POST'))
+            return http.HttpResponse(path, content_type="text/plain")
+        except urls.NoReverseMatch:
+            return http.HttpResponse("Error", content_type="text/plain")
+    return http.HttpResponseNotAllowed(("GET", "POST"))
 
 
 def _return_thumbnail(image, thumb_options=None, width=None, height=None):
     thumbnail_options = {}
     if thumb_options is not None:
         thumbnail_options = ThumbnailOption.objects.get(pk=thumb_options).as_dict
 
     if width is not None or height is not None:
         width = int(width)
         height = int(height)
 
         size = (width, height)
-        thumbnail_options.update({'size': size})
+        thumbnail_options.update({"size": size})
 
     if thumbnail_options != {}:
         thumbnailer = image.easy_thumbnails_thumbnailer
         image = thumbnailer.get_thumbnail(thumbnail_options)
         return image
     return None
 
@@ -84,38 +66,38 @@
     :param image_id: Filer image ID
     :param thumb_options: ThumbnailOption ID
     :param width: user-provided width
     :param height: user-provided height
     :return: JSON serialized URL components ('url', 'width', 'height')
     """
     image = File.objects.get(pk=image_id)
-    if getattr(image, 'canonical_url', None):
+    if getattr(image, "canonical_url", None):
         url = image.canonical_url
     else:
         url = image.url
     thumb = _return_thumbnail(image, thumb_options, width, height)
     if thumb:
         image = thumb
         url = image.url
     data = {
-        'url': url,
-        'width': image.width,
-        'height': image.height,
+        "url": url,
+        "width": image.width,
+        "height": image.height,
     }
-    return http.HttpResponse(json.dumps(data), content_type='application/json')
+    return http.HttpResponse(json.dumps(data), content_type="application/json")
 
 
 def thumbnail_options(request):
     """
     Returns the requested ThumbnailOption as JSON
 
     :param request: Request object
     :return: JSON serialized ThumbnailOption
     """
-    response_data = [{'id': opt.pk, 'name': opt.name} for opt in ThumbnailOption.objects.all()]
+    response_data = [{"id": opt.pk, "name": opt.name} for opt in ThumbnailOption.objects.all()]
     return http.HttpResponse(json.dumps(response_data), content_type="application/json")
 
 
 def serve_image(request, image_id, thumb_options=None, width=None, height=None):
     """
     returns the content of an image sized according to the parameters
 
@@ -123,15 +105,15 @@
     :param image_id: Filer image ID
     :param thumb_options: ThumbnailOption ID
     :param width: user-provided width
     :param height: user-provided height
     :return: JSON serialized URL components ('url', 'width', 'height')
     """
     image = File.objects.get(pk=image_id)
-    if getattr(image, 'canonical_url', None):
+    if getattr(image, "canonical_url", None):
         url = image.canonical_url
     else:
         url = image.url
     thumb = _return_thumbnail(image, thumb_options, width, height)
     if thumb:
         return server.serve(request, file_obj=thumb, save_as=False)
     else:
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/PKG-INFO` & `django-ckeditor-filebrowser-filer-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,192 +1,197 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-ckeditor-filebrowser-filer
-Version: 0.3.0
+Version: 0.4.0
 Summary: A django-filer based CKEditor filebrowser
 Home-page: https://github.com/nephila/django-ckeditor-filebrowser-filer
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: BSD
-Description: =================================
-        django-ckeditor-filebrowser-filer
-        =================================
-        
-        |Gitter| |PyPiVersion| |PyVersion| |License|
-        
-        A django-filer based CKEditor filebrowser
-        
-        Supported versions
-        ==================
-        
-        Python: 2.7, 3.5, 3.6, 2.7
-        
-        Django: 1.11 to 2.1
-        
-        django-filer: 1.2 and above
-        
-        Documentation
-        -------------
-        
-        Original code is taken from `django-ckeditor-filer`_
-        
-        It supports both ckeditor widget provided by `django-ckeditor`_ and the one provided
-        by `djangocms-text-ckeditor`_.
-        
-        .. warning:: if you are using filer<1.2 this plugin requires `django CMS`_
-          `cmsplugin_filer_image`_, thus you need to install and configure both according
-          to their respective documentation.
-        
-        
-        Quickstart
-        ----------
-        
-        * Install django-ckeditor-filebrowser-filer::
-        
-            pip install django-ckeditor-filebrowser-filer
-        
-        * Add it to INSTALLED_APPS along with its dependencies::
-        
-            'filer',
-            'ckeditor_filebrowser_filer',
-        
-        * Configure django-filer `Canonical URLs`_
-        
-        * Add `ckeditor_filebrowser_filer` to urlconf::
-        
-            url(r'^filebrowser_filer/', include('ckeditor_filebrowser_filer.urls')),
-        
-          Currently only ``filebrowser_filer/`` is supported as url path
-        
-        * Add `FilerImage` button to you CKEditor configuration:
-        
-          * Add ``'FilerImage'`` to a toolbar in ``CKEDITOR_CONFIGS``
-          * Add ``'filerimage'`` in `` 'extraPlugins'`` in ``CKEDITOR_CONFIGS``
-          * Add ``'image'`` in `` 'removePlugins'`` in ``CKEDITOR_CONFIGS``
-        
-        Example::
-        
-            CKEDITOR_CONFIGS = {
-                'default': {
-                    'toolbar': 'Custom',
-                    'toolbar_Custom': [
-                        ...
-                        ['FilerImage']
-                    ],
-                    'extraPlugins': 'filerimage',
-                    'removePlugins': 'image'
-                },
-            }
-        
-        when using `djangocms-text-ckeditor`_ use ``CKEDITOR_SETTINGS`` instead of
-        ``CKEDITOR_CONFIGS``.
-        
-        
-        .. _Canonical URLs: https://django-filer.readthedocs.io/en/latest/installation.html#canonical-urls
-        .. _django CMS: https://pypi.python.org/pypi/django-cms
-        .. _django-filer: https://pypi.python.org/pypi/django-filer
-        .. _cmsplugin_filer_image: https://pypi.python.org/pypi/cmsplugin_filer_image
-        .. _django-ckeditor: https://pypi.python.org/pypi/django-ckeditor
-        .. _djangocms-text-ckeditor: https://pypi.python.org/pypi/djangocms-text-ckeditor
-        .. _django-ckeditor-filer: https://github.com/ikresoft/django-ckeditor-filer/
-        
-        
-        .. |Gitter| image:: https://img.shields.io/badge/GITTER-join%20chat-brightgreen.svg?style=flat-square
-            :target: https://gitter.im/nephila/applications
-            :alt: Join the Gitter chat
-        
-        .. |PyPiVersion| image:: https://img.shields.io/pypi/v/django-ckeditor-filebrowser-filer.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
-            :alt: Latest PyPI version
-        
-        .. |PyVersion| image:: https://img.shields.io/pypi/pyversions/django-ckeditor-filebrowser-filer.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
-            :alt: Python versions
-        
-        .. |Status| image:: https://img.shields.io/travis/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
-            :target: https://travis-ci.org/nephila/django-ckeditor-filebrowser-filer
-            :alt: Latest Travis CI build status
-        
-        .. |TestCoverage| image:: https://img.shields.io/coveralls/nephila/django-ckeditor-filebrowser-filer/master.svg?style=flat-square
-            :target: https://coveralls.io/r/nephila/django-ckeditor-filebrowser-filer?branch=master
-            :alt: Test coverage
-        
-        .. |License| image:: https://img.shields.io/github/license/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
-           :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer/
-            :alt: License
-        
-        .. |CodeClimate| image:: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer/badges/gpa.svg?style=flat-square
-           :target: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer
-           :alt: Code Climate
-        
-        
-        
-        
-        History
-        -------
-        
-        0.3.0 (2019-03-23)
-        ++++++++++++++++++
-        
-        * Added compatibility with Django 2.0
-        
-        0.2.5 (2018-03-29)
-        ++++++++++++++++++
-        
-        * Fixed error when editing an image
-        
-        0.2.4 (2018-01-09)
-        ++++++++++++++++++
-        
-        * Fixed filer version detection
-        * Added support for Django 1.11
-        
-        0.2.3 (2017-04-19)
-        ++++++++++++++++++
-        
-        * Added russian translations
-        
-        0.2.2 (2017-03-14)
-        ++++++++++++++++++
-        
-        * Added french translations
-        
-        0.2.1 (2017-01-01)
-        ++++++++++++++++++
-        
-        * Added support for Django 1.10
-        
-        0.2.0 (2016-10-22)
-        ++++++++++++++++++
-        
-        * Added support for canonical urls feature of filer 1.0
-        * Added support to django-ckeditor (without django CMS)
-        * Added support to filer up to 1.2
-        * Added support to ThumbnailOption
-        * Updated to work with djangocms-text-ckeditor 2.7
-        * Fixed support for advanced deployment structure
-        
-        0.1.1 (2014-09-27)
-        ++++++++++++++++++
-        
-        * Fix static files position
-        
-        0.1.0 (2014-01-27)
-        ++++++++++++++++++
-        
-        * First release on PyPI.
-        
-Keywords: django-ckeditor-filebrowser-filer,django,filer,ckeditor,filebrowser
-Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=================================
+django-ckeditor-filebrowser-filer
+=================================
+
+|Gitter| |PyPiVersion| |PyVersion| |License|
+
+A django-filer based CKEditor filebrowser
+
+Supported versions
+==================
+
+Python: 3.7 to 3.11
+
+Django: 3.2 to 4.2
+
+django-filer: 2.0 and above
+
+Documentation
+-------------
+
+Original code is taken from `django-ckeditor-filer`_
+
+It supports both ckeditor widget provided by `django-ckeditor`_ and the one provided
+by `djangocms-text-ckeditor`_.
+
+.. warning:: if you are using filer<1.2 this plugin requires `django CMS`_
+  `cmsplugin_filer_image`_, thus you need to install and configure both according
+  to their respective documentation.
+
+
+Quickstart
+----------
+
+* Install django-ckeditor-filebrowser-filer::
+
+    pip install django-ckeditor-filebrowser-filer
+
+* Add it to INSTALLED_APPS along with its dependencies::
+
+    'filer',
+    'ckeditor_filebrowser_filer',
+
+* Configure django-filer `Canonical URLs`_
+
+* Add `ckeditor_filebrowser_filer` to urlconf::
+
+    url(r'^filebrowser_filer/', include('ckeditor_filebrowser_filer.urls')),
+
+  Currently only ``filebrowser_filer/`` is supported as url path
+
+* Add `FilerImage` button to you CKEditor configuration:
+
+  * Add ``'FilerImage'`` to a toolbar in ``CKEDITOR_CONFIGS``
+  * Add ``'filerimage'`` in `` 'extraPlugins'`` in ``CKEDITOR_CONFIGS``
+  * Add ``'image'`` in `` 'removePlugins'`` in ``CKEDITOR_CONFIGS``
+
+Example::
+
+    CKEDITOR_CONFIGS = {
+        'default': {
+            'toolbar': 'Custom',
+            'toolbar_Custom': [
+                ...
+                ['FilerImage']
+            ],
+            'extraPlugins': 'filerimage',
+            'removePlugins': 'image'
+        },
+    }
+
+when using `djangocms-text-ckeditor`_ use ``CKEDITOR_SETTINGS`` instead of
+``CKEDITOR_CONFIGS``.
+
+
+.. _Canonical URLs: https://django-filer.readthedocs.io/en/latest/installation.html#canonical-urls
+.. _django CMS: https://pypi.python.org/pypi/django-cms
+.. _django-filer: https://pypi.python.org/pypi/django-filer
+.. _cmsplugin_filer_image: https://pypi.python.org/pypi/cmsplugin_filer_image
+.. _django-ckeditor: https://pypi.python.org/pypi/django-ckeditor
+.. _djangocms-text-ckeditor: https://pypi.python.org/pypi/djangocms-text-ckeditor
+.. _django-ckeditor-filer: https://github.com/ikresoft/django-ckeditor-filer/
+
+
+.. |Gitter| image:: https://img.shields.io/badge/GITTER-join%20chat-brightgreen.svg?style=flat-square
+    :target: https://gitter.im/nephila/applications
+    :alt: Join the Gitter chat
+
+.. |PyPiVersion| image:: https://img.shields.io/pypi/v/django-ckeditor-filebrowser-filer.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
+    :alt: Latest PyPI version
+
+.. |PyVersion| image:: https://img.shields.io/pypi/pyversions/django-ckeditor-filebrowser-filer.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
+    :alt: Python versions
+
+.. |Status| image:: https://img.shields.io/travis/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
+    :target: https://travis-ci.org/nephila/django-ckeditor-filebrowser-filer
+    :alt: Latest Travis CI build status
+
+.. |TestCoverage| image:: https://img.shields.io/coveralls/nephila/django-ckeditor-filebrowser-filer/master.svg?style=flat-square
+    :target: https://coveralls.io/r/nephila/django-ckeditor-filebrowser-filer?branch=master
+    :alt: Test coverage
+
+.. |License| image:: https://img.shields.io/github/license/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
+   :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer/
+    :alt: License
+
+.. |CodeClimate| image:: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer/badges/gpa.svg?style=flat-square
+   :target: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer
+   :alt: Code Climate
+
+.. :changelog:
+
+History
+-------
+
+0.4.0 (2023-08-03)
+++++++++++++++++++
+
+* Added compatibility with Django 4.2
+* Drop support for Django<3.2
+
+0.3.0 (2019-03-23)
+++++++++++++++++++
+
+* Added compatibility with Django 2.0
+
+0.2.5 (2018-03-29)
+++++++++++++++++++
+
+* Fixed error when editing an image
+
+0.2.4 (2018-01-09)
+++++++++++++++++++
+
+* Fixed filer version detection
+* Added support for Django 1.11
+
+0.2.3 (2017-04-19)
+++++++++++++++++++
+
+* Added russian translations
+
+0.2.2 (2017-03-14)
+++++++++++++++++++
+
+* Added french translations
+
+0.2.1 (2017-01-01)
+++++++++++++++++++
+
+* Added support for Django 1.10
+
+0.2.0 (2016-10-22)
+++++++++++++++++++
+
+* Added support for canonical urls feature of filer 1.0
+* Added support to django-ckeditor (without django CMS)
+* Added support to filer up to 1.2
+* Added support to ThumbnailOption
+* Updated to work with djangocms-text-ckeditor 2.7
+* Fixed support for advanced deployment structure
+
+0.1.1 (2014-09-27)
+++++++++++++++++++
+
+* Fix static files position
+
+0.1.0 (2014-01-27)
+++++++++++++++++++
+
+* First release on PyPI.
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/django_ckeditor_filebrowser_filer.egg-info/SOURCES.txt` & `django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 ckeditor_filebrowser_filer/__init__.py
 ckeditor_filebrowser_filer/models.py
 ckeditor_filebrowser_filer/urls.py
 ckeditor_filebrowser_filer/views.py
 ckeditor_filebrowser_filer/static/admin/img/icon_deletelink.gif
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/CONTRIBUTING.rst` & `django-ckeditor-filebrowser-filer-0.4.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ============
 Contributing
 ============
 
 Contributions are welcome, and they are greatly appreciated! Every
-little bit helps, and credit will always be given. 
+little bit helps, and credit will always be given.
 
 You can contribute in many ways:
 
 Types of Contributions
 ----------------------
 
 Report Bugs
@@ -32,15 +32,15 @@
 
 Look through the GitHub issues for features. Anything tagged with "feature"
 is open to whoever wants to implement it.
 
 Write Documentation
 ~~~~~~~~~~~~~~~~~~~
 
-django-ckeditor-filebrowser-filer could always use more documentation, whether as part of the 
+django-ckeditor-filebrowser-filer could always use more documentation, whether as part of the
 official django-ckeditor-filebrowser-filer docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
 The best way to send feedback is to file an issue at https://github.com/nephila/django-ckeditor-filebrowser-filer/issues.
@@ -77,15 +77,15 @@
 5. When you're done making changes, check that your changes pass flake8 and the
 tests, including testing other Python versions with tox::
 
     $ flake8 ckeditor_filebrowser_filer tests
     $ python setup.py test
     $ tox
 
-To get flake8 and tox, just pip install them into your virtualenv. 
+To get flake8 and tox, just pip install them into your virtualenv.
 
 6. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
@@ -96,17 +96,17 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check 
+3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check
    https://travis-ci.org/nephila/django-ckeditor-filebrowser-filer/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
-    $ python -m unittest tests.test_ckeditor_filebrowser_filer
+    $ python -m unittest tests.test_ckeditor_filebrowser_filer
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/HISTORY.rst` & `django-ckeditor-filebrowser-filer-0.4.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.4.0 (2023-08-03)
+++++++++++++++++++
+
+* Added compatibility with Django 4.2
+* Drop support for Django<3.2
+
 0.3.0 (2019-03-23)
 ++++++++++++++++++
 
 * Added compatibility with Django 2.0
 
 0.2.5 (2018-03-29)
 ++++++++++++++++++
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/LICENSE` & `django-ckeditor-filebrowser-filer-0.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
 * Neither the name of django-ckeditor-filebrowser-filer nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/README.rst` & `django-ckeditor-filebrowser-filer-0.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 |Gitter| |PyPiVersion| |PyVersion| |License|
 
 A django-filer based CKEditor filebrowser
 
 Supported versions
 ==================
 
-Python: 2.7, 3.5, 3.6, 2.7
+Python: 3.7 to 3.11
 
-Django: 1.11 to 2.1
+Django: 3.2 to 4.2
 
-django-filer: 1.2 and above
+django-filer: 2.0 and above
 
 Documentation
 -------------
 
 Original code is taken from `django-ckeditor-filer`_
 
 It supports both ckeditor widget provided by `django-ckeditor`_ and the one provided
```

### Comparing `django-ckeditor-filebrowser-filer-0.3.0/PKG-INFO` & `django-ckeditor-filebrowser-filer-0.4.0/django_ckeditor_filebrowser_filer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,192 +1,197 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-ckeditor-filebrowser-filer
-Version: 0.3.0
+Version: 0.4.0
 Summary: A django-filer based CKEditor filebrowser
 Home-page: https://github.com/nephila/django-ckeditor-filebrowser-filer
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: BSD
-Description: =================================
-        django-ckeditor-filebrowser-filer
-        =================================
-        
-        |Gitter| |PyPiVersion| |PyVersion| |License|
-        
-        A django-filer based CKEditor filebrowser
-        
-        Supported versions
-        ==================
-        
-        Python: 2.7, 3.5, 3.6, 2.7
-        
-        Django: 1.11 to 2.1
-        
-        django-filer: 1.2 and above
-        
-        Documentation
-        -------------
-        
-        Original code is taken from `django-ckeditor-filer`_
-        
-        It supports both ckeditor widget provided by `django-ckeditor`_ and the one provided
-        by `djangocms-text-ckeditor`_.
-        
-        .. warning:: if you are using filer<1.2 this plugin requires `django CMS`_
-          `cmsplugin_filer_image`_, thus you need to install and configure both according
-          to their respective documentation.
-        
-        
-        Quickstart
-        ----------
-        
-        * Install django-ckeditor-filebrowser-filer::
-        
-            pip install django-ckeditor-filebrowser-filer
-        
-        * Add it to INSTALLED_APPS along with its dependencies::
-        
-            'filer',
-            'ckeditor_filebrowser_filer',
-        
-        * Configure django-filer `Canonical URLs`_
-        
-        * Add `ckeditor_filebrowser_filer` to urlconf::
-        
-            url(r'^filebrowser_filer/', include('ckeditor_filebrowser_filer.urls')),
-        
-          Currently only ``filebrowser_filer/`` is supported as url path
-        
-        * Add `FilerImage` button to you CKEditor configuration:
-        
-          * Add ``'FilerImage'`` to a toolbar in ``CKEDITOR_CONFIGS``
-          * Add ``'filerimage'`` in `` 'extraPlugins'`` in ``CKEDITOR_CONFIGS``
-          * Add ``'image'`` in `` 'removePlugins'`` in ``CKEDITOR_CONFIGS``
-        
-        Example::
-        
-            CKEDITOR_CONFIGS = {
-                'default': {
-                    'toolbar': 'Custom',
-                    'toolbar_Custom': [
-                        ...
-                        ['FilerImage']
-                    ],
-                    'extraPlugins': 'filerimage',
-                    'removePlugins': 'image'
-                },
-            }
-        
-        when using `djangocms-text-ckeditor`_ use ``CKEDITOR_SETTINGS`` instead of
-        ``CKEDITOR_CONFIGS``.
-        
-        
-        .. _Canonical URLs: https://django-filer.readthedocs.io/en/latest/installation.html#canonical-urls
-        .. _django CMS: https://pypi.python.org/pypi/django-cms
-        .. _django-filer: https://pypi.python.org/pypi/django-filer
-        .. _cmsplugin_filer_image: https://pypi.python.org/pypi/cmsplugin_filer_image
-        .. _django-ckeditor: https://pypi.python.org/pypi/django-ckeditor
-        .. _djangocms-text-ckeditor: https://pypi.python.org/pypi/djangocms-text-ckeditor
-        .. _django-ckeditor-filer: https://github.com/ikresoft/django-ckeditor-filer/
-        
-        
-        .. |Gitter| image:: https://img.shields.io/badge/GITTER-join%20chat-brightgreen.svg?style=flat-square
-            :target: https://gitter.im/nephila/applications
-            :alt: Join the Gitter chat
-        
-        .. |PyPiVersion| image:: https://img.shields.io/pypi/v/django-ckeditor-filebrowser-filer.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
-            :alt: Latest PyPI version
-        
-        .. |PyVersion| image:: https://img.shields.io/pypi/pyversions/django-ckeditor-filebrowser-filer.svg?style=flat-square
-            :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
-            :alt: Python versions
-        
-        .. |Status| image:: https://img.shields.io/travis/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
-            :target: https://travis-ci.org/nephila/django-ckeditor-filebrowser-filer
-            :alt: Latest Travis CI build status
-        
-        .. |TestCoverage| image:: https://img.shields.io/coveralls/nephila/django-ckeditor-filebrowser-filer/master.svg?style=flat-square
-            :target: https://coveralls.io/r/nephila/django-ckeditor-filebrowser-filer?branch=master
-            :alt: Test coverage
-        
-        .. |License| image:: https://img.shields.io/github/license/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
-           :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer/
-            :alt: License
-        
-        .. |CodeClimate| image:: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer/badges/gpa.svg?style=flat-square
-           :target: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer
-           :alt: Code Climate
-        
-        
-        
-        
-        History
-        -------
-        
-        0.3.0 (2019-03-23)
-        ++++++++++++++++++
-        
-        * Added compatibility with Django 2.0
-        
-        0.2.5 (2018-03-29)
-        ++++++++++++++++++
-        
-        * Fixed error when editing an image
-        
-        0.2.4 (2018-01-09)
-        ++++++++++++++++++
-        
-        * Fixed filer version detection
-        * Added support for Django 1.11
-        
-        0.2.3 (2017-04-19)
-        ++++++++++++++++++
-        
-        * Added russian translations
-        
-        0.2.2 (2017-03-14)
-        ++++++++++++++++++
-        
-        * Added french translations
-        
-        0.2.1 (2017-01-01)
-        ++++++++++++++++++
-        
-        * Added support for Django 1.10
-        
-        0.2.0 (2016-10-22)
-        ++++++++++++++++++
-        
-        * Added support for canonical urls feature of filer 1.0
-        * Added support to django-ckeditor (without django CMS)
-        * Added support to filer up to 1.2
-        * Added support to ThumbnailOption
-        * Updated to work with djangocms-text-ckeditor 2.7
-        * Fixed support for advanced deployment structure
-        
-        0.1.1 (2014-09-27)
-        ++++++++++++++++++
-        
-        * Fix static files position
-        
-        0.1.0 (2014-01-27)
-        ++++++++++++++++++
-        
-        * First release on PyPI.
-        
-Keywords: django-ckeditor-filebrowser-filer,django,filer,ckeditor,filebrowser
-Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=================================
+django-ckeditor-filebrowser-filer
+=================================
+
+|Gitter| |PyPiVersion| |PyVersion| |License|
+
+A django-filer based CKEditor filebrowser
+
+Supported versions
+==================
+
+Python: 3.7 to 3.11
+
+Django: 3.2 to 4.2
+
+django-filer: 2.0 and above
+
+Documentation
+-------------
+
+Original code is taken from `django-ckeditor-filer`_
+
+It supports both ckeditor widget provided by `django-ckeditor`_ and the one provided
+by `djangocms-text-ckeditor`_.
+
+.. warning:: if you are using filer<1.2 this plugin requires `django CMS`_
+  `cmsplugin_filer_image`_, thus you need to install and configure both according
+  to their respective documentation.
+
+
+Quickstart
+----------
+
+* Install django-ckeditor-filebrowser-filer::
+
+    pip install django-ckeditor-filebrowser-filer
+
+* Add it to INSTALLED_APPS along with its dependencies::
+
+    'filer',
+    'ckeditor_filebrowser_filer',
+
+* Configure django-filer `Canonical URLs`_
+
+* Add `ckeditor_filebrowser_filer` to urlconf::
+
+    url(r'^filebrowser_filer/', include('ckeditor_filebrowser_filer.urls')),
+
+  Currently only ``filebrowser_filer/`` is supported as url path
+
+* Add `FilerImage` button to you CKEditor configuration:
+
+  * Add ``'FilerImage'`` to a toolbar in ``CKEDITOR_CONFIGS``
+  * Add ``'filerimage'`` in `` 'extraPlugins'`` in ``CKEDITOR_CONFIGS``
+  * Add ``'image'`` in `` 'removePlugins'`` in ``CKEDITOR_CONFIGS``
+
+Example::
+
+    CKEDITOR_CONFIGS = {
+        'default': {
+            'toolbar': 'Custom',
+            'toolbar_Custom': [
+                ...
+                ['FilerImage']
+            ],
+            'extraPlugins': 'filerimage',
+            'removePlugins': 'image'
+        },
+    }
+
+when using `djangocms-text-ckeditor`_ use ``CKEDITOR_SETTINGS`` instead of
+``CKEDITOR_CONFIGS``.
+
+
+.. _Canonical URLs: https://django-filer.readthedocs.io/en/latest/installation.html#canonical-urls
+.. _django CMS: https://pypi.python.org/pypi/django-cms
+.. _django-filer: https://pypi.python.org/pypi/django-filer
+.. _cmsplugin_filer_image: https://pypi.python.org/pypi/cmsplugin_filer_image
+.. _django-ckeditor: https://pypi.python.org/pypi/django-ckeditor
+.. _djangocms-text-ckeditor: https://pypi.python.org/pypi/djangocms-text-ckeditor
+.. _django-ckeditor-filer: https://github.com/ikresoft/django-ckeditor-filer/
+
+
+.. |Gitter| image:: https://img.shields.io/badge/GITTER-join%20chat-brightgreen.svg?style=flat-square
+    :target: https://gitter.im/nephila/applications
+    :alt: Join the Gitter chat
+
+.. |PyPiVersion| image:: https://img.shields.io/pypi/v/django-ckeditor-filebrowser-filer.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
+    :alt: Latest PyPI version
+
+.. |PyVersion| image:: https://img.shields.io/pypi/pyversions/django-ckeditor-filebrowser-filer.svg?style=flat-square
+    :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer
+    :alt: Python versions
+
+.. |Status| image:: https://img.shields.io/travis/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
+    :target: https://travis-ci.org/nephila/django-ckeditor-filebrowser-filer
+    :alt: Latest Travis CI build status
+
+.. |TestCoverage| image:: https://img.shields.io/coveralls/nephila/django-ckeditor-filebrowser-filer/master.svg?style=flat-square
+    :target: https://coveralls.io/r/nephila/django-ckeditor-filebrowser-filer?branch=master
+    :alt: Test coverage
+
+.. |License| image:: https://img.shields.io/github/license/nephila/django-ckeditor-filebrowser-filer.svg?style=flat-square
+   :target: https://pypi.python.org/pypi/django-ckeditor-filebrowser-filer/
+    :alt: License
+
+.. |CodeClimate| image:: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer/badges/gpa.svg?style=flat-square
+   :target: https://codeclimate.com/github/nephila/django-ckeditor-filebrowser-filer
+   :alt: Code Climate
+
+.. :changelog:
+
+History
+-------
+
+0.4.0 (2023-08-03)
+++++++++++++++++++
+
+* Added compatibility with Django 4.2
+* Drop support for Django<3.2
+
+0.3.0 (2019-03-23)
+++++++++++++++++++
+
+* Added compatibility with Django 2.0
+
+0.2.5 (2018-03-29)
+++++++++++++++++++
+
+* Fixed error when editing an image
+
+0.2.4 (2018-01-09)
+++++++++++++++++++
+
+* Fixed filer version detection
+* Added support for Django 1.11
+
+0.2.3 (2017-04-19)
+++++++++++++++++++
+
+* Added russian translations
+
+0.2.2 (2017-03-14)
+++++++++++++++++++
+
+* Added french translations
+
+0.2.1 (2017-01-01)
+++++++++++++++++++
+
+* Added support for Django 1.10
+
+0.2.0 (2016-10-22)
+++++++++++++++++++
+
+* Added support for canonical urls feature of filer 1.0
+* Added support to django-ckeditor (without django CMS)
+* Added support to filer up to 1.2
+* Added support to ThumbnailOption
+* Updated to work with djangocms-text-ckeditor 2.7
+* Fixed support for advanced deployment structure
+
+0.1.1 (2014-09-27)
+++++++++++++++++++
+
+* Fix static files position
+
+0.1.0 (2014-01-27)
+++++++++++++++++++
+
+* First release on PyPI.
```

