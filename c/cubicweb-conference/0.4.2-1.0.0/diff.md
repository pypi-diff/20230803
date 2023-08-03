# Comparing `tmp/cubicweb-conference-0.4.2.tar.gz` & `tmp/cubicweb-conference-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-conference-0.4.2.tar", last modified: Mon Apr 26 16:49:46 2010, max compression, from Unix
+gzip compressed data, was "cubicweb-conference-1.0.0.tar", last modified: Thu Aug  3 09:51:34 2023, max compression
```

## Comparing `cubicweb-conference-0.4.2.tar` & `cubicweb-conference-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,96 @@
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/
--rw-rw-r--   0 syt       (1004) syt       (1004)      265 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/site_cubicweb.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     2641 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/entities.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     5782 2010-04-26 13:00:06.000000 cubicweb-conference-0.4.2/setup.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      568 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/xy.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/i18n/
--rw-rw-r--   0 syt       (1004) syt       (1004)    14898 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/i18n/fr.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     9469 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/i18n/es.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     9803 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/i18n/en.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     1887 2010-04-26 13:22:41.000000 cubicweb-conference-0.4.2/__pkginfo__.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      458 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/PKG-INFO
--rw-rw-r--   0 syt       (1004) syt       (1004)      367 2009-10-19 08:57:05.000000 cubicweb-conference-0.4.2/MANIFEST.in
--rw-rw-r--   0 syt       (1004) syt       (1004)       26 2009-10-19 08:57:05.000000 cubicweb-conference-0.4.2/__init__.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/views/
--rw-rw-r--   0 syt       (1004) syt       (1004)     1504 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/views/stats.py
--rw-rw-r--   0 syt       (1004) syt       (1004)    10024 2010-04-26 13:00:06.000000 cubicweb-conference-0.4.2/views/primary.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1998 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/actions.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     2861 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/semantic.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1262 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/facets.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1050 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/startup.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      300 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/formrenderers.py
--rw-rw-r--   0 syt       (1004) syt       (1004)        0 2009-10-19 08:57:05.000000 cubicweb-conference-0.4.2/views/sections.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      642 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/forms.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1379 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/views/__init__.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     3992 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/views/boxes.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     4847 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/views/workflow.py
--rw-rw-r--   0 syt       (1004) syt       (1004)    13991 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/views/secondaries.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     6294 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/sobjects.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      156 2010-04-26 13:00:06.000000 cubicweb-conference-0.4.2/README
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/test/
--rw-rw-r--   0 syt       (1004) syt       (1004)     5303 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/test/unittest_notifications.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1148 2008-10-28 14:33:57.000000 cubicweb-conference-0.4.2/test/pytestconf.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      281 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/test/test_conference.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1106 2008-10-28 14:33:57.000000 cubicweb-conference-0.4.2/test/realdb_test_conference.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/data/
--rw-rw-r--   0 syt       (1004) syt       (1004)     2797 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/data/cubes.conference.css
--rw-rw-r--   0 syt       (1004) syt       (1004)     1166 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/data/stat.png
--rw-rw-r--   0 syt       (1004) syt       (1004)      560 2009-10-19 08:57:05.000000 cubicweb-conference-0.4.2/data/noattend.jpeg
--rw-rw-r--   0 syt       (1004) syt       (1004)      543 2009-08-25 10:49:34.000000 cubicweb-conference-0.4.2/data/external_resources
--rw-rw-r--   0 syt       (1004) syt       (1004)       45 2008-12-17 10:59:05.000000 cubicweb-conference-0.4.2/data/cubes.conference.js
--rw-rw-r--   0 syt       (1004) syt       (1004)     2889 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/data/icon_pen.gif
--rw-rw-r--   0 syt       (1004) syt       (1004)      525 2009-10-19 08:57:05.000000 cubicweb-conference-0.4.2/data/attend.jpeg
--rw-rw-r--   0 syt       (1004) syt       (1004)     5635 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/schema.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/wdoc/
--rw-rw-r--   0 syt       (1004) syt       (1004)      237 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/wdoc/ChangeLog_fr
--rw-rw-r--   0 syt       (1004) syt       (1004)      189 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/wdoc/ChangeLog_en
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/migration/
--rw-rw-r--   0 syt       (1004) syt       (1004)       29 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/migration/0.2.0_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1064 2010-04-26 13:00:02.000000 cubicweb-conference-0.4.2/migration/0.4.0_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1952 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/migration/postcreate.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1903 2010-03-08 11:30:49.000000 cubicweb-conference-0.4.2/migration/0.3.0_Any.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/cubicweb_conference.egg-info/
--rw-rw-r--   0 syt       (1004) syt       (1004)      111 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/cubicweb_conference.egg-info/requires.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)       11 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/cubicweb_conference.egg-info/top_level.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)        1 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/cubicweb_conference.egg-info/dependency_links.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)     1347 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/cubicweb_conference.egg-info/SOURCES.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)      458 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/cubicweb_conference.egg-info/PKG-INFO
--rw-rw-r--   0 syt       (1004) syt       (1004)       59 2010-04-26 16:49:46.000000 cubicweb-conference-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      615 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.686243 cubicweb-conference-1.0.0/cubicweb_conference/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.690243 cubicweb-conference-1.0.0/cubicweb_conference/data/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/attend.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/cubes.conference.css
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/cubes.conference.js
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/icon_pen.gif
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/noattend.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/stat.png
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/ticket-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     9777 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/ticket-icon.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4749 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.694243 cubicweb-conference-1.0.0/cubicweb_conference/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    12221 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    12700 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)    12220 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    17790 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.698243 cubicweb-conference-1.0.0/cubicweb_conference/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.10.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.10.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.13.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.3.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.4.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.5.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.6.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.7.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.8.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.9.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.9.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10014 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.702243 cubicweb-conference-1.0.0/cubicweb_conference/views/
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7631 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9770 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/calendarview.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/components.py
+-rw-rw-rw-   0 root         (0) root         (0)     6877 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/conference.py
+-rw-rw-rw-   0 root         (0) root         (0)      964 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3352 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/semantic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/talk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/track.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.690243 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      615 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      226 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.710243 cubicweb-conference-1.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.710243 cubicweb-conference-1.0.0/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/test/data/acceptance/
+-rw-rw-rw-   0 root         (0) root         (0)    14953 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/BBQ_logo_3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    10221 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/ELE_logo_1.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    12589 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Pell_logo_3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    98005 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Programme_SemWebPro2010.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Shell_logo_1.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     7541 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Untel_logo_2.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8210 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/novia_logo_2.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     9017 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/orange_logo_3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    15382 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/demo_conference.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/review-process.txt
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/test_acceptance.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/test_conference.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4563 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     5465 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7005 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/wdoc/ChangeLog_fr
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-conference-0.4.2/entities.py` & `cubicweb-conference-1.0.0/cubicweb_conference/views/forms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,93 @@
-"""this contains the template-specific entities' classes"""
+from cubicweb.predicates import is_instance, match_user_groups
+from cubicweb_web.views import autoform
 
-__docformat__ = "restructuredtext en"
+# vocabulary for add / talk form
 
-from logilab.common.date import todate
 
-from cubicweb.mixins import TreeMixIn
-from cubicweb.entities import AnyEntity
-from cubicweb.interfaces import ITree, ICalendarable
-
-class Conference(TreeMixIn, AnyEntity):
-    """customized class for Conference entities"""
-    __regid__ = 'Conference'
-    __implements__ = AnyEntity.__implements__ + (ITree,)
-
-    tree_attribute = 'in_conf'
-
-    def children(self, entities=True):
-        """
-        Return children entities.
-        Overriden to get only Track entities.
-        """
-        return self.different_type_children(entities)
-
-    def dates(self):
-        return (self.start_on, self.end_on)
-
-    def breadcrumbs(self, view=None, recurs=False):
-        return [(self.absolute_url(), self.dc_title()),]
-
-    def get_talks_by_track(self, track):
-        rql = 'Any T WHERE T in_track TR, TR eid %(tr)s'
-        return self._cw.execute(rql, {'tr': track.eid})
-
-    def has_talk(self, day, track):
-        for talk in self.get_talks_by_track(track).entities():
-            if talk.is_on_day(day):
-                return True
-        return False
-
-class Track(TreeMixIn, AnyEntity):
-    """customized class for Track entities"""
-    __regid__ = 'Track'
-    __implements__ = AnyEntity.__implements__ + (ITree,)
-
-    tree_attribute = 'in_track'
-
-    def children(self, entities=True):
-        """
-        Return children entities.
-        Overriden to get only Talk entities.
-        """
-        return self.different_type_children(entities)
-
-    def dates(self):
-        return
-
-    def breadcrumbs(self, view=None, recurs=False):
-        try:
-            breadcrumbs = self.in_conf[0].breadcrumbs(view, True)
-        except IndexError:
-            breadcrumbs = []
-        breadcrumbs += [(self.absolute_url(), self.dc_title()), ]
-        return breadcrumbs
-
-class Talk(AnyEntity):
-    __regid__ = 'Talk'
-    __implements__ = AnyEntity.__implements__ + (ICalendarable,)
-
-    def breadcrumbs(self, view=None, recurs=False):
-        try:
-            breadcrumbs = self.in_track[0].breadcrumbs(view, True)
-        except IndexError:
-            breadcrumbs = []
-        breadcrumbs += [(self.absolute_url(), self.dc_title()), ]
-        return breadcrumbs
-
-    @property
-    def start(self):
-        return self.start_time
-
-    @property
-    def stop(self):
-        return self.end_time
-
-    def is_on_day(self, day):
-        date = todate(day)
-        if self.start_time:
-            talk_date = todate(self.start_time)
-            return date == talk_date
-        else:
-            return False
+def reviewers_vocabulary(form, field):
+    entity = form.edited_entity
+    rset = form._cw.execute(
+        "Any U WHERE U is_reviewer_at C, X in_conf C, " "X is Talk, X eid %(x)s",
+        {"x": entity.eid},
+    )
+    return [(item.dc_long_title(), item.eid) for item in rset.entities()]
+
+
+def subject_call_open_conf_vocabulary(form, field):
+    options = []
+    edited_entity = form.edited_entity
+    if edited_entity.has_eid() and edited_entity.in_conf:
+        conf = edited_entity.in_conf[0]
+        options = [(conf.dc_title(), conf.eid)]
+    if form._cw.user.matching_groups("managers"):
+        rset = form._cw.execute("Any C WHERE C is Conference")
+    else:
+        rset = form._cw.execute(
+            "Any C WHERE C is Conference, C call_open True, "
+            'C in_state S, S name "scheduled"'
+        )
+    for entity in rset.entities():
+        if edited_entity.has_eid() and conf.eid == entity.eid:
+            continue
+        options.append((entity.dc_title(), entity.eid))
+    return options
+
+
+def subject_reg_open_conf_vocabulary(form, field):
+    options = []
+    edited_entity = form.edited_entity
+    if edited_entity.has_eid() and edited_entity.book_conf:
+        conf = edited_entity.book_conf[0]
+        options = [(conf.dc_title(), conf.eid)]
+    if form._cw.user.matching_groups("managers"):
+        rset = form._cw.execute("Any C WHERE C is Conference")
+    else:
+        rset = form._cw.execute(
+            "Any C WHERE C is Conference, C reg_open True, "
+            'C in_state S, S name "scheduled"'
+        )
+    for entity in rset.entities():
+        if edited_entity.has_eid() and conf.eid == entity.eid:
+            continue
+        options.append((entity.dc_title(), entity.eid))
+    return options
+
+
+def subject_in_track_vocabulary(form, field):
+    options = []
+    edited_entity = form.edited_entity
+    if edited_entity.has_eid() and edited_entity.in_track:
+        track = edited_entity.in_track[0]
+        options = [(track.dc_title(), track.eid)]
+    if form._cw.user.matching_groups("managers"):
+        rset = form._cw.execute("Any T WHERE T is Track")
+    else:
+        rset = form._cw.execute(
+            "DISTINCT Any T WHERE T is Track, T in_conf C, "
+            'C call_open True, C in_state S, S name "scheduled"'
+        )
+    for entity in rset.entities():
+        if edited_entity.has_eid() and track.eid == entity.eid:
+            continue
+        options.append((entity.dc_title(), entity.eid))
+    return options
+
+
+class TalkAutoForm(autoform.AutomaticEntityForm):
+    __select__ = (
+        autoform.AutomaticEntityForm.__select__
+        & is_instance("Talk")
+        & match_user_groups("managers")
+    )
+
+    def editable_relations(self):
+        result = super().editable_relations()
+        rschema = self._cw.vreg.schema.rschema("leads")
+        result.append(
+            (
+                rschema.display_name(self.edited_entity._cw, "object", "Talk"),
+                rschema,
+                "object",
+            )
+        )
+        return sorted(result)
```

### Comparing `cubicweb-conference-0.4.2/i18n/fr.po` & `cubicweb-conference-1.0.0/cubicweb_conference/i18n/fr.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,56 @@
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR Free Software Foundation, Inc.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: 2.0\n"
 "POT-Creation-Date: 2006-01-12 17:35+CET\n"
-"PO-Revision-Date: 2010-03-23 17:03+0100\n"
+"PO-Revision-Date: 2010-06-24 20:03+0200\n"
 "Last-Translator: Logilab\n"
-"Language-Team: French <devel@logilab.fr.org>\n"
+"Language-Team: French <cubicweb@lists.cubicweb.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Abstract"
 msgstr "Résumé"
 
-msgid "Abstract submission is open !"
-msgstr "Appel à soumission"
+msgid "Answer the call for talks !"
+msgstr "Répondez à l'appel à communication !"
 
 msgid "At the same time"
 msgstr "Au même moment"
 
 msgid "Attachments"
 msgstr "Pièces jointes"
 
+msgid "Authentication is needed to perform this action"
+msgstr "Vous devez vous authentifier pour exécuter cette action"
+
+msgid "Begin"
+msgstr "Début"
+
 msgid "Call for paper"
-msgstr "Appel à soumission"
+msgstr "Appel à communication"
 
 # schema pot file, generated on 2009-09-02 11:27:38
 #
 # singular and plural forms for each entity type
 msgid "Conference"
 msgstr "Conférence"
 
 msgid "Conference_plural"
 msgstr "Conférences"
 
 msgid "Date"
-msgstr ""
+msgstr "Date"
 
 #, python-format
 msgid ""
 "Dear %(firstname)s %(lastname)s,\n"
 "\n"
 "The talk '%(talk_name)s' was added on %(date)s.\n"
 "\n"
@@ -72,45 +82,54 @@
 "Sincerely,\n"
 "\n"
 "--\n"
 "The conference organizing committee.\n"
 msgstr ""
 
 msgid "Description"
-msgstr ""
+msgstr "Description"
 
 msgid ""
-"Do you plan to attend a specific talk ? Please click on the \"I plan to "
-"attend\" button positionned at the top right of each talk summary."
+"Do you plan to attend a specific talk ? Please click on the attendancy "
+"button positionned at the top right of each talk summary."
+msgstr ""
+"Prévoyez-vous d'assister à certaines présentations en particulier ? Cliquez "
+"sur le bouton que vous trouverez en haut à droite sur chaque page de "
+"présentation."
+
+msgid "End"
+msgstr "Fin"
+
+msgctxt "inlined:Sponsor.has_logo.subject"
+msgid "File"
 msgstr ""
 
 msgid "First talk"
 msgstr "Première présentation"
 
-msgid "I do not plan to attend"
-msgstr "Je n'y assiste pas"
+msgid "Generate badges"
+msgstr "Générer les badges"
 
-msgid "I plan to attend"
-msgstr "Je vais y assister"
+msgid "If you already have an account, please log in"
+msgstr "Si vous avez déjà en compte, veuillez vous connecter"
 
 msgid "If you are interested in sponsoring or partnering"
-msgstr ""
+msgstr "Si vous souhaitez sponsoriser cette conférence ou en être partenaire"
 
-msgctxt "inlined:Sponsor.has_logo.subject"
-msgid "Image"
-msgstr ""
+msgid "If you do not have an account yet, please create one"
+msgstr "Si vous n'avez pas encore de compte, veuillez en créer un"
 
 msgid "Index"
 msgstr ""
 
 msgid "Last talk"
 msgstr "Dernière présentation"
 
 msgid "Location"
-msgstr "Lieu"
+msgstr "Salle"
 
 msgid "New Conference"
 msgstr "Nouvelle conférence"
 
 msgid "New Sponsor"
 msgstr "Nouveau sponsor"
 
@@ -119,35 +138,48 @@
 
 msgid "New Talk"
 msgstr "Nouvelle présentation"
 
 msgid "New Track"
 msgstr "Nouvelle session"
 
+msgid "No accepted talk yet in this conference"
+msgstr ""
+"Aucune présentation n'a pour le moment été acceptée pour cette conférence."
+
+msgid "No accepted talk yet in this track"
+msgstr ""
+"Aucune présentation n'a pour le moment été acceptée pour cette session."
+
 msgid "No conference planned for now..."
 msgstr "Pas de conférence de prévue pour le moment..."
 
-msgid "No talk yet in this conference"
-msgstr "Aucune présentation dans la conférence à ce jour"
-
 msgid "No track yet in this conference."
 msgstr "Pas encore de session définie pour cette conférence"
 
 msgid "Number of participant by Talk"
 msgstr "Nombre de participants par présentation"
 
 msgid "Past conferences"
 msgstr "Conférences précédentes"
 
 msgid "Please, assign a reviewer to :"
 msgstr "Merci d'assigner un relecteur à :"
 
+msgctxt "inlined:Conference.take_place_at.subject"
+msgid "PostalAddress"
+msgstr ""
+
 msgid "Presented by"
 msgstr "Présenté par"
 
+msgid "Remember you have already submitted a talk."
+msgstr ""
+"Rappelez-vous que vous avez déjà déposé une proposition de présentation."
+
 msgid "Representing"
 msgstr "Représentant"
 
 msgid "Speaker"
 msgstr "Conférencier"
 
 msgid "Sponsor"
@@ -164,35 +196,30 @@
 
 msgid "Talk"
 msgstr "Présentation"
 
 msgid "Talk state details"
 msgstr "Statut de la présentation"
 
-msgid "Talk submission informations"
-msgstr ""
-
 msgid "Talk title"
 msgstr "Titre de la présentation"
 
 msgid "Talk_plural"
 msgstr "Présentations"
 
+#, python-format
+msgid "Talks you have to review (in state %s)"
+msgstr "Les propositions de présentation que vous devez juger (dans l'état %s)"
+
 msgid "The conference was divided into the following tracks:"
 msgstr "La conférence était composée des sessions suivantes:"
 
 msgid "The conference will be divided into the following tracks:"
 msgstr "La conférence sera composée des sessions suivantes:"
 
-msgid "The following talks were presented:"
-msgstr "Le programme des présentations était:"
-
-msgid "The following talks will be presented:"
-msgstr "Le programme des présentations sera:"
-
 msgid "This Conference"
 msgstr "Cette conférence"
 
 msgid "This Sponsor"
 msgstr "Ce sponsor"
 
 msgid "This SponsorShip"
@@ -200,14 +227,54 @@
 
 msgid "This Talk"
 msgstr "Cette présentation"
 
 msgid "This Track"
 msgstr "Cette session"
 
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means it needs to be submitted before it "
+"can be considered by the reviewers."
+msgstr ""
+"Cette présentation est dans l'état \"%s\", ce qui veut dire qu'elle doit "
+"être soumise avant de pouvoir être prise en compte par les rapporteurs."
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means the author needs to answer the "
+"comments of the reviewers."
+msgstr ""
+"Cette présentation est dans l'état \"%s\", ce qui veut dire que l'auteur "
+"doit répondre aux commentaires des rapporteurs."
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means the reviewers will soon send you "
+"their comments."
+msgstr ""
+"Cette présentation est dans l'état \"%s\", ce qui veut dire que les "
+"rapporteurs vont bientôt vous envoyer leurs commentaires."
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means you have to review it. You can ask "
+"the author for modifications, accept or reject this talk."
+msgstr ""
+"Cette présentation est dans l'état \"%s\", ce qui veut dire que vous devez "
+"l'évaluer. Vous pouvez demander à l'auteur des modifications, l'accepter ou "
+"la rejeter."
+
+msgid ""
+"This talk was reviewed and is now awaiting a final decision by the "
+"conference chairs."
+msgstr ""
+"Cette proposition a été traitée par les rapporteurs et attend la décision "
+"finale des organisateurs."
+
 msgid "Total talks"
 msgstr "Total présentations"
 
 msgid "Track"
 msgstr "Session"
 
 msgid "Track title"
@@ -215,60 +282,80 @@
 
 msgid "Track_plural"
 msgstr "Sessions"
 
 msgid "Upcoming conferences"
 msgstr "Conférences à venir"
 
-msgid "View statistics"
-msgstr "Voir les statistiques"
+msgid "You are planning to attend these talks:"
+msgstr "Vous prévoyez d'assister à ces présentations:"
+
+msgid "You can select a new logo, else the site's logo will be taken"
+msgstr ""
+
+msgid "You do not plan to attend"
+msgstr "Vous ne comptez pas y assister."
 
-msgid "Workflow history"
-msgstr "historique"
+msgid ""
+"You need to create an account and sign in before you can submit an abstract"
+msgstr ""
+"Vous devez créer un compte et vous authentifier avant de pouvoir\n"
+"soumettre une proposition de communication."
 
-msgid "You are registered for these talks:"
-msgstr "Vous êtes inscrit à ces présentations:"
+msgid "You plan to attend"
+msgstr "Vous comptez y assister."
+
+#, python-format
+msgid "Your talks in state %s"
+msgstr "Vos présentations dans l'état %s"
 
 #, python-format
-msgid "[%s] a talk was added."
+msgid "[%s] a talk was added"
 msgstr "[%s] ajout d'une présentation"
 
 #, python-format
-msgid "[%s] talk status was updated"
+msgid "[%s] a talk was updated"
 msgstr "[%s] modification d'une présentation"
 
+#, python-format
+msgid "[%s] talk status was updated"
+msgstr "[%s] modification de l'état d'une présentation"
+
 msgid "accept talk"
 msgstr "accepter cette présentation"
 
+msgid "accept_pending"
+msgstr "en attente d'acceptation"
+
 msgid "accepted"
 msgstr "accepté"
 
-# Ajout document
-msgid "actions_adddoc"
-msgstr "Ajout document"
-
-msgid "actions_adddoc_description"
-msgstr "Description du document"
-
 # add related box generated message
 msgid "add Talk has_attachments File subject"
 msgstr "fichier"
 
+msgid "add Talk in_conf Conference object"
+msgstr "présentation"
+
 msgid "add Talk in_track Track object"
 msgstr "présentation"
 
-msgid "add Track in conference Conference object"
+msgid "add Track in_conf Conference object"
 msgstr "session"
 
 msgctxt "inlined:Sponsor.has_logo.subject"
-msgid "add a Image"
-msgstr "Ajouter une image"
+msgid "add a File"
+msgstr "ajouter un fichier"
 
-msgid "add document to the talk"
-msgstr "Ajouter un document"
+msgctxt "inlined:Conference.take_place_at.subject"
+msgid "add a PostalAddress"
+msgstr "ajouter une adresse"
+
+msgid "adminview"
+msgstr "admin"
 
 msgid "archive"
 msgstr "archiver"
 
 msgid "archived"
 msgstr "archivé"
 
@@ -287,98 +374,115 @@
 msgctxt "Talk"
 msgid "attend_object"
 msgstr "Réservation"
 
 msgid "attend_object"
 msgstr "Réservation"
 
-msgid "boxes_attachments_downloads_box"
-msgstr ""
+msgid "call_open"
+msgstr "appel ouvert"
 
-msgid "boxes_attachments_downloads_box_description"
+msgctxt "Conference"
+msgid "call_open"
 msgstr ""
 
-msgid "boxes_atthesametimebox"
-msgstr ""
+msgid "click here if you do not plan to attend this talk"
+msgstr "cliquez ici si vous ne comptez pas assister à cette présentation"
+
+msgid "click here if you plan to attend this talk"
+msgstr "cliquer ici si vous souhaitez assister à cette présentation"
+
+msgctxt "Talk"
+msgid "comments_object"
+msgstr "Commentaire"
+
+msgid "conference workflow"
+msgstr "diagramme des états de la conférence"
 
-msgid "boxes_atthesametimebox_description"
+msgid "confinfo"
+msgstr "Informations"
+
+msgid "correction"
 msgstr ""
 
-msgid "boxes_callbox"
+msgid "creating File (Talk %(linkto)s has_attachments File)"
+msgstr "Joindre un fichier à la présentation %(linkto)s"
+
+msgid "creating Track (Track in_conf Conference %(linkto)s)"
+msgstr "Ajouter une session dans la conférence %(linkto)s"
+
+msgid "ctxcomponents_attachments_downloads_box"
 msgstr ""
 
-msgid "boxes_callbox_description"
+msgid "ctxcomponents_attachments_downloads_box_description"
 msgstr ""
 
-msgid "boxes_sponsorbox"
-msgstr "boîte des sponsors"
+msgid "ctxcomponents_attendance"
+msgstr ""
 
-msgid "boxes_sponsorbox_description"
+msgid "ctxcomponents_attendance_description"
 msgstr ""
 
-#, python-format
-msgid "click here if you don't want to attend this %s anymore"
-msgstr "cliquer ici si vous ne souhaitez plus assister à ce %s"
+msgid "ctxcomponents_atthesametimebox"
+msgstr ""
 
-#, python-format
-msgid "click here to attend this %s"
-msgstr "cliquer ici pour assister a ce %s"
+msgid "ctxcomponents_atthesametimebox_description"
+msgstr ""
 
-msgid "comment"
-msgstr "Commentaire"
+msgid "ctxcomponents_callbox"
+msgstr ""
 
-msgctxt "Talk"
-msgid "comments_object"
-msgstr "Commentaire"
+msgid "ctxcomponents_callbox_description"
+msgstr ""
 
-msgid "conference workflow"
-msgstr "diagramme des états de la conférence"
+msgid "ctxcomponents_review-status"
+msgstr ""
 
-msgid "confinfo"
-msgstr "Informations"
+msgid "ctxcomponents_review-status_description"
+msgstr ""
 
-msgid "contentnavigation_adminviewcomponent"
+msgid "ctxcomponents_sponsorbox"
 msgstr ""
 
-msgid "contentnavigation_adminviewcomponent_description"
+msgid "ctxcomponents_sponsorbox_description"
 msgstr ""
 
-msgid "contentnavigation_attendance"
+msgid "ctxcomponents_talk-status"
 msgstr ""
 
-msgid "contentnavigation_attendance_description"
+msgid "ctxcomponents_talk-status_description"
 msgstr ""
 
-msgid "correction"
+msgid "ctxcomponents_talkstate"
 msgstr ""
 
-msgid "creating File (Talk %(linkto)s has_attachments File)"
-msgstr "Joindre un fichier à la présentation %(linkto)s"
+msgid "ctxcomponents_talkstate2"
+msgstr ""
 
-msgid "creating Talk (Talk in_track Track %(linkto)s)"
-msgstr "Ajouter une présentation dans la session %(linkto)s"
+msgid "ctxcomponents_talkstate2_description"
+msgstr ""
 
-msgid "date"
+msgid "ctxcomponents_talkstate_description"
 msgstr ""
 
 msgctxt "Conference"
 msgid "description"
-msgstr ""
+msgstr "description"
 
 msgctxt "Track"
 msgid "description"
-msgstr ""
+msgstr "description"
 
 msgctxt "Sponsor"
 msgid "description"
-msgstr ""
+msgstr "description"
 
 msgctxt "Talk"
 msgid "description"
-msgstr ""
+msgstr "description"
 
 msgctxt "Conference"
 msgid "description_format"
 msgstr ""
 
 msgctxt "Track"
 msgid "description_format"
@@ -388,17 +492,14 @@
 msgid "description_format"
 msgstr ""
 
 msgctxt "Talk"
 msgid "description_format"
 msgstr ""
 
-msgid "download icon"
-msgstr "icône de téléchargement"
-
 msgid "draft"
 msgstr "brouillon"
 
 msgid "end_on"
 msgstr "date de fin"
 
 msgctxt "Conference"
@@ -426,43 +527,39 @@
 
 msgid "facets_track-facet"
 msgstr ""
 
 msgid "facets_track-facet_description"
 msgstr ""
 
-msgid "from_state"
-msgstr "de l'état"
+msgid "generate badges"
+msgstr "générer les badges"
 
 msgid "has_attachments"
 msgstr "a des pièces jointes"
 
 msgctxt "Talk"
 msgid "has_attachments"
 msgstr "lié au fichier"
 
-msgctxt "Image"
-msgid "has_attachments_object"
-msgstr ""
-
 msgctxt "File"
 msgid "has_attachments_object"
 msgstr "est lié à l'objet"
 
 msgid "has_attachments_object"
 msgstr "a un fichier attaché"
 
 msgid "has_logo"
 msgstr "a un logo"
 
 msgctxt "Sponsor"
 msgid "has_logo"
 msgstr "a un logo"
 
-msgctxt "Image"
+msgctxt "File"
 msgid "has_logo_object"
 msgstr "a un logo"
 
 msgid "has_logo_object"
 msgstr "a un logo"
 
 msgid "in"
@@ -502,41 +599,69 @@
 
 msgid "in_track_object"
 msgstr "est dans la session"
 
 msgid "inreview"
 msgstr "en relecture"
 
+msgid "is_chair_at"
+msgstr ""
+
+msgctxt "CWUser"
+msgid "is_chair_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "is_chair_at_object"
+msgstr ""
+
+msgid "is_chair_at_object"
+msgstr ""
+
+msgid "is_reviewer_at"
+msgstr ""
+
+msgctxt "CWUser"
+msgid "is_reviewer_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "is_reviewer_at_object"
+msgstr ""
+
+msgid "is_reviewer_at_object"
+msgstr ""
+
 msgid "is_sponsor"
 msgstr "est sponsor"
 
 msgctxt "Sponsor"
 msgid "is_sponsor"
 msgstr "est sponsor"
 
 msgctxt "SponsorShip"
 msgid "is_sponsor_object"
 msgstr ""
 
 msgid "is_sponsor_object"
-msgstr ""
+msgstr "sponsorise"
 
 msgid "leads"
 msgstr "dirige"
 
 msgctxt "CWUser"
 msgid "leads"
 msgstr "dirige"
 
 msgctxt "Talk"
 msgid "leads_object"
 msgstr ""
 
 msgid "leads_object"
-msgstr ""
+msgstr "dirigé par"
 
 msgid "level"
 msgstr "niveau"
 
 msgctxt "SponsorShip"
 msgid "level"
 msgstr ""
@@ -547,35 +672,57 @@
 msgctxt "Talk"
 msgid "location"
 msgstr "salle"
 
 msgid "need correction"
 msgstr "nécessite des corrections"
 
+msgid "need more review"
+msgstr ""
+
 #, python-format
 msgid "on %(sdate)s from %(stime)s to %(etime)s"
-msgstr ""
+msgstr "le %(sdate)s de %(stime)s à %(etime)s"
 
 msgid "one day"
 msgstr "un jour"
 
-msgid "people were registered"
-msgstr "inscrits"
+msgid "people plan to attend"
+msgstr "personnes comptent y assister"
 
 msgid "planned"
 msgstr "prévu"
 
 msgid "please contact us"
+msgstr "veuillez nous contacter"
+
+msgid "propose to accept"
+msgstr ""
+
+msgid "propose to reject"
+msgstr ""
+
+msgid "redraft"
+msgstr ""
+
+msgid "reg_open"
+msgstr "inscription ouverte"
+
+msgctxt "Conference"
+msgid "reg_open"
 msgstr ""
 
 msgid "reject talk"
-msgstr "rejeter cette présentation"
+msgstr "refuser cette présentation"
+
+msgid "reject_pending"
+msgstr "attente de refus"
 
 msgid "rejected"
-msgstr "rejeté"
+msgstr "refusé"
 
 msgid "representing"
 msgstr "représentant"
 
 msgctxt "CWUser"
 msgid "representing"
 msgstr "représente"
@@ -642,21 +789,35 @@
 
 msgid "submit your work"
 msgstr "soumettre votre travail"
 
 msgid "submitted"
 msgstr "soumis"
 
-msgid "swrc"
+msgid "swc"
 msgstr ""
 
 msgctxt "Talk"
 msgid "tags_object"
 msgstr ""
 
+msgid "take_place_at"
+msgstr "a lieu"
+
+msgctxt "Conference"
+msgid "take_place_at"
+msgstr ""
+
+msgctxt "PostalAddress"
+msgid "take_place_at_object"
+msgstr ""
+
+msgid "take_place_at_object"
+msgstr ""
+
 msgid "talk workflow"
 msgstr "diagramme des états d'une présentation"
 
 msgid "talkslist"
 msgstr "Liste des présentations"
 
 msgid "talksschedule"
@@ -664,153 +825,105 @@
 
 msgctxt "Conference"
 msgid "title"
 msgstr "titre"
 
 msgctxt "SponsorShip"
 msgid "title"
-msgstr ""
+msgstr "titre"
 
 msgctxt "Track"
 msgid "title"
 msgstr "titre"
 
-msgctxt "Sponsor"
+msgctxt "Talk"
 msgid "title"
 msgstr "titre"
 
-msgctxt "Talk"
+msgctxt "Sponsor"
 msgid "title"
 msgstr "titre"
 
-msgid "to_state"
-msgstr "vers l'état"
+msgid "trackinfo"
+msgstr "description"
+
+msgid "tracktalkslist"
+msgstr "présentations"
+
+msgid "tracktalksschedule"
+msgstr "programme"
+
+msgid "unique conference identifier for url"
+msgstr ""
 
 msgid "url"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "url"
 msgstr ""
 
+msgid "url_id"
+msgstr ""
+
+msgctxt "Conference"
+msgid "url_id"
+msgstr ""
+
 msgid "userconfschedule"
-msgstr "planning personnel"
+msgstr "programme personnel"
 
 msgid "you are not anymore registered to attend this talk"
 msgstr "Vous n'êtes plus inscrit"
 
 msgid "you are now registered to attend this talk"
 msgstr "Vous êtes maintenant inscrit"
 
-#~ msgid ", on"
-#~ msgstr ", le"
-
-#~ msgid "Coming soon"
-#~ msgstr "A venir"
-
-# schema pot file, generated on 2009-04-13 15:10:08
-#
-# singular and plural forms for each entity type
-#~ msgid "Conférence"
-#~ msgstr "Conférence"
-
-#~ msgid "Conférence_plural"
-#~ msgstr "Conférences"
-
-#~ msgid "Following talks were presented:"
-#~ msgstr "Les conférences suivantes ont été présentées:"
-
-#~ msgid ""
-#~ "If you are interested in sponsoring or partnering, please contact us."
-#~ msgstr ""
-#~ "Si vous souhaitez devenir sponsor, merci de contacter les organisateurs"
-
-#~ msgid "New Conférence"
-#~ msgstr "Nouvelle Conférence"
-
-#~ msgid "No talks yet in this conference"
-#~ msgstr "Pas encore de présentations pour cette conférence"
-
-#~ msgid "Previous conferences"
-#~ msgstr "Conférences précédentes"
-
-#~ msgid "The conference covered the following tracks:"
-#~ msgstr "La conférence a couvert les sujets suivants:"
+msgid "your reviews"
+msgstr ""
 
-#~ msgid "The following tracks will be covered during the conference:"
-#~ msgstr "Les sujets suivants seront couverts durant la conférence:"
+msgid "your talks"
+msgstr "vos présentations"
 
-# [%s] une présentation a été mise à jour.
-#~ msgid "[%s] a talk was updated."
-#~ msgstr "[%s] une présentation a été mise à jour."
+#~ msgid "Workflow history"
+#~ msgstr "historique"
 
-#~ msgid "accept"
-#~ msgstr "accepter"
+#~ msgid "[%s] a talk was added."
+#~ msgstr "[%s] ajout d'une présentation"
 
-#~ msgid "actions_addtrack"
+#~ msgid "add Track in conference Conference object"
 #~ msgstr "session"
 
-#~ msgid "add Sponsor supports_conf Conference object"
-#~ msgstr "sponsor"
-
-#~ msgid "add Sponsor supports_conf Conference subject"
-#~ msgstr "sponsor"
-
-#~ msgid "add a Conference"
-#~ msgstr "ajouter une conférence"
-
-#~ msgid "add a Talk"
-#~ msgstr "ajouter une présentation"
-
-#~ msgid "add a Track"
-#~ msgstr "ajouter un sujet"
-
-#~ msgid "approve"
-#~ msgstr "approuver"
-
-#~ msgid "approved"
-#~ msgstr "approuve"
-
-#~ msgid "at"
-#~ msgstr "à"
-
-#~ msgid "creating Sponsor (Sponsor supports_conf Conference %(linkto)s)"
-#~ msgstr "Ajouter un sponsor pour la conférence %(linkto)s"
-
-#~ msgctxt "Sponsor"
-#~ msgid "level"
-#~ msgstr "niveau"
-
-#~ msgid "proposed"
-#~ msgstr "proposé"
+#~ msgctxt "inlined:Sponsor.has_logo.subject"
+#~ msgid "add a Image"
+#~ msgstr "Ajouter une image"
 
-#~ msgid "reject"
-#~ msgstr "rejeter"
+#~ msgid "add document to the talk"
+#~ msgstr "Ajouter un document"
 
-#~ msgid "remove this Conference"
-#~ msgstr "supprimer cette conférence"
+#~ msgid "boxes_sponsorbox"
+#~ msgstr "boîte des sponsors"
 
-#~ msgctxt "inlined:Sponsor.has_logo.subject"
-#~ msgid "remove this Image"
-#~ msgstr "supprimer cette image"
+#~ msgid "comment"
+#~ msgstr "Commentaire"
 
-#~ msgid "remove this Talk"
-#~ msgstr "supprimer cette présentation"
+#~ msgid "creating Talk (Talk in_conf Conference %(linkto)s)"
+#~ msgstr "Ajouter une présentation dans la conférence %(linkto)s"
 
-#~ msgid "remove this Track"
-#~ msgstr "supprimer ce sujet"
+#~ msgid "creating Talk (Talk in_track Track %(linkto)s)"
+#~ msgstr "Ajouter une présentation dans la session %(linkto)s"
 
-#~ msgid "speaker"
-#~ msgstr "intervenant"
+#~ msgid "date"
+#~ msgstr "date"
 
-#~ msgid "supports_conf"
-#~ msgstr "soutien la conférence"
+#~ msgid "download icon"
+#~ msgstr "icône de téléchargement"
 
-#~ msgctxt "Sponsor"
-#~ msgid "supports_conf"
-#~ msgstr "soutien la conférence"
+#~ msgid "from_state"
+#~ msgstr "de l'état"
 
-#~ msgid "you are not anymore registered to attend this %s"
-#~ msgstr "vous n'êtes plus enregistré pour assister à ce %s"
+#~ msgctxt "Image"
+#~ msgid "has_logo_object"
+#~ msgstr "a un logo"
 
-#~ msgid "you are now registered to attend this %s"
-#~ msgstr "vous êtes enregistré pour assister à ce %s"
+#~ msgid "to_state"
+#~ msgstr "vers l'état"
```

### Comparing `cubicweb-conference-0.4.2/i18n/es.po` & `cubicweb-conference-1.0.0/cubicweb_conference/i18n/de.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: cubicweb 3.5.12\n"
+"Project-Id-Version: cubicweb 3.10.5\n"
 "PO-Revision-Date: 2008-03-28 18:14+0100\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
 "Language-Team: fr <contact@logilab.fr>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: cubicweb-devtools\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Abstract"
 msgstr ""
 
-msgid "Abstract submission is open !"
+msgid "Answer the call for talks !"
 msgstr ""
 
 msgid "At the same time"
 msgstr ""
 
 msgid "Attachments"
 msgstr ""
 
+msgid "Authentication is needed to perform this action"
+msgstr ""
+
+msgid "Begin"
+msgstr ""
+
 msgid "Call for paper"
 msgstr ""
 
-# schema pot file, generated on 2010-02-10 20:30:40
+# schema pot file, generated on 2010-11-29 11:39:39
 #
 # singular and plural forms for each entity type
 msgid "Conference"
 msgstr ""
 
 msgid "Conference_plural"
 msgstr ""
@@ -74,32 +80,38 @@
 "The conference organizing committee.\n"
 msgstr ""
 
 msgid "Description"
 msgstr ""
 
 msgid ""
-"Do you plan to attend a specific talk ? Please click on the \"I plan to "
-"attend\" button positionned at the top right of each talk summary."
+"Do you plan to attend a specific talk ? Please click on the attendancy "
+"button positionned at the top right of each talk summary."
+msgstr ""
+
+msgid "End"
+msgstr ""
+
+msgctxt "inlined:Sponsor.has_logo.subject"
+msgid "File"
 msgstr ""
 
 msgid "First talk"
 msgstr ""
 
-msgid "I do not plan to attend"
+msgid "Generate badges"
 msgstr ""
 
-msgid "I plan to attend"
+msgid "If you already have an account, please log in"
 msgstr ""
 
 msgid "If you are interested in sponsoring or partnering"
 msgstr ""
 
-msgctxt "inlined:Sponsor.has_logo.subject"
-msgid "Image"
+msgid "If you do not have an account yet, please create one"
 msgstr ""
 
 msgid "Index"
 msgstr ""
 
 msgid "Last talk"
 msgstr ""
@@ -118,35 +130,45 @@
 
 msgid "New Talk"
 msgstr ""
 
 msgid "New Track"
 msgstr ""
 
-msgid "No conference planned for now..."
+msgid "No accepted talk yet in this conference"
 msgstr ""
 
-msgid "No talk yet in this conference"
+msgid "No accepted talk yet in this track"
+msgstr ""
+
+msgid "No conference planned for now..."
 msgstr ""
 
 msgid "No track yet in this conference."
 msgstr ""
 
 msgid "Number of participant by Talk"
 msgstr ""
 
 msgid "Past conferences"
 msgstr ""
 
 msgid "Please, assign a reviewer to :"
 msgstr ""
 
+msgctxt "inlined:Conference.take_place_at.subject"
+msgid "PostalAddress"
+msgstr ""
+
 msgid "Presented by"
 msgstr ""
 
+msgid "Remember you have already submitted a talk."
+msgstr ""
+
 msgid "Representing"
 msgstr ""
 
 msgid "Speaker"
 msgstr ""
 
 msgid "Sponsor"
@@ -163,33 +185,28 @@
 
 msgid "Talk"
 msgstr ""
 
 msgid "Talk state details"
 msgstr ""
 
-msgid "Talk submission informations"
-msgstr ""
-
 msgid "Talk title"
 msgstr ""
 
 msgid "Talk_plural"
 msgstr ""
 
-msgid "The conference was divided into the following tracks:"
-msgstr ""
-
-msgid "The conference will be divided into the following tracks:"
+#, python-format
+msgid "Talks you have to review (in state %s)"
 msgstr ""
 
-msgid "The following talks were presented:"
+msgid "The conference was divided into the following tracks:"
 msgstr ""
 
-msgid "The following talks will be presented:"
+msgid "The conference will be divided into the following tracks:"
 msgstr ""
 
 msgid "This Conference"
 msgstr ""
 
 msgid "This Sponsor"
 msgstr ""
@@ -199,14 +216,43 @@
 
 msgid "This Talk"
 msgstr ""
 
 msgid "This Track"
 msgstr ""
 
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means it needs to be submitted before it "
+"can be considered by the reviewers."
+msgstr ""
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means the author needs to answer the "
+"comments of the reviewers."
+msgstr ""
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means the reviewers will soon send you "
+"their comments."
+msgstr ""
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means you have to review it. You can ask "
+"the author for modifications, accept or reject this talk."
+msgstr ""
+
+msgid ""
+"This talk was reviewed and is now awaiting a final decision by the "
+"conference chairs."
+msgstr ""
+
 msgid "Total talks"
 msgstr ""
 
 msgid "Track"
 msgstr ""
 
 msgid "Track title"
@@ -214,151 +260,187 @@
 
 msgid "Track_plural"
 msgstr ""
 
 msgid "Upcoming conferences"
 msgstr ""
 
-msgid "View statistics"
+msgid "You are planning to attend these talks:"
+msgstr ""
+
+msgid "You can select a new logo, else the site's logo will be taken"
+msgstr ""
+
+msgid "You do not plan to attend"
 msgstr ""
 
-msgid "Workflow history"
+msgid ""
+"You need to create an account and sign in before you can submit an abstract"
+msgstr ""
+
+msgid "You plan to attend"
+msgstr ""
+
+#, python-format
+msgid "Your talks in state %s"
 msgstr ""
 
-msgid "You are registered for these talks:"
+#, python-format
+msgid "[%s] a talk was added"
 msgstr ""
 
 #, python-format
-msgid "[%s] a talk was added."
+msgid "[%s] a talk was updated"
 msgstr ""
 
 #, python-format
 msgid "[%s] talk status was updated"
 msgstr ""
 
 msgid "accept talk"
 msgstr ""
 
-msgid "accepted"
+msgid "accept_pending"
 msgstr ""
 
-msgid "actions_adddoc"
+msgid "accepted"
 msgstr ""
 
-msgid "actions_adddoc_description"
+msgid "add Talk has_attachments File subject"
 msgstr ""
 
-msgid "add Talk has_attachments File subject"
+msgid "add Talk in_conf Conference object"
 msgstr ""
 
 msgid "add Talk in_track Track object"
 msgstr ""
 
-msgid "add Track in conference Conference object"
+msgid "add Track in_conf Conference object"
 msgstr ""
 
 msgctxt "inlined:Sponsor.has_logo.subject"
-msgid "add a Image"
+msgid "add a File"
+msgstr ""
+
+msgctxt "inlined:Conference.take_place_at.subject"
+msgid "add a PostalAddress"
 msgstr ""
 
-msgid "add document to the talk"
+msgid "adminview"
 msgstr ""
 
 msgid "archive"
 msgstr ""
 
 msgid "archived"
 msgstr ""
 
 msgid "ask for correction"
 msgstr ""
 
 # subject and object forms for each relation type
-# (no object form for final or symetric relation types)
+# (no object form for final or symmetric relation types)
 msgid "attend"
 msgstr ""
 
 msgctxt "CWUser"
 msgid "attend"
 msgstr ""
 
 msgctxt "Talk"
 msgid "attend_object"
 msgstr ""
 
 msgid "attend_object"
 msgstr ""
 
-msgid "boxes_attachments_downloads_box"
+msgid "call_open"
 msgstr ""
 
-msgid "boxes_attachments_downloads_box_description"
+msgctxt "Conference"
+msgid "call_open"
 msgstr ""
 
-msgid "boxes_atthesametimebox"
+msgid "click here if you do not plan to attend this talk"
 msgstr ""
 
-msgid "boxes_atthesametimebox_description"
+msgid "click here if you plan to attend this talk"
 msgstr ""
 
-msgid "boxes_callbox"
+msgctxt "Talk"
+msgid "comments_object"
 msgstr ""
 
-msgid "boxes_callbox_description"
+msgid "conference workflow"
 msgstr ""
 
-msgid "boxes_sponsorbox"
+msgid "confinfo"
 msgstr ""
 
-msgid "boxes_sponsorbox_description"
+msgid "correction"
 msgstr ""
 
-#, python-format
-msgid "click here if you don't want to attend this %s anymore"
+msgid "creating File (Talk %(linkto)s has_attachments File)"
 msgstr ""
 
-#, python-format
-msgid "click here to attend this %s"
+msgid "creating Track (Track in_conf Conference %(linkto)s)"
 msgstr ""
 
-msgid "comment"
+msgid "ctxcomponents_attachments_downloads_box"
 msgstr ""
 
-msgctxt "Talk"
-msgid "comments_object"
+msgid "ctxcomponents_attachments_downloads_box_description"
 msgstr ""
 
-msgid "conference workflow"
+msgid "ctxcomponents_attendance"
 msgstr ""
 
-msgid "confinfo"
+msgid "ctxcomponents_attendance_description"
 msgstr ""
 
-msgid "contentnavigation_adminviewcomponent"
+msgid "ctxcomponents_atthesametimebox"
 msgstr ""
 
-msgid "contentnavigation_adminviewcomponent_description"
+msgid "ctxcomponents_atthesametimebox_description"
 msgstr ""
 
-msgid "contentnavigation_attendance"
+msgid "ctxcomponents_callbox"
 msgstr ""
 
-msgid "contentnavigation_attendance_description"
+msgid "ctxcomponents_callbox_description"
 msgstr ""
 
-msgid "correction"
+msgid "ctxcomponents_review-status"
 msgstr ""
 
-msgid "creating File (Talk %(linkto)s has_attachments File)"
+msgid "ctxcomponents_review-status_description"
+msgstr ""
+
+msgid "ctxcomponents_sponsorbox"
 msgstr ""
 
-msgid "creating Talk (Talk in_track Track %(linkto)s)"
+msgid "ctxcomponents_sponsorbox_description"
 msgstr ""
 
-msgid "date"
+msgid "ctxcomponents_talk-status"
+msgstr ""
+
+msgid "ctxcomponents_talk-status_description"
+msgstr ""
+
+msgid "ctxcomponents_talkstate"
+msgstr ""
+
+msgid "ctxcomponents_talkstate2"
+msgstr ""
+
+msgid "ctxcomponents_talkstate2_description"
+msgstr ""
+
+msgid "ctxcomponents_talkstate_description"
 msgstr ""
 
 msgctxt "Conference"
 msgid "description"
 msgstr ""
 
 msgctxt "Track"
@@ -385,17 +467,14 @@
 msgid "description_format"
 msgstr ""
 
 msgctxt "Talk"
 msgid "description_format"
 msgstr ""
 
-msgid "download icon"
-msgstr ""
-
 msgid "draft"
 msgstr ""
 
 msgid "end_on"
 msgstr ""
 
 msgctxt "Conference"
@@ -423,43 +502,39 @@
 
 msgid "facets_track-facet"
 msgstr ""
 
 msgid "facets_track-facet_description"
 msgstr ""
 
-msgid "from_state"
+msgid "generate badges"
 msgstr ""
 
 msgid "has_attachments"
 msgstr ""
 
 msgctxt "Talk"
 msgid "has_attachments"
 msgstr ""
 
-msgctxt "Image"
-msgid "has_attachments_object"
-msgstr ""
-
 msgctxt "File"
 msgid "has_attachments_object"
 msgstr ""
 
 msgid "has_attachments_object"
 msgstr ""
 
 msgid "has_logo"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "has_logo"
 msgstr ""
 
-msgctxt "Image"
+msgctxt "File"
 msgid "has_logo_object"
 msgstr ""
 
 msgid "has_logo_object"
 msgstr ""
 
 msgid "in"
@@ -499,14 +574,42 @@
 
 msgid "in_track_object"
 msgstr ""
 
 msgid "inreview"
 msgstr ""
 
+msgid "is_chair_at"
+msgstr ""
+
+msgctxt "CWUser"
+msgid "is_chair_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "is_chair_at_object"
+msgstr ""
+
+msgid "is_chair_at_object"
+msgstr ""
+
+msgid "is_reviewer_at"
+msgstr ""
+
+msgctxt "CWUser"
+msgid "is_reviewer_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "is_reviewer_at_object"
+msgstr ""
+
+msgid "is_reviewer_at_object"
+msgstr ""
+
 msgid "is_sponsor"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "is_sponsor"
 msgstr ""
 
@@ -544,33 +647,55 @@
 msgctxt "Talk"
 msgid "location"
 msgstr ""
 
 msgid "need correction"
 msgstr ""
 
+msgid "need more review"
+msgstr ""
+
 #, python-format
 msgid "on %(sdate)s from %(stime)s to %(etime)s"
 msgstr ""
 
 msgid "one day"
 msgstr ""
 
-msgid "people were registered"
+msgid "people plan to attend"
 msgstr ""
 
 msgid "planned"
 msgstr ""
 
 msgid "please contact us"
 msgstr ""
 
+msgid "propose to accept"
+msgstr ""
+
+msgid "propose to reject"
+msgstr ""
+
+msgid "redraft"
+msgstr ""
+
+msgid "reg_open"
+msgstr ""
+
+msgctxt "Conference"
+msgid "reg_open"
+msgstr ""
+
 msgid "reject talk"
 msgstr ""
 
+msgid "reject_pending"
+msgstr ""
+
 msgid "rejected"
 msgstr ""
 
 msgid "representing"
 msgstr ""
 
 msgctxt "CWUser"
@@ -639,21 +764,35 @@
 
 msgid "submit your work"
 msgstr ""
 
 msgid "submitted"
 msgstr ""
 
-msgid "swrc"
+msgid "swc"
 msgstr ""
 
 msgctxt "Talk"
 msgid "tags_object"
 msgstr ""
 
+msgid "take_place_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "take_place_at"
+msgstr ""
+
+msgctxt "PostalAddress"
+msgid "take_place_at_object"
+msgstr ""
+
+msgid "take_place_at_object"
+msgstr ""
+
 msgid "talk workflow"
 msgstr ""
 
 msgid "talkslist"
 msgstr ""
 
 msgid "talksschedule"
@@ -667,33 +806,55 @@
 msgid "title"
 msgstr ""
 
 msgctxt "Track"
 msgid "title"
 msgstr ""
 
-msgctxt "Sponsor"
+msgctxt "Talk"
 msgid "title"
 msgstr ""
 
-msgctxt "Talk"
+msgctxt "Sponsor"
 msgid "title"
 msgstr ""
 
-msgid "to_state"
+msgid "trackinfo"
+msgstr ""
+
+msgid "tracktalkslist"
+msgstr ""
+
+msgid "tracktalksschedule"
+msgstr ""
+
+msgid "unique conference identifier for url"
 msgstr ""
 
 msgid "url"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "url"
 msgstr ""
 
+msgid "url_id"
+msgstr ""
+
+msgctxt "Conference"
+msgid "url_id"
+msgstr ""
+
 msgid "userconfschedule"
 msgstr ""
 
 msgid "you are not anymore registered to attend this talk"
 msgstr ""
 
 msgid "you are now registered to attend this talk"
 msgstr ""
+
+msgid "your reviews"
+msgstr ""
+
+msgid "your talks"
+msgstr ""
```

### Comparing `cubicweb-conference-0.4.2/i18n/en.po` & `cubicweb-conference-1.0.0/cubicweb_conference/i18n/es.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: cubicweb 3.1.5\n"
-"PO-Revision-Date: 2010-02-10 20:02+0100\n"
+"Project-Id-Version: cubicweb 3.5.12\n"
+"PO-Revision-Date: 2008-03-28 18:14+0100\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
 "Language-Team: fr <contact@logilab.fr>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: cubicweb-devtools\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Abstract"
 msgstr ""
 
-msgid "Abstract submission is open !"
+msgid "Answer the call for talks !"
 msgstr ""
 
 msgid "At the same time"
 msgstr ""
 
 msgid "Attachments"
 msgstr ""
 
+msgid "Authentication is needed to perform this action"
+msgstr ""
+
+msgid "Begin"
+msgstr ""
+
 msgid "Call for paper"
 msgstr ""
 
-# schema pot file, generated on 2009-04-13 15:10:08
+# schema pot file, generated on 2010-02-10 20:30:40
 #
 # singular and plural forms for each entity type
 msgid "Conference"
 msgstr ""
 
 msgid "Conference_plural"
-msgstr "Conferences"
+msgstr ""
 
 msgid "Date"
 msgstr ""
 
 #, python-format
 msgid ""
 "Dear %(firstname)s %(lastname)s,\n"
@@ -74,32 +80,38 @@
 "The conference organizing committee.\n"
 msgstr ""
 
 msgid "Description"
 msgstr ""
 
 msgid ""
-"Do you plan to attend a specific talk ? Please click on the \"I plan to "
-"attend\" button positionned at the top right of each talk summary."
+"Do you plan to attend a specific talk ? Please click on the attendancy "
+"button positionned at the top right of each talk summary."
+msgstr ""
+
+msgid "End"
+msgstr ""
+
+msgctxt "inlined:Sponsor.has_logo.subject"
+msgid "File"
 msgstr ""
 
 msgid "First talk"
 msgstr ""
 
-msgid "I do not plan to attend"
+msgid "Generate badges"
 msgstr ""
 
-msgid "I plan to attend"
+msgid "If you already have an account, please log in"
 msgstr ""
 
 msgid "If you are interested in sponsoring or partnering"
 msgstr ""
 
-msgctxt "inlined:Sponsor.has_logo.subject"
-msgid "Image"
+msgid "If you do not have an account yet, please create one"
 msgstr ""
 
 msgid "Index"
 msgstr ""
 
 msgid "Last talk"
 msgstr ""
@@ -118,35 +130,45 @@
 
 msgid "New Talk"
 msgstr ""
 
 msgid "New Track"
 msgstr ""
 
-msgid "No conference planned for now..."
+msgid "No accepted talk yet in this conference"
+msgstr ""
+
+msgid "No accepted talk yet in this track"
 msgstr ""
 
-msgid "No talk yet in this conference"
+msgid "No conference planned for now..."
 msgstr ""
 
 msgid "No track yet in this conference."
 msgstr ""
 
 msgid "Number of participant by Talk"
 msgstr ""
 
 msgid "Past conferences"
 msgstr ""
 
 msgid "Please, assign a reviewer to :"
 msgstr ""
 
+msgctxt "inlined:Conference.take_place_at.subject"
+msgid "PostalAddress"
+msgstr ""
+
 msgid "Presented by"
 msgstr ""
 
+msgid "Remember you have already submitted a talk."
+msgstr ""
+
 msgid "Representing"
 msgstr ""
 
 msgid "Speaker"
 msgstr ""
 
 msgid "Sponsor"
@@ -155,41 +177,36 @@
 msgid "SponsorShip"
 msgstr ""
 
 msgid "SponsorShip_plural"
 msgstr ""
 
 msgid "Sponsor_plural"
-msgstr "Sponsors"
+msgstr ""
 
 msgid "Talk"
 msgstr ""
 
 msgid "Talk state details"
 msgstr ""
 
-msgid "Talk submission informations"
-msgstr ""
-
 msgid "Talk title"
 msgstr ""
 
 msgid "Talk_plural"
-msgstr "Talks"
-
-msgid "The conference was divided into the following tracks:"
 msgstr ""
 
-msgid "The conference will be divided into the following tracks:"
+#, python-format
+msgid "Talks you have to review (in state %s)"
 msgstr ""
 
-msgid "The following talks were presented:"
+msgid "The conference was divided into the following tracks:"
 msgstr ""
 
-msgid "The following talks will be presented:"
+msgid "The conference will be divided into the following tracks:"
 msgstr ""
 
 msgid "This Conference"
 msgstr ""
 
 msgid "This Sponsor"
 msgstr ""
@@ -199,167 +216,231 @@
 
 msgid "This Talk"
 msgstr ""
 
 msgid "This Track"
 msgstr ""
 
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means it needs to be submitted before it "
+"can be considered by the reviewers."
+msgstr ""
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means the author needs to answer the "
+"comments of the reviewers."
+msgstr ""
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means the reviewers will soon send you "
+"their comments."
+msgstr ""
+
+#, python-format
+msgid ""
+"This talk is in state \"%s\", which means you have to review it. You can ask "
+"the author for modifications, accept or reject this talk."
+msgstr ""
+
+msgid ""
+"This talk was reviewed and is now awaiting a final decision by the "
+"conference chairs."
+msgstr ""
+
 msgid "Total talks"
 msgstr ""
 
 msgid "Track"
 msgstr ""
 
 msgid "Track title"
 msgstr ""
 
 msgid "Track_plural"
-msgstr "Tracks"
+msgstr ""
 
 msgid "Upcoming conferences"
 msgstr ""
 
-msgid "View statistics"
+msgid "You are planning to attend these talks:"
+msgstr ""
+
+msgid "You can select a new logo, else the site's logo will be taken"
+msgstr ""
+
+msgid "You do not plan to attend"
+msgstr ""
+
+msgid ""
+"You need to create an account and sign in before you can submit an abstract"
+msgstr ""
+
+msgid "You plan to attend"
 msgstr ""
 
-msgid "Workflow history"
+#, python-format
+msgid "Your talks in state %s"
 msgstr ""
 
-msgid "You are registered for these talks:"
+#, python-format
+msgid "[%s] a talk was added"
 msgstr ""
 
 #, python-format
-msgid "[%s] a talk was added."
+msgid "[%s] a talk was updated"
 msgstr ""
 
 #, python-format
 msgid "[%s] talk status was updated"
 msgstr ""
 
 msgid "accept talk"
 msgstr ""
 
-msgid "accepted"
+msgid "accept_pending"
 msgstr ""
 
-msgid "actions_adddoc"
+msgid "accepted"
 msgstr ""
 
-msgid "actions_adddoc_description"
+msgid "add Talk has_attachments File subject"
 msgstr ""
 
-# add related box generated message
-msgid "add Talk has_attachments File subject"
-msgstr "file"
+msgid "add Talk in_conf Conference object"
+msgstr ""
 
 msgid "add Talk in_track Track object"
-msgstr "talk"
+msgstr ""
 
-msgid "add Track in conference Conference object"
-msgstr "track"
+msgid "add Track in_conf Conference object"
+msgstr ""
 
 msgctxt "inlined:Sponsor.has_logo.subject"
-msgid "add a Image"
+msgid "add a File"
+msgstr ""
+
+msgctxt "inlined:Conference.take_place_at.subject"
+msgid "add a PostalAddress"
 msgstr ""
 
-msgid "add document to the talk"
+msgid "adminview"
 msgstr ""
 
 msgid "archive"
 msgstr ""
 
 msgid "archived"
 msgstr ""
 
 msgid "ask for correction"
 msgstr ""
 
 # subject and object forms for each relation type
-# (no object form for final relation types)
+# (no object form for final or symetric relation types)
 msgid "attend"
 msgstr ""
 
 msgctxt "CWUser"
 msgid "attend"
 msgstr ""
 
 msgctxt "Talk"
 msgid "attend_object"
 msgstr ""
 
 msgid "attend_object"
 msgstr ""
 
-msgid "boxes_attachments_downloads_box"
+msgid "call_open"
 msgstr ""
 
-msgid "boxes_attachments_downloads_box_description"
+msgctxt "Conference"
+msgid "call_open"
 msgstr ""
 
-msgid "boxes_atthesametimebox"
+msgid "click here if you do not plan to attend this talk"
 msgstr ""
 
-msgid "boxes_atthesametimebox_description"
+msgid "click here if you plan to attend this talk"
 msgstr ""
 
-msgid "boxes_callbox"
+msgctxt "Talk"
+msgid "comments_object"
 msgstr ""
 
-msgid "boxes_callbox_description"
+msgid "conference workflow"
 msgstr ""
 
-msgid "boxes_sponsorbox"
+msgid "confinfo"
 msgstr ""
 
-msgid "boxes_sponsorbox_description"
+msgid "correction"
 msgstr ""
 
-#, python-format
-msgid "click here if you don't want to attend this %s anymore"
+msgid "creating File (Talk %(linkto)s has_attachments File)"
 msgstr ""
 
-#, python-format
-msgid "click here to attend this %s"
+msgid "creating Track (Track in_conf Conference %(linkto)s)"
 msgstr ""
 
-msgid "comment"
+msgid "ctxcomponents_attachments_downloads_box"
 msgstr ""
 
-msgctxt "Talk"
-msgid "comments_object"
+msgid "ctxcomponents_attachments_downloads_box_description"
 msgstr ""
 
-msgid "conference workflow"
+msgid "ctxcomponents_attendance"
 msgstr ""
 
-msgid "confinfo"
+msgid "ctxcomponents_attendance_description"
 msgstr ""
 
-msgid "contentnavigation_adminviewcomponent"
+msgid "ctxcomponents_atthesametimebox"
 msgstr ""
 
-msgid "contentnavigation_adminviewcomponent_description"
+msgid "ctxcomponents_atthesametimebox_description"
 msgstr ""
 
-msgid "contentnavigation_attendance"
+msgid "ctxcomponents_callbox"
 msgstr ""
 
-msgid "contentnavigation_attendance_description"
+msgid "ctxcomponents_callbox_description"
 msgstr ""
 
-msgid "correction"
+msgid "ctxcomponents_review-status"
 msgstr ""
 
-msgid "creating File (Talk %(linkto)s has_attachments File)"
+msgid "ctxcomponents_review-status_description"
+msgstr ""
+
+msgid "ctxcomponents_sponsorbox"
+msgstr ""
+
+msgid "ctxcomponents_sponsorbox_description"
+msgstr ""
+
+msgid "ctxcomponents_talk-status"
 msgstr ""
 
-msgid "creating Talk (Talk in_track Track %(linkto)s)"
+msgid "ctxcomponents_talk-status_description"
 msgstr ""
 
-msgid "date"
+msgid "ctxcomponents_talkstate"
+msgstr ""
+
+msgid "ctxcomponents_talkstate2"
+msgstr ""
+
+msgid "ctxcomponents_talkstate2_description"
+msgstr ""
+
+msgid "ctxcomponents_talkstate_description"
 msgstr ""
 
 msgctxt "Conference"
 msgid "description"
 msgstr ""
 
 msgctxt "Track"
@@ -386,29 +467,26 @@
 msgid "description_format"
 msgstr ""
 
 msgctxt "Talk"
 msgid "description_format"
 msgstr ""
 
-msgid "download icon"
-msgstr ""
-
 msgid "draft"
 msgstr ""
 
 msgid "end_on"
-msgstr "end on"
+msgstr ""
 
 msgctxt "Conference"
 msgid "end_on"
 msgstr ""
 
 msgid "end_time"
-msgstr "end time"
+msgstr ""
 
 msgctxt "Talk"
 msgid "end_time"
 msgstr ""
 
 msgid "facets_conference-facet"
 msgstr ""
@@ -424,57 +502,53 @@
 
 msgid "facets_track-facet"
 msgstr ""
 
 msgid "facets_track-facet_description"
 msgstr ""
 
-msgid "from_state"
+msgid "generate badges"
 msgstr ""
 
 msgid "has_attachments"
-msgstr "has attachments"
+msgstr ""
 
 msgctxt "Talk"
 msgid "has_attachments"
 msgstr ""
 
-msgctxt "Image"
-msgid "has_attachments_object"
-msgstr ""
-
 msgctxt "File"
 msgid "has_attachments_object"
 msgstr ""
 
 msgid "has_attachments_object"
 msgstr ""
 
 msgid "has_logo"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "has_logo"
 msgstr ""
 
-msgctxt "Image"
+msgctxt "File"
 msgid "has_logo_object"
 msgstr ""
 
 msgid "has_logo_object"
 msgstr ""
 
 msgid "in"
 msgstr ""
 
 msgid "in room"
 msgstr ""
 
 msgid "in_conf"
-msgstr "is in conference"
+msgstr ""
 
 msgctxt "Track"
 msgid "in_conf"
 msgstr ""
 
 msgctxt "Talk"
 msgid "in_conf"
@@ -484,15 +558,15 @@
 msgid "in_conf_object"
 msgstr ""
 
 msgid "in_conf_object"
 msgstr ""
 
 msgid "in_track"
-msgstr "is in track"
+msgstr ""
 
 msgctxt "Talk"
 msgid "in_track"
 msgstr ""
 
 msgctxt "Track"
 msgid "in_track_object"
@@ -500,14 +574,42 @@
 
 msgid "in_track_object"
 msgstr ""
 
 msgid "inreview"
 msgstr ""
 
+msgid "is_chair_at"
+msgstr ""
+
+msgctxt "CWUser"
+msgid "is_chair_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "is_chair_at_object"
+msgstr ""
+
+msgid "is_chair_at_object"
+msgstr ""
+
+msgid "is_reviewer_at"
+msgstr ""
+
+msgctxt "CWUser"
+msgid "is_reviewer_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "is_reviewer_at_object"
+msgstr ""
+
+msgid "is_reviewer_at_object"
+msgstr ""
+
 msgid "is_sponsor"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "is_sponsor"
 msgstr ""
 
@@ -545,33 +647,55 @@
 msgctxt "Talk"
 msgid "location"
 msgstr ""
 
 msgid "need correction"
 msgstr ""
 
+msgid "need more review"
+msgstr ""
+
 #, python-format
 msgid "on %(sdate)s from %(stime)s to %(etime)s"
 msgstr ""
 
 msgid "one day"
 msgstr ""
 
-msgid "people were registered"
+msgid "people plan to attend"
 msgstr ""
 
 msgid "planned"
 msgstr ""
 
 msgid "please contact us"
 msgstr ""
 
+msgid "propose to accept"
+msgstr ""
+
+msgid "propose to reject"
+msgstr ""
+
+msgid "redraft"
+msgstr ""
+
+msgid "reg_open"
+msgstr ""
+
+msgctxt "Conference"
+msgid "reg_open"
+msgstr ""
+
 msgid "reject talk"
 msgstr ""
 
+msgid "reject_pending"
+msgstr ""
+
 msgid "rejected"
 msgstr ""
 
 msgid "representing"
 msgstr ""
 
 msgctxt "CWUser"
@@ -621,86 +745,116 @@
 msgid "sponsoring_conf_object"
 msgstr ""
 
 msgid "sponsoring_conf_object"
 msgstr ""
 
 msgid "start_on"
-msgstr "start on"
+msgstr ""
 
 msgctxt "Conference"
 msgid "start_on"
 msgstr ""
 
 msgid "start_time"
-msgstr "start time"
+msgstr ""
 
 msgctxt "Talk"
 msgid "start_time"
 msgstr ""
 
 msgid "submit your work"
 msgstr ""
 
 msgid "submitted"
 msgstr ""
 
-msgid "swrc"
+msgid "swc"
 msgstr ""
 
 msgctxt "Talk"
 msgid "tags_object"
 msgstr ""
 
+msgid "take_place_at"
+msgstr ""
+
+msgctxt "Conference"
+msgid "take_place_at"
+msgstr ""
+
+msgctxt "PostalAddress"
+msgid "take_place_at_object"
+msgstr ""
+
+msgid "take_place_at_object"
+msgstr ""
+
 msgid "talk workflow"
 msgstr ""
 
 msgid "talkslist"
-msgstr "talks list"
+msgstr ""
 
 msgid "talksschedule"
-msgstr "talks schedule"
+msgstr ""
 
 msgctxt "Conference"
 msgid "title"
 msgstr ""
 
 msgctxt "SponsorShip"
 msgid "title"
 msgstr ""
 
 msgctxt "Track"
 msgid "title"
 msgstr ""
 
-msgctxt "Sponsor"
+msgctxt "Talk"
 msgid "title"
 msgstr ""
 
-msgctxt "Talk"
+msgctxt "Sponsor"
 msgid "title"
 msgstr ""
 
-msgid "to_state"
+msgid "trackinfo"
+msgstr ""
+
+msgid "tracktalkslist"
+msgstr ""
+
+msgid "tracktalksschedule"
+msgstr ""
+
+msgid "unique conference identifier for url"
 msgstr ""
 
 msgid "url"
 msgstr ""
 
 msgctxt "Sponsor"
 msgid "url"
 msgstr ""
 
+msgid "url_id"
+msgstr ""
+
+msgctxt "Conference"
+msgid "url_id"
+msgstr ""
+
 msgid "userconfschedule"
-msgstr "personal schedule"
+msgstr ""
 
 msgid "you are not anymore registered to attend this talk"
 msgstr ""
 
 msgid "you are now registered to attend this talk"
 msgstr ""
 
-#~ msgid "add Sponsor supports_conf Conference object"
-#~ msgstr "sponsor"
+msgid "your reviews"
+msgstr ""
 
-#~ msgid "add Sponsor supports_conf Conference subject"
-#~ msgstr "sponsor"
+msgid "your talks"
+msgstr ""
```

### Comparing `cubicweb-conference-0.4.2/views/actions.py` & `cubicweb-conference-1.0.0/cubicweb_conference/views/actions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,68 @@
-from cubicweb.web.action import LinkToEntityAction
-from cubicweb.web.views.actions import CopyAction, ModifyAction, AddNewAction, AddRelatedActions
-from cubicweb.selectors import implements, match_user_groups, score_entity, rql_condition
-from cubicweb.schema import ERQLExpression, RRQLExpression
-
-# actions
-
-class ConferenceAddTrackAction(LinkToEntityAction):
-    __regid__ = 'addtrack'
-    __select__ = (LinkToEntityAction.__select__ &
-                  implements('Conference') &
-                  match_user_groups('managers'))
-    etype = 'Track'
-    rtype = 'in_conf'
-    target = 'subject'
-    title = _('add Track in conference Conference object')
-
-# There is an "attend" relation. This relation is always visible so we have to
-# redefined the "modify" action for managers & owners.
-
-class ManagersAddAction(AddRelatedActions):
-     __select__ = AddRelatedActions.__select__ & match_user_groups('managers')
-
-class ManagersModifyAction(ModifyAction):
-    __select__ = ModifyAction.__select__ & match_user_groups('managers')
-
-class OwnersModifyAction(ModifyAction):
-    __select__ = (ModifyAction.__select__ &
-                  implements('Talk') &
-                  match_user_groups('owners') &
-                  score_entity(lambda x: x.state in ('draft', 'correction')))
-
-class AddDocument(LinkToEntityAction):
-    __regid__ = 'adddoc'
-    __select__ = (LinkToEntityAction.__select__ &
-                  implements('Talk') &
-                  (match_user_groups('managers') |
-                   (rql_condition('X owned_by U') &
-                    score_entity(lambda x: x.state in ('draft', 'correction')))))
-    target_etype = 'File'
-    rtype = 'has_attachments'
-    target = 'object'
-    title = _(u'add document to the talk')
+from cubicweb import _
+from cubicweb_web.action import Action, LinkToEntityAction
+from cubicweb_web.views import actions
+from cubicweb.predicates import (
+    one_line_rset,
+    has_permission,
+    is_instance,
+    match_user_groups,
+    rql_condition,
+    match_search_state,
+    partial_relation_possible,
+)
+
+
+# don't add action to add a talk in uicfg
+# (actionbox_appearsin_addmenu) because these actions must be display
+# only for managers, users have a specific button (confCallForPaper)
+# to add a talk
+class AddTalkInConferenceAction(LinkToEntityAction):
+    __regid__ = "addtalkinconf"
+    __select__ = (
+        match_search_state("normal")
+        & one_line_rset()
+        & partial_relation_possible(action="add", strict=False)
+        & is_instance("Conference")
+        & (match_user_groups("managers") | rql_condition("U is_chair_at X"))
+    )
+
+    title = _("add Talk in_conf Conference object")
+    target_etype = "Talk"
+    rtype = "in_conf"
+    role = "object"
+
+
+class AddTalkInTrackAction(LinkToEntityAction):
+    __regid__ = "addtalkintrack"
+    __select__ = (
+        match_search_state("normal")
+        & one_line_rset()
+        & partial_relation_possible(action="add", strict=False)
+        & is_instance("Track")
+        & (
+            match_user_groups("managers")
+            | rql_condition("U is_chair_at C, X is Track, X in_conf C")
+        )
+    )
+
+    title = _("add Talk in_track Track object")
+    target_etype = "Talk"
+    rtype = "in_track"
+    role = "object"
+
+
+class ModifyAction(actions.ModifyAction):
+    # remove has_permission('update') from __select__
+    # indeed user can set "attend" relation to a talk
+    # but this action is done with a specific button
+    # in the talk primary view
+    # we want to see the modify action only if user can
+    # update the entity
+    __select__ = Action.__select__ & one_line_rset() & has_permission("update")
 
-# score_entity
 
 def registration_callback(vreg):
-    vreg.unregister(CopyAction)
-    vreg.unregister(AddRelatedActions)
-    vreg.register(ManagersModifyAction)
-    vreg.register(AddDocument)
-    vreg.register_and_replace(OwnersModifyAction, ModifyAction)
-
+    vreg.unregister(actions.CopyAction)
+    vreg.register_and_replace(ModifyAction, actions.ModifyAction)
+    for entity in (AddTalkInConferenceAction, AddTalkInTrackAction):
+        vreg.register(entity)
```

### Comparing `cubicweb-conference-0.4.2/sobjects.py` & `cubicweb-conference-1.0.0/cubicweb_conference/sobjects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,172 +1,243 @@
-"""this contains the server-side objects"""
 import datetime
 
-from cubicweb.selectors import implements
-from cubicweb.server.hook import Hook, match_rtype
-from cubicweb.server.hook import match_rtype
-from cubicweb.sobjects.notification import (RecipientsFinder,
-                                            NotificationView,
-                                            StatusChangeMixIn)
+from logilab.common.registry import objectify_predicate
+
+from cubicweb import _
+from cubicweb.predicates import is_instance
+from cubicweb.server.hook import Hook, match_rtype, Operation, DataOperationMixIn
+from cubicweb.sobjects.notification import (
+    RecipientsFinder,
+    NotificationView,
+    StatusChangeMixIn,
+)
+
+from cubicweb_conference.utils import normalize_name
+
+
+def get_unique_url_id(execute, conference):
+    url_id = normalize_name(conference.title)
+    suffix = 0
+    new_url_id = url_id
+    while True:
+        rset = execute("Any C WHERE C url_id %(url)s", {"url": new_url_id})
+        if not rset:
+            return new_url_id
+        suffix += 1
+        new_url_id = f"{url_id}_{suffix}"
+
+
+class ConferenceUrlIdentifierHook(Hook):
+    """
+    If the conference has no url_id attribute, generate it automatically.
+    """
+
+    __regid__ = "conference-url-identifier-hook"
+    __select__ = Hook.__select__ & is_instance("Conference")
+    events = ("before_add_entity",)
+
+    def __call__(self):
+        if not self.entity.url_id:
+            url_id = get_unique_url_id(self._cw.execute, self.entity)
+            self.entity.cw_edited["url_id"] = url_id
+
 
 class AddTalkLeadHook(Hook):
-    __regid__ = 'add-talk-lead-hook'
-    __select__ = implements('Talk')
-    events = ('after_add_entity',)
+    __regid__ = "add-talk-lead-hook"
+    __select__ = is_instance("Talk")
+    events = ("after_add_entity",)
+
     def __call__(self):
         if not self._cw.is_internal_session:
             asession = self._cw
-            asession.execute('SET U leads X WHERE X eid %(x)s, U eid %(u)s, NOT U attend X',
-                             {'x': self.entity.eid, 'u': self._cw.user.eid}, 'x')
+            asession.execute(
+                "SET U leads X WHERE X eid %(x)s, U eid %(u)s, NOT U attend X",
+                {"x": self.entity.eid, "u": self._cw.user.eid},
+            )
+
 
 class LeadsHook(Hook):
     """
     Create relation attend on CWUser who leads a Talk:
     U leads T => U attend T
     """
-    __regid__ = 'lead-entails-attend-hook'
-    __select__ = Hook.__select__ & match_rtype('leads')
-    events = ('after_add_relation',)
+
+    __regid__ = "lead-entails-attend-hook"
+    __select__ = Hook.__select__ & match_rtype("leads")
+    events = ("after_add_relation",)
 
     def __call__(self):
         if not self._cw.is_internal_session:
             asession = self._cw
-            asession.execute('SET U attend X WHERE X eid %(x)s, U eid %(u)s, NOT U attend X',
-                             {'x': self.eidto, 'u': self.eidfrom}, 'x')
+            asession.execute(
+                "SET U attend X WHERE X eid %(x)s, U eid %(u)s, NOT U attend X",
+                {"x": self.eidto, "u": self.eidfrom},
+            )
+
+
+class SyncInConfOp(DataOperationMixIn, Operation):
+    def precommit_event(self):
+        for talk, track in self.get_data():
+            self.cnx.execute(
+                "SET T in_conf C WHERE T eid %(t)s, T in_track K, K in_conf C, K eid %(k)s, "
+                "NOT T in_conf C",
+                {"t": talk, "k": track},
+            )
+
 
 class InTrackHook(Hook):
     """
     When a Talk is added to a Track, automatically add it to the Conference:
     T in_track TR => T in_conf C
     """
-    __regid__ = 'in_track-entails-in_conf-hook'
-    __select__ = Hook.__select__ & match_rtype('in_track')
-    events = ('before_add_relation',)
 
-    def __call__(self):
-        if not self._cw.is_internal_session:
-            asession = self._cw
-            rql = 'Any C WHERE TR in_conf C, TR eid %(tr)s'
-            conf = asession.execute(rql, {'tr': self.eidto})
-            asession.execute('SET T in_conf C WHERE T eid %(t)s, C eid %(c)s, NOT T in_conf C',
-                             {'t': self.eidfrom, 'c': conf[0][0]})
-
-class InConfHook(Hook):
-    """
-    Remove already existing relation X in_conf C when trying to add a new
-    relation X in_conf C
-    """
-    __regid__ = 'switch-in_conf-hook'
-    __select__ = Hook.__select__ & match_rtype('in_conf')
-    events = ('before_add_relation',)
+    __regid__ = "in_track-entails-in_conf-hook"
+    __select__ = Hook.__select__ & match_rtype("in_track")
+    events = ("before_add_relation",)
 
     def __call__(self):
-         if not self._cw.is_internal_session:
-            asession = self._cw
-            rql = 'Any C WHERE X in_conf C, X eid %(x)s'
-            conf = asession.execute(rql, {'x': self.eidfrom})
-            if conf:
-                asession.execute('DELETE X in_conf C WHERE X eid %(x)s, C eid %(c)s',
-                                 {'x': self.eidfrom, 'c': conf[0][0]})
+        if not self._cw.is_internal_session:
+            SyncInConfOp.get_instance(self._cw).add_data((self.eidfrom, self.eidto))
 
 
-#-------------------
+# -------------------
 # Email notification
-#-------------------
+# -------------------
+
 
 class TalkNotificationView(NotificationView):
-    __select__ = NotificationView.__select__ & implements('Talk',)
+    __select__ = NotificationView.__select__ & is_instance(
+        "Talk",
+    )
 
     def context(self, **kwargs):
-        context = super(TalkNotificationView, self).context(**kwargs)
-        entity = self.cw_rset.complete_entity(0,0)
-        context.update({'talk_name': entity.title,
-                        'date': datetime.date.today().isoformat(),
-                        'firstname': entity.reverse_leads[0].firstname,
-                        'lastname': entity.reverse_leads[0].surname,
-                        'conference': entity.in_track[0].in_conf[0].title})
+        context = super().context(**kwargs)
+        entity = self.cw_rset.complete_entity(0, 0)
+        context.update(
+            {
+                "talk_name": entity.title,
+                "date": datetime.date.today().isoformat(),
+                "firstname": entity.reverse_leads[0].firstname,
+                "lastname": entity.reverse_leads[0].surname,
+                "conference": entity.in_conf[0].title,
+            }
+        )
         return context
 
     def recipients(self):
         recipients = []
         for finderid in self.recipients_finder:
-            finder = self._cw.vreg['components'].select(finderid, self._cw,
-                                                        rset= self.cw_rset)
+            finder = self._cw.vreg["services"].select(
+                finderid, self._cw, rset=self.cw_rset
+            )
             recipients += finder.recipients()
         return recipients
 
+
 class TalkAddRecipientsFinder(RecipientsFinder):
-    __select__ = RecipientsFinder.__select__ & implements('Talk',)
-    __regid__ = 'manager_finder'
+    __select__ = RecipientsFinder.__select__ & is_instance(
+        "Talk",
+    )
+    __regid__ = "manager_finder"
 
     @property
     def user_rql(self):
-        return ('Any U, E, A WHERE U is CWUser, U in_group N, N name "managers", U primary_email E, E address A')
+        return (
+            'Any U, E, A WHERE U is CWUser, U in_group N, N name "managers", U primary_email E,'
+            " E address A"
+        )
+
 
 class TalkUpdateRecipientsFinder(RecipientsFinder):
-    __select__ = RecipientsFinder.__select__ & implements('Talk',)
-    __regid__ = 'interested_by_finder'
+    __select__ = RecipientsFinder.__select__ & is_instance(
+        "Talk",
+    )
+    __regid__ = "interested_by_finder"
 
     @property
     def user_rql(self):
-        return ('Any U, E, A WHERE X eid %(eid)s, (U reviews X) OR (U leads X), U primary_email E, E address A' %
-                {'eid':  self.cw_rset[0][0]})
+        return (
+            "Any U, E, A WHERE X eid %(eid)s, EXISTS(U reviews X) "
+            "OR EXISTS(U leads X), U primary_email E, E address A"
+            % {"eid": self.cw_rset[0][0]}
+        )
+
 
 class TalkAdd(TalkNotificationView):
-    """  Send an email to managers after a talk creation
-    """
-    __regid__ = 'notif_after_add_entity'
+    """Send an email to managers after a talk creation"""
+
+    __regid__ = "notif_after_add_entity"
 
-    recipients_finder = ('manager_finder',)
+    recipients_finder = ("manager_finder",)
 
-    content = _(u""
-                u"Dear %(firstname)s %(lastname)s,\n"
-                u"\n"
-                u"The talk '%(talk_name)s' was added on %(date)s.\n"
-                u"\n"
-                u"Sincerely,\n"
-                u"\n"
-                u"--\n"
-                u"The %(conference)s organizing committee.\n")
+    content = _(
+        ""
+        "Dear %(firstname)s %(lastname)s,\n"
+        "\n"
+        "The talk '%(talk_name)s' was added on %(date)s.\n"
+        "\n"
+        "Sincerely,\n"
+        "\n"
+        "--\n"
+        "The %(conference)s organizing committee.\n"
+    )
 
     def subject(self):
-        entity = self.cw_rset.get_entity(0,0)
-        return self._cw._('[%s] a talk was added.') % entity.in_track[0].in_conf[0].title
+        entity = self.cw_rset.get_entity(0, 0)
+        return self._cw._("[%s] a talk was added") % entity.in_conf[0].title
 
-class TalkUpdate(TalkNotificationView):
-    __regid__ = 'notif_after_update_entity'
 
-    recipients_finder = ('manager_finder', 'interested_by_finder',)
+# XXX move to framework ?
+# XXX why metaattrsupdate is updated at before_update_entity ?
+@objectify_predicate
+def entity_really_edited(cls, req, rset=None, **kwargs):
+    # when the status of an entity changes, the modification_date of the entity changes too
+    # in case of talks, don't call talkupdate if only modification_date attribute has changed
+    entity = rset.get_entity(0, 0)
+    if getattr(entity, "cw_edited", None) is None:
+        return 0
+    if len(entity.cw_edited) == 1 and "modification_date" in entity.cw_edited:
+        return 0
+    return 1
+
 
-    content = _(u""
-                u"Dear %(firstname)s %(lastname)s,\n"
-                u"\n"
-                u"The talk '%(talk_name)s' was modified on %(date)s.\n"
-                u"\n"
-                u"Sincerely,\n"
-                u"\n"
-                u"--\n"
-                u"The %(conference)s organizing committee.\n")
+class TalkUpdate(TalkNotificationView):
+    __regid__ = "notif_after_update_entity"
+    recipients_finder = (
+        "manager_finder",
+        "interested_by_finder",
+    )
+    __select__ = TalkNotificationView.__select__ & entity_really_edited()
+
+    content = _(
+        ""
+        "Dear %(firstname)s %(lastname)s,\n"
+        "\n"
+        "The talk '%(talk_name)s' was modified on %(date)s.\n"
+        "\n"
+        "Sincerely,\n"
+        "\n"
+        "--\n"
+        "The %(conference)s organizing committee.\n"
+    )
 
     def subject(self):
-        entity = self.cw_rset.get_entity(0,0)
-        return self._cw._('[%s] a talk was added.') % entity.in_track[0].in_conf[0].title
+        entity = self.cw_rset.get_entity(0, 0)
+        return self._cw._("[%s] a talk was updated") % entity.in_conf[0].title
 
-class TalkStatusUpdate(StatusChangeMixIn, TalkNotificationView):
-    """
-    """
 
-    recipients_finder = ('manager_finder', 'interested_by_finder')
+class TalkStatusUpdate(StatusChangeMixIn, TalkNotificationView):
+    recipients_finder = ("manager_finder", "interested_by_finder")
 
-    content = _(u""
-                u"Dear user,\n\n"
-                u"The '%(title)s' status was updated from '%(previous_state)s' to '%(current_state)s'.\n\n"
-                u"Sincerely,\n"
-                u"\n"
-                u"--\n"
-                u"The conference organizing committee.\n")
+    content = _(
+        ""
+        "Dear user,\n\n"
+        "The '%(title)s' status was updated from '%(previous_state)s' to '%(current_state)s'.\n\n"
+        "Sincerely,\n"
+        "\n"
+        "--\n"
+        "The conference organizing committee.\n"
+    )
 
     def subject(self):
-        entity = self.cw_rset.get_entity(0,0)
-        return _(u'[%s] talk status was updated' % entity.in_track[0].in_conf[0].title)
-
-
+        entity = self.cw_rset.get_entity(0, 0)
+        return _(f"[{entity.in_track[0].in_conf[0].title}] talk status was updated")
```

### Comparing `cubicweb-conference-0.4.2/data/stat.png` & `cubicweb-conference-1.0.0/cubicweb_conference/data/stat.png`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-0.4.2/data/noattend.jpeg` & `cubicweb-conference-1.0.0/cubicweb_conference/data/noattend.jpeg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-0.4.2/data/icon_pen.gif` & `cubicweb-conference-1.0.0/cubicweb_conference/data/icon_pen.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-0.4.2/data/attend.jpeg` & `cubicweb-conference-1.0.0/cubicweb_conference/data/attend.jpeg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-0.4.2/migration/postcreate.py` & `cubicweb-conference-1.0.0/cubicweb_conference/migration/postcreate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,115 @@
 # postcreate script. You could setup a workflow here for example
 
-_ = unicode
+from cubicweb import _
 
-moderators = add_entity('CWGroup', name=u"moderators")
+# constants used for permissions
 
-set_property('boxes.blog_summary_box.visible', u'')
+TALK_CHAIR = "U is_chair_at C, X in_conf C, X is Talk"
+CONF_CHAIR = "U is_chair_at X"
+REVIEWER = "U is_reviewer_at C, X in_conf C"
+OWNER_CALL_OPEN = "X owned_by U, X in_conf C, C call_open True"
+MANAGER = ("managers",)
+OWNER_MANAGER = ("owners", "managers")
 
 # Conference Workflow
 
+
 def define_conference_workflow():
-    twf = add_workflow(_('conference workflow'), 'Conference')
-    planned = twf.add_state(_('planned'), initial=True)
-    scheduled = twf.add_state(_('scheduled'))
-    archived = twf.add_state(_('archived'))
-    twf.add_transition(_('schedule'), (planned,), scheduled,
-                       ('managers',),)
-    twf.add_transition(_('archive'), (scheduled,), archived,
-                       ('managers',),)
+    twf = add_workflow(_("conference workflow"), "Conference")
+    planned = twf.add_state(_("planned"), initial=True)
+    scheduled = twf.add_state(_("scheduled"))
+    archived = twf.add_state(_("archived"))
+    twf.add_transition(
+        _("schedule"), (planned,), scheduled, MANAGER, conditions=CONF_CHAIR
+    )
+    twf.add_transition(
+        _("archive"), (scheduled,), archived, MANAGER, conditions=CONF_CHAIR
+    )
+
 
 define_conference_workflow()
 
 # Talk Workflow
 
-talk_states = rql('Any T, N ORDERBY T WHERE T in_state S, S name N, T is Talk').rows
-
-rql('DELETE Workflow WF WHERE WF workflow_of X, X name "Talk"')
 
 def define_talk_workflow():
-    twf = add_workflow(_('talk workflow'), 'Talk')
-    draft = twf.add_state(_('draft'), initial=True)
-    submitted = twf.add_state(_('submitted'))
-    correction = twf.add_state(_('correction'))
-    inreview = twf.add_state(_('inreview'))
-    accepted = twf.add_state(_('accepted'))
-    rejected = twf.add_state(_('rejected'))
-    twf.add_transition(_('draft'), (draft,), submitted,
-                       ('owners',))
-    twf.add_transition(_('send to reviewer'), (submitted,), inreview,
-                       ('managers',))
-    twf.add_transition(_('need correction'), (inreview,), correction,
-                       ('managers',), conditions=('U reviews X',))
-    twf.add_transition(_('resend to reviewer'), (correction,), inreview,
-                       ('owners',))
-    twf.add_transition(_('accept talk'), (inreview,), accepted,
-                       ('managers',), conditions=('U reviews X',))
-    twf.add_transition(_('reject talk'), (inreview,), rejected,
-                       ('managers',), conditions=('U reviews X',))
+    twf = add_workflow(_("talk workflow"), "Talk")
+    draft = twf.add_state(_("draft"), initial=True)
+    submitted = twf.add_state(_("submitted"))
+    correction = twf.add_state(_("correction"))
+    inreview = twf.add_state(_("inreview"))
+    accept_pending = twf.add_state(_("accept_pending"))
+    reject_pending = twf.add_state(_("reject_pending"))
+    accepted = twf.add_state(_("accepted"))
+    rejected = twf.add_state(_("rejected"))
+    twf.add_transition(
+        _("submit your work"),
+        (draft,),
+        submitted,
+        MANAGER,
+        conditions=(TALK_CHAIR, OWNER_CALL_OPEN),
+    )
+    twf.add_transition(
+        _("redraft"),
+        (submitted,),
+        draft,
+        MANAGER,
+        conditions=(TALK_CHAIR, OWNER_CALL_OPEN),
+    )
+    twf.add_transition(
+        _("send to reviewer"), (submitted,), inreview, MANAGER, conditions=TALK_CHAIR
+    )
+    twf.add_transition(
+        _("need correction"),
+        (inreview,),
+        correction,
+        MANAGER,
+        conditions=(REVIEWER, TALK_CHAIR),
+    )
+    twf.add_transition(
+        _("resend to reviewer"),
+        (correction,),
+        inreview,
+        OWNER_MANAGER,
+        conditions=TALK_CHAIR,
+    )
+    twf.add_transition(
+        _("propose to accept"),
+        (inreview,),
+        accept_pending,
+        MANAGER,
+        conditions=(REVIEWER, TALK_CHAIR),
+    )
+    twf.add_transition(
+        _("propose to reject"),
+        (inreview,),
+        reject_pending,
+        MANAGER,
+        conditions=(REVIEWER, TALK_CHAIR),
+    )
+    twf.add_transition(
+        _("need more review"),
+        (accept_pending, reject_pending),
+        inreview,
+        MANAGER,
+        conditions=(REVIEWER, TALK_CHAIR),
+    )
+    twf.add_transition(
+        _("accept talk"),
+        (accept_pending, reject_pending),
+        accepted,
+        MANAGER,
+        conditions=TALK_CHAIR,
+    )
+    twf.add_transition(
+        _("reject talk"),
+        (reject_pending, accept_pending),
+        rejected,
+        MANAGER,
+        conditions=TALK_CHAIR,
+    )
+
 
 define_talk_workflow()
 
 commit()
```

