# Comparing `tmp/skyCatalogs-1.4.0rc5.tar.gz` & `tmp/skyCatalogs-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyCatalogs-1.4.0rc5.tar", last modified: Tue Jun 13 03:03:55 2023, max compression
+gzip compressed data, was "skyCatalogs-1.5.0rc1.tar", last modified: Wed Aug  2 21:58:09 2023, max compression
```

## Comparing `skyCatalogs-1.4.0rc5.tar` & `skyCatalogs-1.5.0rc1.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.917149 skyCatalogs-1.4.0rc5/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/LICENSE
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     3225 2023-06-13 03:03:55.916754 skyCatalogs-1.4.0rc5/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/README.md
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      774 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/pyproject.toml
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.895034 skyCatalogs-1.4.0rc5/python/
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.896773 skyCatalogs-1.4.0rc5/python/desc/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       66 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/__init__.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.899379 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       93 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       26 2023-06-13 02:56:05.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/_version.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    36150 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/catalog_creator.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.902067 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/objects/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       27 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/objects/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    29080 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/objects/base_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     3748 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/objects/galaxy_object.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.903382 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/readers/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/readers/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2379 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/readers/parquet_reader.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    33685 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/skyCatalogs.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.911993 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1077 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/SED_parquet.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      198 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/common_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    11009 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/config_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      533 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/exceptions.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1211 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/make_fake.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     7656 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/parquet_schema_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     8165 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/sed_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1411 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/sn_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     9870 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/translate_utils.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.914487 skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     3225 2023-06-13 03:03:55.913054 skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1151 2023-06-13 03:03:55.913414 skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/SOURCES.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2023-06-13 03:03:55.913790 skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/dependency_links.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       44 2023-06-13 03:03:55.914161 skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/requires.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        5 2023-06-13 03:03:55.914532 skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/top_level.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2023-06-13 03:03:55.917209 skyCatalogs-1.4.0rc5/setup.cfg
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-13 03:03:55.915852 skyCatalogs-1.4.0rc5/tests/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    11941 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/tests/test_API.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      642 2023-06-13 02:54:22.000000 skyCatalogs-1.4.0rc5/tests/test_skyCatalogs.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.727145 skyCatalogs-1.5.0rc1/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/LICENSE
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3225 2023-08-02 21:58:09.726859 skyCatalogs-1.5.0rc1/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/README.md
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      774 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/pyproject.toml
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.703109 skyCatalogs-1.5.0rc1/python/
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.704722 skyCatalogs-1.5.0rc1/python/desc/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       66 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/__init__.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.707444 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       93 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       26 2023-08-02 19:40:46.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/_version.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    36267 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/catalog_creator.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.711944 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       54 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    23569 2023-08-02 18:13:01.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/base_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     9260 2023-08-02 18:13:01.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/gaia_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     5474 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/galaxy_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1112 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/sncosmo_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1327 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/star_object.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.713079 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/readers/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/readers/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2379 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/readers/parquet_reader.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    34481 2023-08-02 18:13:01.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/skyCatalogs.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.720620 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1077 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/SED_parquet.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      220 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1573 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/catalog_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/common_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11327 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/config_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      533 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/exceptions.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1211 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/make_fake.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     6742 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/parquet_schema_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     7631 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/sed_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2524 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/shapes.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1443 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/sn_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    10239 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/translate_utils.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.723471 skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3225 2023-08-02 21:58:09.722377 skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1460 2023-08-02 21:58:09.722712 skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/SOURCES.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2023-08-02 21:58:09.722983 skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/dependency_links.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       44 2023-08-02 21:58:09.723267 skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/requires.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        5 2023-08-02 21:58:09.723512 skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/top_level.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2023-08-02 21:58:09.727213 skyCatalogs-1.5.0rc1/setup.cfg
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-08-02 21:58:09.726228 skyCatalogs-1.5.0rc1/tests/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11797 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/tests/test_API.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3069 2023-08-02 18:13:01.000000 skyCatalogs-1.5.0rc1/tests/test_gaia_objects.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3747 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/tests/test_object_api.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     5698 2023-08-01 00:25:22.000000 skyCatalogs-1.5.0rc1/tests/test_pointsource.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      642 2023-06-13 02:54:22.000000 skyCatalogs-1.5.0rc1/tests/test_skyCatalogs.py
```

### Comparing `skyCatalogs-1.4.0rc5/LICENSE` & `skyCatalogs-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/PKG-INFO` & `skyCatalogs-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyCatalogs
-Version: 1.4.0rc5
+Version: 1.5.0rc1
 Summary: Writes, reads catalogs input to LSST DESC simulations
 Author-email: Joanne Bogart <jrb@slac.stanford.edu>
 License: Copyright (c) 2018, the skyCatalogs contributors on GitHub, https://github.com/LSSTDESC/skyCatalogs/graphs/contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `skyCatalogs-1.4.0rc5/README.md` & `skyCatalogs-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/pyproject.toml` & `skyCatalogs-1.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/catalog_creator.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/catalog_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 from multiprocessing import Process, Pipe
 from astropy.coordinates import SkyCoord
 import sqlite3
 from desc.skycatalogs.utils.common_utils import print_date
-from desc.skycatalogs.utils.sed_tools import ObservedSedFactory, get_star_sed_path
+from desc.skycatalogs.utils.sed_tools import TophatSedFactory, get_star_sed_path
 from desc.skycatalogs.utils.config_utils import create_config, assemble_SED_models
 from desc.skycatalogs.utils.config_utils import assemble_MW_extinction, assemble_cosmology, assemble_object_types, assemble_provenance, write_yaml
 from desc.skycatalogs.utils.parquet_schema_utils import make_galaxy_schema, make_galaxy_flux_schema, make_star_flux_schema, make_pointsource_schema
-from desc.skycatalogs.objects.base_object import LSST_BANDS, BaseObject
+from desc.skycatalogs.objects.base_object import LSST_BANDS
 
 from desc.skycatalogs.objects.base_object import ObjectCollection
 
 # from dm stack
 from dustmaps.sfd import SFDQuery
 
 """
@@ -87,46 +87,46 @@
                     dict with keys id, lsst_flux_u, ... lsst_flux_y
     '''
     out_dict = {}
 
     o_list = galaxy_collection[l_bnd : u_bnd]
     out_dict['galaxy_id'] = [o.get_native_attribute('galaxy_id') for o in o_list]
     all_fluxes =  [o.get_LSST_fluxes(as_dict=False) for o in o_list]
-    ###all_fluxes = [galaxy_collection[i].get_LSST_fluxes(as_dict=False) for i in range(l_bnd, u_bnd)]
     all_fluxes_transpose = zip(*all_fluxes)
     for i, band in enumerate(LSST_BANDS):
         v = all_fluxes_transpose.__next__()
         out_dict[f'lsst_flux_{band}'] = v
 
     if send_conn:
         send_conn.send(out_dict)
     else:
         return out_dict
 
 class CatalogCreator:
-    def __init__(self, parts, area_partition, skycatalog_root=None,
+    def __init__(self, parts, area_partition=None, skycatalog_root=None,
                  catalog_dir='.', galaxy_truth=None,
                  star_truth=None, sn_truth=None,
                  config_path=None, catalog_name='skyCatalog',
                  output_type='parquet', mag_cut=None,
                  sed_subdir='galaxyTopHatSED', knots_mag_cut=27.0,
                  knots=True, logname='skyCatalogs.creator',
                  pkg_root=None, skip_done=False, flux_only=False,
                  main_only=False, flux_parallel=16, provenance=None,
-                 dc2=False):
+                 dc2=False, sn_object_type='sncosmo'):
         """
         Store context for catalog creation
 
         Parameters
         ----------
         parts           Segments for which catalog is to be generated. If
                         partition type is HEALpix, parts will be a collection
                         of HEALpix pixels
-        area_partition  Dict characterizing partition; e.g. HEALpix,
-                        nside=<something>
+        area_partition  Dict characterizing partition globally (e.g. HEALpix,
+                        nside=<something>) or None.  Defaults to None,
+                        meaning partition is on per-source-type basis
         skycatalog_root Typically absolute directory containing one or
                         more subdirectories for sky catalogs. Defaults
                         to current directory
         catalog_dir     Directory relative to skycatalog_root where catalog
                         will be written.  Defaults to '.'
         galaxy_truth    GCRCatalogs name for galaxy truth (e.g. cosmoDC2)
         config_path     Where to write config file. Default is data
@@ -146,14 +146,15 @@
                         Output info message in either case if file exists.
         flux_only       Only create flux files, not main files
         main_only       Only create main files, not flux files
         flux_parallel   Number of processes to divide work of computing fluxes
         provenance      Whether to write per-output-file git repo provenance
         dc2             Whether to adjust values to provide input comparable
                         to that for the DC2 run
+        sn_object_type  Which object type to use for SNe.
 
         Might want to add a way to specify template for output file name
         and template for input sedLookup file name.
         """
 
         _cosmo_cat = 'cosmodc2_v1.1.4_image_addon_knots'
         _star_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/dc2_stellar_healpixel.db'
@@ -162,35 +163,38 @@
         self._galaxy_stride = 1000000
         if pkg_root:
             self._pkg_root = pkg_root
         else:
             self._pkg_root = os.path.join(os.path.dirname(__file__),
                                           '../../..')
 
-        if area_partition['type'] != 'healpix':
-            raise NotImplementedError(f'CatalogCreator: Unknown partition type {area_partition["type"]} ')
+        self._global_partition = area_partition
+        if area_partition is not None:
+            if area_partition['type'] != 'healpix':
+                raise NotImplementedError(f'CatalogCreator: Unknown partition type {area_partition["type"]} ')
 
         if output_type != 'parquet':
             raise NotImplementedError(f'CatalogCreator: Output type {output_type} not supported')
 
         self._galaxy_truth = galaxy_truth
         if galaxy_truth is None:
             self._galaxy_truth = _cosmo_cat
 
         self._sn_truth = sn_truth
         if self._sn_truth is None:
             self._sn_truth = _sn_db
 
+        self._sn_object_type = sn_object_type
+
         self._star_truth = star_truth
         if self._star_truth is None:
             self._star_truth = _star_db
         self._cat = None
 
         self._parts = parts
-        self._area_partition = area_partition
         if skycatalog_root:
             self._skycatalog_root = skycatalog_root
         else:
             self._skycatalog_root = './'
         if catalog_dir:
             self._catalog_dir = catalog_dir
         else:
@@ -339,16 +343,16 @@
         self._sed_bins = [[int(re.match(tophat_bulge_re, s)['start']), int(re.match(tophat_bulge_re, s)['width'])] for s in sed_bulge_names]
 
         # Sort by value for start
         def _bin_start_key(start_width):
             return start_width[0]
         self._sed_bins.sort(key=_bin_start_key)
 
-        self._obs_sed_factory = ObservedSedFactory(self._sed_bins,
-                                                   assemble_cosmology(self._cosmology))
+        self._obs_sed_factory = TophatSedFactory(self._sed_bins,
+                                                 assemble_cosmology(self._cosmology))
 
         def _sed_bulge_key(s):
             return int(re.match(tophat_bulge_re, s)['start'])
         def _sed_disk_key(s):
             return int(re.match(tophat_disk_re, s)['start'])
 
         # Sort into increaing order by start wavelength
@@ -529,16 +533,15 @@
                 return
 
         # Use same value for row group as was used for main file
         stride = self._galaxy_stride
 
         # If there are multiple row groups, each is stored in a separate
         # object collection. Need to loop over them
-        object_list = self._cat.get_objects_by_hp(pixel,
-                                                  obj_type_set={'galaxy'})
+        object_list = self._cat.get_object_type_by_hp(pixel, 'galaxy')
         writer = None
         global _galaxy_collection
 
         for object_coll in object_list.get_collections():
             _galaxy_collection = object_coll
             # prefetch everything we need. Getting a quantity for one object
             # ensures the quantity is read for the whole row group
@@ -701,15 +704,15 @@
             q1 = f'select {cols} from sne_params where hpid={pixel} '
             q2 = f'select {params} from sne_params where hpid={pixel} '
             with sqlite3.connect(sn_cat) as conn:
                 sn_df = pd.read_sql_query(q1, conn)
                 params_df = pd.read_sql_query(q2, conn)
 
             nobj = len(sn_df['ra'])
-            sn_df['object_type'] = np.full((nobj,), 'sn')
+            sn_df['object_type'] = np.full((nobj,), self._sn_object_type)
 
             sn_df['MW_rv'] = np.full((nobj,), _MW_rv_constant, np.float32())
             sn_df['MW_av'] = _make_MW_extinction(np.array(sn_df['ra']),
                                                    np.array(sn_df['dec']))
 
             # Add fillers for columns not relevant for sn
             sn_df['sed_filepath'] = np.full((nobj),'')
@@ -791,16 +794,15 @@
         if os.path.exists(output_path):
             if not self._skip_done:
                 self._logger.info(f'Overwriting file {output_path}')
             else:
                 self._logger.info(f'Skipping regeneration of {output_path}')
                 return
 
-        object_list = self._cat.get_objects_by_hp(pixel,
-                                                  obj_type_set={'star'})
+        object_list = self._cat.get_object_type_by_hp(pixel, 'star')
         last_row_ix = len(object_list) - 1
         writer = None
 
         # Write out as a single rowgroup as was done for main catalog
         l_bnd = 0
         u_bnd = last_row_ix + 1
 
@@ -851,15 +853,16 @@
             self._config_path = self._output_dir
 
         if path_only:
             return os.path.join(self._config_path, self._catalog_name + '.yaml')
 
 
         config = create_config(self._catalog_name, self._logname)
-        config.add_key('area_partition', self._area_partition)
+        if self._global_partition is not None:
+            config.add_key('area_partition', self._area_partition)
         config.add_key('skycatalog_root', self._skycatalog_root)
         config.add_key('catalog_dir' , self._catalog_dir)
 
         config.add_key('SED_models',
                        assemble_SED_models(self._sed_bins))
         config.add_key('MW_extinction_values', assemble_MW_extinction())
         config.add_key('Cosmology', assemble_cosmology(self._cosmology))
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/objects/base_object.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/objects/base_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,52 +9,31 @@
 from dust_extinction.parameter_averages import F19
 import galsim
 import logging
 from galsim.errors import GalSimRangeError
 
 from desc.skycatalogs.utils.translate_utils import form_object_string
 from desc.skycatalogs.utils.config_utils import Config
-from desc.skycatalogs.utils.sed_tools import ObservedSedFactory
-from desc.skycatalogs.utils.sn_tools import SNObject
 
 '''
 Main object types.   There are also may be subtypes. For example,
 there could be two subtypes for bulge components, differing in the
 form of their associated SEDs
 '''
 
-__all__ = ['BaseObject', 'ObjectCollection', 'ObjectList', 'OBJECT_TYPES',
-           'LSST_BANDS', 'load_lsst_bandpasses', 'CatalogContext']
-GALAXY=1
-GALAXY_BULGE=2
-GALAXY_DISK=3
-GALAXY_KNOTS=4
-STAR=5
-AGN=6
-SN=7
-
-OBJECT_TYPES = {'galaxy' : GALAXY, 'bulge_basic' : GALAXY_BULGE,
-                'disk_basic' : GALAXY_DISK, 'knots_basic' : GALAXY_KNOTS,
-                'star' : STAR, 'agn' : AGN, 'sn' : SN}
+__all__ = ['BaseObject', 'ObjectCollection', 'ObjectList',
+           'LSST_BANDS', 'load_lsst_bandpasses']
 
 LSST_BANDS = ('ugrizy')
 
 # global for easy access for code run within mp
-
-class CatalogContext:
-    def __init__(self, the_sky_cat):
-        global sky_cat
-        self._sky_cat = the_sky_cat
-        sky_cat = the_sky_cat
-
 def load_lsst_bandpasses():
     '''
     Read in lsst bandpasses from standard place, trim, and store in global dict
     Returns: The dict
-
     '''
     global lsst_bandpasses
     lsst_bandpasses = dict()
     rubin_sim_dir = os.getenv('RUBIN_SIM_DATA_DIR', None)
     bp_dir = None
     if rubin_sim_dir:
         bp_dir = os.path.join(rubin_sim_dir, 'throughputs', 'baseline')
@@ -85,32 +64,41 @@
     '''
     Abstract base class for static (in position coordinates) objects.
     Likely need a variant for SSO.
     '''
 
     _bp500 = galsim.Bandpass(galsim.LookupTable([499, 500, 501],[0, 1, 0]),
                              wave_type='nm').withZeropoint('AB')
-    def __init__(self, ra, dec, id, object_type, redshift=None,
-                 belongs_to=None, belongs_index=None):
+
+    def __init__(self, ra, dec, id, object_type, belongs_to, belongs_index,
+                 redshift=None):
         '''
-        Minimum information needed for static (not SSO) objects
-        ra, dec needed to check for region containment
-        belongs_to is object collection, if any, this object belongs to
+        Save at least minimum info needed a fixed (not SSO) object to
+        determine if it's in a region and discover all its other properties.
+        Parameters
+        ra, dec         float         in degrees
+        id              string or int, depending on object type
+        object_type     string        e.g. 'galaxy', 'star', ...
+                                      must appear in catalog config file
+        belongs_to      ObjectCollection  collection this object belongs to
+        belongs_index   int           index of object within its collection
+        redshift        float
         '''
         self._ra = ra
         self._dec = dec
         self._id = id
         self._object_type = object_type
         self._redshift = redshift
         self._belongs_to = belongs_to
         self._belongs_index = belongs_index
 
         # All objects also include redshift information. Also MW extinction,
         # but extinction is by subcomponent for galaxies
 
+
     @property
     def ra(self):
         return self._ra
 
     @property
     def dec(self):
         return self._dec
@@ -181,206 +169,96 @@
         Return the string corresponding to instance catalog line
         Parameters:
             band       One of ['u', 'g', 'r', 'i', 'z', 'y']
             component  Required iff the object has subcomponents (i.e.,
                        object type is 'galaxy')
         Returns: A string formatted like a line in an instance catalog
         '''
-        if self.object_type == 'galaxy':
-            if component not in self.subcomponents:
-                return ''
         return form_object_string(self, band, component)
 
-    def get_sed(self, component=None, resolution=None, mjd=None):
+    def _get_sed(self, component=None, resolution=None, mjd=None):
         '''
         Return sed and mag_norm for a galaxy component or for a star
         Parameters
         ----------
         component    one of 'bulge', 'disk', 'knots' for now. Other components
                      may be supported.  Ignored for stars
         resolution   desired resolution of lambda in nanometers. Ignored
                      for stars.
+        mjd          ignored for static objects
 
         Returns
         -------
         A pair (sed, mag_norm)
+
+        Must be implemented by subclass
         '''
 
-        if self._object_type == 'star':
-            # read in the file; return data from it. Arguments are ignored
-            if component:
-                warnings.warn(f'get_sed: component argument ignored for object type {self._object_type}')
-            if resolution:
-                warnings.warn(f'get_sed: resolution argument ignored for object type {self._object_type}')
-            mag_norm = self.get_native_attribute('magnorm')
-            rel_path = self.get_native_attribute('sed_filepath')
-
-            fpath = os.path.join(os.getenv('SIMS_SED_LIBRARY_DIR'),
-                                 self.get_native_attribute('sed_filepath'))
-
-            return sky_cat.observed_sed_factory.create_pointsource(rel_path), mag_norm
-        elif self._object_type == 'sn':
-            # Make an SNObject and get SED
-            params = self.get_native_attribute('salt2_params')
-            sn = SNObject(params=params)
-            if mjd < sn.mintime() or mjd > sn.maxtime():
-                return None, 0.0
-            # Already normalized so magnorm is zero
-            return sn.get_sed(mjd), 0.0
-        if self._object_type != 'galaxy':
-            raise ValueError('get_sed function only available for stars, sne and galaxy components')
-        if component not in ['disk', 'bulge', 'knots']:
-            raise ValueError(f'Cannot fetch SED for component type {component}')
-
-        th_val = self.get_native_attribute(f'sed_val_{component}')
-        if  th_val is None:   #  values for this component are not in the file
-            raise ValueError(f'{component} not part of this catalog')
-
-        # if values are all zeros or nearly no point in trying to convert
-        if max(th_val) < np.finfo('float').resolution:
-            return None, 0.0
-
-        z_h = self.get_native_attribute('redshift_hubble')
-        z = self.get_native_attribute('redshift')
-
-        sed = sky_cat.observed_sed_factory.create(th_val, z_h, z,
-                                                  resolution=resolution)
-        magnorm = sky_cat.observed_sed_factory.magnorm(th_val, z_h)
+        raise NotImplementedError('Must be implemented by BaseObject subclass if needed')
 
-        return sed, magnorm
 
     def write_sed(self, sed_file_path, component=None, resolution=None,
                   mjd=None):
-        sed, _ = self.get_sed(component=component, resolution=None, mjd=None)
+        sed, _ = self._get_sed(component=component, resolution=None, mjd=None)
 
         wl = sed.wave_list
         flambda = [sed(w) for w in wl]
 
         with open(sed_file_path, 'w') as sed_file:
             for lam, flam in zip(wl, flambda):
                 sed_file.write(f'{lam} {flam}\n')
 
-    def get_dust(self):
+    def _get_dust(self):
         """Return the Av, Rv parameters for internal and Milky Way extinction."""
         internal_av = 0
         internal_rv = 1.
+        # Fails for object types without these native attributes
         galactic_av = self.get_native_attribute('MW_av')
         galactic_rv = self.get_native_attribute('MW_rv')
         return internal_av, internal_rv, galactic_av, galactic_rv
 
-    def get_wl_params(self):
-        """Return the weak lensing parameters, g1, g2, mu."""
-        gamma1 = self.get_native_attribute('shear_1')
-        gamma2 = self.get_native_attribute('shear_2')
-        kappa =  self.get_native_attribute('convergence')
-        # Compute reduced shears and magnification.
-        g1 = gamma1/(1. - kappa)    # real part of reduced shear
-        g2 = gamma2/(1. - kappa)    # imaginary part of reduced shear
-        mu = 1./((1. - kappa)**2 - (gamma1**2 + gamma2**2)) # magnification
-        return g1, g2, mu
+    def _apply_component_extinction(self, sed):
+        # Apply Milky Way extinction.
+
+        iAv, iRv, mwAv, mwRv = self._get_dust()
+
+        sky_cat = self._belongs_to._sky_catalog
+        sed = sky_cat.extinguisher.extinguish(sed, mwAv)
+
+        return sed
+
+    def _get_sed_from_file(self, fpath, redshift=0):
+        sed = galsim.SED(fpath, wave_type='nm', flux_type='flambda')
+        if redshift > 0:
+            sed = sed.atRedshift(redshift)
+        return sed
 
     def get_gsobject_components(self, gsparams=None, rng=None):
         """
         Return a dictionary of the GSObject components for the
         sky catalogs object, keyed by component name.
+        Must be implemented by subclass
         """
-        if gsparams is not None:
-            gsparams = galsim.GSParams(**gsparams)
-        if self.object_type == 'star' or self.object_type == 'sn':
-            return {None: galsim.DeltaFunction(gsparams=gsparams)}
-        if self.object_type != 'galaxy':
-            raise RuntimeError("Do not know how to handle object type "
-                               f"{self.object_type}")
-        obj_dict = {}
-        for component in self.subcomponents:
-            # knots use the same major/minor axes as the disk component.
-            my_component = 'disk' if component != 'bulge' else 'bulge'
-            a = self.get_native_attribute(
-                f'size_{my_component}_true')
-            b = self.get_native_attribute(
-                f'size_minor_{my_component}_true')
-            assert a >= b
-            hlr = (a*b)**0.5   # approximation for half-light radius
-
-            e1 = self.get_native_attribute(
-                f'ellipticity_1_{my_component}_true')
-            e2 = self.get_native_attribute(
-                f'ellipticity_2_{my_component}_true')
-
-            if component == 'knots':
-                npoints = self.get_native_attribute('n_knots')
-                assert npoints > 0
-                obj = galsim.RandomKnots(npoints=npoints,
-                                         half_light_radius=hlr, rng=rng,
-                                         gsparams=gsparams)
-            else:
-                n = self.get_native_attribute(f'sersic_{component}')
-                # Quantize the n values at 0.05 so that galsim can
-                # possibly amortize sersic calculations from the previous
-                # galaxy.
-                n = round(n*20.)/20.
-                obj = galsim.Sersic(n=n, half_light_radius=hlr,
-                                    gsparams=gsparams)
-
-            # NOTE: Whether or not the minus signs in the next executable
-            # line are needed in general or just for generating DC2-like
-            # results is still TBD. They are included here in order to
-            # reproduce the effect of adding 90 degrees to position angle
-            # in the old code.
-            shear = galsim.Shear(g1=-e1, g2=-e2)
-            obj = obj._shear(shear)
-            g1, g2, mu = self.get_wl_params()
-            obj_dict[component] = obj._lens(g1, g2, mu)
-        return obj_dict
+        raise NotImplementedError('Subclass must implement get_gsobject_components')
 
     def get_observer_sed_component(self, component, mjd=None):
         """
         Return the SED for the specified subcomponent of the SkyCatalog
         object, applying internal extinction, redshift, and Milky Way
         extinction.
 
         For Milky Way extinction, the Fitzpatrick, et al. (2019) (F19)
         model, as implemented in the dust_extinction package, is used.
 
         The SEDs are computed assuming exposure times of 1 second.
-        """
-        # Create a galsim.SED for this subcomponent.
-
-        if self._object_type == 'star':
-            sed, magnorm = self.get_sed(component=component, mjd=mjd)
-            # The SED is in units of photons/nm/cm^2/s
-            # -0.9210340371976184 = -np.log(10)/2.5. Use to convert mag to flux
-            flux_500 = np.exp(-0.9210340371976184 * magnorm)
-            sed = sed.withMagnitude(0, self._bp500)
-            sed = sed*flux_500
-        elif self._object_type == 'galaxy':
-            # For sn & galaxy components sed already has correct normalization
-            sed, _ = self.get_sed(component=component)
-            if sed is None:
-                # This subcomponent has zero emission so return None.
-                return None
-        elif self._object_type == 'sn':
-            sed, _ = self.get_sed(component=component, mjd=mjd)
-            if sed is None:
-                return None
-        else:
-            # Raise NYI exception?
-            pass
 
-        iAv, iRv, mwAv, mwRv = self.get_dust()
-        if iAv > 0:
-            # Apply internal extinction model, which is assumed
-            # to be the same for all subcomponents.
-            pass  #TODO add implementation for internal extinction.
+        Must be implemented by subclass
+        """
 
-        # redshift already applied by create or create_pointsource
-
-        # Apply Milky Way extinction.
-        sed = sky_cat.extinguisher.extinguish(sed, mwAv)
-        return sed
+        raise NotImplementedError('get_observer_sed_component must be implemented by subclass')
 
     def get_observer_sed_components(self, mjd=None):
         """
         Return a dictionary of the SEDs, keyed by component name.
         """
         sed_components = {}
         subcomponents = [None] if not self.subcomponents \
@@ -399,19 +277,14 @@
         sed = None
         for sed_component in self.get_observer_sed_components(mjd=mjd).values():
             if sed is None:
                 sed = sed_component
             else:
                 sed += sed_component
 
-        if sed is None:
-            return sed
-        if 'shear_1' in self.native_columns:
-            _, _, mu = self.get_wl_params()
-            sed *= mu
         return sed
 
     def get_flux(self, bandpass, sed=None, mjd=None):
         """
         Return the total object flux integrated over the bandpass
         in photons/sec/cm^2
         Use supplied sed if there is one
@@ -435,28 +308,26 @@
 
         return [sed.calculateFlux(b) for b in bandpasses]
 
     def get_LSST_flux(self, band, sed=None, cache=True, mjd=None):
         if not band in LSST_BANDS:
             return None
         att = f'lsst_flux_{band}'
-        if mjd is None:
-            # Check if it's already an attribute
-            val = getattr(self, att, None)
-            if val is not None:
-                return val
 
-        # For now exclude sn
-        if self.object_type != 'sn':
-            if att in self.native_columns:
-                return self.get_native_attribute(att)
+        # Check if it's already an attribute
+        val = getattr(self, att, None)
+        if val is not None:
+            return val
+
+        if att in self.native_columns:
+            return self.get_native_attribute(att)
 
         val = self.get_flux(lsst_bandpasses[band], sed=sed, mjd=mjd)
 
-        if cache and mjd is None:
+        if cache:
             setattr(self, att, val)
         return val
 
     def get_LSST_fluxes(self, cache=True, as_dict=True, mjd=None):
         '''
         Return a dict of fluxes for LSST bandpasses or, if as_dict is False,
         just a list in the same order as LSST_BANDS
@@ -471,61 +342,74 @@
                 fluxes[band] = self.get_LSST_flux(band, sed=sed,
                                                   cache=cache, mjd=mjd)
         if as_dict:
             return fluxes
         else:
             return list(fluxes.values())
 
+
 class ObjectCollection(Sequence):
     '''
-    Class for collection of static objects coming from the same
+    Class for collection of fixed (not SSO) objects coming from the same
     source (e.g., file for particular healpix)
     Many of the methods look the same as for BaseObject but they return arrays
     rather than a single number.  There are some additional methods
     '''
     def __init__(self, ra, dec, id, object_type, partition_id, sky_catalog,
-                 region=None, mask=None, readers=None, row_group=0):
+                 region=None, mjd=None, mask=None, readers=None, row_group=0):
         '''
-        Minimum information needed for static objects.
-        specified, has already been used by the caller to generate mask.
-        ra, dec, id must be array-like and the same length
-        object_type  may be either single value or array-like (could be
-        useful if more than one object type is stored in the same file)
-        partition_id (e.g. healpix id)
-        sky_catalog instance of SkyCatalog class
-        (redshift should probably be ditched; no need for it)
-        (similarly for region with current code structure. Information
-        needed is encoded in mask)
-
-        mask  indices to be masked off, e.g. because region does not
-              include the entire healpix pixel
-        readers one per file associated with the type(s).
+        Parameters
+        ra, dec      float, array-like of same length
+        id           array-like, same length as ra and dec.   int or string
+        object_type  single string or (if contained objects may be of
+                     different types) array-like
+        parition_id  int (e.g. healpix id)  if objects are partitioned by
+                     location; else None
+        sky_catalog  Instance of SkyCatalog class, typically obtained by
+                     calling open_catalog
+        region       maybe be used to determine which objects are in the
+                     collection
+        mjd          MJD of the observation epoch.  This is used by
+                     time-varying objects, e.g., SNe, stars.
+        mask         indices to be masked off, e.g. in case not all objects
+                     in the partition (such as healpixel) are in the region
+        readers      may be used to recover properties for objects in this
+                     collection, one reader per relevant file
+        row_group    used in case backing files are in parquet format
+
         '''
         self._ra = np.array(ra)
         self._dec = np.array(dec)
         self._id = np.array(id)
         self._rdrs = readers
         self._partition_id = partition_id
-        self._sky_catalog = sky_catalog   # might not need this
+        self._sky_catalog = sky_catalog
         self._config = Config(sky_catalog.raw_config)
         self._mask = mask
         self._row_group = row_group
 
+        self._object_class = sky_catalog.cat_cxt.lookup_source_type(object_type)
+
         # Maybe the following is silly and object_type should always be stored
         # as arrays
         if isinstance(object_type, list):
             self._object_types = np.array(object_type)
             self._object_type_unique = None
             self._uniform_object_type = False
         else:
             self._object_types = None
             self._object_type_unique = object_type
             self._uniform_object_type = True
 
         self._region = region
+        self._mjd = mjd
+
+    @property
+    def mjd(self):
+        return self._mjd
 
     @property
     def partition_id(self):
         return self._partition_id
 
     @property
     def config(self):
@@ -547,21 +431,23 @@
             columns = columns.union(rdr.columns)
         return columns
 
     @property
     def subcomponents(self):
         '''
         Return list of all subcomponents for objects in this collection.
-        Only galaxies have subcomponents
+        Only galaxies have true subcomponents
         '''
         subs = []
         if self._object_type_unique == 'galaxy':
             for s in ['bulge', 'disk', 'knots']:
                 if f'sed_val_{s}' in self.native_columns:
                     subs.append(s)
+        else:
+            return ['this_object']
         return subs
 
     def get_native_attribute(self, attribute_name):
         '''
         Retrieve a particular attribute for a collection
         If we already have it, just return it.  Otherwise attempt
         to fetch.   Reader should check whether the attribute actually
@@ -651,29 +537,28 @@
 
         if self._uniform_object_type:
             object_type = self._object_type_unique
         else:
             object_type = self._object_types[key]
 
         if isinstance(key, int) or isinstance(key, np.int64):
-            return BaseObject(self._ra[key], self._dec[key], self._id[key],
-                              object_type, belongs_to=self,
-                              belongs_index=key)
+            return self._object_class(self._ra[key], self._dec[key],
+                                      self._id[key], object_type, self, key)
 
         elif type(key) == slice:
             ixdata = [i for i in range(min(key.stop,len(self._ra)))]
             ixes = itertools.islice(ixdata, key.start, key.stop, key.step)
-            return [BaseObject(self._ra[i], self._dec[i], self._id[i],
-                               object_type, belongs_to=self, belongs_index=i)
+            return [self._object_class(self._ra[i], self._dec[i], self._id[i],
+                                       object_type, self, i)
                     for i in ixes]
 
         elif type(key) == tuple and isinstance(key[0], Iterable):
             #  check it's a list of int-like?
-            return [BaseObject(self._ra[i], self._dec[i], self._id[i],
-                               object_type, belongs_to=self, belongs_index=i)
+            return [self._object_class(self._ra[i], self._dec[i], self._id[i],
+                                       object_type, self, i)
                     for i in key[0]]
 
 
     def get_partition_id(self):
         return self._partition_id
 
     def count(self, obj):
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/readers/parquet_reader.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/readers/parquet_reader.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/skyCatalogs.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/skyCatalogs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,38 @@
 import os
 import sys
 import re
 import yaml
 import logging
-from collections import namedtuple
 import healpy
 import numpy as np
 import numpy.ma as ma
 import pyarrow.parquet as pq
 from astropy import units as u
 from desc.skycatalogs.objects.base_object import load_lsst_bandpasses
-from desc.skycatalogs.objects.base_object import  CatalogContext
-from desc.skycatalogs.objects import *
-from desc.skycatalogs.readers import *
+from desc.skycatalogs.utils.catalog_utils import CatalogContext
+from desc.skycatalogs.objects.base_object import ObjectList, ObjectCollection
+from desc.skycatalogs.objects.gaia_object import GaiaObject, GaiaCollection
 from desc.skycatalogs.readers import ParquetReader
-from desc.skycatalogs.utils.sed_tools import ObservedSedFactory
+from desc.skycatalogs.utils.sed_tools import TophatSedFactory
 from desc.skycatalogs.utils.sed_tools import MilkyWayExtinction
 from desc.skycatalogs.utils.config_utils import Config
+from desc.skycatalogs.utils.shapes import Box, Disk, PolygonalRegion
+from desc.skycatalogs.objects.sncosmo_object import SncosmoObject
+from desc.skycatalogs.objects.star_object import StarObject
+from desc.skycatalogs.objects.galaxy_object import GalaxyObject
 
-__all__ = ['SkyCatalog', 'open_catalog', 'Box', 'Disk', 'PolygonalRegion']
-
-
-Box = namedtuple('Box', ['ra_min', 'ra_max', 'dec_min', 'dec_max'])
-
-# radius is measured in arcseconds
-Disk = namedtuple('Disk', ['ra', 'dec', 'radius_as'])
-
-from lsst.sphgeom import ConvexPolygon, UnitVector3d, LonLat
-class PolygonalRegion:
-
-    def __init__(self, vertices_radec=None, convex_polygon=None):
-        '''
-        Supply either an object of type lsst.sphgeom.ConvexPolygon
-        or a list of vertices, each a tuple (ra, dec) in degrees,
-        which describe a convex polygon
-        '''
-        if convex_polygon:
-            if isinstance(convex_polygon, ConvexPolygon):
-                self._convex_polygon = convex_polygon
-                return
-        if vertices_radec:
-            if not isinstance(vertices_radec, list):
-                raise TypeError(f'PolygonalRegion: Argument {vertices_radec} is not a list')
-            vertices = [UnitVector3d(LonLat.fromDegrees(v_rd[0], v_rd[1])) for v_rd in vertices_radec]
-            self._convex_polygon = ConvexPolygon(vertices)
-            return
-        raise ValueError('PolygonalRegion: Either vertices_radec or convex_polygon must have an acceptable value')
-
-    def get_vertices(self):
-        '''
-        Return vertices as list of 3d vectors
-        '''
-        return self._convex_polygon.getVertices()
-
-    def get_vertices_radec(self):
-        v3d = self.get_vertices()
-        vertices_radec = []
-        for v in v3d:
-            vertices_radec.append((LonLat.longitudeOf(v).asDegrees(),
-                                   LonLat.latitudeOf(v).asDegrees()))
-        return vertices_radec
-
-    def get_containment_mask(self, ra, dec, included=True):
-        '''
-        Parameters
-        ----------
-        ra, dec      parallel float arrays, units are degrees. Together
-                     they define the list of points to be checked for
-                     containment
-        included     boolean   If true, mask bit will be set to True for
-                               contained points, else False.    Reverse
-                               the settings if included is False
-        '''
-        # convert to radians
-        ra = [(r * u.degree).to_value(u.radian) for r in ra]
-        dec = [(d * u.degree).to_value(u.radian) for d in dec]
-
-        mask = self._convex_polygon.contains(ra, dec)
-        if included:
-            return mask
-        else:
-            return np.logical_not(mask)
+__all__ = ['SkyCatalog', 'open_catalog']
 
 # This function should maybe be moved to utils
 def _get_intersecting_hps(hp_ordering, nside, region):
     '''
     Given healpixel structure defined by hp_ordering and nside, find
-    all healpixels which instersect region, where region may be either
-    a box or a disk.
+    all healpixels which intersect region, where region may be a box,
+    a disk or a polygonal region.
     Return as some kind of iterable
     Note it's possible extra hps which don't actually intersect the region
     will be returned
     '''
     # First convert region description to an array (4,3) with (x,y,z) coords
     # for each vertex
     if isinstance(region, Box):
@@ -117,16 +58,18 @@
                                     inclusive=True, nest=False)
 
 def _compress_via_mask(tbl, id_column, region, galaxy=True):
     '''
     Parameters
     ----------
     tbl          data table including columns named "ra", "dec", and id_column
+                 (and also "object_type" colum if galaxy is False)
     id_column    string
     region       mask should restrict to this region (or not at all if None)
+    galaxy       flag so we know whether or not to return "object_type"
 
     Returns
     -------
     4 values for galaxies: ra, dec, id, mask
     5 values for pointsources: ra, dec, id, object_type, mask
     If objects are in the region, ra, dec, id correspond to those objects.
     mask will mask off unused objects
@@ -238,14 +181,18 @@
         ----------
         config:  dict.  Typically the result of loading a yaml file
         mp:      boolean  Default False. Set True to enable multiprocessing.
         skycatalog_root: If not None, overrides value in config or
                          in environment variable SKYCATALOG_ROOT
         '''
         self._config = Config(config)
+        self._global_partition = None
+        if 'area_partition' in self._config.keys():       # old-style config
+            self._global_partition = self._config['area_partition']
+
         self._logger = logging.getLogger('skyCatalogs.client')
 
         if not self._logger.hasHandlers():
             self._logger.setLevel(loglevel)
             ch = logging.StreamHandler()
             ch.setLevel(loglevel)
             formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
@@ -269,28 +216,49 @@
         self._logger.info(f'Catalog data will be read from {self._cat_dir}')
         # There may be more to do at this point but not too much.
         # In particular, don't read in anything from data files
 
         self.verbose = verbose
         self._validate_config()
 
+
         # Outer dict: hpid for key. Value is another dict
         #    with keys 'files', 'object_types', each with value another dict
-        #    for 'files', map filepath to handle (initially None)
-        #    for 'object_types', map object type to filepath
+        #       for 'files', map filepath to handle (initially None)
+        #       for 'object_types', map object type to filepath
         self._hp_info = dict()
         hps = self._find_all_hps()
 
+        # NOTE: the use of TophatSedFactory is appropriate *only* for an
+        # input galaxy catalog with format like cosmoDC2, which includes
+        # definitions of tophat SEDs. A different implementation will
+        # be needed for newer galaxy catalogs
+        th_parameters = self._config.get_tophat_parameters();
         self._observed_sed_factory =\
-            ObservedSedFactory(self._config.get_tophat_parameters(),
-                               config['Cosmology'])
-        self._extinguisher = MilkyWayExtinction(self.observed_sed_factory)
+            TophatSedFactory(th_parameters, config['Cosmology'])
+
+        self._extinguisher = MilkyWayExtinction()
 
         # Make our properties accessible to BaseObject, etc.
-        self.catalog_context = CatalogContext(self)
+        self.cat_cxt = CatalogContext(self)
+
+        # register object types which are in the config
+        if 'gaia_star' in config['object_types']:
+            self.cat_cxt.register_source_type('gaia_star',
+                                              object_class=GaiaObject,
+                                              collection_class=GaiaCollection)
+        if 'sncosmo' in config['object_types']:
+            self.cat_cxt.register_source_type('sncosmo',
+                                              object_class=SncosmoObject)
+        if 'star' in config['object_types']:
+            self.cat_cxt.register_source_type('star',
+                                              object_class=StarObject)
+        if 'galaxy' in config['object_types']:
+            self.cat_cxt.register_source_type('galaxy',
+                                              object_class=GalaxyObject)
 
     @property
     def observed_sed_factory(self):
         return self._observed_sed_factory
 
     @property
     def extinguisher(self):
@@ -318,16 +286,15 @@
         and the object types included in those files.
 
         Returns
         -------
         Set of healpix pixels with at least one file in the directory
 
         '''
-
-        # If major organization is by healpix, healpix # will be in
+        # If major organization is by healpix, healpix # could be in
         # subdirectory name.  Otherwise there may be no subdirectories
         # or data may be organized by component type.
         # Here only handle case where data files are directly in root dir
         files = os.listdir(self._cat_dir)
         o_types = self._config['object_types']
 
         hp_set = set()
@@ -351,234 +318,232 @@
                                 this_hp['files'][f] = None
                             if ot in this_hp['object_types']:
                                 this_hp['object_types'][ot].append(f)
                             else:
                                 this_hp['object_types'][ot] = [f]
         return hp_set
 
-    def get_hps_by_region(self, region):
+    def get_hps_by_region(self, region, object_type='galaxy'):
         '''
         Parameters
         ----------
         Region can be a box (named 4-tuple (min-ra, max-ra, min-dec, max-dec)),
         a circle (named 3-tuple (ra, dec, radius)) or of type
         PolygonalRegion.
         Catalog area partition must be by healpix
 
         Returns
         -------
         Set of healpixels intersecting the region
         '''
         # If area_partition doesn't use healpix, raise exception
-
-        return _get_intersecting_hps(
-            self._config['area_partition']['ordering'],
-            self._config['area_partition']['nside'],
-            region)
+        if self._global_partition is None:
+            partition = self._config['object_types'][object_type]['area_partition']
+        else:
+            partition = self._global_partition
+        return _get_intersecting_hps(partition['ordering'], partition['nside'],
+                                     region)
 
     def get_object_type_names(self):
         '''
         Returns
         -------
         All object type names in the catalog's config
         '''
         return set(self._config['object_types'].keys())
 
     # Add more functions to return parts of config of possible interest
     # to user
 
-    def get_objects_by_region(self, region, obj_type_set=None, datetime=None):
+    def toplevel_only(self, object_types):
+        '''
+        Parameters
+        ----------
+        object_types     Set of object type names
+        Remove object types with a parent.  Add in the parent.
+
+        Return the resulting set
+        '''
+        objs_copy = set(object_types)
+        for obj in object_types:
+            parent = self._config.get_object_parent(obj)
+            if parent is not None:
+                objs_copy.remove(obj)
+                objs_copy.add(parent)
+        return objs_copy
+
+    def get_objects_by_region(self, region, obj_type_set=None, mjd=None):
         '''
         Parameters
         ----------
         region         region is a named tuple(may be box or circle)
                        or object of type PolygonalRegion
         obj_type_set   Return only these objects. Defaults to all available
-        datetime       Python datetime object. Ignored except for SSO
+        mjd            MJD of observation epoch.
 
         Returns
         -------
         ObjectList containing sky objects visible in the region
         [at the specified time]
         '''
         # Take intersection of obj_type_list and available object types
         # Determine healpix intersecting the region
 
         if self.verbose:
             print("Region ", region)
             print("obj_type_set ", obj_type_set)
-        if self._config['area_partition']['type'] == 'healpix':
-            hps = self.get_hps_by_region(region)
+        # This must be done per object type
+        # if self._config['area_partition']['type'] == 'healpix':
+        #     hps = self.get_hps_by_region(region)
 
         # otherwise raise a not-supported exception
 
         object_list = ObjectList()
         if obj_type_set is None:
             obj_types = self.get_object_type_names()
         else:
             obj_types = self.get_object_type_names().intersection(obj_type_set)
-        for hp in hps:
-            # Maybe have a multiprocessing switch? Run-time option when
-            # catalog is opened?
-            c = self.get_objects_by_hp(hp, region, obj_types, datetime)
-            if (len(c)) > 0:
-                object_list.append_object_list(c)
+        obj_types = self.toplevel_only(obj_types)
+
+        for ot in obj_types:
+            new_list = self.get_object_type_by_region(region, ot, mjd=mjd)
+            object_list.append_object_list(new_list)
 
         return object_list
 
-    def get_object_iterator_by_region(self, region=None, obj_type_set=None,
-                                      max_chunk=None, datetime=None):
+    def get_object_type_by_region(self, region, object_type, mjd=None):
         '''
-        Not yet implemented.
-
         Parameters
         ----------
-        region         Either a box or a circle (each represented as
-                       named tuple) or object of type PolygonalRegion
-        obj_type_set   Return only these objects. Defaults to all available
-        max_chunk      If specified, iterator will return no more than this
-                       number of objections per iteration
-        datetime       Python datetime object. Ignored for all but SSO
+        region        box, circle or PolygonalRegion. Supported region
+                      types made depend on object_type
+        object_type   known object type without parent
+        mjd           MJD of observation epoch.
 
-        Returns
-        -------
-        An iterator
+        Returns all objects found
         '''
-        raise NotImplementedError('get_object_iterator_by_region not implemented yet. See get_objects_by_region instead for now')
 
-    def get_objects_by_hp(self, hp, region=None, obj_type_set=None,
-                          datetime=None):
-        '''
-        Find all objects in the healpixl (and region if specified)
-        of requested types
+        out_list = ObjectList()
+        if self._global_partition is not None:
+            partition = self._global_partition
+        else:
+            partition = self._config['object_types'][object_type]['area_partition']
 
-        Parameters
-        ----------
-        hp     The healpix pixel.
-        region If supplied defines a disk, box or convex polygon.
-               Return only objects contained in it
-        obj_type_set   Type of objects to fetch.  Defaults to all
-        datetime       Ignored for now; no support for moving objects
+        coll_type = self.cat_cxt.lookup_collection_type(object_type)
+        if coll_type is not None:
+            out_list.append_collection(coll_type.load_collection(region, self,
+                                                                 mjd=mjd))
+            return out_list
+
+        if partition != 'None':
+            if partition['type'] == 'healpix':
+                hps = self.get_hps_by_region(region, object_type)
+                for hp in hps:
+                    c = self.get_object_type_by_hp(hp, object_type, region, mjd)
+                    if len(c) > 0:
+                        out_list.append_object_list(c)
+                return out_list
+        else:
+            raise NotImplementedError(f'Unsupported object type {object_type}')
 
-        Returns
-        -------
-        ObjectList containing sky objects in the region and the hp
-        '''
+    def get_object_type_by_hp(self, hp, object_type, region=None, mjd=None):
         object_list = ObjectList()
 
+        #  Do we need to check more specifically by object type?
         if hp not in self._hp_info:
-            print(f'WARNING: In SkyCatalog.get_objects_by_hp healpixel {hp} intersects region but has no catalog file')
+            print(f'WARNING: In SkyCatalog.get_object_type_by_hp healpixel {hp} intersects region but has no catalog file')
             return object_list
 
-        G_COLUMNS = ['galaxy_id', 'ra', 'dec']
-        PS_COLUMNS = ['object_type', 'id', 'ra', 'dec']
+        if object_type == 'galaxy':
+            COLUMNS = ['galaxy_id', 'ra', 'dec']
+            id_name = 'galaxy_id'
+        elif object_type in ['star', 'sncosmo']:
+            COLUMNS = ['object_type', 'id', 'ra', 'dec']
+            id_name = 'id'
+        else:
+            raise NotImplementedError(f'Unsupported object type {object_type}')
+
         if self.verbose:
             print('Working on healpix pixel ', hp)
-
-        obj_types = obj_type_set
-        if obj_types is None:
-            obj_types = self._config['object_types'].keys()
-        else:
-            parents = set()
-            for ot in obj_types:
-                if 'parent' in self._config['object_types'][ot]:
-                    parents.add(self._config['object_types'][ot]['parent'])
-            obj_types = obj_types.union(parents)
-
-        # Find the right Sky Catalog file or files (depends on obj_type_set)
-        # Get file handle(s) and store if we don't already have it (them)
-
-        # Associate object types with files and files with readers.
-        # May be > one type per reader (e.g. different kinds of point sources
-        # stored in a single file)
-        # Also may be more than one file per type (galaxy has two)
         rdr_ot = dict()   # maps readers to set of object types it reads
 
-        for ot in obj_types:
-            # FInd files associated with this type
-            if 'file_template' in self._config['object_types'][ot]:
-                f_list = self._hp_info[hp]['object_types'][ot]
-            elif 'parent' in self._config['object_types'][ot]:
-                f_list = self._hp_info[hp]['object_types'][self._config['object_types'][ot]['parent']]
-
-            for f in f_list:
-                if self._hp_info[hp]['files'][f] is None:            # no reader yet
-                    full_path = os.path.join(self._cat_dir, f)
-                    the_reader = parquet_reader.ParquetReader(full_path, mask=None)
-                    self._hp_info[hp]['files'][f] = the_reader
-                else:
-                    the_reader = self._hp_info[hp]['files'][f]
+        if 'file_template' in self._config['object_types'][object_type]:
+            f_list = self._hp_info[hp]['object_types'][object_type]
+        elif 'parent' in self._config['object_types'][object_type]:
+            f_list = self._hp_info[hp]['object_types'][self._config['object_types'][ot]['parent']]
+
+        for f in f_list:
+            if self._hp_info[hp]['files'][f] is None:            # no reader yet
+                full_path = os.path.join(self._cat_dir, f)
+                the_reader = ParquetReader(full_path, mask=None)
+                self._hp_info[hp]['files'][f] = the_reader
+            else:
+                the_reader = self._hp_info[hp]['files'][f]
                 # associate object type with this reader
-                if the_reader in rdr_ot:
-                    rdr_ot[the_reader].add(ot)
-                else:
-                    rdr_ot[the_reader] = set([ot])
-
-        # Now get minimal columns for objects using the readers
-        galaxy_readers = []
-        pointsource_readers = []
+            if the_reader in rdr_ot:
+                rdr_ot[the_reader].add(object_type)
+            else:
+                rdr_ot[the_reader] = set([object_type])
 
-        # First make a pass to separate out the readers
+        # Find readers needed to get minimal columns for our object type
+        the_readers = []
         for rdr in rdr_ot:
-            if 'galaxy' in rdr_ot[rdr]:
-                galaxy_readers.append(rdr)
-            elif ot in rdr_ot[rdr]:
-                pointsource_readers.append(rdr)
-
-        # Make galaxy collections
-        for rdr in galaxy_readers:
-            if 'ra' not in rdr.columns:
-                continue
-
-            # Make a collection for each row group
-
-            for rg in range(rdr.n_row_groups):
-                arrow_t = rdr.read_columns(G_COLUMNS, None, rg)
-
-                ra_c, dec_c, id_c, mask = _compress_via_mask(arrow_t,
-                                                             'galaxy_id',
-                                                             region)
-
-                if ra_c is not None:
-                    new_collection = ObjectCollection(ra_c, dec_c, id_c,
-                                                      'galaxy', hp, self,
-                                                      region=region, mask=mask,
-                                                      readers=galaxy_readers,
-                                                      row_group=rg)
-                    object_list.append_collection(new_collection)
+            if object_type in rdr_ot[rdr]:
+                the_readers.append(rdr)
 
-        # Make point source collection
-        for rdr in pointsource_readers:
+        # Unfortunately galaxies and point sources can't be handled quite
+        # the same way since we need to read an extra column for pointsources
+        # There will have to be some "if galaxy... else ... code"
+        for rdr in the_readers:
             if 'ra' not in rdr.columns:
                 continue
 
             # Make a collection for each row group
             for rg in range(rdr.n_row_groups):
-                arrow_t = rdr.read_columns(PS_COLUMNS, None, rg)
-
-                ra_c, dec_c, id_c, object_type,mask = _compress_via_mask(arrow_t, 'id', region, galaxy=False)
+                arrow_t = rdr.read_columns(COLUMNS, None, rg)
+                if object_type == 'galaxy':
+                    ra_c, dec_c, id_c, mask = _compress_via_mask(arrow_t,
+                                                                 id_name,
+                                                                 region)
+                    if ra_c is not None:
+                        new_collection = ObjectCollection(ra_c, dec_c, id_c,
+                                                          'galaxy', hp, self,
+                                                          region=region,
+                                                          mjd=mjd,
+                                                          mask=mask,
+                                                          readers=the_readers,
+                                                          row_group=rg)
+                        object_list.append_collection(new_collection)
 
-                if ra_c is not None and object_type[0] in obj_type_set:
-                    new_collection = ObjectCollection(ra_c, dec_c, id_c,
-                                                      object_type[0], hp, self,
-                                                      region=region, mask=mask,
-                                                      readers=pointsource_readers, row_group=rg)
-                    object_list.append_collection(new_collection)
+                else:
+                    ra_c, dec_c, id_c, object_type_c, mask =\
+                        _compress_via_mask(arrow_t, id_name, region,
+                                           galaxy=False)
+                    if ra_c is not None and object_type_c[0] == object_type:
+                        new_collection = ObjectCollection(ra_c, dec_c, id_c,
+                                                          object_type_c[0], hp,
+                                                          self, region=region,
+                                                          mjd=mjd,
+                                                          mask=mask,
+                                                          readers=the_readers,
+                                                          row_group=rg)
+                        object_list.append_collection(new_collection)
 
         return object_list
 
+
     # For generator version, do this a row group at a time
     #    but if region cut leaves too small a list, read more rowgroups
     #    to achieve a reasonable size list (or exhaust the file)
     def get_object_iterator_by_hp(self, hp, obj_type_set=None,
-                                  max_chunk=None, datetime=None):
+                                  max_chunk=None, mjd=None):
         '''
         Parameters
         ----------
-        datetime       Python datetime object.
+        mjd            MJD of observation epoch
         hp             A healpix id
         obj_type_set   Return only these objects. Defaults to all available
         max_chunk      If specified, iterator will return no more than this
                        number of objections per iteration
         Returns
         -------
         An iterator
@@ -600,32 +565,34 @@
                     to find the catalog data.
 
     Returns
     -------
     SkyCatalog
     '''
     # Get LSST bandpasses in case we need to compute fluxes
-    load_lsst_bandpasses()
+    band_passes = load_lsst_bandpasses()
     with open(config_file) as f:
         return SkyCatalog(yaml.safe_load(f), skycatalog_root=skycatalog_root,
                           mp=mp, verbose=verbose)
 
 if __name__ == '__main__':
     import time
-    ###cfg_file_name = 'latest.yaml'
-    cfg_file_name = 'future_latest.yaml'
-    skycatalog_root = os.path.join(os.getenv('SCRATCH'),'desc/skycatalogs')
-
+    cfg_file_name = 'skyCatalog.yaml'
+    ###skycatalog_root = os.path.join(os.getenv('SCRATCH'),'desc/skycatalogs')
+    skycatalog_root = os.getenv('SKYCATALOG_ROOT')
+    catalog_dir = 'reorg'
     if len(sys.argv) > 1:
-        cfg_file_name = sys.argv[1]
-    cfg_file = os.path.join('/global/homes/j/jrbogart/desc_git/skyCatalogs/cfg',
-                            cfg_file_name)
+        catalog_dir = sys.argv[1]
+    if len(sys.argv) > 2:
+        cfg_file_name = sys.argv[2]
+
+    cfg_file = os.path.join(skycatalog_root, catalog_dir, cfg_file_name)
 
     write_sed = False
-    if len(sys.argv) > 2:
+    if len(sys.argv) > 3:
         write_sed = True
 
     # For tract 3828
     #   55.73604 < ra < 57.563452
     #  -37.19001 < dec < -35.702481
 
 
@@ -657,31 +624,39 @@
     print("For region ", rgn)
     print("intersecting pixels are ", intersect_hps)
 
     intersect_poly_hps = _get_intersecting_hps('ring', 32, rgn_poly)
     print("For region ", rgn_poly)
     print("intersecting pixels are ", intersect_poly_hps)
 
+    at_slac = os.getenv('HOME').startswith('/sdf/home/')
+    if not at_slac:
+        obj_types = {'star', 'galaxy', 'sncosmo'}
+    else:
+        obj_types = {'star', 'galaxy', 'sncosmo', 'gaia_star'}
 
-    print('Invoke get_objects_by_region with box region')
+    print('Invoke get_objects_by_region with box region, no gaia')
     t0 = time.time()
-    object_list = cat.get_objects_by_region(rgn)
+    object_list = cat.get_objects_by_region(rgn,
+                                            obj_type_set={'star','galaxy',
+                                                          'sncosmo'})
     t_done = time.time()
     print('Took ', t_done - t0)
                                             ##### temporary obj_type_set={'galaxy', 'star'} )
     #                                        obj_type_set=set(['galaxy']) )
     # Try out get_objects_by_hp with no region
     #colls = cat.get_objects_by_hp(9812, None, set(['galaxy']) )
 
     print('Number of collections returned for box:  ', object_list.collection_count)
     print('Object count for box: ', len(object_list))
 
     print('Invoke get_objects_by_region with polygonal region')
     t0 = time.time()
-    object_list_poly = cat.get_objects_by_region(rgn_poly)
+    object_list_poly = cat.get_objects_by_region(rgn_poly,
+                                                 obj_type_set=obj_types)
     t_done = time.time()
     print('Took ', t_done - t0)
 
     print('Number of collections returned for polygon:  ',
           object_list_poly.collection_count)
     assert(object_list.collection_count == object_list_poly.collection_count)
     print('Object count for polygon: ', len(object_list_poly))
@@ -699,84 +674,95 @@
 
     intersect_diamond_hps = _get_intersecting_hps('ring', 32, rgn_diamond)
     print("for diamond region ", rgn_diamond)
     print("intersecting pixels are ", intersect_diamond_hps)
 
     print('Invoke get_objects_by_region with diamond region')
     t0 = time.time()
-    object_list_diamond = cat.get_objects_by_region(rgn_diamond)
+    object_list_diamond = cat.get_objects_by_region(rgn_diamond,
+                                                    obj_type_set=obj_types)
     t_done = time.time()
     print('Took ', t_done - t0)
 
     print('Number of collections returned for diamond:  ',
           object_list_diamond.collection_count)
     print('Object count for diamond: ', len(object_list_diamond))
 
 
     #### TEMP FOR DEBUGGING
     ### exit(0)
 
+    # For now SIMS_SED_LIBRARY_DIR is undefined at SLAC, making it impossible
+    # to get SEDs for stars. So (crudely) determine whether or not
+    # we're running at SLAC
 
     colls = object_list.get_collections()
     got_a_sed = False
     for c in colls:
         n_obj = len(c)
         print("For hpid ", c.get_partition_id(), "found ", n_obj, " objects")
+        if (n_obj) < 1:
+            continue
         print("First object: ")
         print(c[0], '\nid=', c[0].id, ' ra=', c[0].ra, ' dec=', c[0].dec,
               ' belongs_index=', c[0]._belongs_index,
               ' object_type: ', c[0].object_type )
 
+        if (n_obj < 3):
+            continue
         print("Slice [1:3]")
         slice13 = c[1:3]
         for o in slice13:
             print('id=',o.id, ' ra=',o.ra, ' dec=',o.dec, ' belongs_index=',
                   o._belongs_index,  ' object_type: ', o.object_type)
             print(o.object_type)
             if o.object_type == 'star':
+                if not at_slac:
+                    print(o.get_instcat_entry())
+                    sed, magnorm = o._get_sed()
+                    print('For star magnorm: ', magnorm)
+                    if magnorm < 1000:
+                        print('Length of sed: ', len(sed.wave_list))
+            elif o.object_type == 'sncosmo':
                 print(o.get_instcat_entry())
-                #(lmbda, f_lambda, magnorm) = o.get_sed(resolution=1.0)
-                sed, magnorm = o.get_sed(resolution=1.0)
-                print('For star magnorm: ', magnorm)
-                if magnorm < 1000:
-                    print('Length of sed: ', len(sed.wave_list))
-            else:
+            elif o.object_type == 'galaxy':
                 for cmp in ['disk', 'bulge', 'knots']:
                     print(cmp)
                     if cmp in o.subcomponents:
-                        print(o.get_instcat_entry(component=cmp))
-                        sed, _ = o.get_sed(cmp)
+                        # broken for galaxies currently
+                        ###print(o.get_instcat_entry(component=cmp))
+                        sed, _ = o._get_sed(cmp)
                         if sed:
                             print('Length of sed table: ', len(sed.wave_list))
                             if not got_a_sed:
                                 got_a_sed = True
                                 th = o.get_native_attribute(f'sed_val_{cmp}')
                                 print('Tophat values: ', th)
-                                sed, _ = o.get_sed(component=cmp)
+                                sed, _ = o._get_sed(component=cmp)
                                 print('Simple sed wavelengths:')
                                 print(sed.wave_list)
                                 print('Simple sed values:')
                                 print([sed(w) for w in sed.wave_list])
                                 if write_sed:
                                     o.write_sed('simple_sed.txt', component=cmp)
-                                sed_fine, _ = o.get_sed(component=cmp,
+                                sed_fine, _ = o._get_sed(component=cmp,
                                                         resolution=1.0)
                                 print('Bin width = 1 nm')
                                 print('Initial wl values', sed_fine.wave_list[:20])
                                 print('Start at bin 100', sed_fine.wave_list[100:120])
                                 print('Initial values')
                                 print([sed_fine(w) for w in sed_fine.wave_list[:20]])
                                 print('Start at bin 100')
                                 print([sed_fine(w) for w in sed_fine.wave_list[100:120]])
                         else:
                             print('All-zero sed')
 
                 # Try out old wrapper functions
                 print("\nget_dust:")
-                i_av, i_rv, g_av, g_rv = o.get_dust()
+                i_av, i_rv, g_av, g_rv = o._get_dust()
                 print(f'i_av={i_av} i_rv={i_rv} g_av={g_av} g_rv={g_rv}')
                 print("\nget_wl_params")
                 g1, g2, mu = o.get_wl_params()
                 print(f'g1={g1} g2={g2} mu={mu}')
                 print("\nget_gsobject_components. Keys of returned dict:")
                 gs_dict = o.get_gsobject_components()
                 print(gs_dict.keys())
@@ -800,14 +786,18 @@
             print('\nobjects indexed 163994 through 163996')
             for o in slice_late:
                 print('id=',o.id, ' ra=',o.ra, ' dec=',o.dec, ' belongs_index=',
                       o._belongs_index)
 
     print('Total object count: ', len(object_list))
 
+    if len(object_list) == 0:
+        print('Empty object list. All done')
+        exit(0)
+
     obj = object_list[0]
     print("Type of element in object_list:", type(obj))
 
     if object_list[0].object_type == 'galaxy':
         redshift0 = object_list[0].get_native_attribute('redshift')
         print('First redshift: ', redshift0)
 
@@ -820,19 +810,26 @@
             print("obj id: ", obj.id)
         if sum > 7220:
             break
 
     print(f'Object list len:  {len(object_list)}')
     print(f'Objects found with "in":  {sum}')
 
+    if len(object_list) < 5:
+        print('Very short object list (< 5 elements).  done')
+        exit(0)
+
     segment = object_list[2:5]
     print('Information for slice 2:5 ')
     for o in segment:
         print(f'object {o.id} of type {o.object_type} belongs to collection {o._belongs_to}')
 
+    if len(object_list) < 304:
+        print('Object list len < 304.  All done')
+        exit(0)
     print('\nInformation for slice 285:300')
     segment = object_list[285:300]
     for o in segment:
         print(f'object {o.id} of type {o.object_type} belongs to collection {o._belongs_to}')
 
     #ixes = ([3,5,8],)
     ixes = (np.array([3,5,8, 300, 303]),)
@@ -841,7 +838,9 @@
         print(o.id)
     print(f'\nObjects in slice [3:9]')
     for o in object_list[3:9]:
         print(o.id)
     print(f'\nObjects in slice [300:304]')
     for o in object_list[300:304]:
         print(o.id)
+
+    print('all done')
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/SED_parquet.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/SED_parquet.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/common_utils.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/config_utils.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,49 +96,55 @@
         return self._cfg['SED_models'][modelname]
 
     def object_is_composite(self, objectname):
         return 'composite' in self._cfg['object_types'][objectname]
 
     def get_object_parent(self, objectname):
         if 'parent' in self._cfg['object_types'][objectname]:
-            return self._cfg['object_type'][objectname]['parent']
+            return self._cfg['object_types'][objectname]['parent']
         else:
             return None
 
     def get_object_sedmodel(self, objectname):
         if 'sed_model' in self._cfg['object_types'][objectname]:
-            return self._cfg['object_type'][objectname]['sed_model']
+            return self._cfg['object_types'][objectname]['sed_model']
         else:
             return None
 
     def get_tophat_parameters(self):
         '''
         Return list of named tuples
         Should maybe be part of Sky Catalogs API
         '''
+        if not self.get_config_value('SED_models/tophat', silent=True):
+            return None
         raw_bins = self._cfg['SED_models']['tophat']['bins']
 
         return [ Tophat(b[0], b[1]) for b in raw_bins]
 
-    def get_config_value(self, key_path):
+    def get_config_value(self, key_path, silent=False):
         '''
         Find value belonging to key in a config.
         Parameters
         ----------
         key_path    string   of form 'a/b/c/../q' where all but last
                              component must be a dict
+        silent      boolean  If False (default) complain when key is not
+                             found.  Else return None
 
         Returns
         -------
         Value associated with key_path if config contains such a path
         '''
         path_items = key_path.split('/')
         d = self._cfg
         for i in path_items[:-1]:
             if not i in d:
+                if silent:
+                    return None
                 raise ValueError(f'Item {i} not found')
             d = d[i]
             if not isinstance(d, dict):
                 raise ValueError(f'intermediate {d} is not a dict')
         return d[path_items[-1]]
 
     def validate(self, schema=None):
@@ -312,15 +318,15 @@
                 'inputs' : inputs}
     else:
         return{'versioning' : version_d, 'skyCatalogs_repo' : git_d}
 
 # In config just keep track of models by object type. Information
 # about the parameters they require is internal to the code.
 _AGN_MODELS = ['agn_random_walk']
-_SN_MODELS = ['sn_salt2_extended']
+_SNCOSMO_MODELS = ['sn_salt2_extended']
 
 def assemble_variability_models(object_types):
     '''
     Add information about all known variability models for supplied object
     types.
     Parameters
     ----------
@@ -332,11 +338,11 @@
     keys = model name and values defining struct of parameters for that
     model, e.g. ordered dict with parameter names for keys and parameter
     data types for values
     '''
     models = dict()
     if 'agn' in object_types:
         models['agn'] = _AGN_MODELS
-    if 'sn' in object_types:
-        models['sn'] = _SN_MODELS
+    if 'sncosmo' in object_types:
+        models['sncosmo'] = _SNCOSMO_MODELS
 
     return models
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/exceptions.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/make_fake.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/make_fake.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/parquet_schema_utils.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/parquet_schema_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyarrow as pa
 import logging
 
 __all__ = ['make_galaxy_schema', 'make_galaxy_flux_schema',
-           'make_star_schema', 'make_pointsource_schema']
+           'make_pointsource_schema', 'make_star_flux_schema']
 
 # This schema is not the same as the one taken from the data,
 # probably because of the indexing in the schema derived from a pandas df.
 def make_galaxy_schema(logname, sed_subdir=False, knots=True):
     fields = [pa.field('galaxy_id', pa.int64()),
               pa.field('ra', pa.float64() , True),
 ##                       metadata={"units" : "radians"}),
@@ -73,33 +73,14 @@
               pa.field('lsst_flux_g', pa.float32() , True),
               pa.field('lsst_flux_r', pa.float32() , True),
               pa.field('lsst_flux_i', pa.float32() , True),
               pa.field('lsst_flux_z', pa.float32() , True),
               pa.field('lsst_flux_y', pa.float32() , True)]
     return pa.schema(fields)
 
-def make_star_schema():
-    '''
-    Minimal schema for non-variable stars.  For variables will need to add fields
-    to express variability.   Will also likely have to make changes to accomodate SNe.
-    If AGN also go in this file will need to include gamma1, gamma2, kappa.
-    Could add field for galactic extinction model, but currently it's always 'CCM'
-    so will put it in config.
-    '''
-    fields = [pa.field('object_type', pa.string(), False),
-              pa.field('id', pa.int64(), False),
-              pa.field('ra', pa.float64(), False),
-              pa.field('dec', pa.float64(), False),
-              pa.field('host_galaxy_id', pa.int64(), True),
-              pa.field('magnorm', pa.float64(), True),
-              pa.field('sed_filepath', pa.string(), True),
-              pa.field('MW_rv', pa.float32(), True),
-              pa.field('MW_av', pa.float32(), True)]
-    return pa.schema(fields)
-
 def make_star_flux_schema(logname):
     '''
     Will make a separate parquet file with lsst flux for each band
     and id for joining with the main star file
     '''
     logger = logging.getLogger(logname)
     logger.debug('Creating star flux schema')
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/sed_tools.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/sed_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,76 +4,75 @@
 from astropy.cosmology import FlatLambdaCDM
 import astropy.constants
 import h5py
 import pandas as pd
 
 import numpy as np
 import numpy.ma as ma
-from numpy.random import default_rng
 from dust_extinction.parameter_averages import F19
 import galsim
 
-__all__ = ['ObservedSedFactory', 'MilkyWayExtinction', 'AB_mag',
-           'get_star_sed_path']
-class ObservedSedFactory:
+__all__ = ['TophatSedFactory', 'MilkyWayExtinction', 'get_star_sed_path']
+class TophatSedFactory:
+    '''
+    Used for modeling cosmoDC2 galaxy SEDs, which are represented with
+    a small number of wide bins
+    '''
     _clight = astropy.constants.c.to('m/s').value
     # Conversion factor below of cosmoDC2 tophat Lnu values to W/Hz comes from
     # https://github.com/LSSTDESC/gcr-catalogs/blob/master/GCRCatalogs/SCHEMA.md
     _to_W_per_Hz = 4.4659e13
 
     def __init__(self, th_definition, cosmology, delta_wl=0.001):
         # Get wavelength and frequency bin boundaries.
-        bins = th_definition
-        wl0 = [_[0] for _ in bins]
-
-        # Find index of original bin which includes 500 nm == 5000 ang
-        ix = -1
-        for w in wl0:
-            if w > 5000:
-                break
-            ix += 1
-
-        self._ix_500nm = ix
-
-        wl0.append(bins[-1][0] + bins[-1][1])
-
-        wl0 = 0.1*np.array(wl0)
-        self.wl = np.array(wl0)
-        self.nu = self._clight/(self.wl*1e-9)  # frequency in Hz
+        if th_definition:
+            bins = th_definition
+            wl0 = [_[0] for _ in bins]
+
+            # Find index of original bin which includes 500 nm == 5000 ang
+            ix = -1
+            for w in wl0:
+                if w > 5000:
+                    break
+                ix += 1
+
+            self._ix_500nm = ix
+
+            wl0.append(bins[-1][0] + bins[-1][1])
+
+            wl0 = 0.1*np.array(wl0)
+            self.wl = np.array(wl0)
+            self.nu = self._clight/(self.wl*1e-9)  # frequency in Hz
+
+            # Also save version of wl where vertical rise is replaced by
+            # steep slope
+            wl_deltas = []
+            for i in range(len(bins)):
+                wl_deltas.extend((self.wl[i], self.wl[i+1] - delta_wl))
+
+            # Prepend more bins which will have 0 value
+            n_bins = int(wl0[0]) - 1
+            pre_wl = [float(i) for i in range(n_bins)]
 
-        # Also save version of wl where vertical rise is replaced by
-        # steep slope
-        wl_deltas = []
-        for i in range(len(bins)):
-            wl_deltas.extend((self.wl[i], self.wl[i+1] - delta_wl))
+            wl_deltas = np.insert(wl_deltas, 0, pre_wl)
 
-        # Prepend more bins which will have 0 value
-        n_bins = int(wl0[0]) - 1
-        pre_wl = [float(i) for i in range(n_bins)]
+            # Also make a matching array of 0 values
+            self.pre_val = [0.0 for i in range(n_bins)]
 
-        wl_deltas = np.insert(wl_deltas, 0, pre_wl)
-
-        # Also make a matching array of 0 values
-        self.pre_val = [0.0 for i in range(n_bins)]
-
-        self._wl_deltas = wl_deltas
-        self._wl_deltas_u_nm = wl_deltas*u.nm
+            self._wl_deltas = wl_deltas
+            self._wl_deltas_u_nm = wl_deltas*u.nm
 
         # Create a FlatLambdaCDM cosmology from a dictionary of input
         # parameters.  This code is based on/borrowed from
         # https://github.com/LSSTDESC/gcr-catalogs/blob/master/GCRCatalogs/cosmodc2.py#L128
         cosmo_astropy_allowed = FlatLambdaCDM.__init__.__code__.co_varnames[1:]
-        ##cosmo_astropy = {k: v for k, v in config['Cosmology'].items()
-        ##                 if k in cosmo_astropy_allowed}
         cosmo_astropy = {k: v for k, v in cosmology.items()
                          if k in cosmo_astropy_allowed}
         self.cosmology = FlatLambdaCDM(**cosmo_astropy)
 
-        self.sims_sed_library_dir = os.getenv('SIMS_SED_LIBRARY_DIR')
-
     # Useful for getting magnorm from f_nu values
     @property
     def ix_500nm(self):
         return self._ix_500nm
 
     @property
     def wl_deltas(self):
@@ -126,76 +125,57 @@
 
         # Create the SED object and apply redshift.
         sed = galsim.SED(lut, wave_type='nm', flux_type='flambda')\
                     .atRedshift(redshift)
 
         return sed
 
-    def create_pointsource(self, rel_path, redshift=0):
-        '''
-        Return a galsim SED from information in a file
-        '''
-        fpath = os.path.join(self.sims_sed_library_dir, rel_path)
-
-        sed = galsim.SED(fpath, wave_type='nm', flux_type='flambda')
-        if redshift > 0:
-            sed = sed.atRedshift(redshift)
-        return sed
-
     def magnorm(self, tophat_values, z_H):
         one_Jy = 1e-26  # W/Hz/m**2
         Lnu = tophat_values[self.ix_500nm]*self._to_W_per_Hz  # convert to W/Hz
         Fnu = Lnu/4/np.pi/self.dl(z_H)**2
         with np.errstate(divide='ignore', invalid='ignore'):
             return -2.5*np.log10(Fnu/one_Jy) + 8.90
 
 class MilkyWayExtinction:
     '''
     Applies extinction to a SED
     '''
-    def __init__(self, sed_factory, ext_bin_width=0.1, mwRv=3.1):
-        '''
-        sed_factory         instance of ObservedSedFactory
-
-        '''
-
-        # Save bins to be used for extinction. F19x_range is in units of
-        # 1/micron so convert.
-        wl_ext_min = 1e3/F19.x_range[1]
-        wl_ext_max = 1e3/F19.x_range[0]
-        wl_extinct = np.linspace(wl_ext_min, wl_ext_max,
-                                 int((wl_ext_max - wl_ext_min)/ext_bin_width))
-        self.wl_extinct = wl_extinct
-        self.wl_extinct_nm = wl_extinct*u.nm
+    def __init__(self, delta_wl=0.1, mwRv=3.1, eps=1e-7):
+        """
+        Parameters
+        ----------
+        sed_factory: (remove)
+        ext_bin_width: (rename to delta_wl?)
+        delta_wl : float [0.1]
+            Wavelength sampling of the extinction function in nm
+        mwRv : float [3.1]
+            Parameter describing the shape of the Milky Way extinction
+            curve.
+        eps : float [1e-7]
+            Small numerical offset to avoid out-of-range errors in
+            the wavelength array passed to the dust_extinction code.
+        """
+        # Wavelength sampling for the extinction function. F19.x_range
+        # is in units of 1/micron so convert to nm.  The eps value
+        # is needed to avoid numerical noise at the end points causing
+        # out of range errors detected by the dust_extinction code.
+        wl_min = 1e3/F19.x_range[1] + eps
+        wl_max = 1e3/F19.x_range[0] - eps
+        npts = int((wl_max - wl_min)/delta_wl)
+        self.wls = np.linspace(wl_min, wl_max, npts)
         self.extinction = F19(Rv=mwRv)
 
-        my_wl = sed_factory.wl_deltas
-        my_wl = my_wl[np.where((wl_ext_min < my_wl) & (my_wl < wl_ext_max))]
-        self.wl_deltas = my_wl
-        self.wl_deltas_u = my_wl*u.nm
-
     def extinguish(self, sed, mwAv):
-        ext = self.extinction.extinguish(self.wl_deltas_u, Av=mwAv)
-        spec = galsim.LookupTable(self.wl_deltas, ext, interpolant='linear')
-        mw_ext = galsim.SED(spec, wave_type='nm', flux_type='1')
+        ext = self.extinction.extinguish(self.wls*u.nm, Av=mwAv)
+        lut = galsim.LookupTable(self.wls, ext, interpolant='linear')
+        mw_ext = galsim.SED(lut, wave_type='nm', flux_type='1')
         sed = sed*mw_ext
-
         return sed
 
-class AB_mag:
-    """
-    Convert flux to AB magnitude for a set of bandpasses.
-    """
-    def __init__(self, bps):
-        ab_sed = galsim.SED(lambda nu : 10**(8.90/2.5 - 23), wave_type='nm',
-                            flux_type='fnu')
-        self.ab_fluxes = {band: ab_sed.calculateFlux(bp) for
-                          band, bp in bps.items()}
-    def __call__(self, flux, band):
-        return -2.5*np.log10(flux/self.ab_fluxes[band])
 
 _standard_dict = {'lte' : 'starSED/phoSimMLT',
                   'bergeron' : 'starSED/wDs',
                   'km|kp' : 'starSED/kurucz'}
 
 def get_star_sed_path(filename, name_to_folder=_standard_dict):
     '''
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/sn_tools.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/sn_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 from astropy import units as u
 import sncosmo
 import galsim
 
+__all__ = ['SncosmoModel']
 
-class SNObject(sncosmo.Model):
+
+class SncosmoModel(sncosmo.Model):
     def __init__(self, source='salt2-extended', params=None):
         '''
         params - dict of params suitable for the model
 
         See also https://sncosmo.readthedocs.io/en/stable/index.html
 
         '''
```

### Comparing `skyCatalogs-1.4.0rc5/python/desc/skycatalogs/utils/translate_utils.py` & `skyCatalogs-1.5.0rc1/python/desc/skycatalogs/utils/translate_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import numpy as np
 
 __all__ = ['column_finder', 'check_file', 'write_to_instance', 'SourceType',
            'STAR_FMT', 'CMP_FMT',
            'form_star_instance_columns', 'form_cmp_instance_columns']
 
 
-STAR_FMT = '{:s} {:d} {:.14f} {:.14f} {:.8f} {:s} {:d} {:d} {:d} {:d} {:d} {:d} {:s} {:s} {:s} {:.8f} {:f}'
+STAR_FMT = '{:s} {:s} {:.14f} {:.14f} {:.8f} {:s} {:d} {:d} {:d} {:d} {:d} {:d} {:s} {:s} {:s} {:.8f} {:f}'
 
 CMP_FMT = '{:s} {:s} {:.14f} {:.14f} {:.8f} {:s} {:.9g} {:.9g} {:.9g} {:.9g} {:d} {:d} {:s} {:.9g} {:.9g} {:f} {:.0f} {:s} {:s} {:.8f} {:f}'
 
 def form_star_instance_columns(band):
     star_instance = [column_finder('prefix', SourceType.FIXED, ('object', np.dtype('U6'))),
-                     column_finder('uniqueId', SourceType.DATA, 'id'),
+                     #column_finder('uniqueId', SourceType.DATA, 'id'),
+                     column_finder('uniquePsId', SourceType.COMPUTE, ['id']),
                      column_finder('raPhoSim', SourceType.DATA, 'ra'),
                      column_finder('decPhoSim', SourceType.DATA, 'dec'),
                      column_finder('maskedMagNorm', SourceType.DATA, 'magnorm'),
                      column_finder('sedFilepath',SourceType.DATA, 'sed_filepath'),
                      column_finder('redshift', SourceType.FIXED, (0, int)),
                      column_finder('gamma1', SourceType.FIXED, (0, int)),
                      column_finder('gamma2', SourceType.FIXED, (0, int)),
@@ -132,15 +133,15 @@
     '''
     parse columns for this object/component type
     fetch data and config values as needed
     form values into a list.
     '''
     row = []
 
-    if obj.object_type == 'star':
+    if obj.object_type in ['star', 'sncosmo']:
         fmt = STAR_FMT
         columns = form_star_instance_columns(band)
     elif obj.object_type in ['galaxy', 'disk', 'bulge']:
         fmt = CMP_FMT
         if obj.object_type == 'galaxy':
             cmp = component
         else:
@@ -165,21 +166,25 @@
             t = c.source_parm[1]
             if str(t) in ['float', 'int']:
                 q = eval(f'{t}({v})')
             else:
                 q = v
             row.append(q)
         elif c.source_type == SourceType.COMPUTE:
-            # only one is sedFilepath, and only for galaxy components
-            if c.instance_name not in ['sedFilepath', 'uniqueId'] or cmp not in ['disk', 'bulge', 'knots']:
-                raise ValueError(f'translate_utils.form_object_string: Bad COMPUTE entry {c.instance_name} for component {cmp}')
+            if c.instance_name not in ['sedFilepath', 'uniqueId',
+                                       'uniquePsId']:
+                raise ValueError(f'translate_utils.form_object_string: Bad COMPUTE entry {c.instance_name}')
             if c.instance_name == 'sedFilepath':
                 row.append(f'{obj.get_native_attribute("galaxy_id")}_{cmp}_sed.txt')
-            else:     # uniqueId
+            elif c.instance_name == 'uniqueId':
+                if cmp not in ['disk', 'bulge', 'knots']:
+                    raise ValueError(f'translate_utils.form_object_string: Bad COMPUTE entry {c.instance_name} for component {cmp}')
                 row.append(f'{str(obj.get_native_attribute("galaxy_id"))}_{cmp}')
+            else:    #  uniquePsId.  Output must be string but input may be int
+                row.append(f'{str(obj.get_native_attribute("id"))}')
         else:
             raise ValueError(f'translate_utils.form_object_string: Unknown source type {c.source_type}')
 
     return write_to_string(row, fmt)
 
 def write_to_string(row, fmt):
     '''
```

### Comparing `skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/PKG-INFO` & `skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyCatalogs
-Version: 1.4.0rc5
+Version: 1.5.0rc1
 Summary: Writes, reads catalogs input to LSST DESC simulations
 Author-email: Joanne Bogart <jrb@slac.stanford.edu>
 License: Copyright (c) 2018, the skyCatalogs contributors on GitHub, https://github.com/LSSTDESC/skyCatalogs/graphs/contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `skyCatalogs-1.4.0rc5/python/skyCatalogs.egg-info/SOURCES.txt` & `skyCatalogs-1.5.0rc1/python/skyCatalogs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,35 @@
 python/desc/__init__.py
 python/desc/skycatalogs/__init__.py
 python/desc/skycatalogs/_version.py
 python/desc/skycatalogs/catalog_creator.py
 python/desc/skycatalogs/skyCatalogs.py
 python/desc/skycatalogs/objects/__init__.py
 python/desc/skycatalogs/objects/base_object.py
+python/desc/skycatalogs/objects/gaia_object.py
 python/desc/skycatalogs/objects/galaxy_object.py
+python/desc/skycatalogs/objects/sncosmo_object.py
+python/desc/skycatalogs/objects/star_object.py
 python/desc/skycatalogs/readers/__init__.py
 python/desc/skycatalogs/readers/parquet_reader.py
 python/desc/skycatalogs/utils/SED_parquet.py
 python/desc/skycatalogs/utils/__init__.py
+python/desc/skycatalogs/utils/catalog_utils.py
 python/desc/skycatalogs/utils/common_utils.py
 python/desc/skycatalogs/utils/config_utils.py
 python/desc/skycatalogs/utils/exceptions.py
 python/desc/skycatalogs/utils/make_fake.py
 python/desc/skycatalogs/utils/parquet_schema_utils.py
 python/desc/skycatalogs/utils/sed_tools.py
+python/desc/skycatalogs/utils/shapes.py
 python/desc/skycatalogs/utils/sn_tools.py
 python/desc/skycatalogs/utils/translate_utils.py
 python/skyCatalogs.egg-info/PKG-INFO
 python/skyCatalogs.egg-info/SOURCES.txt
 python/skyCatalogs.egg-info/dependency_links.txt
 python/skyCatalogs.egg-info/requires.txt
 python/skyCatalogs.egg-info/top_level.txt
 tests/test_API.py
+tests/test_gaia_objects.py
+tests/test_object_api.py
+tests/test_pointsource.py
 tests/test_skyCatalogs.py
```

### Comparing `skyCatalogs-1.4.0rc5/tests/test_API.py` & `skyCatalogs-1.5.0rc1/tests/test_API.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import time
         cat = self._cat
 
 
         hps = cat._find_all_hps()
         print('Found {} healpix pixels '.format(len(hps)))
         for h in hps: print(h)
-        assert(set(hps) == {9556, 9683, 9684, 9812, 9813, 9940})
+        assert(set(hps) == {9556, 9557, 9683, 9684, 9812, 9813, 9940})
 
         # These hps are the ones covering tract 3828
         # For this tract ra is between 55.736 and 57.564
         # dec is between -37.190 and -35.702
 
         # Catalogs for testing are sparse, so make a large box
         ra_min_small = 55.8
@@ -98,15 +98,15 @@
                 print('id=',o.id, ' ra=',o.ra, ' dec=',o.dec, ' belongs_index=',
                       o._belongs_index)
 
         box_count = len(object_list)
         print('Total object count: ', box_count)
 
         obj = object_list[0]
-        assert(type(obj) == BaseObject)
+        assert(isinstance(obj, BaseObject))
 
         redshift0 = object_list[0].get_native_attribute('redshift')
         print('First redshift: ', redshift0)
 
         sed_bulges = colls[0].get_native_attribute('sed_val_bulge')
 
         # Now make a polygon which describes same region as the box
@@ -193,15 +193,15 @@
             print('id=', c[0].id, ' ra=', c[0].ra, ' dec=', c[0].dec,
                   ' belongs_index=', c[0]._belongs_index, ' object_type=',
                   c[0].object_type)
             fluxes = c[0].get_LSST_fluxes()
             assert(len(fluxes) == 6)
             print('Found fluxes')
 
-            assert(type(c[0]) == BaseObject)
+            assert(isinstance(c[0], BaseObject))
 
 
         print('List len: ', len(object_list))
         print('Sum over collections: ', total_object_count)
         assert(total_object_count == len(object_list))
 
 
@@ -238,20 +238,17 @@
                 else:
                     print(f'No native attribute "{att}" for this object')
         ####   end of included function for printing
 
         hp = 9556
 
         cat = self._cat
-        obj_types = {'galaxy'}
-        specified = cat.get_objects_by_hp(hp, region=None, obj_type_set=obj_types)
-        print_from_objects(f'From hp {hp} with object types {str(obj_types)}', specified)
-
-        none_specified = cat.get_objects_by_hp(hp)
-        print_from_objects(f'From hp {hp}, no specified object types', none_specified)
+        obj_type = 'galaxy'
+        specified = cat.get_object_type_by_hp(hp, obj_type, region=None)
+        print_from_objects(f'From hp {hp} with object types {obj_type}', specified)
     def testAPI_rowgroup(self):
         '''
         Compare results of get_objects_by_region when skyCatalog files
         each have a single row group or have several
         '''
         def compare_objects(no_rg, has_rg):
             no_rg_coll = no_rg.get_collections()
```

### Comparing `skyCatalogs-1.4.0rc5/tests/test_skyCatalogs.py` & `skyCatalogs-1.5.0rc1/tests/test_skyCatalogs.py`

 * *Files identical despite different names*

