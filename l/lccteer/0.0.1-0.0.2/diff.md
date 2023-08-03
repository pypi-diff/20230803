# Comparing `tmp/lccteer-0.0.1.tar.gz` & `tmp/lccteer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccteer-0.0.1.tar", last modified: Thu May 18 16:30:48 2023, max compression
+gzip compressed data, was "lccteer-0.0.2.tar", last modified: Thu Aug  3 06:59:05 2023, max compression
```

## Comparing `lccteer-0.0.1.tar` & `lccteer-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    10943 2023-04-25 13:18:06.439303 lccteer-0.0.1/LICENSE
--rw-r--r--   0        0        0      124 2023-05-18 16:30:45.131696 lccteer-0.0.1/lccteer.py
--rw-r--r--   0        0        0      314 2023-05-18 16:30:45.119685 lccteer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      162 1970-01-01 00:00:00.000000 lccteer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2023-08-03 06:58:53.044978 lccteer-0.0.2/README.md
+-rw-r--r--   0        0        0       16 2023-08-03 06:55:10.738879 lccteer-0.0.2/lccteer.py
+-rw-r--r--   0        0        0      244 2023-08-03 06:56:03.984889 lccteer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      300 1970-01-01 00:00:00.000000 lccteer-0.0.2/PKG-INFO
```

