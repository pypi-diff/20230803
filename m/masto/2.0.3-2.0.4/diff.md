# Comparing `tmp/masto-2.0.3.tar.gz` & `tmp/masto-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masto-2.0.3.tar", last modified: Wed Aug  2 23:17:01 2023, max compression
+gzip compressed data, was "masto-2.0.4.tar", last modified: Wed Aug  2 23:54:44 2023, max compression
```

## Comparing `masto-2.0.3.tar` & `masto-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:17:01.352710 masto-2.0.3/
--rw-r--r--   0 imac33     (501) staff       (20)     7039 2023-08-02 23:17:01.352459 masto-2.0.3/PKG-INFO
--rw-r--r--   0 imac33     (501) staff       (20)     6540 2023-08-02 23:06:40.000000 masto-2.0.3/README.md
-drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:17:01.350237 masto-2.0.3/masto/
--rw-r--r--   0 imac33     (501) staff       (20)        0 2023-08-02 19:15:17.000000 masto-2.0.3/masto/__init__.py
--rw-r--r--   0 imac33     (501) staff       (20)     8052 2023-08-02 21:43:34.000000 masto-2.0.3/masto/masto.py
-drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:17:01.352023 masto-2.0.3/masto.egg-info/
--rw-r--r--   0 imac33     (501) staff       (20)     7039 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/PKG-INFO
--rw-r--r--   0 imac33     (501) staff       (20)      195 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/SOURCES.txt
--rw-r--r--   0 imac33     (501) staff       (20)        1 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/dependency_links.txt
--rw-r--r--   0 imac33     (501) staff       (20)       35 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/requires.txt
--rw-r--r--   0 imac33     (501) staff       (20)        6 2023-08-02 23:17:01.000000 masto-2.0.3/masto.egg-info/top_level.txt
--rw-r--r--   0 imac33     (501) staff       (20)       38 2023-08-02 23:17:01.352922 masto-2.0.3/setup.cfg
--rw-r--r--   0 imac33     (501) staff       (20)      976 2023-08-02 23:12:32.000000 masto-2.0.3/setup.py
+drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:54:44.565329 masto-2.0.4/
+-rw-r--r--   0 imac33     (501) staff       (20)     7045 2023-08-02 23:54:44.565097 masto-2.0.4/PKG-INFO
+-rw-r--r--   0 imac33     (501) staff       (20)     6540 2023-08-02 23:06:40.000000 masto-2.0.4/README.md
+drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:54:44.562753 masto-2.0.4/masto/
+-rw-r--r--   0 imac33     (501) staff       (20)        0 2023-08-02 19:15:17.000000 masto-2.0.4/masto/__init__.py
+-rw-r--r--   0 imac33     (501) staff       (20)     8052 2023-08-02 21:43:34.000000 masto-2.0.4/masto/masto.py
+drwxr-xr-x   0 imac33     (501) staff       (20)        0 2023-08-02 23:54:44.564706 masto-2.0.4/masto.egg-info/
+-rw-r--r--   0 imac33     (501) staff       (20)     7045 2023-08-02 23:54:44.000000 masto-2.0.4/masto.egg-info/PKG-INFO
+-rw-r--r--   0 imac33     (501) staff       (20)      227 2023-08-02 23:54:44.000000 masto-2.0.4/masto.egg-info/SOURCES.txt
+-rw-r--r--   0 imac33     (501) staff       (20)        1 2023-08-02 23:54:44.000000 masto-2.0.4/masto.egg-info/dependency_links.txt
+-rw-r--r--   0 imac33     (501) staff       (20)       43 2023-08-02 23:54:44.000000 masto-2.0.4/masto.egg-info/entry_points.txt
+-rw-r--r--   0 imac33     (501) staff       (20)       35 2023-08-02 23:54:44.000000 masto-2.0.4/masto.egg-info/requires.txt
+-rw-r--r--   0 imac33     (501) staff       (20)        6 2023-08-02 23:54:44.000000 masto-2.0.4/masto.egg-info/top_level.txt
+-rw-r--r--   0 imac33     (501) staff       (20)       38 2023-08-02 23:54:44.565404 masto-2.0.4/setup.cfg
+-rw-r--r--   0 imac33     (501) staff       (20)     1090 2023-08-02 23:50:52.000000 masto-2.0.4/setup.py
```

### Comparing `masto-2.0.3/PKG-INFO` & `masto-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: masto
-Version: 2.0.3
+Version: 2.0.4
 Summary: Masto OSINT Tool Python package for Mastodon social OSINT investigations.
-Home-page: https://github.com/OSINT-Tactical/masto
-Author: OSINT_Tactical AKA C3n7ral051nt4g3ncy
+Home-page: https://github.com/C3n7ral051nt4g3ncy/Masto
+Author: OSINT_Tactical (AKA C3n7ral051nt4g3ncy)
 Author-email: C3n7ral051nt4g3ncy@tactical-osint-academy.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `masto-2.0.3/README.md` & `masto-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `masto-2.0.3/masto/masto.py` & `masto-2.0.4/masto/masto.py`

 * *Files identical despite different names*

### Comparing `masto-2.0.3/masto.egg-info/PKG-INFO` & `masto-2.0.4/masto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: masto
-Version: 2.0.3
+Version: 2.0.4
 Summary: Masto OSINT Tool Python package for Mastodon social OSINT investigations.
-Home-page: https://github.com/OSINT-Tactical/masto
-Author: OSINT_Tactical AKA C3n7ral051nt4g3ncy
+Home-page: https://github.com/C3n7ral051nt4g3ncy/Masto
+Author: OSINT_Tactical (AKA C3n7ral051nt4g3ncy)
 Author-email: C3n7ral051nt4g3ncy@tactical-osint-academy.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

