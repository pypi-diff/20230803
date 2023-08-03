# Comparing `tmp/simulation_engine-0.1.4.tar.gz` & `tmp/simulation_engine-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation_engine-0.1.4.tar", last modified: Thu Aug  3 00:20:50 2023, max compression
+gzip compressed data, was "simulation_engine-0.1.5.tar", last modified: Thu Aug  3 00:21:57 2023, max compression
```

## Comparing `simulation_engine-0.1.4.tar` & `simulation_engine-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 00:20:50.944350 simulation_engine-0.1.4/
--rw-rw-rw-   0        0        0      409 2023-08-03 00:20:50.943851 simulation_engine-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 00:20:50.944350 simulation_engine-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-08-03 00:19:49.000000 simulation_engine-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:20:50.940843 simulation_engine-0.1.4/simulation_engine/
--rw-rw-rw-   0        0        0     5111 2023-08-03 00:20:39.000000 simulation_engine-0.1.4/simulation_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:20:50.943350 simulation_engine-0.1.4/simulation_engine.egg-info/
--rw-rw-rw-   0        0        0      409 2023-08-03 00:20:50.000000 simulation_engine-0.1.4/simulation_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-08-03 00:20:50.000000 simulation_engine-0.1.4/simulation_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 00:20:50.000000 simulation_engine-0.1.4/simulation_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-03 00:20:50.000000 simulation_engine-0.1.4/simulation_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-03 00:20:50.000000 simulation_engine-0.1.4/simulation_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 00:21:57.477424 simulation_engine-0.1.5/
+-rw-rw-rw-   0        0        0      409 2023-08-03 00:21:57.476925 simulation_engine-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 00:21:57.477424 simulation_engine-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-08-03 00:21:50.000000 simulation_engine-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:21:57.474921 simulation_engine-0.1.5/simulation_engine/
+-rw-rw-rw-   0        0        0     5099 2023-08-03 00:21:46.000000 simulation_engine-0.1.5/simulation_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:21:57.476925 simulation_engine-0.1.5/simulation_engine.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-03 00:21:57.000000 simulation_engine-0.1.5/simulation_engine.egg-info/top_level.txt
```

### Comparing `simulation_engine-0.1.4/setup.py` & `simulation_engine-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.4' 
+VERSION = '0.1.5' 
 DESCRIPTION = 'Engine for simulating relic drops in Warframe.'
 LONG_DESCRIPTION = 'Engine for simulating relic drops in Warframe, has several features and is very extensible.'
 
 setup(
         name="simulation_engine", 
         version=VERSION,
         author="Jacob McBride",
```

### Comparing `simulation_engine-0.1.4/simulation_engine/__init__.py` & `simulation_engine-0.1.5/simulation_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,10 +162,10 @@
     if style in num_runs_dict:
         num_runs = num_runs_dict[style]
     else:
         num_runs = 1
     
     
     reward_list, reward_screen = zip(*[process_run(drops, offcycle_drops, style, drop_priority)
-                                       for _ in itertools.repeat(None, int(amount * num_runs_dict[style]))])
+                                       for _ in itertools.repeat(None, int(amount * num_runs))])
 
     return list(reward_list), list(reward_screen)
```

