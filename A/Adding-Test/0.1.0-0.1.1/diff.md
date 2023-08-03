# Comparing `tmp/Adding_Test-0.1.0.tar.gz` & `tmp/Adding_Test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Adding_Test-0.1.0.tar", last modified: Thu Aug  3 05:52:45 2023, max compression
+gzip compressed data, was "Adding_Test-0.1.1.tar", last modified: Thu Aug  3 06:50:30 2023, max compression
```

## Comparing `Adding_Test-0.1.0.tar` & `Adding_Test-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 05:52:45.798303 Adding_Test-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-08-03 05:52:45.791312 Adding_Test-0.1.0/Adding_Test/
--rw-rw-rw-   0        0        0        0 2023-08-03 05:47:18.000000 Adding_Test-0.1.0/Adding_Test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 05:52:45.796303 Adding_Test-0.1.0/Adding_Test.egg-info/
--rw-rw-rw-   0        0        0       58 2023-08-03 05:52:45.000000 Adding_Test-0.1.0/Adding_Test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-08-03 05:52:45.000000 Adding_Test-0.1.0/Adding_Test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 05:52:45.000000 Adding_Test-0.1.0/Adding_Test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 05:52:45.000000 Adding_Test-0.1.0/Adding_Test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       58 2023-08-03 05:52:45.798303 Adding_Test-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 05:52:45.798303 Adding_Test-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-08-03 05:49:51.000000 Adding_Test-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:50:30.332327 Adding_Test-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-08-03 06:50:30.324327 Adding_Test-0.1.1/Adding_Test/
+-rw-rw-rw-   0        0        0       35 2023-08-03 06:23:55.000000 Adding_Test-0.1.1/Adding_Test/__init__.py
+-rw-rw-rw-   0        0        0      105 2023-08-03 05:49:31.000000 Adding_Test-0.1.1/Adding_Test/addition.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:50:30.330326 Adding_Test-0.1.1/Adding_Test.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-03 06:50:30.000000 Adding_Test-0.1.1/Adding_Test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-08-03 06:50:30.000000 Adding_Test-0.1.1/Adding_Test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 06:50:30.000000 Adding_Test-0.1.1/Adding_Test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 06:50:30.000000 Adding_Test-0.1.1/Adding_Test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       58 2023-08-03 06:50:30.331327 Adding_Test-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 06:50:30.332327 Adding_Test-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-08-03 06:30:38.000000 Adding_Test-0.1.1/setup.py
```

