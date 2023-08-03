# Comparing `tmp/liplustools-0.1.tar.gz` & `tmp/liplustools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liplustools-0.1.tar", last modified: Thu Aug  3 03:54:49 2023, max compression
+gzip compressed data, was "dist/liplustools-0.2.tar", last modified: Thu Aug  3 05:29:12 2023, max compression
```

## Comparing `liplustools-0.1.tar` & `liplustools-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 sqb        (501) staff       (20)        0 2023-08-03 03:54:49.000000 liplustools-0.1/
--rw-r--r--   0 sqb        (501) staff       (20)      243 2023-08-03 03:54:49.000000 liplustools-0.1/PKG-INFO
-drwxr-xr-x   0 sqb        (501) staff       (20)        0 2023-08-03 03:54:49.000000 liplustools-0.1/liplustools/
--rw-r--r--   0 sqb        (501) staff       (20)      312 2023-08-03 03:49:57.000000 liplustools-0.1/liplustools/__init__.py
-drwxr-xr-x   0 sqb        (501) staff       (20)        0 2023-08-03 03:54:49.000000 liplustools-0.1/liplustools.egg-info/
--rw-r--r--   0 sqb        (501) staff       (20)      243 2023-08-03 03:54:49.000000 liplustools-0.1/liplustools.egg-info/PKG-INFO
--rw-r--r--   0 sqb        (501) staff       (20)      206 2023-08-03 03:54:49.000000 liplustools-0.1/liplustools.egg-info/SOURCES.txt
--rw-r--r--   0 sqb        (501) staff       (20)        1 2023-08-03 03:54:49.000000 liplustools-0.1/liplustools.egg-info/dependency_links.txt
--rw-r--r--   0 sqb        (501) staff       (20)        1 2023-08-03 03:47:48.000000 liplustools-0.1/liplustools.egg-info/not-zip-safe
--rw-r--r--   0 sqb        (501) staff       (20)       12 2023-08-03 03:54:49.000000 liplustools-0.1/liplustools.egg-info/top_level.txt
--rw-r--r--   0 sqb        (501) staff       (20)       38 2023-08-03 03:54:49.000000 liplustools-0.1/setup.cfg
--rw-r--r--   0 sqb        (501) staff       (20)      398 2023-08-03 03:44:19.000000 liplustools-0.1/setup.py
+drwxr-xr-x   0 sqb        (501) staff       (20)        0 2023-08-03 05:29:12.000000 liplustools-0.2/
+-rw-r--r--   0 sqb        (501) staff       (20)      242 2023-08-03 05:29:12.000000 liplustools-0.2/PKG-INFO
+drwxr-xr-x   0 sqb        (501) staff       (20)        0 2023-08-03 05:29:12.000000 liplustools-0.2/liplustools/
+-rw-r--r--   0 sqb        (501) staff       (20)      144 2023-08-03 05:23:45.000000 liplustools-0.2/liplustools/__init__.py
+-rw-r--r--   0 sqb        (501) staff       (20)      263 2023-08-03 05:22:55.000000 liplustools-0.2/liplustools/text.py
+drwxr-xr-x   0 sqb        (501) staff       (20)        0 2023-08-03 05:29:12.000000 liplustools-0.2/liplustools.egg-info/
+-rw-r--r--   0 sqb        (501) staff       (20)      242 2023-08-03 05:29:12.000000 liplustools-0.2/liplustools.egg-info/PKG-INFO
+-rw-r--r--   0 sqb        (501) staff       (20)      226 2023-08-03 05:29:12.000000 liplustools-0.2/liplustools.egg-info/SOURCES.txt
+-rw-r--r--   0 sqb        (501) staff       (20)        1 2023-08-03 05:29:12.000000 liplustools-0.2/liplustools.egg-info/dependency_links.txt
+-rw-r--r--   0 sqb        (501) staff       (20)        1 2023-08-03 03:47:48.000000 liplustools-0.2/liplustools.egg-info/not-zip-safe
+-rw-r--r--   0 sqb        (501) staff       (20)       12 2023-08-03 05:29:12.000000 liplustools-0.2/liplustools.egg-info/top_level.txt
+-rw-r--r--   0 sqb        (501) staff       (20)       38 2023-08-03 05:29:12.000000 liplustools-0.2/setup.cfg
+-rw-r--r--   0 sqb        (501) staff       (20)      397 2023-08-03 05:27:25.000000 liplustools-0.2/setup.py
```

