# Comparing `tmp/tortoise_api_model-0.1.0.tar.gz` & `tmp/tortoise_api_model-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.1.0.tar", last modified: Mon Jul 31 11:47:54 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.2.1.tar", last modified: Thu Aug  3 08:03:16 2023, max compression
```

## Comparing `tortoise_api_model-0.1.0.tar` & `tortoise_api_model-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:47:54.118318 tortoise_api_model-0.1.0/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 11:47:54.118059 tortoise_api_model-0.1.0/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 11:47:54.118383 tortoise_api_model-0.1.0/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-31 11:46:49.000000 tortoise_api_model-0.1.0/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:47:54.116377 tortoise_api_model-0.1.0/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)       90 2023-07-30 17:17:05.000000 tortoise_api_model-0.1.0/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     1821 2023-07-31 11:47:20.000000 tortoise_api_model-0.1.0/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:47:54.117770 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 08:03:16.949791 tortoise_api_model-0.2.1/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-08-03 08:03:16.949575 tortoise_api_model-0.2.1/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-03 08:03:16.949845 tortoise_api_model-0.2.1/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-08-03 06:39:10.000000 tortoise_api_model-0.2.1/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 08:03:16.948372 tortoise_api_model-0.2.1/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)      140 2023-08-01 16:56:50.000000 tortoise_api_model-0.2.1/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)      280 2023-07-30 18:24:21.000000 tortoise_api_model-0.2.1/tortoise_api_model/consts.py
+-rw-r--r--   0 sol        (501) staff       (20)     1538 2023-08-02 10:01:54.000000 tortoise_api_model-0.2.1/tortoise_api_model/fields.py
+-rw-r--r--   0 sol        (501) staff       (20)     6436 2023-08-03 06:28:34.000000 tortoise_api_model-0.2.1/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 08:03:16.949335 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      334 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.1.0/setup.py` & `tortoise_api_model-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

### Comparing `tortoise_api_model-0.1.0/tortoise_api_model/model.py` & `tortoise_api_model-0.2.1/tortoise_api_model/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 from asyncpg import Point, Polygon, Range
-from tortoise import Model as BaseModel
 from tortoise.fields import Field, IntField, FloatField
 from tortoise.fields.base import VALUE
 
 
-class Model(BaseModel):
-    # id: int = IntField(pk=True)
-    _name: str = 'name'
-    def repr(self):
-        if self._name in self._meta.db_fields:
-            return getattr(self, self._name)
-        return self.__repr__()
-
-
-# Custom Fields
 class ListField(Field[VALUE]):
     base_field = Field[VALUE]
     labels: tuple
 
     # def __getattr__(self, attr):
     #     return None
```

