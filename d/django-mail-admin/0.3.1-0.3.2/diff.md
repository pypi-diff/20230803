# Comparing `tmp/django_mail_admin-0.3.1.tar.gz` & `tmp/django_mail_admin-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mail_admin-0.3.1.tar", last modified: Thu May  5 07:29:17 2022, max compression
+gzip compressed data, was "django_mail_admin-0.3.2.tar", last modified: Thu Aug  3 11:50:35 2023, max compression
```

## Comparing `django_mail_admin-0.3.1.tar` & `django_mail_admin-0.3.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.699481 django_mail_admin-0.3.1/
--rw-r--r--   0 delneg     (501) staff       (20)      154 2017-11-02 22:45:55.000000 django_mail_admin-0.3.1/AUTHORS.rst
--rw-r--r--   0 delneg     (501) staff       (20)     3284 2017-11-02 22:45:55.000000 django_mail_admin-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 delneg     (501) staff       (20)     1187 2022-05-05 07:28:48.000000 django_mail_admin-0.3.1/HISTORY.rst
--rw-r--r--   0 delneg     (501) staff       (20)     1075 2017-11-02 22:45:55.000000 django_mail_admin-0.3.1/LICENSE
--rw-r--r--   0 delneg     (501) staff       (20)      185 2017-11-02 22:45:55.000000 django_mail_admin-0.3.1/MANIFEST.in
--rw-r--r--   0 delneg     (501) staff       (20)     8692 2022-05-05 07:29:17.699639 django_mail_admin-0.3.1/PKG-INFO
--rw-r--r--   0 delneg     (501) staff       (20)     7492 2020-10-18 21:42:27.000000 django_mail_admin-0.3.1/README.rst
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.688069 django_mail_admin-0.3.1/django_mail_admin/
--rw-r--r--   0 delneg     (501) staff       (20)       90 2022-05-05 07:28:55.000000 django_mail_admin-0.3.1/django_mail_admin/__init__.py
--rw-r--r--   0 delneg     (501) staff       (20)    11036 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/admin.py
--rw-r--r--   0 delneg     (501) staff       (20)      217 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/apps.py
--rw-r--r--   0 delneg     (501) staff       (20)     2935 2020-09-29 09:22:09.000000 django_mail_admin-0.3.1/django_mail_admin/backends.py
--rw-r--r--   0 delneg     (501) staff       (20)      720 2017-11-04 00:56:57.000000 django_mail_admin-0.3.1/django_mail_admin/cache.py
--rw-r--r--   0 delneg     (501) staff       (20)     1146 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/connections.py
--rw-r--r--   0 delneg     (501) staff       (20)     1569 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/fields.py
--rw-r--r--   0 delneg     (501) staff       (20)      322 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/forms.py
--rw-r--r--   0 delneg     (501) staff       (20)     3205 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/google_utils.py
--rw-r--r--   0 delneg     (501) staff       (20)     4594 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/lockfile.py
--rw-r--r--   0 delneg     (501) staff       (20)     1114 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/logutils.py
--rw-r--r--   0 delneg     (501) staff       (20)     9296 2020-10-18 21:42:27.000000 django_mail_admin-0.3.1/django_mail_admin/mail.py
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.690531 django_mail_admin-0.3.1/django_mail_admin/management/
--rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-13 12:53:46.000000 django_mail_admin-0.3.1/django_mail_admin/management/__init__.py
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.691747 django_mail_admin-0.3.1/django_mail_admin/management/commands/
--rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-13 12:53:57.000000 django_mail_admin-0.3.1/django_mail_admin/management/commands/__init__.py
--rw-r--r--   0 delneg     (501) staff       (20)     1925 2018-06-02 21:06:16.000000 django_mail_admin-0.3.1/django_mail_admin/management/commands/cleanup_email.py
--rw-r--r--   0 delneg     (501) staff       (20)      921 2018-01-07 12:28:05.000000 django_mail_admin-0.3.1/django_mail_admin/management/commands/get_new_mail.py
--rw-r--r--   0 delneg     (501) staff       (20)     2077 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/management/commands/send_queued_mail.py
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.692900 django_mail_admin-0.3.1/django_mail_admin/migrations/
--rw-r--r--   0 delneg     (501) staff       (20)    12858 2017-12-29 00:48:26.000000 django_mail_admin-0.3.1/django_mail_admin/migrations/0001_initial.py
--rw-r--r--   0 delneg     (501) staff       (20)      707 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/migrations/0002_auto_20190709_1139.py
--rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-13 12:31:50.000000 django_mail_admin-0.3.1/django_mail_admin/migrations/__init__.py
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.694998 django_mail_admin-0.3.1/django_mail_admin/models/
--rw-r--r--   0 delneg     (501) staff       (20)      123 2017-11-16 18:54:44.000000 django_mail_admin-0.3.1/django_mail_admin/models/__init__.py
--rw-r--r--   0 delneg     (501) staff       (20)    15918 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/models/configurations.py
--rw-r--r--   0 delneg     (501) staff       (20)    12093 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/models/incoming.py
--rw-r--r--   0 delneg     (501) staff       (20)      922 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/models/logs.py
--rw-r--r--   0 delneg     (501) staff       (20)     9827 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/models/outgoing.py
--rw-r--r--   0 delneg     (501) staff       (20)     1880 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/models/templates.py
--rw-r--r--   0 delneg     (501) staff       (20)     3827 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/settings.py
--rw-r--r--   0 delneg     (501) staff       (20)      190 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/signals.py
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.699157 django_mail_admin-0.3.1/django_mail_admin/transports/
--rw-r--r--   0 delneg     (501) staff       (20)      490 2017-11-03 09:43:30.000000 django_mail_admin-0.3.1/django_mail_admin/transports/__init__.py
--rw-r--r--   0 delneg     (501) staff       (20)      160 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/babyl.py
--rw-r--r--   0 delneg     (501) staff       (20)      288 2017-11-16 19:05:37.000000 django_mail_admin-0.3.1/django_mail_admin/transports/base.py
--rw-r--r--   0 delneg     (501) staff       (20)      645 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/generic.py
--rw-r--r--   0 delneg     (501) staff       (20)     2042 2017-11-03 10:12:12.000000 django_mail_admin-0.3.1/django_mail_admin/transports/gmail.py
--rw-r--r--   0 delneg     (501) staff       (20)     4435 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/imap.py
--rw-r--r--   0 delneg     (501) staff       (20)      242 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/maildir.py
--rw-r--r--   0 delneg     (501) staff       (20)      157 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/mbox.py
--rw-r--r--   0 delneg     (501) staff       (20)      151 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/mh.py
--rw-r--r--   0 delneg     (501) staff       (20)      157 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/transports/mmdf.py
--rw-r--r--   0 delneg     (501) staff       (20)     1345 2017-11-03 09:50:40.000000 django_mail_admin-0.3.1/django_mail_admin/transports/pop3.py
--rw-r--r--   0 delneg     (501) staff       (20)       75 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/urls.py
--rw-r--r--   0 delneg     (501) staff       (20)     4522 2019-07-11 09:00:11.000000 django_mail_admin-0.3.1/django_mail_admin/utils.py
--rw-r--r--   0 delneg     (501) staff       (20)     1737 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/django_mail_admin/validators.py
--rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-02 22:45:55.000000 django_mail_admin-0.3.1/django_mail_admin/views.py
-drwxr-xr-x   0 delneg     (501) staff       (20)        0 2022-05-05 07:29:17.690306 django_mail_admin-0.3.1/django_mail_admin.egg-info/
--rw-r--r--   0 delneg     (501) staff       (20)     8692 2022-05-05 07:29:17.000000 django_mail_admin-0.3.1/django_mail_admin.egg-info/PKG-INFO
--rw-r--r--   0 delneg     (501) staff       (20)     1895 2022-05-05 07:29:17.000000 django_mail_admin-0.3.1/django_mail_admin.egg-info/SOURCES.txt
--rw-r--r--   0 delneg     (501) staff       (20)        1 2022-05-05 07:29:17.000000 django_mail_admin-0.3.1/django_mail_admin.egg-info/dependency_links.txt
--rw-r--r--   0 delneg     (501) staff       (20)        1 2022-05-05 07:29:17.000000 django_mail_admin-0.3.1/django_mail_admin.egg-info/not-zip-safe
--rw-r--r--   0 delneg     (501) staff       (20)       42 2022-05-05 07:29:17.000000 django_mail_admin-0.3.1/django_mail_admin.egg-info/requires.txt
--rw-r--r--   0 delneg     (501) staff       (20)       18 2022-05-05 07:29:17.000000 django_mail_admin-0.3.1/django_mail_admin.egg-info/top_level.txt
--rw-r--r--   0 delneg     (501) staff       (20)      335 2022-05-05 07:29:17.700309 django_mail_admin-0.3.1/setup.cfg
--rwxr-xr-x   0 delneg     (501) staff       (20)     2697 2022-05-05 07:28:16.000000 django_mail_admin-0.3.1/setup.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.229139 django_mail_admin-0.3.2/
+-rw-r--r--   0 delneg     (501) staff       (20)      154 2017-11-02 22:45:55.000000 django_mail_admin-0.3.2/AUTHORS.rst
+-rw-r--r--   0 delneg     (501) staff       (20)     3284 2017-11-02 22:45:55.000000 django_mail_admin-0.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 delneg     (501) staff       (20)     1187 2022-05-05 07:28:48.000000 django_mail_admin-0.3.2/HISTORY.rst
+-rw-r--r--   0 delneg     (501) staff       (20)     1075 2017-11-02 22:45:55.000000 django_mail_admin-0.3.2/LICENSE
+-rw-r--r--   0 delneg     (501) staff       (20)      185 2017-11-02 22:45:55.000000 django_mail_admin-0.3.2/MANIFEST.in
+-rw-------   0 delneg     (501) staff       (20)     8743 2023-08-03 11:50:35.229265 django_mail_admin-0.3.2/PKG-INFO
+-rw-r--r--   0 delneg     (501) staff       (20)     7492 2023-08-03 11:50:04.000000 django_mail_admin-0.3.2/README.rst
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.224317 django_mail_admin-0.3.2/django_mail_admin/
+-rw-r--r--   0 delneg     (501) staff       (20)       90 2023-08-03 11:50:04.000000 django_mail_admin-0.3.2/django_mail_admin/__init__.py
+-rw-r--r--   0 delneg     (501) staff       (20)    12070 2023-08-03 11:50:04.000000 django_mail_admin-0.3.2/django_mail_admin/admin.py
+-rw-r--r--   0 delneg     (501) staff       (20)      271 2023-08-03 11:50:04.000000 django_mail_admin-0.3.2/django_mail_admin/apps.py
+-rw-r--r--   0 delneg     (501) staff       (20)     2935 2020-09-29 09:22:09.000000 django_mail_admin-0.3.2/django_mail_admin/backends.py
+-rw-r--r--   0 delneg     (501) staff       (20)      720 2017-11-04 00:56:57.000000 django_mail_admin-0.3.2/django_mail_admin/cache.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1146 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/connections.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1569 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/fields.py
+-rw-r--r--   0 delneg     (501) staff       (20)      322 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/forms.py
+-rw-r--r--   0 delneg     (501) staff       (20)     3205 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/google_utils.py
+-rw-r--r--   0 delneg     (501) staff       (20)     4594 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/lockfile.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1114 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/logutils.py
+-rw-r--r--   0 delneg     (501) staff       (20)     9296 2020-10-18 21:42:27.000000 django_mail_admin-0.3.2/django_mail_admin/mail.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.225259 django_mail_admin-0.3.2/django_mail_admin/management/
+-rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-13 12:53:46.000000 django_mail_admin-0.3.2/django_mail_admin/management/__init__.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.225790 django_mail_admin-0.3.2/django_mail_admin/management/commands/
+-rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-13 12:53:57.000000 django_mail_admin-0.3.2/django_mail_admin/management/commands/__init__.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1925 2018-06-02 21:06:16.000000 django_mail_admin-0.3.2/django_mail_admin/management/commands/cleanup_email.py
+-rw-r--r--   0 delneg     (501) staff       (20)      921 2018-01-07 12:28:05.000000 django_mail_admin-0.3.2/django_mail_admin/management/commands/get_new_mail.py
+-rw-r--r--   0 delneg     (501) staff       (20)     2077 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/management/commands/send_queued_mail.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.226218 django_mail_admin-0.3.2/django_mail_admin/migrations/
+-rw-r--r--   0 delneg     (501) staff       (20)    12858 2017-12-29 00:48:26.000000 django_mail_admin-0.3.2/django_mail_admin/migrations/0001_initial.py
+-rw-r--r--   0 delneg     (501) staff       (20)      707 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/migrations/0002_auto_20190709_1139.py
+-rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-13 12:31:50.000000 django_mail_admin-0.3.2/django_mail_admin/migrations/__init__.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.227362 django_mail_admin-0.3.2/django_mail_admin/models/
+-rw-r--r--   0 delneg     (501) staff       (20)      123 2017-11-16 18:54:44.000000 django_mail_admin-0.3.2/django_mail_admin/models/__init__.py
+-rw-r--r--   0 delneg     (501) staff       (20)    15918 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/models/configurations.py
+-rw-r--r--   0 delneg     (501) staff       (20)    12093 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/models/incoming.py
+-rw-r--r--   0 delneg     (501) staff       (20)      922 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/models/logs.py
+-rw-r--r--   0 delneg     (501) staff       (20)     9827 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/models/outgoing.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1880 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/models/templates.py
+-rw-r--r--   0 delneg     (501) staff       (20)     3827 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/settings.py
+-rw-r--r--   0 delneg     (501) staff       (20)      190 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/signals.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.228988 django_mail_admin-0.3.2/django_mail_admin/transports/
+-rw-r--r--   0 delneg     (501) staff       (20)      490 2017-11-03 09:43:30.000000 django_mail_admin-0.3.2/django_mail_admin/transports/__init__.py
+-rw-r--r--   0 delneg     (501) staff       (20)      160 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/babyl.py
+-rw-r--r--   0 delneg     (501) staff       (20)      288 2017-11-16 19:05:37.000000 django_mail_admin-0.3.2/django_mail_admin/transports/base.py
+-rw-r--r--   0 delneg     (501) staff       (20)      645 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/generic.py
+-rw-r--r--   0 delneg     (501) staff       (20)     2042 2017-11-03 10:12:12.000000 django_mail_admin-0.3.2/django_mail_admin/transports/gmail.py
+-rw-r--r--   0 delneg     (501) staff       (20)     4435 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/imap.py
+-rw-r--r--   0 delneg     (501) staff       (20)      242 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/maildir.py
+-rw-r--r--   0 delneg     (501) staff       (20)      157 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/mbox.py
+-rw-r--r--   0 delneg     (501) staff       (20)      151 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/mh.py
+-rw-r--r--   0 delneg     (501) staff       (20)      157 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/transports/mmdf.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1345 2017-11-03 09:50:40.000000 django_mail_admin-0.3.2/django_mail_admin/transports/pop3.py
+-rw-r--r--   0 delneg     (501) staff       (20)       75 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/urls.py
+-rw-r--r--   0 delneg     (501) staff       (20)     4522 2019-07-11 09:00:11.000000 django_mail_admin-0.3.2/django_mail_admin/utils.py
+-rw-r--r--   0 delneg     (501) staff       (20)     1737 2022-05-05 07:28:16.000000 django_mail_admin-0.3.2/django_mail_admin/validators.py
+-rw-r--r--   0 delneg     (501) staff       (20)        0 2017-11-02 22:45:55.000000 django_mail_admin-0.3.2/django_mail_admin/views.py
+drwx------   0 delneg     (501) staff       (20)        0 2023-08-03 11:50:35.225123 django_mail_admin-0.3.2/django_mail_admin.egg-info/
+-rw-------   0 delneg     (501) staff       (20)     8743 2023-08-03 11:50:34.000000 django_mail_admin-0.3.2/django_mail_admin.egg-info/PKG-INFO
+-rw-------   0 delneg     (501) staff       (20)     1895 2023-08-03 11:50:34.000000 django_mail_admin-0.3.2/django_mail_admin.egg-info/SOURCES.txt
+-rw-------   0 delneg     (501) staff       (20)        1 2023-08-03 11:50:34.000000 django_mail_admin-0.3.2/django_mail_admin.egg-info/dependency_links.txt
+-rw-------   0 delneg     (501) staff       (20)        1 2023-08-03 11:50:34.000000 django_mail_admin-0.3.2/django_mail_admin.egg-info/not-zip-safe
+-rw-------   0 delneg     (501) staff       (20)       42 2023-08-03 11:50:34.000000 django_mail_admin-0.3.2/django_mail_admin.egg-info/requires.txt
+-rw-------   0 delneg     (501) staff       (20)       18 2023-08-03 11:50:34.000000 django_mail_admin-0.3.2/django_mail_admin.egg-info/top_level.txt
+-rw-r--r--   0 delneg     (501) staff       (20)      335 2023-08-03 11:50:35.229727 django_mail_admin-0.3.2/setup.cfg
+-rwxr-xr-x   0 delneg     (501) staff       (20)     2747 2023-08-03 11:50:04.000000 django_mail_admin-0.3.2/setup.py
```

### Comparing `django_mail_admin-0.3.1/CONTRIBUTING.rst` & `django_mail_admin-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/HISTORY.rst` & `django_mail_admin-0.3.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/LICENSE` & `django_mail_admin-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/PKG-INFO` & `django_mail_admin-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_mail_admin
-Version: 0.3.1
+Version: 0.3.2
 Summary: The one and only django app to receive & send mail with templates and multiple configurations.
 Home-page: https://github.com/delneg/django_mail_admin
 Author: Denis Bobrov
 Author-email: delneg@yandex.ru
 License: MIT
 Keywords: django_mail_admin
 Platform: UNKNOWN
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gmail
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============================
 Django Mail Admin
 =============================
@@ -68,15 +69,15 @@
 
 * `django >= 1.9 <http://djangoproject.com/>`_
 * `django-jsonfield <https://github.com/bradjasper/django-jsonfield>`_
 
 Documentation
 -------------
 
-The full documentation is at https://django_mail_admin.readthedocs.io.
+The full documentation is at https://django-mail-admin.readthedocs.io.
 
 Quickstart
 ----------
 
 **Q**: What versions of Django/Python are supported?
 **A**: Take a look at https://travis-ci.org/delneg/django_mail_admin
```

### Comparing `django_mail_admin-0.3.1/README.rst` & `django_mail_admin-0.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 * `django >= 1.9 <http://djangoproject.com/>`_
 * `django-jsonfield <https://github.com/bradjasper/django-jsonfield>`_
 
 Documentation
 -------------
 
-The full documentation is at https://django_mail_admin.readthedocs.io.
+The full documentation is at https://django-mail-admin.readthedocs.io.
 
 Quickstart
 ----------
 
 **Q**: What versions of Django/Python are supported?
 **A**: Take a look at https://travis-ci.org/delneg/django_mail_admin
```

### Comparing `django_mail_admin-0.3.1/django_mail_admin/admin.py` & `django_mail_admin-0.3.2/django_mail_admin/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 
 from django.conf import settings
 from django.contrib import admin
 from django.contrib import messages
 from django.forms.widgets import TextInput
+from django.http import HttpResponse
 from django.shortcuts import reverse
+from django.template import Context
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from django_mail_admin.models import Mailbox, IncomingAttachment, IncomingEmail, TemplateVariable, OutgoingEmail, \
     Outbox, EmailTemplate, STATUS, Log, Attachment
 from django_mail_admin.signals import message_received
@@ -244,14 +246,35 @@
 
 
     MailboxAdmin.get_row_actions = get_row_actions
 
 
 class EmailTemplateAdmin(admin.ModelAdmin):
     list_display = ('name', 'description', 'subject')
+    readonly_fields = ['preview_template_field']
+
+    def preview_template_field(self, o):
+        if o.id:
+            url = reverse('admin:django_mail_admin_emailtemplate_change', kwargs={'object_id': o.pk})
+            url = url + '?preview_template=true'
+            return mark_safe(f'<a href="{url}" target="_blank">Preview this template</a>')
+        else:
+            return '---'
+    preview_template_field.short_description='Preview'
+
+    def change_view(self, request, object_id, form_url='', extra_context=None):
+        if request.GET.get('preview_template', '').lower()=='true':
+            return self.preview_template_view(request, object_id)
+        return super().change_view(request, object_id, form_url, extra_context)
+
+    def preview_template_view(self, request, object_id):
+        obj = self.get_object(request, object_id)
+        content = obj.render_html_text(Context())
+        return HttpResponse(content, content_type='text/html')
+
 
 
 class TemplateVariableInline(admin.TabularInline):
     model = TemplateVariable
     extra = 1
 
 
@@ -271,21 +294,21 @@
 
 
 class CommaSeparatedEmailWidget(TextInput):
     def __init__(self, *args, **kwargs):
         super(CommaSeparatedEmailWidget, self).__init__(*args, **kwargs)
         self.attrs.update({'class': 'vTextField'})
 
-    def _format_value(self, value):
+    def format_value(self, value):
         # If the value is a string wrap it in a list so it does not get sliced.
         if not value:
             return ''
         if isinstance(value, str):
             value = [value, ]
-        return ','.join([item for item in value])
+        return ', '.join([item for item in value])
 
 
 def requeue(modeladmin, request, queryset):
     """An admin action to requeue emails."""
     queryset.update(status=STATUS.queued)
```

### Comparing `django_mail_admin-0.3.1/django_mail_admin/backends.py` & `django_mail_admin-0.3.2/django_mail_admin/backends.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/cache.py` & `django_mail_admin-0.3.2/django_mail_admin/cache.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/connections.py` & `django_mail_admin-0.3.2/django_mail_admin/connections.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/fields.py` & `django_mail_admin-0.3.2/django_mail_admin/fields.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/google_utils.py` & `django_mail_admin-0.3.2/django_mail_admin/google_utils.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/lockfile.py` & `django_mail_admin-0.3.2/django_mail_admin/lockfile.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/logutils.py` & `django_mail_admin-0.3.2/django_mail_admin/logutils.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/mail.py` & `django_mail_admin-0.3.2/django_mail_admin/mail.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/management/commands/cleanup_email.py` & `django_mail_admin-0.3.2/django_mail_admin/management/commands/cleanup_email.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/management/commands/get_new_mail.py` & `django_mail_admin-0.3.2/django_mail_admin/management/commands/get_new_mail.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/management/commands/send_queued_mail.py` & `django_mail_admin-0.3.2/django_mail_admin/management/commands/send_queued_mail.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/migrations/0001_initial.py` & `django_mail_admin-0.3.2/django_mail_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/migrations/0002_auto_20190709_1139.py` & `django_mail_admin-0.3.2/django_mail_admin/migrations/0002_auto_20190709_1139.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/models/configurations.py` & `django_mail_admin-0.3.2/django_mail_admin/models/configurations.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/models/incoming.py` & `django_mail_admin-0.3.2/django_mail_admin/models/incoming.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/models/logs.py` & `django_mail_admin-0.3.2/django_mail_admin/models/logs.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/models/outgoing.py` & `django_mail_admin-0.3.2/django_mail_admin/models/outgoing.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/models/templates.py` & `django_mail_admin-0.3.2/django_mail_admin/models/templates.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/settings.py` & `django_mail_admin-0.3.2/django_mail_admin/settings.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/transports/generic.py` & `django_mail_admin-0.3.2/django_mail_admin/transports/generic.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/transports/gmail.py` & `django_mail_admin-0.3.2/django_mail_admin/transports/gmail.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/transports/imap.py` & `django_mail_admin-0.3.2/django_mail_admin/transports/imap.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/transports/pop3.py` & `django_mail_admin-0.3.2/django_mail_admin/transports/pop3.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/utils.py` & `django_mail_admin-0.3.2/django_mail_admin/utils.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin/validators.py` & `django_mail_admin-0.3.2/django_mail_admin/validators.py`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/django_mail_admin.egg-info/PKG-INFO` & `django_mail_admin-0.3.2/django_mail_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mail-admin
-Version: 0.3.1
+Version: 0.3.2
 Summary: The one and only django app to receive & send mail with templates and multiple configurations.
 Home-page: https://github.com/delneg/django_mail_admin
 Author: Denis Bobrov
 Author-email: delneg@yandex.ru
 License: MIT
 Keywords: django_mail_admin
 Platform: UNKNOWN
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gmail
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============================
 Django Mail Admin
 =============================
@@ -68,15 +69,15 @@
 
 * `django >= 1.9 <http://djangoproject.com/>`_
 * `django-jsonfield <https://github.com/bradjasper/django-jsonfield>`_
 
 Documentation
 -------------
 
-The full documentation is at https://django_mail_admin.readthedocs.io.
+The full documentation is at https://django-mail-admin.readthedocs.io.
 
 Quickstart
 ----------
 
 **Q**: What versions of Django/Python are supported?
 **A**: Take a look at https://travis-ci.org/delneg/django_mail_admin
```

### Comparing `django_mail_admin-0.3.1/django_mail_admin.egg-info/SOURCES.txt` & `django_mail_admin-0.3.2/django_mail_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_mail_admin-0.3.1/setup.py` & `django_mail_admin-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,12 +75,13 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     extras_require={
         'gmail': ['social-auth-app-django']
     }
 )
```

