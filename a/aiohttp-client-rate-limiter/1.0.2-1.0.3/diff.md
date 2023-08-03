# Comparing `tmp/aiohttp_client_rate_limiter-1.0.2.tar.gz` & `tmp/aiohttp_client_rate_limiter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_client_rate_limiter-1.0.2.tar", last modified: Thu Aug  3 00:56:37 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aiohttp_client_rate_limiter-1.0.2.tar` & `aiohttp_client_rate_limiter-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:56:37.248962 aiohttp_client_rate_limiter-1.0.2/
--rw-r--r--   0 peterbigmac   (501) staff       (20)    11357 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.2/LICENSE
--rw-r--r--   0 peterbigmac   (501) staff       (20)      543 2023-08-03 00:56:37.248290 aiohttp_client_rate_limiter-1.0.2/PKG-INFO
--rw-r--r--   0 peterbigmac   (501) staff       (20)       54 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.2/README.md
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:56:37.242601 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/
--rw-r--r--   0 peterbigmac   (501) staff       (20)     2842 2023-08-03 00:32:26.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/ClientSession.py
--rw-r--r--   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:31:52.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/__init__.py
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:56:37.246920 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/
--rw-r--r--   0 peterbigmac   (501) staff       (20)      543 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/PKG-INFO
--rw-r--r--   0 peterbigmac   (501) staff       (20)      365 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)        1 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)      150 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/requires.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)       28 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/top_level.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)       38 2023-08-03 00:56:37.249171 aiohttp_client_rate_limiter-1.0.2/setup.cfg
--rw-r--r--   0 peterbigmac   (501) staff       (20)     1055 2023-08-03 00:56:33.000000 aiohttp_client_rate_limiter-1.0.2/setup.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/example.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/setup.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/aiohttp_client_rate_limiter/ClientSession.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/aiohttp_client_rate_limiter/__init__.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 aiohttp_client_rate_limiter-1.0.3/PKG-INFO
```

### Comparing `aiohttp_client_rate_limiter-1.0.2/LICENSE` & `aiohttp_client_rate_limiter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_client_rate_limiter-1.0.2/setup.py` & `aiohttp_client_rate_limiter-1.0.3/setup.py`

 * *Files identical despite different names*

