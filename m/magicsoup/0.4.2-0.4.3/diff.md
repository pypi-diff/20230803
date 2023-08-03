# Comparing `tmp/magicsoup-0.4.2.tar.gz` & `tmp/magicsoup-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.4.2.tar", last modified: Sun Jul  9 21:35:45 2023, max compression
+gzip compressed data, was "magicsoup-0.4.3.tar", last modified: Mon Jul 10 20:08:03 2023, max compression
```

## Comparing `magicsoup-0.4.2.tar` & `magicsoup-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.300153 magicsoup-0.4.2/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.2/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 21:35:45.300153 magicsoup-0.4.2/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.2/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.2/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-07-09 21:35:45.300153 magicsoup-0.4.2/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.296153 magicsoup-0.4.2/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.296153 magicsoup-0.4.2/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-07-09 21:35:34.000000 magicsoup-0.4.2/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.2/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.2/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.300153 magicsoup-0.4.2/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.2/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.2/src/magicsoup/examples/co2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.2/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.2/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.2/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.2/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    40933 2023-07-09 21:34:46.000000 magicsoup-0.4.2/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.2/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.2/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.2/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.296153 magicsoup-0.4.2/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.300153 magicsoup-0.4.2/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.2/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.2/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.2/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.2/tests/test_kinetics_integration.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.2/tests/test_mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.2/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.2/tests/test_world.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.2/tests/test_world_integration.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-10 20:08:02.997192 magicsoup-0.4.3/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.3/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-10 20:08:02.997192 magicsoup-0.4.3/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.3/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.3/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-07-10 20:08:02.997192 magicsoup-0.4.3/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-10 20:08:02.993192 magicsoup-0.4.3/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-10 20:08:02.997192 magicsoup-0.4.3/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-07-10 20:07:50.000000 magicsoup-0.4.3/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.3/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.3/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-10 20:08:02.997192 magicsoup-0.4.3/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.3/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.3/src/magicsoup/examples/co2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.3/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.3/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.3/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.3/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    40808 2023-07-10 19:08:24.000000 magicsoup-0.4.3/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.3/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.3/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.3/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-10 20:08:02.997192 magicsoup-0.4.3/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-10 20:08:02.000000 magicsoup-0.4.3/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-07-10 20:08:02.000000 magicsoup-0.4.3/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-07-10 20:08:02.000000 magicsoup-0.4.3/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-07-10 20:08:02.000000 magicsoup-0.4.3/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-10 20:08:02.997192 magicsoup-0.4.3/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.3/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.3/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.3/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.3/tests/test_kinetics_integration.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.3/tests/test_mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.3/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.3/tests/test_world.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.3/tests/test_world_integration.py
```

### Comparing `magicsoup-0.4.2/LICENSE` & `magicsoup-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/PKG-INFO` & `magicsoup-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.2
+Version: 0.4.3
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.4.2/README.md` & `magicsoup-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/pyproject.toml` & `magicsoup-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/constants.py` & `magicsoup-0.4.3/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/containers.py` & `magicsoup-0.4.3/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/examples/co2_fixing.py` & `magicsoup-0.4.3/src/magicsoup/examples/co2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.4.3/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.4.3/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.4.3/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/genetics.py` & `magicsoup-0.4.3/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/kinetics.py` & `magicsoup-0.4.3/src/magicsoup/kinetics.py`

 * *Files 2% similar despite different names*

```diff
@@ -684,41 +684,36 @@
             # thus result velocity should be clamped again
             V = V.clamp(max=_MAX)
 
             # naive Xd, might produce negative X
             Xd = torch.einsum("cps,cp->cs", self.N, V)  # (c, s)
 
             # proteins can deconstruct more of a molecule than available in a cell
-            # but I can't just clip X at 0 because then reactions would not adhere
-            # to their stoichiometry anymore
-            # instead I need to reduce protein velocity
-            # However, a cell's Xd is the sum of all its protein's activities
-            # if I reduce the velocity of 1 protein, it could create a new
-            # below-zero situation for another one
-            # One would have to repeat this action until all conflicts are satisfied
+            # this happens mainly with multiple proteins with low Km trying to deconstruct
+            # the same molecule species in one cell
+            # reaction stoichiometry must be obeyed, so mere X.clamp(0.0) is not allowed
+            # One could factor out which proteins must be slowed down by how much,
+            # and selectively only slow down these proteins by a certain trimming factor.
+            # However, this could create a follow-up X<0.0 situation with one of the other proteins
+            # which were not slowed down. To solve this, one would have to construct a
+            # dependency graph of the protein network, or just iterate this process often enough.
             # Here, I am instead reducing all the cell's proteins by the same factor
-            # that way these secondary below-zero situations cannot appear
+            # that way these follow-up X<0.0 situations cannot appear
             # due to floating point precision I need to lift the cutoff from 0 to EPS
-            ma = Xd < 0.0
-            mb = X + Xd < 0.0
-            trim_to_zero = torch.where(ma & mb, X / -Xd - _EPS, 1.0).amin(1)  # (c,)
-            Xd = torch.einsum("cs,c->cs", Xd, trim_to_zero)
+            trim_factors = (X / -Xd - _EPS).clamp(0.0)
+            cell_trims = torch.where(X + Xd < 0.0, trim_factors, 1.0).amin(1)  # (c,)
+            Xd = torch.einsum("cs,c->cs", Xd, cell_trims)
 
             # update signals, this time no negative X
             X = X + Xd
 
-            # The above should make it impossible to create negative X
-            # However in some simulations I see negative values, they usually
-            # create extremely high values within 1 or 2 steps (cell molecule concentrations)
-            # I was not able to reproduce this in any of the tests
-            # TODO: luca/e1_co2_fixing has this problem but it can be avoided
-            #       by clamping after every computation
-            # it seems that clamping here does not create molecules from nothing
-            # my hypothesis is that the negative value was a floating point error
-            # and so clamping does not necessarily create molecules from nothing
+            # above was tested without clamp(0.0) and it never failed
+            # However, if due to some floating point inaccuracies, a negative X slips through
+            # it could create either NaNs or extremely large values (it would ruin a simulation)
+            # Thus, as a final measure clamp is used (it should never actually do anything)
             X = X.clamp(0.0)
 
         # NaNs can be created when overflow creates Infs (most likely in aggregate_signals)
         # with kinetics default values I have not been able to achieve this (>100 testruns)
         # however non-default values (e.g. large Vmax) might achieve that
         # once a 1 NaN is generated, it will spread over the whole simulation
         # this is a last effort in avoiding that
```

### Comparing `magicsoup-0.4.2/src/magicsoup/mutations.py` & `magicsoup-0.4.3/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/util.py` & `magicsoup-0.4.3/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup/world.py` & `magicsoup-0.4.3/src/magicsoup/world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.4.3/src/magicsoup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.2
+Version: 0.4.3
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.4.2/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.4.3/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_containers.py` & `magicsoup-0.4.3/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_genetics.py` & `magicsoup-0.4.3/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_kinetics.py` & `magicsoup-0.4.3/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_kinetics_integration.py` & `magicsoup-0.4.3/tests/test_kinetics_integration.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_mutations.py` & `magicsoup-0.4.3/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_util.py` & `magicsoup-0.4.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_world.py` & `magicsoup-0.4.3/tests/test_world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.2/tests/test_world_integration.py` & `magicsoup-0.4.3/tests/test_world_integration.py`

 * *Files identical despite different names*

