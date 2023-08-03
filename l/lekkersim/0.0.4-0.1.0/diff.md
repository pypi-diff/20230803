# Comparing `tmp/lekkersim-0.0.4.tar.gz` & `tmp/lekkersim-0.1.0.tar.gz`

## Comparing `lekkersim-0.0.4.tar` & `lekkersim-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,14 @@
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 lekkersim-0.0.4/.readthedocs.yaml
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 lekkersim-0.0.4/localdocs
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 lekkersim-0.0.4/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/Makefile
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/api_summary.rst
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/conf.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/how_it_works.rst
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/index.rst
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/installation.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/make.bat
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/reference-manual.rst
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/requirements.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/_static/theme_overrides.css
--rw-r--r--   0        0        0   563355 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/Basic_usage.ipynb
--rw-r--r--   0        0        0   150477 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/Monitors.ipynb
--rw-r--r--   0        0        0   555001 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/Nazca Integration.ipynb
--rw-r--r--   0        0        0   140393 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/Nazca Multiple Polarization.ipynb
--rw-r--r--   0        0        0   513419 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/Parametric.ipynb
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/Smatrix.png
--rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/debug.ipynb
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lekkersim-0.0.4/Docs/jupyter/examples.rst
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/_version.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/log.py
--rw-r--r--   0        0        0    60544 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/model.py
--rw-r--r--   0        0        0    25346 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/nazca_integration.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/scattering.py
--rw-r--r--   0        0        0    33043 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/sol.py
--rw-r--r--   0        0        0    23721 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/structure.py
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 lekkersim-0.0.4/lekkersim/utils.py
--rw-r--r--   0        0        0    14587 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/skip_models_generation.py
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/skip_nazca.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_basic.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_export_sm.py
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_flatten.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_fpr_gaussian.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_monitor.py
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_params.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_solver.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/test_split.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/references/s_matrix_fpr_gaussian.pkl
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pytest/references/s_matrix_fpr_gaussian_asym.pkl
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 lekkersim-0.0.4/.gitignore
--rw-r--r--   0        0        0    34283 2020-02-02 00:00:00.000000 lekkersim-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 lekkersim-0.0.4/README.md
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 lekkersim-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 lekkersim-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/_version.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/log.py
+-rw-r--r--   0        0        0    60544 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/model.py
+-rw-r--r--   0        0        0    25346 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/nazca_integration.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/scattering.py
+-rw-r--r--   0        0        0    33043 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/sol.py
+-rw-r--r--   0        0        0    23721 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/structure.py
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 lekkersim-0.1.0/lekkersim/utils.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 lekkersim-0.1.0/.gitignore
+-rw-r--r--   0        0        0    34283 2020-02-02 00:00:00.000000 lekkersim-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 lekkersim-0.1.0/README.md
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 lekkersim-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 lekkersim-0.1.0/PKG-INFO
```

### Comparing `lekkersim-0.0.4/lekkersim/__init__.py` & `lekkersim-0.1.0/lekkersim/__init__.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/log.py` & `lekkersim-0.1.0/lekkersim/log.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/model.py` & `lekkersim-0.1.0/lekkersim/model.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/nazca_integration.py` & `lekkersim-0.1.0/lekkersim/nazca_integration.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/scattering.py` & `lekkersim-0.1.0/lekkersim/scattering.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/sol.py` & `lekkersim-0.1.0/lekkersim/sol.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/structure.py` & `lekkersim-0.1.0/lekkersim/structure.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/lekkersim/utils.py` & `lekkersim-0.1.0/lekkersim/utils.py`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/LICENSE.md` & `lekkersim-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/README.md` & `lekkersim-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lekkersim-0.0.4/pyproject.toml` & `lekkersim-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 doc = [
   "sphinx>=5.3.0",
   "sphinx-rtd-theme>=1.1.1",
   "nbsphinx>=0.8.12",
   "notebook>=6.5.2",
 ]
 
+[tool.hatch.build]
+include = [
+  "lekkersim/*",
+]
+
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 version_scheme = "post-release"
 
 [tool.hatch.build.hooks.vcs]
```

### Comparing `lekkersim-0.0.4/PKG-INFO` & `lekkersim-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lekkersim
-Version: 0.0.4
+Version: 0.1.0
 Summary: The lekker tool for photonic circuit simulation.
 Author-email: Marco Passoni <mpasson91@gmail.com>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE.md
 Keywords: photonic circuits,photonics,scattering matrix,simulation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

