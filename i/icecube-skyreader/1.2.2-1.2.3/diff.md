# Comparing `tmp/icecube-skyreader-1.2.2.tar.gz` & `tmp/icecube-skyreader-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-1.2.2.tar", last modified: Thu Jul 13 21:16:51 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.2.3.tar", last modified: Thu Aug  3 16:19:57 2023, max compression
```

## Comparing `icecube-skyreader-1.2.2.tar` & `icecube-skyreader-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.305630 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1762 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.305630 icecube-skyreader-1.2.2/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-13 21:16:48.000000 icecube-skyreader-1.2.2/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9057 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    47135 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:19:57.297475 icecube-skyreader-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-08-03 16:19:57.297475 icecube-skyreader-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:19:57.293475 icecube-skyreader-1.2.3/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-08-03 16:19:57.000000 icecube-skyreader-1.2.3/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-08-03 16:19:57.000000 icecube-skyreader-1.2.3/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 16:19:57.000000 icecube-skyreader-1.2.3/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-08-03 16:19:57.000000 icecube-skyreader-1.2.3/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 16:19:57.000000 icecube-skyreader-1.2.3/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-08-03 16:19:57.297475 icecube-skyreader-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:19:57.297475 icecube-skyreader-1.2.3/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-03 16:19:53.000000 icecube-skyreader-1.2.3/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:19:57.297475 icecube-skyreader-1.2.3/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    47519 2023-08-03 16:19:52.000000 icecube-skyreader-1.2.3/skyreader/result.py
```

### Comparing `icecube-skyreader-1.2.2/LICENSE` & `icecube-skyreader-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.2/PKG-INFO` & `icecube-skyreader-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.2.2
+Version: 1.2.3
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.2.2/README.md` & `icecube-skyreader-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.2/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.2.3/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.2.2
+Version: 1.2.3
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.2.2/setup.cfg` & `icecube-skyreader-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.2/skyreader/__init__.py` & `icecube-skyreader-1.2.3/skyreader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-1.2.2/skyreader/event_metadata.py` & `icecube-skyreader-1.2.3/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.2/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.2.3/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.2/skyreader/result.py` & `icecube-skyreader-1.2.3/skyreader/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import io
 import itertools as it
 import json
 import logging
 import pickle
 from functools import cached_property
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, TypedDict, Union
+from typing import Any, Dict, Final, List, Optional, Tuple, TypedDict, Union
 
 import healpy  # type: ignore[import]
 import matplotlib  # type: ignore[import]
 import meander  # type: ignore[import]
 import numpy as np
 import pandas as pd  # type: ignore[import]
 from astropy.io import ascii  # type: ignore[import]
@@ -64,20 +64,21 @@
 PyDictResult = Dict[str, PyDictNSidePixels]
 
 
 ###############################################################################
 # MAIN CLASS
 
 class SkyScanResult:
-    """This class parses a nsides_dict and stores the relevant numeric result
+    """This class parses a scan result and stores the relevant numeric results
     of the scan. Ideally it should serve as the basic data structure for
     plotting / processing / transmission of the scan result.
 
-    nsides_dict is a dictionary keyed by 'nside' values for which a scan
-    result is available (e.g. 8, 64, 512), see `pixel_classes.NSidesDict`.
+    `result` is a dictionary keyed by 'nside: str' values for which a scan
+    result is available (e.g. 8, 64, 512).
+
     The scan result is a dictionary:
     - i (pixel index, integer) ->
         'frame', 'llh', 'recoLossesInside', 'recoLossesTotal'
 
     The numeric values of interest are 'llh', 'recoLossesInside',
     'recoLossesTotal'. The pixel indices in the input dictionary are in
     general unsorted (python dict are unsorted by design) and are
@@ -91,14 +92,16 @@
 
     PIXEL_TYPE = np.dtype(
         [("index", int), ("llh", float), ("E_in", float), ("E_tot", float)]
     )
     PIXEL_FIELDS: Tuple[str, ...] = PIXEL_TYPE.names  # type: ignore[assignment]
     ATOL = 1.0e-8  # 1.0e-8 is the default used by np.isclose()
 
+    MINIMAL_METADATA_FIELDS: Final[List[str]] = "run_id event_id mjd event_type nside".split()
+
     def __init__(self, result: Dict[str, np.ndarray]):
         self.logger = logging.getLogger(__name__)
 
         # validate result data
         if not isinstance(result, dict):
             raise ValueError("'result' must be an instance of Dict[str, np.ndarray]")
         for nside in result:
@@ -197,27 +200,27 @@
                 diff, test = s_val - o_val, s_val == o_val
 
             diff_vals.append(diff)
             test_vals.append(test)
 
         return diff_vals, test_vals
 
-    def has_metadata(self) -> bool:
+    def has_minimal_metadata(self) -> bool:
         """Check that the minimum metadata is set."""
-        for mk in "run_id event_id mjd event_type nside".split():
+        for mk in self.MINIMAL_METADATA_FIELDS:
             for k in self.result:
                 if self.result[k].dtype.metadata is None:
                     return False
                 if mk not in self.result[k].dtype.metadata:
                     return False
         return True
 
     def get_event_metadata(self) -> EventMetadata:
         """Get the EventMetadata portion of the result's metadata."""
-        if self.has_metadata():
+        if self.has_minimal_metadata():
             first_metadata = self.result[list(self.result.keys())[0]].dtype.metadata
             return EventMetadata(
                 first_metadata['run_id'],
                 first_metadata['event_id'],
                 first_metadata['event_type'],
                 first_metadata['mjd'],
                 first_metadata.get('is_real_event', False),  # assume simulated event
@@ -519,20 +522,26 @@
                 ]
             },
             ...
         }
         """
         pydict: PyDictResult = {}
         for nside in self.result:
+            nside_data: np.ndarray = self.result[nside]
             df = pd.DataFrame(
-                self.result[nside],
-                columns=list(self.result[nside].dtype.names),
+                nside_data,
+                columns=list(nside_data.dtype.names),
             )
             pydict[nside] = {k:v for k,v in df.to_dict(orient='split').items() if k != 'index'}  # type: ignore[assignment]
-            pydict[nside]['metadata'] = dict(self.result[nside].dtype.metadata)
+            pydict[nside]['metadata'] = dict()
+
+            for key in nside_data.dtype.metadata:
+                # dtype.metadata is a mappingproxy (dict-like) containing numpy-typed values
+                # convert numpy types to python bultins to be JSON-friendly
+                pydict[nside]['metadata'][key] = nside_data.dtype.metadata[key].item()
         return pydict
 
     """
     Querying
     """
 
     def llh(self, ra, dec):
@@ -948,15 +957,15 @@
         # Calculate the contours
         if systematics:
             # from Pan-Starrs event 127852
             contour_levels = (np.array([22.2, 64.2])+min_value) # these are values determined from MC by Will on the TS (2*LLH)
             contour_labels = [r'50% (IC160427A syst.)', r'90% (IC160427A syst.)']
             contour_colors=['k', 'r']
         else:
-            # # Wilk's
+            # Wilks
             contour_levels = (np.array([1.39, 4.61, 11.83, 28.74])+min_value)[:3]
             contour_labels = [r'50%', r'90%', r'3$\sigma$', r'5$\sigma$'][:3]
             contour_colors=['k', 'r', 'g', 'b'][:3]
 
         sample_points = np.array([np.pi/2 - grid_dec, grid_ra]).T
         # Call meander module to find contours
         contours_by_level = meander.spherical_contours(sample_points,
@@ -1236,15 +1245,15 @@
             fig.savefig(plot_filename, dpi=dpi, transparent=True)
 
         print("done.")
 
         if systematics is True:
             title = "Millipede contour, assuming IC160427A systematics:"
         else:
-            title = "Millipede contour, assuming Wilk's Theorum:"
+            title = "Millipede contour, assuming Wilks' Theorem:"
 
         for i, ch in enumerate(final_channels):
             imgdata = io.BytesIO()
             fig.savefig(imgdata, format='png', dpi=600, transparent=True)
             imgdata.seek(0)
 
             savename = plot_filename[:-4] + ".png"
```

