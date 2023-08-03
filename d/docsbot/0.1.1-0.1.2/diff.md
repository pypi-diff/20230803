# Comparing `tmp/docsbot-0.1.1.tar.gz` & `tmp/docsbot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsbot-0.1.1.tar", last modified: Mon Jul 31 05:29:10 2023, max compression
+gzip compressed data, was "docsbot-0.1.2.tar", last modified: Thu Aug  3 15:58:49 2023, max compression
```

## Comparing `docsbot-0.1.1.tar` & `docsbot-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-31 05:29:10.025109 docsbot-0.1.1/
--rw-r--r--   0 jeffrey    (501) staff       (20)      148 2023-07-31 05:29:10.024954 docsbot-0.1.1/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      940 2023-07-31 05:23:15.000000 docsbot-0.1.1/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-31 05:29:10.024771 docsbot-0.1.1/docsbot.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      148 2023-07-31 05:29:09.000000 docsbot-0.1.1/docsbot.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      176 2023-07-31 05:29:10.000000 docsbot-0.1.1/docsbot.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-31 05:29:09.000000 docsbot-0.1.1/docsbot.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-07-31 05:29:09.000000 docsbot-0.1.1/docsbot.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-31 05:29:09.000000 docsbot-0.1.1/docsbot.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-31 05:29:10.025141 docsbot-0.1.1/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      335 2023-07-31 05:29:06.000000 docsbot-0.1.1/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-03 15:58:49.653809 docsbot-0.1.2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1807 2023-08-03 15:58:49.653709 docsbot-0.1.2/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1618 2023-08-03 14:33:32.000000 docsbot-0.1.2/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-03 15:58:49.653580 docsbot-0.1.2/docsbot.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1807 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       80 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-03 15:58:49.653841 docsbot-0.1.2/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      667 2023-08-03 15:58:46.000000 docsbot-0.1.2/setup.py
```

