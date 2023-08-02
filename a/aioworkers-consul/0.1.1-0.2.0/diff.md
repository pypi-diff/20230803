# Comparing `tmp/aioworkers-consul-0.1.1.tar.gz` & `tmp/aioworkers_consul-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworkers-consul-0.1.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aioworkers-consul-0.1.1.tar` & `aioworkers_consul-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11357 2022-01-14 19:32:17.788281 aioworkers-consul-0.1.1/LICENSE
--rw-r--r--   0        0        0      719 2022-01-14 19:32:17.788281 aioworkers-consul-0.1.1/README.rst
--rw-r--r--   0        0        0     1124 2022-01-14 19:32:17.788281 aioworkers-consul-0.1.1/aioworkers_consul/__init__.py
--rw-r--r--   0        0        0       39 2022-01-14 19:32:17.788281 aioworkers-consul-0.1.1/aioworkers_consul/config.ini
--rw-r--r--   0        0        0     1376 2022-01-14 19:32:39.296491 aioworkers-consul-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1410 2022-01-14 19:32:40.457136 aioworkers-consul-0.1.1/setup.py
--rw-r--r--   0        0        0     1712 2022-01-14 19:32:40.457497 aioworkers-consul-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/aioworkers_consul/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/aioworkers_consul/config.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/aioworkers_consul/py.typed
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/README.rst
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 aioworkers_consul-0.2.0/PKG-INFO
```

### Comparing `aioworkers-consul-0.1.1/LICENSE` & `aioworkers_consul-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworkers-consul-0.1.1/aioworkers_consul/__init__.py` & `aioworkers_consul-0.2.0/aioworkers_consul/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Any, Mapping
 
 from aioworkers.core.config import ValueExtractor
 from aioworkers.storage.http import Storage
 
 BASE = Path(__file__).parent
-
+__version__ = "0.2.0"
 configs = (BASE / "config.ini",)
 
 
 class Client(Storage):
     _service: Mapping[str, Any]
 
     def set_config(self, config: ValueExtractor):
```

