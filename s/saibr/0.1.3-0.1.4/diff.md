# Comparing `tmp/saibr-0.1.3.tar.gz` & `tmp/saibr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saibr-0.1.3.tar", last modified: Wed Apr 26 14:31:49 2023, max compression
+gzip compressed data, was "/home/runner/work/saibr_python/saibr_python/dist/.tmp-tzz127j1/saibr-0.1.4.tar", last modified: Thu Aug  3 11:08:39 2023, max compression
```

## Comparing `saibr-0.1.3.tar` & `saibr-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:31:49.020202 saibr-0.1.3/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 saibr-0.1.3/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     1492 2023-04-26 14:31:49.020418 saibr-0.1.3/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      834 2023-01-23 21:47:17.000000 saibr-0.1.3/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:31:49.004396 saibr-0.1.3/saibr/
--rw-r--r--   0 blandt   (743162876) 1934034978       63 2023-01-23 19:24:43.000000 saibr-0.1.3/saibr/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978      319 2023-01-14 15:33:40.000000 saibr-0.1.3/saibr/legacy.py
--rw-r--r--   0 blandt   (743162876) 1934034978     3094 2023-01-14 14:49:51.000000 saibr-0.1.3/saibr/misc.py
--rw-r--r--   0 blandt   (743162876) 1934034978    19923 2023-01-16 18:18:13.000000 saibr-0.1.3/saibr/saibr.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:31:49.019304 saibr-0.1.3/saibr.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     1492 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      243 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       82 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        6 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:31:49.022991 saibr-0.1.3/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      997 2023-04-26 14:31:32.000000 saibr-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:08:39.000000 saibr-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 11:08:26.000000 saibr-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-03 11:08:39.000000 saibr-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-03 11:08:26.000000 saibr-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/saibr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 11:08:39.000000 saibr-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-03 11:08:26.000000 saibr-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `saibr-0.1.3/LICENSE` & `saibr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saibr-0.1.3/saibr/misc.py` & `saibr-0.1.4/saibr/misc.py`

 * *Files identical despite different names*

### Comparing `saibr-0.1.3/saibr/saibr.py` & `saibr-0.1.4/saibr/saibr.py`

 * *Files identical despite different names*

### Comparing `saibr-0.1.3/setup.py` & `saibr-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='saibr',
-    version='0.1.3',
+    version='0.1.4',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     url='https://github.com/goehringlab/saibr_python',
     install_requires=['numpy',
                       'matplotlib',
```

