# Comparing `tmp/agamaddd-0.1.0.tar.gz` & `tmp/agamaddd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agamaddd-0.1.0.tar", max compression
+gzip compressed data, was "agamaddd-0.1.2.tar", max compression
```

## Comparing `agamaddd-0.1.0.tar` & `agamaddd-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-08-03 16:01:09.396828 agamaddd-0.1.0/agamaddd/__init__.py
--rw-r--r--   0        0        0      296 2023-08-03 16:03:48.910227 agamaddd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-03 16:01:09.396828 agamaddd-0.1.0/README.md
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 agamaddd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 16:01:09.396828 agamaddd-0.1.2/agamaddd/__init__.py
+-rw-r--r--   0        0        0      286 2023-08-03 16:30:20.857452 agamaddd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 16:01:09.396828 agamaddd-0.1.2/README.md
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 agamaddd-0.1.2/PKG-INFO
```

