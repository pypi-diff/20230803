# Comparing `tmp/sourmash_mixers-0.2.tar.gz` & `tmp/sourmash_mixers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_mixers-0.2.tar", last modified: Tue Aug  1 14:37:44 2023, max compression
+gzip compressed data, was "sourmash_mixers-0.2.1.tar", last modified: Thu Aug  3 14:10:22 2023, max compression
```

## Comparing `sourmash_mixers-0.2.tar` & `sourmash_mixers-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:37:44.922162 sourmash_mixers-0.2/
--rw-r--r--   0 t          (502) staff       (20)     1501 2023-07-27 23:30:51.000000 sourmash_mixers-0.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)      287 2023-08-01 14:37:44.921671 sourmash_mixers-0.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)       74 2023-07-27 23:30:51.000000 sourmash_mixers-0.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      628 2023-08-01 14:36:32.000000 sourmash_mixers-0.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-08-01 14:37:44.922224 sourmash_mixers-0.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:37:44.921499 sourmash_mixers-0.2/sourmash_mixers.egg-info/
--rw-r--r--   0 t          (502) staff       (20)      287 2023-08-01 14:37:44.000000 sourmash_mixers-0.2/sourmash_mixers.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      226 2023-08-01 14:37:44.000000 sourmash_mixers-0.2/sourmash_mixers.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-08-01 14:37:44.000000 sourmash_mixers-0.2/sourmash_mixers.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      135 2023-08-01 14:37:44.000000 sourmash_mixers-0.2/sourmash_mixers.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-08-01 14:37:44.000000 sourmash_mixers-0.2/sourmash_mixers.egg-info/top_level.txt
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:10:22.127921 sourmash_mixers-0.2.1/
+-rw-r--r--   0 t          (502) staff       (20)     1501 2023-07-27 23:30:51.000000 sourmash_mixers-0.2.1/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)      289 2023-08-03 14:10:22.127779 sourmash_mixers-0.2.1/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)       74 2023-07-27 23:30:51.000000 sourmash_mixers-0.2.1/README.md
+-rw-r--r--   0 t          (502) staff       (20)      622 2023-08-03 14:08:51.000000 sourmash_mixers-0.2.1/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-03 14:10:22.127960 sourmash_mixers-0.2.1/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:10:22.127635 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)      289 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      226 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      166 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/top_level.txt
```

### Comparing `sourmash_mixers-0.2/LICENSE` & `sourmash_mixers-0.2.1/LICENSE`

 * *Files identical despite different names*

