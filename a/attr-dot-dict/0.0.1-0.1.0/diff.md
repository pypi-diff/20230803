# Comparing `tmp/attr-dot-dict-0.0.1.tar.gz` & `tmp/attr-dot-dict-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attr-dot-dict-0.0.1.tar", last modified: Wed Aug  2 22:22:40 2023, max compression
+gzip compressed data, was "attr-dot-dict-0.1.0.tar", last modified: Thu Aug  3 00:48:29 2023, max compression
```

## Comparing `attr-dot-dict-0.0.1.tar` & `attr-dot-dict-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 nick.mireles   (502) staff       (20)        0 2023-08-02 22:22:40.884177 attr-dot-dict-0.0.1/
--rw-r--r--   0 nick.mireles   (502) staff       (20)    35149 2023-08-02 20:04:56.000000 attr-dot-dict-0.0.1/LICENSE
--rw-r--r--   0 nick.mireles   (502) staff       (20)    41977 2023-08-02 22:22:40.884045 attr-dot-dict-0.0.1/PKG-INFO
--rw-r--r--   0 nick.mireles   (502) staff       (20)     1164 2023-08-02 21:46:57.000000 attr-dot-dict-0.0.1/README.md
-drwxr-xr-x   0 nick.mireles   (502) staff       (20)        0 2023-08-02 22:22:40.883778 attr-dot-dict-0.0.1/attr_dot_dict.egg-info/
--rw-r--r--   0 nick.mireles   (502) staff       (20)    41977 2023-08-02 22:22:40.000000 attr-dot-dict-0.0.1/attr_dot_dict.egg-info/PKG-INFO
--rw-r--r--   0 nick.mireles   (502) staff       (20)      200 2023-08-02 22:22:40.000000 attr-dot-dict-0.0.1/attr_dot_dict.egg-info/SOURCES.txt
--rw-r--r--   0 nick.mireles   (502) staff       (20)        1 2023-08-02 22:22:40.000000 attr-dot-dict-0.0.1/attr_dot_dict.egg-info/dependency_links.txt
--rw-r--r--   0 nick.mireles   (502) staff       (20)        8 2023-08-02 22:22:40.000000 attr-dot-dict-0.0.1/attr_dot_dict.egg-info/top_level.txt
--rw-r--r--   0 nick.mireles   (502) staff       (20)      584 2023-08-02 21:10:11.000000 attr-dot-dict-0.0.1/dotdict.py
--rw-r--r--   0 nick.mireles   (502) staff       (20)      378 2023-08-02 22:22:06.000000 attr-dot-dict-0.0.1/pyproject.toml
--rw-r--r--   0 nick.mireles   (502) staff       (20)       38 2023-08-02 22:22:40.884218 attr-dot-dict-0.0.1/setup.cfg
--rw-r--r--   0 nick.mireles   (502) staff       (20)       38 2023-08-02 20:36:40.000000 attr-dot-dict-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:48:29.920180 attr-dot-dict-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:48:29.920180 attr-dot-dict-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:48:29.920180 attr-dot-dict-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 00:48:19.000000 attr-dot-dict-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 00:48:19.000000 attr-dot-dict-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42029 2023-08-03 00:48:29.920180 attr-dot-dict-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 00:48:19.000000 attr-dot-dict-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:48:29.920180 attr-dot-dict-0.1.0/attr_dot_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42029 2023-08-03 00:48:29.000000 attr-dot-dict-0.1.0/attr_dot_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 00:48:29.000000 attr-dot-dict-0.1.0/attr_dot_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:48:29.000000 attr-dot-dict-0.1.0/attr_dot_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 00:48:29.000000 attr-dot-dict-0.1.0/attr_dot_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-03 00:48:19.000000 attr-dot-dict-0.1.0/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 00:48:19.000000 attr-dot-dict-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:48:29.920180 attr-dot-dict-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:48:19.000000 attr-dot-dict-0.1.0/setup.py
```

### Comparing `attr-dot-dict-0.0.1/LICENSE` & `attr-dot-dict-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attr-dot-dict-0.0.1/PKG-INFO` & `attr-dot-dict-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attr-dot-dict
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple class that allows for the chaining of attributes.
 Author-email: Nick Mireles <nick.mireles@dave.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -708,15 +708,15 @@
 config = dd()
 
 config.host = 'localhost'
 config.users.foo = 'bar'
 ```
 
 ## Installation
-Installation is simple: From this directory, run `pip install .`
+Installation is simple: `pip install attr-dot-dict`. Alternatively: `pip install .` from the root of the repository.
 
 ## Usage
 Usage is equally as simple:
 ```python
 from dotdict import DotDict as dd
 
 x = dd()
```

### Comparing `attr-dot-dict-0.0.1/README.md` & `attr-dot-dict-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 config = dd()
 
 config.host = 'localhost'
 config.users.foo = 'bar'
 ```
 
 ## Installation
-Installation is simple: From this directory, run `pip install .`
+Installation is simple: `pip install attr-dot-dict`. Alternatively: `pip install .` from the root of the repository.
 
 ## Usage
 Usage is equally as simple:
 ```python
 from dotdict import DotDict as dd
 
 x = dd()
```

### Comparing `attr-dot-dict-0.0.1/attr_dot_dict.egg-info/PKG-INFO` & `attr-dot-dict-0.1.0/attr_dot_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attr-dot-dict
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple class that allows for the chaining of attributes.
 Author-email: Nick Mireles <nick.mireles@dave.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -708,15 +708,15 @@
 config = dd()
 
 config.host = 'localhost'
 config.users.foo = 'bar'
 ```
 
 ## Installation
-Installation is simple: From this directory, run `pip install .`
+Installation is simple: `pip install attr-dot-dict`. Alternatively: `pip install .` from the root of the repository.
 
 ## Usage
 Usage is equally as simple:
 ```python
 from dotdict import DotDict as dd
 
 x = dd()
```

