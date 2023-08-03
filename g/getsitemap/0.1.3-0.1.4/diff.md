# Comparing `tmp/getsitemap-0.1.3.tar.gz` & `tmp/getsitemap-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsitemap-0.1.3.tar", last modified: Thu May 11 21:40:40 2023, max compression
+gzip compressed data, was "getsitemap-0.1.4.tar", last modified: Thu Aug  3 12:58:35 2023, max compression
```

## Comparing `getsitemap-0.1.3.tar` & `getsitemap-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.277587 getsitemap-0.1.3/
--rw-r--r--   0 james      (501) staff       (20)     1048 2023-05-11 21:19:35.000000 getsitemap-0.1.3/LICENSE.md
--rw-r--r--   0 james      (501) staff       (20)     1523 2023-05-11 21:40:40.277648 getsitemap-0.1.3/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      967 2023-05-11 21:19:35.000000 getsitemap-0.1.3/README.rst
--rw-r--r--   0 james      (501) staff       (20)      285 2023-05-11 21:19:35.000000 getsitemap-0.1.3/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)      642 2023-05-11 21:40:40.277897 getsitemap-0.1.3/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.275972 getsitemap-0.1.3/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.277252 getsitemap-0.1.3/src/getsitemap.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1523 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      229 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.277378 getsitemap-0.1.3/tests/
--rw-r--r--   0 james      (501) staff       (20)     1059 2023-05-11 21:19:35.000000 getsitemap-0.1.3/tests/test_retrieve_sitemap.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:58:35.929548 getsitemap-0.1.4/
+-rw-r--r--   0 james      (501) staff       (20)     1048 2023-08-03 10:12:55.000000 getsitemap-0.1.4/LICENSE.md
+-rw-r--r--   0 james      (501) staff       (20)     2563 2023-08-03 12:58:35.929283 getsitemap-0.1.4/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     2109 2023-08-03 10:12:55.000000 getsitemap-0.1.4/README.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:58:35.927396 getsitemap-0.1.4/getsitemap/
+-rw-r--r--   0 james      (501) staff       (20)      198 2023-08-03 12:58:23.000000 getsitemap-0.1.4/getsitemap/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7157 2023-08-03 10:12:55.000000 getsitemap-0.1.4/getsitemap/retrieve_sitemap.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:58:35.928624 getsitemap-0.1.4/getsitemap.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2563 2023-08-03 12:58:35.000000 getsitemap-0.1.4/getsitemap.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      299 2023-08-03 12:58:35.000000 getsitemap-0.1.4/getsitemap.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-03 12:58:35.000000 getsitemap-0.1.4/getsitemap.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       77 2023-08-03 12:58:35.000000 getsitemap-0.1.4/getsitemap.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       11 2023-08-03 12:58:35.000000 getsitemap-0.1.4/getsitemap.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)      285 2023-08-03 10:12:55.000000 getsitemap-0.1.4/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-08-03 12:58:35.929629 getsitemap-0.1.4/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1095 2023-08-03 12:57:47.000000 getsitemap-0.1.4/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:58:35.928905 getsitemap-0.1.4/tests/
+-rw-r--r--   0 james      (501) staff       (20)     1059 2023-08-03 10:12:55.000000 getsitemap-0.1.4/tests/test_retrieve_sitemap.py
```

### Comparing `getsitemap-0.1.3/LICENSE.md` & `getsitemap-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getsitemap-0.1.3/tests/test_retrieve_sitemap.py` & `getsitemap-0.1.4/tests/test_retrieve_sitemap.py`

 * *Files identical despite different names*

