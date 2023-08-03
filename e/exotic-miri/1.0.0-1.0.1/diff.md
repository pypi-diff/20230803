# Comparing `tmp/exotic-miri-1.0.0.tar.gz` & `tmp/exotic-miri-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exotic-miri-1.0.0.tar", last modified: Mon Jul 31 09:41:56 2023, max compression
+gzip compressed data, was "exotic-miri-1.0.1.tar", last modified: Thu Aug  3 13:02:09 2023, max compression
```

## Comparing `exotic-miri-1.0.0.tar` & `exotic-miri-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.946228 exotic-miri-1.0.0/exotic_miri/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.946228 exotic-miri-1.0.0/exotic_miri/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_default_gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_default_readnoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_integration_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_wavelength_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/set_custom_gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/set_custom_linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/exotic_miri/stage_1/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/drop_groups_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/drop_integrations_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/group_level_background_subtract_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/reference_pixel_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/regroup_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/exotic_miri/stage_2/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/align_spectra_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/background_subtract_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/clean_outliers_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/extract_1d_box_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/extract_1d_optimal_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/inspect_dq_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.946228 exotic-miri-1.0.0/exotic_miri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/tests/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/tests/test_stage_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/tests/test_stage_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.259609 exotic-miri-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-03 13:02:09.259609 exotic-miri-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.247609 exotic-miri-1.0.1/exotic_miri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.251609 exotic-miri-1.0.1/exotic_miri/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/get_default_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/get_default_readnoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/get_integration_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/get_wavelength_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/set_custom_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/reference/set_custom_linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.255609 exotic-miri-1.0.1/exotic_miri/stage_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_1/drop_groups_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_1/drop_integrations_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_1/group_level_background_subtract_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_1/reference_pixel_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_1/regroup_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.255609 exotic-miri-1.0.1/exotic_miri/stage_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/align_spectra_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/background_subtract_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/clean_outliers_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/extract_1d_box_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/extract_1d_optimal_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/exotic_miri/stage_2/inspect_dq_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.251609 exotic-miri-1.0.1/exotic_miri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-03 13:02:09.000000 exotic-miri-1.0.1/exotic_miri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 13:02:09.000000 exotic-miri-1.0.1/exotic_miri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:02:09.000000 exotic-miri-1.0.1/exotic_miri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 13:02:09.000000 exotic-miri-1.0.1/exotic_miri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 13:02:09.000000 exotic-miri-1.0.1/exotic_miri.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 13:02:09.259609 exotic-miri-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:02:09.259609 exotic-miri-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/tests/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/tests/test_stage_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-08-03 13:01:57.000000 exotic-miri-1.0.1/tests/test_stage_2.py
```

### Comparing `exotic-miri-1.0.0/LICENSE` & `exotic-miri-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/__init__.py` & `exotic-miri-1.0.1/exotic_miri/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/get_default_gain.py` & `exotic-miri-1.0.1/exotic_miri/reference/get_default_gain.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def process(self, input):
         """ Get and save gain data from the default CRDS files.
 
         Parameters
         ----------
         input: jwst.datamodels.RampModel or jwst.datamodels.CubeModel
-            This is either an uncal.fits and rateints.fits loaded
+            This is either an uncal.fits or rateints.fits loaded
             data segment. The gain will be the same no matter which
             data segment you pass in.
         median_value : boolean
             If True only return the median value rather than the gain
             model. Default is False.
         save : boolean
             If True save the gain model to disc. Default is False.
```

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/get_default_readnoise.py` & `exotic-miri-1.0.1/exotic_miri/reference/get_default_readnoise.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def process(self, input):
         """ Get and save readnoise data from the default CRDS files.
 
         Parameters
         ----------
         input: jwst.datamodels.RampModel or jwst.datamodels.CubeModel
-            This is either an uncal.fits and rateints.fits loaded
+            This is either an uncal.fits or rateints.fits loaded
             data segment. The readnoise will be the same no matter which
             data segment you pass in.
         median_value : boolean
             If True only return the median value rather than the readnoise
             model. Default is False.
         save : boolean
             If True save the readnoise model to disc. Default is False.
```

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/get_integration_times.py` & `exotic-miri-1.0.1/exotic_miri/reference/get_integration_times.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/get_wavelength_map.py` & `exotic-miri-1.0.1/exotic_miri/reference/get_wavelength_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class GetWavelengthMap(Step):
     """ Get the wavelength map. """
 
     spec = """
     trim_col_start = integer(default=0)  # trim columns before this index.
-    trim_col_end = integer(default=73)  # trim columns on and after this index.
+    trim_col_end = integer(default=72)  # trim columns on and after this index.
     save = boolean(default=False)  # save map to disk as .fits.
     save_path = string(default=None)  # save map path.
     """
 
     def process(self, input):
         """ Get and save the wavelength map data. This is the mapping from
         the detector pixels (row_idx, col_idx) to wavelength (lambda). To
```

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/set_custom_gain.py` & `exotic-miri-1.0.1/exotic_miri/reference/set_custom_gain.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/reference/set_custom_linearity.py` & `exotic-miri-1.0.1/exotic_miri/reference/set_custom_linearity.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,34 @@
     draw_corrections = boolean(default=False)  # draw corrections
     """
 
     def process(self, input):
         """ Make self-calibrated linearity corrections per amplifier. This
         step uses the uncal.fits data to create a new linearity model.
         This model can then be passed to the jwst.calwebb_detector1.linearity_step
-        via the arg 'override_gain'.
+        via the arg 'override_linearity'.
 
-        The correction involves extrapolating a linear fit to an assumed linear, or
-        well behaved section of the ramps, and then fitting a polynomial to the
+        The correction involves extrapolating a linear fit to an assumed linear
+        /“well-behaved” section of the ramps, and then fitting a polynomial to the
         residuals. The polynomial has the constant- and linear-term coefficients
         fixed at 0 and 1 respectively. Recommended usage requires a large number
         of groups, >~40, although this is still experimental.
 
         Parameters
         ----------
         input: jwst.datamodels.RampModel
             This is an uncal.fits loaded data segment.
         group_idx_start_fit: integer
             The first group index included in the linear fit. This corresponds to
-            the start of the ramp which is assumed to be well behaved. Default is
-            10.
+            the start of the section of the ramp which is assumed to be well behaved.
+            Default is 10.
         group_idx_end_fit: integer
             The last group index included in the linear fit. This corresponds to
-            the end of the ramp which is assumed to be well behaved. Default is
-            40.
+            the end of the section of the ramp which is assumed to be well behaved.
+            Default is 40.
         group_idx_start_derive: integer
             The first group index included in the derived linearity correction.
             Default is 10.
         group_idx_end_derive: integer
             The last group index included in the derived linearity correction.
             Default is -1.
         row_idx_start_used: integer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_1/__init__.py` & `exotic-miri-1.0.1/exotic_miri/stage_1/__init__.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_1/drop_groups_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_1/drop_groups_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
     spec = """
     drop_groups = int_list(default=None)  # groups to drop, zero-indexed.
     """
 
     def process(self, input):
         """ Drop groups which may be adversely affecting the ramps. This
-        may be due to detector effects such RSCD and the last frame effect.
+        may be due to detector effects such RSCD and/or the last frame effect.
         This step simply marks groups as do_not_use and are thus ignored
         in subsequent processing, such as by jwst.calwebb_detector1.ramp_fit_step.
 
         Parameters
         ----------
         input: jwst.datamodels.RampModel
             This is an uncal.fits loaded data segment.
         drop_groups: list of integers
             These integers are the groups to be dropped. The integers are
             zero-indexed such that 0 is the first group.
 
         Returns
         -------
         output: jwst.datamodels.RampModel
-            A RampModel with groupdg flags set as do_not_use (2**0).
+            A RampModel with groupdq flags set as do_not_use (2**0).
 
         """
         with datamodels.open(input) as input_model:
 
             # Copy input model.
             thinned_model = input_model.copy()
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_1/drop_integrations_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_1/drop_integrations_step.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_1/group_level_background_subtract_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_1/group_level_background_subtract_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         """ Subtract the background at the group level.
 
         Parameters
         ----------
         input: jwst.datamodels.RampModel
             This is an uncal.fits loaded data segment.
         method: string
-            The background subtraction method. constant: the background is
-            estimated as a median over the entire background region. row_wise
-            the background is estimated as a median per row. col_wise the
+            The background subtraction method: constant, the background is
+            estimated as a median over the entire background region; row_wise,
+            the background is estimated as a median per row; col_wise; the
             background is estimated within a row as a linear function of
             column number. Default is row_wise.
         bkg_col_left_start: integer
             The column index of the start of the background region on the
             left side of the spectral trace. Default is 8.
         bkg_col_left_end: integer
             The column index of the end of the background region on the
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_1/reference_pixel_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_1/reference_pixel_step.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_1/regroup_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_1/regroup_step.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/__init__.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/__init__.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/align_spectra_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/align_spectra_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,29 @@
         """ Align the 1D stellar spectra. This step measures, by cross-correlation,
         the x- and y-positions of the spectral trace through time. These positions
         are returned and the spectra can optionally be realigned by the y-positions.
 
         Parameters
         ----------
         input: jwst.datamodels.CubeModel
-            This is an rateints.fits loaded data segment.
+            This is a rateints.fits loaded data segment.
         align_spectra: boolean
             If True the spectra are realigned by the measured y-positions. Default
-            is False.
+            is True.
         draw_cross_correlation_fits: boolean
             Plot the cross-correlation function and the fit to this determining the
             trace position.
         draw_trace_positions: boolean
-            Plot the measure trace positions.
+            Plot the measured trace positions.
 
         Returns
         -------
         spectra, spectra_uncertainties, x_shifts, y_shifts: tuple(np.ndarray, np.ndarray, np.ndarray, np.ndarray)
             The time-series spectra and their uncertainties each with
-            shape (n_ints, n_wavelengths) and the measure trace shifts
+            shape (n_ints, n_wavelengths) and the measured trace shifts
             in x and y each with shape (n_ints,).
 
         """
         with datamodels.open(input) as input_model:
 
             # Check input model type.
             if not isinstance(input_model, datamodels.CubeModel):
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/background_subtract_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/background_subtract_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         """ Subtract the background from the rate-images.
 
         Parameters
         ----------
         input: jwst.datamodels.CubeModel
             This is a rateints.fits loaded data segment.
         method: string
-            The background subtraction method. constant: the background is
-            estimated as a median over the entire background region. row_wise
-            the background is estimated as a median per row. col_wise the
+            The background subtraction method: constant, the background is
+            estimated as a median over the entire background region; row_wise,
+            the background is estimated as a median per row; col_wise, the
             background is estimated within a row as a linear function of
             column number. Default is row_wise.
         bkg_col_left_start: integer
             The column index of the start of the background region on the
             left side of the spectral trace. Default is 8.
         bkg_col_left_end: integer
             The column index of the end of the background region on the
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/clean_outliers_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/clean_outliers_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import matplotlib.patches as patches
 
 
 class CleanOutliersStep(Step):
     """ Clean outliers step. """
 
     spec = """
-    window_widths = int_list(default=None)  # window widths for spatial profile fitting.
+    window_heights = int_list(default=None)  # window heights for spatial profile fitting.
     dq_bits_to_mask = int_list(default=None)  # dq flags for which pixels to clean.
     poly_order = integer(default=4)  # spatial profile polynomial fitting order.
     outlier_threshold = float(default=4.0)  # spatial profile fitting outlier sigma.
     spatial_profile_left_idx = integer(default=26)  # left-side of aperture width.
     spatial_profile_right_idx = integer(default=47)  # right-side of aperture width.
     draw_cleaning_col = boolean(default=False)  # draw columns of window cleaning.
     draw_spatial_profiles = boolean(default=False)  # draw spatial profile.
@@ -37,25 +37,25 @@
 
         NB. DQ array bit values as per:
         `https://jwst-pipeline.readthedocs.io/en/latest/jwst/references_general/references_general.html?#data-quality-flags`.
 
         Parameters
         ----------
         input: jwst.datamodels.CubeModel
-            This is an rateints.fits loaded data segment.
-        window_widths: list of integers
+            This is a rateints.fits loaded data segment.
+        window_heights: list of integers
             The size of the windows in pixels, in the dispersion direction, to
             use when fitting polynomials to the spatial profile. The size of the
             window iterates cyclically through the list until the total height
             of the detector is reached. Recommended to use smaller window sizes
             at the shorter wavelengths (larger row indexes) as the throughput *
             stellar spectra show larger variations here. For example,
             [150, 100, 50, 50, 20, 20, 20].
         dq_bits_to_mask: list of integers
-            A list of data quality flags to clean. These pixels are replaces by
+            A list of data quality flags to clean. These pixels are replaced by
             the spatial profile values. See link above for definitions of the
             DQ bit values. For example, [0, ] cleans pixes marked as 2**0
             (do_not_use) in the DQ array.
         poly_order: integer
             Polynomial order for fitting to the windows of data. Default is 4.
         outlier_threshold: float
             Number of standard deviations away from the spatial profile for a
@@ -74,15 +74,15 @@
         no_clean: boolean
             Override, and just remove any nans. This is for quick tests.
 
         Returns
         -------
         output, spatial profile cube, outlier counts cube: tuple(CubeModel, np.ndarray, np.ndarray)
             A CubeModel with outliers cleaned, a 3D array of the
-            fitted spatial profiles,and a count of the number of outliers
+            fitted spatial profiles, and a count of the number of outliers
             cleaned within 0-4 pixels of the spectral trace (column index 36).
 
         """
         with datamodels.open(input) as input_model:
 
             # Copy input model.
             cleaned_model = input_model.copy()
@@ -114,19 +114,19 @@
         # Count number of replaced pixels on and near the spectral trace.
         outliers = self._count_outliers(cleaned_model)
 
         return cleaned_model, self.P, outliers
 
     def _clean(self):
         """ Clean dq bits and via optimal extraction method of Horne 1986. """
-        # Prep cycling of window widths to span all rows.
+        # Prep cycling of window heights to span all rows.
         n_ints, n_rows, n_cols = self.D.shape
-        window_widths = np.tile(self.window_widths, int(np.ceil(
-            n_rows / np.sum(self.window_widths))))
-        window_start_idxs = np.concatenate([[0, ], np.cumsum(window_widths)])
+        window_heights = np.tile(self.window_heights, int(np.ceil(
+            n_rows / np.sum(self.window_heights))))
+        window_start_idxs = np.concatenate([[0, ], np.cumsum(window_heights)])
 
         # Iterate integrations.
         for int_idx in range(n_ints):
 
             # Iterate windows of several rows.
             for win_start_idx, win_end_idx in zip(window_start_idxs, window_start_idxs[1:]):
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/extract_1d_box_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/extract_1d_box_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 
     def process(self, input, wavelength_map):
         """ Extract time-series 1D stellar spectra using a box aperture.
 
         Parameters
         ----------
         input: jwst.datamodels.CubeModel
-            This is an rateints.fits loaded data segment.
+            This is a rateints.fits loaded data segment.
         wavelength_map: np.ndarray
             The wavelength map. This is output from
             exotic_miri.reference.GetWavelengthMap.
         trace_position: string
             The method for locating the spectral trace per detector row.
             constant: uses the value specified by aperture_center.
             gaussian_fits: fit a Gaussian to each row to find the centre.
         aperture_center: integer
             The defined centre of the spectral trace in terms of column
             index. Default is 36.
         aperture_left_width: integer
             The half-width of the box aperture in pixels away from the
-            aperture_center. Default is 4, and so this aperture would
-            include the aperture_center, say column 36, and 4 columns
+            aperture_center to the left. Default is 4, and so this aperture
+            would include the aperture_center, say column 36, and 4 columns
             to the left of this.
         aperture_right_width: integer
             The half-width of the box aperture in pixels away from the
-            aperture_center. Default is 4, and so this aperture would
-            include the aperture_center, say column 36, and 4 columns
+            aperture_center to the right. Default is 4, and so this aperture
+            would include the aperture_center, say column 36, and 4 columns
             to the right of this.
         draw_psf_fits: boolean
             Plot Gaussina fits to the PSF.
         draw_aperture: boolean
             Plot the defined aperture.
         draw_spectra: boolean
             Plot the extracted 1D spectra.
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/extract_1d_optimal_step.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/extract_1d_optimal_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """ Extract time-series 1D stellar spectra using optimal
         extraction as detailed in Horne 1986. The spatial profile
         must be pre-computed and input.
 
         Parameters
         ----------
         input: jwst.datamodels.CubeModel
-            This is an rateints.fits loaded data segment.
+            This is a rateints.fits loaded data segment.
         wavelength_map: np.ndarray
             The wavelength map. This is output from
             exotic_miri.reference.GetWavelengthMap.
         P: np.ndarray
             A cube of spatial profiles, one for each integration, of shape
             (n_ints, n_rows, n_cols). The should be normalised within
             each row (cross-disperion direction). These data can be made
```

### Comparing `exotic-miri-1.0.0/exotic_miri/stage_2/inspect_dq_flags.py` & `exotic-miri-1.0.1/exotic_miri/stage_2/inspect_dq_flags.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/exotic_miri.egg-info/SOURCES.txt` & `exotic-miri-1.0.1/exotic_miri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/setup.py` & `exotic-miri-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     h = os.path.dirname(os.path.realpath(__file__))
     with codecs.open(os.path.join(h, *parts), "rb", "utf-8") as f:
         return f.read()
 
 
 setup(
     name="exotic-miri",
-    version="1.0.0",
+    version="1.0.1",
     author="David Grant",
     author_email="david.grant@bristol.ac.uk",
     url="https://github.com/Exo-TiC/ExoTiC-MIRI",
     license="MIT",
     packages=["exotic_miri.stage_1", "exotic_miri.stage_2", "exotic_miri.reference"],
     description="ExoTiC MIRI data reduction steps",
     long_description=read("README.rst"),
```

### Comparing `exotic-miri-1.0.0/tests/test_reference.py` & `exotic-miri-1.0.1/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/tests/test_stage_1.py` & `exotic-miri-1.0.1/tests/test_stage_1.py`

 * *Files identical despite different names*

### Comparing `exotic-miri-1.0.0/tests/test_stage_2.py` & `exotic-miri-1.0.1/tests/test_stage_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         custom_clean_outliers = CleanOutliersStep()
         for dq_m in [[], [0,], [0, 2]]:
             for ww in [[100], [150, 100, 50, 50, 20, 20, 20]]:
                 for po in [1, 3]:
                     self.cube_model, P, O = custom_clean_outliers.call(
                         self.cube_model, dq_bits_to_mask=dq_m,
-                        window_widths=ww, poly_order=po, outlier_threshold=5.0)
+                        window_heights=ww, poly_order=po, outlier_threshold=5.0)
 
                     self.assertIsInstance(self.cube_model, datamodels.CubeModel)
                     self.assertIsInstance(P, np.ndarray)
                     self.assertIsInstance(O, np.ndarray)
 
                     self.assertEqual(self.cube_model.shape, (3, 416, 72))
                     self.assertEqual(P.shape, (3, 416, 72))
```

