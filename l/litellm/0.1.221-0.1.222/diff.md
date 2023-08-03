# Comparing `tmp/litellm-0.1.221.tar.gz` & `tmp/litellm-0.1.222.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.221.tar", last modified: Thu Aug  3 05:26:24 2023, max compression
+gzip compressed data, was "litellm-0.1.222.tar", last modified: Thu Aug  3 13:28:32 2023, max compression
```

## Comparing `litellm-0.1.221.tar` & `litellm-0.1.222.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 05:26:24.034352 litellm-0.1.221/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-03 05:26:12.000000 litellm-0.1.221/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 05:26:24.034352 litellm-0.1.221/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-08-03 05:26:12.000000 litellm-0.1.221/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 05:26:24.030351 litellm-0.1.221/litellm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11192 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 05:26:24.034352 litellm-0.1.221/litellm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-08-03 05:26:24.000000 litellm-0.1.221/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-03 05:26:12.000000 litellm-0.1.221/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 05:26:24.034352 litellm-0.1.221/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-08-03 05:26:12.000000 litellm-0.1.221/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 13:28:32.089393 litellm-0.1.222/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.222/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 13:28:32.089276 litellm-0.1.222/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.222/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 13:28:32.088179 litellm-0.1.222/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      969 2023-08-03 02:58:58.000000 litellm-0.1.222/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.222/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.222/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    14924 2023-08-03 12:53:34.000000 litellm-0.1.222/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 13:28:32.089102 litellm-0.1.222/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 13:28:32.000000 litellm-0.1.222/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.222/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 13:28:32.089452 litellm-0.1.222/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 13:27:36.000000 litellm-0.1.222/setup.py
```

### Comparing `litellm-0.1.221/LICENSE` & `litellm-0.1.222/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.221/README.md` & `litellm-0.1.222/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.221/litellm/__init__.py` & `litellm-0.1.222/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.221/litellm/main.py` & `litellm-0.1.222/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.221/litellm/timeout.py` & `litellm-0.1.222/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.221/litellm/utils.py` & `litellm-0.1.222/litellm/utils.py`

 * *Files identical despite different names*

