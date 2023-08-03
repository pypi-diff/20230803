# Comparing `tmp/ap_features-2023.4.0.tar.gz` & `tmp/ap_features-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ap_features-2023.4.0.tar", last modified: Sun Jun 18 14:21:25 2023, max compression
+gzip compressed data, was "ap_features-2023.5.0.tar", last modified: Thu Aug  3 14:13:55 2023, max compression
```

## Comparing `ap_features-2023.4.0.tar` & `ap_features-2023.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.671556 ap_features-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-18 14:20:46.000000 ap_features-2023.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-18 14:20:46.000000 ap_features-2023.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-18 14:20:46.000000 ap_features-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 14:20:46.000000 ap_features-2023.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-18 14:21:25.671556 ap_features-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-18 14:20:46.000000 ap_features-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.663555 ap_features-2023.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-18 14:20:46.000000 ap_features-2023.4.0/docs/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-18 14:20:46.000000 ap_features-2023.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-18 14:20:46.000000 ap_features-2023.4.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-18 14:20:46.000000 ap_features-2023.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:21:25.671556 ap_features-2023.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.663555 ap_features-2023.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.667556 ap_features-2023.4.0/src/ap_features/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    39210 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/beat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.667556 ap_features-2023.4.0/src/ap_features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.667556 ap_features-2023.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.663555 ap_features-2023.4.0/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.671556 ap_features-2023.4.0/tests/baseline_images/test_plot/
--rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/beats.png
--rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/beats_aligned.png
--rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/poincare.png
--rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat.png
--rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/cost_terms.npy
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/data.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/real_data.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_beat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.205902 ap_features-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 14:13:09.000000 ap_features-2023.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-03 14:13:09.000000 ap_features-2023.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-03 14:13:09.000000 ap_features-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 14:13:09.000000 ap_features-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-03 14:13:55.205902 ap_features-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-08-03 14:13:09.000000 ap_features-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.201901 ap_features-2023.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 14:13:09.000000 ap_features-2023.5.0/docs/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-03 14:13:09.000000 ap_features-2023.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-08-03 14:13:09.000000 ap_features-2023.5.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-03 14:13:09.000000 ap_features-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:13:55.205902 ap_features-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.197901 ap_features-2023.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.201901 ap_features-2023.5.0/src/ap_features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39341 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-03 14:13:09.000000 ap_features-2023.5.0/src/ap_features/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.201901 ap_features-2023.5.0/src/ap_features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-03 14:13:55.000000 ap_features-2023.5.0/src/ap_features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 14:13:55.000000 ap_features-2023.5.0/src/ap_features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:13:55.000000 ap_features-2023.5.0/src/ap_features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-03 14:13:55.000000 ap_features-2023.5.0/src/ap_features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:13:55.000000 ap_features-2023.5.0/src/ap_features.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.205902 ap_features-2023.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.197901 ap_features-2023.5.0/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:13:55.205902 ap_features-2023.5.0/tests/baseline_images/test_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/baseline_images/test_plot/beats.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/baseline_images/test_plot/beats_aligned.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/baseline_images/test_plot/poincare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/baseline_images/test_plot/simple_beat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/baseline_images/test_plot/simple_beat_with_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/cost_terms.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/real_data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-03 14:13:09.000000 ap_features-2023.5.0/tests/test_plot.py
```

### Comparing `ap_features-2023.4.0/CONTRIBUTING.md` & `ap_features-2023.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/LICENSE` & `ap_features-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/PKG-INFO` & `ap_features-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ap_features
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Package to compute features of traces from action potential models
 Author-email: Henrik Finsberg <henriknf@simula.no>, "Kristian G. Hustad" <kghustad@simula.no>
 License: LGPL-2.1
 Project-URL: Homepage, https://computationalphysiology.github.io/ap_features
 Project-URL: Documentation, https://computationalphysiology.github.io/ap_features
 Project-URL: Source, https://github.com/ComputationalPhysiology/ap_features
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/ap_features/issues
```

### Comparing `ap_features-2023.4.0/README.md` & `ap_features-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/docs/INSTALL.md` & `ap_features-2023.5.0/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/docs/api.rst` & `ap_features-2023.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/docs/logo.png` & `ap_features-2023.5.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/pyproject.toml` & `ap_features-2023.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "oldest-supported-numpy; python_version>='3.5'",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ap_features"
-version = "2023.4.0"
+version = "2023.5.0"
 description = "Package to compute features of traces from action potential models"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}, {name = "Kristian G. Hustad", email = "kghustad@simula.no" }]
 license = {text = "LGPL-2.1"}
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["action potential", "cell", "models", "features"]
 dependencies = [
```

### Comparing `ap_features-2023.4.0/src/ap_features/__init__.py` & `ap_features-2023.5.0/src/ap_features/__init__.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/_numba.py` & `ap_features-2023.5.0/src/ap_features/_numba.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/average.py` & `ap_features-2023.5.0/src/ap_features/average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/background.py` & `ap_features-2023.5.0/src/ap_features/background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/beat.py` & `ap_features-2023.5.0/src/ap_features/beat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1038,15 +1038,19 @@
         Returns
         -------
         List[float]
             List of frequencies
         """
         signals: List[Array] = [beat.y for beat in self.beats]
         times: List[Array] = [beat.t for beat in self.beats]
-        return features.beating_frequency_from_peaks(signals=signals, times=times)
+
+        if len(signals) > 1:
+            return features.beating_frequency_from_peaks(signals=signals, times=times)
+        else:
+            return features.beating_frequency_from_apd_line(y=self.y, time=self.t)
 
     @property
     def beating_frequency(self) -> float:
         """The median frequency of all beats"""
         return np.median(self.beating_frequencies)
 
     @property
```

### Comparing `ap_features-2023.4.0/src/ap_features/chopping.py` & `ap_features-2023.5.0/src/ap_features/chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/features.py` & `ap_features-2023.5.0/src/ap_features/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,14 +554,56 @@
 
     dt = np.diff(t_maxs)
     if unit == "ms":
         dt = np.divide(dt, 1000.0)
     return np.divide(1, dt)
 
 
+def beating_frequency_from_apd_line(
+    y: np.ndarray,
+    time: np.ndarray,
+    unit: str = "ms",
+) -> Sequence[float]:
+    """Returns the beating frequency in Hz by using
+    the intersection of the APD50 line
+
+    Parameters
+    ----------
+    signals : List[Array]
+        The signal values for each beat
+    times : List[Array]
+        The time stamps of all beats
+    unit : str, optional
+        Unit of time, by default "ms"
+
+    Returns
+    -------
+    List[float]
+        Beating frequency in Hz for each beat
+    """
+
+    from . import chopping
+
+    starts, ends, zeros = chopping.locate_chop_points(
+        time,
+        y,
+        threshold_factor=0.5,
+        min_window=50,
+    )
+
+    if len(starts) > 1:
+        dt = np.diff(starts)
+    else:
+        dt = np.diff(ends)
+
+    if unit == "ms":
+        dt = np.divide(dt, 1000.0)
+    return np.divide(1, dt)
+
+
 def find_upstroke_values(
     t: np.ndarray,
     y: np.ndarray,
     upstroke_duration: int = 50,
     normalize: bool = True,
 ) -> np.ndarray:
     # Find intersection with APD50 line
```

### Comparing `ap_features-2023.4.0/src/ap_features/filters.py` & `ap_features-2023.5.0/src/ap_features/filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/plot.py` & `ap_features-2023.5.0/src/ap_features/plot.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/testing.py` & `ap_features-2023.5.0/src/ap_features/testing.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features/utils.py` & `ap_features-2023.5.0/src/ap_features/utils.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/src/ap_features.egg-info/PKG-INFO` & `ap_features-2023.5.0/src/ap_features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ap-features
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Package to compute features of traces from action potential models
 Author-email: Henrik Finsberg <henriknf@simula.no>, "Kristian G. Hustad" <kghustad@simula.no>
 License: LGPL-2.1
 Project-URL: Homepage, https://computationalphysiology.github.io/ap_features
 Project-URL: Documentation, https://computationalphysiology.github.io/ap_features
 Project-URL: Source, https://github.com/ComputationalPhysiology/ap_features
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/ap_features/issues
```

### Comparing `ap_features-2023.4.0/src/ap_features.egg-info/SOURCES.txt` & `ap_features-2023.5.0/src/ap_features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/baseline_images/test_plot/beats.png` & `ap_features-2023.5.0/tests/baseline_images/test_plot/beats.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/baseline_images/test_plot/beats_aligned.png` & `ap_features-2023.5.0/tests/baseline_images/test_plot/beats_aligned.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/baseline_images/test_plot/poincare.png` & `ap_features-2023.5.0/tests/baseline_images/test_plot/poincare.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat.png` & `ap_features-2023.5.0/tests/baseline_images/test_plot/simple_beat.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_background.png` & `ap_features-2023.5.0/tests/baseline_images/test_plot/simple_beat_with_background.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png` & `ap_features-2023.5.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/conftest.py` & `ap_features-2023.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/cost_terms.npy` & `ap_features-2023.5.0/tests/cost_terms.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/data.npy` & `ap_features-2023.5.0/tests/data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/real_data.npy` & `ap_features-2023.5.0/tests/real_data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/test_average.py` & `ap_features-2023.5.0/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/test_background.py` & `ap_features-2023.5.0/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/test_beat.py` & `ap_features-2023.5.0/tests/test_beat.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/test_chopping.py` & `ap_features-2023.5.0/tests/test_chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/test_features.py` & `ap_features-2023.5.0/tests/test_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,37 +212,31 @@
 
 @pytest.mark.parametrize("factor", range(10, 90, 5))
 def test_upstroke(factor, triangle_signal):
     x, y = triangle_signal
     assert np.isclose(apf.features.upstroke(x, y, a=factor / 100), factor)
 
 
-def test_beating_frequency(multiple_beats):
-    x, y = multiple_beats
-    beats = apf.Beats(y, x).beats
-    times = [beat.t for beat in beats]
-    assert np.isclose(
-        apf.features.beating_frequency(times),
-        13.297872340425531,
-        atol=0.2,
-    )
-
-
 def test_beating_frequency_from_peaks(multiple_beats):
     x, y = multiple_beats
     beats = apf.Beats(y, x).beats
     times = [beat.t for beat in beats]
     signals = [beat.y for beat in beats]
     assert np.isclose(
         apf.features.beating_frequency_from_peaks(signals, times),
         12.8,
         atol=0.2,
     ).all()
 
 
+def test_beating_frequency_from_apd_line(multiple_beats):
+    x, y = multiple_beats
+    assert np.isclose(apf.features.beating_frequency_from_apd_line(y, x), 12.82, atol=0.3).all()
+
+
 def test_max_relative_upstroke_velocity_sigmoid(calcium_trace):
     x, y = calcium_trace
     max_up = apf.features.max_relative_upstroke_velocity(x, y, sigmoid_fit=True)
     assert np.isclose(max_up.value, 0.03523266321708668)
     assert np.isclose(max_up.x0, 23.41210719885557)
```

### Comparing `ap_features-2023.4.0/tests/test_filters.py` & `ap_features-2023.5.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.4.0/tests/test_plot.py` & `ap_features-2023.5.0/tests/test_plot.py`

 * *Files identical despite different names*

