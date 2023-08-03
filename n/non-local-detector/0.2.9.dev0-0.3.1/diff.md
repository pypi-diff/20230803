# Comparing `tmp/non_local_detector-0.2.9.dev0.tar.gz` & `tmp/non_local_detector-0.3.1.tar.gz`

## Comparing `non_local_detector-0.2.9.dev0.tar` & `non_local_detector-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/.gitattributes
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/environment.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/environment_gpu.yml
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/.github/workflows/test_package_build.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/.vscode/settings.json
--rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test.ipynb
--rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_clusterless.ipynb
--rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_non_local.ipynb
--rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_non_local_2D.ipynb
--rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_non_local_spike_times.ipynb
--rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
--rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_simulated.ipynb
--rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_simulated2.ipynb
--rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_sorted_spikes.ipynb
--rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/notebooks/test_spike_times.ipynb
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/_version.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/continuous_state_transitions.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/core.py
--rw-r--r--   0        0        0    19344 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/discrete_state_transitions.py
--rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/environment.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/initial_conditions.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/observation_models.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/types.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/visualization.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/__init__.py
--rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/no_spike.py
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/models/__init__.py
--rw-r--r--   0        0        0    51343 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/models/base.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/models/cont_frag_model.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/models/decoder.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/models/multienvironment_model.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/models/non_local_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/__init__.py
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/clusterless_simulation.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/simulate.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/src/non_local_detector/tests/test_version_import.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/LICENSE
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/README.md
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/pyproject.toml
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 non_local_detector-0.2.9.dev0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/.gitattributes
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/environment.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/environment_gpu.yml
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/.github/workflows/test_package_build.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test.ipynb
+-rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_clusterless.ipynb
+-rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_non_local.ipynb
+-rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_non_local_2D.ipynb
+-rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_non_local_spike_times.ipynb
+-rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_non_stationary_discrete_transition.ipynb
+-rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_simulated.ipynb
+-rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_simulated2.ipynb
+-rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_sorted_spikes.ipynb
+-rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/notebooks/test_spike_times.ipynb
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/_version.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/continuous_state_transitions.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/core.py
+-rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/discrete_state_transitions.py
+-rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/environment.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/initial_conditions.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/observation_models.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/types.py
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/visualization.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/likelihoods/__init__.py
+-rw-r--r--   0        0        0    16767 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/likelihoods/clusterless_kde.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/likelihoods/no_spike.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/likelihoods/sorted_spikes_glm.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/likelihoods/sorted_spikes_kde.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/models/__init__.py
+-rw-r--r--   0        0        0    51315 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/models/base.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/models/cont_frag_model.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/models/decoder.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/models/multienvironment_model.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/models/non_local_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/simulate/__init__.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/simulate/clusterless_simulation.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/simulate/simulate.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/simulate/sorted_spikes_simulation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/src/non_local_detector/tests/test_version_import.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/LICENSE
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 non_local_detector-0.3.1/PKG-INFO
```

### Comparing `non_local_detector-0.2.9.dev0/.github/workflows/test_package_build.yml` & `non_local_detector-0.3.1/.github/workflows/test_package_build.yml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test.ipynb` & `non_local_detector-0.3.1/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_clusterless.ipynb` & `non_local_detector-0.3.1/notebooks/test_clusterless.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_non_local.ipynb` & `non_local_detector-0.3.1/notebooks/test_non_local.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_non_local_2D.ipynb` & `non_local_detector-0.3.1/notebooks/test_non_local_2D.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_non_local_spike_times.ipynb` & `non_local_detector-0.3.1/notebooks/test_non_local_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_non_stationary_discrete_transition.ipynb` & `non_local_detector-0.3.1/notebooks/test_non_stationary_discrete_transition.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_simulated.ipynb` & `non_local_detector-0.3.1/notebooks/test_simulated.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_simulated2.ipynb` & `non_local_detector-0.3.1/notebooks/test_simulated2.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_sorted_spikes.ipynb` & `non_local_detector-0.3.1/notebooks/test_sorted_spikes.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/notebooks/test_spike_times.ipynb` & `non_local_detector-0.3.1/notebooks/test_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/continuous_state_transitions.py` & `non_local_detector-0.3.1/src/non_local_detector/continuous_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/core.py` & `non_local_detector-0.3.1/src/non_local_detector/core.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/discrete_state_transitions.py` & `non_local_detector-0.3.1/src/non_local_detector/discrete_state_transitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -484,14 +484,46 @@
 
         """
         diag = np.asarray(self.diagonal_values)
         return make_transition_from_diag(diag), None, None
 
 
 @dataclass
+class DiscreteStationaryCustom:
+    """Creates a custom discrete transition matrix.
+
+
+    Attributes
+    ----------
+    values : np.ndarray, shape (n_states, n_states)
+        The values of the transition matrix.
+
+    """
+
+    values: np.ndarray
+
+    def make_state_transition(self, *args, **kwargs) -> tuple[np.ndarray, None, None]:
+        """Constructs the initial discrete transition matrix.
+
+        Returns
+        -------
+        discrete_transition : np.ndarray, shape (n_states, n_states)
+            The initial discrete transition matrix.
+        discrete_transition_coefficients : None
+            The coefficients for the non-stationary transition matrix.
+            It is None here because the transition matrix is stationary.
+        discrete_transition_design_matrix : None
+            The design matrix for the non-stationary transition matrix.
+            It is None here because the transition matrix is stationary.
+
+        """
+        return np.asarray(self.values), None, None
+
+
+@dataclass
 class DiscreteNonStationaryDiagonal:
     """Covariate driven transition matrix that changes over time.
 
     Initialized with a stationary diagonal matrix.
 
     Off-diagonals are probability: (1 - `diagonal_value`) / (`n_states` - 1)
```

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/environment.py` & `non_local_detector-0.3.1/src/non_local_detector/environment.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/initial_conditions.py` & `non_local_detector-0.3.1/src/non_local_detector/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/observation_models.py` & `non_local_detector-0.3.1/src/non_local_detector/observation_models.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/types.py` & `non_local_detector-0.3.1/src/non_local_detector/types.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/__init__.py` & `non_local_detector-0.3.1/src/non_local_detector/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/clusterless_kde.py` & `non_local_detector-0.3.1/src/non_local_detector/likelihoods/clusterless_kde.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,16 +41,14 @@
 
 def block_kde(
     eval_points: jnp.ndarray,
     samples: jnp.ndarray,
     std: jnp.ndarray,
     block_size: int = 100,
 ) -> jnp.ndarray:
-    if eval_points.shape[1] != samples.shape[1] or std.shape[0] != samples.shape[1]:
-        raise ValueError("Dimension mismatch between eval_points, samples, and std")
     n_eval_points = eval_points.shape[0]
     density = jnp.zeros((n_eval_points,))
     for start_ind in range(0, n_eval_points, block_size):
         block_inds = slice(start_ind, start_ind + block_size)
         density = jax.lax.dynamic_update_slice(
             density,
             kde(eval_points[block_inds], samples, std).squeeze(),
@@ -60,16 +58,14 @@
     return density
 
 
 def kde_distance(
     eval_points: jnp.ndarray, samples: jnp.ndarray, std: jnp.ndarray
 ) -> jnp.ndarray:
     distance = jnp.ones((samples.shape[0], eval_points.shape[0]))
-    if eval_points.shape[1] != samples.shape[1] or std.shape[0] != samples.shape[1]:
-        raise ValueError("Dimension mismatch between eval_points, samples, and std")
     for dim_eval_points, dim_samples, dim_std in zip(eval_points.T, samples.T, std):
         distance *= gaussian_pdf(
             jnp.expand_dims(dim_eval_points, axis=0),
             jnp.expand_dims(dim_samples, axis=1),
             dim_std,
         )
     return distance
@@ -221,15 +217,18 @@
     position_std: float = 6.0,
     waveform_std: float = 24.0,
     block_size: int = 100,
     disable_progress_bar: bool = False,
 ):
     position = position if position.ndim > 1 else jnp.expand_dims(position, axis=1)
     if isinstance(position_std, (int, float)):
-        position_std = jnp.array([position_std] * position.shape[1])
+        if environment.track_graph is not None and position.shape[1] > 1:
+            position_std = jnp.array([position_std])
+        else:
+            position_std = jnp.array([position_std] * position.shape[1])
     if isinstance(waveform_std, (int, float)):
         waveform_std = jnp.array([waveform_std] * spike_waveform_features[0].shape[1])
 
     is_track_interior = environment.is_track_interior_.ravel(order="F")
     interior_place_bin_centers = environment.place_bin_centers_[is_track_interior]
 
     if environment.track_graph is not None and position.shape[1] > 1:
@@ -321,75 +320,31 @@
     is_local: bool = False,
     block_size: int = 100,
     disable_progress_bar: bool = False,
 ):
     n_time = len(time)
 
     if is_local:
-        # Need to interpolate position
-        interpolated_position = get_position_at_time(
-            position_time, position, time, environment
-        )
-        occupancy = occupancy_model.predict(interpolated_position)
-
-        log_likelihood = jnp.zeros((n_time, 1))
-        for (
-            electrode_encoding_spike_waveform_features,
-            electrode_encoding_positions,
-            electrode_mean_rate,
-            electrode_gpi_model,
-            electrode_decoding_spike_waveform_features,
-            electrode_spike_times,
-        ) in zip(
-            tqdm(
-                encoding_spike_waveform_features,
-                unit="electrode",
-                desc="Local Likelihood",
-                disable=disable_progress_bar,
-            ),
+        log_likelihood = compute_local_log_likelihood(
+            time,
+            position_time,
+            position,
+            spike_times,
+            spike_waveform_features,
+            occupancy_model,
+            gpi_models,
+            encoding_spike_waveform_features,
             encoding_positions,
+            environment,
             mean_rates,
-            gpi_models,
-            spike_waveform_features,
-            spike_times,
-        ):
-            is_in_bounds = jnp.logical_and(
-                electrode_spike_times >= time[0],
-                electrode_spike_times <= time[-1],
-            )
-            electrode_spike_times = electrode_spike_times[is_in_bounds]
-            electrode_decoding_spike_waveform_features = (
-                electrode_decoding_spike_waveform_features[is_in_bounds]
-            )
-            position_distance = kde_distance(
-                interpolated_position,
-                electrode_encoding_positions,
-                std=position_std,
-            )
-
-            log_likelihood += jax.ops.segment_sum(
-                block_estimate_log_joint_mark_intensity(
-                    electrode_decoding_spike_waveform_features,
-                    electrode_encoding_spike_waveform_features,
-                    waveform_std,
-                    occupancy,
-                    electrode_mean_rate,
-                    position_distance,
-                    block_size,
-                ),
-                get_spike_time_bin_ind(electrode_spike_times, time),
-                indices_are_sorted=False,
-                num_segments=n_time,
-            )
-
-            log_likelihood -= electrode_mean_rate * jnp.where(
-                occupancy > 0.0,
-                electrode_gpi_model.predict(interpolated_position) / occupancy,
-                0.0,
-            )
+            position_std,
+            waveform_std,
+            block_size,
+            disable_progress_bar,
+        )
     else:
         is_track_interior = environment.is_track_interior_.ravel(order="F")
         interior_place_bin_centers = environment.place_bin_centers_[is_track_interior]
 
         log_likelihood = (
             jnp.zeros((is_track_interior.shape[0],))
             .at[is_track_interior]
@@ -441,7 +396,107 @@
                     get_spike_time_bin_ind(electrode_spike_times, time),
                     indices_are_sorted=False,
                     num_segments=n_time,
                 )
             )
 
     return log_likelihood
+
+
+def compute_local_log_likelihood(
+    time: jnp.ndarray,
+    position_time: jnp.ndarray,
+    position: jnp.ndarray,
+    spike_times: list[jnp.ndarray],
+    spike_waveform_features: list[jnp.ndarray],
+    occupancy_model,
+    gpi_models,
+    encoding_spike_waveform_features,
+    encoding_positions,
+    environment,
+    mean_rates,
+    position_std,
+    waveform_std,
+    block_size: int = 100,
+    disable_progress_bar: bool = False,
+):
+    # Need to interpolate position
+    interpolated_position = get_position_at_time(
+        position_time, position, time, environment
+    )
+    occupancy = occupancy_model.predict(interpolated_position)
+
+    n_time = len(time)
+    log_likelihood = jnp.zeros((n_time,))
+    for (
+        electrode_encoding_spike_waveform_features,
+        electrode_encoding_positions,
+        electrode_mean_rate,
+        electrode_gpi_model,
+        electrode_decoding_spike_waveform_features,
+        electrode_spike_times,
+    ) in zip(
+        tqdm(
+            encoding_spike_waveform_features,
+            unit="electrode",
+            desc="Local Likelihood",
+            disable=disable_progress_bar,
+        ),
+        encoding_positions,
+        mean_rates,
+        gpi_models,
+        spike_waveform_features,
+        spike_times,
+    ):
+        is_in_bounds = jnp.logical_and(
+            electrode_spike_times >= time[0],
+            electrode_spike_times <= time[-1],
+        )
+        electrode_spike_times = electrode_spike_times[is_in_bounds]
+        electrode_decoding_spike_waveform_features = (
+            electrode_decoding_spike_waveform_features[is_in_bounds]
+        )
+
+        position_at_spike_time = get_position_at_time(
+            position_time, position, electrode_spike_times, environment
+        )
+
+        marginal_density = block_kde(
+            eval_points=jnp.concatenate(
+                (
+                    position_at_spike_time,
+                    electrode_decoding_spike_waveform_features,
+                ),
+                axis=1,
+            ),
+            samples=jnp.concatenate(
+                (
+                    electrode_encoding_positions,
+                    electrode_encoding_spike_waveform_features,
+                ),
+                axis=1,
+            ),
+            std=jnp.concatenate((position_std, waveform_std)),
+            block_size=block_size,
+        )
+        occupancy_at_spike_time = occupancy_model.predict(position_at_spike_time)
+
+        log_likelihood += jax.ops.segment_sum(
+            jnp.log(
+                electrode_mean_rate
+                * jnp.where(
+                    occupancy_at_spike_time > 0.0,
+                    marginal_density / occupancy_at_spike_time,
+                    0.0,
+                )
+            ),
+            get_spike_time_bin_ind(electrode_spike_times, time),
+            indices_are_sorted=False,
+            num_segments=n_time,
+        )
+
+        log_likelihood -= electrode_mean_rate * jnp.where(
+            occupancy > 0.0,
+            electrode_gpi_model.predict(interpolated_position) / occupancy,
+            0.0,
+        )
+    return log_likelihood[:, jnp.newaxis]
```

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/no_spike.py` & `non_local_detector-0.3.1/src/non_local_detector/likelihoods/no_spike.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py` & `non_local_detector-0.3.1/src/non_local_detector/likelihoods/sorted_spikes_glm.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py` & `non_local_detector-0.3.1/src/non_local_detector/likelihoods/sorted_spikes_kde.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,21 @@
     spike_times: list[jnp.ndarray],
     environment: Environment,
     sampling_frequency: int = 500,
     position_std: float = 6.0,
     block_size: int = 100,
     disable_progress_bar: bool = False,
 ):
+    position = position if position.ndim > 1 else jnp.expand_dims(position, axis=1)
+    if isinstance(position_std, (int, float)):
+        if environment.track_graph is not None and position.shape[1] > 1:
+            position_std = jnp.array([position_std])
+        else:
+            position_std = jnp.array([position_std] * position.shape[1])
+
     is_track_interior = environment.is_track_interior_.ravel(order="F")
     interior_place_bin_centers = environment.place_bin_centers_[is_track_interior]
 
     if environment.track_graph is not None and position.shape[1] > 1:
         # convert to 1D
         position1D = get_linearized_position(
             position,
@@ -154,17 +161,18 @@
         neuron_marginal_model = KDEModel(std=position_std, block_size=block_size).fit(
             get_position_at_time(
                 position_time, position, neuron_spike_times, environment
             )
         )
         marginal_models.append(neuron_marginal_model)
         marginal_density = neuron_marginal_model.predict(interior_place_bin_centers)
-        place_field = jnp.zeros((is_track_interior.shape[0],))
         place_fields.append(
-            place_field.at[is_track_interior].set(
+            jnp.zeros((is_track_interior.shape[0],))
+            .at[is_track_interior]
+            .set(
                 jnp.clip(
                     mean_rates[-1]
                     * jnp.where(occupancy > 0.0, marginal_density / occupancy, EPS),
                     a_min=EPS,
                     a_max=None,
                 )
             )
@@ -261,15 +269,16 @@
                 )
             ]
             spike_count_per_time_bin = np.bincount(
                 np.digitize(neuron_spike_times, time[1:-1]),
                 minlength=time.shape[0],
             )
             log_likelihood += jax.scipy.special.xlogy(
-                spike_count_per_time_bin[:, jnp.newaxis], place_field[jnp.newaxis]
+                jnp.expand_dims(spike_count_per_time_bin, axis=1),
+                jnp.expand_dims(place_field, axis=0),
             )
-        log_likelihood -= no_spike_part_log_likelihood[jnp.newaxis]
+        log_likelihood -= no_spike_part_log_likelihood
         log_likelihood = jnp.where(
             is_track_interior[jnp.newaxis, :], log_likelihood, jnp.log(EPS)
         )
 
     return log_likelihood
```

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/models/__init__.py` & `non_local_detector-0.3.1/src/non_local_detector/models/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/models/base.py` & `non_local_detector-0.3.1/src/non_local_detector/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 _DEFAULT_CLUSTERLESS_ALGORITHM_PARAMS = {
     "waveform_std": 24.0,
     "position_std": 6.0,
     "block_size": 10_000,
 }
 _DEFAULT_SORTED_SPIKES_ALGORITHM_PARAMS = {
     "position_std": 6.0,
-    "use_diffusion": False,
     "block_size": 10_000,
 }
 
 State = namedtuple("state", ("environment_name", "encoding_group"))
 
 
 class _DetectorBase(BaseEstimator):
```

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/models/cont_frag_model.py` & `non_local_detector-0.3.1/src/non_local_detector/models/cont_frag_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/models/decoder.py` & `non_local_detector-0.3.1/src/non_local_detector/models/decoder.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/models/multienvironment_model.py` & `non_local_detector-0.3.1/src/non_local_detector/models/multienvironment_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/models/non_local_model.py` & `non_local_detector-0.3.1/src/non_local_detector/models/non_local_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from non_local_detector.continuous_state_transitions import (
     Discrete,
     RandomWalk,
     Uniform,
 )
-from non_local_detector.discrete_state_transitions import DiscreteStationaryDiagonal
+from non_local_detector.discrete_state_transitions import DiscreteStationaryCustom
 from non_local_detector.environment import Environment
 from non_local_detector.initial_conditions import UniformInitialConditions
 from non_local_detector.models.base import (
     _DEFAULT_CLUSTERLESS_ALGORITHM_PARAMS,
     _DEFAULT_SORTED_SPIKES_ALGORITHM_PARAMS,
     ClusterlessDetector,
     SortedSpikesDetector,
@@ -46,18 +46,56 @@
     UniformInitialConditions(),
     UniformInitialConditions(),
     UniformInitialConditions(),
 ]
 
 discrete_transition_stickiness = np.array([30.0, 100_000.0, 30.0, 200.0])
 
-discrete_transition_type = DiscreteStationaryDiagonal(
-    diagonal_values=np.array([0.90, 0.90, 0.90, 0.98])
+# transition probability to no spike state
+no_spike_trans_prob = 1e-5
+# probability of staying in local or continuous non-local state
+local_prob = cont_non_local_prob = 0.9
+# probability of staying in non-local fragmented state
+non_local_frag_prob = 0.98
+# probability of staying in no-spike state
+no_spike_prob = 0.99
+
+discrete_transition_type = DiscreteStationaryCustom(
+    values=np.array(
+        [
+            [
+                local_prob,
+                no_spike_trans_prob,
+                (1 - local_prob - no_spike_trans_prob) / 2,
+                (1 - local_prob - no_spike_trans_prob) / 2,
+            ],
+            [
+                (1 - no_spike_prob) / 3,
+                no_spike_prob,
+                (1 - no_spike_prob) / 3,
+                (1 - no_spike_prob) / 3,
+            ],
+            [
+                (1 - cont_non_local_prob - no_spike_trans_prob) / 2,
+                no_spike_trans_prob,
+                cont_non_local_prob,
+                (1 - cont_non_local_prob - no_spike_trans_prob) / 2,
+            ],
+            [
+                (1 - non_local_frag_prob - no_spike_trans_prob) / 2,
+                no_spike_trans_prob,
+                (1 - non_local_frag_prob - no_spike_trans_prob) / 2,
+                non_local_frag_prob,
+            ],
+        ]
+    )
 )
 
+no_spike_rate = 1e-50
+
 state_names = [
     "Local",
     "No-Spike",
     "Non-Local Continuous",
     "Non-Local Fragmented",
 ]
 
@@ -74,16 +112,16 @@
         continuous_transition_types: ContinuousTransitions = continuous_transition_types,
         observation_models: Observations = observation_models,
         environments: Environments = environment,
         sorted_spikes_algorithm: str = "sorted_spikes_kde",
         sorted_spikes_algorithm_params: dict = _DEFAULT_SORTED_SPIKES_ALGORITHM_PARAMS,
         infer_track_interior: bool = True,
         state_names: list[str] | None = state_names,
-        sampling_frequency: float = 500,
-        no_spike_rate: float = 1e-10,
+        sampling_frequency: float = 500.0,
+        no_spike_rate: float = no_spike_rate,
     ):
         super().__init__(
             discrete_initial_conditions,
             continuous_initial_conditions_types,
             discrete_transition_type,
             discrete_transition_concentration,
             discrete_transition_stickiness,
@@ -113,15 +151,15 @@
         observation_models: Observations = observation_models,
         environments: Environments = environment,
         clusterless_algorithm: str = "clusterless_kde",
         clusterless_algorithm_params: dict = _DEFAULT_CLUSTERLESS_ALGORITHM_PARAMS,
         infer_track_interior: bool = True,
         state_names: list[str] | None = state_names,
         sampling_frequency: float = 500.0,
-        no_spike_rate: float = 1e-10,
+        no_spike_rate: float = no_spike_rate,
     ):
         super().__init__(
             discrete_initial_conditions,
             continuous_initial_conditions_types,
             discrete_transition_type,
             discrete_transition_concentration,
             discrete_transition_stickiness,
```

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/clusterless_simulation.py` & `non_local_detector-0.3.1/src/non_local_detector/simulate/clusterless_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/simulate.py` & `non_local_detector-0.3.1/src/non_local_detector/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py` & `non_local_detector-0.3.1/src/non_local_detector/simulate/sorted_spikes_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/.gitignore` & `non_local_detector-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/LICENSE` & `non_local_detector-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/pyproject.toml` & `non_local_detector-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.9.dev0/PKG-INFO` & `non_local_detector-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non_local_detector
-Version: 0.2.9.dev0
+Version: 0.3.1
 Summary: A python package to decode non-local activity from neural data
 Project-URL: Homepage, https://github.com/LorenFrankLab/non_local_detector
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/non_local_detector/issues
 Author-email: Eric Denovellis <eric.denovellis@ucsf.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Denovellis
```

