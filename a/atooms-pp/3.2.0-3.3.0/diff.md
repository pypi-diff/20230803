# Comparing `tmp/atooms-pp-3.2.0.tar.gz` & `tmp/atooms-pp-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms-pp-3.2.0.tar", last modified: Sat Jul  1 07:37:40 2023, max compression
+gzip compressed data, was "atooms-pp-3.3.0.tar", last modified: Thu Aug  3 14:37:31 2023, max compression
```

## Comparing `atooms-pp-3.2.0.tar` & `atooms-pp-3.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.2.0/LICENSE
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.2.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.472302 atooms-pp-3.2.0/atooms/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.2.0/atooms/__init__.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.480302 atooms-pp-3.2.0/atooms/postprocessing/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      662 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.2.0/atooms/postprocessing/_commit.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-07-01 07:37:38.000000 atooms-pp-3.2.0/atooms/postprocessing/_version.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/alpha2.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15572 2022-10-13 10:18:27.000000 atooms-pp-3.2.0/atooms/postprocessing/api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.2.0/atooms/postprocessing/ba.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.2.0/atooms/postprocessing/chi4t.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.2.0/atooms/postprocessing/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.2.0/atooms/postprocessing/correlation.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/filter.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/fkt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.2.0/atooms/postprocessing/fourierspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13938 2023-04-15 13:28:00.000000 atooms-pp-3.2.0/atooms/postprocessing/fourierspace.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13913 2023-06-30 17:00:38.000000 atooms-pp-3.2.0/atooms/postprocessing/gr.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.2.0/atooms/postprocessing/ik.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/linkedcells.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/msd.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.2.0/atooms/postprocessing/partial.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/progress.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/qt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.2.0/atooms/postprocessing/realspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/s4kt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/sacf.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     9867 2022-10-13 10:49:58.000000 atooms-pp-3.2.0/atooms/postprocessing/sk.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/susceptibility.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/vacf.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/atooms_pp.egg-info/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/top_level.txt
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/bin/
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.2.0/bin/acf.py
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.2.0/bin/pp.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/setup.cfg
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.2.0/setup.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.3.0/LICENSE
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.3.0/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.564976 atooms-pp-3.3.0/atooms/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.3.0/atooms/__init__.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/atooms/postprocessing/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      705 2023-08-03 14:31:56.000000 atooms-pp-3.3.0/atooms/postprocessing/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.3.0/atooms/postprocessing/_commit.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-08-03 14:37:30.000000 atooms-pp-3.3.0/atooms/postprocessing/_version.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/alpha2.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15526 2023-08-03 14:32:24.000000 atooms-pp-3.3.0/atooms/postprocessing/api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.3.0/atooms/postprocessing/ba.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.3.0/atooms/postprocessing/chi4t.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.3.0/atooms/postprocessing/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.3.0/atooms/postprocessing/correlation.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/filter.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/fkt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.3.0/atooms/postprocessing/fourierspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15322 2023-08-03 14:31:23.000000 atooms-pp-3.3.0/atooms/postprocessing/fourierspace.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13996 2023-07-01 09:58:27.000000 atooms-pp-3.3.0/atooms/postprocessing/gr.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.3.0/atooms/postprocessing/ik.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/linkedcells.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/msd.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.3.0/atooms/postprocessing/partial.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/progress.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/qt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.3.0/atooms/postprocessing/realspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/s4kt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/sacf.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9955 2023-08-03 14:25:52.000000 atooms-pp-3.3.0/atooms/postprocessing/sk.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/susceptibility.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/vacf.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/atooms_pp.egg-info/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/top_level.txt
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/bin/
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.3.0/bin/acf.py
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.3.0/bin/pp.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/setup.cfg
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.3.0/setup.py
```

### Comparing `atooms-pp-3.2.0/LICENSE` & `atooms-pp-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/PKG-INFO` & `atooms-pp-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.2.0
+Version: 3.3.0
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atooms-pp-3.2.0/README.md` & `atooms-pp-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/__init__.py` & `atooms-pp-3.3.0/atooms/postprocessing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 from .correlation import *
 from .partial import *
 from .filter import Filter
 from .susceptibility import Susceptibility
+from .fourierspace import FourierSpaceGrid
 
 # Real space correlation functions
 from .alpha2 import *
 from .chi4t import *
 from .gr import *
 from .msd import *
 from .qt import *
```

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/alpha2.py` & `atooms-pp-3.3.0/atooms/postprocessing/alpha2.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/api.py` & `atooms-pp-3.3.0/atooms/postprocessing/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,32 +101,30 @@
     if global_args['fast']:
         backend = pp.StructureFactorFast
     else:
         backend = pp.StructureFactorLegacy
     if kgrid is not None:
         kgrid = [float(_) for _ in kgrid.split(',')]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
-        cf = backend(th, kgrid=kgrid,
-                     norigins=global_args['norigins'], kmin=kmin,
-                     kmax=kmax, nk=nk, dk=dk, ksamples=ksamples)
+        fourier_grid = pp.FourierSpaceGrid(th, kgrid, kmin=kmin,
+                                        kmax=kmax, nk=nk, dk=dk, ksamples=ksamples)
+        cf = backend(th, kgrid=kgrid, norigins=global_args['norigins'])
         if global_args['filter'] is not None:
             cf = pp.Filter(cf, global_args['filter'])
         if weight_trajectory is not None:
             weight_trajectory = TrajectoryXYZ(weight_trajectory)
         cf.add_weight(trajectory=weight_trajectory,
                       field=weight,
                       fluctuations=weight_fluctuations)
         cf.do(update=global_args['update'])
 
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
-            cf = Partial(backend, ids, th, kgrid=kgrid,
-                         norigins=global_args['norigins'],
-                         kmin=kmin, kmax=kmax, nk=nk, dk=dk,
-                         ksamples=ksamples)
+            cf = Partial(backend, ids, th, kgrid=fourier_grid,
+                         norigins=global_args['norigins'])
             cf.add_weight(trajectory=weight_trajectory,
                           field=weight,
                           fluctuations=weight_fluctuations)
             cf.do(update=global_args['update'])
 
 def ik(input_file, trajectory_radius=None, nk=20, dk=0.1, kmin=-1.0,
        kmax=15.0, kgrid=None, ksamples=30, *input_files,
```

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/ba.py` & `atooms-pp-3.3.0/atooms/postprocessing/ba.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/chi4t.py` & `atooms-pp-3.3.0/atooms/postprocessing/chi4t.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/core.py` & `atooms-pp-3.3.0/atooms/postprocessing/core.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/correlation.py` & `atooms-pp-3.3.0/atooms/postprocessing/correlation.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/filter.py` & `atooms-pp-3.3.0/atooms/postprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/fkt.py` & `atooms-pp-3.3.0/atooms/postprocessing/fkt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/fourierspace.f90` & `atooms-pp-3.3.0/atooms/postprocessing/fourierspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/fourierspace.py` & `atooms-pp-3.3.0/atooms/postprocessing/fourierspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from collections import defaultdict
 
 import numpy
 
 from .helpers import linear_grid
 from .correlation import Correlation
 
-__all__ = ['expo_sphere', 'expo_sphere_safe', 'FourierSpaceCorrelation']
+__all__ = ['expo_sphere', 'expo_sphere_safe', 'FourierSpaceCorrelation', 'FourierSpaceGrid']
 
 _log = logging.getLogger(__name__)
 
 
 def expo_sphere(k0, nk_max, pos):
     """Returns the exponentials of the input positions for each k."""
 
@@ -115,15 +115,87 @@
     prescribed value k_i.
 
     See the doc of `Correlation` for information about the rest of the
     instance variables.
     """
 
     def __init__(self, trajectory, grid, norigins=None, nk=8, dk=0.1,
-                 kmin=-1, kmax=10, ksamples=20, fix_cm=False, normalize=True):
+                 kmin=-1, kmax=10, ksamples=20, fix_cm=False,
+                 normalize=True):
+        super(FourierSpaceCorrelation, self).__init__(trajectory,
+                                                      grid, norigins=norigins,
+                                                      fix_cm=fix_cm)
+        # Some additional variables. 
+        self.normalize = normalize
+        
+        # Find grid of k-vector norms and store it sorted as self.kgrid
+        # We first try with self.grid
+        variables = self.short_name.split('(')[1][:-1]
+        variables = variables.split(',')
+        if len(variables) > 1:
+            self.kgrid = self.grid[variables.index('k')]
+        else:
+            self.kgrid = self.grid
+
+        # Define k-vectors
+        if isinstance(self.kgrid, FourierSpaceGrid):
+            # We keep the FourierSpaceGrid instance as a private variable
+            self._kgrid = self.kgrid
+        else:
+            # The user has not provided a FourierSpaceGrid: we construct it internally
+            # from the other input arguments
+            self._kgrid = FourierSpaceGrid(trajectory, kgrid=self.kgrid, nk=nk,
+                                           dk=dk, kmin=kmin, kmax=kmax,
+                                           ksamples=ksamples)
+            
+        # Wrap around these variables, which are now handled by FourierSpaceGrid
+        # Smallest k-vector compatible with the boundary conditions
+        self.k0 = self._kgrid.k0
+        # This is the actual grid of k-vector norms
+        self.kgrid = self._kgrid.kgrid
+        # Private variables, used by subclasses
+        self._kvectors = self._kgrid._kvectors
+        self._koffset = self._kgrid._koffset
+            
+    def compute(self):
+        super(FourierSpaceCorrelation, self).compute()
+
+    @property
+    def kvectors(self):
+        return self._kgrid.kvectors
+
+    @kvectors.setter
+    def kvectors(self, kvectors):
+        raise AttributeError('cannot set kvectors, pass them to the constructor')
+
+    def report(self, verbose=False):
+        return self._kgrid.report(verbose=verbose)
+    
+
+class FourierSpaceGrid:
+
+    """
+    Grid of vectors in Fourier space.
+
+    The correlation function is computed for each of the scalar values
+    k_i of the provided `kgrid`. If the latter is `None`, the grid is
+    built using `ksamples` entries linearly spaced between `kmin` and
+    `kmax`.
+
+    For each sample k_i in `kgrid`, the correlation function is
+    computed over at most `nk` wave-vectors (k_x, k_y, k_z) such that
+    their norm (k_x^2+k_y^2+k_z^2)^{1/2} lies within `dk` of the
+    prescribed value k_i.
+
+    See the doc of `Correlation` for information about the rest of the
+    instance variables.
+    """
+
+    def __init__(self, trajectory, kgrid=None, nk=8,
+                 dk=0.1, kmin=-1, kmax=10, ksamples=20, sample=-1, kvectors=None):
         """
         Possible inputs:
 
         1. kgrid is None:
 
         the k grid is determined internally from kmin, kmax, ksamples
         and the kvectors are sampled using nk and dk parameters
@@ -161,87 +233,59 @@
           where offset_j is the absolute value of the minimum of the
           whole set of (jx, jy, jz). This way we are sure that indices
           start from 1. This is necessary with numpy arrays, for which
           negative indices have a different meaning.
 
         - _koffset: value of offset_j defined above
         """
-        super(FourierSpaceCorrelation, self).__init__(trajectory,
-                                                      grid, norigins=norigins, fix_cm=fix_cm)
         # Some additional variables. k0 = smallest wave vectors
         # compatible with the boundary conditions
-        self.normalize = normalize
-        self.nk = nk
-        self.dk = dk
-        self.kmin = kmin
-        self.kmax = kmax
-        self.ksamples = ksamples
-        self.kgrid = None
-        self.k0 = []
         self._kvectors = []
         self._koffset = 0
-
-    def compute(self):
-        # Setup grid once. If cell changes we'll call it again
-        self._setup()
-        # Now compute
-        super(FourierSpaceCorrelation, self).compute()
-
-    def _setup(self, sample=0):
-        # We skip setup if the kgrid is already set up and we are not
-        # asking to rebuild it (for a sample != 0).
-        # This allows to copy over the kvectors and kgrid
-        if sample == 0 and self.kgrid is not None:
-            return
-
-        # We subclass compute to define k grid at compute time
-        # Find k-norms grid and store it a self.kgrid (the norms are sorted)
-        variables = self.short_name.split('(')[1][:-1]
-        variables = variables.split(',')
-        if len(variables) > 1:
-            self.kgrid = self.grid[variables.index('k')]
-        else:
-            self.kgrid = self.grid
-
         # Smallest kvector
-        self.k0 = 2*math.pi/self.trajectory[sample].cell.side
-        # If grid is not provided, setup a linear grid from kmin,kmax,ksamples data
-        # TODO: This shouldnt be allowed with fluctuating cells
-        # Or we should fix the smallest k to some average of smallest k per sample
-        if self.kgrid is None:
-            if self.kmin > 0:
-                self.kgrid = linear_grid(self.kmin, self.kmax, self.ksamples)
-            else:
-                self.kgrid = linear_grid(min(self.k0), self.kmax, self.ksamples)
-        else:
-            # Sort, since code below depends on kgrid[0] being the smallest k-value.
-            self.kgrid.sort()
-            # If the first wave-vector is negative we replace it by k0
-            if self.kgrid[0] < 0.0:
-                self.kgrid[0] = min(self.k0)
-
+        self.k0 = 2*math.pi / trajectory[max(sample, 0)].cell.side
+        
         # Setup the grid of wave-vectors
-        self._kvectors, self._koffset = self._setup_grid_sphere(len(self.kgrid) * [self.dk],
-                                                                self.kgrid, self.k0)
+        if kvectors is not None:
+            self._kvectors, self._koffset = self._setup_from_kvectors(kvectors, self.k0)
+        else:
+            # If kgrid of kvectors are not provided, setup a linear grid from kmin,kmax,ksamples data
+            # TODO: This shouldnt be allowed with fluctuating cells
+            # Or we should fix the smallest k to some average of smallest k per sample
+            if kgrid is None:
+                if kmin > 0:
+                    kgrid = linear_grid(kmin, kmax, ksamples)
+                else:
+                    kgrid = linear_grid(min(self.k0), kmax, ksamples)
+            else:
+                # Sort, since code below depends on kgrid[0] being the smallest k-value.
+                kgrid.sort()
+                # If the first wave-vector is negative we replace it by k0
+                if kgrid[0] < 0.0:
+                    kgrid[0] = min(self.k0)
+
+            # Now find the wave-vectors
+            self._kvectors, self._koffset = self._setup_grid_sphere(len(kgrid) * [dk],
+                                                                    kgrid, self.k0)
+            # Decimate them.
+            # Setting the seed here once so as to get the same set
+            # independent of filters.
+            # TODO: use a local random instance here
+            random.seed(1)
+            # Pick up a random, unique set of nk vectors out ot the avilable ones
+            # without exceeding maximum number of vectors in shell nkmax
+            # self.kgrid, self.selection = self._decimate_k()
+            for i, klist in enumerate(self._kvectors):
+                self._kvectors[i] = random.sample(klist, min(nk, len(klist)))
 
-        # Decimate
-        # Setting the seed here once so as to get the same set
-        # independent of filters.
-        random.seed(1)
-        # Pick up a random, unique set of nk vectors out ot the avilable ones
-        # without exceeding maximum number of vectors in shell nkmax
-        # self.kgrid, self.selection = self._decimate_k()
-        for i, klist in enumerate(self._kvectors):
-            nk = min(self.nk, len(klist))
-            self._kvectors[i] = random.sample(klist, nk)
-
-        # Define the grid using the actual kvectors
-        # average k norms appear after decimation.
-        for i, klist in enumerate(self._kvectors):
-            self.kgrid[i] = numpy.mean([_k_norm(kvec, self.k0, self._koffset) for kvec in klist])
+        # Define the actual kgrid now
+        self.kgrid = []
+        for klist in self._kvectors:
+            knorm = numpy.mean([_k_norm(kvec, self.k0, self._koffset) for kvec in klist])
+            self.kgrid.append(knorm)
 
     @staticmethod
     def _setup_grid_sphere(dk, kgrid, k0):
         """
         Setup wave vector grid with spherical average (no symmetry),
         picking up vectors that fit into shells of width `dk` centered around
         the values specified in the input list `kgrid`.
@@ -251,16 +295,16 @@
         _log.info('setting up the wave-vector grid')
         kvec = [[] for _ in range(len(kgrid))]  # defaultdict(list)
 
         # With elongated box, we choose the smallest k0 component to
         # setup the integer grid. This must be consistent with
         # expo_grid() otherwise it wont find the vectors
         kmax = kgrid[-1] + dk[-1]
-        kbin_max = 1 + int(kmax / min(k0))
         kmax_sq = kmax**2
+        kbin_max = 1 + int(kmax / min(k0))
 
         # Choose iterator of spatial grid
         ndims = len(k0)
         if ndims == 3:
             _iterator = _sphere
         elif ndims == 2:
             _iterator = _disk
@@ -287,80 +331,68 @@
         all_good = True
         for i in range(len(kvec)):
             if len(kvec[i]) == 0:
                 dk[i] *= 1.2
                 _log.info('increasing kbin {} to {}'.format(i, dk[i]))
                 all_good = False
         if not all_good:
-            return FourierSpaceCorrelation._setup_grid_sphere(dk, kgrid, k0)
+            return FourierSpaceGrid._setup_grid_sphere(dk, kgrid, k0)
         else:
             return kvec, kbin_max
 
-    @property
-    def kvectors(self):
-        # Return actual kvectors
-        kvectors = []
-        for k, klist in enumerate(self._kvectors):
-            kvectors.append([])
-            for kvec in klist:
-                actual_vec = self.k0 * (numpy.array(kvec) - self._koffset)
-                kvectors[-1].append(list(actual_vec))
-        return kvectors
-
-    @kvectors.setter
-    def kvectors(self, kvectors):
-        # Smallest kvector
-        sample = 0
-        self.k0 = 2*math.pi/self.trajectory[sample].cell.side
-
+    @staticmethod
+    def _setup_from_kvectors(kvectors, k0):
         # Collect kvectors and compute shift
-        self._kvectors = []
+        _kvectors = []
         shift = 0
         for klist in kvectors:
-            self._kvectors.append([])
+            _kvectors.append([])
             for kvec in klist:
-                rounded = numpy.rint(kvec / self.k0)
-                self._kvectors[-1].append(numpy.array(rounded, dtype=int))
+                rounded = numpy.rint(kvec / k0)
+                _kvectors[-1].append(numpy.array(rounded, dtype=int))
                 # Update shift
                 shift = min(shift, int(min(rounded)))
 
         # Shift to make all array indices start from 0
-        self._koffset = int(abs(shift)) + 1
-        for klist in self._kvectors:
+        _koffset = int(abs(shift)) + 1
+        for klist in _kvectors:
             for i in range(len(klist)):
-                klist[i] = tuple(klist[i] + self._koffset)
+                klist[i] = tuple(klist[i] + _koffset)
 
-        # Define kgrid
-        self.kgrid = []
-        for klist in self._kvectors:
-            knorm = numpy.mean([_k_norm(kvec, self.k0, self._koffset) for kvec in klist])
-            self.kgrid.append(knorm)
+        return _kvectors, _koffset
 
+    @property
+    def kvectors(self):
+        # Return actual kvectors
+        kvectors = []
+        for k, klist in enumerate(self._kvectors):
+            kvectors.append([])
+            for kvec in klist:
+                actual_vec = self.k0 * (numpy.array(kvec) - self._koffset)
+                kvectors[-1].append(list(actual_vec))
+        return kvectors
+            
     def report(self, verbose=False):
         """
         Return a formatted report of the wave-vector grid used to compute
         the correlation function
 
         The `verbose` option turns on writing of the individuals
         wavectors (also accessible via the `kvectors` property).
         """
         txt = '# k-point, average, std, vectors in shell\n'
         for i, klist in enumerate(self.kvectors):
-            knorms = []
-            for kvec in klist:
-                k_sq = numpy.dot(kvec, kvec)
-                knorms.append(math.sqrt(k_sq))
-            knorms = numpy.array(knorms)
+            knorms = numpy.array([numpy.dot(kvec, kvec)**0.5 for kvec in klist])
             txt += "{} {:f} {:f} {}\n".format(self.kgrid[i], knorms.mean(),
-                                              knorms.std(),
-                                              len(klist))
+                                              knorms.std(), len(klist))
         if verbose:
             txt += '\n# k-point, k-vector\n'
             for i, klist in enumerate(self.kvectors):
                 for kvec in klist:
                     # Reformat numpy array
                     as_str = str(kvec)
                     as_str = as_str.replace(',', '')
                     as_str = as_str.replace('[', '')
                     as_str = as_str.replace(']', '')
                     txt += '{} {}\n'.format(self.kgrid[i], as_str)
         return txt
+
```

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/gr.py` & `atooms-pp-3.3.0/atooms/postprocessing/gr.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,15 @@
                     'partly periodic cells are not supported yet'
                 for i in range(len(side)):
                     if not system.cell.periodic[i]:
                         side[i] = sys.float_info.max
             else:
                 # If the system does not have a cell, wrap it in an
                 # infinite cell. This way we can still use PBC in f90 kernels
+                # Note that normalization is taken care of by system.density below
                 side = sys.float_info.max * numpy.ones(ndims, dtype=float)
 
             # Store number of particles for normalization
             N_0.append(pos_0.shape[0])
             if distinct:
                 N_1.append(pos_1.shape[0])
             else:
```

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/helpers.py` & `atooms-pp-3.3.0/atooms/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/ik.py` & `atooms-pp-3.3.0/atooms/postprocessing/ik.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/linkedcells.py` & `atooms-pp-3.3.0/atooms/postprocessing/linkedcells.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/msd.py` & `atooms-pp-3.3.0/atooms/postprocessing/msd.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/partial.py` & `atooms-pp-3.3.0/atooms/postprocessing/partial.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/progress.py` & `atooms-pp-3.3.0/atooms/postprocessing/progress.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/qt.py` & `atooms-pp-3.3.0/atooms/postprocessing/qt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/realspace.f90` & `atooms-pp-3.3.0/atooms/postprocessing/realspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/s4kt.py` & `atooms-pp-3.3.0/atooms/postprocessing/s4kt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/sacf.py` & `atooms-pp-3.3.0/atooms/postprocessing/sacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/sk.py` & `atooms-pp-3.3.0/atooms/postprocessing/sk.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         rho_0_av = [complex(0., 0.) for k in kgrid]
         rho_1_av = [complex(0., 0.) for k in kgrid]
         rho2_av = [complex(0., 0.) for k in kgrid]
         variable_cell = is_cell_variable(self.trajectory)
         for i in progress(range(0, nsteps, self.skip), total=nsteps // self.skip):
             # If cell changes we have to update the wave vectors
             if variable_cell:
-                self._setup(i)
+                raise ValueError('cannot handle sk with fluctuating cell')
 
             # Tabulate exponentials
             # Note: tabulating and computing takes about the same time
             if self._pos_0[i] is self._pos_1[i]:
                 # Identical species
                 expo_0 = expo_sphere(self.k0, self._koffset, self._pos_0[i])
                 expo_1 = expo_0
@@ -191,15 +191,15 @@
         cnt = [0 for k in kgrid]
         rho_av = [complex(0., 0.) for k in kgrid]
         rho2_av = [complex(0., 0.) for k in kgrid]
         variable_cell = is_cell_variable(self.trajectory)
         for i in range(0, nsteps, self.skip):
             # If cell changes we have to update the wave vectors
             if variable_cell:
-                self._setup(i)
+                raise ValueError('cannot handle sk with fluctuating cell')
 
             # Tabulate exponentials
             # Note: tabulating and computing takes about the same time
             if self._pos_0[i] is self._pos_1[i]:
                 # Identical species
                 expo_0 = expo_sphere(self.k0, self._koffset, self._pos_0[i])
                 expo_1 = expo_0
```

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/susceptibility.py` & `atooms-pp-3.3.0/atooms/postprocessing/susceptibility.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms/postprocessing/vacf.py` & `atooms-pp-3.3.0/atooms/postprocessing/vacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/atooms_pp.egg-info/PKG-INFO` & `atooms-pp-3.3.0/atooms_pp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.2.0
+Version: 3.3.0
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atooms-pp-3.2.0/atooms_pp.egg-info/SOURCES.txt` & `atooms-pp-3.3.0/atooms_pp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/bin/acf.py` & `atooms-pp-3.3.0/bin/acf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/bin/pp.py` & `atooms-pp-3.3.0/bin/pp.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.2.0/setup.py` & `atooms-pp-3.3.0/setup.py`

 * *Files identical despite different names*

