# Comparing `tmp/bletl-1.3.1.tar.gz` & `tmp/bletl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bletl-1.3.1.tar", last modified: Tue Jun 20 12:43:55 2023, max compression
+gzip compressed data, was "bletl-1.4.0.tar", last modified: Thu Aug  3 11:26:33 2023, max compression
```

## Comparing `bletl-1.3.1.tar` & `bletl-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.626867 bletl-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34452 2023-06-20 12:34:36.000000 bletl-1.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 12:34:36.000000 bletl-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-20 12:43:55.622867 bletl-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-20 12:34:36.000000 bletl-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/bletl/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/bletl/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/parsing/bl1.py
--rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/parsing/blpro.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/splines.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/bletl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:34:44.000000 bletl-1.3.1/bletl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-20 12:34:36.000000 bletl-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:43:55.626867 bletl-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-20 12:34:36.000000 bletl-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.965824 bletl-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34452 2023-08-03 11:13:45.000000 bletl-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 11:13:45.000000 bletl-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-03 11:26:33.965824 bletl-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-03 11:13:45.000000 bletl-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.957825 bletl-1.4.0/bletl/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.961825 bletl-1.4.0/bletl/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/parsing/bl1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/parsing/blpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/splines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.961825 bletl-1.4.0/bletl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:13:55.000000 bletl-1.4.0/bletl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 11:13:45.000000 bletl-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:26:33.965824 bletl-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-03 11:13:45.000000 bletl-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.965824 bletl-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_splines.py
```

### Comparing `bletl-1.3.1/LICENSE.md` & `bletl-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/PKG-INFO` & `bletl-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bletl
-Version: 1.3.1
+Version: 1.4.0
 Summary: Package for parsing and transforming BioLector raw data.
 Home-page: https://github.com/jubiotech/bletl
 Author: Michael Osthege
 Author-email: m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3.0
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `bletl-1.3.1/README.md` & `bletl-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/bletl/__init__.py` & `bletl-1.4.0/bletl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from .heuristics import find_do_peak
 from .splines import get_crossvalidated_spline
 from .types import (
     BioLectorModel,
     BLData,
     BLDParser,
     FilterTimeSeries,
+    FluidicsSource,
     IncompatibleFileError,
     InvalidLotNumberError,
     LotInformationError,
     LotInformationMismatch,
     LotInformationNotFound,
     NoMeasurementData,
 )
 
-__version__ = "1.3.1"
+__version__ = "1.4.0"
```

### Comparing `bletl-1.3.1/bletl/core.py` & `bletl-1.4.0/bletl/core.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/bletl/features.py` & `bletl-1.4.0/bletl/features.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/bletl/growth.py` & `bletl-1.4.0/bletl/growth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import logging
-import typing
 from typing import Dict, Optional, Sequence, Tuple, Union
 
 import arviz
 import calibr8
 import numpy
 import pymc as pm
+import pytensor.tensor as pt
 from packaging import version
 
-try:
-    import pytensor.tensor as pt
-except ModuleNotFoundError:
-    import aesara.tensor as pt  # type: ignore
-
-
 _log = logging.getLogger(__file__)
 
 
 class GrowthRateResult:
     """Represents the result of applying the µ(t) model to one dataset."""
 
     def __init__(
@@ -194,16 +188,16 @@
     Returns
     -------
     random_walk : TensorVariable
         The tensor variable of the random walk.
     """
     pmversion = version.parse(pm.__version__)
 
-    if pmversion < version.parse("4.2.2"):
-        raise NotImplementedError("PyMC versions <4.2.2 are no longer supported.")
+    if pmversion < version.parse("5.0.0"):
+        raise NotImplementedError("PyMC versions <5.0.0 are no longer supported.")
 
     if student_t:
         innov_dist = pm.StudentT.dist(mu=mu, sigma=sigma, nu=nu)
     else:
         innov_dist = pm.Normal.dist(mu=mu, sigma=sigma)
 
     rw = pm.RandomWalk(
```

### Comparing `bletl-1.3.1/bletl/heuristics.py` & `bletl-1.4.0/bletl/heuristics.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/bletl/parsing/bl1.py` & `bletl-1.4.0/bletl/parsing/bl1.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/bletl/parsing/blpro.py` & `bletl-1.4.0/bletl/parsing/blpro.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from .. import utils
 from ..types import (
     BioLectorModel,
     BLData,
     BLDParser,
     FilterTimeSeries,
+    FluidicsSource,
     InvalidLotNumberError,
 )
 
 logger = logging.getLogger("blpro")
 
 
 _MF_WELL_NUMC_TO_ID = {
@@ -342,15 +343,15 @@
 
 
 def extract_fluidics(dfraw):
     ocol_ncol_type = [
         ("Cycle", "cycle", int),
         ("Well", "well", int),
         ("Time", "time", float),
-        ("Reservoir", "reservoir", float),
+        ("Reservoir", "reservoir", FluidicsSource),
         ("MF_Volume", "mf_volume", float),
         ("Temp_Ch4", "volume", float),
     ]
     df = utils.__to_typed_cols__(dfraw[dfraw["Type"] == "F"], ocol_ncol_type)
     df["well"] = [_MF_WELL_NUMM_TO_ID[w] for w in df["well"]]
     df = df.sort_values(["well", "cycle"]).set_index(["well"])
     return standardize(df)
```

### Comparing `bletl-1.3.1/bletl/splines.py` & `bletl-1.4.0/bletl/splines.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/bletl/types.py` & `bletl-1.4.0/bletl/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Specifies the base types for parsing and representing BioLector CSV files."""
 import abc
 import enum
 import os
 import typing
-import warnings
 from typing import Dict, Optional, Tuple, Union
 
 import numpy
 import pandas
 
 
 class BioLectorModel(enum.Enum):
@@ -15,14 +14,28 @@
 
     BL1 = "bl1"
     BL2 = "bl2"
     BLPro = "blpro"
     XT = "blXT"
 
 
+class FluidicsSource(enum.IntEnum):
+    """Number that identifies the source of volume changes."""
+
+    ReservoirA = 1
+
+    """Additions from reservoir A."""
+    ReservoirB = 2
+
+    """Additions from reservoir B."""
+
+    Pipetting = -1
+    """Additions from pipetting."""
+
+
 class BLData(dict):
     """Standardized data type for BioLector data."""
 
     def __init__(
         self,
         model: BioLectorModel,
         environment: pandas.DataFrame,
```

### Comparing `bletl-1.3.1/bletl/utils.py` & `bletl-1.4.0/bletl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Contains helper functions that do not depend on other modules within this package."""
 import datetime
+import enum
 import pathlib
 import re
 import urllib
-from typing import Optional, Sequence, Tuple, Union
+from typing import Optional, Sequence, Tuple
 
 import pandas
 
 from . import core
 
 
 def __to_typed_cols__(
@@ -28,14 +29,17 @@
     dfout : DataFrame
         A new data frame with converted & renamed columns as specified by `ocol_ncol_type`.
     """
     dfout = pandas.DataFrame()
     for ocol, ncol, typ in ocol_ncol_type:
         if ocol is None or not ocol in dfin:
             dfout[ncol] = None
+        elif issubclass(typ, enum.Enum):
+            # Enum types are kept as object-series
+            dfout[ncol] = dfin[ocol].apply(lambda x: typ(x), convert_dtype=False)
         else:
             dfout[ncol] = dfin[ocol].astype(typ)
     return dfout
 
 
 def _unindex(dataframe: pandas.DataFrame) -> Tuple[Sequence[Optional[str]], pandas.DataFrame]:
     """Resets the index of the DataFrame.
```

### Comparing `bletl-1.3.1/bletl.egg-info/PKG-INFO` & `bletl-1.4.0/bletl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bletl
-Version: 1.3.1
+Version: 1.4.0
 Summary: Package for parsing and transforming BioLector raw data.
 Home-page: https://github.com/jubiotech/bletl
 Author: Michael Osthege
 Author-email: m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3.0
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `bletl-1.3.1/bletl.egg-info/SOURCES.txt` & `bletl-1.4.0/bletl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/setup.py` & `bletl-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/tests/test_core.py` & `bletl-1.4.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,7 +631,13 @@
         assert bldata.fluidics.loc["C01", "volume"][0] == 800
         assert bldata.fluidics.loc["C01", "volume"][-1] == 1201.776
         assert bldata.fluidics.loc["D01", "volume"][-1] == 1204.892
         assert bldata.fluidics.loc["D02", "volume"][-1] == 954.68
         assert bldata.fluidics.loc["E06", "volume"][-1] == 913.16
         assert bldata.fluidics.loc["F01", "volume"][-1] == 1202.719
         pass
+
+    def test_fluidics_source(self):
+        fp = dir_testfiles / "BLPro" / "18-FZJ-Test2--2018-02-07-10-01-11.csv"
+        bldata = bletl.parse(fp)
+        assert isinstance(bldata.fluidics["reservoir"][0], bletl.FluidicsSource)
+        pass
```

### Comparing `bletl-1.3.1/tests/test_features.py` & `bletl-1.4.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/tests/test_growth.py` & `bletl-1.4.0/tests/test_growth.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/tests/test_heuristics.py` & `bletl-1.4.0/tests/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `bletl-1.3.1/tests/test_splines.py` & `bletl-1.4.0/tests/test_splines.py`

 * *Files identical despite different names*

