# Comparing `tmp/ccs_fit-0.21.8.tar.gz` & `tmp/ccs_fit-0.21.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs_fit-0.21.8.tar", max compression
+gzip compressed data, was "ccs_fit-0.21.9.tar", max compression
```

## Comparing `ccs_fit-0.21.8.tar` & `ccs_fit-0.21.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-06-16 14:35:41.711630 ccs_fit-0.21.8/LICENSE
--rw-r--r--   0        0        0     7898 2023-06-16 14:35:41.711630 ccs_fit-0.21.8/README.md
--rw-r--r--   0        0        0     2483 2023-06-16 14:36:21.067774 ccs_fit-0.21.8/pyproject.toml
--rw-r--r--   0        0        0     1027 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/ase_calculator/buck.py
--rw-r--r--   0        0        0     8028 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
--rw-r--r--   0        0        0    10653 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
--rw-r--r--   0        0        0      488 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/common/__init__.py
--rw-r--r--   0        0        0      628 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/common/exceptions.py
--rw-r--r--   0        0        0     1476 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/common/io.py
--rw-r--r--   0        0        0      486 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/common/math/__init__.py
--rw-r--r--   0        0        0     1071 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/common/math/ewald.py
--rw-r--r--   0        0        0     2156 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/common/neighborlist.py
--rw-r--r--   0        0        0      488 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/data/__init__.py
--rw-r--r--   0        0        0      854 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/data/conversion.py
--rw-r--r--   0        0        0      805 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/debugging_tools/timing.py
--rw-r--r--   0        0        0      488 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/fitting/__init__.py
--rw-r--r--   0        0        0    13479 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/fitting/main copy.py
--rw-r--r--   0        0        0    14597 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/fitting/main.py
--rw-r--r--   0        0        0    23883 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/fitting/objective.py
--rw-r--r--   0        0        0    11717 2023-06-16 14:35:42.687636 ccs_fit-0.21.8/src/ccs_fit/fitting/spline_functions.py
--rw-r--r--   0        0        0    20046 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/ppmd_interface/ccs_ppmd.py
--rw-r--r--   0        0        0     6913 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/regression_tool/regression.py
--rw-r--r--   0        0        0      488 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/__init__.py
--rw-r--r--   0        0        0     7361 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_build_db copy.py
--rw-r--r--   0        0        0     7229 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_build_db.py
--rw-r--r--   0        0        0     8555 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_export_FF.py
--rw-r--r--   0        0        0     4155 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_export_sktable.py
--rw-r--r--   0        0        0     8623 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_fetch.py
--rw-r--r--   0        0        0     2537 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_fit.py
--rw-r--r--   0        0        0     6482 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_prune.py
--rw-r--r--   0        0        0     6754 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_validate.py
--rw-r--r--   0        0        0     1784 2023-06-16 14:35:42.691636 ccs_fit-0.21.8/src/ccs_fit/scripts/jsonTotable.py
--rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 ccs_fit-0.21.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-03 12:56:44.579397 ccs_fit-0.21.9/LICENSE
+-rw-r--r--   0        0        0     7898 2023-08-03 12:56:44.579397 ccs_fit-0.21.9/README.md
+-rw-r--r--   0        0        0     2483 2023-08-03 12:57:23.048105 ccs_fit-0.21.9/pyproject.toml
+-rw-r--r--   0        0        0     1027 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/__init__.py
+-rw-r--r--   0        0        0     9636 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/ase_calculator/buck.py
+-rw-r--r--   0        0        0     8028 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
+-rw-r--r--   0        0        0    10653 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
+-rw-r--r--   0        0        0      488 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/__init__.py
+-rw-r--r--   0        0        0      628 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/exceptions.py
+-rw-r--r--   0        0        0     1476 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/io.py
+-rw-r--r--   0        0        0      486 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/math/__init__.py
+-rw-r--r--   0        0        0     1071 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/math/ewald.py
+-rw-r--r--   0        0        0     2156 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/neighborlist.py
+-rw-r--r--   0        0        0      488 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/data/__init__.py
+-rw-r--r--   0        0        0      854 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/data/conversion.py
+-rw-r--r--   0        0        0      805 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/debugging_tools/timing.py
+-rw-r--r--   0        0        0      488 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/fitting/__init__.py
+-rw-r--r--   0        0        0    13479 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/fitting/main copy.py
+-rw-r--r--   0        0        0    14597 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/fitting/main.py
+-rw-r--r--   0        0        0    23897 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/fitting/objective.py
+-rw-r--r--   0        0        0    11717 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/fitting/spline_functions.py
+-rw-r--r--   0        0        0    20046 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/ppmd_interface/ccs_ppmd.py
+-rw-r--r--   0        0        0     6913 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/regression_tool/regression.py
+-rw-r--r--   0        0        0      488 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/__init__.py
+-rw-r--r--   0        0        0     7361 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db copy.py
+-rw-r--r--   0        0        0     7229 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db.py
+-rw-r--r--   0        0        0     8555 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_FF.py
+-rw-r--r--   0        0        0     4155 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_sktable.py
+-rw-r--r--   0        0        0     8623 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fetch.py
+-rw-r--r--   0        0        0     2537 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fit.py
+-rw-r--r--   0        0        0     6482 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_prune.py
+-rw-r--r--   0        0        0     6754 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_validate.py
+-rw-r--r--   0        0        0     1784 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/jsonTotable.py
+-rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 ccs_fit-0.21.9/PKG-INFO
```

### Comparing `ccs_fit-0.21.8/LICENSE` & `ccs_fit-0.21.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/README.md` & `ccs_fit-0.21.9/README.md`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/pyproject.toml` & `ccs_fit-0.21.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ccs_fit"
-version = "0.21.8"
+version = "0.21.9"
 description = "Fitting tools for repulsive two body interactions using curvature constrained splines."
 authors = [
     "Akshay Krishna AK",
     "Jolla Kullgren <jolla.kullgren@kemi.uu.se>",
     "Eddie Wadbro <eddie.wadbro@umu.se>"
     ]
 maintainers = [
```

### Comparing `ccs_fit-0.21.8/src/ccs_fit/__init__.py` & `ccs_fit-0.21.9/src/ccs_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/ase_calculator/buck.py` & `ccs_fit-0.21.9/src/ccs_fit/ase_calculator/buck.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/ase_calculator/ccs_ase_G2B.py` & `ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_G2B.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/ase_calculator/ccs_ase_calculator.py` & `ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_calculator.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/common/exceptions.py` & `ccs_fit-0.21.9/src/ccs_fit/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/common/io.py` & `ccs_fit-0.21.9/src/ccs_fit/common/io.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/common/math/ewald.py` & `ccs_fit-0.21.9/src/ccs_fit/common/math/ewald.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/common/neighborlist.py` & `ccs_fit-0.21.9/src/ccs_fit/common/neighborlist.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/data/conversion.py` & `ccs_fit-0.21.9/src/ccs_fit/data/conversion.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/debugging_tools/timing.py` & `ccs_fit-0.21.9/src/ccs_fit/debugging_tools/timing.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/fitting/main copy.py` & `ccs_fit-0.21.9/src/ccs_fit/fitting/main copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/fitting/main.py` & `ccs_fit-0.21.9/src/ccs_fit/fitting/main.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/fitting/objective.py` & `ccs_fit-0.21.9/src/ccs_fit/fitting/objective.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,28 +525,28 @@
             two_body_dict["dr"] = self.l_twb[k].res
             r_values = list(np.array(self.l_twb[k].rn))
             two_body_dict["r"] = list(r_values)
             two_body_dict["exp_a"] = self.l_twb[k].expcoeffs[0]
             if not isnan(self.l_twb[k].expcoeffs[1]):
                 two_body_dict["exp_b"] = self.l_twb[k].expcoeffs[1]
             else: 
-                print("WARNING: THE EXPONENTIAL FOR PAIR {} IS POORLY RESOLVED, PROCEED WITH CAUTION!".format(self.l_twb[k].name))
+                # print("WARNING: THE EXPONENTIAL FOR PAIR {} IS POORLY RESOLVED, PROCEED WITH CAUTION!".format(self.l_twb[k].name))
                 two_body_dict["exp_b"] = 0
             if not isnan(self.l_twb[k].expcoeffs[2]):
                 two_body_dict["exp_c"] = self.l_twb[k].expcoeffs[2]
             else: 
                 two_body_dict["exp_c"] = 0
-            if two_body_dict["exp_a"]<0:
-                print("STRONG WARNING: THE EXPONENTIAL WALL IS ACTUALLY ATTRACTIVE!!!!!!!")
+            # if two_body_dict["exp_a"]<0:
+                # print("STRONG WARNING: THE EXPONENTIAL WALL IS ACTUALLY ATTRACTIVE!!!!!!!")
             a_values = list(self.l_twb[k].splcoeffs[:, 0])
             a_values.append(0)
             two_body_dict["spl_a"] = a_values
             b_values = list(self.l_twb[k].splcoeffs[:, 1])
-            if b_values[0]>0:
-                print("WARNING: THE PAIR {} IS ONLY SAMPLED IN A REGION WHERE IT IS STILL REPULSIVE. THIS INDICATES THAT THE INTERACTION IS MOST LIKELY POORLY RESOLVED, PROCEED WITH CAUTION!".format(self.l_twb[k].name))
+            # if b_values[0]>0:
+                # print("WARNING: THE PAIR {} IS ONLY SAMPLED IN A REGION WHERE IT IS STILL REPULSIVE. THIS INDICATES THAT THE INTERACTION IS MOST LIKELY POORLY RESOLVED, PROCEED WITH CAUTION!".format(self.l_twb[k].name))
             b_values.append(0)
             two_body_dict["spl_b"] = b_values
             c_values = list(self.l_twb[k].splcoeffs[:, 2])
             c_values.append(0)
             two_body_dict["spl_c"] = c_values
             d_values = list(self.l_twb[k].splcoeffs[:, 3])
             d_values.append(0)
```

### Comparing `ccs_fit-0.21.8/src/ccs_fit/fitting/spline_functions.py` & `ccs_fit-0.21.9/src/ccs_fit/fitting/spline_functions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/ppmd_interface/ccs_ppmd.py` & `ccs_fit-0.21.9/src/ccs_fit/ppmd_interface/ccs_ppmd.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/regression_tool/regression.py` & `ccs_fit-0.21.9/src/ccs_fit/regression_tool/regression.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_build_db copy.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_build_db.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_export_FF.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_FF.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_export_sktable.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_sktable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_fetch.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fetch.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_fit.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fit.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_prune.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_prune.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/ccs_validate.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_validate.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/src/ccs_fit/scripts/jsonTotable.py` & `ccs_fit-0.21.9/src/ccs_fit/scripts/jsonTotable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.8/PKG-INFO` & `ccs_fit-0.21.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-fit
-Version: 0.21.8
+Version: 0.21.9
 Summary: Fitting tools for repulsive two body interactions using curvature constrained splines.
 Home-page: https://github.com/Teoroo-CMC/CCS
 License: GPL-3
 Keywords: Curvature,Constrained,Splines,Two-Body,Interatomic,Repulsive,Fitting
 Author: Akshay Krishna AK
 Maintainer: Jolla Kullgren
 Maintainer-email: jolla.kullgren@kemi.uu.se
```

