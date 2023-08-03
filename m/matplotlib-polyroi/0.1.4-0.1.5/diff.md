# Comparing `tmp/matplotlib-polyroi-0.1.4.tar.gz` & `tmp/matplotlib-polyroi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib-polyroi-0.1.4.tar", last modified: Wed Apr 26 14:48:43 2023, max compression
+gzip compressed data, was "/home/runner/work/matplotlib-polyroi/matplotlib-polyroi/dist/.tmp-i0r8f2_y/matplotlib-polyroi-0.1.5.tar", last modified: Thu Aug  3 11:04:33 2023, max compression
```

## Comparing `matplotlib-polyroi-0.1.4.tar` & `matplotlib-polyroi-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:48:43.910197 matplotlib-polyroi-0.1.4/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 matplotlib-polyroi-0.1.4/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     2150 2023-04-26 14:48:43.910567 matplotlib-polyroi-0.1.4/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     1344 2023-01-24 09:54:13.000000 matplotlib-polyroi-0.1.4/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:48:43.896574 matplotlib-polyroi-0.1.4/matplotlib_polyroi/
--rw-r--r--   0 blandt   (743162876) 1934034978       40 2023-01-23 19:32:08.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978      361 2023-01-24 09:26:01.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi/funcs.py
--rw-r--r--   0 blandt   (743162876) 1934034978    16086 2023-01-24 09:40:30.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi/roi.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:48:43.908325 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     2150 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      330 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       55 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       19 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:48:43.915171 matplotlib-polyroi-0.1.4/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      881 2023-04-26 14:48:30.000000 matplotlib-polyroi-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 11:04:16.000000 matplotlib-polyroi-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-03 11:04:16.000000 matplotlib-polyroi-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 11:04:16.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 11:04:16.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-08-03 11:04:16.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/matplotlib_polyroi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 11:04:33.000000 matplotlib-polyroi-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 11:04:16.000000 matplotlib-polyroi-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `matplotlib-polyroi-0.1.4/LICENSE` & `matplotlib-polyroi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib-polyroi-0.1.4/matplotlib_polyroi/roi.py` & `matplotlib-polyroi-0.1.5/matplotlib_polyroi/roi.py`

 * *Files identical despite different names*

### Comparing `matplotlib-polyroi-0.1.4/setup.py` & `matplotlib-polyroi-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='matplotlib-polyroi',
-    version='0.1.4',
+    version='0.1.5',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'scipy',
```

