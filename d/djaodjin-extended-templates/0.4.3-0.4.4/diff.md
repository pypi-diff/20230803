# Comparing `tmp/djaodjin-extended-templates-0.4.3.tar.gz` & `tmp/djaodjin-extended-templates-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-extended-templates-0.4.3.tar", last modified: Fri Jul  7 15:33:51 2023, max compression
+gzip compressed data, was "djaodjin-extended-templates-0.4.4.tar", last modified: Thu Aug  3 00:40:43 2023, max compression
```

## Comparing `djaodjin-extended-templates-0.4.3.tar` & `djaodjin-extended-templates-0.4.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.315857 djaodjin-extended-templates-0.4.3/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     2687 2023-07-07 15:33:51.315922 djaodjin-extended-templates-0.4.3/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1868 2023-07-07 15:32:14.000000 djaodjin-extended-templates-0.4.3/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.301870 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     2687 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2641 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      227 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       19 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/top_level.txt
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.305028 djaodjin-extended-templates-0.4.3/extended_templates/
--rw-r--r--   0 smirolo    (501) staff       (20)     1447 2023-07-07 15:32:44.000000 djaodjin-extended-templates-0.4.3/extended_templates/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.306845 djaodjin-extended-templates-0.4.3/extended_templates/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4265 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/less_variables.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3582 2023-02-24 18:30:59.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1976 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/sitecss.py
--rw-r--r--   0 smirolo    (501) staff       (20)    19365 2023-02-17 19:40:33.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/sources.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5034 2023-02-03 04:47:19.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9953 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/upload_media.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.307776 djaodjin-extended-templates-0.4.3/extended_templates/backends/
--rw-r--r--   0 smirolo    (501) staff       (20)     3261 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9469 2023-04-05 21:35:22.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/eml.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9459 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/pdf.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1721 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/s3.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7332 2023-02-07 21:34:10.000000 djaodjin-extended-templates-0.4.3/extended_templates/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2934 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/decorators.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3188 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3058 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/extras.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3152 2023-02-08 00:52:56.000000 djaodjin-extended-templates-0.4.3/extended_templates/helpers.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.307937 djaodjin-extended-templates-0.4.3/extended_templates/management/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.308330 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2696 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/install_theme.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3398 2023-02-13 23:22:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/list_css_classes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6691 2023-02-07 20:38:57.000000 djaodjin-extended-templates-0.4.3/extended_templates/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3581 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10334 2022-08-23 21:36:15.000000 djaodjin-extended-templates-0.4.3/extended_templates/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1471 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.299581 djaodjin-extended-templates-0.4.3/extended_templates/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.311159 djaodjin-extended-templates-0.4.3/extended_templates/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)     8818 2023-02-07 18:55:03.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-code-editor.js
--rw-r--r--   0 smirolo    (501) staff       (20)    22871 2023-04-27 17:26:14.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-editor.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:05.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (501) staff       (20)    27061 2022-07-27 20:10:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-sidebar-gallery.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12248 2022-07-27 19:55:29.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-style-editor.js
--rw-r--r--   0 smirolo    (501) staff       (20)     1149 2022-09-01 18:19:11.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-themes-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)    14671 2022-07-27 20:39:43.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-upload.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.299699 djaodjin-extended-templates-0.4.3/extended_templates/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.312259 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/
--rw-r--r--   0 smirolo    (501) staff       (20)     1933 2022-07-29 20:52:36.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_bottom.html
--rw-r--r--   0 smirolo    (501) staff       (20)      105 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_bottom_edit_tools.html
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_top.html
--rw-r--r--   0 smirolo    (501) staff       (20)    12462 2022-07-29 20:55:46.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_edit_tools.html
--rw-r--r--   0 smirolo    (501) staff       (20)      682 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/edit.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1646 2022-07-29 21:12:01.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/theme.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.312592 djaodjin-extended-templates-0.4.3/extended_templates/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)      650 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templatetags/extended_templates_tags.py
--rw-r--r--   0 smirolo    (501) staff       (20)    16499 2023-02-24 17:54:24.000000 djaodjin-extended-templates-0.4.3/extended_templates/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4370 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/thread_locals.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2845 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/uploadhandler.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.312725 djaodjin-extended-templates-0.4.3/extended_templates/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1525 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.313374 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1772 2022-08-10 04:49:00.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2178 2023-01-07 00:10:20.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/assets.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1997 2023-01-07 00:09:49.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/templates.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.314214 djaodjin-extended-templates-0.4.3/extended_templates/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1478 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1683 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/views/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8083 2023-03-03 21:48:25.000000 djaodjin-extended-templates-0.4.3/extended_templates/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.315636 djaodjin-extended-templates-0.4.3/extended_templates/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-07-29 19:32:33.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/pages.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4929 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/static.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4602 2023-02-07 22:05:52.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1578 2023-07-07 13:42:34.000000 djaodjin-extended-templates-0.4.3/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-07-07 15:33:51.316130 djaodjin-extended-templates-0.4.3/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-07-07 13:42:54.000000 djaodjin-extended-templates-0.4.3/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.862730 djaodjin-extended-templates-0.4.4/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     2579 2023-08-03 00:40:43.862796 djaodjin-extended-templates-0.4.4/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1760 2023-08-03 00:24:36.000000 djaodjin-extended-templates-0.4.4/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.849459 djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2579 2023-08-03 00:40:43.000000 djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2641 2023-08-03 00:40:43.000000 djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-08-03 00:40:43.000000 djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      227 2023-08-03 00:40:43.000000 djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       19 2023-08-03 00:40:43.000000 djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/top_level.txt
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.852664 djaodjin-extended-templates-0.4.4/extended_templates/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1447 2023-08-03 00:39:47.000000 djaodjin-extended-templates-0.4.4/extended_templates/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.854494 djaodjin-extended-templates-0.4.4/extended_templates/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4265 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/less_variables.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3582 2023-02-24 18:30:59.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1976 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/sitecss.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    19365 2023-02-17 19:40:33.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/sources.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5034 2023-02-03 04:47:19.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9953 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/api/upload_media.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.855430 djaodjin-extended-templates-0.4.4/extended_templates/backends/
+-rw-r--r--   0 smirolo    (501) staff       (20)     3261 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/backends/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9469 2023-04-05 21:35:22.000000 djaodjin-extended-templates-0.4.4/extended_templates/backends/eml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9459 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/backends/pdf.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1721 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/backends/s3.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7332 2023-02-07 21:34:10.000000 djaodjin-extended-templates-0.4.4/extended_templates/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2934 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/decorators.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3188 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3058 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/extras.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3152 2023-02-08 00:52:56.000000 djaodjin-extended-templates-0.4.4/extended_templates/helpers.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.855588 djaodjin-extended-templates-0.4.4/extended_templates/management/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/management/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.855953 djaodjin-extended-templates-0.4.4/extended_templates/management/commands/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/management/commands/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2696 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/management/commands/install_theme.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3398 2023-02-13 23:22:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/management/commands/list_css_classes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6691 2023-02-07 20:38:57.000000 djaodjin-extended-templates-0.4.4/extended_templates/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3581 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10334 2022-08-23 21:36:15.000000 djaodjin-extended-templates-0.4.4/extended_templates/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1471 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.847385 djaodjin-extended-templates-0.4.4/extended_templates/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.859045 djaodjin-extended-templates-0.4.4/extended_templates/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)     8827 2023-07-29 17:25:35.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-code-editor.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    22871 2023-04-27 17:26:14.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-editor.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    52445 2023-08-03 00:12:25.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     6624 2023-08-03 00:12:25.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    27061 2022-07-27 20:10:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-sidebar-gallery.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12248 2022-07-27 19:55:29.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-style-editor.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     1149 2022-09-01 18:19:11.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-themes-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    14671 2022-07-27 20:39:43.000000 djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-upload.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.847507 djaodjin-extended-templates-0.4.4/extended_templates/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.860138 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1933 2022-07-29 20:52:36.000000 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/_body_bottom.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      105 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/_body_bottom_edit_tools.html
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/_body_top.html
+-rw-r--r--   0 smirolo    (501) staff       (20)    12364 2023-08-03 00:24:33.000000 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/_edit_tools.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      682 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/edit.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1646 2022-07-29 21:12:01.000000 djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/theme.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.860478 djaodjin-extended-templates-0.4.4/extended_templates/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      650 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/templatetags/extended_templates_tags.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    16499 2023-02-24 17:54:24.000000 djaodjin-extended-templates-0.4.4/extended_templates/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4370 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/thread_locals.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2845 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/uploadhandler.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.860623 djaodjin-extended-templates-0.4.4/extended_templates/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1525 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.861329 djaodjin-extended-templates-0.4.4/extended_templates/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1772 2022-08-10 04:49:00.000000 djaodjin-extended-templates-0.4.4/extended_templates/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2178 2023-01-07 00:10:20.000000 djaodjin-extended-templates-0.4.4/extended_templates/urls/api/assets.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1997 2023-01-07 00:09:49.000000 djaodjin-extended-templates-0.4.4/extended_templates/urls/api/templates.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.861780 djaodjin-extended-templates-0.4.4/extended_templates/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1478 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1683 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/urls/views/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8083 2023-03-03 21:48:25.000000 djaodjin-extended-templates-0.4.4/extended_templates/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-08-03 00:40:43.862495 djaodjin-extended-templates-0.4.4/extended_templates/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-07-29 19:32:33.000000 djaodjin-extended-templates-0.4.4/extended_templates/views/pages.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4929 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.4/extended_templates/views/static.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4602 2023-02-07 22:05:52.000000 djaodjin-extended-templates-0.4.4/extended_templates/views/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1578 2023-07-07 13:42:34.000000 djaodjin-extended-templates-0.4.4/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-08-03 00:40:43.863007 djaodjin-extended-templates-0.4.4/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-07-07 13:42:54.000000 djaodjin-extended-templates-0.4.4/setup.py
```

### Comparing `djaodjin-extended-templates-0.4.3/LICENSE.txt` & `djaodjin-extended-templates-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/PKG-INFO` & `djaodjin-extended-templates-0.4.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-extended-templates
-Version: 0.4.3
+Version: 0.4.4
 Summary: DjaoDjin's Template wrappers for HTML email and PDF templates
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-extended-templates
 Project-URL: documentation, https://djaodjin-extended-templates.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-extended-templates/changelog
@@ -78,14 +78,12 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.4.3
+0.4.4
 
-  * sends raw text e-mail if premail resources cannot be found
-  * compatibles with django-storages==1.13
-  * installs using pyproject.toml
+  * compatibles with Bootstrap5
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-extended-templates-0.4.3/README.md` & `djaodjin-extended-templates-0.4.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -59,14 +59,12 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.4.3
+0.4.4
 
-  * sends raw text e-mail if premail resources cannot be found
-  * compatibles with django-storages==1.13
-  * installs using pyproject.toml
+  * compatibles with Bootstrap5
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/PKG-INFO` & `djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-extended-templates
-Version: 0.4.3
+Version: 0.4.4
 Summary: DjaoDjin's Template wrappers for HTML email and PDF templates
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-extended-templates
 Project-URL: documentation, https://djaodjin-extended-templates.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-extended-templates/changelog
@@ -78,14 +78,12 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.4.3
+0.4.4
 
-  * sends raw text e-mail if premail resources cannot be found
-  * compatibles with django-storages==1.13
-  * installs using pyproject.toml
+  * compatibles with Bootstrap5
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/SOURCES.txt` & `djaodjin-extended-templates-0.4.4/djaodjin_extended_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/__init__.py` & `djaodjin-extended-templates-0.4.4/extended_templates/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the extended_templates django app.
 """
 
-__version__ = '0.4.3'
+__version__ = '0.4.4'
```

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/api/less_variables.py` & `djaodjin-extended-templates-0.4.4/extended_templates/api/less_variables.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/api/serializers.py` & `djaodjin-extended-templates-0.4.4/extended_templates/api/serializers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/api/sitecss.py` & `djaodjin-extended-templates-0.4.4/extended_templates/api/sitecss.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/api/sources.py` & `djaodjin-extended-templates-0.4.4/extended_templates/api/sources.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/api/themes.py` & `djaodjin-extended-templates-0.4.4/extended_templates/api/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/api/upload_media.py` & `djaodjin-extended-templates-0.4.4/extended_templates/api/upload_media.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/backends/__init__.py` & `djaodjin-extended-templates-0.4.4/extended_templates/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/backends/eml.py` & `djaodjin-extended-templates-0.4.4/extended_templates/backends/eml.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/backends/pdf.py` & `djaodjin-extended-templates-0.4.4/extended_templates/backends/pdf.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/backends/s3.py` & `djaodjin-extended-templates-0.4.4/extended_templates/backends/s3.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/compat.py` & `djaodjin-extended-templates-0.4.4/extended_templates/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/decorators.py` & `djaodjin-extended-templates-0.4.4/extended_templates/decorators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/docs.py` & `djaodjin-extended-templates-0.4.4/extended_templates/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/extras.py` & `djaodjin-extended-templates-0.4.4/extended_templates/extras.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/helpers.py` & `djaodjin-extended-templates-0.4.4/extended_templates/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/management/commands/install_theme.py` & `djaodjin-extended-templates-0.4.4/extended_templates/management/commands/install_theme.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/management/commands/list_css_classes.py` & `djaodjin-extended-templates-0.4.4/extended_templates/management/commands/list_css_classes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/mixins.py` & `djaodjin-extended-templates-0.4.4/extended_templates/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/models.py` & `djaodjin-extended-templates-0.4.4/extended_templates/models.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/settings.py` & `djaodjin-extended-templates-0.4.4/extended_templates/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/signals.py` & `djaodjin-extended-templates-0.4.4/extended_templates/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-code-editor.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-code-editor.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -140,15 +140,15 @@
             init: function() {
                 var self = this;
 
                 function addPanel(element, name, beforeElem) {
                     var tabsContainer = element.find("[role='tablist']");
                     var contentsContainer = element.find(".tab-content");
                     var idx = tabsContainer.find(">li").length;
-                    var tab = $("<li class=\"nav-item\"><a class=\"nav-link" + (idx === 0 ? " active" : "") + "\" href=\"#tab-" + idx + "\" data-toggle=\"tab\">" + name + "</a></li>");
+                    var tab = $("<li class=\"nav-item\"><a class=\"nav-link" + (idx === 0 ? " active" : "") + "\" href=\"#tab-" + idx + "\" data-bs-toggle=\"tab\">" + name + "</a></li>");
                     var content = $("<div id=\"tab-" + idx + "\" class=\"tab-pane" + (idx === 0 ? " active" : "") + " role=\"tabpanel\" style=\"width:100%;height:100%;\"><div class=\"content\" data-content=\"" + name + "\" style=\"width:100%;min-height:100%;\"></div></div>");
                     if (typeof beforeElem !== 'undefined') {
                         beforeElem.before(tab);
                     } else {
                         tabsContainer.append(tab);
                     }
                     contentsContainer.append(content);
@@ -165,15 +165,15 @@
                 }
                 if (templates.length > 0) {
                     self.$element.find(".tab-content .tpl-loader").remove();
                     for (var idx = 0; idx < templates.length; ++idx) {
                         addPanel(self.$element, templates[idx].name);
                     }
                 }
-                self.$element.find("[role='tablist']").append("<li id=\"new-source-btn\" class=\"nav-item\"><a class=\"nav-link\" href=\"#new-source\" data-toggle=\"modal\" data-target=\"#new-source\"><i class=\"fa fa-plus\"></i> New</a></li>");
+                self.$element.find("[role='tablist']").append("<li id=\"new-source-btn\" class=\"nav-item\"><a class=\"nav-link\" href=\"#new-source\" data-bs-toggle=\"modal\" data-bs-target=\"#new-source\"><i class=\"fa fa-plus\"></i> New</a></li>");
                 self.$element.find("#new-source-submit").click(function(event) {
                     event.preventDefault();
                     var name = self.$element.find("#new-source [name='name']").val();
                     var path = null;
                     while (name.length > 0 && name[0] === '/') {
                         name = name.substr(1);
                     }
```

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-editor.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-editor.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources-vue.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-resources-vue.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -104,31 +104,47 @@
                 var messagesElement = vm.getMessagesElement();
                 if (typeof toastr !== 'undefined' &&
                     $(toastr.options.containerId).length > 0) {
                     for (var i = 0; i < messages.length; ++i) {
                         toastr[style](messages[i]);
                     }
                 } else {
-                    var messageBlock = "<div class=\"alert alert-block";
+                    var blockStyle = "";
                     if (style) {
                         if (style === "error") {
                             style = "danger";
                         }
-                        messageBlock += " alert-" + style;
+                        blockStyle = " alert-" + style;
+                    }
+                    var messageBlock = messagesElement.find(
+                        ".alert" + blockStyle.replace(' ', '.'));
+                    if (messageBlock.length === 0) {
+                        const blockText = "<div class=\"alert" + blockStyle +
+                            " alert-dismissible fade show\">" +
+                            "<button type=\"button\" class=\"btn-close\"" +
+                            " data-bs-dismiss=\"alert\" aria-label=\"Close\">" +
+                            "</button></div>";
+                        var div = document.createElement('div');
+                        div.innerHTML = blockText;
+                        messageBlock = jQuery(div.firstChild);
+                    } else {
+                        messageBlock = jQuery(messageBlock[0].cloneNode(true));
                     }
-                    messageBlock += "\"><button type=\"button\" class=\"close\" data-dismiss=\"alert\">&times;</button>";
 
+                    // insert the actual messages
                     if (typeof messages === "string") {
                         messages = [messages];
                     }
                     for (var i = 0; i < messages.length; ++i) {
-                        messageBlock += "<div>" + messages[i] + "</div>";
+                        messageBlock.append("<div>" + messages[i] + "</div>");
                     }
-                    messageBlock += "</div>";
-                    vm.getMessagesElement().append(messageBlock);
+                    if (messageBlock.css('display') === 'none') {
+                        messageBlock.css('display', 'block');
+                    }
+                    messagesElement.append(messageBlock);
                 }
                 var messagesContainer = messagesElement.parent();
                 if (messagesContainer && messagesContainer.hasClass("hidden")) {
                     messagesContainer.removeClass("hidden");
                 }
                 if (vm.scrollToTopOnMessages) {
                     jQuery("html, body").animate({
@@ -936,19 +952,21 @@
                 vm.mergeResults = false;
             },
             handleScroll: function(evt) {
                 var vm = this;
                 let element = this.$el;
                 if (element.getBoundingClientRect().bottom < window.innerHeight) {
                     let menubar = vm.$el.querySelector('[role="pagination"]');
-                    var style = window.getComputedStyle(menubar);
-                    if (style.display == 'none') {
-                        // We are not displaying the pagination menubar,
-                        // so let's scroll!
-                        vm.paginationHandler();
+                    if (menubar) {
+                        var style = window.getComputedStyle(menubar);
+                        if (style.display == 'none') {
+                            // We are not displaying the pagination menubar,
+                            // so let's scroll!
+                            vm.paginationHandler();
+                        }
                     }
                 }
             },
             paginationHandler: function($state) {
                 var vm = this;
                 if (!vm.itemsLoaded || vm.mergeResults) {
                     // this handler is triggered on initial get() too.
```

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-resources.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -28,31 +28,48 @@
         if (typeof toastr !== 'undefined' &&
             jQuery(toastr.options.containerId).length > 0) {
             for (var i = 0; i < messages.length; ++i) {
                 toastr[style](messages[i]);
             }
 
         } else {
-            var messageBlock = "<div class=\"alert alert-block";
+            var messagesElement = jQuery("#messages-content");
+            var blockStyle = "";
             if (style) {
                 if (style === "error") {
                     style = "danger";
                 }
-                messageBlock += " alert-" + style;
+                blockStyle = " alert-" + style;
+            }
+            var messageBlock = messagesElement.find(
+                ".alert" + blockStyle.replace(' ', '.'));
+            if (messageBlock.length === 0) {
+                const blockText = "<div class=\"alert" + blockStyle +
+                    " alert-dismissible fade show\">" +
+                    "<button type=\"button\" class=\"btn-close\"" +
+                    " data-bs-dismiss=\"alert\" aria-label=\"Close\">" +
+                    "</button></div>";
+                var div = document.createElement('div');
+                div.innerHTML = blockText;
+                messageBlock = jQuery(div.firstChild);
+            } else {
+                messageBlock = jQuery(messageBlock[0].cloneNode(true));
             }
-            messageBlock += "\"><button type=\"button\" class=\"close\" data-dismiss=\"alert\">&times;</button>";
 
+            // insert the actual messages
             if (typeof messages === "string") {
                 messages = [messages];
             }
             for (var i = 0; i < messages.length; ++i) {
-                messageBlock += "<div>" + messages[i] + "</div>";
+                messageBlock.append("<div>" + messages[i] + "</div>");
+            }
+            if (messageBlock.css('display') === 'none') {
+                messageBlock.css('display', 'block');
             }
-            messageBlock += "</div>";
-            jQuery("#messages-content").append(messageBlock);
+            messagesElement.append(messageBlock);
         }
         jQuery("#messages").removeClass("hidden");
         jQuery("html, body").animate({
             // scrollTop: jQuery("#messages").offset().top - 50
             // avoid weird animation when messages at the top:
             scrollTop: jQuery("body").offset().top
         }, 500);
```

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-sidebar-gallery.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-sidebar-gallery.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-style-editor.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-style-editor.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-themes-vue.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-themes-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-upload.js` & `djaodjin-extended-templates-0.4.4/extended_templates/static/js/djaodjin-upload.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_bottom.html` & `djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/_body_bottom.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_edit_tools.html` & `djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/_edit_tools.html`

 * *Files 5% similar despite different names*

```diff
@@ -279,19 +279,19 @@
   });
 });
   </script>
 </div>
 
 <!-- Buttons to open/close the sliding edit panels -->
 <div style="top:200px;position:fixed;right:-1px;z-index:10000" class="btn-group-vertical btn-group-sm btn-tools" role="group" aria-label="...">
-  <button class="btn btn-primary" style="opacity:0.9;" id="toggle-media-gallery" data-target="#media-gallery" data-default-width="300" data-intro="Image gallery" data-position="left" title="Image Gallery"><i class="glyphicon glyphicon-film"></i></button>
+  <button class="btn btn-primary" style="opacity:0.9;" id="toggle-media-gallery" data-target="#media-gallery" data-default-width="300" data-intro="Image gallery" data-position="left" title="Image Gallery"><i>G</i></button>
 </div>
 <div style="top:230px;position:fixed;right:-1px;z-index:10000" class="btn-group-vertical btn-group-sm btn-tools" role="group" aria-label="...">
-  <button id="toggle-code-editor" class="btn btn-primary" style="opacity:0.9;" data-target="#code-editor" data-default-width="800" data-intro="Code Editor" data-position="left" title="Code"><i class="glyphicon glyphicon-edit"></i></button>
-  <button id="toggle-style-editor" class="btn btn-primary" style="opacity:0.9;" data-target="#style-editor" data-default-width="800" data-intro="Style Editor" data-position="left" title="Styles"><i class="glyphicon glyphicon-italic"></i></button>
+  <button id="toggle-code-editor" class="btn btn-primary" style="opacity:0.9;" data-target="#code-editor" data-default-width="800" data-intro="Code Editor" data-position="left" title="Code"><i>C</i></button>
+  <button id="toggle-style-editor" class="btn btn-primary" style="opacity:0.9;" data-target="#style-editor" data-default-width="800" data-intro="Style Editor" data-position="left" title="Styles"><i>S</i></button>
 <script type="text/javascript">
 jQuery(document).ready(function($) {
     if( window.location !== window.top.location ) {
         $(".btn-tools").hide();
     } else {
         $(".btn-tools .btn").panelButton();
         $(".btn-tools .btn").click(function(){
```

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/edit.html` & `djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/edit.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/theme.html` & `djaodjin-extended-templates-0.4.4/extended_templates/templates/extended_templates/theme.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/templatetags/extended_templates_tags.py` & `djaodjin-extended-templates-0.4.4/extended_templates/templatetags/extended_templates_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/themes.py` & `djaodjin-extended-templates-0.4.4/extended_templates/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/thread_locals.py` & `djaodjin-extended-templates-0.4.4/extended_templates/thread_locals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/uploadhandler.py` & `djaodjin-extended-templates-0.4.4/extended_templates/uploadhandler.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/urls/__init__.py` & `djaodjin-extended-templates-0.4.4/extended_templates/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/urls/api/__init__.py` & `djaodjin-extended-templates-0.4.4/extended_templates/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/urls/api/assets.py` & `djaodjin-extended-templates-0.4.4/extended_templates/urls/api/assets.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/urls/api/templates.py` & `djaodjin-extended-templates-0.4.4/extended_templates/urls/api/templates.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/urls/views/__init__.py` & `djaodjin-extended-templates-0.4.4/extended_templates/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/urls/views/themes.py` & `djaodjin-extended-templates-0.4.4/extended_templates/urls/views/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/utils.py` & `djaodjin-extended-templates-0.4.4/extended_templates/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/views/pages.py` & `djaodjin-extended-templates-0.4.4/extended_templates/views/pages.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/views/static.py` & `djaodjin-extended-templates-0.4.4/extended_templates/views/static.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/extended_templates/views/themes.py` & `djaodjin-extended-templates-0.4.4/extended_templates/views/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/pyproject.toml` & `djaodjin-extended-templates-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.3/setup.py` & `djaodjin-extended-templates-0.4.4/setup.py`

 * *Files identical despite different names*

