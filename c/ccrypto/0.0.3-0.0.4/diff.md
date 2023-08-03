# Comparing `tmp/ccrypto-0.0.3.tar.gz` & `tmp/ccrypto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccrypto-0.0.3.tar", last modified: Thu Aug  3 16:35:48 2023, max compression
+gzip compressed data, was "ccrypto-0.0.4.tar", last modified: Thu Aug  3 16:37:47 2023, max compression
```

## Comparing `ccrypto-0.0.3.tar` & `ccrypto-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:35:48.057438 ccrypto-0.0.3/
--rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:35:48.057556 ccrypto-0.0.3/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.3/README.rst
--rw-r--r--   0 pawel      (501) staff       (20)      107 2023-08-03 16:35:48.058032 ccrypto-0.0.3/setup.cfg
--rw-r--r--   0 pawel      (501) staff       (20)      511 2023-08-03 16:35:46.000000 ccrypto-0.0.3/setup.py
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:35:48.054805 ccrypto-0.0.3/src/
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:35:48.057194 ccrypto-0.0.3/src/ccrypto.egg-info/
--rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:35:47.000000 ccrypto-0.0.3/src/ccrypto.egg-info/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      203 2023-08-03 16:35:48.000000 ccrypto-0.0.3/src/ccrypto.egg-info/SOURCES.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:35:47.000000 ccrypto-0.0.3/src/ccrypto.egg-info/dependency_links.txt
--rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-03 16:35:47.000000 ccrypto-0.0.3/src/ccrypto.egg-info/requires.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:35:47.000000 ccrypto-0.0.3/src/ccrypto.egg-info/top_level.txt
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:37:47.324912 ccrypto-0.0.4/
+-rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:37:47.325011 ccrypto-0.0.4/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.4/README.rst
+-rw-r--r--   0 pawel      (501) staff       (20)      107 2023-08-03 16:37:47.325546 ccrypto-0.0.4/setup.cfg
+-rw-r--r--   0 pawel      (501) staff       (20)      511 2023-08-03 16:37:29.000000 ccrypto-0.0.4/setup.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:37:47.322447 ccrypto-0.0.4/src/
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:37:47.324683 ccrypto-0.0.4/src/ccrypto.egg-info/
+-rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      203 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/requires.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/top_level.txt
```

