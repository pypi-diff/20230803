# Comparing `tmp/entity-type-local-0.0.3.tar.gz` & `tmp/entity-type-local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity-type-local-0.0.3.tar", last modified: Wed Aug  2 16:46:31 2023, max compression
+gzip compressed data, was "entity-type-local-0.0.4.tar", last modified: Thu Aug  3 16:56:15 2023, max compression
```

## Comparing `entity-type-local-0.0.3.tar` & `entity-type-local-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/entity_type_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/tests/test_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:56:15.760993 entity-type-local-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-03 16:56:15.760993 entity-type-local-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-03 16:55:56.000000 entity-type-local-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:56:15.760993 entity-type-local-0.0.4/entity_type_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-03 16:56:15.000000 entity-type-local-0.0.4/entity_type_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 16:56:15.000000 entity-type-local-0.0.4/entity_type_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:56:15.000000 entity-type-local-0.0.4/entity_type_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 16:56:15.000000 entity-type-local-0.0.4/entity_type_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 16:55:56.000000 entity-type-local-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:56:15.760993 entity-type-local-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 16:55:56.000000 entity-type-local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:56:15.760993 entity-type-local-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-03 16:55:56.000000 entity-type-local-0.0.4/src/EntityType.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:55:56.000000 entity-type-local-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:56:15.760993 entity-type-local-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 16:55:56.000000 entity-type-local-0.0.4/tests/test_entity.py
```

### Comparing `entity-type-local-0.0.3/setup.py` & `entity-type-local-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      name='entity-type-local',
-     version='0.0.3',
+     version='0.0.4',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Entity Type Python (Currently empty package)",
      long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `entity-type-local-0.0.3/tests/test_entity.py` & `entity-type-local-0.0.4/tests/test_entity.py`

 * *Files identical despite different names*

