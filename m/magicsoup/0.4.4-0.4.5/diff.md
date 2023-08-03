# Comparing `tmp/magicsoup-0.4.4.tar.gz` & `tmp/magicsoup-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.4.4.tar", last modified: Thu Aug  3 19:31:27 2023, max compression
+gzip compressed data, was "magicsoup-0.4.5.tar", last modified: Thu Aug  3 19:35:22 2023, max compression
```

## Comparing `magicsoup-0.4.4.tar` & `magicsoup-0.4.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:31:27.671840 magicsoup-0.4.4/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.4/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5367 2023-08-03 19:31:27.671840 magicsoup-0.4.4/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4430 2023-08-03 19:27:14.000000 magicsoup-0.4.4/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.4/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-08-03 19:31:27.671840 magicsoup-0.4.4/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:31:27.667840 magicsoup-0.4.4/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:31:27.671840 magicsoup-0.4.4/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-08-03 19:31:14.000000 magicsoup-0.4.4/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.4/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.4/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:31:27.671840 magicsoup-0.4.4/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.4/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.4/src/magicsoup/examples/co2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.4/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.4/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.4/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.4/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    40808 2023-07-10 19:08:24.000000 magicsoup-0.4.4/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.4/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.4/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.4/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:31:27.671840 magicsoup-0.4.4/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5367 2023-08-03 19:31:27.000000 magicsoup-0.4.4/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-08-03 19:31:27.000000 magicsoup-0.4.4/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-08-03 19:31:27.000000 magicsoup-0.4.4/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-08-03 19:31:27.000000 magicsoup-0.4.4/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:31:27.671840 magicsoup-0.4.4/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.4/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.4/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.4/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.4/tests/test_kinetics_integration.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.4/tests/test_mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.4/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.4/tests/test_world.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.4/tests/test_world_integration.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.5/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5377 2023-08-03 19:35:22.086588 magicsoup-0.4.5/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4440 2023-08-03 19:34:38.000000 magicsoup-0.4.5/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.5/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-08-03 19:35:22.086588 magicsoup-0.4.5/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.082588 magicsoup-0.4.5/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.082588 magicsoup-0.4.5/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-08-03 19:35:12.000000 magicsoup-0.4.5/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.5/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.5/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.5/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.5/src/magicsoup/examples/co2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.5/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.5/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.5/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.5/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    40808 2023-07-10 19:08:24.000000 magicsoup-0.4.5/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.5/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.5/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.5/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5377 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.5/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.5/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.5/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.5/tests/test_kinetics_integration.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.5/tests/test_mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.5/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.5/tests/test_world.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.5/tests/test_world_integration.py
```

### Comparing `magicsoup-0.4.4/LICENSE` & `magicsoup-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/PKG-INFO` & `magicsoup-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.4
+Version: 0.4.5
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
@@ -34,15 +34,15 @@
 ---
 
 This game simulates cell metabolic and transduction pathway evolution.
 Define a 2D world with certain molecules and reactions.
 Add a few cells and create evolutionary pressure by selectively replicating and killing them.
 Then run and see what random mutations can do.
 
-![random cells](https://github.com/mRcSchwering/magic-soup/blob/main/docs/img/animation.gif)
+![random cells](https://raw.githubusercontent.com/mRcSchwering/magic-soup/main/docs/img/animation.gif)
 
 _Cell growth of 1000 cells with different genomes were simulated. Top row: Cell map showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line when energy levels were high, celline 2 when they wer low. Middle and bottom rows: Development of total cell count and molecule species concentrations over time._
 
 ### Installation
 
 For CPU alone you can just do:
```

### Comparing `magicsoup-0.4.4/README.md` & `magicsoup-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ---
 
 This game simulates cell metabolic and transduction pathway evolution.
 Define a 2D world with certain molecules and reactions.
 Add a few cells and create evolutionary pressure by selectively replicating and killing them.
 Then run and see what random mutations can do.
 
-![random cells](https://github.com/mRcSchwering/magic-soup/blob/main/docs/img/animation.gif)
+![random cells](https://raw.githubusercontent.com/mRcSchwering/magic-soup/main/docs/img/animation.gif)
 
 _Cell growth of 1000 cells with different genomes were simulated. Top row: Cell map showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line when energy levels were high, celline 2 when they wer low. Middle and bottom rows: Development of total cell count and molecule species concentrations over time._
 
 ### Installation
 
 For CPU alone you can just do:
```

### Comparing `magicsoup-0.4.4/pyproject.toml` & `magicsoup-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/constants.py` & `magicsoup-0.4.5/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/containers.py` & `magicsoup-0.4.5/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/examples/co2_fixing.py` & `magicsoup-0.4.5/src/magicsoup/examples/co2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.4.5/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.4.5/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.4.5/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/genetics.py` & `magicsoup-0.4.5/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/kinetics.py` & `magicsoup-0.4.5/src/magicsoup/kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/mutations.py` & `magicsoup-0.4.5/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/util.py` & `magicsoup-0.4.5/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup/world.py` & `magicsoup-0.4.5/src/magicsoup/world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.4.5/src/magicsoup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.4
+Version: 0.4.5
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
@@ -34,15 +34,15 @@
 ---
 
 This game simulates cell metabolic and transduction pathway evolution.
 Define a 2D world with certain molecules and reactions.
 Add a few cells and create evolutionary pressure by selectively replicating and killing them.
 Then run and see what random mutations can do.
 
-![random cells](https://github.com/mRcSchwering/magic-soup/blob/main/docs/img/animation.gif)
+![random cells](https://raw.githubusercontent.com/mRcSchwering/magic-soup/main/docs/img/animation.gif)
 
 _Cell growth of 1000 cells with different genomes were simulated. Top row: Cell map showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line when energy levels were high, celline 2 when they wer low. Middle and bottom rows: Development of total cell count and molecule species concentrations over time._
 
 ### Installation
 
 For CPU alone you can just do:
```

### Comparing `magicsoup-0.4.4/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.4.5/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_containers.py` & `magicsoup-0.4.5/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_genetics.py` & `magicsoup-0.4.5/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_kinetics.py` & `magicsoup-0.4.5/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_kinetics_integration.py` & `magicsoup-0.4.5/tests/test_kinetics_integration.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_mutations.py` & `magicsoup-0.4.5/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_util.py` & `magicsoup-0.4.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_world.py` & `magicsoup-0.4.5/tests/test_world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.4/tests/test_world_integration.py` & `magicsoup-0.4.5/tests/test_world_integration.py`

 * *Files identical despite different names*

