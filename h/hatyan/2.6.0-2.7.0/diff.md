# Comparing `tmp/hatyan-2.6.0.tar.gz` & `tmp/hatyan-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatyan-2.6.0.tar", last modified: Wed Feb 15 14:43:39 2023, max compression
+gzip compressed data, was "hatyan-2.7.0.tar", last modified: Thu Aug  3 10:48:34 2023, max compression
```

## Comparing `hatyan-2.6.0.tar` & `hatyan-2.7.0.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 14:43:39.719034 hatyan-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2023-02-15 14:43:29.000000 hatyan-2.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    19938 2023-02-15 14:43:29.000000 hatyan-2.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-02-15 14:43:29.000000 hatyan-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3701 2023-02-15 14:43:39.719034 hatyan-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-02-15 14:43:29.000000 hatyan-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 14:43:39.719034 hatyan-2.6.0/hatyan/
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30779 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/analysis_prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)    57251 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/astrog.py
--rw-r--r--   0 runner    (1001) docker     (122)    10775 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 14:43:39.719034 hatyan-2.6.0/hatyan/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/data_M2phasediff_perstation.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/data_foreman_frequencies.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/data_foreman_harmonic.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/data_foreman_shallowrelations.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10407 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/data_schureman_harmonic.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6918 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/data_schureman_shallowrelations.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10666 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/data/leap-seconds.list
--rw-r--r--   0 runner    (1001) docker     (122)    19158 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/foreman.py
--rw-r--r--   0 runner    (1001) docker     (122)    25385 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/getonlinedata.py
--rw-r--r--   0 runner    (1001) docker     (122)    26586 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/hatyan_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     7360 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/kw_gemgetij.py
--rw-r--r--   0 runner    (1001) docker     (122)     9960 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/kw_havengetallen.py
--rw-r--r--   0 runner    (1001) docker     (122)    18245 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/kw_overschrijding.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/kw_slotgemiddelden.py
--rw-r--r--   0 runner    (1001) docker     (122)    17662 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/schureman.py
--rw-r--r--   0 runner    (1001) docker     (122)    86970 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     6547 2023-02-15 14:43:30.000000 hatyan-2.6.0/hatyan/wrapper_RWS.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 14:43:39.719034 hatyan-2.6.0/hatyan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3701 2023-02-15 14:43:39.000000 hatyan-2.6.0/hatyan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-02-15 14:43:39.000000 hatyan-2.6.0/hatyan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-15 14:43:39.000000 hatyan-2.6.0/hatyan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-15 14:43:39.000000 hatyan-2.6.0/hatyan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-15 14:43:39.000000 hatyan-2.6.0/hatyan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-02-15 14:43:39.000000 hatyan-2.6.0/hatyan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-02-15 14:43:30.000000 hatyan-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-02-15 14:43:30.000000 hatyan-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-02-15 14:43:39.719034 hatyan-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-15 14:43:30.000000 hatyan-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 14:43:39.719034 hatyan-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 14:43:30.000000 hatyan-2.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-02-15 14:43:30.000000 hatyan-2.6.0/tests/test_astrog_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-02-15 14:43:30.000000 hatyan-2.6.0/tests/test_hatyan_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)    56813 2023-02-15 14:43:30.000000 hatyan-2.6.0/tests/test_hatyan_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.814918 hatyan-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-03 10:48:16.000000 hatyan-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-08-03 10:48:34.814918 hatyan-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-08-03 10:48:16.000000 hatyan-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.810918 hatyan-2.7.0/hatyan/
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30963 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/analysis_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57251 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/astrog.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10775 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.810918 hatyan-2.7.0/hatyan/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_M2phasediff_perstation.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_foreman_frequencies.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_foreman_harmonic.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_foreman_shallowrelations.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10407 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_schureman_harmonic.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6918 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_schureman_shallowrelations.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10666 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/leap-seconds.list
+-rw-r--r--   0 runner    (1001) docker     (122)    19158 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25385 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/getonlinedata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26586 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/hatyan_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7360 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_gemgetij.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9960 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_havengetallen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18245 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_overschrijding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_slotgemiddelden.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17662 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/schureman.py
+-rw-r--r--   0 runner    (1001) docker     (122)    87281 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6547 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/wrapper_RWS.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.810918 hatyan-2.7.0/hatyan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-08-03 10:48:16.000000 hatyan-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-03 10:48:16.000000 hatyan-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-08-03 10:48:34.814918 hatyan-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-03 10:48:16.000000 hatyan-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.814918 hatyan-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/test_astrog_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/test_hatyan_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60311 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/test_hatyan_main.py
```

### Comparing `hatyan-2.6.0/PKG-INFO` & `hatyan-2.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 Metadata-Version: 2.1
 Name: hatyan
-Version: 2.6.0
+Version: 2.7.0
 Summary: hatyan is a tidal analysis and prediction tool of Rijkswaterstaat
 Home-page: https://github.com/Deltares/hatyan
 Author: Jelmer Veenstra
 Author-email: Jelmer.Veenstra@Deltares.nl
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: hatyan,tidal analysis,tidal prediction
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
 
-[![generate-documentation](https://github.com/Deltares/hatyan/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/hatyan/actions/workflows/generate-documentation.yml)
+[![codecov](https://img.shields.io/codecov/c/github/deltares/hatyan.svg?style=flat-square)](https://app.codecov.io/gh/deltares/hatyan)
 [![pytest-hmcenv](https://github.com/Deltares/hatyan/actions/workflows/pytest-hmcenv.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-devenv.yml)
+[![pytest-py38](https://github.com/Deltares/hatyan/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/hatyan/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py39.yml)
+[![pytest-py310](https://github.com/Deltares/hatyan/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py310.yml)
+[![pytest-py311](https://github.com/Deltares/hatyan/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py311.yml)
 [![sigrid-publish](https://github.com/Deltares/hatyan/actions/workflows/sigrid-publish.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/sigrid-publish.yml)
 [![pypi-upload](https://github.com/Deltares/hatyan/actions/workflows/pypi-upload.yml/badge.svg?event=release)](https://github.com/Deltares/hatyan/actions/workflows/pypi-upload.yml)
+[![Supported versions](https://img.shields.io/pypi/pyversions/hatyan.svg)](https://pypi.org/project/hatyan)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_hatyan&metric=alert_status)](https://sonarcloud.io/dashboard?id=Deltares_hatyan)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD)
-
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD?urlpath=/tree/docs/notebooks)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6885342.svg)](https://doi.org/10.5281/zenodo.6885342)
 
 # hatyan
 
 A Python package for harmonic tidal analysis and prediction, based on the FORTRAN version and developed for Rijkswaterstaat. Hatyan contains the methods to derive water level extremes (high and low waters) and several other water level indicators (Kenmerkende Waarden). Furthermore, hatyan provides easier access to Rijkswaterstaat data via their data distribution layer (DataDistributieLaag, DDL).
 
+## Information
 
-Information and examples
---------
+- install with ``pip install hatyan -U``
+- [online documentation](https://deltares.github.io/hatyan) with contributing guide, tutorials/examples, API reference and a convenient search box.
 - [docs folder](https://github.com/Deltares/hatyan/tree/main/docs) with background information
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/hatyan/blob/main/docs/hatyan/index.html) generated from docstrings (replace 'main' in the url with any tagname to view older versions)
-- [jupyter notebooks](https://github.com/Deltares/hatyan/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/hatyan/tree/main/tests/examples) with more example scripts
-
-
-Installation
---------
-
-- optional: download and install Anaconda 64 bit Python 3.8 (or higher) from https://www.anaconda.com/distribution/#download-section
-- open anaconda prompt
-- optional: ``conda create --name hatyan_env -c conda-forge python=3.8 git spyder -y`` (or higher python version)
-- optional: ``conda activate hatyan_env``
-- ``python -m pip install hatyan`` (this installs hatyan and all required packages from PyPI, add a version like ``==2.3.0`` if you require a specific version. Optionally add ``--upgrade``)
-- alternatively: ``python -m pip install git+https://github.com/Deltares/hatyan`` (this installs hatyan and all required packages from github, add a tag like ``@v2.3.0`` if you require a specific release/branch.)
+- Bug or feature request? Create a [GitHub issue](https://github.com/Deltares/dfm_tools/issues)
```

### Comparing `hatyan-2.6.0/hatyan/__init__.py` & `hatyan-2.7.0/hatyan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 .. include:: ../README.md
 """
 
 __author__ = """Jelmer Veenstra"""
 __email__ = 'jelmer.veenstra@deltares.nl'
-__version__ = '2.6.0'
+__version__ = '2.7.0'
 
 from hatyan.analysis_prediction import *
 from hatyan.astrog import *
 from hatyan.components import *
 from hatyan.hatyan_core import *
 from hatyan.foreman import *
 from hatyan.schureman import *
```

### Comparing `hatyan-2.6.0/hatyan/analysis_prediction.py` & `hatyan-2.7.0/hatyan/analysis_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         raise Exception('both arguments hatyan_settings and other settings (e.g. nodalfactors) are provided, this is not valid')
         
     #create sorted and complete component list
     const_list_inclCS_raw = comp.index.tolist() + hatyan_settings.CS_comps['CS_comps_derive'].tolist()
     const_list_inclCS = sort_const_list(const_list=const_list_inclCS_raw)
 
     #retrieve freq and speed
-    t_const_freq_pd, CS_v_0i_rad = get_freqv0_generic(hatyan_settings, const_list=const_list_inclCS, dood_date_mid=dood_date_mid, dood_date_start=dood_date_mid) # with split_components, v0 is calculated on the same timestep as u and f (middle of original series)
+    _, CS_v_0i_rad = get_freqv0_generic(hatyan_settings, const_list=const_list_inclCS, dood_date_mid=dood_date_mid, dood_date_start=dood_date_mid) # with split_components, v0 is calculated on the same timestep as u and f (middle of original series)
     CS_u_i_rad, CS_f_i = get_uf_generic(hatyan_settings, const_list=const_list_inclCS, dood_date_fu=dood_date_mid)
     
     comp_inclCS = pd.DataFrame(comp,index=const_list_inclCS,columns=comp.columns)
     #comp_inclCS_preCS = comp_inclCS.copy()
         
     for comp_main in np.unique(hatyan_settings.CS_comps['CS_comps_from']):
         bool_CS_maincomp = hatyan_settings.CS_comps['CS_comps_from'] == comp_main #boolean of which rows of CS_comps dataframe corresponds to a main constituent, also makes it possible to select two rows
@@ -528,21 +528,22 @@
     else:
         dood_date_fu = dood_date_mid
     u_i_rad, f_i = get_uf_generic(hatyan_settings, const_list, dood_date_fu)
 
     print('PREDICTION started')
     omega_i_rads = t_const_speed_all.T/3600 #angular frequency, 2pi/T, in rad/s, https://en.wikipedia.org/wiki/Angular_frequency (2*np.pi)/(1/x*3600) = 2*np.pi*x/3600
     if not isinstance(times_pred_all_pdDTI,pd.DatetimeIndex): #support for years<1677, have to use Index instead of DatetimeIndex (DatetimeIndex is also Index, so isinstance(times_pred_all_pdDTI,pd.Index) does not work
-        times_from0allpred_s_orig = (times_pred_all_pdDTI-dood_date_start).total_seconds().values
+        tdiff = pd.TimedeltaIndex(times_pred_all_pdDTI-dood_date_start) #pd.TimedeltaIndex is around it to avoid it being an Index in case of outofbounds timesteps (necessary from pandas 2.0.0)
     else:
-        times_from0allpred_s_orig = (times_pred_all_pdDTI-dood_date_start[0]).total_seconds().values
+        tdiff = pd.TimedeltaIndex(times_pred_all_pdDTI-dood_date_start[0]) #pd.TimedeltaIndex is not necessary here, but for conformity with above
+    times_from0allpred_s_orig = tdiff.total_seconds().values
     times_from0allpred_s = np.transpose(times_from0allpred_s_orig[np.newaxis])
     
     f_A = np.multiply(f_i.values,A)
-    omeg_t = np.multiply(times_from0allpred_s,omega_i_rads)#_td)
+    omeg_t = np.multiply(times_from0allpred_s,omega_i_rads)
     v_u_phi = np.subtract(np.add(v_0i_rad.values,u_i_rad.values),phi_rad)
     omeg_t_v_u_phi = np.add(omeg_t,v_u_phi)
     ht_res = np.sum(np.multiply(f_A,np.cos(omeg_t_v_u_phi)),axis=1) #not necessary to add A0, since it is already part of the component list
     
     ts_prediction_pd = pd.DataFrame({'values': ht_res},index=times_pred_all_pdDTI)
     print('PREDICTION finished')
```

### Comparing `hatyan-2.6.0/hatyan/astrog.py` & `hatyan-2.7.0/hatyan/astrog.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/components.py` & `hatyan-2.7.0/hatyan/components.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/convert.py` & `hatyan-2.7.0/hatyan/convert.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/data/data_M2phasediff_perstation.txt` & `hatyan-2.7.0/hatyan/data/data_M2phasediff_perstation.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/data/data_foreman_frequencies.txt` & `hatyan-2.7.0/hatyan/data/data_foreman_frequencies.txt`

 * *Files 6% similar despite different names*

```diff
@@ -142,8 +142,11 @@
 ST31 0.4069168759
 ST32 0.4082008687
 ST33 0.4471596822
 M12 0.4830684040
 ST34 0.4858903367
 ST35 0.4874282766
 ########## ADDED FROM R-TABLE #########
-M1C 0.04025583333333334
+M1C 0.04025583333333334
+########## added from hatyan.get_schureman_freqs() #########
+MSQM 0.00587202
+M1 0.04026859
```

### Comparing `hatyan-2.6.0/hatyan/data/data_foreman_harmonic.txt` & `hatyan-2.7.0/hatyan/data/data_foreman_harmonic.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/data/data_foreman_shallowrelations.txt` & `hatyan-2.7.0/hatyan/data/data_foreman_shallowrelations.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/data/data_schureman_harmonic.csv` & `hatyan-2.7.0/hatyan/data/data_schureman_harmonic.csv`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/data/data_schureman_shallowrelations.csv` & `hatyan-2.7.0/hatyan/data/data_schureman_shallowrelations.csv`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/data/leap-seconds.list` & `hatyan-2.7.0/hatyan/data/leap-seconds.list`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/foreman.py` & `hatyan-2.7.0/hatyan/foreman.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/getonlinedata.py` & `hatyan-2.7.0/hatyan/getonlinedata.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/hatyan_core.py` & `hatyan-2.7.0/hatyan/hatyan_core.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/kw_gemgetij.py` & `hatyan-2.7.0/hatyan/kw_gemgetij.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/kw_havengetallen.py` & `hatyan-2.7.0/hatyan/kw_havengetallen.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/kw_overschrijding.py` & `hatyan-2.7.0/hatyan/kw_overschrijding.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/kw_slotgemiddelden.py` & `hatyan-2.7.0/hatyan/kw_slotgemiddelden.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/schureman.py` & `hatyan-2.7.0/hatyan/schureman.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan/timeseries.py` & `hatyan-2.7.0/hatyan/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,33 +80,36 @@
     M2_period_sec = get_schureman_freqs(['M2']).loc['M2','period [hr]']*3600
     ts_steps_sec_most = np.argmax(np.bincount((ts.index.to_series().diff().iloc[1:].dt.total_seconds()).astype(int).values))
     if ts_steps_sec_most > 60:
         print(f'WARNING: the timestep of the series for which to calculate extremes/HWLW is {ts_steps_sec_most/60:.2f} minutes, but 1 minute is recommended')
     elif ts_steps_sec_most == 0:
         raise Exception('ERROR: ts_steps_sec_most=0, check rounding issue')
     M2period_numsteps = M2_period_sec/ts_steps_sec_most
+    minwidth_numsteps = 2*3600/ts_steps_sec_most # minimal width of 2 hours makes peakfinding more robust: https://github.com/Deltares/hatyan/issues/85
 
     data_pd_HWLW = pd.DataFrame({'times':ts.index,'values':ts['values'],'HWLWcode':np.nan}).reset_index(drop=True)
     #create empty HWLW dataframe
     if data_pd_HWLW['values'].isnull().any():
         data_pd_HWLW = data_pd_HWLW[~data_pd_HWLW['values'].isnull()].reset_index(drop=True)
         print('WARNING: the provided ts for extreme/HWLW calculation contained NaN values. To avoid unexpected results from scipy.signal.find_peaks(), the %i NaN values were removed from the ts (%.2f%%) before calculating extremes/HWLW.'%(len(ts)-len(data_pd_HWLW), (len(ts)-len(data_pd_HWLW))/len(ts)*100))
 
+    min_prominence = 0.01 #minimal prominence to exclude very minor dips/peaks from being seen as aggers.
+    
     if calc_HWLW345 or calc_HWLW1122:
-        #get all local extremes, including aggers and second high waters (1/2/11/22) #takes first value of two equal peaks, prominence naar 0.01 om matige aggers uit te sluiten
-        LWid_all, LWid_all_properties = ssig.find_peaks(-data_pd_HWLW['values'].values, prominence=(0.01,None), width=(None,None), distance=None)
-        HWid_all, HWid_all_properties = ssig.find_peaks(data_pd_HWLW['values'].values, prominence=(0.01,None), width=(None,None), distance=None)
+        #get all local extremes, including aggers and second high waters (1/2/11/22) #takes first value of two equal peaks
+        LWid_all, LWid_all_properties = ssig.find_peaks(-data_pd_HWLW['values'].values, prominence=(min_prominence,None), width=(None,None), distance=None)
+        HWid_all, HWid_all_properties = ssig.find_peaks(data_pd_HWLW['values'].values, prominence=(min_prominence,None), width=(None,None), distance=None)
         data_pd_HWLW.loc[LWid_all,'HWLWcode'] = 22 #all LW
         data_pd_HWLW.loc[HWid_all,'HWLWcode'] = 11 #all HW
 
     #get HWLW (extremes per tidal period).
-    LWid_main_raw,LWid_main_properties = ssig.find_peaks(-data_pd_HWLW['values'].values, prominence=(0.01,None), width=(None,None), distance=M2period_numsteps/1.7) #most stations work with factor 1.4. 1.5 results in all LW values for HoekvanHolland for 2000, 1.7 results in all LW values for Rotterdam for 2000 (also for 1999-2002).
-    HWid_main_raw,HWid_main_properties = ssig.find_peaks(data_pd_HWLW['values'].values, prominence=(0.01,None), width=(None,None), distance=M2period_numsteps/1.9) #most stations work with factor 1.4. 1.5 value results in all HW values for DenHelder for year 2000 (also for 1999-2002). 1.7 results in all HW values for LITHDP 2018. 1.9 results in all correct values for LITHDP 2022
+    LWid_main_raw,LWid_main_properties = ssig.find_peaks(-data_pd_HWLW['values'].values, prominence=(min_prominence,None), width=(minwidth_numsteps,None), distance=M2period_numsteps/1.7) #most stations work with factor 1.4. 1.5 results in all LW values for HoekvanHolland for 2000, 1.7 results in all LW values for Rotterdam for 2000 (also for 1999-2002).
+    HWid_main_raw,HWid_main_properties = ssig.find_peaks(data_pd_HWLW['values'].values, prominence=(min_prominence,None), width=(minwidth_numsteps,None), distance=M2period_numsteps/1.9) #most stations work with factor 1.4. 1.5 value results in all HW values for DenHelder for year 2000 (also for 1999-2002). 1.7 results in all HW values for LITHDP 2018. 1.9 results in all correct values for LITHDP 2022
     # remove main extremes within 6 hours of start/end of timeseries, since they are often missed or invalid.
-    validtimes_idx = data_pd_HWLW.loc[(data_pd_HWLW['times']>=ts.index[0]+dt.timedelta(hours=buffer_hr)) & (data_pd_HWLW['times']<=ts.index[-1]-dt.timedelta(hours=buffer_hr))].index
+    validtimes_idx = data_pd_HWLW.loc[(data_pd_HWLW['times']>=data_pd_HWLW['times'].iloc[0]+dt.timedelta(hours=buffer_hr)) & (data_pd_HWLW['times']<=data_pd_HWLW['times'].iloc[-1]-dt.timedelta(hours=buffer_hr))].index
     LWid_main = LWid_main_raw[np.in1d(LWid_main_raw,validtimes_idx)]
     HWid_main = HWid_main_raw[np.in1d(HWid_main_raw,validtimes_idx)]
     #use valid values to continue process
     data_pd_HWLW.loc[LWid_main,'HWLWcode'] = 2
     data_pd_HWLW.loc[HWid_main,'HWLWcode'] = 1
     
     #drop all non-(local)extreme timesteps and convert HWLWcode column to integers
```

### Comparing `hatyan-2.6.0/hatyan/wrapper_RWS.py` & `hatyan-2.7.0/hatyan/wrapper_RWS.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/hatyan.egg-info/PKG-INFO` & `hatyan-2.7.0/hatyan.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 Metadata-Version: 2.1
 Name: hatyan
-Version: 2.6.0
+Version: 2.7.0
 Summary: hatyan is a tidal analysis and prediction tool of Rijkswaterstaat
 Home-page: https://github.com/Deltares/hatyan
 Author: Jelmer Veenstra
 Author-email: Jelmer.Veenstra@Deltares.nl
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: hatyan,tidal analysis,tidal prediction
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
 
-[![generate-documentation](https://github.com/Deltares/hatyan/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/hatyan/actions/workflows/generate-documentation.yml)
+[![codecov](https://img.shields.io/codecov/c/github/deltares/hatyan.svg?style=flat-square)](https://app.codecov.io/gh/deltares/hatyan)
 [![pytest-hmcenv](https://github.com/Deltares/hatyan/actions/workflows/pytest-hmcenv.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-devenv.yml)
+[![pytest-py38](https://github.com/Deltares/hatyan/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/hatyan/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py39.yml)
+[![pytest-py310](https://github.com/Deltares/hatyan/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py310.yml)
+[![pytest-py311](https://github.com/Deltares/hatyan/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py311.yml)
 [![sigrid-publish](https://github.com/Deltares/hatyan/actions/workflows/sigrid-publish.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/sigrid-publish.yml)
 [![pypi-upload](https://github.com/Deltares/hatyan/actions/workflows/pypi-upload.yml/badge.svg?event=release)](https://github.com/Deltares/hatyan/actions/workflows/pypi-upload.yml)
+[![Supported versions](https://img.shields.io/pypi/pyversions/hatyan.svg)](https://pypi.org/project/hatyan)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_hatyan&metric=alert_status)](https://sonarcloud.io/dashboard?id=Deltares_hatyan)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD)
-
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD?urlpath=/tree/docs/notebooks)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6885342.svg)](https://doi.org/10.5281/zenodo.6885342)
 
 # hatyan
 
 A Python package for harmonic tidal analysis and prediction, based on the FORTRAN version and developed for Rijkswaterstaat. Hatyan contains the methods to derive water level extremes (high and low waters) and several other water level indicators (Kenmerkende Waarden). Furthermore, hatyan provides easier access to Rijkswaterstaat data via their data distribution layer (DataDistributieLaag, DDL).
 
+## Information
 
-Information and examples
---------
+- install with ``pip install hatyan -U``
+- [online documentation](https://deltares.github.io/hatyan) with contributing guide, tutorials/examples, API reference and a convenient search box.
 - [docs folder](https://github.com/Deltares/hatyan/tree/main/docs) with background information
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/hatyan/blob/main/docs/hatyan/index.html) generated from docstrings (replace 'main' in the url with any tagname to view older versions)
-- [jupyter notebooks](https://github.com/Deltares/hatyan/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/hatyan/tree/main/tests/examples) with more example scripts
-
-
-Installation
---------
-
-- optional: download and install Anaconda 64 bit Python 3.8 (or higher) from https://www.anaconda.com/distribution/#download-section
-- open anaconda prompt
-- optional: ``conda create --name hatyan_env -c conda-forge python=3.8 git spyder -y`` (or higher python version)
-- optional: ``conda activate hatyan_env``
-- ``python -m pip install hatyan`` (this installs hatyan and all required packages from PyPI, add a version like ``==2.3.0`` if you require a specific version. Optionally add ``--upgrade``)
-- alternatively: ``python -m pip install git+https://github.com/Deltares/hatyan`` (this installs hatyan and all required packages from github, add a tag like ``@v2.3.0`` if you require a specific release/branch.)
+- Bug or feature request? Create a [GitHub issue](https://github.com/Deltares/dfm_tools/issues)
```

### Comparing `hatyan-2.6.0/hatyan.egg-info/SOURCES.txt` & `hatyan-2.7.0/hatyan.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-CONTRIBUTING.md
-HISTORY.rst
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 hatyan/__init__.py
```

### Comparing `hatyan-2.6.0/tests/test_astrog_main.py` & `hatyan-2.7.0/tests/test_astrog_main.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/tests/test_hatyan_examples.py` & `hatyan-2.7.0/tests/test_hatyan_examples.py`

 * *Files identical despite different names*

### Comparing `hatyan-2.6.0/tests/test_hatyan_main.py` & `hatyan-2.7.0/tests/test_hatyan_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -308,14 +308,78 @@
     assert ts_prediction_direct.index[-1].to_pydatetime() == times_ext_pred[-1]
     assert len(ts_prediction_direct_values) == len(expected_ts_prediction_data_pd_values)
     assert type(ts_prediction_direct_values) == type(expected_ts_prediction_data_pd_values)
     assert (np.abs(ts_prediction_direct_values - expected_ts_prediction_data_pd_values) < 10E-9).all()
 
 
 @pytest.mark.systemtest
+def test_meas_HWLW_toomuch():
+    """
+    this test will fail if the minimal prominence is set to 0.01 or lower, or of the minimal width=None
+    Then there will be an additional LW found right after the HW. With a slightly higher minimal prominence (>0.02) this is avoided.
+    This testcase originates from an issue with a FEWS timeseries: https://github.com/Deltares/hatyan/issues/85
+    """
+    wl_vals = np.array([ 0.4437,  0.563 ,  0.6677,  0.7498,  0.8125,  0.8732,  0.9181,
+            0.9384,  0.944 ,  0.94  ,  0.9254,  0.9033,  0.8602,  0.8258,
+            0.8177,  0.7867,  0.7184,  0.6672,  0.6314,  0.5722,  0.5028,
+            0.428 ,  0.3539,  0.2822,  0.2003,  0.1141,  0.0317, -0.0457,
+           -0.1233, -0.2187, -0.3101, -0.3945, -0.476 , -0.5503, -0.6137,
+           -0.671 , -0.7262, -0.7742, -0.8025, -0.8145, -0.8271, -0.829 ,
+           -0.8131, -0.7856, -0.7616, -0.7289, -0.7176, -0.7114, -0.7088,
+           -0.7111, -0.7113, -0.7106, -0.715 , -0.7282, -0.7392, -0.7434,
+           -0.7384, -0.7405, -0.7321, -0.7202, -0.7054, -0.6847, -0.6514,
+           -0.6082, -0.5656, -0.5155, -0.4549, -0.3814, -0.2934, -0.1994,
+           -0.0949,  0.0291,  0.1794,  0.3537,  0.5279,  0.6908,  0.8318,
+            0.9402,  1.024 ,  1.0951,  1.1474,  1.1639,  1.1582,  1.147 ,
+            1.1298,  1.0997,  1.0717,  1.0828,  1.078 ,  1.0232,  0.9849,
+            0.969 ,  0.9424,  0.9058,  0.8601,  0.8045,  0.7569,  0.6917,
+            0.6198,  0.5531,  0.4802,  0.4109,  0.3291,  0.2442,  0.1692,
+            0.0838, -0.0073, -0.088 , -0.1659, -0.2412, -0.3055, -0.3647,
+           -0.405 , -0.4294, -0.4459, -0.4414, -0.4359, -0.4387, -0.4455,
+           -0.4544, -0.4641, -0.4793, -0.4984, -0.5001, -0.4996, -0.5065,
+           -0.5022, -0.4981, -0.5046, -0.5136, -0.5243, -0.526 , -0.5254,
+           -0.5239, -0.5131, -0.4995, -0.4831, -0.4595, -0.4368, -0.4089,
+           -0.3758, -0.3415, -0.299 , -0.2475, -0.1889, -0.11  , -0.0254,
+            0.0702,  0.1958,  0.3341,  0.4824,  0.6129,  0.709 ,  0.7898,
+            0.8648,  0.9185,  0.955 ,  0.9721,  0.971 ,  0.9652,  0.9486,
+            0.9194,  0.8885,  0.8618,  0.8491,  0.8154,  0.7478,  0.7017,
+            0.6724,  0.6105,  0.5356,  0.4669,  0.3918,  0.323 ,  0.2405])
+    wl_times = pd.date_range('2023-06-13 21:00','2023-06-15 02:00',freq='10min')
+
+    # Then store it as a pandas dataframe and compute extremes
+    wl_pd = pd.DataFrame({'values':wl_vals},index=wl_times)
+
+    wl_pd_ext = hatyan.calc_HWLW(wl_pd)
+
+    assert len(wl_pd_ext) == 3
+    assert (wl_pd_ext['HWLWcode'] == [2,1,2]).all()
+
+
+@pytest.mark.systemtest
+def test_meas_HWLW_toomuch_19y():
+    """
+    Additional testcase for https://github.com/Deltares/hatyan/issues/85
+    The min_width parameter for calc_HWLW() has to be approx 2hrs to properly compute and number almost all of the 19y timeseries
+    Stations HELLVSS/KRIMPADLK/RAKND still fail, but it seems arbitrary and sometimes computing+numbering extremes per year does work
+    """
+    current_station = 'HOEKVHLD'
+    file_dia = os.path.join(dir_testdata,f'{current_station}_obs19.txt')
+    
+    wl_pd = hatyan.readts_dia(file_dia)
+    
+    wl_pd_ext = hatyan.calc_HWLW(wl_pd)
+    
+    # For testing: plot water level timeseries with peaks identified and labeled. 
+    #hatyan.plot_timeseries(ts=wl_pd,ts_ext=wl_pd_ext)
+    
+    # RUN HATYAN: Assign numbers to the extremes
+    wl_pd_ext = hatyan.calc_HWLWnumbering(wl_pd_ext,station=current_station)
+
+
+@pytest.mark.systemtest
 def test_frommergedcomp_HWLW_toomuch():
     """
     This test produces a very short prediction for DENHDR, based on an imported component list. It then calculates extremes (HW/LW) and numbers them both.
     This test is meant to tweak the prominence parameter of scipy.signal.find_peaks() in hatyan.calc_HWLW() and it fails when the prominence is not set or is too small.
     A prominence value of None works for most stations, but fails for DENHDR in this period since a local dip is interpreted as a low water.
     This incorrect LW has a prominence of ~0.03, other peaks in this timeseries have a prominence of >1 and even when lowering M2 to an unrealistic value (0.5*M2) the prominence of peaks is >0.2
     A prominence value of 0.1 makes sure this test succeeds.
```

