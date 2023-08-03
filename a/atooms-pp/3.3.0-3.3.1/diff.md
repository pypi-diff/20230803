# Comparing `tmp/atooms-pp-3.3.0.tar.gz` & `tmp/atooms-pp-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms-pp-3.3.0.tar", last modified: Thu Aug  3 14:37:31 2023, max compression
+gzip compressed data, was "atooms-pp-3.3.1.tar", last modified: Thu Aug  3 17:23:34 2023, max compression
```

## Comparing `atooms-pp-3.3.0.tar` & `atooms-pp-3.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.3.0/LICENSE
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.3.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.564976 atooms-pp-3.3.0/atooms/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.3.0/atooms/__init__.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/atooms/postprocessing/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      705 2023-08-03 14:31:56.000000 atooms-pp-3.3.0/atooms/postprocessing/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.3.0/atooms/postprocessing/_commit.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-08-03 14:37:30.000000 atooms-pp-3.3.0/atooms/postprocessing/_version.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/alpha2.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15526 2023-08-03 14:32:24.000000 atooms-pp-3.3.0/atooms/postprocessing/api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.3.0/atooms/postprocessing/ba.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.3.0/atooms/postprocessing/chi4t.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.3.0/atooms/postprocessing/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.3.0/atooms/postprocessing/correlation.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/filter.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/fkt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.3.0/atooms/postprocessing/fourierspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15322 2023-08-03 14:31:23.000000 atooms-pp-3.3.0/atooms/postprocessing/fourierspace.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13996 2023-07-01 09:58:27.000000 atooms-pp-3.3.0/atooms/postprocessing/gr.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.3.0/atooms/postprocessing/ik.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/linkedcells.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/msd.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.3.0/atooms/postprocessing/partial.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/progress.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/qt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.3.0/atooms/postprocessing/realspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.3.0/atooms/postprocessing/s4kt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/sacf.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     9955 2023-08-03 14:25:52.000000 atooms-pp-3.3.0/atooms/postprocessing/sk.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/susceptibility.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.3.0/atooms/postprocessing/vacf.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/atooms_pp.egg-info/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-08-03 14:37:31.000000 atooms-pp-3.3.0/atooms_pp.egg-info/top_level.txt
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/bin/
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.3.0/bin/acf.py
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.3.0/bin/pp.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-08-03 14:37:31.568976 atooms-pp-3.3.0/setup.cfg
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.3.0/setup.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.3.1/LICENSE
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.3.1/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.203422 atooms-pp-3.3.1/atooms/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.3.1/atooms/__init__.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/atooms/postprocessing/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      705 2023-08-03 14:31:56.000000 atooms-pp-3.3.1/atooms/postprocessing/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.3.1/atooms/postprocessing/_commit.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-08-03 17:23:32.000000 atooms-pp-3.3.1/atooms/postprocessing/_version.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/alpha2.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15568 2023-08-03 17:17:23.000000 atooms-pp-3.3.1/atooms/postprocessing/api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.3.1/atooms/postprocessing/ba.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.3.1/atooms/postprocessing/chi4t.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.3.1/atooms/postprocessing/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.3.1/atooms/postprocessing/correlation.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/filter.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/fkt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.3.1/atooms/postprocessing/fourierspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15946 2023-08-03 17:10:40.000000 atooms-pp-3.3.1/atooms/postprocessing/fourierspace.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13996 2023-07-01 09:58:27.000000 atooms-pp-3.3.1/atooms/postprocessing/gr.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.3.1/atooms/postprocessing/ik.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/linkedcells.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/msd.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.3.1/atooms/postprocessing/partial.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/progress.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/qt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.3.1/atooms/postprocessing/realspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/s4kt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/sacf.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9945 2023-08-03 15:53:28.000000 atooms-pp-3.3.1/atooms/postprocessing/sk.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/susceptibility.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/vacf.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/atooms_pp.egg-info/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/top_level.txt
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/bin/
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.3.1/bin/acf.py
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.3.1/bin/pp.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/setup.cfg
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.3.1/setup.py
```

### Comparing `atooms-pp-3.3.0/LICENSE` & `atooms-pp-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/PKG-INFO` & `atooms-pp-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.3.0
+Version: 3.3.1
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atooms-pp-3.3.0/README.md` & `atooms-pp-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/__init__.py` & `atooms-pp-3.3.1/atooms/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/alpha2.py` & `atooms-pp-3.3.1/atooms/postprocessing/alpha2.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/api.py` & `atooms-pp-3.3.1/atooms/postprocessing/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,16 +101,17 @@
     if global_args['fast']:
         backend = pp.StructureFactorFast
     else:
         backend = pp.StructureFactorLegacy
     if kgrid is not None:
         kgrid = [float(_) for _ in kgrid.split(',')]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
-        fourier_grid = pp.FourierSpaceGrid(th, kgrid, kmin=kmin,
-                                        kmax=kmax, nk=nk, dk=dk, ksamples=ksamples)
+        fourier_grid = pp.FourierSpaceGrid(kgrid, kmin=kmin,
+                                           kmax=kmax, nk=nk, dk=dk,
+                                           ksamples=ksamples)
         cf = backend(th, kgrid=kgrid, norigins=global_args['norigins'])
         if global_args['filter'] is not None:
             cf = pp.Filter(cf, global_args['filter'])
         if weight_trajectory is not None:
             weight_trajectory = TrajectoryXYZ(weight_trajectory)
         cf.add_weight(trajectory=weight_trajectory,
                       field=weight,
```

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/ba.py` & `atooms-pp-3.3.1/atooms/postprocessing/ba.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/chi4t.py` & `atooms-pp-3.3.1/atooms/postprocessing/chi4t.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/core.py` & `atooms-pp-3.3.1/atooms/postprocessing/core.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/correlation.py` & `atooms-pp-3.3.1/atooms/postprocessing/correlation.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/filter.py` & `atooms-pp-3.3.1/atooms/postprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/fkt.py` & `atooms-pp-3.3.1/atooms/postprocessing/fkt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/fourierspace.f90` & `atooms-pp-3.3.1/atooms/postprocessing/fourierspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/fourierspace.py` & `atooms-pp-3.3.1/atooms/postprocessing/fourierspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,49 +128,61 @@
         self.normalize = normalize
         
         # Find grid of k-vector norms and store it sorted as self.kgrid
         # We first try with self.grid
         variables = self.short_name.split('(')[1][:-1]
         variables = variables.split(',')
         if len(variables) > 1:
-            self.kgrid = self.grid[variables.index('k')]
+            kgrid = self.grid[variables.index('k')]
         else:
-            self.kgrid = self.grid
+            kgrid = self.grid
 
         # Define k-vectors
-        if isinstance(self.kgrid, FourierSpaceGrid):
+        if isinstance(kgrid, FourierSpaceGrid):
             # We keep the FourierSpaceGrid instance as a private variable
-            self._kgrid = self.kgrid
+            self._kgrid = kgrid
         else:
             # The user has not provided a FourierSpaceGrid: we construct it internally
             # from the other input arguments
-            self._kgrid = FourierSpaceGrid(trajectory, kgrid=self.kgrid, nk=nk,
+            self._kgrid = FourierSpaceGrid(kgrid=kgrid, nk=nk,
                                            dk=dk, kmin=kmin, kmax=kmax,
                                            ksamples=ksamples)
-            
-        # Wrap around these variables, which are now handled by FourierSpaceGrid
-        # Smallest k-vector compatible with the boundary conditions
-        self.k0 = self._kgrid.k0
-        # This is the actual grid of k-vector norms
-        self.kgrid = self._kgrid.kgrid
-        # Private variables, used by subclasses
-        self._kvectors = self._kgrid._kvectors
-        self._koffset = self._kgrid._koffset
-            
+
     def compute(self):
+        self._kgrid.setup(self.trajectory[0].cell.side)
         super(FourierSpaceCorrelation, self).compute()
 
+    # Wrap attributes of FourierSpaceGrid to keep compatibility with previous code
+    @property
+    def k0(self):
+        """Smallest k-vector compatible with the boundary conditions"""
+        return self._kgrid.k0
+
+    @property
+    def kgrid(self):
+        """Actual grid of k-vector norms"""
+        return self._kgrid.kgrid
+
     @property
     def kvectors(self):
         return self._kgrid.kvectors
-
+    
     @kvectors.setter
     def kvectors(self, kvectors):
         raise AttributeError('cannot set kvectors, pass them to the constructor')
+    
+    # Private properties, used by subclasses
+    @property
+    def _kvectors(self):
+        return self._kgrid._kvectors
 
+    @property
+    def _koffset(self):
+        return self._kgrid._koffset
+    
     def report(self, verbose=False):
         return self._kgrid.report(verbose=verbose)
     
 
 class FourierSpaceGrid:
 
     """
@@ -186,16 +198,16 @@
     their norm (k_x^2+k_y^2+k_z^2)^{1/2} lies within `dk` of the
     prescribed value k_i.
 
     See the doc of `Correlation` for information about the rest of the
     instance variables.
     """
 
-    def __init__(self, trajectory, kgrid=None, nk=8,
-                 dk=0.1, kmin=-1, kmax=10, ksamples=20, sample=-1, kvectors=None):
+    def __init__(self, kgrid=None, nk=8, dk=0.1, kmin=-1, kmax=10,
+                 ksamples=20, kvectors=None):
         """
         Possible inputs:
 
         1. kgrid is None:
 
         the k grid is determined internally from kmin, kmax, ksamples
         and the kvectors are sampled using nk and dk parameters
@@ -233,53 +245,66 @@
           where offset_j is the absolute value of the minimum of the
           whole set of (jx, jy, jz). This way we are sure that indices
           start from 1. This is necessary with numpy arrays, for which
           negative indices have a different meaning.
 
         - _koffset: value of offset_j defined above
         """
-        # Some additional variables. k0 = smallest wave vectors
+        self.kgrid = kgrid
+        self.nk = nk
+        self.dk = dk
+        self.kmin = kmin
+        self.kmax = kmax
+        self.ksamples = ksamples
+        self.kvectors_input = kvectors
+        self.k0 = []
+        
+        # Some internal variables
         # compatible with the boundary conditions
         self._kvectors = []
         self._koffset = 0
+
+    # TODO: by adding setup() when can postpone grid setup. This way we need not compute the grid too early and we can more easily respect the update argument of do().
+    # TODO: we actually need only the cell here! Not the trajectory.
+    def setup(self, side):
         # Smallest kvector
-        self.k0 = 2*math.pi / trajectory[max(sample, 0)].cell.side
+        self.k0 = 2*math.pi / side
         
         # Setup the grid of wave-vectors
-        if kvectors is not None:
-            self._kvectors, self._koffset = self._setup_from_kvectors(kvectors, self.k0)
+        if self.kvectors_input is not None:
+            self._kvectors, self._koffset = self._setup_from_kvectors(self.kvectors_input, self.k0)
         else:
             # If kgrid of kvectors are not provided, setup a linear grid from kmin,kmax,ksamples data
             # TODO: This shouldnt be allowed with fluctuating cells
             # Or we should fix the smallest k to some average of smallest k per sample
-            if kgrid is None:
-                if kmin > 0:
-                    kgrid = linear_grid(kmin, kmax, ksamples)
+            if self.kgrid is None:
+                if self.kmin > 0:
+                    self.kgrid = linear_grid(self.kmin, self.kmax, self.ksamples)
                 else:
-                    kgrid = linear_grid(min(self.k0), kmax, ksamples)
+                    self.kgrid = linear_grid(min(self.k0), self.kmax, self.ksamples)
             else:
                 # Sort, since code below depends on kgrid[0] being the smallest k-value.
-                kgrid.sort()
+                self.kgrid.sort()
                 # If the first wave-vector is negative we replace it by k0
-                if kgrid[0] < 0.0:
-                    kgrid[0] = min(self.k0)
+                if self.kgrid[0] < 0.0:
+                    self.kgrid[0] = min(self.k0)
 
             # Now find the wave-vectors
-            self._kvectors, self._koffset = self._setup_grid_sphere(len(kgrid) * [dk],
-                                                                    kgrid, self.k0)
+            self._kvectors, self._koffset = self._setup_grid_sphere(len(self.kgrid) * [self.dk],
+                                                                    self.kgrid, self.k0)
             # Decimate them.
             # Setting the seed here once so as to get the same set
             # independent of filters.
             # TODO: use a local random instance here
             random.seed(1)
             # Pick up a random, unique set of nk vectors out ot the avilable ones
             # without exceeding maximum number of vectors in shell nkmax
             # self.kgrid, self.selection = self._decimate_k()
             for i, klist in enumerate(self._kvectors):
-                self._kvectors[i] = random.sample(klist, min(nk, len(klist)))
+                self._kvectors[i] = random.sample(klist, min(self.nk, len(klist)))
 
         # Define the actual kgrid now
         self.kgrid = []
         for klist in self._kvectors:
             knorm = numpy.mean([_k_norm(kvec, self.k0, self._koffset) for kvec in klist])
             self.kgrid.append(knorm)
```

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/gr.py` & `atooms-pp-3.3.1/atooms/postprocessing/gr.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/helpers.py` & `atooms-pp-3.3.1/atooms/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/ik.py` & `atooms-pp-3.3.1/atooms/postprocessing/ik.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/linkedcells.py` & `atooms-pp-3.3.1/atooms/postprocessing/linkedcells.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/msd.py` & `atooms-pp-3.3.1/atooms/postprocessing/msd.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/partial.py` & `atooms-pp-3.3.1/atooms/postprocessing/partial.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/progress.py` & `atooms-pp-3.3.1/atooms/postprocessing/progress.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/qt.py` & `atooms-pp-3.3.1/atooms/postprocessing/qt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/realspace.f90` & `atooms-pp-3.3.1/atooms/postprocessing/realspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/s4kt.py` & `atooms-pp-3.3.1/atooms/postprocessing/s4kt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/sacf.py` & `atooms-pp-3.3.1/atooms/postprocessing/sacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/sk.py` & `atooms-pp-3.3.1/atooms/postprocessing/sk.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         rho_0_av = [complex(0., 0.) for k in kgrid]
         rho_1_av = [complex(0., 0.) for k in kgrid]
         rho2_av = [complex(0., 0.) for k in kgrid]
         variable_cell = is_cell_variable(self.trajectory)
         for i in progress(range(0, nsteps, self.skip), total=nsteps // self.skip):
             # If cell changes we have to update the wave vectors
             if variable_cell:
-                raise ValueError('cannot handle sk with fluctuating cell')
-
+                self._kgrid.setup(self.trajectory[i].cell.side)
+            
             # Tabulate exponentials
             # Note: tabulating and computing takes about the same time
             if self._pos_0[i] is self._pos_1[i]:
                 # Identical species
                 expo_0 = expo_sphere(self.k0, self._koffset, self._pos_0[i])
                 expo_1 = expo_0
             else:
@@ -191,15 +191,15 @@
         cnt = [0 for k in kgrid]
         rho_av = [complex(0., 0.) for k in kgrid]
         rho2_av = [complex(0., 0.) for k in kgrid]
         variable_cell = is_cell_variable(self.trajectory)
         for i in range(0, nsteps, self.skip):
             # If cell changes we have to update the wave vectors
             if variable_cell:
-                raise ValueError('cannot handle sk with fluctuating cell')
+                self._kgrid.setup(self.trajectory[i].cell.side)
 
             # Tabulate exponentials
             # Note: tabulating and computing takes about the same time
             if self._pos_0[i] is self._pos_1[i]:
                 # Identical species
                 expo_0 = expo_sphere(self.k0, self._koffset, self._pos_0[i])
                 expo_1 = expo_0
```

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/susceptibility.py` & `atooms-pp-3.3.1/atooms/postprocessing/susceptibility.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms/postprocessing/vacf.py` & `atooms-pp-3.3.1/atooms/postprocessing/vacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/atooms_pp.egg-info/PKG-INFO` & `atooms-pp-3.3.1/atooms_pp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.3.0
+Version: 3.3.1
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atooms-pp-3.3.0/atooms_pp.egg-info/SOURCES.txt` & `atooms-pp-3.3.1/atooms_pp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/bin/acf.py` & `atooms-pp-3.3.1/bin/acf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/bin/pp.py` & `atooms-pp-3.3.1/bin/pp.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.0/setup.py` & `atooms-pp-3.3.1/setup.py`

 * *Files identical despite different names*

