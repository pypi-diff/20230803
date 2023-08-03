# Comparing `tmp/st-supabase-connection-0.0.2.tar.gz` & `tmp/st-supabase-connection-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-supabase-connection-0.0.2.tar", last modified: Mon Jul 31 19:48:54 2023, max compression
+gzip compressed data, was "st-supabase-connection-0.1.0.tar", last modified: Thu Aug  3 21:16:31 2023, max compression
```

## Comparing `st-supabase-connection-0.0.2.tar` & `st-supabase-connection-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/src/st_supabase_connection/
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/src/st_supabase_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:16:31.878907 st-supabase-connection-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-03 21:16:19.000000 st-supabase-connection-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 21:16:19.000000 st-supabase-connection-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-08-03 21:16:31.878907 st-supabase-connection-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-08-03 21:16:19.000000 st-supabase-connection-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:16:31.878907 st-supabase-connection-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-03 21:16:19.000000 st-supabase-connection-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:16:31.874906 st-supabase-connection-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:16:31.874906 st-supabase-connection-0.1.0/src/st_supabase_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-08-03 21:16:19.000000 st-supabase-connection-0.1.0/src/st_supabase_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:16:31.878907 st-supabase-connection-0.1.0/src/st_supabase_connection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-08-03 21:16:31.000000 st-supabase-connection-0.1.0/src/st_supabase_connection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 21:16:31.000000 st-supabase-connection-0.1.0/src/st_supabase_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:16:31.000000 st-supabase-connection-0.1.0/src/st_supabase_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 21:16:31.000000 st-supabase-connection-0.1.0/src/st_supabase_connection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 21:16:31.000000 st-supabase-connection-0.1.0/src/st_supabase_connection.egg-info/top_level.txt
```

### Comparing `st-supabase-connection-0.0.2/LICENSE` & `st-supabase-connection-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-0.0.2/setup.py` & `st-supabase-connection-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,13 +36,16 @@
         "Environment :: Plugins",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Database",
+        "Topic :: Database :: Front-Ends",
+        "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: User Interfaces",
     ],
     keywords=["streamlit", "supabase", "connection", "integration"],
     python_requires=">=3.8",
-    install_requires=["streamlit>=1.2", "supabase"],
+    install_requires=["streamlit", "supabase"],
 )
```

