# Comparing `tmp/scrapifurs-0.1.0.tar.gz` & `tmp/scrapifurs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapifurs-0.1.0.tar", last modified: Wed Aug  2 23:20:30 2023, max compression
+gzip compressed data, was "scrapifurs-0.1.2.tar", last modified: Wed Aug  2 23:50:06 2023, max compression
```

## Comparing `scrapifurs-0.1.0.tar` & `scrapifurs-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:20:30.932855 scrapifurs-0.1.0/
--rw-r--r--   0 phil       (501) staff       (20)     1069 2023-08-02 22:23:20.000000 scrapifurs-0.1.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)       76 2023-08-02 23:20:30.932542 scrapifurs-0.1.0/PKG-INFO
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:20:30.929720 scrapifurs-0.1.0/scrapifurs/
--rw-r--r--   0 phil       (501) staff       (20)     1761 2023-08-02 23:16:46.000000 scrapifurs-0.1.0/scrapifurs/GPTinstructions.py
--rw-r--r--   0 phil       (501) staff       (20)       70 2023-08-02 23:16:04.000000 scrapifurs-0.1.0/scrapifurs/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2161 2023-08-01 00:36:26.000000 scrapifurs-0.1.0/scrapifurs/tempCodeRunnerFile.py
--rw-r--r--   0 phil       (501) staff       (20)     4908 2023-08-01 18:22:54.000000 scrapifurs-0.1.0/scrapifurs/utils.py
--rw-r--r--   0 phil       (501) staff       (20)     3407 2023-08-01 16:17:08.000000 scrapifurs-0.1.0/scrapifurs/working_example.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:20:30.931702 scrapifurs-0.1.0/scrapifurs.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)       76 2023-08-02 23:20:30.000000 scrapifurs-0.1.0/scrapifurs.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      306 2023-08-02 23:20:30.000000 scrapifurs-0.1.0/scrapifurs.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-08-02 23:20:30.000000 scrapifurs-0.1.0/scrapifurs.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       17 2023-08-02 23:20:30.000000 scrapifurs-0.1.0/scrapifurs.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-08-02 23:20:30.932947 scrapifurs-0.1.0/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      225 2023-07-31 17:57:10.000000 scrapifurs-0.1.0/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:20:30.932130 scrapifurs-0.1.0/tests/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-31 20:35:20.000000 scrapifurs-0.1.0/tests/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:50:06.185206 scrapifurs-0.1.2/
+-rw-r--r--   0 phil       (501) staff       (20)     1069 2023-08-02 22:23:20.000000 scrapifurs-0.1.2/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)       76 2023-08-02 23:50:06.184807 scrapifurs-0.1.2/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      463 2023-08-02 23:45:53.000000 scrapifurs-0.1.2/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:50:06.180878 scrapifurs-0.1.2/scrapifurs/
+-rw-r--r--   0 phil       (501) staff       (20)     1761 2023-08-02 23:16:46.000000 scrapifurs-0.1.2/scrapifurs/GPTinstructions.py
+-rw-r--r--   0 phil       (501) staff       (20)       70 2023-08-02 23:16:04.000000 scrapifurs-0.1.2/scrapifurs/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2161 2023-08-01 00:36:26.000000 scrapifurs-0.1.2/scrapifurs/tempCodeRunnerFile.py
+-rw-r--r--   0 phil       (501) staff       (20)     4908 2023-08-01 18:22:54.000000 scrapifurs-0.1.2/scrapifurs/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)     3407 2023-08-01 16:17:08.000000 scrapifurs-0.1.2/scrapifurs/working_example.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:50:06.183613 scrapifurs-0.1.2/scrapifurs.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)       76 2023-08-02 23:50:06.000000 scrapifurs-0.1.2/scrapifurs.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      349 2023-08-02 23:50:06.000000 scrapifurs-0.1.2/scrapifurs.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-08-02 23:50:06.000000 scrapifurs-0.1.2/scrapifurs.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)      104 2023-08-02 23:50:06.000000 scrapifurs-0.1.2/scrapifurs.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       17 2023-08-02 23:50:06.000000 scrapifurs-0.1.2/scrapifurs.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-08-02 23:50:06.185315 scrapifurs-0.1.2/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      340 2023-08-02 23:50:04.000000 scrapifurs-0.1.2/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-08-02 23:50:06.184313 scrapifurs-0.1.2/tests/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-31 20:35:20.000000 scrapifurs-0.1.2/tests/__init__.py
```

### Comparing `scrapifurs-0.1.0/LICENSE` & `scrapifurs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapifurs-0.1.0/scrapifurs/GPTinstructions.py` & `scrapifurs-0.1.2/scrapifurs/GPTinstructions.py`

 * *Files identical despite different names*

### Comparing `scrapifurs-0.1.0/scrapifurs/tempCodeRunnerFile.py` & `scrapifurs-0.1.2/scrapifurs/tempCodeRunnerFile.py`

 * *Files identical despite different names*

### Comparing `scrapifurs-0.1.0/scrapifurs/utils.py` & `scrapifurs-0.1.2/scrapifurs/utils.py`

 * *Files identical despite different names*

### Comparing `scrapifurs-0.1.0/scrapifurs/working_example.py` & `scrapifurs-0.1.2/scrapifurs/working_example.py`

 * *Files identical despite different names*

