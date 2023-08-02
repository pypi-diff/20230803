# Comparing `tmp/django-sphinx-hosting-1.2.2.tar.gz` & `tmp/django-sphinx-hosting-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.2.2.tar", last modified: Tue Aug  1 22:00:58 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.2.3.tar", last modified: Wed Aug  2 22:50:52 2023, max compression
```

## Comparing `django-sphinx-hosting-1.2.2.tar` & `django-sphinx-hosting-1.2.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.219938 django-sphinx-hosting-1.2.2/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.2.2/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.2.2/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-08-01 22:00:58.220160 django-sphinx-hosting-1.2.2/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.2.2/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.172030 django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-08-01 22:00:58.000000 django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2947 2023-08-01 22:00:58.000000 django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-08-01 22:00:58.000000 django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-08-01 22:00:58.000000 django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-08-01 22:00:58.000000 django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1281 2023-08-01 22:00:58.221728 django-sphinx-hosting-1.2.2/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-08-01 22:00:35.000000 django-sphinx-hosting-1.2.2/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.185201 django-sphinx-hosting-1.2.2/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-08-01 22:00:35.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.189505 django-sphinx-hosting-1.2.2/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/api/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1122 2023-07-31 22:42:09.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/api/permissions.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    13981 2023-07-31 19:04:28.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/exc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/fields.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.190175 django-sphinx-hosting-1.2.2/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/fixtures/classifiers.json
--rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/form_fields.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    24175 2023-07-31 22:51:10.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.191017 django-sphinx-hosting-1.2.2/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.194403 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/fix_broken_hrefs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.204916 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0011_machinenamefield.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0012_project_relatedlinks.py
--rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/search_indexes.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/signals.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.164816 django-sphinx-hosting-1.2.2/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.165127 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.208792 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.209465 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.165884 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.165565 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.165689 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.210441 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.210995 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/templates/sphinx_hosting/base.html
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.211842 django-sphinx-hosting-1.2.2/sphinx_hosting/templatetags/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/templatetags/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/templatetags/sphinx_hosting.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    26582 2023-07-31 19:00:50.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.217843 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-01 22:00:58.219668 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    18051 2023-07-27 20:11:32.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.253510 django-sphinx-hosting-1.2.3/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.2.3/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.2.3/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-08-02 22:50:52.253738 django-sphinx-hosting-1.2.3/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.2.3/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.162234 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2947 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-08-02 22:50:52.000000 django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1281 2023-08-02 22:50:52.255389 django-sphinx-hosting-1.2.3/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-08-02 22:46:23.000000 django-sphinx-hosting-1.2.3/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.177356 django-sphinx-hosting-1.2.3/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-08-02 22:46:23.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.184586 django-sphinx-hosting-1.2.3/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1122 2023-07-31 22:42:09.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/permissions.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    13981 2023-07-31 19:04:28.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.189556 django-sphinx-hosting-1.2.3/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/fixtures/classifiers.json
+-rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    24175 2023-07-31 22:51:10.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.193230 django-sphinx-hosting-1.2.3/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.204980 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/fix_broken_hrefs.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.228230 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0012_project_relatedlinks.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/search_indexes.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.155223 django-sphinx-hosting-1.2.3/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.155734 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.236200 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.237204 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.156545 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.156215 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.156340 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.241128 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.242638 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templates/sphinx_hosting/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.243916 django-sphinx-hosting-1.2.3/sphinx_hosting/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templatetags/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/templatetags/sphinx_hosting.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    26582 2023-07-31 19:00:50.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.251230 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-08-02 22:50:52.253008 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    19342 2023-08-02 17:26:20.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.2.2/LICENSE.txt` & `django-sphinx-hosting-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/PKG-INFO` & `django-sphinx-hosting-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.2.2
+Version: 1.2.3
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.2.2/README.md` & `django-sphinx-hosting-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.2.2
+Version: 1.2.3
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.2.2/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.2.3/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/setup.cfg` & `django-sphinx-hosting-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/setup.py` & `django-sphinx-hosting-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.2.2",
+    version="1.2.3",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
```

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/api/permissions.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/fields.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/fields.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.2.3/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/forms.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/importers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/fix_broken_hrefs.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/fix_broken_hrefs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0011_machinenamefield.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0011_machinenamefield.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0012_project_relatedlinks.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0012_project_relatedlinks.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/models.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/models.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/signals.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/signals.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.2.3/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.2.3/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/validators.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/views.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/navigation.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,22 +163,35 @@
             header_text="Versions",
             badge_text=Project.objects.get(pk=self.project_id).versions.count(),
         )
         return header
 
 
 class ProjectClassifierSelectorWidget(ToggleableManyToManyFieldBlock):
+    """
+    This is an editable listing of :py:class:`sphinx_hosting.models.Classifier`
+    objects for a particular :py:class:`sphinx_hosting.models.Project`.
+
+    It is used in the project edit view.
+    """
 
     model = Project
     field_name = 'classifiers'
     title = 'Classifiers'
     icon = 'collection'
 
 
 class ProjectClassifierListWidget(ListModelWidget):
+    """
+    This is a :py:class:`wildewidgets.ListModelWidget` that renders a list of
+    :py:class:`sphinx_hosting.models.Classifier` objects.  It is used in the
+    project detail view as a read-only list of classifiers.
+
+    The editable version of this widget is :py:class:`ProjectClassifierSelectorWidget`.
+    """
 
     paginate_by: int = 100
     item_label: str = 'Classifier'
     title = 'Classifiers'
     icon = 'collection'
 
     def get_object_text(self, instance: Classifier) -> str:
@@ -189,15 +202,16 @@
 
 
 class ProjectDetailWidget(
     CrispyFormWidget,
     Widget
 ):
     """
-    This widget renders an update form for a :py:class:`sphinx_hosting.models.Project`.
+    This widget renders an update form for a
+    :py:class:`sphinx_hosting.models.Project`.
 
     Use directly it like so::
 
         >>> project = Project.objects.get(pk=1)
         >>> form = ProjectUpdateForm(instance=project)
         >>> widget = ProjectDetailWidget(form=form)
 
@@ -212,14 +226,20 @@
 
 
 #------------------------------------------------------
 # ProjectRelatedLink related widgets
 #------------------------------------------------------
 
 class ProjectRelatedLinkListItemWidget(HorizontalLayoutBlock):
+    """
+    This is used by :py:class:`ProjectRelatedLinksWidget` to render a single
+    :py:class:`sphinx_hosting.models.ProjectRelatedLink` object in its list.
+    """
+
+    css_class: str = "mb-2"
 
     def __init__(self, object: ProjectRelatedLink):  # pylint: disable=redefined-builtin
         modal_id = f"projectrelatedlink__update__{object.pk}"
         super().__init__(
             Link(object.title, url=object.uri, title=object.title),
             Block(
                 ModalButton(text='Edit', color="azure", target=f'#{modal_id}'),
@@ -236,14 +256,20 @@
 
 
 class ProjectRelatedLinksWidget(CardWidget):
     """
     This is a :py:class:`wildewidgets.CardWidget` that allows us to
     manage the :py:class:`sphinx_hosting.models.ProjectRelatedLink` objects
     for this :py:class:`sphinx_hosting.models.Project`.
+
+    It renders a list of :py:class:`ProjectRelatedLinkListItemWidget` objects
+    and a "Add Related Link" button that opens a modal dialog.
+
+    This is used on the project update page, and is the editable version of
+    :py:class:`ProjectRelatedLinksListWidget`.
     """
 
     title: str = "Related Links"
     icon: str = "box-arrow-up-right"
 
     def __init__(self, project: Project, **kwargs):
         self.project = project
@@ -265,14 +291,22 @@
             color="primary",
             target=f'#{ProjectRelatedLinkCreateModalWidget.modal_id}'
         )
         return header
 
 
 class ProjectRelatedLinksListWidget(ListModelWidget):
+    """
+    This widget renders a list of
+    :py:class:`sphinx_hosting.models.ProjectRelatedLink` objects as a list of
+    :py:class:`wildewidgets.Link` objects.
+
+    This is used on the project detail page, and is the read-only version of
+    :py:class:`ProjectRelatedLinksWidget`.
+    """
 
     paginate_by: int = 100
     item_label: str = 'Related Link'
     title: str = 'Related Links'
     icon: str = "external-link"
 
     def get_model_subblock(self, instance: ProjectRelatedLink) -> Block:
```

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.2/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.2.3/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

