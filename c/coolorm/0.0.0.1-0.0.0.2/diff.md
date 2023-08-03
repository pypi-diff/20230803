# Comparing `tmp/coolORM-0.0.0.1.tar.gz` & `tmp/coolorm-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolORM-0.0.0.1.tar", last modified: Sat Jul 15 03:25:00 2023, max compression
+gzip compressed data, was "coolorm-0.0.0.2.tar", last modified: Thu Aug  3 16:47:40 2023, max compression
```

## Comparing `coolORM-0.0.0.1.tar` & `coolorm-0.0.0.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0       16 2023-07-15 03:24:57.518481 coolORM-0.0.0.1/coolORM.py
--rw-r--r--   0        0        0      224 2023-07-15 03:24:57.503933 coolORM-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0      113 1970-01-01 00:00:00.000000 coolORM-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-08-03 16:47:30.545536 coolorm-0.0.0.2/coolorm.py
+-rw-r--r--   0        0        0      224 2023-08-03 16:47:35.823159 coolorm-0.0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      113 1970-01-01 00:00:00.000000 coolorm-0.0.0.2/PKG-INFO
```

