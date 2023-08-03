# Comparing `tmp/pyvalem-2.5.8.tar.gz` & `tmp/pyvalem-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvalem-2.5.8.tar", last modified: Sun Jul  3 12:54:38 2022, max compression
+gzip compressed data, was "pyvalem-2.5.9.tar", last modified: Mon Jul  4 15:58:02 2022, max compression
```

## Comparing `pyvalem-2.5.8.tar` & `pyvalem-2.5.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 12:54:38.706380 pyvalem-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-07-03 12:54:17.000000 pyvalem-2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-03 12:54:38.706380 pyvalem-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2022-07-03 12:54:17.000000 pyvalem-2.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-07-03 12:54:17.000000 pyvalem-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-03 12:54:38.706380 pyvalem-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-03 12:54:17.000000 pyvalem-2.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 12:54:38.702380 pyvalem-2.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 12:54:38.702380 pyvalem-2.5.8/src/pyvalem/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/_data_atomic_weights.txt
--rw-r--r--   0 runner    (1001) docker     (121)   158055 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/_data_isotope_masses.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/_special_cases.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/atom_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    23560 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/formula.py
--rw-r--r--   0 runner    (1001) docker     (121)    15666 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/stateful_species.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 12:54:38.706380 pyvalem-2.5.8/src/pyvalem/states/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/_base_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    10410 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/atomic_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/atomic_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     8354 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/diatomic_molecular_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/generic_excited_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/key_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (121)     6843 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/molecular_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/racah_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/rotational_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-07-03 12:54:17.000000 pyvalem-2.5.8/src/pyvalem/states/vibrational_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 12:54:38.702380 pyvalem-2.5.8/src/pyvalem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-03 12:54:38.000000 pyvalem-2.5.8/src/pyvalem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-07-03 12:54:38.000000 pyvalem-2.5.8/src/pyvalem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-03 12:54:38.000000 pyvalem-2.5.8/src/pyvalem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-03 12:54:38.000000 pyvalem-2.5.8/src/pyvalem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-03 12:54:38.000000 pyvalem-2.5.8/src/pyvalem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-07-04 15:57:47.000000 pyvalem-2.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-04 15:58:02.472142 pyvalem-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6564 2022-07-04 15:57:47.000000 pyvalem-2.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2022-07-04 15:57:47.000000 pyvalem-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-04 15:58:02.472142 pyvalem-2.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-04 15:57:47.000000 pyvalem-2.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.468142 pyvalem-2.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/src/pyvalem/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_data_atomic_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   158055 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_data_isotope_masses.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_special_cases.py
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/atom_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23560 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/formula.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15666 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/stateful_species.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/src/pyvalem/states/
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/_base_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/_state_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10410 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/atomic_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/atomic_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8354 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/diatomic_molecular_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/generic_excited_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/key_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6843 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/molecular_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/racah_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/rotational_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/vibrational_state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/src/pyvalem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/top_level.txt
```

### Comparing `pyvalem-2.5.8/LICENSE` & `pyvalem-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/PKG-INFO` & `pyvalem-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalem
-Version: 2.5.8
+Version: 2.5.9
 Summary: A package for managing simple chemical species and states
 Home-page: https://github.com/xnx/pyvalem
 Author: Christian Hill
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/pyvalem/issues
 Keywords: chemistry,formula,species,state,reaction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvalem-2.5.8/README.rst` & `pyvalem-2.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/pyproject.toml` & `pyvalem-2.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/setup.py` & `pyvalem-2.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 root = Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (root / "README.rst").read_text(encoding="utf-8")
 
 setup(
     name="pyvalem",
-    version="2.5.8",
+    version="2.5.9",
     description="A package for managing simple chemical species and states",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/xnx/pyvalem",
     author="Christian Hill",
     author_email="ch.hill@iaea.org",
     classifiers=[
```

### Comparing `pyvalem-2.5.8/src/pyvalem/_data_atomic_weights.txt` & `pyvalem-2.5.9/src/pyvalem/_data_atomic_weights.txt`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/_data_isotope_masses.txt` & `pyvalem-2.5.9/src/pyvalem/_data_isotope_masses.txt`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/_special_cases.py` & `pyvalem-2.5.9/src/pyvalem/_special_cases.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/_utils.py` & `pyvalem-2.5.9/src/pyvalem/_utils.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/atom_data.py` & `pyvalem-2.5.9/src/pyvalem/atom_data.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/formula.py` & `pyvalem-2.5.9/src/pyvalem/formula.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/reaction.py` & `pyvalem-2.5.9/src/pyvalem/reaction.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/stateful_species.py` & `pyvalem-2.5.9/src/pyvalem/stateful_species.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/__init__.py` & `pyvalem-2.5.9/src/pyvalem/states/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/_base_state.py` & `pyvalem-2.5.9/src/pyvalem/states/_base_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/_state_parser.py` & `pyvalem-2.5.9/src/pyvalem/states/_state_parser.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/atomic_configuration.py` & `pyvalem-2.5.9/src/pyvalem/states/atomic_configuration.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/atomic_term_symbol.py` & `pyvalem-2.5.9/src/pyvalem/states/atomic_term_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/diatomic_molecular_configuration.py` & `pyvalem-2.5.9/src/pyvalem/states/diatomic_molecular_configuration.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/generic_excited_state.py` & `pyvalem-2.5.9/src/pyvalem/states/generic_excited_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/key_value_pair.py` & `pyvalem-2.5.9/src/pyvalem/states/key_value_pair.py`

 * *Files 26% similar despite different names*

```diff
@@ -51,9 +51,12 @@
 
     def __repr__(self):
         return self.state_str
 
     @property
     def ordering(self):
         if self.key == "n":
-            return 0
-        return ord(self.key)
+            # Move up n to the first position for ordering by replacing it with
+            # a space (ASCII 32, the first printable character and not a real valid
+            # key.
+            return " "
+        return self.key
```

### Comparing `pyvalem-2.5.8/src/pyvalem/states/molecular_term_symbol.py` & `pyvalem-2.5.9/src/pyvalem/states/molecular_term_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/racah_symbol.py` & `pyvalem-2.5.9/src/pyvalem/states/racah_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/rotational_state.py` & `pyvalem-2.5.9/src/pyvalem/states/rotational_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem/states/vibrational_state.py` & `pyvalem-2.5.9/src/pyvalem/states/vibrational_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.8/src/pyvalem.egg-info/PKG-INFO` & `pyvalem-2.5.9/src/pyvalem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalem
-Version: 2.5.8
+Version: 2.5.9
 Summary: A package for managing simple chemical species and states
 Home-page: https://github.com/xnx/pyvalem
 Author: Christian Hill
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/pyvalem/issues
 Keywords: chemistry,formula,species,state,reaction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvalem-2.5.8/src/pyvalem.egg-info/SOURCES.txt` & `pyvalem-2.5.9/src/pyvalem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

