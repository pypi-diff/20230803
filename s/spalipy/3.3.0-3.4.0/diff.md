# Comparing `tmp/spalipy-3.3.0.tar.gz` & `tmp/spalipy-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spalipy-3.3.0.tar", last modified: Tue Nov 22 17:43:33 2022, max compression
+gzip compressed data, was "dist/spalipy-3.4.0.tar", last modified: Thu Aug  3 21:03:27 2023, max compression
```

## Comparing `spalipy-3.3.0.tar` & `spalipy-3.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2022-11-22 17:43:33.498820 spalipy-3.3.0/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)    32422 2018-07-30 16:05:55.000000 spalipy-3.3.0/LICENSE.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       13 2018-07-31 10:12:11.000000 spalipy-3.3.0/MANIFEST.in
--rw-r--r--   0 jdl       (1000) jdl       (1000)    10190 2022-11-22 17:43:33.498820 spalipy-3.3.0/PKG-INFO
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     7891 2022-01-27 18:16:16.000000 spalipy-3.3.0/README.md
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       50 2022-11-22 17:36:14.000000 spalipy-3.3.0/requirements.txt
--rw-r--r--   0 jdl       (1000) jdl       (1000)      115 2022-11-22 17:43:33.498820 spalipy-3.3.0/setup.cfg
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     1788 2022-04-11 15:44:57.000000 spalipy-3.3.0/setup.py
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2022-11-22 17:43:33.496820 spalipy-3.3.0/spalipy/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      788 2022-11-22 17:41:48.000000 spalipy-3.3.0/spalipy/__init__.py
--rw-rw-r--   0 jdl       (1000) jdl       (1000)    64821 2022-11-22 17:38:01.000000 spalipy-3.3.0/spalipy/spalipy.py
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2022-11-22 17:43:33.497820 spalipy-3.3.0/spalipy.egg-info/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)    10190 2022-11-22 17:43:32.000000 spalipy-3.3.0/spalipy.egg-info/PKG-INFO
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      370 2022-11-22 17:43:32.000000 spalipy-3.3.0/spalipy.egg-info/SOURCES.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)        1 2022-11-22 17:43:32.000000 spalipy-3.3.0/spalipy.egg-info/dependency_links.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      101 2022-11-22 17:43:32.000000 spalipy-3.3.0/spalipy.egg-info/entry_points.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       51 2022-11-22 17:43:32.000000 spalipy-3.3.0/spalipy.egg-info/requires.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       13 2022-11-22 17:43:32.000000 spalipy-3.3.0/spalipy.egg-info/top_level.txt
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2022-11-22 17:43:33.498820 spalipy-3.3.0/test/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)        0 2021-04-01 14:53:21.000000 spalipy-3.3.0/test/__init__.py
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     1117 2022-04-20 16:09:30.000000 spalipy-3.3.0/test/check_mem.py
--rw-r--r--   0 jdl       (1000) jdl       (1000)     1162 2022-04-22 14:29:51.000000 spalipy-3.3.0/test/debugging.py
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     9977 2022-11-22 17:31:27.000000 spalipy-3.3.0/test/test_spalipy.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-08-03 21:03:27.608216 spalipy-3.4.0/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)    32422 2018-07-30 16:05:55.000000 spalipy-3.4.0/LICENSE.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       13 2018-07-31 10:12:11.000000 spalipy-3.4.0/MANIFEST.in
+-rw-r--r--   0 jdl       (1000) jdl       (1000)    10190 2023-08-03 21:03:27.608216 spalipy-3.4.0/PKG-INFO
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)     7891 2022-01-27 18:16:16.000000 spalipy-3.4.0/README.md
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       50 2022-11-22 17:36:14.000000 spalipy-3.4.0/requirements.txt
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      115 2023-08-03 21:03:27.609216 spalipy-3.4.0/setup.cfg
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)     1788 2022-04-11 15:44:57.000000 spalipy-3.4.0/setup.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-08-03 21:03:27.605216 spalipy-3.4.0/spalipy/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      788 2023-08-03 21:02:55.000000 spalipy-3.4.0/spalipy/__init__.py
+-rw-r--r--   0 jdl       (1000) jdl       (1000)    64842 2023-08-03 21:02:55.000000 spalipy-3.4.0/spalipy/spalipy.py
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      545 2023-08-03 21:02:55.000000 spalipy-3.4.0/spalipy/utils.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-08-03 21:03:27.607216 spalipy-3.4.0/spalipy.egg-info/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)    10190 2023-08-03 21:03:27.000000 spalipy-3.4.0/spalipy.egg-info/PKG-INFO
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)      387 2023-08-03 21:03:27.000000 spalipy-3.4.0/spalipy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)        1 2023-08-03 21:03:27.000000 spalipy-3.4.0/spalipy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)      101 2023-08-03 21:03:27.000000 spalipy-3.4.0/spalipy.egg-info/entry_points.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       51 2023-08-03 21:03:27.000000 spalipy-3.4.0/spalipy.egg-info/requires.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       13 2023-08-03 21:03:27.000000 spalipy-3.4.0/spalipy.egg-info/top_level.txt
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-08-03 21:03:27.608216 spalipy-3.4.0/test/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)        0 2021-04-01 14:53:21.000000 spalipy-3.4.0/test/__init__.py
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)     1117 2022-04-20 16:09:30.000000 spalipy-3.4.0/test/check_mem.py
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     1162 2022-04-22 14:29:51.000000 spalipy-3.4.0/test/debugging.py
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)     9977 2022-11-22 17:31:27.000000 spalipy-3.4.0/test/test_spalipy.py
```

### Comparing `spalipy-3.3.0/LICENSE.txt` & `spalipy-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spalipy-3.3.0/PKG-INFO` & `spalipy-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spalipy
-Version: 3.3.0
+Version: 3.4.0
 Summary: Detection-based astrononmical image registration
 Home-page: https://github.com/Lyalpha/spalipy
 Author: Joe Lyman
 Author-email: joedlyman@gmail.com
 License: UNKNOWN
 Description: # spalipy
```

### Comparing `spalipy-3.3.0/README.md` & `spalipy-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `spalipy-3.3.0/setup.py` & `spalipy-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `spalipy-3.3.0/spalipy/__init__.py` & `spalipy-3.4.0/spalipy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .spalipy import Spalipy
 
-__version__ = "3.3.0"
+__version__ = "3.4.0"
```

### Comparing `spalipy-3.3.0/spalipy/spalipy.py` & `spalipy-3.4.0/spalipy/spalipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 import sep
 from astropy.io import fits
 from astropy.table import Table, vstack
 from scipy import linalg, interpolate
 from scipy.ndimage import interpolation, map_coordinates
 from scipy.spatial import cKDTree, distance
 
+from spalipy.utils import _c_array_prep
+
 # expose dfitpack errors so we can catch them later
 try:
     interpolate.dfitpack.sproot(-1, -1, -1)
 except Exception as _e:
     dfitpackError = type(_e)
 
 
@@ -204,14 +206,18 @@
     cval_mask : float, optional
         The value used to fill regions of the aligned mask where
         there is no overlap with template image.
     skip_checking : boolean
         Whether to skip some basic checking of input arguments for
         minor speed up when setting-up. Useful when inputs are fixed
         and already known.
+    copy : boolean
+        Source and Template data is converted to float64 internally,
+        if true, a copy of the input data is made to avoid modifying
+        the original, otherwise the input data is modified in-place.
     """
 
     x_col = "x"
     y_col = "y"
     flux_col = "flux"
     fwhm_col = "fwhm"
     flag_col = "flag"
@@ -241,14 +247,15 @@
         min_fwhm: float = 1,
         bad_flag_bits: int = 0,
         min_sep: float = None,
         preserve_footprints: bool = False,
         cval: float = 0,
         cval_mask: float = 0,
         skip_checking: bool = False,
+        copy: bool = True,
     ):
 
         self.n_det = n_det
         self.n_quad_det = n_quad_det
         self.min_quad_sep = min_quad_sep
         self.max_match_dist = max_match_dist
         self.min_n_match = min_n_match
@@ -268,14 +275,15 @@
         self.cval_mask = cval_mask
 
         if isinstance(source_data, np.ndarray):
             source_data = [source_data]
             self._source_inputs_as_list = False
         else:
             self._source_inputs_as_list = True
+
         self._n_source_entry = len(source_data)
         if source_mask is None or isinstance(source_mask, np.ndarray):
             source_mask = [source_mask] * self._n_source_entry
         if output_shape is None or isinstance(output_shape, tuple):
             output_shape = [output_shape] * self._n_source_entry
         if source_det is None or isinstance(source_det, Table):
             source_det = [source_det] * self._n_source_entry
@@ -318,14 +326,26 @@
             if template_data is None and template_det is None:
                 raise ValueError("One of template_data or template_det must be provided")
             if template_data is not None and template_data.ndim != 2:
                 raise ValueError(f"The dimensionality of template_data is not 2")
             if preserve_footprints and template_data is None:
                 raise ValueError("preserve_footprints=True requires template_data to be provided")
 
+        for i, arr in enumerate(source_data):
+            if arr.dtype != np.float64:
+                if copy:
+                    source_data[i] = arr.astype(np.float64)
+                else:
+                    arr.astype(np.float64, copy=False)
+        if template_data is not None and template_data.dtype != np.float64:
+            if copy:
+                template_data = template_data.astype(np.float64)
+            else:
+                template_data.astype(np.float64, copy=False)
+
         self._source_data = source_data
         self._source_mask = source_mask
         self._source_det = []
         self._source_coo = []
         self._output_shape = []
         for i, (_source_data, _source_det, _output_shape) in enumerate(
             zip(source_data, source_det, output_shape)
@@ -922,34 +942,16 @@
                     ) & (np.abs(sub_tile_centre_y - coo[:, 1]) <= (sub_tile_height / 2))
                     if edge_mask is not None:
                         sub_tile_mask &= edge_mask
                     yield sub_tile_mask
 
     def _extract_detections(self, data):
         """Return an astropy Table of detections found in input data"""
-
-        def get_background(_data):
-            try:
-                _bkg = sep.Background(_data)
-            except ValueError as e:
-                # See https://sep.readthedocs.io/en/latest/tutorial.html#Finally-a-brief-word-on-byte-order
-                if "has non-native byte order" in str(e):
-                    _data = _data.byteswap(inplace=True).newbyteorder()
-                elif "input array dtype not supported" in str(e):
-                    logging.warning(f"Converting data from dtype {_data.dtype} to float64")
-                    _data = _data.astype(np.float64)
-                _bkg = sep.Background(_data)
-            return _bkg
-
-        # Try twice to get the background to allow once for non-native byte order, and once for wrong dtype
-        for i in range(2):
-            bkg = get_background(data)
-            break
-        else:
-            raise RuntimeError("Failed to get background")
+        data = _c_array_prep(data)
+        bkg = sep.Background(data)
 
         bkg_rms = bkg.rms()
         data_sub = data - bkg.back()
 
         extracted_det = sep.extract(data_sub, thresh=self.sep_thresh, err=bkg_rms,)
         det = Table(extracted_det)
         det["fwhm"] = 2.0 * (np.log(2) * (det["a"] ** 2.0 + det["b"] ** 2.0)) ** 0.5
@@ -1224,15 +1226,16 @@
     args_dict.pop("source_cat", None)
     args_dict.pop("template_cat", None)
     args_dict.pop("source_ext", None)
     args_dict.pop("template_ext", None)
     args_dict.pop("verbose", None)
 
     logging.info("Initialising Spalipy instance")
-    s = Spalipy(**args_dict)
+    # Always use copy=False since we're reading/writing to files anyway
+    s = Spalipy(**args_dict, copy=False)
     s.align()
     s.log_transform_stats()
 
     logging.info(f"Writing aligned source data to {output_filename}")
     fits.writeto(output_filename, data=s.aligned_data, overwrite=overwrite)
```

### Comparing `spalipy-3.3.0/spalipy.egg-info/PKG-INFO` & `spalipy-3.4.0/spalipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spalipy
-Version: 3.3.0
+Version: 3.4.0
 Summary: Detection-based astrononmical image registration
 Home-page: https://github.com/Lyalpha/spalipy
 Author: Joe Lyman
 Author-email: joedlyman@gmail.com
 License: UNKNOWN
 Description: # spalipy
```

### Comparing `spalipy-3.3.0/test/check_mem.py` & `spalipy-3.4.0/test/check_mem.py`

 * *Files identical despite different names*

### Comparing `spalipy-3.3.0/test/debugging.py` & `spalipy-3.4.0/test/debugging.py`

 * *Files identical despite different names*

### Comparing `spalipy-3.3.0/test/test_spalipy.py` & `spalipy-3.4.0/test/test_spalipy.py`

 * *Files identical despite different names*

