# Comparing `tmp/parmscheck-1.0.0.tar.gz` & `tmp/parmscheck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\parmscheck-1.0.0.tar", last modified: Thu Aug  3 12:16:14 2023, max compression
+gzip compressed data, was "dist\parmscheck-1.0.1.tar", last modified: Thu Aug  3 12:16:44 2023, max compression
```

## Comparing `parmscheck-1.0.0.tar` & `parmscheck-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 12:16:14.382018 parmscheck-1.0.0/
--rw-rw-rw-   0        0        0       46 2023-08-03 11:20:31.000000 parmscheck-1.0.0/.gitignore
--rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmscheck-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      265 2023-08-03 12:16:14.381017 parmscheck-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmscheck-1.0.0/README.md
--rw-rw-rw-   0        0        0       54 2023-08-03 11:03:35.000000 parmscheck-1.0.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 12:16:14.329019 parmscheck-1.0.0/__pycache__/
--rw-rw-rw-   0        0        0     5816 2023-08-03 11:03:35.000000 parmscheck-1.0.0/__pycache__/typecheck.cpython-38.pyc
--rw-rw-rw-   0        0        0     6470 2023-08-03 12:06:17.000000 parmscheck-1.0.0/check.py
-drwxrwxrwx   0        0        0        0 2023-08-03 12:16:14.378020 parmscheck-1.0.0/parmscheck.egg-info/
--rw-rw-rw-   0        0        0      265 2023-08-03 12:16:14.000000 parmscheck-1.0.0/parmscheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-08-03 12:16:14.000000 parmscheck-1.0.0/parmscheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 12:16:14.000000 parmscheck-1.0.0/parmscheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 12:16:14.000000 parmscheck-1.0.0/parmscheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 12:16:14.383048 parmscheck-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      308 2023-08-03 12:15:55.000000 parmscheck-1.0.0/setup.py
--rw-rw-rw-   0        0        0     4829 2023-08-03 11:03:35.000000 parmscheck-1.0.0/test.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:16:44.493328 parmscheck-1.0.1/
+-rw-rw-rw-   0        0        0       46 2023-08-03 11:20:31.000000 parmscheck-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmscheck-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      265 2023-08-03 12:16:44.491327 parmscheck-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmscheck-1.0.1/README.md
+-rw-rw-rw-   0        0        0       54 2023-08-03 11:03:35.000000 parmscheck-1.0.1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:16:44.441328 parmscheck-1.0.1/__pycache__/
+-rw-rw-rw-   0        0        0     5816 2023-08-03 11:03:35.000000 parmscheck-1.0.1/__pycache__/typecheck.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6470 2023-08-03 12:06:17.000000 parmscheck-1.0.1/check.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:16:44.488327 parmscheck-1.0.1/parmscheck.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-08-03 12:16:44.000000 parmscheck-1.0.1/parmscheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-08-03 12:16:44.000000 parmscheck-1.0.1/parmscheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:16:44.000000 parmscheck-1.0.1/parmscheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:16:44.000000 parmscheck-1.0.1/parmscheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 12:16:44.493328 parmscheck-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      308 2023-08-03 12:16:39.000000 parmscheck-1.0.1/setup.py
+-rw-rw-rw-   0        0        0     4829 2023-08-03 11:03:35.000000 parmscheck-1.0.1/test.py
```

### Comparing `parmscheck-1.0.0/LICENSE` & `parmscheck-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.0/README.md` & `parmscheck-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.0/__pycache__/typecheck.cpython-38.pyc` & `parmscheck-1.0.1/__pycache__/typecheck.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.0/check.py` & `parmscheck-1.0.1/check.py`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.0/test.py` & `parmscheck-1.0.1/test.py`

 * *Files identical despite different names*

