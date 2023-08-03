# Comparing `tmp/ccrypto-0.0.4.tar.gz` & `tmp/ccrypto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccrypto-0.0.4.tar", last modified: Thu Aug  3 16:37:47 2023, max compression
+gzip compressed data, was "ccrypto-0.0.5.tar", last modified: Thu Aug  3 16:47:13 2023, max compression
```

## Comparing `ccrypto-0.0.4.tar` & `ccrypto-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:37:47.324912 ccrypto-0.0.4/
--rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:37:47.325011 ccrypto-0.0.4/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.4/README.rst
--rw-r--r--   0 pawel      (501) staff       (20)      107 2023-08-03 16:37:47.325546 ccrypto-0.0.4/setup.cfg
--rw-r--r--   0 pawel      (501) staff       (20)      511 2023-08-03 16:37:29.000000 ccrypto-0.0.4/setup.py
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:37:47.322447 ccrypto-0.0.4/src/
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:37:47.324683 ccrypto-0.0.4/src/ccrypto.egg-info/
--rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      203 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/SOURCES.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/dependency_links.txt
--rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/requires.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:37:47.000000 ccrypto-0.0.4/src/ccrypto.egg-info/top_level.txt
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:47:13.046659 ccrypto-0.0.5/
+-rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:47:13.046763 ccrypto-0.0.5/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.5/README.rst
+-rw-r--r--   0 pawel      (501) staff       (20)      107 2023-08-03 16:47:13.047361 ccrypto-0.0.5/setup.cfg
+-rw-r--r--   0 pawel      (501) staff       (20)      511 2023-08-03 16:45:59.000000 ccrypto-0.0.5/setup.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:47:13.043592 ccrypto-0.0.5/src/
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:47:13.044957 ccrypto-0.0.5/src/ccrypto/
+-rw-r--r--   0 pawel      (501) staff       (20)        2 2023-08-03 16:45:00.000000 ccrypto-0.0.5/src/ccrypto/__init__.py
+-rw-r--r--   0 pawel      (501) staff       (20)     2672 2023-08-03 16:19:35.000000 ccrypto-0.0.5/src/ccrypto/get_cmc_coins_by_mcap.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:47:13.046464 ccrypto-0.0.5/src/ccrypto.egg-info/
+-rw-r--r--   0 pawel      (501) staff       (20)      226 2023-08-03 16:47:12.000000 ccrypto-0.0.5/src/ccrypto.egg-info/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      264 2023-08-03 16:47:12.000000 ccrypto-0.0.5/src/ccrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:47:12.000000 ccrypto-0.0.5/src/ccrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-03 16:47:12.000000 ccrypto-0.0.5/src/ccrypto.egg-info/requires.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        8 2023-08-03 16:47:12.000000 ccrypto-0.0.5/src/ccrypto.egg-info/top_level.txt
```

