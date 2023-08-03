# Comparing `tmp/radicalpy-0.6.4.tar.gz` & `tmp/radicalpy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.6.4.tar", last modified: Thu Jul 27 08:40:56 2023, max compression
+gzip compressed data, was "radicalpy-0.6.5.tar", last modified: Thu Aug  3 09:33:38 2023, max compression
```

## Comparing `radicalpy-0.6.4.tar` & `radicalpy-0.6.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-27 08:40:45.000000 radicalpy-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-27 08:40:56.683224 radicalpy-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-27 08:40:45.000000 radicalpy-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-27 08:40:45.000000 radicalpy-0.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.679224 radicalpy-0.6.4/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7250 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/classical.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/radicalpy/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/constants.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/radicalpy/data/molecules/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20209 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     9706 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 08:40:45.000000 radicalpy-0.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 08:40:56.683224 radicalpy-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_relaxations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.497286 radicalpy-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-08-03 09:33:28.000000 radicalpy-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-08-03 09:33:38.497286 radicalpy-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-08-03 09:33:28.000000 radicalpy-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-08-03 09:33:28.000000 radicalpy-0.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.493286 radicalpy-0.6.5/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7266 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/classical.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.493286 radicalpy-0.6.5/radicalpy/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.497286 radicalpy-0.6.5/radicalpy/data/molecules/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20384 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9706 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37681 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.493286 radicalpy-0.6.5/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-08-03 09:33:28.000000 radicalpy-0.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 09:33:38.497286 radicalpy-0.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.497286 radicalpy-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_simulation.py
```

### Comparing `radicalpy-0.6.4/LICENSE` & `radicalpy-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/PKG-INFO` & `radicalpy-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.4/README.md` & `radicalpy-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/pyproject.toml` & `radicalpy-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/classical.py` & `radicalpy-0.6.5/radicalpy/classical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 
 from typing import Tuple
 
+import graphviz
 import numpy as np
 import scipy as sp
 
 from . import utils
 
 
 def get_delta_r(mutual_diffusion: float, delta_T: float) -> float:
```

### Comparing `radicalpy-0.6.4/radicalpy/data/constants.json` & `radicalpy-0.6.5/radicalpy/data/constants.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/data/molecules/flavin_anion.json` & `radicalpy-0.6.5/radicalpy/data/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/data/molecules/flavin_neutral.json` & `radicalpy-0.6.5/radicalpy/data/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/data/molecules/tryptophan_cation.json` & `radicalpy-0.6.5/radicalpy/data/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/data/molecules/tyrosine_neutral.json` & `radicalpy-0.6.5/radicalpy/data/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/data/spin_data.json` & `radicalpy-0.6.5/radicalpy/data/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/data.py` & `radicalpy-0.6.5/radicalpy/data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/estimations.py` & `radicalpy-0.6.5/radicalpy/estimations.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,38 +147,50 @@
 
 def autocorrelation_fit(
     ts: np.ndarray,
     trajectory: np.ndarray,
     tau_begin: float,
     tau_end: float,
     num_exp: int = 100,
+    normalise: bool = False,
 ) -> dict:
     """Fit multiexponential to autocorrelation plot and calculate the
     effective rotational correlation time.
 
     Args:
+
         ts (np.ndarray): Time interval (x-axis of the `trajectory`)
             (s).
+
         trajectory (np.ndarray): The raw data which will be fit and
             used to calculate `tau_c`.
+
         tau_begin (float): Initial lag time (s).
+
         tau_end (float): Final lag time (s).
+
         num_exp (int): Number of exponential terms in the
             multiexponential fit (default=100).
 
+        normalise (bool): When set to true, the autocorrelation is
+            normalised (default=False).
+
     Returns:
-            dict:
-                - `fit` is the multiexponential fit to the autocorrelation.
-                - `tau_c` is the effective rotational correlation time.
+        dict:
+
+        - `fit` is the multiexponential fit to the autocorrelation.
+        - `tau_c` is the effective rotational correlation time.
 
+    Thank you, Gesa Grüning!
     """
     acf = autocorrelation(trajectory)
     zero_point_crossing = np.where(np.diff(np.sign(acf)))[0][0]
     acf = acf[0:zero_point_crossing]
-    acf /= acf[0]
+    if normalise:
+        acf /= acf[0]
     taus = np.geomspace(tau_begin, tau_end, num=num_exp)
 
     def multiexponential(x, *params):
         return sum(a * np.exp(-x / t) for a, t in zip(params, taus))
 
     acf_popt, acf_pcov = curve_fit(
         multiexponential,
```

### Comparing `radicalpy-0.6.4/radicalpy/kinetics.py` & `radicalpy-0.6.5/radicalpy/kinetics.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/plot.py` & `radicalpy-0.6.5/radicalpy/plot.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/relaxation.py` & `radicalpy-0.6.5/radicalpy/relaxation.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/shared.py` & `radicalpy-0.6.5/radicalpy/shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy/simulation.py` & `radicalpy-0.6.5/radicalpy/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -283,16 +283,14 @@
 
         Returns:
             np.ndarray:
 
                 Projection operator corresponding to the `State`
                 `state`.
 
-        .. todo:: Write proper docs.
-
         """
         # Spin operators
         SAx, SAy, SAz = [self.spin_operator(0, ax) for ax in "xyz"]
         SBx, SBy, SBz = [self.spin_operator(1, ax) for ax in "xyz"]
 
         # Product operators
         SASB = self.product_operator(0, 1)
@@ -674,16 +672,16 @@
             raise ValueError("Observable state should not be EQUILIBRIUM")
         obs = self.observable_projection_operator(obs)
         return np.real(np.trace(obs @ rhos, axis1=-2, axis2=-1))
 
     @staticmethod
     def product_yield(product_probability, time, k):
         """Calculate the product yield and the product yield sum."""
-        product_yield = sp.integrate.cumtrapz(product_probability, time, initial=0) * k
-        product_yield_sum = np.trapz(product_probability, dx=time[1]) * k
+        product_yield = k * sp.integrate.cumtrapz(product_probability, time, initial=0)
+        product_yield_sum = k * np.trapz(product_probability, dx=time[1])
         return product_yield, product_yield_sum
 
     def apply_liouville_hamiltonian_modifiers(self, H, modifiers):
         for K in modifiers:  # skip in hilbert
             K.init(self)
             K.adjust_hamiltonian(H)
 
@@ -793,59 +791,145 @@
             HFE=HFE,
         )
 
     def anisotropy_loop(
         self,
         init_state: State,
         time: np.ndarray,
-        B: float,
+        B0: float,
         H_base: np.ndarray,
-        theta: float | np.ndarray,
-        phi: float | np.ndarray,
-    ):
+        theta: np.ndarray,
+        phi: np.ndarray,
+    ) -> np.ndarray:
+        """Inner loop of anisotropy experiment.
+
+        Args:
+
+            init_state (State): Initial `State` of the density matrix.
+
+            time (np.ndarray): An sequence of (uniform) time points,
+                usually created using `np.arange` or `np.linspace`.
+
+            B0 (float): External magnetic field intensity (milli
+                Tesla) (see `zeeman_hamiltonian`).
+
+            H_base (np.ndarray): A "base" Hamiltonian, i.e., the
+                Zeeman Hamiltonian will be added to this base, usually
+                obtained with `total_hamiltonian` and `B0=0`.
+
+            theta (np.ndarray): rotation (polar) angle between the
+                external magnetic field and the fixed molecule. See
+                `zeeman_hamiltonian_3d`.
+
+            phi (np.ndarray): rotation (azimuth) angle between the
+                external magnetic field and the fixed molecule. See
+                `zeeman_hamiltonian_3d`.
+
+        Returns:
+            np.ndarray:
+
+            A tensor which has a series of density matrices for each
+            angle `theta` and `phi` obtained by running
+            `time_evolution` for each of them (with `time`
+            time\-steps, `B0` magnetic intensity).
+
+        """
         shape = self._get_rho_shape(H_base.shape[0])
         rhos = np.zeros((len(theta), len(phi), len(time), *shape), dtype=complex)
 
         iters = itertools.product(enumerate(theta), enumerate(phi))
         for (i, th), (j, ph) in tqdm(list(iters)):
-            H_zee = self.zeeman_hamiltonian(B, th, ph)
+            H_zee = self.zeeman_hamiltonian(B0, th, ph)
             H = H_base + self.convert(H_zee)
             rhos[i, j] = self.time_evolution(init_state, time, H)
         return rhos
 
     def anisotropy(
         self,
         init_state: State,
         obs_state: State,
         time: np.ndarray,
         theta: np.ndarray | float,
         phi: np.ndarray | float,
-        B: float,
+        B0: float,
         D: np.ndarray,
         J: float,
         kinetics: list[HilbertIncoherentProcessBase] = [],
         relaxations: list[HilbertIncoherentProcessBase] = [],
     ) -> dict:
+        """Anisotropy experiment.
+
+        Args:
+
+            init_state (State): Initial `State` of the density matrix.
+
+            obs_state (State): Observable `State` of the density matrix.
+
+            time (np.ndarray): An sequence of (uniform) time points,
+                usually created using `np.arange` or `np.linspace`.
+
+            H_base (np.ndarray): A "base" Hamiltonian, i.e., the
+                Zeeman Hamiltonian will be added to this base, usually
+                obtained with `total_hamiltonian` and `B0=0`.
+
+            theta (np.ndarray): rotation (polar) angle between the
+                external magnetic field and the fixed molecule. See
+                `zeeman_hamiltonian_3d`.
+
+            B0 (float): External magnetic field intensity (milli
+                Tesla) (see `zeeman_hamiltonian`).
+
+            phi (np.ndarray): rotation (azimuth) angle between the
+                external magnetic field and the fixed molecule. See
+                `zeeman_hamiltonian_3d`.
+
+            D (np.ndarray): Dipolar coupling constant (see
+                `dipolar_hamiltonian`).
+
+            J (float): Exchange coupling constant (see
+                `exchange_hamiltonian`).
+
+            kinetics (list): A list of kinetic (super)operators of
+                type `radicalpy.kinetics.HilbertKineticsBase` or
+                `radicalpy.kinetics.LiouvilleKineticsBase`.
+
+            relaxations (list): A list of relaxation superoperators of
+                type `radicalpy.relaxation.LiouvilleRelaxationBase`.
+
+        Returns:
+            dict:
+
+            - time: the original `time` object
+            - B0: `B0` parameter
+            - theta: `theta` parameter
+            - phi: `phi` parameter
+            - rhos: tensor of sequences of time evolution of density
+              matrices
+            - time_evolutions: product probabilities
+            - product_yields: product yields
+            - product_yield_sums: product yield sums
+
+        """
         H = self.total_hamiltonian(B0=0, D=D, J=J, hfc_anisotropy=True)
 
         self.apply_liouville_hamiltonian_modifiers(H, kinetics + relaxations)
         theta, phi = utils.anisotropy_check(theta, phi)
-        rhos = self.anisotropy_loop(init_state, time, B, H, theta=theta, phi=phi)
+        rhos = self.anisotropy_loop(init_state, time, B0, H, theta=theta, phi=phi)
         product_probabilities = self.product_probability(obs_state, rhos)
 
         self.apply_hilbert_kinetics(time, product_probabilities, kinetics)
         k = kinetics[0].rate_constant if kinetics else 1.0
         product_yields, product_yield_sums = self.product_yield(
             product_probabilities, time, k
         )
         rhos = self._square_liouville_rhos(rhos)
 
         return dict(
             time=time,
-            B=B,
+            B0=B0,
             theta=theta,
             phi=phi,
             rhos=rhos,
             time_evolutions=product_probabilities,
             product_yields=product_yields,
             product_yield_sums=product_yield_sums,
         )
```

### Comparing `radicalpy-0.6.4/radicalpy/utils.py` & `radicalpy-0.6.5/radicalpy/utils.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/radicalpy.egg-info/PKG-INFO` & `radicalpy-0.6.5/radicalpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.4/radicalpy.egg-info/SOURCES.txt` & `radicalpy-0.6.5/radicalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/tests/test_data.py` & `radicalpy-0.6.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/tests/test_estimations.py` & `radicalpy-0.6.5/tests/test_estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/tests/test_shared.py` & `radicalpy-0.6.5/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.4/tests/test_simulation.py` & `radicalpy-0.6.5/tests/test_simulation.py`

 * *Files identical despite different names*

