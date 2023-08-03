# Comparing `tmp/spectrum_fundamentals-0.4.1.tar.gz` & `tmp/spectrum_fundamentals-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.4.1.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.4.2.tar", max compression
```

## Comparing `spectrum_fundamentals-0.4.1.tar` & `spectrum_fundamentals-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/LICENSE
--rw-r--r--   0        0        0     2611 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/README.rst
--rw-r--r--   0        0        0     2367 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      940 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    11160 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1372 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0     7807 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    12267 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    14554 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1435 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    22868 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    22390 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0     9443 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-03 14:26:08.045496 spectrum_fundamentals-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2611 2023-08-03 14:26:08.045496 spectrum_fundamentals-0.4.2/README.rst
+-rw-r--r--   0        0        0     2367 2023-08-03 14:26:08.045496 spectrum_fundamentals-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      940 2023-08-03 14:26:08.045496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2023-08-03 14:26:08.045496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2023-08-03 14:26:08.045496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    11729 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1372 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0     7807 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    13757 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    14554 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1435 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    22868 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    22262 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0     9443 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:26:08.049496 spectrum_fundamentals-0.4.2/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.4.2/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.4.1/LICENSE` & `spectrum_fundamentals-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/README.rst` & `spectrum_fundamentals-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/pyproject.toml` & `spectrum_fundamentals-0.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.4.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.4.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamentals public repo"
 authors = ["WassimG <wassim.gabriel@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Initialize fundamentals."""
 __author__ = "Victor Giurcoiu"
 __email__ = "victor.giurcoiu@tum.de"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/annotation/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,17 @@
     original_length = len(matched_peaks_df.index)
     matched_peaks_df = matched_peaks_df.drop_duplicates(subset=["ion_type", "no", "charge"], keep="first")
     # matched_peaks_df = matched_peaks_df[matched_peaks_df['intensity']>0.01]
     length_after_matches = len(matched_peaks_df.index)
     return matched_peaks_df, (original_length - length_after_matches)
 
 
-def annotate_spectra(un_annot_spectra: pd.DataFrame) -> pd.DataFrame:
+def annotate_spectra(
+    un_annot_spectra: pd.DataFrame, mass_tolerance: Optional[float] = None, unit_mass_tolerance: Optional[str] = None
+) -> pd.DataFrame:
     """
     Annotate a set of spectra.
 
     This function takes a DataFrame of raw peaks and metadata, and for each spectrum, it calls the `parallel_annotate` function
     to annotate the spectrum and extract the necessary information. If there are any redundant peaks found in the annotation
     process, the function removes them and logs the information. Finally, it returns a Pandas DataFrame containing the annotated
     spectra with meta data.
@@ -130,20 +132,22 @@
     The returned DataFrame has the following columns:
     - INTENSITIES: a NumPy array containing the intensity values of each peak in the annotated spectrum
     - MZ: a NumPy array containing the m/z values of each peak in the annotated spectrum
     - CALCULATED_MASS: a float representing the calculated mass of the spectrum
     - removed_peaks: a NumPy array containing the indices of any peaks that were removed during the annotation process
 
     :param un_annot_spectra: a Pandas DataFrame containing the raw peaks and metadata to be annotated
+    :param mass_tolerance: mass tolerance to calculate min and max mass
+    :param unit_mass_tolerance: unit for the mass tolerance (da or ppm)
     :return: a Pandas DataFrame containing the annotated spectra with meta data
     """
     raw_file_annotations = []
     index_columns = {col: un_annot_spectra.columns.get_loc(col) for col in un_annot_spectra.columns}
     for row in un_annot_spectra.values:
-        results = parallel_annotate(row, index_columns)
+        results = parallel_annotate(row, index_columns, mass_tolerance, unit_mass_tolerance)
         if not results:
             continue
         raw_file_annotations.append(results)
     results_df = pd.DataFrame(raw_file_annotations)
     results_df.columns = ["INTENSITIES", "MZ", "CALCULATED_MASS", "removed_peaks"]
     logger.info(f"Removed {results_df['removed_peaks'].describe()} redundant peaks")
 
@@ -201,37 +205,46 @@
         mask_peaks = range((len(unmod_seq) - 1) * 6, ((len(unmod_seq) - 1) * 6) + 6)
         intensity[mask_peaks] = -1.0
         mass[mask_peaks] = -1.0
 
     return intensity, mass
 
 
-def parallel_annotate(spectrum: np.ndarray, index_columns: dict) -> Optional[Tuple[np.ndarray, np.ndarray, float, int]]:
+def parallel_annotate(
+    spectrum: np.ndarray,
+    index_columns: dict,
+    mass_tolerance: Optional[float] = None,
+    unit_mass_tolerance: Optional[str] = None,
+) -> Optional[Tuple[np.ndarray, np.ndarray, float, int]]:
     """
     Perform parallel annotation of a spectrum.
 
     This function takes a spectrum and its index columns and performs parallel annotation of the spectrum. It starts by
     initializing the peaks and extracting necessary data from the spectrum. It then matches the peaks to the spectrum and
     generates an annotation matrix based on the matched peaks. If there are multiple matches found, it removes the redundant
     matches. Finally, it returns annotated spectrum with meta data including intensity values, masses, calculated masses,
     and any peaks that were removed. The function is designed to run in different threads to speed up the annotation pipeline.
 
     :param spectrum: a np.ndarray that contains the spectrum to be annotated
     :param index_columns: a dictionary that contains the index columns of the spectrum
+    :param mass_tolerance: mass tolerance to calculate min and max mass
+    :param unit_mass_tolerance: unit for the mass tolerance (da or ppm)
     :return: a tuple containing intensity values (np.ndarray), masses (np.ndarray), calculated mass (float),
              and any removed peaks (List[str])
     """
     mod_seq_column = "MODIFIED_SEQUENCE"
     if "MODIFIED_SEQUENCE_MSA" in index_columns:
         mod_seq_column = "MODIFIED_SEQUENCE_MSA"
 
     fragments_meta_data, tmt_n_term, unmod_sequence, calc_mass = initialize_peaks(
         spectrum[index_columns[mod_seq_column]],
         spectrum[index_columns["MASS_ANALYZER"]],
         spectrum[index_columns["PRECURSOR_CHARGE"]],
+        mass_tolerance,
+        unit_mass_tolerance,
     )
     if not unmod_sequence:
         return None
     matched_peaks = match_peaks(
         fragments_meta_data,
         spectrum[index_columns["INTENSITIES"]],
         spectrum[index_columns["MZ"]],
```

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/constants.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/fragments.py`

 * *Files 16% similar despite different names*

```diff
@@ -102,21 +102,29 @@
     for i in range(0, peptide_length):  # generate substrings
         forward_sum += constants.AA_MASSES[peptide_sequence[i]]  # sum left to right
         if i in modification_deltas:  # add mass of modification if present
             forward_sum += modification_deltas[i]
     return forward_sum + ion_type_offsets[0] + ion_type_offsets[1]
 
 
-def initialize_peaks(sequence: str, mass_analyzer: str, charge: int) -> Tuple[List[dict], int, str, float]:
+def initialize_peaks(
+    sequence: str,
+    mass_analyzer: str,
+    charge: int,
+    mass_tolerance: Optional[float] = None,
+    unit_mass_tolerance: Optional[str] = None,
+) -> Tuple[List[dict], int, str, float]:
     """
     Generate theoretical peaks for a modified peptide sequence.
 
     :param sequence: Modified peptide sequence
     :param mass_analyzer: Type of mass analyzer used eg. FTMS, ITMS
     :param charge: Precursor charge
+    :param mass_tolerance: mass tolerance to calculate min and max mass
+    :param unit_mass_tolerance: unit for the mass tolerance (da or ppm)
     :raises AssertionError:  if peptide sequence contained an unknown modification. TODO do this within the get_mod func.
     :return: List of theoretical peaks, Flag to indicate if there is a tmt on n-terminus, Un modified peptide sequence
     """
     peptide_sequence = sequence
     modifications = _get_modifications(peptide_sequence)
     if modifications is None:
         raise AssertionError("Modification not found.")
@@ -186,24 +194,47 @@
                         "max_mass": max_mass,  # max mass
                     }
                 )
     fragments_meta_data = sorted(fragments_meta_data, key=itemgetter("mass"))
     return fragments_meta_data, tmt_n_term, peptide_sequence, (forward_sum + ion_type_offsets[0] + ion_type_offsets[1])
 
 
-def get_min_max_mass(mass_analyzer: str, mass: float) -> Tuple[float, float]:
+def get_min_max_mass(
+    mass_analyzer: str, mass: float, mass_tolerance: Optional[float] = None, unit_mass_tolerance: Optional[str] = None
+) -> Tuple[float, float]:
     """Helper function to get min and max mass based on mass analyzer.
 
+    If both mass_tolerance and unit_mass_tolerance are provided, the function uses the provided tolerance
+    to calculate the min and max mass. If either `mass_tolerance` or `unit_mass_tolerance` is missing
+    (or both are None), the function falls back to the default tolerances based on the `mass_analyzer`.
+
+    Default mass tolerances for different mass analyzers:
+    - FTMS: +/- 20 ppm
+    - TOF: +/- 40 ppm
+    - ITMS: +/- 0.35 daltons
+
+    :param mass_tolerance: mass tolerance to calculate min and max mass
+    :param unit_mass_tolerance: unit for the mass tolerance (da or ppm)
     :param mass_analyzer: the type of mass analyzer used to determine the tolerance.
     :param mass: the theoretical fragment mass
     :raises ValueError: if mass_analyzer is other than one of FTMS, TOF, ITMS
+    :raises ValueError: if unit_mass_tolerance is other than one of ppm, da
 
     :return: a tuple (min, max) denoting the mass tolerance range.
     """
-    if mass_analyzer == "FTMS":
+    if mass_tolerance is not None and unit_mass_tolerance is not None:
+        if unit_mass_tolerance == "ppm":
+            min_mass = (mass * -mass_tolerance / 1000000) + mass
+            max_mass = (mass * mass_tolerance / 1000000) + mass
+        elif unit_mass_tolerance == "da":
+            min_mass = mass - mass_tolerance
+            max_mass = mass + mass_tolerance
+        else:
+            raise ValueError(f"Unsupported unit for the mass tolerance: {unit_mass_tolerance}")
+    elif mass_analyzer == "FTMS":
         min_mass = (mass * -20 / 1000000) + mass
         max_mass = (mass * 20 / 1000000) + mass
     elif mass_analyzer == "TOF":
         min_mass = (mass * -40 / 1000000) + mass
         max_mass = (mass * 40 / 1000000) + mass
     elif mass_analyzer == "ITMS":
         min_mass = mass - 0.35
```

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/percolator.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/metrics/similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,37 +212,35 @@
                                      0 intensity indicates invalid peaks (charge state > peptide charge state or \
                                      position >= peptide length), array of length 174
         :param predicted_intensities: predicted intensities, see observed_intensities for details, array of length 174
         :param charge: to filter by the peak charges, 0 means everything
         :param method: either pearson or spearman
         :return: calculated correlations
         """
-        observed_intensities = observed_intensities.toarray()
-        predicted_intensities = predicted_intensities.toarray()
+        observed_intensities_array = observed_intensities.toarray()
+        predicted_intensities_array = predicted_intensities.toarray()
 
         if charge != 0:
             if charge == 1:
                 boolean_array = constants.SINGLE_CHARGED_MASK
             elif charge == 2:
                 boolean_array = constants.DOUBLE_CHARGED_MASK
             elif charge == 3:
                 boolean_array = constants.TRIPLE_CHARGED_MASK
             elif charge == 4:
                 boolean_array = constants.B_ION_MASK
             else:
                 boolean_array = constants.Y_ION_MASK
 
             boolean_array = scipy.sparse.csr_matrix(boolean_array)
-            observed_intensities = scipy.sparse.csr_matrix(observed_intensities)
-            predicted_intensities = scipy.sparse.csr_matrix(predicted_intensities)
-            observed_intensities = observed_intensities.multiply(boolean_array).toarray()
-            predicted_intensities = predicted_intensities.multiply(boolean_array).toarray()
+            observed_intensities_array = observed_intensities.multiply(boolean_array).toarray()
+            predicted_intensities_array = predicted_intensities.multiply(boolean_array).toarray()
 
         pear_corr = []
-        for obs, pred in zip(observed_intensities, predicted_intensities):
+        for obs, pred in zip(observed_intensities_array, predicted_intensities_array):
             valid_ion_mask = pred > constants.EPSILON
             obs = obs[valid_ion_mask]
             pred = pred[valid_ion_mask]
             obs = obs[~np.isnan(obs)]
             pred = pred[~np.isnan(pred)]
             if len(obs) > 2 and len(pred) > 2:
                 corr = (
```

### Comparing `spectrum_fundamentals-0.4.1/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.4.2/spectrum_fundamentals/mod_string.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.1/PKG-INFO` & `spectrum_fundamentals-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-fundamentals
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fundamentals public repo
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: WassimG
 Author-email: wassim.gabriel@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

