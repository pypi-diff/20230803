# Comparing `tmp/parmscheck-1.0.5.tar.gz` & `tmp/parmscheck-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\parmscheck-1.0.5.tar", last modified: Thu Aug  3 12:55:43 2023, max compression
+gzip compressed data, was "dist\parmscheck-1.0.6.tar", last modified: Thu Aug  3 16:59:34 2023, max compression
```

## Comparing `parmscheck-1.0.5.tar` & `parmscheck-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 12:55:43.119673 parmscheck-1.0.5/
--rw-rw-rw-   0        0        0       46 2023-08-03 12:17:19.000000 parmscheck-1.0.5/.gitignore
--rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmscheck-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      229 2023-08-03 12:55:43.118674 parmscheck-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmscheck-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 12:55:43.000677 parmscheck-1.0.5/parmscheck/
--rw-rw-rw-   0        0        0       54 2023-08-03 11:03:35.000000 parmscheck-1.0.5/parmscheck/__init__.py
--rw-rw-rw-   0        0        0     6470 2023-08-03 12:06:17.000000 parmscheck-1.0.5/parmscheck/check.py
-drwxrwxrwx   0        0        0        0 2023-08-03 12:55:43.112707 parmscheck-1.0.5/parmscheck.egg-info/
--rw-rw-rw-   0        0        0      229 2023-08-03 12:55:42.000000 parmscheck-1.0.5/parmscheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-03 12:55:42.000000 parmscheck-1.0.5/parmscheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 12:55:42.000000 parmscheck-1.0.5/parmscheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-03 12:55:42.000000 parmscheck-1.0.5/parmscheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 12:55:43.120674 parmscheck-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      318 2023-08-03 12:55:28.000000 parmscheck-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 12:55:43.115672 parmscheck-1.0.5/test/
--rw-rw-rw-   0        0        0     4834 2023-08-03 12:38:44.000000 parmscheck-1.0.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:59:34.524093 parmscheck-1.0.6/
+-rw-rw-rw-   0        0        0       46 2023-08-03 12:17:19.000000 parmscheck-1.0.6/.gitignore
+-rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmscheck-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-08-03 16:59:34.522097 parmscheck-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmscheck-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 16:59:34.428096 parmscheck-1.0.6/parmscheck/
+-rw-rw-rw-   0        0        0       54 2023-08-03 11:03:35.000000 parmscheck-1.0.6/parmscheck/__init__.py
+-rw-rw-rw-   0        0        0     6535 2023-08-03 16:59:09.000000 parmscheck-1.0.6/parmscheck/check.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:59:34.515095 parmscheck-1.0.6/parmscheck.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-08-03 16:59:32.000000 parmscheck-1.0.6/parmscheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-03 16:59:33.000000 parmscheck-1.0.6/parmscheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 16:59:32.000000 parmscheck-1.0.6/parmscheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 16:59:32.000000 parmscheck-1.0.6/parmscheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 16:59:34.524093 parmscheck-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      318 2023-08-03 16:48:56.000000 parmscheck-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:59:34.518103 parmscheck-1.0.6/test/
+-rw-rw-rw-   0        0        0     4811 2023-08-03 16:53:46.000000 parmscheck-1.0.6/test/test.py
```

### Comparing `parmscheck-1.0.5/LICENSE` & `parmscheck-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.5/README.md` & `parmscheck-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `parmscheck-1.0.5/parmscheck/check.py` & `parmscheck-1.0.6/parmscheck/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     """
     The decorator that checks types at runtime for a class
     
     """
     for name, method in inspect.getmembers(cls):
         if (not inspect.ismethod(method) and not inspect.isfunction(method)) or inspect.isbuiltin(method):
             continue
+        if method.__name__ == '__init__':
+            continue
         setattr(cls, name, check_args(method))
     return cls
 
 
 def check_type(obj: Any,
                candidate_type: Any,
                reltype: str = 'invariant'):
```

### Comparing `parmscheck-1.0.5/test/test.py` & `parmscheck-1.0.6/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from parmscheck import check_args, DetailedTypeError, check_args_for_class
+from check import check_args,  check_args_for_class
 from typing import (
     Any,
     Dict,
     List,
     NamedTuple,
     Tuple,
     TypeVar,
```

