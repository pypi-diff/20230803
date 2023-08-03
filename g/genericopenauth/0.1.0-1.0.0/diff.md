# Comparing `tmp/genericopenauth-0.1.0.tar.gz` & `tmp/genericopenauth-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genericopenauth-0.1.0.tar", last modified: Thu Aug  3 16:50:55 2023, max compression
+gzip compressed data, was "genericopenauth-1.0.0.tar", last modified: Thu Aug  3 17:05:03 2023, max compression
```

## Comparing `genericopenauth-0.1.0.tar` & `genericopenauth-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 16:50:55.096416 genericopenauth-0.1.0/
--rw-rw-rw-   0        0        0      142 2023-08-03 16:50:55.095417 genericopenauth-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-03 14:22:01.000000 genericopenauth-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 16:50:55.075330 genericopenauth-0.1.0/genericopenauth/
--rw-rw-rw-   0        0        0       56 2023-08-03 15:34:49.000000 genericopenauth-0.1.0/genericopenauth/__init__.py
--rw-rw-rw-   0        0        0     1306 2023-08-03 14:24:52.000000 genericopenauth-0.1.0/genericopenauth/genericopenauth.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:50:55.094419 genericopenauth-0.1.0/genericopenauth.egg-info/
--rw-rw-rw-   0        0        0      142 2023-08-03 16:50:54.000000 genericopenauth-0.1.0/genericopenauth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-08-03 16:50:55.000000 genericopenauth-0.1.0/genericopenauth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 16:50:54.000000 genericopenauth-0.1.0/genericopenauth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 16:50:54.000000 genericopenauth-0.1.0/genericopenauth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 16:50:55.096416 genericopenauth-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      290 2023-08-03 14:27:19.000000 genericopenauth-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:05:03.688674 genericopenauth-1.0.0/
+-rw-rw-rw-   0        0        0      142 2023-08-03 17:05:03.687667 genericopenauth-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:22:01.000000 genericopenauth-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 17:05:03.665671 genericopenauth-1.0.0/genericopenauth/
+-rw-rw-rw-   0        0        0       56 2023-08-03 15:34:49.000000 genericopenauth-1.0.0/genericopenauth/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-08-03 14:24:52.000000 genericopenauth-1.0.0/genericopenauth/genericopenauth.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:05:03.686667 genericopenauth-1.0.0/genericopenauth.egg-info/
+-rw-rw-rw-   0        0        0      142 2023-08-03 17:05:03.000000 genericopenauth-1.0.0/genericopenauth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-08-03 17:05:03.000000 genericopenauth-1.0.0/genericopenauth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:05:03.000000 genericopenauth-1.0.0/genericopenauth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 17:05:03.000000 genericopenauth-1.0.0/genericopenauth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 17:05:03.000000 genericopenauth-1.0.0/genericopenauth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:05:03.688674 genericopenauth-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      295 2023-08-03 17:04:17.000000 genericopenauth-1.0.0/setup.py
```

### Comparing `genericopenauth-0.1.0/genericopenauth/genericopenauth.py` & `genericopenauth-1.0.0/genericopenauth/genericopenauth.py`

 * *Files identical despite different names*

