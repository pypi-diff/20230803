# Comparing `tmp/django-modeltrans-0.7.4.tar.gz` & `tmp/django-modeltrans-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-modeltrans-0.7.4.tar", last modified: Mon Apr  3 09:02:49 2023, max compression
+gzip compressed data, was "django-modeltrans-0.7.5.tar", last modified: Thu Aug  3 12:13:51 2023, max compression
```

## Comparing `django-modeltrans-0.7.4.tar` & `django-modeltrans-0.7.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.350441 django-modeltrans-0.7.4/
--rw-r--r--   0 jieter     (501) staff       (20)     5364 2023-04-03 09:01:59.000000 django-modeltrans-0.7.4/CHANGELOG.md
--rw-r--r--   0 jieter     (501) staff       (20)     1528 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/LICENSE
--rw-r--r--   0 jieter     (501) staff       (20)      108 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/MANIFEST.in
--rw-r--r--   0 jieter     (501) staff       (20)     2875 2023-04-03 09:02:49.350277 django-modeltrans-0.7.4/PKG-INFO
--rw-r--r--   0 jieter     (501) staff       (20)     1643 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/README.md
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.344989 django-modeltrans-0.7.4/django_modeltrans.egg-info/
--rw-r--r--   0 jieter     (501) staff       (20)     2875 2023-04-03 09:02:49.000000 django-modeltrans-0.7.4/django_modeltrans.egg-info/PKG-INFO
--rw-r--r--   0 jieter     (501) staff       (20)     1575 2023-04-03 09:02:49.000000 django-modeltrans-0.7.4/django_modeltrans.egg-info/SOURCES.txt
--rw-r--r--   0 jieter     (501) staff       (20)        1 2023-04-03 09:02:49.000000 django-modeltrans-0.7.4/django_modeltrans.egg-info/dependency_links.txt
--rw-r--r--   0 jieter     (501) staff       (20)       12 2023-04-03 09:02:49.000000 django-modeltrans-0.7.4/django_modeltrans.egg-info/requires.txt
--rw-r--r--   0 jieter     (501) staff       (20)       27 2023-04-03 09:02:49.000000 django-modeltrans-0.7.4/django_modeltrans.egg-info/top_level.txt
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.346368 django-modeltrans-0.7.4/modeltrans/
--rw-r--r--   0 jieter     (501) staff       (20)       81 2023-04-03 09:01:24.000000 django-modeltrans-0.7.4/modeltrans/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)     1128 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/modeltrans/admin.py
--rw-r--r--   0 jieter     (501) staff       (20)      394 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/apps.py
--rw-r--r--   0 jieter     (501) staff       (20)     3114 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/conf.py
--rw-r--r--   0 jieter     (501) staff       (20)    12107 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/fields.py
--rw-r--r--   0 jieter     (501) staff       (20)    15163 2023-03-06 13:00:13.000000 django-modeltrans-0.7.4/modeltrans/forms.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.342937 django-modeltrans-0.7.4/modeltrans/locale/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.342763 django-modeltrans-0.7.4/modeltrans/locale/de/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.346857 django-modeltrans-0.7.4/modeltrans/locale/de/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      593 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      879 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.342869 django-modeltrans-0.7.4/modeltrans/locale/fr/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.347358 django-modeltrans-0.7.4/modeltrans/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      593 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      881 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.342975 django-modeltrans-0.7.4/modeltrans/locale/nl/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.347688 django-modeltrans-0.7.4/modeltrans/locale/nl/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      577 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      867 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.347851 django-modeltrans-0.7.4/modeltrans/management/
--rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/management/__init__.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.348064 django-modeltrans-0.7.4/modeltrans/management/commands/
--rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/management/commands/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)     1473 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/modeltrans/management/commands/i18n_makemigrations.py
--rw-r--r--   0 jieter     (501) staff       (20)    14834 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/modeltrans/manager.py
--rw-r--r--   0 jieter     (501) staff       (20)     7281 2023-03-06 14:35:17.000000 django-modeltrans-0.7.4/modeltrans/migration.py
--rw-r--r--   0 jieter     (501) staff       (20)    10184 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/modeltrans/translator.py
--rw-r--r--   0 jieter     (501) staff       (20)     3612 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/modeltrans/utils.py
--rw-r--r--   0 jieter     (501) staff       (20)       57 2023-03-06 13:00:13.000000 django-modeltrans-0.7.4/pyproject.toml
--rw-r--r--   0 jieter     (501) staff       (20)       38 2023-04-03 09:02:49.350488 django-modeltrans-0.7.4/setup.cfg
--rwxr-xr-x   0 jieter     (501) staff       (20)     2254 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/setup.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.348775 django-modeltrans-0.7.4/test_migrations/
--rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/__init__.py
--rwxr-xr-x   0 jieter     (501) staff       (20)      527 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/clean.py
--rwxr-xr-x   0 jieter     (501) staff       (20)      255 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/manage.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.349113 django-modeltrans-0.7.4/test_migrations/migrate_test/
--rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/__init__.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.349694 django-modeltrans-0.7.4/test_migrations/migrate_test/app/
--rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)      245 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/admin.py
--rw-r--r--   0 jieter     (501) staff       (20)       81 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/apps.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-04-03 09:02:49.350080 django-modeltrans-0.7.4/test_migrations/migrate_test/app/migrations/
--rw-r--r--   0 jieter     (501) staff       (20)     1435 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/migrations/0001_initial.py
--rw-r--r--   0 jieter     (501) staff       (20)     1851 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/migrations/0002_auto_20170516_1521.py
--rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/migrations/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)      886 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/models.py
--rw-r--r--   0 jieter     (501) staff       (20)      379 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/app/translation.py
--rw-r--r--   0 jieter     (501) staff       (20)     3310 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/settings.py
--rw-r--r--   0 jieter     (501) staff       (20)      762 2023-03-06 12:17:17.000000 django-modeltrans-0.7.4/test_migrations/migrate_test/urls.py
--rw-r--r--   0 jieter     (501) staff       (20)     1484 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/post_migrate_tests.py
--rw-r--r--   0 jieter     (501) staff       (20)     1140 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/pre_migrate_tests.py
--rwxr-xr-x   0 jieter     (501) staff       (20)     3090 2023-03-06 14:35:12.000000 django-modeltrans-0.7.4/test_migrations/test.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.751128 django-modeltrans-0.7.5/
+-rw-r--r--   0 jieter     (501) staff       (20)     5441 2023-08-03 12:13:02.000000 django-modeltrans-0.7.5/CHANGELOG.md
+-rw-r--r--   0 jieter     (501) staff       (20)     1528 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/LICENSE
+-rw-r--r--   0 jieter     (501) staff       (20)      108 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/MANIFEST.in
+-rw-r--r--   0 jieter     (501) staff       (20)     2875 2023-08-03 12:13:51.750537 django-modeltrans-0.7.5/PKG-INFO
+-rw-r--r--   0 jieter     (501) staff       (20)     1643 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/README.md
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.745901 django-modeltrans-0.7.5/django_modeltrans.egg-info/
+-rw-r--r--   0 jieter     (501) staff       (20)     2875 2023-08-03 12:13:51.000000 django-modeltrans-0.7.5/django_modeltrans.egg-info/PKG-INFO
+-rw-r--r--   0 jieter     (501) staff       (20)     1575 2023-08-03 12:13:51.000000 django-modeltrans-0.7.5/django_modeltrans.egg-info/SOURCES.txt
+-rw-r--r--   0 jieter     (501) staff       (20)        1 2023-08-03 12:13:51.000000 django-modeltrans-0.7.5/django_modeltrans.egg-info/dependency_links.txt
+-rw-r--r--   0 jieter     (501) staff       (20)       12 2023-08-03 12:13:51.000000 django-modeltrans-0.7.5/django_modeltrans.egg-info/requires.txt
+-rw-r--r--   0 jieter     (501) staff       (20)       27 2023-08-03 12:13:51.000000 django-modeltrans-0.7.5/django_modeltrans.egg-info/top_level.txt
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.747046 django-modeltrans-0.7.5/modeltrans/
+-rw-r--r--   0 jieter     (501) staff       (20)       81 2023-08-03 12:12:35.000000 django-modeltrans-0.7.5/modeltrans/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)     1128 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/modeltrans/admin.py
+-rw-r--r--   0 jieter     (501) staff       (20)      394 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/apps.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3114 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/conf.py
+-rw-r--r--   0 jieter     (501) staff       (20)    12107 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/fields.py
+-rw-r--r--   0 jieter     (501) staff       (20)    15163 2023-03-06 13:00:13.000000 django-modeltrans-0.7.5/modeltrans/forms.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.744040 django-modeltrans-0.7.5/modeltrans/locale/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.743877 django-modeltrans-0.7.5/modeltrans/locale/de/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.747423 django-modeltrans-0.7.5/modeltrans/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      593 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      879 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.743978 django-modeltrans-0.7.5/modeltrans/locale/fr/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.747828 django-modeltrans-0.7.5/modeltrans/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      593 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      881 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.744078 django-modeltrans-0.7.5/modeltrans/locale/nl/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.748120 django-modeltrans-0.7.5/modeltrans/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      577 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      867 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.748260 django-modeltrans-0.7.5/modeltrans/management/
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/management/__init__.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.748450 django-modeltrans-0.7.5/modeltrans/management/commands/
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/management/commands/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)     1473 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/modeltrans/management/commands/i18n_makemigrations.py
+-rw-r--r--   0 jieter     (501) staff       (20)    14852 2023-08-03 12:11:03.000000 django-modeltrans-0.7.5/modeltrans/manager.py
+-rw-r--r--   0 jieter     (501) staff       (20)     7281 2023-03-06 14:35:17.000000 django-modeltrans-0.7.5/modeltrans/migration.py
+-rw-r--r--   0 jieter     (501) staff       (20)    10184 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/modeltrans/translator.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3612 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/modeltrans/utils.py
+-rw-r--r--   0 jieter     (501) staff       (20)       57 2023-03-06 13:00:13.000000 django-modeltrans-0.7.5/pyproject.toml
+-rw-r--r--   0 jieter     (501) staff       (20)       38 2023-08-03 12:13:51.751233 django-modeltrans-0.7.5/setup.cfg
+-rwxr-xr-x   0 jieter     (501) staff       (20)     2254 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/setup.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.749126 django-modeltrans-0.7.5/test_migrations/
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/__init__.py
+-rwxr-xr-x   0 jieter     (501) staff       (20)      527 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/clean.py
+-rwxr-xr-x   0 jieter     (501) staff       (20)      255 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/manage.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.749447 django-modeltrans-0.7.5/test_migrations/migrate_test/
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/__init__.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.749998 django-modeltrans-0.7.5/test_migrations/migrate_test/app/
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)      245 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/admin.py
+-rw-r--r--   0 jieter     (501) staff       (20)       81 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/apps.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-08-03 12:13:51.750359 django-modeltrans-0.7.5/test_migrations/migrate_test/app/migrations/
+-rw-r--r--   0 jieter     (501) staff       (20)     1435 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/migrations/0001_initial.py
+-rw-r--r--   0 jieter     (501) staff       (20)     1851 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/migrations/0002_auto_20170516_1521.py
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/migrations/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)      886 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/models.py
+-rw-r--r--   0 jieter     (501) staff       (20)      379 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/app/translation.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3310 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/settings.py
+-rw-r--r--   0 jieter     (501) staff       (20)      762 2023-03-06 12:17:17.000000 django-modeltrans-0.7.5/test_migrations/migrate_test/urls.py
+-rw-r--r--   0 jieter     (501) staff       (20)     1484 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/post_migrate_tests.py
+-rw-r--r--   0 jieter     (501) staff       (20)     1140 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/pre_migrate_tests.py
+-rwxr-xr-x   0 jieter     (501) staff       (20)     3090 2023-03-06 14:35:12.000000 django-modeltrans-0.7.5/test_migrations/test.py
```

### Comparing `django-modeltrans-0.7.4/CHANGELOG.md` & `django-modeltrans-0.7.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 django-modeltrans change log
 ============================
 
+## 0.7.5 (2023-08-03)
+- Fix crash with `limit_choices_to` (#100) fixes: #94
+
 ## 0.7.4 (2023-04-03)
 - Add support for Django 4.2
 
 ## 0.7.3 (2022-05-25)
 - Revert: Use `TranslationModelForm` to implement `ActiveLanguageMixin` (#86)
 
 ## 0.7.2 (2021-10-21)
```

### Comparing `django-modeltrans-0.7.4/LICENSE` & `django-modeltrans-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/PKG-INFO` & `django-modeltrans-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modeltrans
-Version: 0.7.4
+Version: 0.7.5
 Summary: Model translations in a jsonb field
 Home-page: https://github.com/zostera/django-modeltrans/
 Author: Jan Pieter Waagmeester
 Author-email: jieter@zostera.nl
 License: Simplified BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-modeltrans-0.7.4/README.md` & `django-modeltrans-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/django_modeltrans.egg-info/PKG-INFO` & `django-modeltrans-0.7.5/django_modeltrans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modeltrans
-Version: 0.7.4
+Version: 0.7.5
 Summary: Model translations in a jsonb field
 Home-page: https://github.com/zostera/django-modeltrans/
 Author: Jan Pieter Waagmeester
 Author-email: jieter@zostera.nl
 License: Simplified BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-modeltrans-0.7.4/django_modeltrans.egg-info/SOURCES.txt` & `django-modeltrans-0.7.5/django_modeltrans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/admin.py` & `django-modeltrans-0.7.5/modeltrans/admin.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/conf.py` & `django-modeltrans-0.7.5/modeltrans/conf.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/fields.py` & `django-modeltrans-0.7.5/modeltrans/fields.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/forms.py` & `django-modeltrans-0.7.5/modeltrans/forms.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/locale/de/LC_MESSAGES/django.mo` & `django-modeltrans-0.7.5/modeltrans/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/locale/de/LC_MESSAGES/django.po` & `django-modeltrans-0.7.5/modeltrans/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/locale/fr/LC_MESSAGES/django.mo` & `django-modeltrans-0.7.5/modeltrans/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/locale/fr/LC_MESSAGES/django.po` & `django-modeltrans-0.7.5/modeltrans/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/locale/nl/LC_MESSAGES/django.mo` & `django-modeltrans-0.7.5/modeltrans/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/locale/nl/LC_MESSAGES/django.po` & `django-modeltrans-0.7.5/modeltrans/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/management/commands/i18n_makemigrations.py` & `django-modeltrans-0.7.5/modeltrans/management/commands/i18n_makemigrations.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/manager.py` & `django-modeltrans-0.7.5/modeltrans/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
             return factory(
                 list(self._rewrite_Q(child) for child in q.children),
                 connector=q.connector,
                 negated=q.negated,
             )
         if isinstance(q, (list, tuple)):
             return self._rewrite_filter_clause(*q)
+        return q
 
     def _rewrite_ordering(self, field_names):
         new_field_names = []
 
         for field_name in field_names:
             if not isinstance(field_name, str):
                 new_field_names.append(self._rewrite_expression(field_name))
@@ -286,15 +287,15 @@
             - `title_nl__contains="foo"` will add an annotation for `title_nl`
             - `title_nl="bar"` will add an annotation for `title_nl`
             - `title_i18n="foo"` will add an annotation for a coalesce of the
                current active language, and all items of the fallback chain.
             - `Q(title_nl__contains="foo") will add an annotation for `title_nl`
 
         In all cases, the field part of the field lookup will be changed to use
-        the annotated verion.
+        the annotated version.
         """
         new_args = [Q(self._rewrite_Q(arg)) for arg in args if arg]
         new_kwargs = dict(
             self._rewrite_filter_clause(field, value) for field, value in kwargs.items()
         )
         return super()._filter_or_exclude(negate, new_args, new_kwargs)
```

### Comparing `django-modeltrans-0.7.4/modeltrans/migration.py` & `django-modeltrans-0.7.5/modeltrans/migration.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/translator.py` & `django-modeltrans-0.7.5/modeltrans/translator.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/modeltrans/utils.py` & `django-modeltrans-0.7.5/modeltrans/utils.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/setup.py` & `django-modeltrans-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/clean.py` & `django-modeltrans-0.7.5/test_migrations/clean.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/migrate_test/app/migrations/0001_initial.py` & `django-modeltrans-0.7.5/test_migrations/migrate_test/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/migrate_test/app/migrations/0002_auto_20170516_1521.py` & `django-modeltrans-0.7.5/test_migrations/migrate_test/app/migrations/0002_auto_20170516_1521.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/migrate_test/app/models.py` & `django-modeltrans-0.7.5/test_migrations/migrate_test/app/models.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/migrate_test/settings.py` & `django-modeltrans-0.7.5/test_migrations/migrate_test/settings.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/migrate_test/urls.py` & `django-modeltrans-0.7.5/test_migrations/migrate_test/urls.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/post_migrate_tests.py` & `django-modeltrans-0.7.5/test_migrations/post_migrate_tests.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/pre_migrate_tests.py` & `django-modeltrans-0.7.5/test_migrations/pre_migrate_tests.py`

 * *Files identical despite different names*

### Comparing `django-modeltrans-0.7.4/test_migrations/test.py` & `django-modeltrans-0.7.5/test_migrations/test.py`

 * *Files identical despite different names*

