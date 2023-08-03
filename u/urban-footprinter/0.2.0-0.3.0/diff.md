# Comparing `tmp/urban-footprinter-0.2.0.tar.gz` & `tmp/urban-footprinter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/urban-footprinter-0.2.0.tar", last modified: Wed Mar  4 16:54:22 2020, max compression
+gzip compressed data, was "urban-footprinter-0.3.0.tar", last modified: Thu Aug  3 11:06:36 2023, max compression
```

## Comparing `urban-footprinter-0.2.0.tar` & `urban-footprinter-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-03-04 16:50:21.000000 urban-footprinter-0.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-03-04 16:50:21.000000 urban-footprinter-0.2.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5264 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4013 2020-03-04 16:50:21.000000 urban-footprinter-0.2.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-03-04 16:50:21.000000 urban-footprinter-0.2.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      290 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2020-03-04 16:50:21.000000 urban-footprinter-0.2.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11293 2020-03-04 16:50:21.000000 urban-footprinter-0.2.0/urban_footprinter/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5264 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      299 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-03-04 16:54:22.000000 urban-footprinter-0.2.0/urban_footprinter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:06:36.022682 urban-footprinter-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 11:06:09.000000 urban-footprinter-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-03 11:06:36.022682 urban-footprinter-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-08-03 11:06:09.000000 urban-footprinter-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 11:06:09.000000 urban-footprinter-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 11:06:09.000000 urban-footprinter-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:06:36.022682 urban-footprinter-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:06:36.018682 urban-footprinter-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-08-03 11:06:09.000000 urban-footprinter-0.3.0/tests/test_urban_footprinter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:06:36.018682 urban-footprinter-0.3.0/urban_footprinter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-03 11:06:36.000000 urban-footprinter-0.3.0/urban_footprinter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 11:06:36.000000 urban-footprinter-0.3.0/urban_footprinter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:06:36.000000 urban-footprinter-0.3.0/urban_footprinter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 11:06:36.000000 urban-footprinter-0.3.0/urban_footprinter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:06:36.000000 urban-footprinter-0.3.0/urban_footprinter.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `urban-footprinter-0.2.0/LICENSE` & `urban-footprinter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urban-footprinter-0.2.0/PKG-INFO` & `urban-footprinter-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,98 +1,115 @@
 Metadata-Version: 2.1
 Name: urban-footprinter
-Version: 0.2.0
+Version: 0.3.0
 Summary: A convolution-based approach to detect urban extents.
-Home-page: https://github.com/martibosch/urban-footprinter
-Author: Martí Bosch
-Author-email: marti.bosch@epfl.ch
+Author-email: Martí Bosch <marti.bosch@epfl.ch>
 License: GPL-3.0
-Description: [![PyPI version fury.io](https://badge.fury.io/py/urban-footprinter.svg)](https://pypi.python.org/pypi/urban-footprinter/)
-        [![Build Status](https://travis-ci.org/martibosch/urban-footprinter.svg?branch=master)](https://travis-ci.org/martibosch/urban-footprinter)
-        [![Coverage Status](https://coveralls.io/repos/github/martibosch/urban-footprinter/badge.svg?branch=master)](https://coveralls.io/github/martibosch/urban-footprinter?branch=master)
-        [![GitHub license](https://img.shields.io/github/license/martibosch/urban-footprinter.svg)](https://github.com/martibosch/urban-footprinter/blob/master/LICENSE)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martibosch/urban-footprinter/master?filepath=notebooks/overview.ipynb)
-        
-        Urban footprinter
-        ===============================
-        
-        A reusable convolution-based approach to detect urban extents from raster datasets.
-        
-        LULC | Convolution result | Computed urban extent
-        :-------------------------:|:-------------------------:|:-------------------------:
-        ![LULC](notebooks/figures/zurich-lulc.png) | ![Convolution result](notebooks/figures/zurich-conv-result.png) | ![Urban extent](notebooks/figures/zurich-extent.png)
-        
-        The approach is built upon the methods used in the [Atlas of Urban Expansion](http://atlasofurbanexpansion.org/). The main idea is that a pixel is considered part of the urban extent depending on the proportion of built-up pixels that surround it. See the [notebook overview](https://github.com/martibosch/urban-footprinter/tree/master/notebooks/overview.ipynb) or [this blog post](https://martibosch.github.io/urban-footprinter/) for a more detailed description of the procedure.
-        
-        
-        Installation and usage
-        ----------------------
-        
-        To install use pip:
-        
-            $ pip install urban-footprinter
-        
-        
-        Or clone the repo:
-        
-            $ git clone https://github.com/martibosch/urban-footprinter.git
-            $ python setup.py install
-        
-        Then use it as:
-        
-        ```python
-        import urban_footprinter as ufp
-        
-        # Or use `ufp.urban_footprint_mask_shp` to obtain the urban extent as a 
-        # shapely geometry
-        urban_mask = ufp.urban_footprint_mask("path/to/raster.tif",
-                                              kernel_radius,
-                                              urban_threshold,
-                                              urban_classes=urban_classes)
-        ```
-        
-        where 
-        
-        
-            help(ufp.urban_footprint_mask)
-        
-            Help on function urban_footprint_mask in module urban_footprinter:
-            
-            urban_footprint_mask(raster, kernel_radius, urban_threshold, urban_classes=None, largest_patch_only=True, buffer_dist=None, res=None)
-                Computes a boolean mask of the urban footprint of a given raster.
-                
-                Parameters
-                ----------
-                raster : ndarray or str, file object or pathlib.Path object
-                    Land use/land cover (LULC) raster. If passing a ndarray (instead of the
-                    path to a geotiff), the resolution (in meters) must be passed to the
-                    `res` keyword argument.
-                kernel_radius : numeric
-                    The radius (in meters) of the circular kernel used in the convolution.
-                urban_threshold : float from 0 to 1
-                    Proportion of neighboring (within the kernel) urban pixels after which
-                    a given pixel is considered urban.
-                urban_classes : int or list-like, optional
-                    Code or codes of the LULC classes that must be considered urban. Not
-                    needed if `raster` is already a boolean array of urban/non-urban LULC
-                    classes.
-                largest_patch_only : boolean, default True
-                    Whether the returned urban/non-urban mask should feature only the
-                    largest urban patch.
-                buffer_dist : numeric, optional
-                    Distance to be buffered around the urban/non-urban mask. If no value is
-                    provided, no buffer is applied.
-                res : numeric, optional
-                    Resolution of the `raster` (assumes square pixels). Ignored if `raster`
-                    is a path to a geotiff.
-                
-                Returns
-                -------
-                urban_mask : ndarray
-        
-Platform: UNKNOWN
+Project-URL: Repository, https://github.com/martibosch/urban-footprinter
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: doc
+License-File: LICENSE
+
+[![PyPI version fury.io](https://badge.fury.io/py/urban-footprinter.svg)](https://pypi.python.org/pypi/urban-footprinter/)
+[![Documentation Status](https://readthedocs.org/projects/urban-footprinter/badge/?version=latest)](https://urban-footprinter.readthedocs.io/en/latest/?badge=latest)
+[![CI/CD](https://github.com/martibosch/urban-footprinter/actions/workflows/dev.yml/badge.svg)](https://github.com/martibosch/urban-footprinter/blob/main/.github/workflows/dev.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/martibosch/urban-footprinter/main.svg)](https://results.pre-commit.ci/latest/github/martibosch/urban-footprinter/main)
+[![codecov](https://codecov.io/gh/martibosch/urban-footprinter/branch/main/graph/badge.svg?token=H8PW6I8DY5)](https://codecov.io/gh/martibosch/urban-footprinter)
+[![GitHub license](https://img.shields.io/github/license/martibosch/urban-footprinter.svg)](https://github.com/martibosch/urban-footprinter/blob/main/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martibosch/urban-footprinter/main?filepath=notebooks/overview.ipynb)
+[![DOI](https://zenodo.org/badge/215518909.svg)](https://zenodo.org/badge/latestdoi/215518909)
+
+# Urban footprinter
+
+A reusable convolution-based approach to detect urban extents from raster datasets.
+
+|                    LULC                    |                       Convolution result                        |                Computed urban extent                 |
+| :----------------------------------------: | :-------------------------------------------------------------: | :--------------------------------------------------: |
+| ![LULC](notebooks/figures/zurich-lulc.png) | ![Convolution result](notebooks/figures/zurich-conv-result.png) | ![Urban extent](notebooks/figures/zurich-extent.png) |
+
+The approach is built upon the methods used in the [Atlas of Urban Expansion](http://atlasofurbanexpansion.org/). The main idea is that a pixel is considered part of the urban extent depending on the proportion of built-up pixels that surround it. See the [notebook overview](https://github.com/martibosch/urban-footprinter/tree/main/notebooks/overview.ipynb) or [this blog post](https://martibosch.github.io/urban-footprinter/) for a more detailed description of the procedure.
+
+**Citation**: Bosch M. 2020. "Urban footprinter: a convolution-based approach to detect urban extents from raster data". Available from [https://github.com/martibosch/urban-footprinter](https://github.com/martibosch/urban-footprinter). Accessed: DD Month YYYY.
+
+An example BibTeX entry is:
+
+```bibtex
+@misc{bosch2020urban,
+  title={Urban footprinter: a convolution-based approach to detect urban extents from raster data},
+  author={Bosch, Mart\'{i}},
+  year={2020},
+  doi={10.5281/zenodo.3699310},
+  howpublished={Available from \url{https://github.com/martibosch/urban-footprinter}. Accessed: DD Month YYYY},
+}
+```
+
+## Installation and usage
+
+To install use pip:
+
+```
+$ pip install urban-footprinter
+```
+
+Then use it as:
+
+```python
+import urban_footprinter as ufp
+
+# Or use `ufp.urban_footprint_mask_shp` to obtain the urban extent as a
+# shapely geometry
+urban_mask = ufp.urban_footprint_mask(
+    "path/to/raster.tif", kernel_radius, urban_threshold, urban_classes=urban_classes
+)
+```
+
+where
+
+```
+help(ufp.urban_footprint_mask)
+
+Help on function urban_footprint_mask in module urban_footprinter:
+
+urban_footprint_mask(raster, kernel_radius, urban_threshold, urban_classes=None, num_patches=1,
+                     buffer_dist=None, res=None)
+    Computes a boolean mask of the urban footprint of a given raster.
+
+    Parameters
+    ----------
+    raster : ndarray or str, file object or pathlib.Path object
+        Land use/land cover (LULC) raster. If passing a ndarray (instead of the
+        path to a geotiff), the resolution (in meters) must be passed to the
+        `res` keyword argument.
+    kernel_radius : numeric
+        The radius (in meters) of the circular kernel used in the convolution.
+    urban_threshold : float from 0 to 1
+        Proportion of neighboring (within the kernel) urban pixels after which
+        a given pixel is considered urban.
+    urban_classes : int or list-like, optional
+        Code or codes of the LULC classes that must be considered urban. Not
+        needed if `raster` is already a boolean array of urban/non-urban LULC
+        classes.
+    num_patches : int, default 1
+        The number of urban patches that should be featured in the returned
+        urban/non-urban mask. If `None` or a value lower than one is provided,
+        the returned urban/non-urban mask will featuer all the urban patches.
+    buffer_dist : numeric, optional
+        Distance to be buffered around the urban/non-urban mask. If no value is
+        provided, no buffer is applied.
+    res : numeric, optional
+        Resolution of the `raster` (assumes square pixels). Ignored if `raster`
+        is a path to a geotiff.
+
+    Returns
+    -------
+    urban_mask : ndarray
+```
```

### Comparing `urban-footprinter-0.2.0/README.md` & `urban-footprinter-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,94 @@
 [![PyPI version fury.io](https://badge.fury.io/py/urban-footprinter.svg)](https://pypi.python.org/pypi/urban-footprinter/)
-[![Build Status](https://travis-ci.org/martibosch/urban-footprinter.svg?branch=master)](https://travis-ci.org/martibosch/urban-footprinter)
-[![Coverage Status](https://coveralls.io/repos/github/martibosch/urban-footprinter/badge.svg?branch=master)](https://coveralls.io/github/martibosch/urban-footprinter?branch=master)
-[![GitHub license](https://img.shields.io/github/license/martibosch/urban-footprinter.svg)](https://github.com/martibosch/urban-footprinter/blob/master/LICENSE)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martibosch/urban-footprinter/master?filepath=notebooks/overview.ipynb)
+[![Documentation Status](https://readthedocs.org/projects/urban-footprinter/badge/?version=latest)](https://urban-footprinter.readthedocs.io/en/latest/?badge=latest)
+[![CI/CD](https://github.com/martibosch/urban-footprinter/actions/workflows/dev.yml/badge.svg)](https://github.com/martibosch/urban-footprinter/blob/main/.github/workflows/dev.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/martibosch/urban-footprinter/main.svg)](https://results.pre-commit.ci/latest/github/martibosch/urban-footprinter/main)
+[![codecov](https://codecov.io/gh/martibosch/urban-footprinter/branch/main/graph/badge.svg?token=H8PW6I8DY5)](https://codecov.io/gh/martibosch/urban-footprinter)
+[![GitHub license](https://img.shields.io/github/license/martibosch/urban-footprinter.svg)](https://github.com/martibosch/urban-footprinter/blob/main/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martibosch/urban-footprinter/main?filepath=notebooks/overview.ipynb)
+[![DOI](https://zenodo.org/badge/215518909.svg)](https://zenodo.org/badge/latestdoi/215518909)
 
-Urban footprinter
-===============================
+# Urban footprinter
 
 A reusable convolution-based approach to detect urban extents from raster datasets.
 
-LULC | Convolution result | Computed urban extent
-:-------------------------:|:-------------------------:|:-------------------------:
-![LULC](notebooks/figures/zurich-lulc.png) | ![Convolution result](notebooks/figures/zurich-conv-result.png) | ![Urban extent](notebooks/figures/zurich-extent.png)
-
-The approach is built upon the methods used in the [Atlas of Urban Expansion](http://atlasofurbanexpansion.org/). The main idea is that a pixel is considered part of the urban extent depending on the proportion of built-up pixels that surround it. See the [notebook overview](https://github.com/martibosch/urban-footprinter/tree/master/notebooks/overview.ipynb) or [this blog post](https://martibosch.github.io/urban-footprinter/) for a more detailed description of the procedure.
-
+|                    LULC                    |                       Convolution result                        |                Computed urban extent                 |
+| :----------------------------------------: | :-------------------------------------------------------------: | :--------------------------------------------------: |
+| ![LULC](notebooks/figures/zurich-lulc.png) | ![Convolution result](notebooks/figures/zurich-conv-result.png) | ![Urban extent](notebooks/figures/zurich-extent.png) |
+
+The approach is built upon the methods used in the [Atlas of Urban Expansion](http://atlasofurbanexpansion.org/). The main idea is that a pixel is considered part of the urban extent depending on the proportion of built-up pixels that surround it. See the [notebook overview](https://github.com/martibosch/urban-footprinter/tree/main/notebooks/overview.ipynb) or [this blog post](https://martibosch.github.io/urban-footprinter/) for a more detailed description of the procedure.
+
+**Citation**: Bosch M. 2020. "Urban footprinter: a convolution-based approach to detect urban extents from raster data". Available from [https://github.com/martibosch/urban-footprinter](https://github.com/martibosch/urban-footprinter). Accessed: DD Month YYYY.
+
+An example BibTeX entry is:
+
+```bibtex
+@misc{bosch2020urban,
+  title={Urban footprinter: a convolution-based approach to detect urban extents from raster data},
+  author={Bosch, Mart\'{i}},
+  year={2020},
+  doi={10.5281/zenodo.3699310},
+  howpublished={Available from \url{https://github.com/martibosch/urban-footprinter}. Accessed: DD Month YYYY},
+}
+```
 
-Installation and usage
-----------------------
+## Installation and usage
 
 To install use pip:
 
-    $ pip install urban-footprinter
-
-
-Or clone the repo:
-
-    $ git clone https://github.com/martibosch/urban-footprinter.git
-    $ python setup.py install
+```
+$ pip install urban-footprinter
+```
 
 Then use it as:
 
 ```python
 import urban_footprinter as ufp
 
-# Or use `ufp.urban_footprint_mask_shp` to obtain the urban extent as a 
+# Or use `ufp.urban_footprint_mask_shp` to obtain the urban extent as a
 # shapely geometry
-urban_mask = ufp.urban_footprint_mask("path/to/raster.tif",
-                                      kernel_radius,
-                                      urban_threshold,
-                                      urban_classes=urban_classes)
-```
-
-where 
-
-
-    help(ufp.urban_footprint_mask)
-
-    Help on function urban_footprint_mask in module urban_footprinter:
-    
-    urban_footprint_mask(raster, kernel_radius, urban_threshold, urban_classes=None, largest_patch_only=True, buffer_dist=None, res=None)
-        Computes a boolean mask of the urban footprint of a given raster.
-        
-        Parameters
-        ----------
-        raster : ndarray or str, file object or pathlib.Path object
-            Land use/land cover (LULC) raster. If passing a ndarray (instead of the
-            path to a geotiff), the resolution (in meters) must be passed to the
-            `res` keyword argument.
-        kernel_radius : numeric
-            The radius (in meters) of the circular kernel used in the convolution.
-        urban_threshold : float from 0 to 1
-            Proportion of neighboring (within the kernel) urban pixels after which
-            a given pixel is considered urban.
-        urban_classes : int or list-like, optional
-            Code or codes of the LULC classes that must be considered urban. Not
-            needed if `raster` is already a boolean array of urban/non-urban LULC
-            classes.
-        largest_patch_only : boolean, default True
-            Whether the returned urban/non-urban mask should feature only the
-            largest urban patch.
-        buffer_dist : numeric, optional
-            Distance to be buffered around the urban/non-urban mask. If no value is
-            provided, no buffer is applied.
-        res : numeric, optional
-            Resolution of the `raster` (assumes square pixels). Ignored if `raster`
-            is a path to a geotiff.
-        
-        Returns
-        -------
-        urban_mask : ndarray
+urban_mask = ufp.urban_footprint_mask(
+    "path/to/raster.tif", kernel_radius, urban_threshold, urban_classes=urban_classes
+)
+```
+
+where
+
+```
+help(ufp.urban_footprint_mask)
+
+Help on function urban_footprint_mask in module urban_footprinter:
+
+urban_footprint_mask(raster, kernel_radius, urban_threshold, urban_classes=None, num_patches=1,
+                     buffer_dist=None, res=None)
+    Computes a boolean mask of the urban footprint of a given raster.
+
+    Parameters
+    ----------
+    raster : ndarray or str, file object or pathlib.Path object
+        Land use/land cover (LULC) raster. If passing a ndarray (instead of the
+        path to a geotiff), the resolution (in meters) must be passed to the
+        `res` keyword argument.
+    kernel_radius : numeric
+        The radius (in meters) of the circular kernel used in the convolution.
+    urban_threshold : float from 0 to 1
+        Proportion of neighboring (within the kernel) urban pixels after which
+        a given pixel is considered urban.
+    urban_classes : int or list-like, optional
+        Code or codes of the LULC classes that must be considered urban. Not
+        needed if `raster` is already a boolean array of urban/non-urban LULC
+        classes.
+    num_patches : int, default 1
+        The number of urban patches that should be featured in the returned
+        urban/non-urban mask. If `None` or a value lower than one is provided,
+        the returned urban/non-urban mask will featuer all the urban patches.
+    buffer_dist : numeric, optional
+        Distance to be buffered around the urban/non-urban mask. If no value is
+        provided, no buffer is applied.
+    res : numeric, optional
+        Resolution of the `raster` (assumes square pixels). Ignored if `raster`
+        is a path to a geotiff.
+
+    Returns
+    -------
+    urban_mask : ndarray
+```
```

### Comparing `urban-footprinter-0.2.0/urban_footprinter.egg-info/PKG-INFO` & `urban-footprinter-0.3.0/urban_footprinter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,98 +1,115 @@
 Metadata-Version: 2.1
 Name: urban-footprinter
-Version: 0.2.0
+Version: 0.3.0
 Summary: A convolution-based approach to detect urban extents.
-Home-page: https://github.com/martibosch/urban-footprinter
-Author: Martí Bosch
-Author-email: marti.bosch@epfl.ch
+Author-email: Martí Bosch <marti.bosch@epfl.ch>
 License: GPL-3.0
-Description: [![PyPI version fury.io](https://badge.fury.io/py/urban-footprinter.svg)](https://pypi.python.org/pypi/urban-footprinter/)
-        [![Build Status](https://travis-ci.org/martibosch/urban-footprinter.svg?branch=master)](https://travis-ci.org/martibosch/urban-footprinter)
-        [![Coverage Status](https://coveralls.io/repos/github/martibosch/urban-footprinter/badge.svg?branch=master)](https://coveralls.io/github/martibosch/urban-footprinter?branch=master)
-        [![GitHub license](https://img.shields.io/github/license/martibosch/urban-footprinter.svg)](https://github.com/martibosch/urban-footprinter/blob/master/LICENSE)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martibosch/urban-footprinter/master?filepath=notebooks/overview.ipynb)
-        
-        Urban footprinter
-        ===============================
-        
-        A reusable convolution-based approach to detect urban extents from raster datasets.
-        
-        LULC | Convolution result | Computed urban extent
-        :-------------------------:|:-------------------------:|:-------------------------:
-        ![LULC](notebooks/figures/zurich-lulc.png) | ![Convolution result](notebooks/figures/zurich-conv-result.png) | ![Urban extent](notebooks/figures/zurich-extent.png)
-        
-        The approach is built upon the methods used in the [Atlas of Urban Expansion](http://atlasofurbanexpansion.org/). The main idea is that a pixel is considered part of the urban extent depending on the proportion of built-up pixels that surround it. See the [notebook overview](https://github.com/martibosch/urban-footprinter/tree/master/notebooks/overview.ipynb) or [this blog post](https://martibosch.github.io/urban-footprinter/) for a more detailed description of the procedure.
-        
-        
-        Installation and usage
-        ----------------------
-        
-        To install use pip:
-        
-            $ pip install urban-footprinter
-        
-        
-        Or clone the repo:
-        
-            $ git clone https://github.com/martibosch/urban-footprinter.git
-            $ python setup.py install
-        
-        Then use it as:
-        
-        ```python
-        import urban_footprinter as ufp
-        
-        # Or use `ufp.urban_footprint_mask_shp` to obtain the urban extent as a 
-        # shapely geometry
-        urban_mask = ufp.urban_footprint_mask("path/to/raster.tif",
-                                              kernel_radius,
-                                              urban_threshold,
-                                              urban_classes=urban_classes)
-        ```
-        
-        where 
-        
-        
-            help(ufp.urban_footprint_mask)
-        
-            Help on function urban_footprint_mask in module urban_footprinter:
-            
-            urban_footprint_mask(raster, kernel_radius, urban_threshold, urban_classes=None, largest_patch_only=True, buffer_dist=None, res=None)
-                Computes a boolean mask of the urban footprint of a given raster.
-                
-                Parameters
-                ----------
-                raster : ndarray or str, file object or pathlib.Path object
-                    Land use/land cover (LULC) raster. If passing a ndarray (instead of the
-                    path to a geotiff), the resolution (in meters) must be passed to the
-                    `res` keyword argument.
-                kernel_radius : numeric
-                    The radius (in meters) of the circular kernel used in the convolution.
-                urban_threshold : float from 0 to 1
-                    Proportion of neighboring (within the kernel) urban pixels after which
-                    a given pixel is considered urban.
-                urban_classes : int or list-like, optional
-                    Code or codes of the LULC classes that must be considered urban. Not
-                    needed if `raster` is already a boolean array of urban/non-urban LULC
-                    classes.
-                largest_patch_only : boolean, default True
-                    Whether the returned urban/non-urban mask should feature only the
-                    largest urban patch.
-                buffer_dist : numeric, optional
-                    Distance to be buffered around the urban/non-urban mask. If no value is
-                    provided, no buffer is applied.
-                res : numeric, optional
-                    Resolution of the `raster` (assumes square pixels). Ignored if `raster`
-                    is a path to a geotiff.
-                
-                Returns
-                -------
-                urban_mask : ndarray
-        
-Platform: UNKNOWN
+Project-URL: Repository, https://github.com/martibosch/urban-footprinter
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: doc
+License-File: LICENSE
+
+[![PyPI version fury.io](https://badge.fury.io/py/urban-footprinter.svg)](https://pypi.python.org/pypi/urban-footprinter/)
+[![Documentation Status](https://readthedocs.org/projects/urban-footprinter/badge/?version=latest)](https://urban-footprinter.readthedocs.io/en/latest/?badge=latest)
+[![CI/CD](https://github.com/martibosch/urban-footprinter/actions/workflows/dev.yml/badge.svg)](https://github.com/martibosch/urban-footprinter/blob/main/.github/workflows/dev.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/martibosch/urban-footprinter/main.svg)](https://results.pre-commit.ci/latest/github/martibosch/urban-footprinter/main)
+[![codecov](https://codecov.io/gh/martibosch/urban-footprinter/branch/main/graph/badge.svg?token=H8PW6I8DY5)](https://codecov.io/gh/martibosch/urban-footprinter)
+[![GitHub license](https://img.shields.io/github/license/martibosch/urban-footprinter.svg)](https://github.com/martibosch/urban-footprinter/blob/main/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martibosch/urban-footprinter/main?filepath=notebooks/overview.ipynb)
+[![DOI](https://zenodo.org/badge/215518909.svg)](https://zenodo.org/badge/latestdoi/215518909)
+
+# Urban footprinter
+
+A reusable convolution-based approach to detect urban extents from raster datasets.
+
+|                    LULC                    |                       Convolution result                        |                Computed urban extent                 |
+| :----------------------------------------: | :-------------------------------------------------------------: | :--------------------------------------------------: |
+| ![LULC](notebooks/figures/zurich-lulc.png) | ![Convolution result](notebooks/figures/zurich-conv-result.png) | ![Urban extent](notebooks/figures/zurich-extent.png) |
+
+The approach is built upon the methods used in the [Atlas of Urban Expansion](http://atlasofurbanexpansion.org/). The main idea is that a pixel is considered part of the urban extent depending on the proportion of built-up pixels that surround it. See the [notebook overview](https://github.com/martibosch/urban-footprinter/tree/main/notebooks/overview.ipynb) or [this blog post](https://martibosch.github.io/urban-footprinter/) for a more detailed description of the procedure.
+
+**Citation**: Bosch M. 2020. "Urban footprinter: a convolution-based approach to detect urban extents from raster data". Available from [https://github.com/martibosch/urban-footprinter](https://github.com/martibosch/urban-footprinter). Accessed: DD Month YYYY.
+
+An example BibTeX entry is:
+
+```bibtex
+@misc{bosch2020urban,
+  title={Urban footprinter: a convolution-based approach to detect urban extents from raster data},
+  author={Bosch, Mart\'{i}},
+  year={2020},
+  doi={10.5281/zenodo.3699310},
+  howpublished={Available from \url{https://github.com/martibosch/urban-footprinter}. Accessed: DD Month YYYY},
+}
+```
+
+## Installation and usage
+
+To install use pip:
+
+```
+$ pip install urban-footprinter
+```
+
+Then use it as:
+
+```python
+import urban_footprinter as ufp
+
+# Or use `ufp.urban_footprint_mask_shp` to obtain the urban extent as a
+# shapely geometry
+urban_mask = ufp.urban_footprint_mask(
+    "path/to/raster.tif", kernel_radius, urban_threshold, urban_classes=urban_classes
+)
+```
+
+where
+
+```
+help(ufp.urban_footprint_mask)
+
+Help on function urban_footprint_mask in module urban_footprinter:
+
+urban_footprint_mask(raster, kernel_radius, urban_threshold, urban_classes=None, num_patches=1,
+                     buffer_dist=None, res=None)
+    Computes a boolean mask of the urban footprint of a given raster.
+
+    Parameters
+    ----------
+    raster : ndarray or str, file object or pathlib.Path object
+        Land use/land cover (LULC) raster. If passing a ndarray (instead of the
+        path to a geotiff), the resolution (in meters) must be passed to the
+        `res` keyword argument.
+    kernel_radius : numeric
+        The radius (in meters) of the circular kernel used in the convolution.
+    urban_threshold : float from 0 to 1
+        Proportion of neighboring (within the kernel) urban pixels after which
+        a given pixel is considered urban.
+    urban_classes : int or list-like, optional
+        Code or codes of the LULC classes that must be considered urban. Not
+        needed if `raster` is already a boolean array of urban/non-urban LULC
+        classes.
+    num_patches : int, default 1
+        The number of urban patches that should be featured in the returned
+        urban/non-urban mask. If `None` or a value lower than one is provided,
+        the returned urban/non-urban mask will featuer all the urban patches.
+    buffer_dist : numeric, optional
+        Distance to be buffered around the urban/non-urban mask. If no value is
+        provided, no buffer is applied.
+    res : numeric, optional
+        Resolution of the `raster` (assumes square pixels). Ignored if `raster`
+        is a path to a geotiff.
+
+    Returns
+    -------
+    urban_mask : ndarray
+```
```

