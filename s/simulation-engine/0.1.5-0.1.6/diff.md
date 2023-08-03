# Comparing `tmp/simulation_engine-0.1.5.tar.gz` & `tmp/simulation_engine-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation_engine-0.1.5.tar", last modified: Thu Aug  3 00:21:57 2023, max compression
+gzip compressed data, was "simulation_engine-0.1.6.tar", last modified: Thu Aug  3 00:24:57 2023, max compression
```

## Comparing `simulation_engine-0.1.5.tar` & `simulation_engine-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 00:21:57.477424 simulation_engine-0.1.5/
--rw-rw-rw-   0        0        0      409 2023-08-03 00:21:57.476925 simulation_engine-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 00:21:57.477424 simulation_engine-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-08-03 00:21:50.000000 simulation_engine-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:21:57.474921 simulation_engine-0.1.5/simulation_engine/
--rw-rw-rw-   0        0        0     5099 2023-08-03 00:21:46.000000 simulation_engine-0.1.5/simulation_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:21:57.476925 simulation_engine-0.1.5/simulation_engine.egg-info/
--rw-rw-rw-   0        0        0      409 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 00:24:57.917429 simulation_engine-0.1.6/
+-rw-rw-rw-   0        0        0      409 2023-08-03 00:24:57.916928 simulation_engine-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 00:24:57.917429 simulation_engine-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-08-03 00:24:55.000000 simulation_engine-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:24:57.914924 simulation_engine-0.1.6/simulation_engine/
+-rw-rw-rw-   0        0        0     5109 2023-08-03 00:24:41.000000 simulation_engine-0.1.6/simulation_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:24:57.916928 simulation_engine-0.1.6/simulation_engine.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-08-03 00:24:57.000000 simulation_engine-0.1.6/simulation_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-08-03 00:24:57.000000 simulation_engine-0.1.6/simulation_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 00:24:57.000000 simulation_engine-0.1.6/simulation_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 00:24:57.000000 simulation_engine-0.1.6/simulation_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-03 00:24:57.000000 simulation_engine-0.1.6/simulation_engine.egg-info/top_level.txt
```

### Comparing `simulation_engine-0.1.5/setup.py` & `simulation_engine-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5' 
+VERSION = '0.1.6' 
 DESCRIPTION = 'Engine for simulating relic drops in Warframe.'
 LONG_DESCRIPTION = 'Engine for simulating relic drops in Warframe, has several features and is very extensible.'
 
 setup(
         name="simulation_engine", 
         version=VERSION,
         author="Jacob McBride",
```

### Comparing `simulation_engine-0.1.5/simulation_engine/__init__.py` & `simulation_engine-0.1.6/simulation_engine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     return reward_screen
 
 
 def process_run(drops, offcycle_drops, style, drop_priority):
     if style == 'Solo':
         num_drops = 1
     else:
-        num_drops = int(style[:1])
+        num_drops = int(style.split('b')[0])
 
     num_offcycle_drops = []
     if style != "4b4":
         if len(offcycle_drops) > 0:
             if len(offcycle_drops) == 1:
                 num_offcycle_drops = [4 - num_drops]
             elif len(offcycle_drops) == 2:
```

