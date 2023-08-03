# Comparing `tmp/parmscheck-1.0.3.tar.gz` & `tmp/parmscheck-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\parmscheck-1.0.3.tar", last modified: Thu Aug  3 12:29:18 2023, max compression
+gzip compressed data, was "dist\parmscheck-1.0.4.tar", last modified: Thu Aug  3 12:43:38 2023, max compression
```

## Comparing `parmscheck-1.0.3.tar` & `parmscheck-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 12:29:18.780550 parmscheck-1.0.3/
--rw-rw-rw-   0        0        0       46 2023-08-03 12:17:19.000000 parmscheck-1.0.3/.gitignore
--rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmscheck-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      265 2023-08-03 12:29:18.778545 parmscheck-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmscheck-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 12:29:18.771546 parmscheck-1.0.3/parmscheck.egg-info/
--rw-rw-rw-   0        0        0      265 2023-08-03 12:29:18.000000 parmscheck-1.0.3/parmscheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-08-03 12:29:18.000000 parmscheck-1.0.3/parmscheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 12:29:18.000000 parmscheck-1.0.3/parmscheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 12:29:18.000000 parmscheck-1.0.3/parmscheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 12:29:18.781551 parmscheck-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      308 2023-08-03 12:28:50.000000 parmscheck-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:43:38.338799 parmscheck-1.0.4/
+-rw-rw-rw-   0        0        0       46 2023-08-03 12:17:19.000000 parmscheck-1.0.4/.gitignore
+-rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmscheck-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-08-03 12:43:38.336795 parmscheck-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmscheck-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 12:43:38.303794 parmscheck-1.0.4/parmscheck/
+-rw-rw-rw-   0        0        0       54 2023-08-03 11:03:35.000000 parmscheck-1.0.4/parmscheck/__init__.py
+-rw-rw-rw-   0        0        0     6470 2023-08-03 12:06:17.000000 parmscheck-1.0.4/parmscheck/check.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:43:38.330794 parmscheck-1.0.4/parmscheck.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-08-03 12:43:37.000000 parmscheck-1.0.4/parmscheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-03 12:43:38.000000 parmscheck-1.0.4/parmscheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:43:37.000000 parmscheck-1.0.4/parmscheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:43:37.000000 parmscheck-1.0.4/parmscheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 12:43:38.340818 parmscheck-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      308 2023-08-03 12:43:19.000000 parmscheck-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:43:38.333797 parmscheck-1.0.4/test/
+-rw-rw-rw-   0        0        0     4834 2023-08-03 12:38:44.000000 parmscheck-1.0.4/test/test.py
```

### Comparing `parmscheck-1.0.3/LICENSE` & `parmscheck-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.3/README.md` & `parmscheck-1.0.4/README.md`

 * *Files identical despite different names*

