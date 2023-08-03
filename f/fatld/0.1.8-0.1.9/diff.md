# Comparing `tmp/fatld-0.1.8.tar.gz` & `tmp/fatld-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fatld-0.1.8.tar", max compression
+gzip compressed data, was "fatld-0.1.9.tar", max compression
```

## Comparing `fatld-0.1.8.tar` & `fatld-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     3238 2023-07-03 09:25:25.776302 fatld-0.1.8/README.md
--rwxr-xr-x   0        0        0      147 2023-04-18 13:22:51.567061 fatld-0.1.8/fatld/__init__.py
--rwxr-xr-x   0        0        0    42796 2023-07-31 19:57:57.077647 fatld-0.1.8/fatld/design.py
--rwxr-xr-x   0        0        0     6967 2023-07-31 19:57:57.091646 fatld-0.1.8/fatld/main.py
--rwxr-xr-x   0        0        0     8611 2023-07-31 19:57:57.093684 fatld-0.1.8/fatld/relation.py
--rwxr-xr-x   0        0        0     1040 2023-07-31 19:57:57.105173 fatld-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 fatld-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     3238 2023-07-03 09:25:25.776302 fatld-0.1.9/README.md
+-rwxr-xr-x   0        0        0      147 2023-08-01 15:54:51.796574 fatld-0.1.9/fatld/__init__.py
+-rwxr-xr-x   0        0        0    43642 2023-08-01 15:54:51.815574 fatld-0.1.9/fatld/design.py
+-rwxr-xr-x   0        0        0     6967 2023-07-31 19:57:57.091646 fatld-0.1.9/fatld/main.py
+-rwxr-xr-x   0        0        0     8611 2023-07-31 19:57:57.093684 fatld-0.1.9/fatld/relation.py
+-rwxr-xr-x   0        0        0     1040 2023-08-01 15:54:51.833574 fatld-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 fatld-0.1.9/PKG-INFO
```

### Comparing `fatld-0.1.8/README.md` & `fatld-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fatld-0.1.8/fatld/design.py` & `fatld-0.1.9/fatld/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,16 +350,19 @@
         for factor_index in range(self.m):
             # Remove the blocking factor and evaluate the WLP of the design
             trmt_wlp = list(
                 map(int, design_oa.deleteColumn(factor_index).GWLP())
             )
             block_wlp = [design_wlp[i] - x for i, x in enumerate(trmt_wlp)]
             w2_vector = build_w2_vector(block_wlp, trmt_wlp)
+            # Nothing is returned if the vectors cannot be combined
+            if w2_vector is None:
+                continue
             # Set as default if it is the first factor we evaluate
-            if factor_index == 0:
+            if factor_index == 0 or best_w2_vector == []:
                 best_w2_vector = w2_vector
             else:
                 if w2_vector < best_w2_vector:
                     best_w2_vector = w2_vector
                     best_factor = chr(65 + factor_index)
         return best_w2_vector, best_factor
 
@@ -376,14 +379,19 @@
 
         Returns
         -------
         list[float]
             The alpha word length pattern
         """
         twlp = self.twlp(max_length=4)
+        # For cases with designs with not enough words
+        if len(twlp) == 0:
+            twlp = [[0, 0, 0], [0, 0, 0, 0]]
+        elif len(twlp) == 1:
+            twlp.append([0, 0, 0, 0])
         a3_vector = twlp[0] + [0] * (3 - len(twlp[0]))  # Right pad with 0
         a4_vector = twlp[1] + [0] * (4 - len(twlp[1]))
         omega_weights = {
             "w2": [3 / 3, 2 / 3, 1 / 3],
             "w4": [0 / 3, 1 / 3, 2 / 3],
             "w22": [6 / 6, 3 / 6, 1 / 6, 0 / 6],
             "w42": [0 / 6, 3 / 6, 4 / 6, 3 / 6],
@@ -958,31 +966,31 @@
     # creating 9)
     # - Interactions between the 3 four-level factors (27 terms)
     elif m == 3:
         # Interactions between 2 of the 3 four-level factors
         fl_contrast_2f_interaction_matrix = np.zeros((N, 27), dtype=float)
         for comb_idx, combi in enumerate([(0, 1), (0, 2), (1, 2)]):
             range1 = [3 * combi[0], 3 * combi[0] + 1, 3 * combi[0] + 2]
-            range2 = [3 * comb[1], 3 * comb[1] + 1, 3 * comb[1] + 2]
+            range2 = [3 * combi[1], 3 * combi[1] + 1, 3 * combi[1] + 2]
             for pair_idx, pair in enumerate(product(range1, range2)):
                 index = 9 * comb_idx + pair_idx
                 fl_contrast_2f_interaction_matrix[:, index] = np.prod(
                     fl_contrast_matrix[:, pair], axis=1
-                )[:, None]
+                )
                 normalized_indices = [i % 3 for i in pair]
                 fl_contrast_length.append(sum(normalized_indices) + 2)
 
         # Interactions between 3 four-level factors
         fl_contrast_3f_interaction_matrix = np.zeros((N, 27), dtype=float)
         for triplet_idx, triplet in enumerate(
             product([0, 1, 2], [3, 4, 5], [6, 7, 8])
         ):
             fl_contrast_3f_interaction_matrix[:, triplet_idx] = np.prod(
                 fl_contrast_matrix[:, triplet], axis=1
-            )[:, None]
+            )
             normalized_indices = [i % 3 for i in triplet]
             fl_contrast_length.append(sum(normalized_indices) + 3)
 
         # Join ME, 2FI, and 3FI into a single matrix
         fl_full_contrast_matrix: np.ndarray = np.hstack(
             (
                 fl_contrast_matrix,
@@ -1118,23 +1126,38 @@
             tfi_model_matrix[c, index] = 1
             index += 1
     return tfi_model_matrix
 
 
 def build_w2_vector(
     blocking_wlp: list[int], treatment_wlp: list[int]
-) -> list[int]:
+) -> list[int] | None:
     """
     Compute the W_2 word length pattern (WLP) of a design, given its treatment
     WLP and blocking WLP.
     Both WLP must start with words of length 0 (so that list indices matches
     word lengths).
     """
     if len(blocking_wlp) != len(treatment_wlp):
         raise ValueError("Both WLP must have the same length")
+    if len(blocking_wlp) <= 3:
+        if any([i != 0 for i in blocking_wlp]) or any(
+            [i != 0 for i in treatment_wlp]
+        ):
+            warnings.warn(
+                "A vector contains a non-zero A_i value for i < 3",
+                UserWarning,
+            )
+            return None
+        else:
+            warnings.warn(
+                "WLPs too short to combine. Returning a zero vector",
+                UserWarning,
+            )
+            return [0, 0, 0]
     w2_vector = [treatment_wlp[3], blocking_wlp[3]]
     n_words = len(blocking_wlp) - 1
     max_i = 1 + (n_words - 1) // 2
     for i in range(2, max_i):
         w2_vector.append(treatment_wlp[2 * i])
         w2_vector.append(treatment_wlp[2 * i + 1])
         w2_vector.append(blocking_wlp[i + 2])
```

### Comparing `fatld-0.1.8/fatld/main.py` & `fatld-0.1.9/fatld/main.py`

 * *Files identical despite different names*

### Comparing `fatld-0.1.8/fatld/relation.py` & `fatld-0.1.9/fatld/relation.py`

 * *Files identical despite different names*

### Comparing `fatld-0.1.8/pyproject.toml` & `fatld-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fatld"
-version = "0.1.8"
+version = "0.1.9"
 description = "Generate and characterize designs with four-and-two-level (FATL) factors"
 authors = ["Alexandre Bohyn <alexandre.bohyn@kuleuven.be>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://abohyndoe.github.io/fatld/"
 repository = "https://github.com/ABohynDOE/fatld"
 keywords = ["design", "doe"]
```

### Comparing `fatld-0.1.8/PKG-INFO` & `fatld-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fatld
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate and characterize designs with four-and-two-level (FATL) factors
 Home-page: https://abohyndoe.github.io/fatld/
 License: MIT
 Keywords: design,doe
 Author: Alexandre Bohyn
 Author-email: alexandre.bohyn@kuleuven.be
 Requires-Python: >=3.8,<4.0
```

