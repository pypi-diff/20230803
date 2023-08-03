# Comparing `tmp/spin_phonon_suite-1.3.0.tar.gz` & `tmp/spin_phonon_suite-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-1.3.0.tar", last modified: Tue Aug  1 12:59:22 2023, max compression
+gzip compressed data, was "spin_phonon_suite-1.3.1.tar", last modified: Thu Aug  3 15:10:27 2023, max compression
```

## Comparing `spin_phonon_suite-1.3.0.tar` & `spin_phonon_suite-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:59:22.185824 spin_phonon_suite-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3750 2023-08-01 12:59:22.185824 spin_phonon_suite-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 12:59:22.185824 spin_phonon_suite-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-08-01 12:59:19.000000 spin_phonon_suite-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:59:22.183990 spin_phonon_suite-1.3.0/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 12:59:19.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10806 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/cells.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)    22303 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    18786 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:59:22.184907 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3750 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      159 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:10:27.725875 spin_phonon_suite-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-08-03 15:10:27.725875 spin_phonon_suite-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 15:10:27.725875 spin_phonon_suite-1.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-08-03 15:10:24.000000 spin_phonon_suite-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:10:27.723875 spin_phonon_suite-1.3.1/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-03 15:10:24.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10806 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/cells.py
+-rw-rw-rw-   0 root         (0) root         (0)    34974 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)    22303 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18786 2023-08-03 15:09:47.000000 spin_phonon_suite-1.3.1/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:10:27.725875 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-08-03 15:10:27.000000 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-03 15:10:27.000000 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:10:27.000000 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-03 15:10:27.000000 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      159 2023-08-03 15:10:27.000000 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 15:10:27.000000 spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-1.3.0/LICENSE` & `spin_phonon_suite-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.3.0/PKG-INFO` & `spin_phonon_suite-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-1.3.0/README.md` & `spin_phonon_suite-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.3.0/setup.py` & `spin_phonon_suite-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
```

### Comparing `spin_phonon_suite-1.3.0/spin_phonon_suite/cells.py` & `spin_phonon_suite-1.3.1/spin_phonon_suite/cells.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.3.0/spin_phonon_suite/cli.py` & `spin_phonon_suite-1.3.1/spin_phonon_suite/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         ho = Harmonic.from_phonopy_hdf5(
             args.poscar,
             args.phonopy_hdf5,
             trans=args.trans,
             distortion_expansion=args.distortion_expansion,
             distortion_expansion_old=args.distortion_expansion_old,
             distortion_cutoff=args.distortion_cutoff,
-            central_index=args.central_index
+            central_idc=args.central_index
         )
 
     if args.active_atoms is not None:
         idc = [idx - 1 for idc in args.active_atoms for idx in idc]
         ho = ho.subset_atoms(active_atom_idc=idc)
 
     elif args.ref_coordinates is not None:
```

### Comparing `spin_phonon_suite-1.3.0/spin_phonon_suite/derivative.py` & `spin_phonon_suite-1.3.1/spin_phonon_suite/derivative.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.3.0/spin_phonon_suite/lvc.py` & `spin_phonon_suite-1.3.1/spin_phonon_suite/lvc.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.3.0/spin_phonon_suite/vibrations.py` & `spin_phonon_suite-1.3.1/spin_phonon_suite/vibrations.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-1.3.1/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-phonon-suite
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

