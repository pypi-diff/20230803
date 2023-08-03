# Comparing `tmp/sourmash_plugin_sketchall-0.2.tar.gz` & `tmp/sourmash_plugin_sketchall-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_sketchall-0.2.tar", last modified: Thu Aug  3 13:58:38 2023, max compression
+gzip compressed data, was "sourmash_plugin_sketchall-0.2.1.tar", last modified: Thu Aug  3 14:00:53 2023, max compression
```

## Comparing `sourmash_plugin_sketchall-0.2.tar` & `sourmash_plugin_sketchall-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 13:58:38.313548 sourmash_plugin_sketchall-0.2/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-01-22 15:12:24.000000 sourmash_plugin_sketchall-0.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)      167 2023-08-03 13:58:38.313432 sourmash_plugin_sketchall-0.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     2756 2023-08-03 13:57:28.000000 sourmash_plugin_sketchall-0.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      348 2023-08-03 13:57:12.000000 sourmash_plugin_sketchall-0.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-08-03 13:58:38.313584 sourmash_plugin_sketchall-0.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 13:58:38.312123 sourmash_plugin_sketchall-0.2/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 13:58:38.313017 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/
--rw-r--r--   0 t          (502) staff       (20)      167 2023-08-03 13:58:38.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      418 2023-08-03 13:58:38.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-08-03 13:58:38.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       78 2023-08-03 13:58:38.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       19 2023-08-03 13:58:38.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       26 2023-08-03 13:58:38.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     7627 2023-08-03 13:57:12.000000 sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 13:58:38.313151 sourmash_plugin_sketchall-0.2/tests/
--rw-r--r--   0 t          (502) staff       (20)     3115 2023-08-03 13:57:12.000000 sourmash_plugin_sketchall-0.2/tests/test_sourmash_sketchall.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:00:53.537612 sourmash_plugin_sketchall-0.2.1/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-01-22 15:12:24.000000 sourmash_plugin_sketchall-0.2.1/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     2966 2023-08-03 14:00:53.537486 sourmash_plugin_sketchall-0.2.1/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     2756 2023-08-03 13:57:28.000000 sourmash_plugin_sketchall-0.2.1/README.md
+-rw-r--r--   0 t          (502) staff       (20)      371 2023-08-03 13:59:43.000000 sourmash_plugin_sketchall-0.2.1/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-03 14:00:53.537646 sourmash_plugin_sketchall-0.2.1/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:00:53.536246 sourmash_plugin_sketchall-0.2.1/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:00:53.537091 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     2966 2023-08-03 14:00:53.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      418 2023-08-03 14:00:53.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-03 14:00:53.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       78 2023-08-03 14:00:53.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       19 2023-08-03 14:00:53.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       26 2023-08-03 14:00:53.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     7627 2023-08-03 13:57:12.000000 sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:00:53.537206 sourmash_plugin_sketchall-0.2.1/tests/
+-rw-r--r--   0 t          (502) staff       (20)     3115 2023-08-03 13:57:12.000000 sourmash_plugin_sketchall-0.2.1/tests/test_sourmash_sketchall.py
```

### Comparing `sourmash_plugin_sketchall-0.2/LICENSE` & `sourmash_plugin_sketchall-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_sketchall-0.2/README.md` & `sourmash_plugin_sketchall-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_sketchall-0.2/src/sourmash_plugin_sketchall.py` & `sourmash_plugin_sketchall-0.2.1/src/sourmash_plugin_sketchall.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_sketchall-0.2/tests/test_sourmash_sketchall.py` & `sourmash_plugin_sketchall-0.2.1/tests/test_sourmash_sketchall.py`

 * *Files identical despite different names*

