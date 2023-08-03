# Comparing `tmp/st-openai-embeddings-connection-0.1.0.tar.gz` & `tmp/st-openai-embeddings-connection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-openai-embeddings-connection-0.1.0.tar", last modified: Thu Aug  3 05:42:08 2023, max compression
+gzip compressed data, was "st-openai-embeddings-connection-0.1.1.tar", last modified: Thu Aug  3 06:07:50 2023, max compression
```

## Comparing `st-openai-embeddings-connection-0.1.0.tar` & `st-openai-embeddings-connection-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 05:42:08.827518 st-openai-embeddings-connection-0.1.0/
--rw-r--r--   0 gerardbentley   (501) staff       (20)    11339 2023-08-03 04:10:15.000000 st-openai-embeddings-connection-0.1.0/LICENSE
--rw-r--r--   0 gerardbentley   (501) staff       (20)      924 2023-08-03 05:42:08.827403 st-openai-embeddings-connection-0.1.0/PKG-INFO
--rw-r--r--   0 gerardbentley   (501) staff       (20)      605 2023-08-03 04:06:22.000000 st-openai-embeddings-connection-0.1.0/README.md
--rw-r--r--   0 gerardbentley   (501) staff       (20)      406 2023-08-03 05:41:45.000000 st-openai-embeddings-connection-0.1.0/pyproject.toml
--rw-r--r--   0 gerardbentley   (501) staff       (20)       38 2023-08-03 05:42:08.827556 st-openai-embeddings-connection-0.1.0/setup.cfg
-drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 05:42:08.826028 st-openai-embeddings-connection-0.1.0/src/
-drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 05:42:08.826620 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection/
--rw-r--r--   0 gerardbentley   (501) staff       (20)      183 2023-08-03 05:32:40.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection/__init__.py
--rw-r--r--   0 gerardbentley   (501) staff       (20)     4278 2023-08-03 05:39:49.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection/connection.py
-drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 05:42:08.827223 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection.egg-info/
--rw-r--r--   0 gerardbentley   (501) staff       (20)      924 2023-08-03 05:42:08.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection.egg-info/PKG-INFO
--rw-r--r--   0 gerardbentley   (501) staff       (20)      424 2023-08-03 05:42:08.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection.egg-info/SOURCES.txt
--rw-r--r--   0 gerardbentley   (501) staff       (20)        1 2023-08-03 05:42:08.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection.egg-info/dependency_links.txt
--rw-r--r--   0 gerardbentley   (501) staff       (20)       18 2023-08-03 05:42:08.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection.egg-info/requires.txt
--rw-r--r--   0 gerardbentley   (501) staff       (20)       32 2023-08-03 05:42:08.000000 st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection.egg-info/top_level.txt
+drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 06:07:50.247910 st-openai-embeddings-connection-0.1.1/
+-rw-r--r--   0 gerardbentley   (501) staff       (20)    11339 2023-08-03 04:10:15.000000 st-openai-embeddings-connection-0.1.1/LICENSE
+-rw-r--r--   0 gerardbentley   (501) staff       (20)     1259 2023-08-03 06:07:50.247787 st-openai-embeddings-connection-0.1.1/PKG-INFO
+-rw-r--r--   0 gerardbentley   (501) staff       (20)      940 2023-08-03 06:02:11.000000 st-openai-embeddings-connection-0.1.1/README.md
+-rw-r--r--   0 gerardbentley   (501) staff       (20)      406 2023-08-03 05:59:27.000000 st-openai-embeddings-connection-0.1.1/pyproject.toml
+-rw-r--r--   0 gerardbentley   (501) staff       (20)       38 2023-08-03 06:07:50.247949 st-openai-embeddings-connection-0.1.1/setup.cfg
+drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 06:07:50.246356 st-openai-embeddings-connection-0.1.1/src/
+drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 06:07:50.246952 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection/
+-rw-r--r--   0 gerardbentley   (501) staff       (20)      183 2023-08-03 05:32:40.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection/__init__.py
+-rw-r--r--   0 gerardbentley   (501) staff       (20)     4278 2023-08-03 05:39:49.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection/connection.py
+drwxr-xr-x   0 gerardbentley   (501) staff       (20)        0 2023-08-03 06:07:50.247570 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection.egg-info/
+-rw-r--r--   0 gerardbentley   (501) staff       (20)     1259 2023-08-03 06:07:50.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection.egg-info/PKG-INFO
+-rw-r--r--   0 gerardbentley   (501) staff       (20)      424 2023-08-03 06:07:50.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 gerardbentley   (501) staff       (20)        1 2023-08-03 06:07:50.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 gerardbentley   (501) staff       (20)       18 2023-08-03 06:07:50.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection.egg-info/requires.txt
+-rw-r--r--   0 gerardbentley   (501) staff       (20)       32 2023-08-03 06:07:50.000000 st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection.egg-info/top_level.txt
```

### Comparing `st-openai-embeddings-connection-0.1.0/LICENSE` & `st-openai-embeddings-connection-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st-openai-embeddings-connection-0.1.0/src/st_openai_embeddings_connection/connection.py` & `st-openai-embeddings-connection-0.1.1/src/st_openai_embeddings_connection/connection.py`

 * *Files identical despite different names*

