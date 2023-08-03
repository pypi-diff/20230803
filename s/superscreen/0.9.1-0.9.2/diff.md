# Comparing `tmp/superscreen-0.9.1.tar.gz` & `tmp/superscreen-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superscreen-0.9.1.tar", last modified: Wed May 17 19:27:44 2023, max compression
+gzip compressed data, was "superscreen-0.9.2.tar", last modified: Mon Jul 10 21:30:08 2023, max compression
```

## Comparing `superscreen-0.9.1.tar` & `superscreen-0.9.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.590081 superscreen-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 19:27:34.000000 superscreen-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 19:27:44.586080 superscreen-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-17 19:27:34.000000 superscreen-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:27:44.590081 superscreen-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 19:27:34.000000 superscreen-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/device/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42839 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/edge_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/fem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46337 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/solve.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/solve_film.py
--rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/vortex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    39839 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.017256 superscreen-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-10 21:29:54.000000 superscreen-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-10 21:30:08.017256 superscreen-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-10 21:29:54.000000 superscreen-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:30:08.017256 superscreen-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-10 21:29:54.000000 superscreen-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.009256 superscreen-0.9.2/superscreen/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.013256 superscreen-0.9.2/superscreen/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43336 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/edge_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/device/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15060 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/fem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46337 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.013256 superscreen-0.9.2/superscreen/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/solver/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/solver/solve_film.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/solver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.013256 superscreen-0.9.2/superscreen/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/sources/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/sources/dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/sources/vortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.017256 superscreen-0.9.2/superscreen/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39839 2023-07-10 21:29:54.000000 superscreen-0.9.2/superscreen/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:30:08.013256 superscreen-0.9.2/superscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-10 21:30:07.000000 superscreen-0.9.2/superscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-10 21:30:07.000000 superscreen-0.9.2/superscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:30:07.000000 superscreen-0.9.2/superscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-10 21:30:07.000000 superscreen-0.9.2/superscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 21:30:07.000000 superscreen-0.9.2/superscreen.egg-info/top_level.txt
```

### Comparing `superscreen-0.9.1/LICENSE` & `superscreen-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/PKG-INFO` & `superscreen-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.9.1
+Version: 0.9.2
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
```

### Comparing `superscreen-0.9.1/README.md` & `superscreen-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/setup.py` & `superscreen-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 EXTRAS_REQUIRE = {
     "dev": [
         "pytest-cov",
         "pre-commit",
     ],
     "docs": [
-        "sphinx",
+        "sphinx<7",
         "sphinx_rtd_theme",
         "sphinx-autodoc-typehints",
         "nbsphinx",
         "pillow",  # required for image scaling in RTD
     ],
 }
```

### Comparing `superscreen-0.9.1/superscreen/__init__.py` & `superscreen-0.9.2/superscreen/__init__.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/about.py` & `superscreen-0.9.2/superscreen/about.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/device/device.py` & `superscreen-0.9.2/superscreen/device/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 from IPython.display import HTML
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 from shapely import geometry as geo
+from tqdm import tqdm
 
 from .. import fem
 from ..geometry import ensure_unique
 from ..units import ureg
 from . import utils
 from .layer import Layer
 from .mesh import Mesh
@@ -427,16 +428,18 @@
             film_terminals = self.terminals.get(name)
             holes = holes_by_layer[film.layer]
             abs_regions = abs_regions_by_layer[film.layer]
             coords = [film.points]
             for poly in holes + abs_regions:
                 if film.contains_points(poly.points).all():
                     coords.append(poly.points)
-            if film_terminals is not None or (
-                buffer_factor[name] is None and buffer[name] is None
+            if (
+                film_terminals is not None
+                or buffer[name] == 0
+                or (buffer_factor[name] is None and buffer[name] is None)
             ):
                 boundary = film.points
             else:
                 boundary = Polygon(points=film.points)
                 if buffer[name] is None:
                     buffer_size = buffer_factor[name] * max(boundary.extents)
                 else:
@@ -561,15 +564,15 @@
         Returns:
             If all_iterations is False, returns a shape ``(n_holes, n_holes)`` mutual
             inductance matrix from the final iteration. Otherwise, returns a list of
             mutual inductance matrices, each with shape ``(n_holes, n_holes)``. The
             length of the list is ``1`` if the device has a single layer, or
             ``iterations + 1`` if the device has multiple layers.
         """
-        from ..solver import solve
+        from ..solver import factorize_model, solve
 
         holes = self.holes
         if hole_polygon_mapping is None:
             from ..fluxoid import make_fluxoid_polygons
 
             hole_polygon_mapping = make_fluxoid_polygons(self)
 
@@ -579,38 +582,48 @@
                 raise ValueError(f"Hole '{hole_name}' does not exist in the device.")
             if not fem.in_polygon(polygon, holes[hole_name].points).all():
                 raise ValueError(
                     f"Hole '{hole_name}' is not completely contained "
                     f"within the given polygon."
                 )
         iterations = solve_kwargs.get("iterations", 1)
+        solve_kwargs["current_units"] = None
         # The magnitude of this current is not important
         I_circ = self.ureg("1 mA")
         if all_iterations:
             n_iter = 1 if len(self.layers) == 1 else iterations + 1
             solution_slice = slice(None)
         else:
             n_iter = 1
             solution_slice = slice(-1, None)
         mutual_inductance = np.zeros((n_iter, n_holes, n_holes))
-        for j, hole_name in enumerate(hole_polygon_mapping):
+        films_by_hole = {}
+        for film, holes in self.holes_by_film().items():
+            for hole in holes:
+                films_by_hole[hole.name] = film
+        model = None
+        for j, hole_name in enumerate(
+            tqdm(hole_polygon_mapping, desc="Holes", disable=n_holes < 2)
+        ):
             logger.info(
                 f"Evaluating {self.name!r} mutual inductance matrix "
                 f"column ({j+1}/{len(hole_polygon_mapping)}), "
                 f"source = {hole_name!r}."
             )
-            solutions = solve(
-                device=self,
-                circulating_currents={hole_name: str(I_circ)},
-                **solve_kwargs,
-            )[solution_slice]
-            films_by_hole = {}
-            for film, holes in self.holes_by_film().items():
-                for hole in holes:
-                    films_by_hole[hole.name] = film
+            if model is None:
+                model = factorize_model(
+                    device=self,
+                    current_units="mA",
+                    circulating_currents={hole_name: str(I_circ)},
+                )
+                I_circ_val = model.circulating_currents[hole_name]
+            else:
+                model.set_circulating_currents({hole_name: I_circ_val})
+            solutions = solve(device=None, model=model, **solve_kwargs)[solution_slice]
+
             for n, solution in enumerate(solutions):
                 logger.info(
                     f"Evaluating fluxoids for solution {n + 1}/{len(solutions)}."
                 )
                 for i, (name, polygon) in enumerate(hole_polygon_mapping.items()):
                     fluxoid = solution.polygon_fluxoid(
                         polygon, film=films_by_hole[name]
```

### Comparing `superscreen-0.9.1/superscreen/device/edge_mesh.py` & `superscreen-0.9.2/superscreen/device/edge_mesh.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/device/layer.py` & `superscreen-0.9.2/superscreen/device/layer.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/device/mesh.py` & `superscreen-0.9.2/superscreen/device/mesh.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/device/polygon.py` & `superscreen-0.9.2/superscreen/device/polygon.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/device/utils.py` & `superscreen-0.9.2/superscreen/device/utils.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/distance.py` & `superscreen-0.9.2/superscreen/distance.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/fem.py` & `superscreen-0.9.2/superscreen/fem.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,37 @@
     adj = adj + adj.T
     adj = (adj > 0).astype(int)
     if sparse:
         return adj
     return adj.toarray()
 
 
+def adj_directed_tri_indices(triangles: np.ndarray, num_sites: int) -> sp.csc_array:
+    """Construct the directed adjacency matrix.
+
+    Each element (i, j) represents an edge in the mesh, and the value at (i, j)
+    is 1 + the index of a triangle containing that edge.
+
+    Args:
+        triangles: The triangle indices, shape ``(m, 3)``
+        num_sites: The number of sites in the mesh
+
+    Returns:
+        A directed adjacency matrix containing triangle indices + 1
+    """
+    t0 = triangles[:, 0]
+    t1 = triangles[:, 1]
+    t2 = triangles[:, 2]
+    i = np.column_stack([t0, t1, t2]).ravel()
+    j = np.column_stack([t1, t2, t0]).ravel()
+    # store triangle index + 1 (zero means no edge connecting i and j)
+    data = np.repeat(np.arange(1, triangles.shape[0] + 1), 3)
+    return sp.csc_array((data, (i, j)), shape=(num_sites, num_sites))
+
+
 def weights_inv_euclidean(
     points: np.ndarray, triangles: np.ndarray, sparse: bool = True
 ) -> Union[np.ndarray, sp.lil_array]:
     """Weights edges by the inverse Euclidean distance of the edge lengths.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices.
@@ -345,36 +368,36 @@
         areas: Shape (m, ) array of triangle areas
 
     Returns:
         x and y gradient matrices, both of which have shape ``(n, n)``
     """
     if areas is None:
         areas = triangle_areas(points, triangles)
-    n = points.shape[0]
+    n = len(points)
     Gx, Gy = gradient_triangles(points, triangles, areas=areas)
-    # Use numpy arrays for fast slicing even though the operators are sparse.
-    Gx = Gx.toarray()
-    Gy = Gy.toarray()
+    Gx = Gx.tolil()
+    Gy = Gy.tolil()
     gx = sp.lil_array((n, n), dtype=float)
     gy = sp.lil_array((n, n), dtype=float)
     # This loop is difficult to vectorize because different vertices
     # have different numbers of adjacent triangles.
+    adj_tri = adj_directed_tri_indices(triangles, n).tolil()
     for i in range(n):
-        adjacent_triangles, _ = np.where(np.isin(triangles, i))
-        t = adjacent_triangles
+        # Triangles adjacent to site i
+        adj = np.array(adj_tri.data[i]) - 1
         # Weight each triangle adjacent to vertex i by its angle at the vertex.
-        vec1 = points[triangles[t, 1]] - points[triangles[t, 0]]
-        vec2 = points[triangles[t, 2]] - points[triangles[t, 0]]
+        vec1 = points[triangles[adj, 1]] - points[triangles[adj, 0]]
+        vec2 = points[triangles[adj, 2]] - points[triangles[adj, 0]]
         weights = np.arccos(
-            np.sum(vec1 * vec2, axis=1)
+            np.einsum("ij, ij -> i", vec1, vec2)
             / (la.norm(vec1, axis=1) * la.norm(vec2, axis=1))
         )
         weights /= weights.sum()
-        gx[i, :] = np.einsum("i, ij -> j", weights, Gx[t, :])
-        gy[i, :] = np.einsum("i, ij -> j", weights, Gy[t, :])
+        gx[i, :] = np.einsum("i, ij -> j", weights, Gx[adj, :].toarray())
+        gy[i, :] = np.einsum("i, ij -> j", weights, Gy[adj, :].toarray())
     return gx.asformat("csr"), gy.asformat("csr")
 
 
 # def gradient_edges(
 #     points: np.ndarray,
 #     edges: np.ndarray,
 #     edge_lengths: np.ndarray,
```

### Comparing `superscreen-0.9.1/superscreen/fluxoid.py` & `superscreen-0.9.2/superscreen/fluxoid.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/geometry.py` & `superscreen-0.9.2/superscreen/geometry.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/io.py` & `superscreen-0.9.2/superscreen/io.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/parameter.py` & `superscreen-0.9.2/superscreen/parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/solution.py` & `superscreen-0.9.2/superscreen/solution.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/solver/solve.py` & `superscreen-0.9.2/superscreen/solver/solve.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,31 +81,34 @@
         film_info: A dict of ``{film_name: FilmInfo}``
         film_systems: A dict of ``{film_name: LinearSystem}``
         hole_systems: A dict of ``{film_name: {hole_name: LinearSystem}}``
         terminal_systems: A dict of ``{film_name: TerminalSystems}``
         terminal_currents: A dict of ``{film_name: {terminal_name: terminal_current}}``
         circulating_currents: A dict of ``{hole_name: circulating_current}``
         vortices: A dict of ``{film_name: vortices}``
+        current_units: str
     """
 
     device: Device
     film_info: Dict[str, FilmInfo]
     film_systems: Dict[str, LinearSystem]
     hole_systems: Dict[str, Dict[str, LinearSystem]]
     terminal_systems: Dict[str, TerminalSystems]
     terminal_currents: Dict[str, Dict[str, float]]
     circulating_currents: Dict[str, float]
     vortices: Dict[str, Sequence[Vortex]]
+    current_units: str
 
     def to_hdf5(self, h5group: h5py.Group) -> None:
         """Save a :class:`superscreen.FactorizedModel` to an :class:`h5py.Group`.
 
         Args:
             h5group: The :class:`h5py.Group` in which to save the model
         """
+        h5group.attrs["current_units"] = self.current_units
         self.device.to_hdf5(h5group.create_group("device"))
         film_info_grp = h5group.create_group("film_info")
         for film, info in self.film_info.items():
             info.to_hdf5(film_info_grp.create_group(film))
         film_systems_grp = h5group.create_group("film_systems")
         for film, system in self.film_systems.items():
             system.to_hdf5(film_systems_grp.create_group(film))
@@ -133,14 +136,15 @@
 
         Args:
             h5group: The :class:`h5py.Group` from which to load the model
 
         Returns:
             The loaded :class:`superscreen.FactorizedModel`
         """
+        current_units = h5group.attrs["current_units"]
         device = Device.from_hdf5(h5group["device"])
         film_info = {
             film: FilmInfo.from_hdf5(grp) for film, grp in h5group["film_info"].items()
         }
         film_systems = {
             film: LinearSystem.from_hdf5(grp)
             for film, grp in h5group["film_systems"].items()
@@ -167,16 +171,39 @@
             film_info=film_info,
             film_systems=film_systems,
             hole_systems=hole_systems,
             terminal_systems=terminal_systems,
             terminal_currents=terminal_currents,
             circulating_currents=circulating_currents,
             vortices=vortices,
+            current_units=current_units,
         )
 
+    def set_circulating_currents(self, circulating_currents: Dict[str, float]) -> None:
+        """Set the circulating currents for the model.
+
+        Args:
+            circulating_currents: A dict of ``{hole_name: current}``, where ``current``
+                is a float in units of ``self.current_units``.
+        """
+        diff = set(circulating_currents) - set(self.device.holes)
+        if diff:
+            raise KeyError(
+                "circulating_currents contains keys not in"
+                f" self.device.holes: {list(diff)!r}"
+            )
+        self.circulating_currents = circulating_currents.copy()
+        holes_by_film = self.device.holes_by_film()
+        for film_name, film_info in self.film_info.items():
+            holes = [hole.name for hole in holes_by_film[film_name]]
+            film_info.circulating_currents = {}
+            for hole, current in self.circulating_currents.items():
+                if hole in holes:
+                    film_info.circulating_currents[hole] = current
+
 
 def factorize_model(
     *,
     device: Device,
     current_units: str,
     terminal_currents: Optional[
         Dict[str, Dict[str, Union[float, str, pint.Quantity]]]
@@ -233,14 +260,15 @@
         film_info,
         film_systems,
         hole_systems,
         terminal_systems,
         terminal_currents,
         circulating_currents,
         vortices,
+        current_units,
     )
 
 
 def solve(
     device: Optional[Device] = None,
     *,
     model: Optional[FactorizedModel] = None,
@@ -312,38 +340,45 @@
         model = factorize_model(
             device=device,
             current_units=current_units,
             terminal_currents=terminal_currents,
             circulating_currents=circulating_currents,
             vortices=vortices,
         )
-    elif (
-        device is not None
-        or terminal_currents is not None
-        or circulating_currents is not None
-        or vortices is not None
-    ):
-        raise ValueError(
-            "If model argument is provided, device, terminal_currents,"
-            " circulating_currents, and vortices must be None."
-        )
+    else:
+        if (
+            device is not None
+            or terminal_currents is not None
+            or circulating_currents is not None
+            or vortices is not None
+        ):
+            raise ValueError(
+                "If model argument is provided, device, terminal_currents,"
+                " circulating_currents, and vortices must be None."
+            )
+        if current_units is not None:
+            logger.warning(
+                "Keyword argument 'current_units' is ignored when"
+                "a factorized model is provided."
+            )
 
     if not isinstance(model, FactorizedModel):
         raise TypeError(
             f"model must be an instance of FactorizedModel (got {type(model)})."
         )
 
     device = model.device
     film_info = model.film_info
     film_systems = model.film_systems
     hole_systems = model.hole_systems
     terminal_systems = model.terminal_systems
     terminal_currents = model.terminal_currents
     circulating_currents = model.circulating_currents
     vortices = model.vortices
+    current_units = model.current_units
 
     if not device.meshes:
         raise ValueError(
             "The device does not have a mesh. Call device.make_mesh() to generate it."
         )
 
     dtype = device.solve_dtype
```

### Comparing `superscreen-0.9.1/superscreen/solver/solve_film.py` & `superscreen-0.9.2/superscreen/solver/solve_film.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         and a dict of ``{film_name: TerminalSystems}``
     """
     film_systems = {}
     hole_systems = {}
     terminal_systems = {}
     for film_name, film_info in film_info_dict.items():
         hole_systems[film_name] = {}
-        film_indices = film_info.film_indices
+        interior_indices = film_info.interior_indices
         boundary_indices = film_info.boundary_indices
         hole_indices = film_info.hole_indices
         Lambda_info = film_info.lambda_info
         inhomogeneous = Lambda_info.inhomogeneous
         Lambda = Lambda_info.Lambda
         terminal_Lambda = 1e10 * np.ones_like(Lambda)
         if inhomogeneous:
@@ -220,15 +220,14 @@
             # Make the boundary linear system
             boundary_system = LinearSystem(
                 A=make_system_1d(boundary_indices, terminal_Lambda),
                 indices=boundary_indices,
                 grad_Lambda_term=grad_Lambda_term,
             )
             # Make the film interior linear system (including holes)
-            interior_indices = np.setdiff1d(film_indices, boundary_indices)
             A = make_system_2d(interior_indices, terminal_Lambda)
             film_without_boundary_system = LinearSystem(
                 A=A,
                 indices=interior_indices,
                 lu_piv=la.lu_factor(-A),
                 grad_Lambda_term=grad_Lambda_term,
             )
@@ -262,15 +261,14 @@
                 film_without_boundary_or_holes=film_without_boundary_or_holes_system,
             )
 
         # Form the linear system for the film:
         # gf = -K @ h, where K = inv(Q * w - Lambda * Del2 - grad_Lambda_term) = inv(A)
         # Eqs. 15-17 in [Brandt], Eqs 12-14 in [Kirtley1], Eqs. 12-14 in [Kirtley2].
         # We want all points that are in a film and not in a hole.
-        interior_indices = film_indices
         if hole_indices:
             interior_indices = np.setdiff1d(
                 interior_indices, np.concatenate(list(hole_indices.values()))
             )
         if film_name in device.terminals:
             interior_indices = np.setdiff1d(interior_indices, boundary_indices)
         A = make_system_2d(interior_indices, Lambda)
```

### Comparing `superscreen-0.9.1/superscreen/solver/utils.py` & `superscreen-0.9.2/superscreen/solver/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,55 +98,56 @@
 
     Args:
         name: The film name
         layer: The layer in which the film exists
         lambda_info: A :class:`superscreen.solver.LambdaInfo` instance defining the
             effective penetration depth in the film
         vortices: Any :class:`superscreen.Vortex` instances located in the film
-        film_indices: The indices of the film in its mesh
+        interior_indices: The indices of the film in its mesh
+        boundary_indices: Indices of the boundary vertices for the mesh,
+            ordered counterclockwise
         hole_indices: A dict containing the indices of each hole in the film's mesh
         in_hole: A boolean array indicated which mesh sites lie inside a hole
         circulating_currents: A dict of ``{hole_name, circulating_current}``
         weights: The mesh weights
         kernel: The mesh self-field kernel :math:`\\mathbf{Q}`
         laplacian: The mesh Laplacian :math:`\\nabla^2`
         gradient: The mesh gradient operator :math:`\\vec{\\nabla}`
         terminal_currents: A dict of ``{terminal_name: terminal_current}``
-        boundary_indices: Indices of the boundary vertices for the mesh,
-            ordered counterclockwise.
     """
 
     name: str
     layer: str
     lambda_info: LambdaInfo
     vortices: Tuple[Vortex]
-    film_indices: np.ndarray
+    interior_indices: np.ndarray
+    boundary_indices: np.ndarray
     hole_indices: Dict[str, np.ndarray]
     in_hole: np.ndarray
     circulating_currents: Dict[str, float]
     weights: np.ndarray
     kernel: np.ndarray
     laplacian: np.ndarray
     gradient: Optional[np.ndarray] = None
     terminal_currents: Optional[Dict[str, float]] = None
-    boundary_indices: Optional[np.ndarray] = None
 
     def to_hdf5(self, h5group: h5py.Group) -> None:
         """Save the :class:`superscreen.solver.FilmInfo` instance to an :class:`h5py.Group`.
 
         Args:
             h5group: The :class:`h5py.Group` in which to save the ``FilmInfo``
         """
         h5group.attrs["name"] = self.name
         h5group.attrs["layer"] = self.layer
         self.lambda_info.to_hdf5(h5group.create_group("lambda_info"))
         vortices_grp = h5group.create_group("vortices")
         for i, vortex in enumerate(self.vortices):
             vortex.to_hdf5(vortices_grp.create_group(str(i)))
-        h5group["film_indices"] = self.film_indices
+        h5group["interior_indices"] = self.interior_indices
+        h5group["boundary_indices"] = self.boundary_indices
         hole_indices_grp = h5group.create_group("hole_indices")
         for hole, indices in self.hole_indices.items():
             hole_indices_grp[hole] = indices
         h5group["in_hole"] = self.in_hole
         circ_grp = h5group.create_group("circulating_currents")
         for hole, current in self.circulating_currents.items():
             circ_grp.attrs[hole] = current
@@ -155,16 +156,14 @@
         h5group["laplacian"] = self.laplacian
         if self.gradient is not None:
             h5group["gradient"] = self.gradient
         if self.terminal_currents is not None:
             term_grp = h5group.create_group("terminal_currents")
             for name, current in self.terminal_currents.items():
                 term_grp.attrs[name] = current
-        if self.boundary_indices is not None:
-            h5group["boundary_indices"] = self.boundary_indices
 
     @staticmethod
     def from_hdf5(h5group: h5py.Group) -> "FilmInfo":
         """Load a :class:`superscreen.solver.FilmInfo` instance from an :class:`h5py.Group`.
 
         Args:
             h5group: The :class:`h5py.Group` from which to load the ``FilmInfo``
@@ -174,45 +173,44 @@
         """
         name = h5group.attrs["name"]
         layer = h5group.attrs["layer"]
         lambda_info = LambdaInfo.from_hdf5(h5group["lambda_info"])
         vortices = []
         for i in sorted(h5group["vortices"], key=int):
             vortices.append(Vortex.from_hdf5(h5group[f"vortices/{i}"]))
-        film_indices = np.array(h5group["film_indices"])
+        interior_indices = np.array(h5group["interior_indices"])
+        boundary_indices = np.array(h5group["boundary_indices"])
         hole_indices = {}
         for hole, indices in h5group["hole_indices"].items():
             hole_indices[hole] = np.array(indices)
         in_hole = np.array(h5group["in_hole"])
         circulating_currents = dict(h5group["circulating_currents"].attrs)
         weights = np.array(h5group["weights"])
         kernel = np.array(h5group["kernel"])
         laplacian = np.array(h5group["laplacian"])
         gradient = terminal_currents = boundary_indices = None
         if "gradient" in h5group:
             gradient = np.array(h5group["gradient"])
         if "terminal_currents" in h5group:
             terminal_currents = dict(h5group["terminal_currents"].attrs)
-        if "boundary_indices" in h5group:
-            boundary_indices = np.array(h5group["boundary_indices"])
         return FilmInfo(
-            name,
-            layer,
-            lambda_info,
-            tuple(vortices),
-            film_indices,
-            hole_indices,
-            in_hole,
-            circulating_currents,
-            weights,
-            kernel,
-            laplacian,
+            name=name,
+            layer=layer,
+            lambda_info=lambda_info,
+            vortices=tuple(vortices),
+            interior_indices=interior_indices,
+            boundary_indices=boundary_indices,
+            hole_indices=hole_indices,
+            in_hole=in_hole,
+            circulating_currents=circulating_currents,
+            weights=weights,
+            kernel=kernel,
+            laplacian=laplacian,
             gradient=gradient,
             terminal_currents=terminal_currents,
-            boundary_indices=boundary_indices,
         )
 
 
 def get_holes_and_vortices_by_film(
     device: Device, vortices: List[Vortex]
 ) -> Tuple[Dict[str, List[Polygon]], Dict[str, List[Vortex]]]:
     vortices_by_film = {film_name: [] for film_name in device.films}
@@ -292,35 +290,39 @@
         Q = mesh.operators.Q.astype(dtype, copy=False)
         laplacian = mesh.operators.laplacian.toarray().astype(dtype, copy=False)
         grad = None
         if lambda_info.inhomogeneous:
             grad_x = mesh.operators.gradient_x.toarray().astype(dtype, copy=False)
             grad_y = mesh.operators.gradient_y.toarray().astype(dtype, copy=False)
             grad = np.array([grad_x, grad_y])
-        boundary_indices = None
         if name in device.terminals:
             boundary_indices = device.boundary_vertices(name)
+        else:
+            boundary_indices = mesh.boundary_indices
+        interior_indices = np.setdiff1d(
+            film.contains_points(mesh.sites, index=True), boundary_indices
+        )
         term_currents = None
         if name in terminal_currents:
             term_currents = terminal_currents[name]
         film_info[name] = FilmInfo(
             name=name,
             layer=layer.name,
             lambda_info=lambda_info,
             vortices=vortices_by_film[name],
-            film_indices=film.contains_points(mesh.sites, index=True),
+            interior_indices=interior_indices,
+            boundary_indices=boundary_indices,
             hole_indices=hole_indices,
             in_hole=in_hole,
             circulating_currents=circ_currents,
             terminal_currents=term_currents,
             weights=weights,
             kernel=Q,
             gradient=grad,
             laplacian=laplacian,
-            boundary_indices=boundary_indices,
         )
     return film_info
 
 
 def current_to_float(
     value: Union[float, str, pint.Quantity], ureg: pint.UnitRegistry, current_units: str
 ):
```

### Comparing `superscreen-0.9.1/superscreen/sources/constant.py` & `superscreen-0.9.2/superscreen/sources/constant.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/sources/current.py` & `superscreen-0.9.2/superscreen/sources/current.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/sources/dipole.py` & `superscreen-0.9.2/superscreen/sources/dipole.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/sources/vortex.py` & `superscreen-0.9.2/superscreen/sources/vortex.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_device.py` & `superscreen-0.9.2/superscreen/test/test_device.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_distance.py` & `superscreen-0.9.2/superscreen/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_parameter.py` & `superscreen-0.9.2/superscreen/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_polygon.py` & `superscreen-0.9.2/superscreen/test/test_polygon.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_solution.py` & `superscreen-0.9.2/superscreen/test/test_solution.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_solve.py` & `superscreen-0.9.2/superscreen/test/test_solve.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_sources.py` & `superscreen-0.9.2/superscreen/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_transport.py` & `superscreen-0.9.2/superscreen/test/test_transport.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/test/test_visualization.py` & `superscreen-0.9.2/superscreen/test/test_visualization.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen/visualization.py` & `superscreen-0.9.2/superscreen/visualization.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.1/superscreen.egg-info/PKG-INFO` & `superscreen-0.9.2/superscreen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.9.1
+Version: 0.9.2
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
```

### Comparing `superscreen-0.9.1/superscreen.egg-info/SOURCES.txt` & `superscreen-0.9.2/superscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

