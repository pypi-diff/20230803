# Comparing `tmp/doctorr-0.1.0.tar.gz` & `tmp/doctorr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctorr-0.1.0.tar", last modified: Tue Aug  1 14:06:24 2023, max compression
+gzip compressed data, was "doctorr-0.1.1.tar", last modified: Thu Aug  3 12:47:16 2023, max compression
```

## Comparing `doctorr-0.1.0.tar` & `doctorr-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 14:06:24.533500 doctorr-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-01 14:06:15.000000 doctorr-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 14:06:15.000000 doctorr-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:06:24.533500 doctorr-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.529499 doctorr-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.529499 doctorr-0.1.0/src/doctorr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/src/doctorr/autocli/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/parse_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/parse_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/src/doctorr/autodoc/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/parse_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/parse_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/watchmode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/src/doctorr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:16.205160 doctorr-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-03 12:47:16.205160 doctorr-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 12:47:04.000000 doctorr-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-03 12:47:04.000000 doctorr-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:47:16.205160 doctorr-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:16.197160 doctorr-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:16.201160 doctorr-0.1.1/src/doctorr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:16.201160 doctorr-0.1.1/src/doctorr/autocli/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/parse_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autocli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:16.205160 doctorr-0.1.1/src/doctorr/autodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autodoc/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autodoc/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autodoc/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autodoc/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/autodoc/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-03 12:47:04.000000 doctorr-0.1.1/src/doctorr/watchmode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:47:16.201160 doctorr-0.1.1/src/doctorr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-03 12:47:16.000000 doctorr-0.1.1/src/doctorr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-03 12:47:16.000000 doctorr-0.1.1/src/doctorr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:47:16.000000 doctorr-0.1.1/src/doctorr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 12:47:16.000000 doctorr-0.1.1/src/doctorr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 12:47:16.000000 doctorr-0.1.1/src/doctorr.egg-info/top_level.txt
```

### Comparing `doctorr-0.1.0/src/doctorr/autocli/parse_argparse.py` & `doctorr-0.1.1/src/doctorr/autocli/parse_argparse.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autocli/parse_config.py` & `doctorr-0.1.1/src/doctorr/autocli/parse_config.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autocli/run.py` & `doctorr-0.1.1/src/doctorr/autocli/run.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autodoc/docstring.py` & `doctorr-0.1.1/src/doctorr/autodoc/docstring.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autodoc/inspection.py` & `doctorr-0.1.1/src/doctorr/autodoc/inspection.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autodoc/parse_config.py` & `doctorr-0.1.1/src/doctorr/autodoc/parse_config.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autodoc/run.py` & `doctorr-0.1.1/src/doctorr/autodoc/run.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/autodoc/templates.py` & `doctorr-0.1.1/src/doctorr/autodoc/templates.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/cli.py` & `doctorr-0.1.1/src/doctorr/cli.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/include.py` & `doctorr-0.1.1/src/doctorr/include.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/parse_config.py` & `doctorr-0.1.1/src/doctorr/parse_config.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/templates.py` & `doctorr-0.1.1/src/doctorr/templates.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr/watchmode.py` & `doctorr-0.1.1/src/doctorr/watchmode.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.1.0/src/doctorr.egg-info/SOURCES.txt` & `doctorr-0.1.1/src/doctorr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

