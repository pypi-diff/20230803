# Comparing `tmp/alns-5.3.0.tar.gz` & `tmp/alns-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alns-5.3.0.tar", max compression
+gzip compressed data, was "alns-5.3.1.tar", max compression
```

## Comparing `alns-5.3.0.tar` & `alns-5.3.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1095 2023-06-23 14:18:28.746303 alns-5.3.0/LICENSE.md
--rw-r--r--   0        0        0     5673 2023-06-23 14:18:28.746303 alns-5.3.0/README.md
--rw-r--r--   0        0        0    11418 2023-06-23 14:18:28.746303 alns-5.3.0/alns/ALNS.py
--rw-r--r--   0        0        0      495 2023-06-23 14:18:28.746303 alns-5.3.0/alns/Outcome.py
--rw-r--r--   0        0        0     5366 2023-06-23 14:18:28.746303 alns-5.3.0/alns/Result.py
--rw-r--r--   0        0        0      637 2023-06-23 14:18:28.746303 alns-5.3.0/alns/State.py
--rw-r--r--   0        0        0     3975 2023-06-23 14:18:28.746303 alns-5.3.0/alns/Statistics.py
--rw-r--r--   0        0        0       89 2023-06-23 14:18:28.746303 alns-5.3.0/alns/__init__.py
--rw-r--r--   0        0        0      885 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/AcceptanceCriterion.py
--rw-r--r--   0        0        0     2266 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/AdaptiveThreshold.py
--rw-r--r--   0        0        0     1855 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/GreatDeluge.py
--rw-r--r--   0        0        0      276 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/HillClimbing.py
--rw-r--r--   0        0        0     2481 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/LateAcceptanceHillClimbing.py
--rw-r--r--   0        0        0     3545 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/NonLinearGreatDeluge.py
--rw-r--r--   0        0        0      179 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/RandomWalk.py
--rw-r--r--   0        0        0     6082 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/RecordToRecordTravel.py
--rw-r--r--   0        0        0     6400 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/SimulatedAnnealing.py
--rw-r--r--   0        0        0     2214 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/WorseAccept.py
--rw-r--r--   0        0        0      478 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/__init__.py
--rw-r--r--   0        0        0     4170 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_adaptive_threshold.py
--rw-r--r--   0        0        0     2311 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_great_deluge.py
--rw-r--r--   0        0        0      820 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_hill_climbing.py
--rw-r--r--   0        0        0     6012 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_late_acceptance_hill_climbing.py
--rw-r--r--   0        0        0     3452 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_non_linear_great_deluge.py
--rw-r--r--   0        0        0      790 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_random_walk.py
--rw-r--r--   0        0        0     5022 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_record_to_record_travel.py
--rw-r--r--   0        0        0     7119 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_simulated_annealing.py
--rw-r--r--   0        0        0     1947 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_threshold_accept.py
--rw-r--r--   0        0        0     1161 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_update.py
--rw-r--r--   0        0        0     4361 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/tests/test_worse_accept.py
--rw-r--r--   0        0        0      907 2023-06-23 14:18:28.746303 alns-5.3.0/alns/accept/update.py
--rw-r--r--   0        0        0     5247 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/AlphaUCB.py
--rw-r--r--   0        0        0     6509 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/MABSelector.py
--rw-r--r--   0        0        0     3516 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/OperatorSelectionScheme.py
--rw-r--r--   0        0        0      635 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/RandomSelect.py
--rw-r--r--   0        0        0     5090 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/RouletteWheel.py
--rw-r--r--   0        0        0     3598 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/SegmentedRouletteWheel.py
--rw-r--r--   0        0        0      268 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/tests/__init__.py
--rw-r--r--   0        0        0     2358 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/tests/test_alpha_ucb.py
--rw-r--r--   0        0        0     4379 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/tests/test_mab_selector.py
--rw-r--r--   0        0        0     2180 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/tests/test_random_select.py
--rw-r--r--   0        0        0     3871 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/tests/test_roulette_wheel.py
--rw-r--r--   0        0        0     2754 2023-06-23 14:18:28.746303 alns-5.3.0/alns/select/tests/test_segmented_roulette_wheel.py
--rw-r--r--   0        0        0      842 2023-06-23 14:18:28.746303 alns-5.3.0/alns/show_versions.py
--rw-r--r--   0        0        0      663 2023-06-23 14:18:28.746303 alns-5.3.0/alns/stop/MaxIterations.py
--rw-r--r--   0        0        0      769 2023-06-23 14:18:28.746303 alns-5.3.0/alns/stop/MaxRuntime.py
--rw-r--r--   0        0        0     1013 2023-06-23 14:18:28.746303 alns-5.3.0/alns/stop/NoImprovement.py
--rw-r--r--   0        0        0      669 2023-06-23 14:18:28.746303 alns-5.3.0/alns/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      166 2023-06-23 14:18:28.746303 alns-5.3.0/alns/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:18:28.750303 alns-5.3.0/alns/stop/tests/__init__.py
--rw-r--r--   0        0        0     1290 2023-06-23 14:18:28.750303 alns-5.3.0/alns/stop/tests/test_max_iterations.py
--rw-r--r--   0        0        0     1811 2023-06-23 14:18:28.750303 alns-5.3.0/alns/stop/tests/test_max_runtime.py
--rw-r--r--   0        0        0     2431 2023-06-23 14:18:28.750303 alns-5.3.0/alns/stop/tests/test_no_improvement.py
--rw-r--r--   0        0        0        0 2023-06-23 14:18:28.750303 alns-5.3.0/alns/tests/__init__.py
--rw-r--r--   0        0        0      385 2023-06-23 14:18:28.750303 alns-5.3.0/alns/tests/conftest.py
--rw-r--r--   0        0        0      834 2023-06-23 14:18:28.750303 alns-5.3.0/alns/tests/states.py
--rw-r--r--   0        0        0    10367 2023-06-23 14:18:28.750303 alns-5.3.0/alns/tests/test_alns.py
--rw-r--r--   0        0        0     6962 2023-06-23 14:18:28.750303 alns-5.3.0/alns/tests/test_result.py
--rw-r--r--   0        0        0     2796 2023-06-23 14:18:28.750303 alns-5.3.0/alns/tests/test_statistics.py
--rw-r--r--   0        0        0     2850 2023-06-23 14:18:28.766304 alns-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 alns-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-08-03 21:30:16.787223 alns-5.3.1/LICENSE.md
+-rw-r--r--   0        0        0     5673 2023-08-03 21:30:16.787223 alns-5.3.1/README.md
+-rw-r--r--   0        0        0    11416 2023-08-03 21:30:16.787223 alns-5.3.1/alns/ALNS.py
+-rw-r--r--   0        0        0      495 2023-08-03 21:30:16.787223 alns-5.3.1/alns/Outcome.py
+-rw-r--r--   0        0        0     5366 2023-08-03 21:30:16.787223 alns-5.3.1/alns/Result.py
+-rw-r--r--   0        0        0      637 2023-08-03 21:30:16.787223 alns-5.3.1/alns/State.py
+-rw-r--r--   0        0        0     3975 2023-08-03 21:30:16.787223 alns-5.3.1/alns/Statistics.py
+-rw-r--r--   0        0        0       89 2023-08-03 21:30:16.787223 alns-5.3.1/alns/__init__.py
+-rw-r--r--   0        0        0      885 2023-08-03 21:30:16.787223 alns-5.3.1/alns/accept/AcceptanceCriterion.py
+-rw-r--r--   0        0        0     2274 2023-08-03 21:30:16.787223 alns-5.3.1/alns/accept/AdaptiveThreshold.py
+-rw-r--r--   0        0        0     1855 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/GreatDeluge.py
+-rw-r--r--   0        0        0      276 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/HillClimbing.py
+-rw-r--r--   0        0        0     2481 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/LateAcceptanceHillClimbing.py
+-rw-r--r--   0        0        0     3543 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/NonLinearGreatDeluge.py
+-rw-r--r--   0        0        0      179 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/RandomWalk.py
+-rw-r--r--   0        0        0     6080 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/RecordToRecordTravel.py
+-rw-r--r--   0        0        0     6398 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/SimulatedAnnealing.py
+-rw-r--r--   0        0        0     2214 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/WorseAccept.py
+-rw-r--r--   0        0        0      478 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/__init__.py
+-rw-r--r--   0        0        0     4170 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_adaptive_threshold.py
+-rw-r--r--   0        0        0     2311 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_great_deluge.py
+-rw-r--r--   0        0        0      820 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_hill_climbing.py
+-rw-r--r--   0        0        0     6012 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_late_acceptance_hill_climbing.py
+-rw-r--r--   0        0        0     3452 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_non_linear_great_deluge.py
+-rw-r--r--   0        0        0      790 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_random_walk.py
+-rw-r--r--   0        0        0     5022 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_record_to_record_travel.py
+-rw-r--r--   0        0        0     7119 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_simulated_annealing.py
+-rw-r--r--   0        0        0     1947 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_threshold_accept.py
+-rw-r--r--   0        0        0     1161 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_update.py
+-rw-r--r--   0        0        0     4361 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_worse_accept.py
+-rw-r--r--   0        0        0      906 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/update.py
+-rw-r--r--   0        0        0     5247 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/AlphaUCB.py
+-rw-r--r--   0        0        0     6462 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/MABSelector.py
+-rw-r--r--   0        0        0     3516 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/OperatorSelectionScheme.py
+-rw-r--r--   0        0        0      635 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/RandomSelect.py
+-rw-r--r--   0        0        0     5090 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/RouletteWheel.py
+-rw-r--r--   0        0        0     3598 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/SegmentedRouletteWheel.py
+-rw-r--r--   0        0        0      268 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/__init__.py
+-rw-r--r--   0        0        0     2358 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_alpha_ucb.py
+-rw-r--r--   0        0        0     4379 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_mab_selector.py
+-rw-r--r--   0        0        0     2180 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_random_select.py
+-rw-r--r--   0        0        0     3871 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_roulette_wheel.py
+-rw-r--r--   0        0        0     2754 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_segmented_roulette_wheel.py
+-rw-r--r--   0        0        0      842 2023-08-03 21:30:16.791223 alns-5.3.1/alns/show_versions.py
+-rw-r--r--   0        0        0      663 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/MaxIterations.py
+-rw-r--r--   0        0        0      769 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/MaxRuntime.py
+-rw-r--r--   0        0        0     1013 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/NoImprovement.py
+-rw-r--r--   0        0        0      669 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      166 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/__init__.py
+-rw-r--r--   0        0        0     1290 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/test_max_iterations.py
+-rw-r--r--   0        0        0     1811 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/test_max_runtime.py
+-rw-r--r--   0        0        0     2431 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/test_no_improvement.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/conftest.py
+-rw-r--r--   0        0        0      834 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/states.py
+-rw-r--r--   0        0        0    10367 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/test_alns.py
+-rw-r--r--   0        0        0     6962 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/test_result.py
+-rw-r--r--   0        0        0     2796 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/test_statistics.py
+-rw-r--r--   0        0        0     3032 2023-08-03 21:30:16.815223 alns-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 alns-5.3.1/PKG-INFO
```

### Comparing `alns-5.3.0/LICENSE.md` & `alns-5.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/README.md` & `alns-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/ALNS.py` & `alns-5.3.1/alns/ALNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         ----------
         .. [1] Pisinger, D., & Røpke, S. (2010). Large Neighborhood Search. In
                M. Gendreau (Ed.), *Handbook of Metaheuristics* (2 ed., pp. 399
                - 420). Springer.
 
         .. [2] S. Røpke and D. Pisinger (2006). A unified heuristic for a large
                class of vehicle routing problems with backhauls. *European
-               Journal of Operational Research*, 171: 750–775.
+               Journal of Operational Research*, 171: 750-775.
         """
         if len(self.destroy_operators) == 0 or len(self.repair_operators) == 0:
             raise ValueError("Missing destroy or repair operators.")
 
         curr = best = initial_solution
         init_obj = initial_solution.objective()
```

### Comparing `alns-5.3.0/alns/Result.py` & `alns-5.3.1/alns/Result.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/State.py` & `alns-5.3.1/alns/State.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/Statistics.py` & `alns-5.3.1/alns/Statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/AcceptanceCriterion.py` & `alns-5.3.1/alns/accept/AcceptanceCriterion.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/AdaptiveThreshold.py` & `alns-5.3.1/alns/accept/AdaptiveThreshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
        \\right)
 
     where :math:`s^*` is the best solution observed in the last :math:`\\gamma`
     iterations, :math:`f(\\cdot)` indicates the objective function,
     :math:`\\eta \\in [0, 1]` and :math:`\\gamma \\in \\mathbb{N}` are
     parameters, and each :math:`s^i` is a recently observed solution. The
     recently observed solutions are stored in a ``history`` attributed of size
-    :math:`\\gamma`.
+    at most :math:`\\gamma`.
 
     Parameters
     ----------
     eta: float
         Used to determine the threshold value. Larger values of :math:`\\eta`
         result in more accepted candidate solutions. Must be in [0, 1].
     gamma: int
```

### Comparing `alns-5.3.0/alns/accept/GreatDeluge.py` & `alns-5.3.1/alns/accept/GreatDeluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/LateAcceptanceHillClimbing.py` & `alns-5.3.1/alns/accept/LateAcceptanceHillClimbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/NonLinearGreatDeluge.py` & `alns-5.3.1/alns/accept/NonLinearGreatDeluge.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
            and the record-to-record travel. *Journal of Computational Physics*
            (1993) 104 (1): 86-92.
     .. [2] Landa-Silva, D., & Obit, J. H. Great deluge with non-linear decay
            rate for solving course timetabling problems. *4th international
            IEEE conference intelligent systems* (2008) Vol. 1: 8-11.
     .. [3] Santini, A., Ropke, S. & Hvattum, L.M. A comparison of acceptance
            criteria for the adaptive large neighbourhood search metaheuristic.
-           *Journal of Heuristics* (2018) 24 (5): 783–815.
+           *Journal of Heuristics* (2018) 24 (5): 783-815.
     """
 
     def __init__(self, alpha: float, beta: float, gamma: float, delta: float):
         super().__init__(alpha, beta)
 
         if gamma <= 0 or delta <= 0:
             raise ValueError("Gamma and delta must be non-negative.")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alns-5.3.0/alns/accept/RecordToRecordTravel.py` & `alns-5.3.1/alns/accept/RecordToRecordTravel.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         the difference between the candidate and current solution instead. This
         yields the behaviour of threshold accepting (TA), see [3] for details.
 
     References
     ----------
     .. [1] Santini, A., Ropke, S. & Hvattum, L.M. A comparison of acceptance
            criteria for the adaptive large neighbourhood search metaheuristic.
-           *Journal of Heuristics* (2018) 24 (5): 783–815.
+           *Journal of Heuristics* (2018) 24 (5): 783-815.
     .. [2] Dueck, G. New optimization heuristics: The great deluge algorithm
            and the record-to-record travel. *Journal of Computational Physics*
            (1993) 104 (1): 86-92.
     .. [3] Dueck, G., Scheuer, T. Threshold accepting: A general purpose
          optimization algorithm appearing superior to simulated annealing.
          *Journal of Computational Physics* (1990) 90 (1): 161-175.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alns-5.3.0/alns/accept/SimulatedAnnealing.py` & `alns-5.3.1/alns/accept/SimulatedAnnealing.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         The updating method, one of {'linear', 'exponential'}. Default
         'exponential'.
 
     References
     ----------
     .. [1] Santini, A., Ropke, S. & Hvattum, L.M. A comparison of acceptance
            criteria for the adaptive large neighbourhood search metaheuristic.
-           *Journal of Heuristics* (2018) 24 (5): 783–815.
+           *Journal of Heuristics* (2018) 24 (5): 783-815.
     .. [2] Kirkpatrick, S., Gerlatt, C. D. Jr., and Vecchi, M. P. Optimization
            by Simulated Annealing. *IBM Research Report* RC 9355, 1982.
     """
 
     def __init__(
         self,
         start_temperature: float,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alns-5.3.0/alns/accept/WorseAccept.py` & `alns-5.3.1/alns/accept/WorseAccept.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_adaptive_threshold.py` & `alns-5.3.1/alns/accept/tests/test_adaptive_threshold.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_great_deluge.py` & `alns-5.3.1/alns/accept/tests/test_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_hill_climbing.py` & `alns-5.3.1/alns/accept/tests/test_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_late_acceptance_hill_climbing.py` & `alns-5.3.1/alns/accept/tests/test_late_acceptance_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_non_linear_great_deluge.py` & `alns-5.3.1/alns/accept/tests/test_non_linear_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_random_walk.py` & `alns-5.3.1/alns/accept/tests/test_random_walk.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_record_to_record_travel.py` & `alns-5.3.1/alns/accept/tests/test_record_to_record_travel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_simulated_annealing.py` & `alns-5.3.1/alns/accept/tests/test_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_threshold_accept.py` & `alns-5.3.1/alns/accept/tests/test_threshold_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_update.py` & `alns-5.3.1/alns/accept/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/tests/test_worse_accept.py` & `alns-5.3.1/alns/accept/tests/test_worse_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/accept/update.py` & `alns-5.3.1/alns/accept/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,12 @@
     -------
     The new criterion threshold.
     """
     method = method.lower()
 
     if method == "linear":
         return current - step
-    elif method == "exponential":
+
+    if method == "exponential":
         return current * step
 
     raise ValueError("Method `{0}' not understood.".format(method))
```

### Comparing `alns-5.3.0/alns/select/AlphaUCB.py` & `alns-5.3.1/alns/select/AlphaUCB.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/MABSelector.py` & `alns-5.3.1/alns/select/MABSelector.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from numpy.random import RandomState
 
 from alns.Outcome import Outcome
 from alns.State import ContextualState
 from alns.select.OperatorSelectionScheme import OperatorSelectionScheme
 
 try:
-    from mabwiser.mab import MAB, LearningPolicy, NeighborhoodPolicy
+    from mabwiser.mab import MAB, LearningPolicyType, NeighborhoodPolicyType
 
     MABWISER_AVAILABLE = True
 except ModuleNotFoundError:
     MABWISER_AVAILABLE = False
 
 
 class MABSelector(OperatorSelectionScheme):
@@ -75,16 +75,16 @@
     """
 
     def __init__(
         self,
         scores: List[float],
         num_destroy: int,
         num_repair: int,
-        learning_policy: "LearningPolicy",
-        neighborhood_policy: Optional["NeighborhoodPolicy"] = None,
+        learning_policy: "LearningPolicyType",
+        neighborhood_policy: Optional["NeighborhoodPolicyType"] = None,
         seed: Optional[int] = None,
         op_coupling: Optional[np.ndarray] = None,
         **kwargs,
     ):
         if not MABWISER_AVAILABLE:
             msg = """
             The MABSelector requires the MABWiser dependency to be installed.
@@ -127,29 +127,28 @@
         self,
         rnd_state: RandomState,
         best: ContextualState,
         curr: ContextualState,
     ) -> Tuple[int, int]:
         """
         Returns the (destroy, repair) operator pair from the underlying MAB
-        strategy
+        strategy.
         """
-        if self._mab._is_initial_fit:
-            has_ctx = self._mab.is_contextual
-            ctx = np.atleast_2d(curr.get_context()) if has_ctx else None
-            prediction = self._mab.predict(contexts=ctx)
-            return arm2ops(prediction)
-        else:
-            # This can happen when the MAB object has not yet been fit on any
-            # observations. In that case we return any feasible operator index
-            # pair as a first observation.
+        if not self._mab._is_initial_fit:  # noqa: SLF001
+            # The MAB object has not yet been fit. In that case we return any
+            # feasible operator index pair as a first observation.
             allowed = np.argwhere(self._op_coupling)
             idx = rnd_state.randint(len(allowed))
             return allowed[idx][0], allowed[idx][1]
 
+        has_ctx = self._mab.is_contextual
+        ctx = np.atleast_2d(curr.get_context()) if has_ctx else None
+        prediction = self._mab.predict(contexts=ctx)
+        return arm2ops(prediction)
+
     def update(  # type: ignore[override]
         self,
         cand: ContextualState,
         d_idx: int,
         r_idx: int,
         outcome: Outcome,
     ):
```

### Comparing `alns-5.3.0/alns/select/OperatorSelectionScheme.py` & `alns-5.3.1/alns/select/OperatorSelectionScheme.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/RandomSelect.py` & `alns-5.3.1/alns/select/RandomSelect.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/RouletteWheel.py` & `alns-5.3.1/alns/select/RouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/SegmentedRouletteWheel.py` & `alns-5.3.1/alns/select/SegmentedRouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/tests/test_alpha_ucb.py` & `alns-5.3.1/alns/select/tests/test_alpha_ucb.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/tests/test_mab_selector.py` & `alns-5.3.1/alns/select/tests/test_mab_selector.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/tests/test_random_select.py` & `alns-5.3.1/alns/select/tests/test_random_select.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/tests/test_roulette_wheel.py` & `alns-5.3.1/alns/select/tests/test_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/select/tests/test_segmented_roulette_wheel.py` & `alns-5.3.1/alns/select/tests/test_segmented_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/show_versions.py` & `alns-5.3.1/alns/show_versions.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/MaxIterations.py` & `alns-5.3.1/alns/stop/MaxIterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/MaxRuntime.py` & `alns-5.3.1/alns/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/NoImprovement.py` & `alns-5.3.1/alns/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/StoppingCriterion.py` & `alns-5.3.1/alns/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/tests/test_max_iterations.py` & `alns-5.3.1/alns/stop/tests/test_max_iterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/tests/test_max_runtime.py` & `alns-5.3.1/alns/stop/tests/test_max_runtime.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/stop/tests/test_no_improvement.py` & `alns-5.3.1/alns/stop/tests/test_no_improvement.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/tests/states.py` & `alns-5.3.1/alns/tests/states.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/tests/test_alns.py` & `alns-5.3.1/alns/tests/test_alns.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/tests/test_result.py` & `alns-5.3.1/alns/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/alns/tests/test_statistics.py` & `alns-5.3.1/alns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.0/pyproject.toml` & `alns-5.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alns"
-version = "5.3.0"
+version = "5.3.1"
 description = "A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/ALNS"
 include = [
     "LICENSE.md",
@@ -29,61 +29,67 @@
 [tool.poetry.urls]
 "Tracker" = "https://github.com/N-Wouda/ALNS/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8, <4.0"
 numpy = ">=1.18.0"
 matplotlib = ">=3.5.0"
-mabwiser = { version = ">=2.7.0", optional = true }
+mabwiser = { version = ">=2.7.1", optional = true }
 
 [tool.poetry.extras]
 mabwiser = ["mabwiser"]  # optional integration with MABWiser
 
 # This group is needed to develop the package itself.
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.6.1"
 codecov = "*"
-mabwiser = ">=2.7.0"
+mabwiser = ">=2.7.1"
 
 # This optional docs group is needed to build the documentation. It is not 
 # required by the package itself.
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 tomli = ">=2.0.1"
 nbsphinx = ">=0.8.9"
 ipython = ">=8.6.0"
 numpydoc = ">=1.5.0"
 sphinx_rtd_theme = ">=0.5.1"
 sphinx-autoapi = ">=2.0.1"
 docutils = "==0.16"
-mabwiser = ">=2.7.0"
+mabwiser = ">=2.7.1"
 
 # This optional examples group is needed to run the example notebooks, but not
 # required for the package itself.
 [tool.poetry.group.examples]
 optional = true
 
 [tool.poetry.group.examples.dependencies]
 vrplib = "^1.0.1"
 networkx = ">=2.4.0"
 tsplib95 = ">=0.7.0"
 jupyter = "^1.0.0"
-mabwiser = ">=2.7.0"
+mabwiser = ">=2.7.1"
 
 [tool.black]
 line-length = 79
 
-[tool.isort]
-case_sensitive = true
-line_length = 79
-profile = "black"
+[tool.ruff]
+line-length = 79
+select = ["E", "F", "I", "NPY", "RET", "RSE", "RUF", "SLF", "SIM", "TCH"]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]  # unused imports
+
+[tool.ruff.isort]
+case-sensitive = true
+known-first-party = ["alns"]
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 markers = [
     "matplotlib: test related to matplotlib functionality.",
```

### Comparing `alns-5.3.0/PKG-INFO` & `alns-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alns
-Version: 5.3.0
+Version: 5.3.1
 Summary: A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm.
 Home-page: https://github.com/N-Wouda/ALNS
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: mabwiser
-Requires-Dist: mabwiser (>=2.7.0) ; extra == "mabwiser"
+Requires-Dist: mabwiser (>=2.7.1) ; extra == "mabwiser"
 Requires-Dist: matplotlib (>=3.5.0)
 Requires-Dist: numpy (>=1.18.0)
 Project-URL: Repository, https://github.com/N-Wouda/ALNS
 Project-URL: Tracker, https://github.com/N-Wouda/ALNS/issues
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/alns.svg)](https://badge.fury.io/py/alns)
```

