# Comparing `tmp/koherent-0.1.0.tar.gz` & `tmp/koherent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koherent-0.1.0.tar", max compression
+gzip compressed data, was "koherent-0.1.1.tar", max compression
```

## Comparing `koherent-0.1.0.tar` & `koherent-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,20 @@
--rw-r--r--   0        0        0       22 2023-07-28 12:08:16.155498 koherent-0.1.0/README.md
--rw-r--r--   0        0        0       21 2023-07-28 12:07:44.119336 koherent-0.1.0/koherent/__init__.py
--rw-r--r--   0        0        0      299 2023-07-28 12:08:00.551419 koherent-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 koherent-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-28 12:08:16.155498 koherent-0.1.1/README.md
+-rw-r--r--   0        0        0       21 2023-07-28 12:07:44.119336 koherent-0.1.1/koherent/__init__.py
+-rw-r--r--   0        0        0       29 2023-08-03 15:27:37.028409 koherent-0.1.1/koherent/admin.py
+-rw-r--r--   0        0        0      148 2023-08-03 15:27:37.032409 koherent-0.1.1/koherent/apps.py
+-rw-r--r--   0        0        0      420 2023-08-03 15:27:37.064409 koherent-0.1.1/koherent/fields.py
+-rw-r--r--   0        0        0      574 2023-08-03 15:27:37.076409 koherent-0.1.1/koherent/filters.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:27:37.008409 koherent-0.1.1/koherent/migrations/__init__.py
+-rw-r--r--   0        0        0      143 2023-08-03 15:27:37.008409 koherent-0.1.1/koherent/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      401 2023-08-03 15:30:08.845298 koherent-0.1.1/koherent/models.py
+-rw-r--r--   0        0        0      638 2023-08-03 15:27:37.096409 koherent-0.1.1/koherent/signals.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:28:08.056589 koherent-0.1.1/koherent/strawberry/__init__.py
+-rw-r--r--   0        0        0      708 2023-08-03 15:30:21.657374 koherent-0.1.1/koherent/strawberry/extension.py
+-rw-r--r--   0        0        0      502 2023-08-03 15:29:02.808906 koherent-0.1.1/koherent/strawberry/filters.py
+-rw-r--r--   0        0        0       26 2023-08-03 15:27:37.108410 koherent-0.1.1/koherent/tests.py
+-rw-r--r--   0        0        0      148 2023-08-03 15:27:37.116410 koherent-0.1.1/koherent/types.py
+-rw-r--r--   0        0        0      145 2023-08-03 15:27:37.128410 koherent-0.1.1/koherent/utils.py
+-rw-r--r--   0        0        0      302 2023-08-03 15:27:37.140410 koherent-0.1.1/koherent/vars.py
+-rw-r--r--   0        0        0       26 2023-08-03 15:27:37.148410 koherent-0.1.1/koherent/views.py
+-rw-r--r--   0        0        0     1676 2023-08-03 15:30:40.081484 koherent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 koherent-0.1.1/PKG-INFO
```

