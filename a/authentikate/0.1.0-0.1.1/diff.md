# Comparing `tmp/authentikate-0.1.0.tar.gz` & `tmp/authentikate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentikate-0.1.0.tar", max compression
+gzip compressed data, was "authentikate-0.1.1.tar", max compression
```

## Comparing `authentikate-0.1.0.tar` & `authentikate-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,18 @@
--rw-r--r--   0        0        0       22 2023-07-28 09:41:36.120221 authentikate-0.1.0/README.md
--rw-r--r--   0        0        0       21 2023-07-28 09:40:37.823933 authentikate-0.1.0/authentikate/__init__.py
--rw-r--r--   0        0        0      323 2023-07-28 09:41:10.532095 authentikate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 authentikate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-28 09:41:36.120221 authentikate-0.1.1/README.md
+-rw-r--r--   0        0        0       21 2023-07-28 09:40:37.823933 authentikate-0.1.1/authentikate/__init__.py
+-rw-r--r--   0        0        0      157 2023-08-03 14:19:57.192109 authentikate-0.1.1/authentikate/admin.py
+-rw-r--r--   0        0        0      156 2023-08-03 14:19:57.200110 authentikate-0.1.1/authentikate/apps.py
+-rw-r--r--   0        0        0      474 2023-08-03 14:19:57.204110 authentikate-0.1.1/authentikate/decode.py
+-rw-r--r--   0        0        0      409 2023-08-03 14:19:57.212109 authentikate-0.1.1/authentikate/errors.py
+-rw-r--r--   0        0        0     2542 2023-08-03 14:19:57.216110 authentikate-0.1.1/authentikate/expand.py
+-rw-r--r--   0        0        0     5875 2023-08-03 14:19:57.180109 authentikate-0.1.1/authentikate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:19:57.180109 authentikate-0.1.1/authentikate/migrations/__init__.py
+-rw-r--r--   0        0        0      850 2023-08-03 14:19:57.228110 authentikate-0.1.1/authentikate/models.py
+-rw-r--r--   0        0        0     1863 2023-08-03 14:19:57.236110 authentikate-0.1.1/authentikate/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:19:29.893577 authentikate-0.1.1/authentikate/strawberry/__init__.py
+-rw-r--r--   0        0        0      300 2023-08-03 15:19:17.041502 authentikate-0.1.1/authentikate/strawberry/filters.py
+-rw-r--r--   0        0        0      241 2023-08-03 15:19:36.301615 authentikate-0.1.1/authentikate/strawberry/types.py
+-rw-r--r--   0        0        0     1810 2023-08-03 14:19:57.244110 authentikate-0.1.1/authentikate/structs.py
+-rw-r--r--   0        0        0     1884 2023-08-03 14:19:57.264110 authentikate-0.1.1/authentikate/utils.py
+-rw-r--r--   0        0        0     1704 2023-08-03 15:20:53.218064 authentikate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 authentikate-0.1.1/PKG-INFO
```

