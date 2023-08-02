# Comparing `tmp/masto-2.0.2.tar.gz` & `tmp/masto-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masto-2.0.2.tar", last modified: Wed Aug  2 22:26:17 2023, max compression
+gzip compressed data, was "masto-2.0.3.tar", last modified: Wed Aug  2 23:17:01 2023, max compression
```

## Comparing `masto-2.0.2.tar` & `masto-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 22:26:17.147042 masto-2.0.2/
--rw-r--r--   0 imac33     (501) staff       (20)      389 2023-08-02 22:26:17.146805 masto-2.0.2/PKG-INFO
-drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 22:26:17.144423 masto-2.0.2/masto/
--rw-r--r--   0 imac33     (501) staff       (20)        0 2023-08-02 19:15:17.000000 masto-2.0.2/masto/__init__.py
--rw-r--r--   0 imac33     (501) staff       (20)     8052 2023-08-02 21:43:34.000000 masto-2.0.2/masto/masto.py
-drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 22:26:17.146443 masto-2.0.2/masto.egg-info/
--rw-r--r--   0 imac33     (501) staff       (20)      389 2023-08-02 22:26:17.000000 masto-2.0.2/masto.egg-info/PKG-INFO
--rw-r--r--   0 imac33     (501) staff       (20)      217 2023-08-02 22:26:17.000000 masto-2.0.2/masto.egg-info/SOURCES.txt
--rw-r--r--   0 imac33     (501) staff       (20)        1 2023-08-02 22:26:17.000000 masto-2.0.2/masto.egg-info/dependency_links.txt
--rw-r--r--   0 imac33     (501) staff       (20)       43 2023-08-02 22:26:17.000000 masto-2.0.2/masto.egg-info/entry_points.txt
--rw-r--r--   0 imac33     (501) staff       (20)       35 2023-08-02 22:26:17.000000 masto-2.0.2/masto.egg-info/requires.txt
--rw-r--r--   0 imac33     (501) staff       (20)        6 2023-08-02 22:26:17.000000 masto-2.0.2/masto.egg-info/top_level.txt
--rw-r--r--   0 imac33     (501) staff       (20)       38 2023-08-02 22:26:17.147122 masto-2.0.2/setup.cfg
--rw-r--r--   0 imac33     (501) staff       (20)      735 2023-08-02 22:25:43.000000 masto-2.0.2/setup.py
+drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:17:01.352710 masto-2.0.3/
+-rw-r--r--   0 imac33     (501) staff       (20)     7039 2023-08-02 23:17:01.352459 masto-2.0.3/PKG-INFO
+-rw-r--r--   0 imac33     (501) staff       (20)     6540 2023-08-02 23:06:40.000000 masto-2.0.3/README.md
+drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:17:01.350237 masto-2.0.3/masto/
+-rw-r--r--   0 imac33     (501) staff       (20)        0 2023-08-02 19:15:17.000000 masto-2.0.3/masto/__init__.py
+-rw-r--r--   0 imac33     (501) staff       (20)     8052 2023-08-02 21:43:34.000000 masto-2.0.3/masto/masto.py
+drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:17:01.352023 masto-2.0.3/masto.egg-info/
+-rw-r--r--   0 imac33     (501) staff       (20)     7039 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/PKG-INFO
+-rw-r--r--   0 imac33     (501) staff       (20)      195 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/SOURCES.txt
+-rw-r--r--   0 imac33     (501) staff       (20)        1 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/dependency_links.txt
+-rw-r--r--   0 imac33     (501) staff       (20)       35 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/requires.txt
+-rw-r--r--   0 imac33     (501) staff       (20)        6 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/top_level.txt
+-rw-r--r--   0 imac33     (501) staff       (20)       38 2023-08-02 23:17:01.352922 masto-2.0.3/setup.cfg
+-rw-r--r--   0 imac33     (501) staff       (20)      976 2023-08-02 23:12:32.000000 masto-2.0.3/setup.py
```

### Comparing `masto-2.0.2/masto/masto.py` & `masto-2.0.3/masto/masto.py`

 * *Files identical despite different names*

